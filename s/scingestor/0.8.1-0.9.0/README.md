# Comparing `tmp/scingestor-0.8.1.tar.gz` & `tmp/scingestor-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scingestor-0.8.1.tar", last modified: Wed Nov  8 10:49:10 2023, max compression
+gzip compressed data, was "scingestor-0.9.0.tar", last modified: Tue Nov 28 15:48:54 2023, max compression
```

## Comparing `scingestor-0.8.1.tar` & `scingestor-0.9.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-11-08 10:49:10.089059 scingestor-0.8.1/
--rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2023-10-27 08:49:07.000000 scingestor-0.8.1/COPYRIGHT
--rw-r--r--   0 jkotan   (15949) irc         (39)      350 2023-10-27 08:49:07.000000 scingestor-0.8.1/MANIFEST.in
--rw-r--r--   0 jkotan   (15949) irc         (39)    12867 2023-11-08 10:49:10.089059 scingestor-0.8.1/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)    10173 2023-10-27 08:49:07.000000 scingestor-0.8.1/README.md
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-11-08 10:49:10.085059 scingestor-0.8.1/config/
--rw-r--r--   0 jkotan   (15949) irc         (39)      657 2023-10-27 08:49:07.000000 scingestor-0.8.1/config/default_template.yaml
--rwxr-xr-x   0 jkotan   (15949) irc         (39)      921 2023-10-27 08:49:07.000000 scingestor-0.8.1/config/format_default.sh
--rw-r--r--   0 jkotan   (15949) irc         (39)      274 2023-10-27 08:49:07.000000 scingestor-0.8.1/config/scingestor.service
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-11-08 10:49:10.085059 scingestor-0.8.1/doc/
--rw-r--r--   0 jkotan   (15949) irc         (39)     4449 2023-10-27 08:49:07.000000 scingestor-0.8.1/doc/conf.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    11181 2023-10-27 08:49:07.000000 scingestor-0.8.1/doc/index.rst
--rw-r--r--   0 jkotan   (15949) irc         (39)      743 2023-10-27 08:49:07.000000 scingestor-0.8.1/doc/scicat_dataset_ingest.rst
--rw-r--r--   0 jkotan   (15949) irc         (39)      857 2023-10-27 08:49:07.000000 scingestor-0.8.1/doc/scicat_dataset_ingestor.rst
--rw-r--r--   0 jkotan   (15949) irc         (39)      966 2023-10-27 08:49:07.000000 scingestor-0.8.1/doc/scicat_ingest.rst
--rw-r--r--   0 jkotan   (15949) irc         (39)     1777 2023-10-27 08:49:07.000000 scingestor-0.8.1/doc/scingestor.rst
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-11-08 10:49:10.085059 scingestor-0.8.1/man/
--rw-r--r--   0 jkotan   (15949) irc         (39)     1777 2023-10-27 08:49:07.000000 scingestor-0.8.1/man/scicat_dataset_ingest.1
--rw-r--r--   0 jkotan   (15949) irc         (39)     1880 2023-10-27 08:49:07.000000 scingestor-0.8.1/man/scicat_dataset_ingestor.1
--rw-r--r--   0 jkotan   (15949) irc         (39)     2031 2023-10-27 08:49:07.000000 scingestor-0.8.1/man/scicat_ingest.1
--rw-r--r--   0 jkotan   (15949) irc         (39)    28455 2023-10-27 08:49:07.000000 scingestor-0.8.1/man/scingestor.1
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       82 2022-07-12 12:52:58.000000 scingestor-0.8.1/scicat_dataset_ingest
--rwxr-xr-x   0 jkotan   (15949) irc         (39)      459 2022-06-01 08:18:09.000000 scingestor-0.8.1/scicat_dataset_ingestor
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       78 2023-10-27 08:49:07.000000 scingestor-0.8.1/scicat_ingest
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-11-08 10:49:10.089059 scingestor-0.8.1/scingestor/
--rw-r--r--   0 jkotan   (15949) irc         (39)      921 2023-11-08 09:50:23.000000 scingestor-0.8.1/scingestor/__init__.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    30359 2023-10-27 08:49:07.000000 scingestor-0.8.1/scingestor/beamtimeWatcher.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1181 2023-03-17 07:14:51.000000 scingestor-0.8.1/scingestor/configuration.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    12533 2023-10-27 08:49:07.000000 scingestor-0.8.1/scingestor/datasetIngest.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    73286 2023-11-08 09:43:13.000000 scingestor-0.8.1/scingestor/datasetIngestor.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    12425 2023-10-27 08:49:07.000000 scingestor-0.8.1/scingestor/datasetWatcher.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2817 2023-10-27 08:49:07.000000 scingestor-0.8.1/scingestor/logger.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     8009 2023-10-27 08:49:07.000000 scingestor-0.8.1/scingestor/modelIngest.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2931 2023-10-27 08:49:07.000000 scingestor-0.8.1/scingestor/pathConverter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     7955 2023-10-27 08:49:07.000000 scingestor-0.8.1/scingestor/safeINotifier.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    17646 2023-10-27 08:49:07.000000 scingestor-0.8.1/scingestor/scanDirWatcher.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-11-08 10:49:10.089059 scingestor-0.8.1/scingestor.egg-info/
--rw-r--r--   0 jkotan   (15949) irc         (39)    12867 2023-11-08 10:49:10.000000 scingestor-0.8.1/scingestor.egg-info/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)      916 2023-11-08 10:49:10.000000 scingestor-0.8.1/scingestor.egg-info/SOURCES.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-11-08 10:49:10.000000 scingestor-0.8.1/scingestor.egg-info/dependency_links.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2022-06-01 09:19:11.000000 scingestor-0.8.1/scingestor.egg-info/not-zip-safe
--rw-r--r--   0 jkotan   (15949) irc         (39)       50 2023-11-08 10:49:10.000000 scingestor-0.8.1/scingestor.egg-info/requires.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)       11 2023-11-08 10:49:10.000000 scingestor-0.8.1/scingestor.egg-info/top_level.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)      193 2023-11-08 10:49:10.089059 scingestor-0.8.1/setup.cfg
--rw-r--r--   0 jkotan   (15949) irc         (39)     4231 2023-10-27 08:49:07.000000 scingestor-0.8.1/setup.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-11-28 15:48:54.859937 scingestor-0.9.0/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2023-10-27 08:49:07.000000 scingestor-0.9.0/COPYRIGHT
+-rw-r--r--   0 jkotan   (15949) irc         (39)      350 2023-10-27 08:49:07.000000 scingestor-0.9.0/MANIFEST.in
+-rw-r--r--   0 jkotan   (15949) irc         (39)    14088 2023-11-28 15:48:54.859937 scingestor-0.9.0/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11298 2023-11-27 07:33:30.000000 scingestor-0.9.0/README.md
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-11-28 15:48:54.859937 scingestor-0.9.0/config/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      657 2023-10-27 08:49:07.000000 scingestor-0.9.0/config/default_template.yaml
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)      921 2023-10-27 08:49:07.000000 scingestor-0.9.0/config/format_default.sh
+-rw-r--r--   0 jkotan   (15949) irc         (39)      274 2023-10-27 08:49:07.000000 scingestor-0.9.0/config/scingestor.service
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-11-28 15:48:54.859937 scingestor-0.9.0/doc/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4449 2023-10-27 08:49:07.000000 scingestor-0.9.0/doc/conf.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    12328 2023-11-27 07:33:30.000000 scingestor-0.9.0/doc/index.rst
+-rw-r--r--   0 jkotan   (15949) irc         (39)      743 2023-10-27 08:49:07.000000 scingestor-0.9.0/doc/scicat_dataset_ingest.rst
+-rw-r--r--   0 jkotan   (15949) irc         (39)      857 2023-10-27 08:49:07.000000 scingestor-0.9.0/doc/scicat_dataset_ingestor.rst
+-rw-r--r--   0 jkotan   (15949) irc         (39)      966 2023-10-27 08:49:07.000000 scingestor-0.9.0/doc/scicat_ingest.rst
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1777 2023-10-27 08:49:07.000000 scingestor-0.9.0/doc/scingestor.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-11-28 15:48:54.859937 scingestor-0.9.0/man/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1777 2023-11-28 15:48:44.000000 scingestor-0.9.0/man/scicat_dataset_ingest.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1880 2023-11-28 15:48:44.000000 scingestor-0.9.0/man/scicat_dataset_ingestor.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2031 2023-11-28 15:48:44.000000 scingestor-0.9.0/man/scicat_ingest.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)    30825 2023-11-28 15:48:34.000000 scingestor-0.9.0/man/scingestor.1
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       82 2022-07-12 12:52:58.000000 scingestor-0.9.0/scicat_dataset_ingest
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)      459 2022-06-01 08:18:09.000000 scingestor-0.9.0/scicat_dataset_ingestor
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       78 2023-10-27 08:49:07.000000 scingestor-0.9.0/scicat_ingest
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-11-28 15:48:54.859937 scingestor-0.9.0/scingestor/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      921 2023-11-13 12:05:19.000000 scingestor-0.9.0/scingestor/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    30359 2023-10-27 08:49:07.000000 scingestor-0.9.0/scingestor/beamtimeWatcher.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1181 2023-03-17 07:14:51.000000 scingestor-0.9.0/scingestor/configuration.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    12610 2023-11-27 07:33:30.000000 scingestor-0.9.0/scingestor/datasetIngest.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    80852 2023-11-27 07:33:30.000000 scingestor-0.9.0/scingestor/datasetIngestor.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    14317 2023-11-27 07:33:30.000000 scingestor-0.9.0/scingestor/datasetWatcher.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2817 2023-10-27 08:49:07.000000 scingestor-0.9.0/scingestor/logger.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     8009 2023-10-27 08:49:07.000000 scingestor-0.9.0/scingestor/modelIngest.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2931 2023-10-27 08:49:07.000000 scingestor-0.9.0/scingestor/pathConverter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7955 2023-10-27 08:49:07.000000 scingestor-0.9.0/scingestor/safeINotifier.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    17646 2023-10-27 08:49:07.000000 scingestor-0.9.0/scingestor/scanDirWatcher.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-11-28 15:48:54.859937 scingestor-0.9.0/scingestor.egg-info/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    14088 2023-11-28 15:48:54.000000 scingestor-0.9.0/scingestor.egg-info/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)      916 2023-11-28 15:48:54.000000 scingestor-0.9.0/scingestor.egg-info/SOURCES.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-11-28 15:48:54.000000 scingestor-0.9.0/scingestor.egg-info/dependency_links.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2022-06-01 09:19:11.000000 scingestor-0.9.0/scingestor.egg-info/not-zip-safe
+-rw-r--r--   0 jkotan   (15949) irc         (39)       50 2023-11-28 15:48:54.000000 scingestor-0.9.0/scingestor.egg-info/requires.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)       11 2023-11-28 15:48:54.000000 scingestor-0.9.0/scingestor.egg-info/top_level.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)      193 2023-11-28 15:48:54.859937 scingestor-0.9.0/setup.cfg
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4231 2023-11-27 07:33:30.000000 scingestor-0.9.0/setup.py
```

### Comparing `scingestor-0.8.1/COPYRIGHT` & `scingestor-0.9.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `scingestor-0.8.1/PKG-INFO` & `scingestor-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scingestor
-Version: 0.8.1
+Version: 0.9.0
 Summary: Scientific Catalog Tools
 Home-page: http://github.com/jkotan/scingestor
 Author: ('Jan Kotanski',)
 Author-email: jankotan@gmail.com
 Maintainer: Jan Kotanski
 Maintainer-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE, version 3
@@ -43,20 +43,30 @@
         * **attachment_metadata_postfix** *(str)* , default: `".attachment.json"`
         * **metadata_in_var_dir** *(bool)* , default: `False`
         * **use_corepath_as_scandir** *(bool)* , default: `False`
         * **beamtime_filename_postfix** *(str)* , default: `"beamtime-metadata-"`
         * **beamtime_filename_prefix** *(str)* , default: `".json"`
         * **datasets_filename_pattern** *(str)* , default: `"scicat-datasets-{beamtimeid}.lst"`
         * **ingested_datasets_filename_pattern** *(str)* , default: `"scicat-ingested-datasets-{beamtimeid}.lst"`
-        * **file_dataset_metadata_generator** *(str)* , default: `"nxsfileinfo metadata -k4  -o {metapath}/{scanname}{scanpostfix}  -b {beamtimefile} -p {beamtimeid}/{scanname}  -w {ownergroup} -c {accessgroups} {scanpath}/{scanname}.{ext}"`
+        * **file_dataset_metadata_generator** *(str)* , default: `"nxsfileinfo metadata -k4  -o {metapath}/{scanname}{scanpostfix}  -b {beamtimefile} -p {beamtimeid}/{scanname}  -w {ownergroup} -c {accessgroups} {mastefile}"`
         * **dataset_metadata_generator** *(str)* , default: `"nxsfileinfo metadata -k4  -o {metapath}/{scanname}{scanpostfix}  -c {accessgroups} -w {ownergroup} -b {beamtimefile} -p {beamtimeid}/{scanname}"`
         * **datablock_metadata_generator** *(str)* , default: `"nxsfileinfo origdatablock  -s *.pyc,*{datablockpostfix},*{scanpostfix},*~  -p {pidprefix}{beamtimeid}/{scanname}  -w {ownergroup} -c {accessgroups} -o {metapath}/{scanname}{datablockpostfix} "`
         * **datablock_metadata_stream_generator** *(str)* , default: `"nxsfileinfo origdatablock  -s *.pyc,*{datablockpostfix},*{scanpostfix},*~  -w {ownergroup} -c {accessgroups} -p {pidprefix}{beamtimeid}/{scanname} "`
         * **datablock_metadata_generator_scanpath_postfix** *(str)* , default: `" {scanpath}/{scanname} "`
-        * **attachment_metadata_generator** *(str)* , default: `"nxsfileinfo attachment  -w {ownergroup} -c {accessgroups} -o {metapath}/{scanname}{attachmentpostfix} "`
+        * **attachment_metadata_generator** *(str)* , default: `"nxsfileinfo attachment  -w {ownergroup} -c {accessgroups} -o {metapath}/{scanname}{attachmentpostfix} {plotfile} "`
+        * **metadata_generated_callback** *(str)* , default: `"nxsfileinfo groupmetadata  {lastmeasurement} -m {metapath}/{scanname}{scanpostfix} -d {metapath}/{scanname}{datablockpostfix} -a {metapath}/{scanname}{attachmentpostfix} -p {beamtimeid}/{lastmeasurement} -f -k4 "`
+        * **metadata_group_map_file** *(str)* , default: `""`
+        * **raw_metadata_callback** *(bool)* , default: `False`
+        * **skip_multi_datablock_ingestion** *(bool)* , default: `False`
+        * **skip_multi_attachment_ingestion** *(bool)* , default: `False`
+        * **skip_scan_dataset_ingestion** *(bool)* , default: `False`
+        * **call_metadata_generated_callback** *(bool)* , default: `False`
+        * **metadata_group_map_file_generator_switch** *(str)* , default: `" --group-map-file {groupmapfile} "`
+        * **raw_metadata_callback_switch** *(str)* , default: `" --raw "`
+        * **execute_commands** *(bool)* , default: `False`
         * **plot_file_extension_list** *(list\<str\>)* , default: `["png", "nxs", "h5", "ndf", "nx", "fio"]`
         * **master_file_extension_list** *(list\<str\>)* , default: `["nxs", "h5", "ndf", "nx", "fio"]`
         * **chmod_generator_switch** *(str)* , default: `" -x {chmod} "`
         * **relative_path_generator_switch** *(str)* , default: `" -r {relpath} "`
         * **oned_dataset_generator_switch** *(str)* , default: `" --oned "`
         * **max_oned_dataset_generator_switch** *(str)* , default: `" --max-oned-size {maxonedsize} "`
         * **override_attachment_signals_generator_switch** *(bool)* , default: `" --override "`
@@ -103,16 +113,18 @@
         
         ### Pattern keywords for configuration variables
         
         The  **datasets_filename_pattern**, **ingested_datasets_filename_pattern**  and **ingestor_var_dir** can contain the *{beamtimeid}* and *{hostname}* keywords,  e.g. `"scicat-ingested-datasets-{beamtimeid}.lst"` or `"scicat-ingested-datasets-{hostname}-{beamtimeid}.lst"` which is instantiated during the ingestor execution.
         
         The  **beamtime_dirs**, **beamtime_base_dir**, **ingestor_var_dir**, **ingestor_credential_file**, **scandir_blacklist** can contain the *{homepath}* keyword.
         
-        Similarly, **file_dataset_metadata_generator**, **dataset_metadata_generator**, **datablock_metadata_generator**,  **datablock_metadata_stream_generator**, **datablock_metadata_generator_scanpath_postfix**, **attachment_metadata_generator**, **chmod_generator_switch**, **relative_path_generator_switch** can contain the following keywords: *{beamtimeid}* , *{scanname}*, *{chmod}*, *{scanpath}*, *{metapath}*, *{relpath}*, *{beamtimeid}*, *{beamline}*, *{pidprefix}*, *{beamtimefile}*, *{scanpostfix}*, *{datablockpostfix}*, *{ownergroup}*, *{accessgroups}*, *{hostname}*, *{homepath}*, *{hiddenattributes}*, *{ext}*
+        Similarly, **file_dataset_metadata_generator**, **dataset_metadata_generator**, **datablock_metadata_generator**,  **datablock_metadata_stream_generator**, **datablock_metadata_generator_scanpath_postfix**, **attachment_metadata_generator**, **chmod_generator_switch**, **relative_path_generator_switch** can contain the following keywords: *{beamtimeid}* , *{scanname}*, *{chmod}*, *{scanpath}*, *{metapath}*, *{relpath}*, *{beamtimeid}*, *{beamline}*, *{pidprefix}*, *{beamtimefile}*, *{scanpostfix}*, *{datablockpostfix}*, *{ownergroup}*, *{accessgroups}*, *{hostname}*, *{homepath}*, *{hiddenattributes}*, *{ext}*, "{masterfile}", "{plotfile}"
         
+        The "{masterfile}" is either equal to   "{scanpath}/{scanname}.{ext}" or "{scanpath}/{scanname}/{scanname}.{ext}". Also
+        the "{plotfile}" is either equal to  "{scanpath}/{scanname}.{plotext}" or "{scanpath}/{scanname}/{scanname}.{plotext}".
         
         
         ## scicat_dataset_ingest
         
         Re-ingestion script for SciCat Datasets and OrigDatablocks is usually launched at the end of the beamtime.
         ```
         scicat_dataset_ingest -c ~/.scingestor.yaml
```

### Comparing `scingestor-0.8.1/README.md` & `scingestor-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,20 +33,30 @@
 * **attachment_metadata_postfix** *(str)* , default: `".attachment.json"`
 * **metadata_in_var_dir** *(bool)* , default: `False`
 * **use_corepath_as_scandir** *(bool)* , default: `False`
 * **beamtime_filename_postfix** *(str)* , default: `"beamtime-metadata-"`
 * **beamtime_filename_prefix** *(str)* , default: `".json"`
 * **datasets_filename_pattern** *(str)* , default: `"scicat-datasets-{beamtimeid}.lst"`
 * **ingested_datasets_filename_pattern** *(str)* , default: `"scicat-ingested-datasets-{beamtimeid}.lst"`
-* **file_dataset_metadata_generator** *(str)* , default: `"nxsfileinfo metadata -k4  -o {metapath}/{scanname}{scanpostfix}  -b {beamtimefile} -p {beamtimeid}/{scanname}  -w {ownergroup} -c {accessgroups} {scanpath}/{scanname}.{ext}"`
+* **file_dataset_metadata_generator** *(str)* , default: `"nxsfileinfo metadata -k4  -o {metapath}/{scanname}{scanpostfix}  -b {beamtimefile} -p {beamtimeid}/{scanname}  -w {ownergroup} -c {accessgroups} {mastefile}"`
 * **dataset_metadata_generator** *(str)* , default: `"nxsfileinfo metadata -k4  -o {metapath}/{scanname}{scanpostfix}  -c {accessgroups} -w {ownergroup} -b {beamtimefile} -p {beamtimeid}/{scanname}"`
 * **datablock_metadata_generator** *(str)* , default: `"nxsfileinfo origdatablock  -s *.pyc,*{datablockpostfix},*{scanpostfix},*~  -p {pidprefix}{beamtimeid}/{scanname}  -w {ownergroup} -c {accessgroups} -o {metapath}/{scanname}{datablockpostfix} "`
 * **datablock_metadata_stream_generator** *(str)* , default: `"nxsfileinfo origdatablock  -s *.pyc,*{datablockpostfix},*{scanpostfix},*~  -w {ownergroup} -c {accessgroups} -p {pidprefix}{beamtimeid}/{scanname} "`
 * **datablock_metadata_generator_scanpath_postfix** *(str)* , default: `" {scanpath}/{scanname} "`
-* **attachment_metadata_generator** *(str)* , default: `"nxsfileinfo attachment  -w {ownergroup} -c {accessgroups} -o {metapath}/{scanname}{attachmentpostfix} "`
+* **attachment_metadata_generator** *(str)* , default: `"nxsfileinfo attachment  -w {ownergroup} -c {accessgroups} -o {metapath}/{scanname}{attachmentpostfix} {plotfile} "`
+* **metadata_generated_callback** *(str)* , default: `"nxsfileinfo groupmetadata  {lastmeasurement} -m {metapath}/{scanname}{scanpostfix} -d {metapath}/{scanname}{datablockpostfix} -a {metapath}/{scanname}{attachmentpostfix} -p {beamtimeid}/{lastmeasurement} -f -k4 "`
+* **metadata_group_map_file** *(str)* , default: `""`
+* **raw_metadata_callback** *(bool)* , default: `False`
+* **skip_multi_datablock_ingestion** *(bool)* , default: `False`
+* **skip_multi_attachment_ingestion** *(bool)* , default: `False`
+* **skip_scan_dataset_ingestion** *(bool)* , default: `False`
+* **call_metadata_generated_callback** *(bool)* , default: `False`
+* **metadata_group_map_file_generator_switch** *(str)* , default: `" --group-map-file {groupmapfile} "`
+* **raw_metadata_callback_switch** *(str)* , default: `" --raw "`
+* **execute_commands** *(bool)* , default: `False`
 * **plot_file_extension_list** *(list\<str\>)* , default: `["png", "nxs", "h5", "ndf", "nx", "fio"]`
 * **master_file_extension_list** *(list\<str\>)* , default: `["nxs", "h5", "ndf", "nx", "fio"]`
 * **chmod_generator_switch** *(str)* , default: `" -x {chmod} "`
 * **relative_path_generator_switch** *(str)* , default: `" -r {relpath} "`
 * **oned_dataset_generator_switch** *(str)* , default: `" --oned "`
 * **max_oned_dataset_generator_switch** *(str)* , default: `" --max-oned-size {maxonedsize} "`
 * **override_attachment_signals_generator_switch** *(bool)* , default: `" --override "`
@@ -93,16 +103,18 @@
 
 ### Pattern keywords for configuration variables
 
 The  **datasets_filename_pattern**, **ingested_datasets_filename_pattern**  and **ingestor_var_dir** can contain the *{beamtimeid}* and *{hostname}* keywords,  e.g. `"scicat-ingested-datasets-{beamtimeid}.lst"` or `"scicat-ingested-datasets-{hostname}-{beamtimeid}.lst"` which is instantiated during the ingestor execution.
 
 The  **beamtime_dirs**, **beamtime_base_dir**, **ingestor_var_dir**, **ingestor_credential_file**, **scandir_blacklist** can contain the *{homepath}* keyword.
 
-Similarly, **file_dataset_metadata_generator**, **dataset_metadata_generator**, **datablock_metadata_generator**,  **datablock_metadata_stream_generator**, **datablock_metadata_generator_scanpath_postfix**, **attachment_metadata_generator**, **chmod_generator_switch**, **relative_path_generator_switch** can contain the following keywords: *{beamtimeid}* , *{scanname}*, *{chmod}*, *{scanpath}*, *{metapath}*, *{relpath}*, *{beamtimeid}*, *{beamline}*, *{pidprefix}*, *{beamtimefile}*, *{scanpostfix}*, *{datablockpostfix}*, *{ownergroup}*, *{accessgroups}*, *{hostname}*, *{homepath}*, *{hiddenattributes}*, *{ext}*
+Similarly, **file_dataset_metadata_generator**, **dataset_metadata_generator**, **datablock_metadata_generator**,  **datablock_metadata_stream_generator**, **datablock_metadata_generator_scanpath_postfix**, **attachment_metadata_generator**, **chmod_generator_switch**, **relative_path_generator_switch** can contain the following keywords: *{beamtimeid}* , *{scanname}*, *{chmod}*, *{scanpath}*, *{metapath}*, *{relpath}*, *{beamtimeid}*, *{beamline}*, *{pidprefix}*, *{beamtimefile}*, *{scanpostfix}*, *{datablockpostfix}*, *{ownergroup}*, *{accessgroups}*, *{hostname}*, *{homepath}*, *{hiddenattributes}*, *{ext}*, "{masterfile}", "{plotfile}"
 
+The "{masterfile}" is either equal to   "{scanpath}/{scanname}.{ext}" or "{scanpath}/{scanname}/{scanname}.{ext}". Also
+the "{plotfile}" is either equal to  "{scanpath}/{scanname}.{plotext}" or "{scanpath}/{scanname}/{scanname}.{plotext}".
 
 
 ## scicat_dataset_ingest
 
 Re-ingestion script for SciCat Datasets and OrigDatablocks is usually launched at the end of the beamtime.
 ```
 scicat_dataset_ingest -c ~/.scingestor.yaml
```

### Comparing `scingestor-0.8.1/config/default_template.yaml` & `scingestor-0.9.0/config/default_template.yaml`

 * *Files identical despite different names*

### Comparing `scingestor-0.8.1/config/format_default.sh` & `scingestor-0.9.0/config/format_default.sh`

 * *Files identical despite different names*

### Comparing `scingestor-0.8.1/doc/conf.py` & `scingestor-0.9.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `scingestor-0.8.1/doc/index.rst` & `scingestor-0.9.0/doc/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -67,20 +67,30 @@
 * **attachment_metadata_postfix** *(str)* , default: ``".attachment.json"``
 * **metadata_in_var_dir** *(bool)* , default: ``False``
 * **use_corepath_as_scandir** *(bool)* , default: ``False``
 * **beamtime_filename_postfix** *(str)* , default: ``"beamtime-metadata-"``
 * **beamtime_filename_prefix** *(str)* , default: ``".json"``
 * **datasets_filename_pattern** *(str)* , default: ``"scicat-datasets-{beamtimeid}.lst"``
 * **ingested_datasets_filename_pattern** *(str)* , default: ``"scicat-ingested-datasets-{beamtimeid}.lst"``
-* **file_dataset_metadata_generator** *(str)* , default: ``"nxsfileinfo metadata -k4 -o {metapath}/{scanname}{scanpostfix}  -b {beamtimefile} -p {beamtimeid}/{scanname}  -w {ownergroup} -c {accessgroups} {scanpath}/{scanname}.{ext}"``
+* **file_dataset_metadata_generator** *(str)* , default: ``"nxsfileinfo metadata -k4 -o {metapath}/{scanname}{scanpostfix}  -b {beamtimefile} -p {beamtimeid}/{scanname}  -w {ownergroup} -c {accessgroups} {masterfile}``
 * **dataset_metadata_generator** *(str)* , default: ``"nxsfileinfo metadata -k4 -o {metapath}/{scanname}{scanpostfix}  -c {accessgroups} -w {ownergroup} -b {beamtimefile} -p {beamtimeid}/{scanname}"``
 * **datablock_metadata_generator** *(str)* , default: ``"nxsfileinfo origdatablock  -s *.pyc,*{datablockpostfix},*{scanpostfix},*~  -p {doiprefix}/{beamtimeid}/{scanname}  -w {ownergroup} -c {accessgroups} -o {metapath}/{scanname}{datablockpostfix} "``
 * **datablock_metadata_stream_generator** *(str)* , default: ``"nxsfileinfo origdatablock  -s *.pyc,*{datablockpostfix},*{scanpostfix},*~  -w {ownergroup} -c {accessgroups} -p {doiprefix}/{beamtimeid}/{scanname} "``
 * **datablock_metadata_generator_scanpath_postfix** *(str)* , default: ``" {scanpath}/{scanname} "``
-* **attachment_metadata_generator** *(str)* , default: ``"nxsfileinfo attachment  -w {ownergroup} -c {accessgroups} -o {metapath}/{scanname}{attachmentpostfix} "``
+* **attachment_metadata_generator** *(str)* , default: ``"nxsfileinfo attachment  -w {ownergroup} -c {accessgroups} -o {metapath}/{scanname}{attachmentpostfix} {plotfile} "``
+* **metadata_generated_callback** *(str)* , default: ``"nxsfileinfo groupmetadata  {lastmeasurement} -m {metapath}/{scanname}{scanpostfix} -d {metapath}/{scanname}{datablockpostfix} -a {metapath}/{scanname}{attachmentpostfix} -p {beamtimeid}/{lastmeasurement} -f -k4 "``
+* **metadata_group_map_file** *(str)* , default: ``""``
+* **raw_metadata_callback** *(bool)* , default: ``False``
+* **skip_multi_datablock_ingestion** *(bool)* , default: ``False``
+* **skip_multi_attachment_ingestion** *(bool)* , default: ``False``
+* **skip_scan_dataset_ingestion** *(bool)* , default: ``False``
+* **call_metadata_generated_callback** *(bool)* , default: ``False``
+* **metadata_group_map_file_generator_switch** *(str)* , default: ``" --group-map-file {groupmapfile} "``
+* **raw_metadata_callback_switch** *(str)* , default: ``" --raw "``
+* **execute_commands** *(bool)* , default: ``False``
 * **plot_file_extension_list** *(list\<str\>)* , default: ``["png", "nxs", "h5", "ndf", "nx", "fio"]``
 * **master_file_extension_list** *(list\<str\>)* , default: ``["nxs", "h5", "ndf", "nx", "fio"]``
 * **chmod_generator_switch** *(str)* , default: ``" -x {chmod} "``
 * **relative_path_generator_switch** *(str)* , default: ``" -r {relpath} "``
 * **oned_dataset_generator_switch** *(str)* , default: ``" --oned "``
 * **max_oned_dataset_generator_switch** *(str)* , default: ``" --max-oned-size {maxonedsize} "``
 * **override_attachment_signals_generator_switch** *(bool)* , default: ``" --override "``
@@ -127,15 +137,19 @@
    ingestor_credential_file: "{homepath}/gpfs/pwd"
 
 Pattern keywords for configuration variables
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The  **datasets_filename_pattern**, **ingested_datasets_filename_pattern**  and **ingestor_var_dir** can contain the *{beamtimeid}* and *{hostname}* keywords,  e.g. ``"scicat-ingested-datasets-{beamtimeid}.lst"`` or ``"scicat-ingested-datasets-{hostname}-{beamtimeid}.lst"``  which is instantiated during the ingestor execution.
 
-Similarly, **file_dataset_metadata_generator**, **dataset_metadata_generator**, **datablock_metadata_generator**,  **datablock_metadata_stream_generator**, **datablock_metadata_generator_scanpath_postfix**, **attachment_metadata_generator**, **chmod_generator_switch**, **relative_path_generator_switch**  can contain the following keywords: *{beamtimeid}* , *{scanname}*, *{chmod}*, *{scanpath}*, *{metapath}*, *{relpath}*, *{beamtimeid}*, *{beamline}*, *{doiprefix}*, *{beamtimefile}*, *{scanpostfix}*, *{datablockpostfix}*, *{ownergroup}*, *{accessgroups}*, *{hostname}*, *{hiddenattributes}*, *{ext}*
+Similarly, **file_dataset_metadata_generator**, **dataset_metadata_generator**, **datablock_metadata_generator**,  **datablock_metadata_stream_generator**, **datablock_metadata_generator_scanpath_postfix**, **attachment_metadata_generator**, **chmod_generator_switch**, **relative_path_generator_switch**  can contain the following keywords: *{beamtimeid}* , *{scanname}*, *{chmod}*, *{scanpath}*, *{metapath}*, *{relpath}*, *{beamtimeid}*, *{beamline}*, *{doiprefix}*, *{beamtimefile}*, *{scanpostfix}*, *{datablockpostfix}*, *{ownergroup}*, *{accessgroups}*, *{hostname}*, *{hiddenattributes}*, *{ext}*, "{masterfile}", "{plotfile}"
+
+The "{masterfile}" is either equal to   "{scanpath}/{scanname}.{ext}" or "{scanpath}/{scanname}/{scanname}.{ext}". Also
+the "{plotfile}" is either equal to  "{scanpath}/{scanname}.{plotext}" or "{scanpath}/{scanname}/{scanname}.{plotext}".
+
 
 
 scicat_dataset_ingest
 ---------------------
 
 Re-ingestion script for SciCat Datasets and OrigDatablocks is usually
 launched at the end of the beamtime.
```

### Comparing `scingestor-0.8.1/doc/scicat_dataset_ingest.rst` & `scingestor-0.9.0/doc/scicat_dataset_ingest.rst`

 * *Files identical despite different names*

### Comparing `scingestor-0.8.1/doc/scicat_dataset_ingestor.rst` & `scingestor-0.9.0/doc/scicat_dataset_ingestor.rst`

 * *Files identical despite different names*

### Comparing `scingestor-0.8.1/doc/scicat_ingest.rst` & `scingestor-0.9.0/doc/scicat_ingest.rst`

 * *Files identical despite different names*

### Comparing `scingestor-0.8.1/doc/scingestor.rst` & `scingestor-0.9.0/doc/scingestor.rst`

 * *Files identical despite different names*

### Comparing `scingestor-0.8.1/man/scicat_dataset_ingest.1` & `scingestor-0.9.0/man/scicat_dataset_ingest.1`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "SCICAT_DATASET_INGEST" "1" "Apr 05, 2023" "0.6" "SciCat Dataset Ingestor"
+.TH "SCICAT_DATASET_INGEST" "1" "Nov 24, 2023" "0.9" "SciCat Dataset Ingestor"
 .SH NAME
 scicat_dataset_ingest \- Reingestion script to upload SciCat Datasets
 .SH DESCRIPTION
 .sp
 Re\-ingestion script for SciCat Datasets.
 .SH SYNOPSIS
 .INDENT 0.0
```

### Comparing `scingestor-0.8.1/man/scicat_dataset_ingestor.1` & `scingestor-0.9.0/man/scicat_dataset_ingestor.1`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "SCICAT_DATASET_INGESTOR" "1" "Apr 05, 2023" "0.6" "SciCat Dataset Ingestor"
+.TH "SCICAT_DATASET_INGESTOR" "1" "Nov 24, 2023" "0.9" "SciCat Dataset Ingestor"
 .SH NAME
 scicat_dataset_ingestor \- Server daemon to ingest SciCat Datasets
 .SH DESCRIPTION
 .sp
 BeamtimeWatcher service SciCat Dataset ingestor.
 .SH SYNOPSIS
 .INDENT 0.0
```

### Comparing `scingestor-0.8.1/man/scicat_ingest.1` & `scingestor-0.9.0/man/scicat_ingest.1`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "SCICAT_INGEST" "1" "Apr 05, 2023" "0.6" "SciCat Dataset Ingestor"
+.TH "SCICAT_INGEST" "1" "Nov 24, 2023" "0.9" "SciCat Dataset Ingestor"
 .SH NAME
 scicat_ingest \- General ingest script to upload SciCat Samples or Instruments
 .SH DESCRIPTION
 .sp
 Re\-ingestion script for SciCat Datasets.
 .SH SYNOPSIS
 .INDENT 0.0
```

### Comparing `scingestor-0.8.1/man/scingestor.1` & `scingestor-0.9.0/man/scingestor.1`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "SCINGESTOR" "1" "Apr 05, 2023" "0.6" "SciCat Dataset Ingestor"
+.TH "SCINGESTOR" "1" "Nov 24, 2023" "0.9" "SciCat Dataset Ingestor"
 .SH NAME
 scingestor \- SciCat Dataset Ingestor Documentation
 .sp
 \fI\%\fP
 \fI\%\fP
 \fI\%\fP
 \fI\%\fP
@@ -53,169 +53,196 @@
 .UNINDENT
 .UNINDENT
 .SS Configuration variables
 .sp
 The configuration written in YAML can contain the following variables
 .INDENT 0.0
 .IP \(bu 2
-\fBscicat_url\fP \fI(str)\fP , default: \fB"http://localhost:3000/api/v3"\fP
+\fBscicat_url\fP \fI(str)\fP , default: \fB\(dqhttp://localhost:3000/api/v3\(dq\fP
 .IP \(bu 2
 \fBingestor_credential_file\fP \fI(str)\fP , default: \fBNone\fP
 .IP \(bu 2
 \fBbeamtime_dirs\fP \fI(list<str>)\fP , default: \fB[]\fP
 .IP \(bu 2
-\fBbeamtime_base_dir\fP \fI(str)\fP , default: \fB""\fP
+\fBbeamtime_base_dir\fP \fI(str)\fP , default: \fB\(dq\(dq\fP
 .IP \(bu 2
-\fBingestor_var_dir\fP \fI(str)\fP , default: \fB""\fP
+\fBingestor_var_dir\fP \fI(str)\fP , default: \fB\(dq\(dq\fP
 .IP \(bu 2
-\fBingestor_username\fP \fI(str)\fP , default: \fB"ingestor"\fP
+\fBingestor_username\fP \fI(str)\fP , default: \fB\(dqingestor\(dq\fP
 .IP \(bu 2
-\fBdataset_pid_prefix\fP \fI(str)\fP , default: \fB""\fP
+\fBdataset_pid_prefix\fP \fI(str)\fP , default: \fB\(dq\(dq\fP
 .IP \(bu 2
-\fBdataset_update_strategy\fP (\fB"no"\fP, \fB"patch"\fP, \fB"create"\fP, \fB"mixed"\fP) , default: \fB"patch"\fP
+\fBdataset_update_strategy\fP (\fB\(dqno\(dq\fP, \fB\(dqpatch\(dq\fP, \fB\(dqcreate\(dq\fP, \fB\(dqmixed\(dq\fP) , default: \fB\(dqpatch\(dq\fP
 .IP \(bu 2
 \fBrelative_path_in_datablock\fP \fI(bool)\fP , default: \fBFalse\fP
 .IP \(bu 2
-\fBscandir_blacklist\fP \fI(list<str>)\fP , default: \fB["/gpfs/current/scratch_bl", "/gpfs/current/processed", "/gpfs/current/shared"]\fP
+\fBscandir_blacklist\fP \fI(list<str>)\fP , default: \fB[\(dq/gpfs/current/scratch_bl\(dq, \(dq/gpfs/current/processed\(dq, \(dq/gpfs/current/shared\(dq]\fP
 .IP \(bu 2
 \fBbeamtimeid_blacklist_file\fP \fI(str)\fP , default: \fBNone\fP
 .IP \(bu 2
-\fBbeamtime_type_blacklist\fP \fI(list<str>)\fP , default: \fB["P"]\fP
+\fBbeamtime_type_blacklist\fP \fI(list<str>)\fP , default: \fB[\(dqP\(dq]\fP
 .IP \(bu 2
 \fBchmod_json_files\fP \fI(str)\fP , default: \fBNone\fP
 .IP \(bu 2
 \fBmax_scandir_depth\fP \fI(int)\fP, default: \fB\-1\fP
 .IP \(bu 2
 \fBoned_in_metadata\fP \fI(bool)\fP , default: \fBFalse\fP
 .IP \(bu 2
 \fBmax_oned_size\fP \fI(int)\fP , default: \fBNone\fP
 .IP \(bu 2
-\fBscan_metadata_postfix\fP \fI(str)\fP , default: \fB".scan.json"\fP
+\fBscan_metadata_postfix\fP \fI(str)\fP , default: \fB\(dq.scan.json\(dq\fP
 .IP \(bu 2
-\fBdatablock_metadata_postfix\fP \fI(str)\fP , default: \fB".origdatablock.json"\fP
+\fBdatablock_metadata_postfix\fP \fI(str)\fP , default: \fB\(dq.origdatablock.json\(dq\fP
 .IP \(bu 2
-\fBattachment_metadata_postfix\fP \fI(str)\fP , default: \fB".attachment.json"\fP
+\fBattachment_metadata_postfix\fP \fI(str)\fP , default: \fB\(dq.attachment.json\(dq\fP
 .IP \(bu 2
 \fBmetadata_in_var_dir\fP \fI(bool)\fP , default: \fBFalse\fP
 .IP \(bu 2
 \fBuse_corepath_as_scandir\fP \fI(bool)\fP , default: \fBFalse\fP
 .IP \(bu 2
-\fBbeamtime_filename_postfix\fP \fI(str)\fP , default: \fB"beamtime\-metadata\-"\fP
+\fBbeamtime_filename_postfix\fP \fI(str)\fP , default: \fB\(dqbeamtime\-metadata\-\(dq\fP
 .IP \(bu 2
-\fBbeamtime_filename_prefix\fP \fI(str)\fP , default: \fB".json"\fP
+\fBbeamtime_filename_prefix\fP \fI(str)\fP , default: \fB\(dq.json\(dq\fP
 .IP \(bu 2
-\fBdatasets_filename_pattern\fP \fI(str)\fP , default: \fB"scicat\-datasets\-{beamtimeid}.lst"\fP
+\fBdatasets_filename_pattern\fP \fI(str)\fP , default: \fB\(dqscicat\-datasets\-{beamtimeid}.lst\(dq\fP
 .IP \(bu 2
-\fBingested_datasets_filename_pattern\fP \fI(str)\fP , default: \fB"scicat\-ingested\-datasets\-{beamtimeid}.lst"\fP
+\fBingested_datasets_filename_pattern\fP \fI(str)\fP , default: \fB\(dqscicat\-ingested\-datasets\-{beamtimeid}.lst\(dq\fP
 .IP \(bu 2
-\fBfile_dataset_metadata_generator\fP \fI(str)\fP , default: \fB"nxsfileinfo metadata  \-k4 \-o {metapath}/{scanname}{scanpostfix}  \-b {beamtimefile} \-p {beamtimeid}/{scanname}  \-w {ownergroup} \-c {accessgroups} {scanpath}/{scanname}.{ext}"\fP
+\fBfile_dataset_metadata_generator\fP \fI(str)\fP , default: \fB\(dqnxsfileinfo metadata \-k4 \-o {metapath}/{scanname}{scanpostfix}  \-b {beamtimefile} \-p {beamtimeid}/{scanname}  \-w {ownergroup} \-c {accessgroups} {masterfile}\fP
 .IP \(bu 2
-\fBdataset_metadata_generator\fP \fI(str)\fP , default: \fB"nxsfileinfo metadata  \-k4 \-o {metapath}/{scanname}{scanpostfix}  \-c {accessgroups} \-w {ownergroup} \-b {beamtimefile} \-p {beamtimeid}/{scanname}"\fP
+\fBdataset_metadata_generator\fP \fI(str)\fP , default: \fB\(dqnxsfileinfo metadata \-k4 \-o {metapath}/{scanname}{scanpostfix}  \-c {accessgroups} \-w {ownergroup} \-b {beamtimefile} \-p {beamtimeid}/{scanname}\(dq\fP
 .IP \(bu 2
-\fBdatablock_metadata_generator\fP \fI(str)\fP , default: \fB"nxsfileinfo origdatablock  \-s *.pyc,*{datablockpostfix},*{scanpostfix},*~  \-p {doiprefix}/{beamtimeid}/{scanname}  \-w {ownergroup} \-c {accessgroups} \-o {metapath}/{scanname}{datablockpostfix} "\fP
+\fBdatablock_metadata_generator\fP \fI(str)\fP , default: \fB\(dqnxsfileinfo origdatablock  \-s *.pyc,*{datablockpostfix},*{scanpostfix},*~  \-p {doiprefix}/{beamtimeid}/{scanname}  \-w {ownergroup} \-c {accessgroups} \-o {metapath}/{scanname}{datablockpostfix} \(dq\fP
 .IP \(bu 2
-\fBdatablock_metadata_stream_generator\fP \fI(str)\fP , default: \fB"nxsfileinfo origdatablock  \-s *.pyc,*{datablockpostfix},*{scanpostfix},*~  \-w {ownergroup} \-c {accessgroups} \-p {doiprefix}/{beamtimeid}/{scanname} "\fP
+\fBdatablock_metadata_stream_generator\fP \fI(str)\fP , default: \fB\(dqnxsfileinfo origdatablock  \-s *.pyc,*{datablockpostfix},*{scanpostfix},*~  \-w {ownergroup} \-c {accessgroups} \-p {doiprefix}/{beamtimeid}/{scanname} \(dq\fP
 .IP \(bu 2
-\fBdatablock_metadata_generator_scanpath_postfix\fP \fI(str)\fP , default: \fB" {scanpath}/{scanname} "\fP
+\fBdatablock_metadata_generator_scanpath_postfix\fP \fI(str)\fP , default: \fB\(dq {scanpath}/{scanname} \(dq\fP
 .IP \(bu 2
-\fBattachment_metadata_generator\fP \fI(str)\fP , default: \fB"nxsfileinfo attachment  \-w {ownergroup} \-c {accessgroups} \-o {metapath}/{scanname}{attachmentpostfix} "\fP
+\fBattachment_metadata_generator\fP \fI(str)\fP , default: \fB\(dqnxsfileinfo attachment  \-w {ownergroup} \-c {accessgroups} \-o {metapath}/{scanname}{attachmentpostfix} {plotfile} \(dq\fP
 .IP \(bu 2
-\fBplot_file_extension_list\fP \fI(list<str>)\fP , default: \fB["png", "nxs", "h5", "ndf", "nx", "fio"]\fP
+\fBmetadata_generated_callback\fP \fI(str)\fP , default: \fB\(dqnxsfileinfo groupmetadata  {lastmeasurement} \-m {metapath}/{scanname}{scanpostfix} \-d {metapath}/{scanname}{datablockpostfix} \-a {metapath}/{scanname}{attachmentpostfix} \-p {beamtimeid}/{lastmeasurement} \-f \-k4 \(dq\fP
 .IP \(bu 2
-\fBmaster_file_extension_list\fP \fI(list<str>)\fP , default: \fB["nxs", "h5", "ndf", "nx", "fio"]\fP
+\fBmetadata_group_map_file\fP \fI(str)\fP , default: \fB\(dq\(dq\fP
 .IP \(bu 2
-\fBchmod_generator_switch\fP \fI(str)\fP , default: \fB" \-x {chmod} "\fP
+\fBraw_metadata_callback\fP \fI(bool)\fP , default: \fBFalse\fP
 .IP \(bu 2
-\fBrelative_path_generator_switch\fP \fI(str)\fP , default: \fB" \-r {relpath} "\fP
+\fBskip_multi_datablock_ingestion\fP \fI(bool)\fP , default: \fBFalse\fP
 .IP \(bu 2
-\fBoned_dataset_generator_switch\fP \fI(str)\fP , default: \fB" \-\-oned "\fP
+\fBskip_multi_attachment_ingestion\fP \fI(bool)\fP , default: \fBFalse\fP
 .IP \(bu 2
-\fBmax_oned_dataset_generator_switch\fP \fI(str)\fP , default: \fB" \-\-max\-oned\-size {maxonedsize} "\fP
+\fBskip_scan_dataset_ingestion\fP \fI(bool)\fP , default: \fBFalse\fP
 .IP \(bu 2
-\fBoverride_attachment_signals_generator_switch\fP \fI(bool)\fP , default: \fB" \-\-override "\fP
+\fBcall_metadata_generated_callback\fP \fI(bool)\fP , default: \fBFalse\fP
 .IP \(bu 2
-\fBhidden_attributes_generator_switch\fP \fI(str)\fP , default: \fB" \-n {hiddenattributes} "\fP
+\fBmetadata_group_map_file_generator_switch\fP \fI(str)\fP , default: \fB\(dq \-\-group\-map\-file {groupmapfile} \(dq\fP
 .IP \(bu 2
-\fBhidden_attributes\fP \fI(str)\fP , default: \fB"nexdatas_source,nexdatas_strategy,units"\fP
+\fBraw_metadata_callback_switch\fP \fI(str)\fP , default: \fB\(dq \-\-raw \(dq\fP
 .IP \(bu 2
-\fBattachment_signals_generator_switch\fP \fI(str)\fP , default: \fB" \-s {signals} "\fP
+\fBexecute_commands\fP \fI(bool)\fP , default: \fBFalse\fP
 .IP \(bu 2
-\fBattachment_axes_generator_switch\fP \fI(str)\fP , default: \fB" \-e {axes} "\fP
+\fBplot_file_extension_list\fP \fI(list<str>)\fP , default: \fB[\(dqpng\(dq, \(dqnxs\(dq, \(dqh5\(dq, \(dqndf\(dq, \(dqnx\(dq, \(dqfio\(dq]\fP
 .IP \(bu 2
-\fBattachment_frame_generator_switch\fP \fI(str)\fP , default: \fB" \-m {frame} "\fP
+\fBmaster_file_extension_list\fP \fI(list<str>)\fP , default: \fB[\(dqnxs\(dq, \(dqh5\(dq, \(dqndf\(dq, \(dqnx\(dq, \(dqfio\(dq]\fP
 .IP \(bu 2
-\fBattachment_signal_names\fP \fI(str)\fP , default: \fB""\fP
+\fBchmod_generator_switch\fP \fI(str)\fP , default: \fB\(dq \-x {chmod} \(dq\fP
 .IP \(bu 2
-\fBattachment_axes_names\fP \fI(str)\fP , default: \fB""\fP
+\fBrelative_path_generator_switch\fP \fI(str)\fP , default: \fB\(dq \-r {relpath} \(dq\fP
 .IP \(bu 2
-\fBattachment_image_frame_number\fP \fI(str)\fP , default: \fB""\fP
+\fBoned_dataset_generator_switch\fP \fI(str)\fP , default: \fB\(dq \-\-oned \(dq\fP
+.IP \(bu 2
+\fBmax_oned_dataset_generator_switch\fP \fI(str)\fP , default: \fB\(dq \-\-max\-oned\-size {maxonedsize} \(dq\fP
+.IP \(bu 2
+\fBoverride_attachment_signals_generator_switch\fP \fI(bool)\fP , default: \fB\(dq \-\-override \(dq\fP
+.IP \(bu 2
+\fBhidden_attributes_generator_switch\fP \fI(str)\fP , default: \fB\(dq \-n {hiddenattributes} \(dq\fP
+.IP \(bu 2
+\fBhidden_attributes\fP \fI(str)\fP , default: \fB\(dqnexdatas_source,nexdatas_strategy,units\(dq\fP
+.IP \(bu 2
+\fBattachment_signals_generator_switch\fP \fI(str)\fP , default: \fB\(dq \-s {signals} \(dq\fP
+.IP \(bu 2
+\fBattachment_axes_generator_switch\fP \fI(str)\fP , default: \fB\(dq \-e {axes} \(dq\fP
+.IP \(bu 2
+\fBattachment_frame_generator_switch\fP \fI(str)\fP , default: \fB\(dq \-m {frame} \(dq\fP
+.IP \(bu 2
+\fBattachment_signal_names\fP \fI(str)\fP , default: \fB\(dq\(dq\fP
+.IP \(bu 2
+\fBattachment_axes_names\fP \fI(str)\fP , default: \fB\(dq\(dq\fP
+.IP \(bu 2
+\fBattachment_image_frame_number\fP \fI(str)\fP , default: \fB\(dq\(dq\fP
 .IP \(bu 2
 \fBingest_dataset_attachment\fP \fI(bool)\fP , default: \fBFalse\fP
 .IP \(bu 2
 \fBoverride_attachment_signals\fP \fI(bool)\fP , default: \fBFalse\fP
 .IP \(bu 2
+\fBretry_failed_dataset_ingestion\fP \fI(bool)\fP , default:\fBFalse\fP
+.IP \(bu 2
+\fBretry_failed_attachment_ingestion\fP \fI(bool)\fP , default:\fBFalse\fP
+.IP \(bu 2
 \fBlog_generator_commands\fP \fI(bool)\fP , default: \fBFalse\fP
 .IP \(bu 2
-\fBadd_empty_units_generator_switch\fP \fI(str)\fP , default: \fB" \-\-add\-empty\-units "\fP
+\fBadd_empty_units_generator_switch\fP \fI(str)\fP , default: \fB\(dq \-\-add\-empty\-units \(dq\fP
 .IP \(bu 2
 \fBadd_empty_units\fP \fI(bool)\fP , default: \fBTrue\fP
 .IP \(bu 2
 \fBmetadata_copy_map_file\fP \fI(str)\fP , default: \fBNone\fP
 .IP \(bu 2
-\fBmetadata_copy_map_file_generator_switch\fP \fI(str)\fP , default: \fB" \-\-copy\-map\-file {copymapfile} "\fP
+\fBmetadata_copy_map_file_generator_switch\fP \fI(str)\fP , default: \fB\(dq \-\-copy\-map\-file {copymapfile} \(dq\fP
 .IP \(bu 2
 \fBinotify_timeout\fP \fI(float)\fP , default: \fB0.1\fP
 .IP \(bu 2
 \fBget_event_timeout\fP \fI(float)\fP , default: \fB0.01\fP
 .IP \(bu 2
 \fBingestion_delay_time\fP \fI(float)\fP , default: \fB5.0\fP
 .IP \(bu 2
 \fBmax_request_tries_number\fP \fI(int)\fP , default: \fB100\fP
 .IP \(bu 2
 \fBrecheck_dataset_list_interval\fP \fI(int)\fP , default: \fB1000\fP
 .IP \(bu 2
 \fBrecheck_beamtime_file_interval\fP \fI(int)\fP , default: \fB1000\fP
 .IP \(bu 2
-\fBrequest_headers\fP \fI(dict<str,str>)\fP , default: \fB{"Content\-Type": "application/json", "Accept": "application/json"}\fP
+\fBrequest_headers\fP \fI(dict<str,str>)\fP , default: \fB{\(dqContent\-Type\(dq: \(dqapplication/json\(dq, \(dqAccept\(dq: \(dqapplication/json\(dq}\fP
 .IP \(bu 2
-\fBscicat_datasets_path\fP \fI(str)\fP , default: \fB"Datasets"\fP
+\fBscicat_datasets_path\fP \fI(str)\fP , default: \fB\(dqDatasets\(dq\fP
 .IP \(bu 2
-\fBscicat_proposals_path\fP \fI(str)\fP , default: \fB"Proposals"\fP
+\fBscicat_proposals_path\fP \fI(str)\fP , default: \fB\(dqProposals\(dq\fP
 .IP \(bu 2
-\fBscicat_datablocks_path\fP \fI(str)\fP, default: \fB"OrigDatablocks"\fP
+\fBscicat_datablocks_path\fP \fI(str)\fP, default: \fB\(dqOrigDatablocks\(dq\fP
 .IP \(bu 2
-\fBscicat_users_login_path\fP \fI(str)\fP, default: \fB"Users/login"\fP
+\fBscicat_users_login_path\fP \fI(str)\fP, default: \fB\(dqUsers/login\(dq\fP
 .IP \(bu 2
-\fBscicat_attachments_path\fP \fI(str)\fP, default: \fB"Datasets/{pid}/Attachments"\fP
+\fBscicat_attachments_path\fP \fI(str)\fP, default: \fB\(dqDatasets/{pid}/Attachments\(dq\fP
 .IP \(bu 2
 \fBowner_access_groups_from_proposal\fP \fI(bool)\fP, default: \fBFalse\fP
 .IP \(bu 2
-\fBmetadata_keywords_without_checks\fP \fI(list<str>)\fP, default: \fB["techniques", "classification", "createdBy", "updatedBy", "datasetlifecycle", "numberOfFiles", "size", "createdAt", "updatedAt", "history", "creationTime", "version", "scientificMetadata", "endTime"]\fP
+\fBmetadata_keywords_without_checks\fP \fI(list<str>)\fP, default: \fB[\(dqtechniques\(dq, \(dqclassification\(dq, \(dqcreatedBy\(dq, \(dqupdatedBy\(dq, \(dqdatasetlifecycle\(dq, \(dqnumberOfFiles\(dq, \(dqsize\(dq, \(dqcreatedAt\(dq, \(dqupdatedAt\(dq, \(dqhistory\(dq, \(dqcreationTime\(dq, \(dqversion\(dq, \(dqscientificMetadata\(dq, \(dqendTime\(dq]\fP
 .UNINDENT
 .sp
 e.g.
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 beamtime_dirs:
-  \- "{homepath}/gpfs/current"
-  \- "{homepath}/gpfs/commissioning"
+  \- \(dq{homepath}/gpfs/current\(dq
+  \- \(dq{homepath}/gpfs/commissioning\(dq
 scicat_url: http://localhost:3000/api/v3
-ingestor_credential_file: "{homepath}/gpfs/pwd"
+ingestor_credential_file: \(dq{homepath}/gpfs/pwd\(dq
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SS Pattern keywords for configuration variables
 .sp
-The  \fBdatasets_filename_pattern\fP, \fBingested_datasets_filename_pattern\fP  and \fBingestor_var_dir\fP can contain the \fI{beamtimeid}\fP and \fI{hostname}\fP keywords,  e.g. \fB"scicat\-ingested\-datasets\-{beamtimeid}.lst"\fP or \fB"scicat\-ingested\-datasets\-{hostname}\-{beamtimeid}.lst"\fP  which is instantiated during the ingestor execution.
+The  \fBdatasets_filename_pattern\fP, \fBingested_datasets_filename_pattern\fP  and \fBingestor_var_dir\fP can contain the \fI{beamtimeid}\fP and \fI{hostname}\fP keywords,  e.g. \fB\(dqscicat\-ingested\-datasets\-{beamtimeid}.lst\(dq\fP or \fB\(dqscicat\-ingested\-datasets\-{hostname}\-{beamtimeid}.lst\(dq\fP  which is instantiated during the ingestor execution.
 .sp
-Similarly, \fBfile_dataset_metadata_generator\fP, \fBdataset_metadata_generator\fP, \fBdatablock_metadata_generator\fP,  \fBdatablock_metadata_stream_generator\fP, \fBdatablock_metadata_generator_scanpath_postfix\fP, \fBattachment_metadata_generator\fP, \fBchmod_generator_switch\fP, \fBrelative_path_generator_switch\fP  can contain the following keywords: \fI{beamtimeid}\fP , \fI{scanname}\fP, \fI{chmod}\fP, \fI{scanpath}\fP, \fI{metapath}\fP, \fI{relpath}\fP, \fI{beamtimeid}\fP, \fI{beamline}\fP, \fI{doiprefix}\fP, \fI{beamtimefile}\fP, \fI{scanpostfix}\fP, \fI{datablockpostfix}\fP, \fI{ownergroup}\fP, \fI{accessgroups}\fP, \fI{hostname}\fP, \fI{hiddenattributes}\fP, \fI{ext}\fP
+Similarly, \fBfile_dataset_metadata_generator\fP, \fBdataset_metadata_generator\fP, \fBdatablock_metadata_generator\fP,  \fBdatablock_metadata_stream_generator\fP, \fBdatablock_metadata_generator_scanpath_postfix\fP, \fBattachment_metadata_generator\fP, \fBchmod_generator_switch\fP, \fBrelative_path_generator_switch\fP  can contain the following keywords: \fI{beamtimeid}\fP , \fI{scanname}\fP, \fI{chmod}\fP, \fI{scanpath}\fP, \fI{metapath}\fP, \fI{relpath}\fP, \fI{beamtimeid}\fP, \fI{beamline}\fP, \fI{doiprefix}\fP, \fI{beamtimefile}\fP, \fI{scanpostfix}\fP, \fI{datablockpostfix}\fP, \fI{ownergroup}\fP, \fI{accessgroups}\fP, \fI{hostname}\fP, \fI{hiddenattributes}\fP, \fI{ext}\fP, \(dq{masterfile}\(dq, \(dq{plotfile}\(dq
+.sp
+The \(dq{masterfile}\(dq is either equal to   \(dq{scanpath}/{scanname}.{ext}\(dq or \(dq{scanpath}/{scanname}/{scanname}.{ext}\(dq. Also
+the \(dq{plotfile}\(dq is either equal to  \(dq{scanpath}/{scanname}.{plotext}\(dq or \(dq{scanpath}/{scanname}/{scanname}.{plotext}\(dq.
 .SH SCICAT_DATASET_INGEST
 .sp
 Re\-ingestion script for SciCat Datasets and OrigDatablocks is usually
 launched at the end of the beamtime.
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -333,15 +360,15 @@
 pip install scingestor
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SS Debian and Ubuntu packages
 .sp
-Debian \fBbookworm\fP, \fBbullseye\fP, \fBbuster\fP or Ubuntu \fBlunar\fP , \fBjammy\fP, \fBfocal\fP packages
+Debian \fBbookworm\fP, \fBbullseye\fP, \fBbuster\fP or Ubuntu \fBlunar\fP, \fBjammy\fP, \fBfocal\fP packages
 can be found in the HDRI repository.
 .sp
 To install the debian packages, add the PGP repository key
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
@@ -751,14 +778,29 @@
 .IP \(bu 2
 \fBtoken\fP (\fI\%str\fP) \-\- access token
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
+.B start_measurement(measurement)
+start measurement
+.INDENT 7.0
+.TP
+.B Parameters
+\fBmeasurement\fP (\fI\%str\fP) \-\- measurement name
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B stop_measurement()
+stop measurement
+.UNINDENT
+.INDENT 7.0
+.TP
 .B update_from_tmpfile()
 clear waitings datasets
 .UNINDENT
 .INDENT 7.0
 .TP
 .B waiting_datasets()
 provides waitings datasets
@@ -770,16 +812,16 @@
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class  scingestor.datasetIngestor.UpdateStrategy(value)
-Bases: \fI\%enum.Enum\fP
+.B class  scingestor.datasetIngestor.UpdateStrategy(value, names=None, *, module=None, qualname=None, type=None, start=1, boundary=None)
+Bases: \fI\%Enum\fP
 .sp
 Update strategy
 .INDENT 7.0
 .TP
 .B CREATE  =  2
 (\fI\%scingestor.datasetIngestor.UpdateStrategy\fP) recreate datasets
 .UNINDENT
@@ -801,15 +843,15 @@
 (\fI\%scingestor.datasetIngestor.UpdateStrategy\fP) patch datasets
 .UNINDENT
 .UNINDENT
 .SS scingestor.datasetWatcher module
 .INDENT 0.0
 .TP
 .B class  scingestor.datasetWatcher.DatasetWatcher(configuration, path, dsfile, idsfile, meta, beamtimefile)
-Bases: \fI\%threading.Thread\fP
+Bases: \fI\%Thread\fP
 .sp
 Dataset  Watcher
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
@@ -844,15 +886,15 @@
 stop the watcher
 .UNINDENT
 .UNINDENT
 .SS scingestor.logger module
 .INDENT 0.0
 .TP
 .B class  scingestor.logger.AccSecFormatter(fmt=None, datefmt=None, style=\(aq%\(aq, validate=True, *, defaults=None)
-Bases: \fI\%logging.Formatter\fP
+Bases: \fI\%Formatter\fP
 .sp
 micro\-second formatter
 .sp
 Initialize the formatter with specified format strings.
 .sp
 Initialize the formatter either with the specified format string, or a
 default as described above. Allow for specialized date formatting with
@@ -1043,30 +1085,30 @@
 .B name
 (\fI\%str\fP) name
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class  scingestor.safeINotifier.SafeINotifier(*args, **kwargs)
-Bases: \fI\%threading.Thread\fP
+Bases: \fI\%Thread\fP
 .sp
 singleton wrapper for inotifyx
 .sp
 This constructor should always be called with keyword arguments. Arguments are:
 .sp
 \fIgroup\fP should be None; reserved for future extension when a ThreadGroup
 class is implemented.
 .sp
 \fItarget\fP is the callable object to be invoked by the run()
 method. Defaults to None, meaning nothing is called.
 .sp
 \fIname\fP is the thread name. By default, a unique name is constructed of
-the form "Thread\-N" where N is a small decimal number.
+the form \(dqThread\-N\(dq where N is a small decimal number.
 .sp
-\fIargs\fP is the argument tuple for the target invocation. Defaults to ().
+\fIargs\fP is a list or tuple of arguments for the target invocation. Defaults to ().
 .sp
 \fIkwargs\fP is a dictionary of keyword arguments for the target
 invocation. Defaults to {}.
 .sp
 If a subclass overrides the constructor, it must make sure to invoke
 the base class constructor (Thread.__init__()) before doing anything
 else to the thread.
@@ -1122,15 +1164,15 @@
 stop the watcher
 .UNINDENT
 .UNINDENT
 .SS scingestor.scanDirWatcher module
 .INDENT 0.0
 .TP
 .B class  scingestor.scanDirWatcher.ScanDirWatcher(configuration, path, meta, beamtimefile, depth)
-Bases: \fI\%threading.Thread\fP
+Bases: \fI\%Thread\fP
 .sp
 ScanDir Watcher
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
@@ -1162,19 +1204,19 @@
 .B stop()
 stop the watcher
 .UNINDENT
 .UNINDENT
 .SS Module contents
 .INDENT 0.0
 .IP \(bu 2
-genindex
+\fI\%Index\fP
 .IP \(bu 2
-modindex
+\fI\%Module Index\fP
 .IP \(bu 2
-search
+\fI\%Search Page\fP
 .UNINDENT
 .SH AUTHOR
 Jan Kotanski
 .SH COPYRIGHT
 2022, DESY, Jan Kotanski
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `scingestor-0.8.1/scingestor/__init__.py` & `scingestor-0.9.0/scingestor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 #    along with scingestor.  If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Jan Kotanski <jan.kotanski@desy.de>
 #
 
 #: (:obj:`str`) the scingestor version
-__version__ = "0.8.1"
+__version__ = "0.9.0"
```

### Comparing `scingestor-0.8.1/scingestor/beamtimeWatcher.py` & `scingestor-0.9.0/scingestor/beamtimeWatcher.py`

 * *Files identical despite different names*

### Comparing `scingestor-0.8.1/scingestor/configuration.py` & `scingestor-0.9.0/scingestor/configuration.py`

 * *Files identical despite different names*

### Comparing `scingestor-0.8.1/scingestor/datasetIngest.py` & `scingestor-0.9.0/scingestor/datasetIngest.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,15 +262,16 @@
                 meta = ingestor.append_proposal_groups()
             try:
                 ingestor.check_list(reingest=True)
                 ingestor.clear_tmpfile()
                 if ingestor.waiting_datasets():
                     token = ingestor.get_token()
                     for scan in ingestor.waiting_datasets():
-                        ingestor.reingest(scan, token)
+                        if scan and not scan.startswith("__command__ "):
+                            ingestor.reingest(scan, token)
                 ingestor.update_from_tmpfile()
             except Exception as e:
                 get_logger().warning(str(e))
 
     def _find_bt_files(self, path, prefix, postfix):
         """ find beamtime files with given prefix and postfix in the given path
```

### Comparing `scingestor-0.8.1/scingestor/datasetIngestor.py` & `scingestor-0.9.0/scingestor/datasetIngestor.py`

 * *Files 11% similar despite different names*

```diff
@@ -144,47 +144,59 @@
         self.__ingest_attachment = False
         #: (:obj:`bool`) retry failed dataset ingestion on next event
         self.__retry_failed_dataset_ingestion = False
         #: (:obj:`bool`) retry failed attachement ingestion on next event
         self.__retry_failed_attachment_ingestion = False
         #: (:obj:`str`) metadata copy map file
         self.__copymapfile = None
+        #: (:obj:`str`) metadata group map file
+        self.__groupmapfile = None
         #: (:obj:`bool`) oned metadata flag
         self.__oned = False
+        #: (:obj:`bool`) raw groups flag
+        self.__raw_groups = False
         #: (:obj:`int`) max oned size of metadata record
         self.__max_oned_size = None
         #: (:obj:`bool`) override attachment signals flag
         self.__override = False
         #: (:obj:`bool`) log generator command flag
         self.__logcommands = False
         #: (:obj:`bool`) empty units flag
         self.__emptyunits = True
+        #: (:obj:`bool`) skip multiple datablock ingestion
+        self.__skip_multi_datablock = False
+        #: (:obj:`bool`) skip multiple attachment ingestion
+        self.__skip_multi_attachment = False
+        #: (:obj:`bool`) skip scan dataset ingestion
+        self.__skip_scan_dataset_ingestion = False
 
         #: (:obj:`int`) maximal counter value for post tries
         self.__maxcounter = 100
 
         #: (:obj:`str`) raw dataset scan postfix
         self.__scanpostfix = ".scan.json"
         #: (:obj:`str`) origin datablock scan postfix
         self.__datablockpostfix = ".origdatablock.json"
         #: (:obj:`str`) origin datablock scan postfix
         self.__attachmentpostfix = ".attachment.json"
 
         #: (:obj:`str`) nexus dataset shell command
         self.__datasetcommandfile = "nxsfileinfo metadata -k4 " \
             " -o {metapath}/{scanname}{scanpostfix} " \
+            " -z '{measurement}'" \
             " -b {beamtimefile} -p {beamtimeid}/{scanname} " \
             " -w {ownergroup}" \
             " -c {accessgroups}" \
-            " {scanpath}/{scanname}.{ext}"
+            " {masterfile}"
         #: (:obj:`str`) datablock shell command
         self.__datasetcommand = "nxsfileinfo metadata -k4 " \
             " -o {metapath}/{scanname}{scanpostfix} " \
             " -c {accessgroups}" \
             " -w {ownergroup}" \
+            " -z '{measurement}'" \
             " -b {beamtimefile} -p {beamtimeid}/{scanname}"
         #: (:obj:`str`) datablock shell command
         self.__datablockcommand = "nxsfileinfo origdatablock " \
             " -s *.pyc,*{datablockpostfix},*{scanpostfix}," \
             "*{attachmentpostfix},*~ " \
             " -p {pidprefix}{beamtimeid}/{scanname} " \
             " -w {ownergroup}" \
@@ -199,22 +211,38 @@
             " -p {pidprefix}{beamtimeid}/{scanname} "
         #: (:obj:`str`) datablock path postfix
         self.__datablockscanpath = " {scanpath}/{scanname} "
         #: (:obj:`str`) attachment shell command
         self.__attachmentcommand = "nxsfileinfo attachment " \
             " -w {ownergroup} -c {accessgroups} " \
             "-o {metapath}/{scanname}{attachmentpostfix} " \
-            " {scanpath}/{scanname}.{plotext}"
+            " {plotfile}"
+        #: (:obj:`str`) last measurement
+        self.__measurement = ""
+        #: (:obj:`bool`) measurement status
+        self.__measurement_status = False
+        #: (:obj:`bool`) call callback after each step
+        self.__callcallback = False
+        #: (:obj:`str`) metadata generated  shell callback
+        self.__metadatageneratedcallback = "nxsfileinfo groupmetadata " \
+            " {lastmeasurement} -m {metapath}/{scanname}{scanpostfix}" \
+            " -d {metapath}/{scanname}{datablockpostfix}" \
+            " -a {metapath}/{scanname}{attachmentpostfix}" \
+            " -p {beamtimeid}/{lastmeasurement} -f -k4 "
 
         #: (:obj:`str`) oned generator switch
         self.__oned_switch = " --oned "
+        #: (:obj:`str`) raw group generator switch
+        self.__raw_groups_switch = " --raw "
         #: (:obj:`str`) max oned size generator switch
         self.__max_oned_switch = " --max-oned-size {maxonedsize} "
         #: (:obj:`str`) copy map file generator switch
         self.__copymapfile_switch = " --copy-map-file {copymapfile} "
+        #: (:obj:`str`) group map file generator switch
+        self.__groupmapfile_switch = " --group-map-file {groupmapfile} "
         #: (:obj:`str`) empty units generator switch
         self.__emptyunits_switch = " --add-empty-units "
         #: (:obj:`str`) chmod generator switch
         self.__chmod_switch = " -x {chmod} "
         #: (:obj:`str`) hidden attributes generator switch
         self.__hiddenattributes_switch = " -n {hiddenattributes} "
         #: (:obj:`str`) relpath generator switch
@@ -365,16 +393,22 @@
         if "attachment_image_frame_number" in self.__config.keys():
             self.__attachmentframe = \
                 self.__config["attachment_image_frame_number"]
         if "metadata_copy_map_file" in self.__config.keys():
             self.__copymapfile = \
                 self.__config["metadata_copy_map_file"].format(
                     homepath=self.__homepath)
+        if "metadata_group_map_file" in self.__config.keys():
+            self.__groupmapfile = \
+                self.__config["metadata_group_map_file"].format(
+                    homepath=self.__homepath)
         if "oned_in_metadata" in self.__config.keys():
             self.__oned = self.__config["oned_in_metadata"]
+        if "raw_metadata_callback" in self.__config.keys():
+            self.__raw_groups = self.__config["raw_metadata_callback"]
         if "max_oned_size" in self.__config.keys():
             self.__max_oned_size = self.__config["max_oned_size"]
         if "override_attachment_signals" in self.__config.keys():
             self.__override = self.__config["override_attachment_signals"]
         if "log_generator_commands" in self.__config.keys():
             self.__logcommands = self.__config["log_generator_commands"]
         if "ingest_dataset_attachment" in self.__config.keys():
@@ -385,14 +419,24 @@
                 self.__config["retry_failed_dataset_ingestion"]
         if "retry_failed_attachment_ingestion" in self.__config.keys():
             self.__retry_failed_attachment_ingestion = \
                 self.__config["retry_failed_attachment_ingestion"]
         if "add_empty_units" in self.__config.keys():
             self.__emptyunits = self.__config["add_empty_units"]
 
+        if "skip_multi_datablock_ingestion" in self.__config.keys():
+            self.__skip_multi_datablock = \
+                self.__config["skip_multi_datablock_ingestion"]
+        if "skip_multi_attachment_ingestion" in self.__config.keys():
+            self.__skip_multi_attachment = \
+                self.__config["skip_multi_attachment_ingestion"]
+        if "skip_scan_dataset_ingestion" in self.__config.keys():
+            self.__skip_scan_dataset_ingestion = \
+                self.__config["skip_scan_dataset_ingestion"]
+
         if "scan_metadata_postfix" in self.__config.keys():
             self.__scanpostfix = self.__config["scan_metadata_postfix"]
         if "datablock_metadata_postfix" in self.__config.keys():
             self.__datablockpostfix = \
                 self.__config["datablock_metadata_postfix"]
         if "attachment_metadata_postfix" in self.__config.keys():
             self.__attachmentpostfix = \
@@ -414,14 +458,22 @@
            in self.__config.keys():
             self.__datablockscanpath = \
                 self.__config["datablock_metadata_generator_scanpath_postfix"]
         if "attachment_metadata_generator" in self.__config.keys():
             self.__attachmentcommand = \
                 self.__config["attachment_metadata_generator"]
 
+        if "call_metadata_generated_callback" in self.__config.keys():
+            self.__callcallback = bool(
+                self.__config["call_metadata_generated_callback"])
+
+        if "metadata_generated_callback" in self.__config.keys():
+            self.__metadatageneratedcallback = \
+                self.__config["metadata_generated_callback"]
+
         if "chmod_generator_switch" in self.__config.keys():
             self.__chmod_switch = \
                 self.__config["chmod_generator_switch"]
 
         if "hidden_attributes_generator_switch" in self.__config.keys():
             self.__hiddenattributes_switch = \
                 self.__config["hidden_attributes_generator_switch"]
@@ -438,22 +490,30 @@
             self.__attachmentframe_switch = \
                 self.__config["attachment_frame_generator_switch"]
 
         if "metadata_copy_map_file_generator_switch" in self.__config.keys():
             self.__copymapfile_switch = \
                 self.__config["metadata_copy_map_file_generator_switch"]
 
+        if "metadata_group_map_file_generator_switch" in self.__config.keys():
+            self.__groupmapfile_switch = \
+                self.__config["metadata_group_map_file_generator_switch"]
+
         if "relative_path_generator_switch" in self.__config.keys():
             self.__relpath_switch = \
                 self.__config["relative_path_generator_switch"]
 
         if "oned_dataset_generator_switch" in self.__config.keys():
             self.__oned_switch = \
                 self.__config["oned_dataset_generator_switch"]
 
+        if "raw_metadata_callback_switch" in self.__config.keys():
+            self.__raw_groups_switch = \
+                self.__config["raw_metadata_callback_switch"]
+
         if "max_oned_dataset_generator_switch" in self.__config.keys():
             self.__max_oned_switch = \
                 self.__config["max_oned_dataset_generator_switch"]
 
         if "override_attachment_signals_generator_switch" \
                 in self.__config.keys():
             self.__attachmentoverride_switch = \
@@ -492,14 +552,29 @@
             if "datablock_metadata_stream_generator" \
                not in self.__config.keys():
                 self.__datablockmemcommand = \
                     self.__datablockmemcommand + self.__chmod_switch
             if "attachment_metadata_generator" not in self.__config.keys():
                 self.__attachmentcommand = \
                     self.__attachmentcommand + self.__chmod_switch
+            if "metadata_generated_callback" not in self.__config.keys():
+                self.__metadatageneratedcallback = \
+                    self.__metadatageneratedcallback + self.__chmod_switch
+
+        if self.__groupmapfile is not None:
+            if "metadata_generated_callback" not in self.__config.keys():
+                self.__metadatageneratedcallback = \
+                    self.__metadatageneratedcallback + \
+                    self.__groupmapfile_switch
+
+        if self.__raw_groups:
+            if "metadata_generated_callback" not in self.__config.keys():
+                self.__metadatageneratedcallback = \
+                    self.__metadatageneratedcallback + \
+                    self.__raw_groups_switch
 
         if self.__hiddenattributes is not None:
             if "dataset_metadata_generator" not in self.__config.keys():
                 self.__datasetcommand = \
                     self.__datasetcommand + self.__hiddenattributes_switch
             if "file_dataset_metadata_generator" not in self.__config.keys():
                 self.__datasetcommandfile = \
@@ -578,14 +653,16 @@
 
         #: (:obj:`dict` <:obj:`str`, :obj:`str`>) command format parameters
         self.__dctfmt = {
             "scanname": None,
             "chmod": self.__chmod,
             "hiddenattributes": self.__hiddenattributes,
             "copymapfile": self.__copymapfile,
+            "plotfile": "",
+            "masterfile": "",
             "scanpath": self.__path,
             "metapath": self.__metapath,
             "relpath": self.__relpath,
             "beamtimeid": self.__bid,
             "beamline": self.__bl,
             "pidprefix": self.__pidprefix,
             "beamtimefile": self.__bfile,
@@ -598,15 +675,23 @@
             "homepath": self.__homepath,
             "ext": self.__ext,
             "plotext": self.__plotext,
             "signals": self.__attachmentsignals,
             "axes": self.__attachmentaxes,
             "frame": self.__attachmentframe,
             "maxonedsize": self.__max_oned_size,
+            "measurement": self.__measurement,
+            "lastmeasurement": self.__measurement,
+            "groupmapfile": self.__groupmapfile,
+
         }
+        self.__dctfmt["masterfile"] = \
+            "{scanpath}/{scanname}.{ext}".format(**self.__dctfmt)
+        self.__dctfmt["plotfile"] = \
+            "{scanpath}/{scanname}.{plotext}".format(**self.__dctfmt)
 
         get_logger().debug(
             'DatasetIngestor: Parameters: %s' % str(self.__dctfmt))
 
         # self.__tokenurl = "http://www-science3d.desy.de:3000/api/v3/" \
         #       "Users/login"
         if not self.__scicat_url.endswith("/"):
@@ -643,21 +728,38 @@
         :param scan: scan name
         :type scan: :obj:`str`
         :returns: a file name of generate file
         :rtype: :obj:`str`
         """
         self.__ext = ""
 
+        self.__dctfmt["masterfile"] = \
+            "{scanpath}/{scanname}/{scanname}.{ext}".format(**self.__dctfmt)
         for ext in self.__master_file_extension_list:
             self.__dctfmt["ext"] = ext
 
             if os.path.isfile(
                     "{scanpath}/{scanname}.{ext}".format(**self.__dctfmt)):
                 self.__ext = ext
+                self.__dctfmt["masterfile"] = \
+                    "{scanpath}/{scanname}.{ext}".format(**self.__dctfmt)
                 break
+        else:
+            for ext in self.__master_file_extension_list:
+                self.__dctfmt["ext"] = ext
+
+                if os.path.isfile(
+                        "{scanpath}/{scanname}/{scanname}.{ext}".
+                        format(**self.__dctfmt)):
+                    self.__ext = ext
+                    self.__dctfmt["masterfile"] = \
+                        "{scanpath}/{scanname}/{scanname}.{ext}".format(
+                            **self.__dctfmt)
+                    break
+
         self.__dctfmt["ext"] = self.__ext
 
         if self.__ext:
             get_logger().info(
                 'DatasetIngestor: Generating %s metadata: %s %s' % (
                     self.__ext, scan,
                     "{metapath}/{scanname}{scanpostfix}".format(
@@ -734,21 +836,37 @@
         :param scan: scan name
         :type scan: :obj:`str`
         :returns: a file name of generate file
         :rtype: :obj:`str`
         """
         self.__plotext = ""
 
+        self.__dctfmt["plotfile"] = \
+            "{scanpath}/{scanname}.{plotext}".format(**self.__dctfmt)
         for ext in self.__plot_file_extension_list:
             self.__dctfmt["plotext"] = ext
 
             if os.path.isfile(
                     "{scanpath}/{scanname}.{plotext}".format(**self.__dctfmt)):
                 self.__plotext = ext
+                self.__dctfmt["plotfile"] = \
+                    "{scanpath}/{scanname}.{plotext}".format(**self.__dctfmt)
                 break
+        else:
+            for ext in self.__plot_file_extension_list:
+                self.__dctfmt["plotext"] = ext
+
+                if os.path.isfile(
+                        "{scanpath}/{scanname}/{scanname}.{plotext}".
+                        format(**self.__dctfmt)):
+                    self.__plotext = ext
+                    self.__dctfmt["plotfile"] = \
+                        "{scanpath}/{scanname}/{scanname}.{plotext}".format(
+                            **self.__dctfmt)
+                    break
         self.__dctfmt["plotext"] = self.__plotext
 
         if self.__dctfmt["plotext"]:
             get_logger().info(
                 'DatasetIngestor: Generating attachment metadata: %s %s' % (
                     scan,
                     "{metapath}/{scanname}{attachmentpostfix}".format(
@@ -1328,15 +1446,15 @@
         :returns: dataset id
         :rtype: :obj:`str`
         """
         try:
             with open(metafile) as fl:
                 smt = fl.read()
                 mt = json.loads(smt)
-            if mt["proposalId"] != self.__bid:
+            if mt["type"] == "raw" and mt["proposalId"] != self.__bid:
                 raise Exception(
                     "Wrong SC proposalId %s for DESY beamtimeId %s in %s"
                     % (mt["proposalId"], self.__bid, metafile))
             if not mt['pid'] or \
                not mt["pid"].startswith("%s/" % (self.__bid)):
                 raise Exception(
                     "Wrong pid %s for DESY beamtimeId %s in  %s"
@@ -1467,55 +1585,84 @@
         odbs = glob.glob(
             "{metapath}/{scan}{postfix}".format(
                 scan=self.__dctfmt["scanname"],
                 postfix=self.__datablockpostfix,
                 metapath=self.__dctfmt["metapath"]))
         if odbs and odbs[0]:
             odb = odbs[0]
+            todb = [odb]
+            with open(odb) as fl:
+                dbmt = json.loads(fl.read())
+                if isinstance(dbmt, list):
+                    if self.__skip_multi_datablock:
+                        todb = []
+                    else:
+                        todb = dbmt
         else:
             odb = self._generate_origdatablock_metadata(scan)
+            todb = [odb]
         mtmdb = 0
         if odb:
             mtmdb = os.path.getmtime(odb)
+        mtmda = 0
         if self.__ingest_attachment:
             adss = glob.glob(
                 "{metapath}/{scan}{postfix}".format(
                     scan=self.__dctfmt["scanname"],
                     postfix=self.__attachmentpostfix,
                     metapath=self.__dctfmt["metapath"]))
             if adss and adss[0]:
                 ads = adss[0]
+                tads = [ads]
+                with open(ads) as fl:
+                    admt = json.loads(fl.read())
+                    if isinstance(admt, list):
+                        if self.__skip_multi_attachment:
+                            tads = []
+                        else:
+                            tads = admt
             else:
                 ads = self._generate_attachment_metadata(
                     self.__dctfmt["scanname"])
+                tads = [ads]
             if ads:
                 mtmda = os.path.getmtime(ads)
 
+        if (self.__callcallback or self.__measurement_status) \
+           and self.__metadatageneratedcallback \
+           and rds and odb:
+            command = self.__metadatageneratedcallback.format(**self.__dctfmt)
+            get_logger().info(
+                'DatasetIngestor: Metadata generated callback: %s ' % (
+                    command))
+            subprocess.run(command, shell=True, check=True)
         dbstatus = None
         dastatus = None
         pid = None
-        if rds and odb:
+        if rds and odb and not self.__skip_scan_dataset_ingestion:
             if rds and rds[0]:
                 pid = self._ingest_rawdataset_metadata(rds, token)
-            if odb and odb[0] and pid:
+            if todb and todb[0] and pid:
                 if pid is None and rdss and rdss[0]:
                     pid = self._get_pid(rdss[0])
-                dbstatus = self._ingest_origdatablock_metadata(
-                    odb, pid, token)
-                if not dbstatus:
-                    mtmdb = -1
+                for odb in todb:
+                    dbstatus = self._ingest_origdatablock_metadata(
+                        odb, pid, token)
+                    if not dbstatus:
+                        mtmdb = -1
             if pid is None and rdss and rdss[0]:
                 pid = self._get_pid(rdss[0])
-            if self.__ingest_attachment and ads and ads[0] and pid:
-                if pid is None and adss and adss[0]:
+            if self.__ingest_attachment and tads and tads[0] and pid:
+                if pid is None and rdss and rdss[0]:
                     pid = self._get_pid(rdss[0])
-                dastatus = self._ingest_attachment_metadata(
-                    ads, pid, token)
-                if not dastatus:
-                    mtmda = -1
+                for ads in tads:
+                    dastatus = self._ingest_attachment_metadata(
+                        ads, pid, token)
+                    if not dastatus:
+                        mtmda = -1
         if pid is None:
             if scan in self.__sc_seingested_map.keys():
                 mtmds = self.__sc_seingested_map[scan][-3]
             else:
                 mtmds = 0
         if dbstatus is None:
             if scan in self.__sc_seingested_map.keys():
@@ -1795,7 +1942,28 @@
     def ingested_datasets(self):
         """ provides ingested datasets
 
         :returns:  ingested datasets list
         :rtype: :obj:`list` <:obj:`str`>
         """
         return list(self.__sc_ingested)
+
+    def stop_measurement(self):
+        """ stop measurement
+
+        """
+        self.__measurement_status = False
+        self.__dctfmt["measurement"] = ""
+        get_logger().debug("Stop Measurement: %s" % self.__measurement)
+
+    def start_measurement(self, measurement):
+        """ start measurement
+
+        :param measurement:  measurement name
+        :type measurement: :obj:`str`
+
+        """
+        self.__measurement = measurement
+        self.__dctfmt["measurement"] = self.__measurement
+        self.__dctfmt["lastmeasurement"] = self.__measurement
+        self.__measurement_status = True
+        get_logger().debug("Start Measurement: %s" % self.__measurement)
```

### Comparing `scingestor-0.8.1/scingestor/datasetWatcher.py` & `scingestor-0.9.0/scingestor/datasetWatcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,20 +70,28 @@
 
         #: (:obj:`bool`) use core path
         self.__usecorepath = False
         if "use_corepath_as_scandir" in self.__config.keys():
             self.__usecorepath = bool(
                 self.__config["use_corepath_as_scandir"])
 
+        #: (:obj:`bool`) execute command
+        self.__executecommands = False
+        if "execute_commands" in self.__config.keys():
+            self.__executecommands = bool(
+                self.__config["execute_commands"])
+
         #: (:class:`scingestor.datasetWatcher.DatasetWatcher`) use core path
         self.__conv = PathConverter(
             self.__corepath, self.__bpath,
             self.__usecorepath and self.__corepath)
 
         #: (:obj:`str`) file with a dataset list
+        self.__measurement_name = ""
+        #: (:obj:`str`) file with a dataset list
         self.__dsfile = dsfile
         #: (:obj:`str`) file with a ingested dataset list
         self.__idsfile = idsfile
         #: (:obj:`float`) delay time for ingestion in s
         self.__delay = 5
         #: (:obj:`int`) notifier ID
         self.__notifier = None
@@ -184,15 +192,28 @@
         if self.__ingestor.waiting_datasets():
             time.sleep(self.__delay)
         if self.__ingestor.waiting_datasets():
             try:
                 token = self.__ingestor.get_token()
                 if token:
                     for scan in self.__ingestor.waiting_datasets():
-                        self.__ingestor.ingest(scan, token)
+                        if scan and scan.startswith("__command__ "):
+                            if self.__executecommands:
+                                sscan = scan.split(" ")
+                                if len(sscan) > 1:
+                                    cmd = sscan[1]
+                                    if cmd == "stop":
+                                        self.__ingestor.stop_measurement()
+                                    if cmd == "start":
+                                        if len(sscan) > 2:
+                                            groupname = sscan[2]
+                                        self.__ingestor.start_measurement(
+                                            groupname)
+                        else:
+                            self.__ingestor.ingest(scan, token)
                     self.__ingestor.clear_waiting_datasets()
             except Exception as e:
                 get_logger().warning(str(e))
 
         counter = 0
         try:
             while self.running:
@@ -279,19 +300,32 @@
                     try:
                         token = self.__ingestor.get_token()
                     except Exception as e:
                         get_logger().warning(str(e))
                         continue
                     if token:
                         for scan in self.__ingestor.waiting_datasets():
-                            try:
-                                self.__ingestor.ingest(scan, token)
-                            except Exception as e:
-                                get_logger().warning(str(e))
-                                continue
+                            if scan and scan.startswith("__command__ "):
+                                if self.__executecommands:
+                                    sscan = scan.split(" ")
+                                    if len(sscan) > 1:
+                                        cmd = sscan[1]
+                                        if cmd == "stop":
+                                            self.__ingestor.stop_measurement()
+                                        if cmd == "start":
+                                            if len(sscan) > 2:
+                                                groupname = sscan[2]
+                                            self.__ingestor.start_measurement(
+                                                groupname)
+                            else:
+                                try:
+                                    self.__ingestor.ingest(scan, token)
+                                except Exception as e:
+                                    get_logger().warning(str(e))
+                                    continue
                         self.__ingestor.clear_waiting_datasets()
                 # else:
                 #     time.sleep(self.__timeout)
         finally:
             self.stop()
 
     def stop(self):
```

### Comparing `scingestor-0.8.1/scingestor/logger.py` & `scingestor-0.9.0/scingestor/logger.py`

 * *Files identical despite different names*

### Comparing `scingestor-0.8.1/scingestor/modelIngest.py` & `scingestor-0.9.0/scingestor/modelIngest.py`

 * *Files identical despite different names*

### Comparing `scingestor-0.8.1/scingestor/pathConverter.py` & `scingestor-0.9.0/scingestor/pathConverter.py`

 * *Files identical despite different names*

### Comparing `scingestor-0.8.1/scingestor/safeINotifier.py` & `scingestor-0.9.0/scingestor/safeINotifier.py`

 * *Files identical despite different names*

### Comparing `scingestor-0.8.1/scingestor/scanDirWatcher.py` & `scingestor-0.9.0/scingestor/scanDirWatcher.py`

 * *Files identical despite different names*

### Comparing `scingestor-0.8.1/scingestor.egg-info/PKG-INFO` & `scingestor-0.9.0/scingestor.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scingestor
-Version: 0.8.1
+Version: 0.9.0
 Summary: Scientific Catalog Tools
 Home-page: http://github.com/jkotan/scingestor
 Author: ('Jan Kotanski',)
 Author-email: jankotan@gmail.com
 Maintainer: Jan Kotanski
 Maintainer-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE, version 3
@@ -43,20 +43,30 @@
         * **attachment_metadata_postfix** *(str)* , default: `".attachment.json"`
         * **metadata_in_var_dir** *(bool)* , default: `False`
         * **use_corepath_as_scandir** *(bool)* , default: `False`
         * **beamtime_filename_postfix** *(str)* , default: `"beamtime-metadata-"`
         * **beamtime_filename_prefix** *(str)* , default: `".json"`
         * **datasets_filename_pattern** *(str)* , default: `"scicat-datasets-{beamtimeid}.lst"`
         * **ingested_datasets_filename_pattern** *(str)* , default: `"scicat-ingested-datasets-{beamtimeid}.lst"`
-        * **file_dataset_metadata_generator** *(str)* , default: `"nxsfileinfo metadata -k4  -o {metapath}/{scanname}{scanpostfix}  -b {beamtimefile} -p {beamtimeid}/{scanname}  -w {ownergroup} -c {accessgroups} {scanpath}/{scanname}.{ext}"`
+        * **file_dataset_metadata_generator** *(str)* , default: `"nxsfileinfo metadata -k4  -o {metapath}/{scanname}{scanpostfix}  -b {beamtimefile} -p {beamtimeid}/{scanname}  -w {ownergroup} -c {accessgroups} {mastefile}"`
         * **dataset_metadata_generator** *(str)* , default: `"nxsfileinfo metadata -k4  -o {metapath}/{scanname}{scanpostfix}  -c {accessgroups} -w {ownergroup} -b {beamtimefile} -p {beamtimeid}/{scanname}"`
         * **datablock_metadata_generator** *(str)* , default: `"nxsfileinfo origdatablock  -s *.pyc,*{datablockpostfix},*{scanpostfix},*~  -p {pidprefix}{beamtimeid}/{scanname}  -w {ownergroup} -c {accessgroups} -o {metapath}/{scanname}{datablockpostfix} "`
         * **datablock_metadata_stream_generator** *(str)* , default: `"nxsfileinfo origdatablock  -s *.pyc,*{datablockpostfix},*{scanpostfix},*~  -w {ownergroup} -c {accessgroups} -p {pidprefix}{beamtimeid}/{scanname} "`
         * **datablock_metadata_generator_scanpath_postfix** *(str)* , default: `" {scanpath}/{scanname} "`
-        * **attachment_metadata_generator** *(str)* , default: `"nxsfileinfo attachment  -w {ownergroup} -c {accessgroups} -o {metapath}/{scanname}{attachmentpostfix} "`
+        * **attachment_metadata_generator** *(str)* , default: `"nxsfileinfo attachment  -w {ownergroup} -c {accessgroups} -o {metapath}/{scanname}{attachmentpostfix} {plotfile} "`
+        * **metadata_generated_callback** *(str)* , default: `"nxsfileinfo groupmetadata  {lastmeasurement} -m {metapath}/{scanname}{scanpostfix} -d {metapath}/{scanname}{datablockpostfix} -a {metapath}/{scanname}{attachmentpostfix} -p {beamtimeid}/{lastmeasurement} -f -k4 "`
+        * **metadata_group_map_file** *(str)* , default: `""`
+        * **raw_metadata_callback** *(bool)* , default: `False`
+        * **skip_multi_datablock_ingestion** *(bool)* , default: `False`
+        * **skip_multi_attachment_ingestion** *(bool)* , default: `False`
+        * **skip_scan_dataset_ingestion** *(bool)* , default: `False`
+        * **call_metadata_generated_callback** *(bool)* , default: `False`
+        * **metadata_group_map_file_generator_switch** *(str)* , default: `" --group-map-file {groupmapfile} "`
+        * **raw_metadata_callback_switch** *(str)* , default: `" --raw "`
+        * **execute_commands** *(bool)* , default: `False`
         * **plot_file_extension_list** *(list\<str\>)* , default: `["png", "nxs", "h5", "ndf", "nx", "fio"]`
         * **master_file_extension_list** *(list\<str\>)* , default: `["nxs", "h5", "ndf", "nx", "fio"]`
         * **chmod_generator_switch** *(str)* , default: `" -x {chmod} "`
         * **relative_path_generator_switch** *(str)* , default: `" -r {relpath} "`
         * **oned_dataset_generator_switch** *(str)* , default: `" --oned "`
         * **max_oned_dataset_generator_switch** *(str)* , default: `" --max-oned-size {maxonedsize} "`
         * **override_attachment_signals_generator_switch** *(bool)* , default: `" --override "`
@@ -103,16 +113,18 @@
         
         ### Pattern keywords for configuration variables
         
         The  **datasets_filename_pattern**, **ingested_datasets_filename_pattern**  and **ingestor_var_dir** can contain the *{beamtimeid}* and *{hostname}* keywords,  e.g. `"scicat-ingested-datasets-{beamtimeid}.lst"` or `"scicat-ingested-datasets-{hostname}-{beamtimeid}.lst"` which is instantiated during the ingestor execution.
         
         The  **beamtime_dirs**, **beamtime_base_dir**, **ingestor_var_dir**, **ingestor_credential_file**, **scandir_blacklist** can contain the *{homepath}* keyword.
         
-        Similarly, **file_dataset_metadata_generator**, **dataset_metadata_generator**, **datablock_metadata_generator**,  **datablock_metadata_stream_generator**, **datablock_metadata_generator_scanpath_postfix**, **attachment_metadata_generator**, **chmod_generator_switch**, **relative_path_generator_switch** can contain the following keywords: *{beamtimeid}* , *{scanname}*, *{chmod}*, *{scanpath}*, *{metapath}*, *{relpath}*, *{beamtimeid}*, *{beamline}*, *{pidprefix}*, *{beamtimefile}*, *{scanpostfix}*, *{datablockpostfix}*, *{ownergroup}*, *{accessgroups}*, *{hostname}*, *{homepath}*, *{hiddenattributes}*, *{ext}*
+        Similarly, **file_dataset_metadata_generator**, **dataset_metadata_generator**, **datablock_metadata_generator**,  **datablock_metadata_stream_generator**, **datablock_metadata_generator_scanpath_postfix**, **attachment_metadata_generator**, **chmod_generator_switch**, **relative_path_generator_switch** can contain the following keywords: *{beamtimeid}* , *{scanname}*, *{chmod}*, *{scanpath}*, *{metapath}*, *{relpath}*, *{beamtimeid}*, *{beamline}*, *{pidprefix}*, *{beamtimefile}*, *{scanpostfix}*, *{datablockpostfix}*, *{ownergroup}*, *{accessgroups}*, *{hostname}*, *{homepath}*, *{hiddenattributes}*, *{ext}*, "{masterfile}", "{plotfile}"
         
+        The "{masterfile}" is either equal to   "{scanpath}/{scanname}.{ext}" or "{scanpath}/{scanname}/{scanname}.{ext}". Also
+        the "{plotfile}" is either equal to  "{scanpath}/{scanname}.{plotext}" or "{scanpath}/{scanname}/{scanname}.{plotext}".
         
         
         ## scicat_dataset_ingest
         
         Re-ingestion script for SciCat Datasets and OrigDatablocks is usually launched at the end of the beamtime.
         ```
         scicat_dataset_ingest -c ~/.scingestor.yaml
```

### Comparing `scingestor-0.8.1/scingestor.egg-info/SOURCES.txt` & `scingestor-0.9.0/scingestor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scingestor-0.8.1/setup.py` & `scingestor-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 IPKG = __import__(PKG)
 
 needs_pytest = set(['test']).intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if needs_pytest else []
 
 install_requires = [
     'argcomplete',
-    'nxstools>=3.48.0',
+    'nxstools>=3.52.0',
     'requests',
     'pyyaml',
     'h5py',
     # 'inotify-py3',
     # 'pytest',
     # 'sphinx',
 ]
```


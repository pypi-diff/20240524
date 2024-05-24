# Comparing `tmp/keycare-0.0.7.tar.gz` & `tmp/keycare-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycare-0.0.7.tar", last modified: Fri May 24 10:29:29 2024, max compression
+gzip compressed data, was "keycare-0.0.8.tar", last modified: Fri May 24 10:37:12 2024, max compression
```

## Comparing `keycare-0.0.7.tar` & `keycare-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:29:29.575306 keycare-0.0.7/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1068 2023-07-28 11:11:56.000000 keycare-0.0.7/LICENSE
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7593 2024-05-24 10:29:29.559863 keycare-0.0.7/PKG-INFO
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     4805 2024-05-24 09:25:31.000000 keycare-0.0.7/README.md
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:29:28.979484 keycare-0.0.7/keycare/
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:29:29.193464 keycare-0.0.7/keycare/keycare/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     4912 2024-02-29 17:21:47.000000 keycare-0.0.7/keycare/keycare/RelExtractor.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)    10195 2024-05-22 15:42:46.000000 keycare-0.0.7/keycare/keycare/TermExtractor.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.7/keycare/keycare/__init__.py
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:29:29.532385 keycare-0.0.7/keycare/keycare.egg-info/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7593 2024-05-24 10:29:28.000000 keycare-0.0.7/keycare/keycare.egg-info/PKG-INFO
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)      319 2024-05-24 10:29:28.000000 keycare-0.0.7/keycare/keycare.egg-info/SOURCES.txt
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)        1 2024-05-24 10:29:28.000000 keycare-0.0.7/keycare/keycare.egg-info/dependency_links.txt
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)      369 2024-05-24 10:29:28.000000 keycare-0.0.7/keycare/keycare.egg-info/requires.txt
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)        8 2024-05-24 10:29:28.000000 keycare-0.0.7/keycare/keycare.egg-info/top_level.txt
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1643 2024-05-24 10:28:16.000000 keycare-0.0.7/pyproject.toml
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)       38 2024-05-24 10:29:29.577814 keycare-0.0.7/setup.cfg
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:37:12.162349 keycare-0.0.8/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1068 2023-07-28 11:11:56.000000 keycare-0.0.8/LICENSE
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7593 2024-05-24 10:37:12.141926 keycare-0.0.8/PKG-INFO
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     4805 2024-05-24 09:25:31.000000 keycare-0.0.8/README.md
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:37:11.430508 keycare-0.0.8/keycare/
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:37:11.700497 keycare-0.0.8/keycare/keycare/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     4912 2024-02-29 17:21:47.000000 keycare-0.0.8/keycare/keycare/RelExtractor.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)    10195 2024-05-22 15:42:46.000000 keycare-0.0.8/keycare/keycare/TermExtractor.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.8/keycare/keycare/__init__.py
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:37:12.100161 keycare-0.0.8/keycare/keycare.egg-info/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7593 2024-05-24 10:37:11.000000 keycare-0.0.8/keycare/keycare.egg-info/PKG-INFO
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)      319 2024-05-24 10:37:11.000000 keycare-0.0.8/keycare/keycare.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)        1 2024-05-24 10:37:11.000000 keycare-0.0.8/keycare/keycare.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)      369 2024-05-24 10:37:11.000000 keycare-0.0.8/keycare/keycare.egg-info/requires.txt
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)        1 2024-05-24 10:37:11.000000 keycare-0.0.8/keycare/keycare.egg-info/top_level.txt
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1646 2024-05-24 10:36:39.000000 keycare-0.0.8/pyproject.toml
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)       38 2024-05-24 10:37:12.170455 keycare-0.0.8/setup.cfg
```

### Comparing `keycare-0.0.7/LICENSE` & `keycare-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `keycare-0.0.7/PKG-INFO` & `keycare-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycare
-Version: 0.0.7
+Version: 0.0.8
 Summary: KeyCARE is a Python library designed for the unsupervised keyword extraction from biomedical documents with the use of different algorithms, the classification of the keywords according to their semantic nature, and the extraction of is a relations among those keywords and with other terminologies.
 Author-email: Sergi Marsol <sergimarsolt@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 nlp4bia-bsc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: keycare Version: 0.0.7 Summary: KeyCARE is a Python
+Metadata-Version: 2.1 Name: keycare Version: 0.0.8 Summary: KeyCARE is a Python
 library designed for the unsupervised keyword extraction from biomedical
 documents with the use of different algorithms, the classification of the
 keywords according to their semantic nature, and the extraction of is a
 relations among those keywords and with other terminologies. Author-email:
 Sergi Marsol
 gmail.com> License: MIT License Copyright (c) 2023 nlp4bia-bsc Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
```

### Comparing `keycare-0.0.7/README.md` & `keycare-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `keycare-0.0.7/keycare/keycare/RelExtractor.py` & `keycare-0.0.8/keycare/keycare/RelExtractor.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.7/keycare/keycare/TermExtractor.py` & `keycare-0.0.8/keycare/keycare/TermExtractor.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.7/keycare/keycare.egg-info/PKG-INFO` & `keycare-0.0.8/keycare/keycare.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycare
-Version: 0.0.7
+Version: 0.0.8
 Summary: KeyCARE is a Python library designed for the unsupervised keyword extraction from biomedical documents with the use of different algorithms, the classification of the keywords according to their semantic nature, and the extraction of is a relations among those keywords and with other terminologies.
 Author-email: Sergi Marsol <sergimarsolt@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 nlp4bia-bsc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: keycare Version: 0.0.7 Summary: KeyCARE is a Python
+Metadata-Version: 2.1 Name: keycare Version: 0.0.8 Summary: KeyCARE is a Python
 library designed for the unsupervised keyword extraction from biomedical
 documents with the use of different algorithms, the classification of the
 keywords according to their semantic nature, and the extraction of is a
 relations among those keywords and with other terminologies. Author-email:
 Sergi Marsol
 gmail.com> License: MIT License Copyright (c) 2023 nlp4bia-bsc Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
```

### Comparing `keycare-0.0.7/pyproject.toml` & `keycare-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
     "setuptools>=69.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["keycare"]
-include = ["keycare"]
+include = ["keycare/**"]
 exclude = ["tests"]
 
 [project]
 name = "keycare"
-version = "0.0.7"
+version = "0.0.8"
 description = "KeyCARE is a Python library designed for the unsupervised keyword extraction from biomedical documents with the use of different algorithms, the classification of the keywords according to their semantic nature, and the extraction of is a relations among those keywords and with other terminologies."
 readme = "README.md"
 authors = [{ name = "Sergi Marsol", email = "sergimarsolt@gmail.com" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 dependencies = [
     "datasets==2.14.4",
```


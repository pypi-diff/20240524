# Comparing `tmp/keycare-0.0.6.tar.gz` & `tmp/keycare-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycare-0.0.6.tar", last modified: Fri May 24 10:23:57 2024, max compression
+gzip compressed data, was "keycare-0.0.7.tar", last modified: Fri May 24 10:29:29 2024, max compression
```

## Comparing `keycare-0.0.6.tar` & `keycare-0.0.7.tar`

### file list

```diff
@@ -1,36 +1,17 @@
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:23:57.929012 keycare-0.0.6/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1068 2023-07-28 11:11:56.000000 keycare-0.0.6/LICENSE
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7593 2024-05-24 10:23:57.908789 keycare-0.0.6/PKG-INFO
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     4805 2024-05-24 09:25:31.000000 keycare-0.0.6/README.md
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:23:56.493732 keycare-0.0.6/keycare/
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:23:56.967969 keycare-0.0.6/keycare/categorizers/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     5858 2024-02-29 17:21:47.000000 keycare-0.0.6/keycare/categorizers/Categorizer.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     4395 2024-02-29 17:21:47.000000 keycare-0.0.6/keycare/categorizers/Clustering.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     5107 2024-05-22 17:26:21.000000 keycare-0.0.6/keycare/categorizers/SetFitClassifier.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7960 2024-05-22 17:26:43.000000 keycare-0.0.6/keycare/categorizers/TransformersClassifier.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.6/keycare/categorizers/__init__.py
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:23:57.237361 keycare-0.0.6/keycare/extractors/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7082 2024-02-29 17:21:47.000000 keycare-0.0.6/keycare/extractors/Extractor.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2909 2024-05-22 15:44:07.000000 keycare-0.0.6/keycare/extractors/KeyBertExtractor.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1706 2024-02-29 17:21:47.000000 keycare-0.0.6/keycare/extractors/RakeExtractor.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1631 2024-02-29 17:21:47.000000 keycare-0.0.6/keycare/extractors/TextRankExtractor.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1503 2024-02-29 17:21:47.000000 keycare-0.0.6/keycare/extractors/YakeExtractor.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.6/keycare/extractors/__init__.py
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:23:57.874734 keycare-0.0.6/keycare/keycare.egg-info/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7593 2024-05-24 10:23:56.000000 keycare-0.0.6/keycare/keycare.egg-info/PKG-INFO
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)      862 2024-05-24 10:23:56.000000 keycare-0.0.6/keycare/keycare.egg-info/SOURCES.txt
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)        1 2024-05-24 10:23:56.000000 keycare-0.0.6/keycare/keycare.egg-info/dependency_links.txt
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)      369 2024-05-24 10:23:56.000000 keycare-0.0.6/keycare/keycare.egg-info/requires.txt
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)        1 2024-05-24 10:23:56.000000 keycare-0.0.6/keycare/keycare.egg-info/top_level.txt
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:23:57.635345 keycare-0.0.6/keycare/relators/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)      517 2024-02-29 17:21:47.000000 keycare-0.0.6/keycare/relators/Relator.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2147 2024-05-22 17:27:08.000000 keycare-0.0.6/keycare/relators/SetFitRelator.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2596 2024-05-22 17:27:22.000000 keycare-0.0.6/keycare/relators/TransformersRelator.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.6/keycare/relators/__init__.py
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:23:57.692419 keycare-0.0.6/keycare/tests/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1495 2024-05-17 10:51:38.000000 keycare-0.0.6/keycare/tests/termextractor_pipeline.py
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:23:57.802045 keycare-0.0.6/keycare/utils/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.6/keycare/utils/__init__.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2355 2024-02-29 17:21:47.000000 keycare-0.0.6/keycare/utils/data_structures.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1643 2024-05-24 10:23:45.000000 keycare-0.0.6/pyproject.toml
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)       38 2024-05-24 10:23:57.929012 keycare-0.0.6/setup.cfg
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:29:29.575306 keycare-0.0.7/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1068 2023-07-28 11:11:56.000000 keycare-0.0.7/LICENSE
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7593 2024-05-24 10:29:29.559863 keycare-0.0.7/PKG-INFO
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     4805 2024-05-24 09:25:31.000000 keycare-0.0.7/README.md
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:29:28.979484 keycare-0.0.7/keycare/
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:29:29.193464 keycare-0.0.7/keycare/keycare/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     4912 2024-02-29 17:21:47.000000 keycare-0.0.7/keycare/keycare/RelExtractor.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)    10195 2024-05-22 15:42:46.000000 keycare-0.0.7/keycare/keycare/TermExtractor.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.7/keycare/keycare/__init__.py
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:29:29.532385 keycare-0.0.7/keycare/keycare.egg-info/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7593 2024-05-24 10:29:28.000000 keycare-0.0.7/keycare/keycare.egg-info/PKG-INFO
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)      319 2024-05-24 10:29:28.000000 keycare-0.0.7/keycare/keycare.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)        1 2024-05-24 10:29:28.000000 keycare-0.0.7/keycare/keycare.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)      369 2024-05-24 10:29:28.000000 keycare-0.0.7/keycare/keycare.egg-info/requires.txt
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)        8 2024-05-24 10:29:28.000000 keycare-0.0.7/keycare/keycare.egg-info/top_level.txt
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1643 2024-05-24 10:28:16.000000 keycare-0.0.7/pyproject.toml
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)       38 2024-05-24 10:29:29.577814 keycare-0.0.7/setup.cfg
```

### Comparing `keycare-0.0.6/LICENSE` & `keycare-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `keycare-0.0.6/PKG-INFO` & `keycare-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycare
-Version: 0.0.6
+Version: 0.0.7
 Summary: KeyCARE is a Python library designed for the unsupervised keyword extraction from biomedical documents with the use of different algorithms, the classification of the keywords according to their semantic nature, and the extraction of is a relations among those keywords and with other terminologies.
 Author-email: Sergi Marsol <sergimarsolt@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 nlp4bia-bsc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: keycare Version: 0.0.6 Summary: KeyCARE is a Python
+Metadata-Version: 2.1 Name: keycare Version: 0.0.7 Summary: KeyCARE is a Python
 library designed for the unsupervised keyword extraction from biomedical
 documents with the use of different algorithms, the classification of the
 keywords according to their semantic nature, and the extraction of is a
 relations among those keywords and with other terminologies. Author-email:
 Sergi Marsol
 gmail.com> License: MIT License Copyright (c) 2023 nlp4bia-bsc Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
```

### Comparing `keycare-0.0.6/README.md` & `keycare-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `keycare-0.0.6/keycare/keycare.egg-info/PKG-INFO` & `keycare-0.0.7/keycare/keycare.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycare
-Version: 0.0.6
+Version: 0.0.7
 Summary: KeyCARE is a Python library designed for the unsupervised keyword extraction from biomedical documents with the use of different algorithms, the classification of the keywords according to their semantic nature, and the extraction of is a relations among those keywords and with other terminologies.
 Author-email: Sergi Marsol <sergimarsolt@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 nlp4bia-bsc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: keycare Version: 0.0.6 Summary: KeyCARE is a Python
+Metadata-Version: 2.1 Name: keycare Version: 0.0.7 Summary: KeyCARE is a Python
 library designed for the unsupervised keyword extraction from biomedical
 documents with the use of different algorithms, the classification of the
 keywords according to their semantic nature, and the extraction of is a
 relations among those keywords and with other terminologies. Author-email:
 Sergi Marsol
 gmail.com> License: MIT License Copyright (c) 2023 nlp4bia-bsc Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
```

### Comparing `keycare-0.0.6/pyproject.toml` & `keycare-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.setuptools.packages.find]
 where = ["keycare"]
 include = ["keycare"]
 exclude = ["tests"]
 
 [project]
 name = "keycare"
-version = "0.0.6"
+version = "0.0.7"
 description = "KeyCARE is a Python library designed for the unsupervised keyword extraction from biomedical documents with the use of different algorithms, the classification of the keywords according to their semantic nature, and the extraction of is a relations among those keywords and with other terminologies."
 readme = "README.md"
 authors = [{ name = "Sergi Marsol", email = "sergimarsolt@gmail.com" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 dependencies = [
     "datasets==2.14.4",
```


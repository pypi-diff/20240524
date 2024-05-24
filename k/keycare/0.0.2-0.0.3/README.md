# Comparing `tmp/keycare-0.0.2.tar.gz` & `tmp/keycare-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycare-0.0.2.tar", last modified: Fri May 24 10:02:57 2024, max compression
+gzip compressed data, was "keycare-0.0.3.tar", last modified: Fri May 24 10:08:47 2024, max compression
```

## Comparing `keycare-0.0.2.tar` & `keycare-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:02:57.315379 keycare-0.0.2/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1068 2023-07-28 11:11:56.000000 keycare-0.0.2/LICENSE
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7593 2024-05-24 10:02:57.296131 keycare-0.0.2/PKG-INFO
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     4805 2024-05-24 09:25:31.000000 keycare-0.0.2/README.md
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:02:56.015001 keycare-0.0.2/keycare/
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:02:56.315141 keycare-0.0.2/keycare/categorizers/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     5858 2024-02-29 17:21:47.000000 keycare-0.0.2/keycare/categorizers/Categorizer.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     4395 2024-02-29 17:21:47.000000 keycare-0.0.2/keycare/categorizers/Clustering.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     5107 2024-05-22 17:26:21.000000 keycare-0.0.2/keycare/categorizers/SetFitClassifier.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7960 2024-05-22 17:26:43.000000 keycare-0.0.2/keycare/categorizers/TransformersClassifier.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.2/keycare/categorizers/__init__.py
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:02:56.611396 keycare-0.0.2/keycare/extractors/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7082 2024-02-29 17:21:47.000000 keycare-0.0.2/keycare/extractors/Extractor.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2909 2024-05-22 15:44:07.000000 keycare-0.0.2/keycare/extractors/KeyBertExtractor.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1706 2024-02-29 17:21:47.000000 keycare-0.0.2/keycare/extractors/RakeExtractor.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1631 2024-02-29 17:21:47.000000 keycare-0.0.2/keycare/extractors/TextRankExtractor.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1503 2024-02-29 17:21:47.000000 keycare-0.0.2/keycare/extractors/YakeExtractor.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.2/keycare/extractors/__init__.py
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:02:57.267686 keycare-0.0.2/keycare/keycare.egg-info/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7593 2024-05-24 10:02:55.000000 keycare-0.0.2/keycare/keycare.egg-info/PKG-INFO
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)      822 2024-05-24 10:02:55.000000 keycare-0.0.2/keycare/keycare.egg-info/SOURCES.txt
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)        1 2024-05-24 10:02:55.000000 keycare-0.0.2/keycare/keycare.egg-info/dependency_links.txt
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)      369 2024-05-24 10:02:55.000000 keycare-0.0.2/keycare/keycare.egg-info/requires.txt
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)       39 2024-05-24 10:02:55.000000 keycare-0.0.2/keycare/keycare.egg-info/top_level.txt
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:02:57.101750 keycare-0.0.2/keycare/relators/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)      517 2024-02-29 17:21:47.000000 keycare-0.0.2/keycare/relators/Relator.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2147 2024-05-22 17:27:08.000000 keycare-0.0.2/keycare/relators/SetFitRelator.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2596 2024-05-22 17:27:22.000000 keycare-0.0.2/keycare/relators/TransformersRelator.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.2/keycare/relators/__init__.py
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:02:57.200254 keycare-0.0.2/keycare/utils/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.2/keycare/utils/__init__.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2355 2024-02-29 17:21:47.000000 keycare-0.0.2/keycare/utils/data_structures.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1620 2024-05-24 09:53:40.000000 keycare-0.0.2/pyproject.toml
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)       38 2024-05-24 10:02:57.315379 keycare-0.0.2/setup.cfg
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:08:47.942385 keycare-0.0.3/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1068 2023-07-28 11:11:56.000000 keycare-0.0.3/LICENSE
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7593 2024-05-24 10:08:47.923662 keycare-0.0.3/PKG-INFO
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     4805 2024-05-24 09:25:31.000000 keycare-0.0.3/README.md
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:08:46.605544 keycare-0.0.3/keycare/
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:08:46.926806 keycare-0.0.3/keycare/categorizers/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     5858 2024-02-29 17:21:47.000000 keycare-0.0.3/keycare/categorizers/Categorizer.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     4395 2024-02-29 17:21:47.000000 keycare-0.0.3/keycare/categorizers/Clustering.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     5107 2024-05-22 17:26:21.000000 keycare-0.0.3/keycare/categorizers/SetFitClassifier.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7960 2024-05-22 17:26:43.000000 keycare-0.0.3/keycare/categorizers/TransformersClassifier.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.3/keycare/categorizers/__init__.py
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:08:47.237364 keycare-0.0.3/keycare/extractors/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7082 2024-02-29 17:21:47.000000 keycare-0.0.3/keycare/extractors/Extractor.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2909 2024-05-22 15:44:07.000000 keycare-0.0.3/keycare/extractors/KeyBertExtractor.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1706 2024-02-29 17:21:47.000000 keycare-0.0.3/keycare/extractors/RakeExtractor.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1631 2024-02-29 17:21:47.000000 keycare-0.0.3/keycare/extractors/TextRankExtractor.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1503 2024-02-29 17:21:47.000000 keycare-0.0.3/keycare/extractors/YakeExtractor.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.3/keycare/extractors/__init__.py
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:08:47.893554 keycare-0.0.3/keycare/keycare.egg-info/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7593 2024-05-24 10:08:46.000000 keycare-0.0.3/keycare/keycare.egg-info/PKG-INFO
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)      862 2024-05-24 10:08:46.000000 keycare-0.0.3/keycare/keycare.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)        1 2024-05-24 10:08:46.000000 keycare-0.0.3/keycare/keycare.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)      369 2024-05-24 10:08:46.000000 keycare-0.0.3/keycare/keycare.egg-info/requires.txt
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)       45 2024-05-24 10:08:46.000000 keycare-0.0.3/keycare/keycare.egg-info/top_level.txt
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:08:47.672159 keycare-0.0.3/keycare/relators/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)      517 2024-02-29 17:21:47.000000 keycare-0.0.3/keycare/relators/Relator.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2147 2024-05-22 17:27:08.000000 keycare-0.0.3/keycare/relators/SetFitRelator.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2596 2024-05-22 17:27:22.000000 keycare-0.0.3/keycare/relators/TransformersRelator.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.3/keycare/relators/__init__.py
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:08:47.732350 keycare-0.0.3/keycare/tests/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1495 2024-05-17 10:51:38.000000 keycare-0.0.3/keycare/tests/termextractor_pipeline.py
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:08:47.821586 keycare-0.0.3/keycare/utils/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.3/keycare/utils/__init__.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2355 2024-02-29 17:21:47.000000 keycare-0.0.3/keycare/utils/data_structures.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1599 2024-05-24 10:07:51.000000 keycare-0.0.3/pyproject.toml
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)       38 2024-05-24 10:08:47.945589 keycare-0.0.3/setup.cfg
```

### Comparing `keycare-0.0.2/LICENSE` & `keycare-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `keycare-0.0.2/PKG-INFO` & `keycare-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycare
-Version: 0.0.2
+Version: 0.0.3
 Summary: KeyCARE is a Python library designed for the unsupervised keyword extraction from biomedical documents with the use of different algorithms, the classification of the keywords according to their semantic nature, and the extraction of is a relations among those keywords and with other terminologies.
 Author-email: Sergi Marsol <sergimarsolt@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 nlp4bia-bsc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: keycare Version: 0.0.2 Summary: KeyCARE is a Python
+Metadata-Version: 2.1 Name: keycare Version: 0.0.3 Summary: KeyCARE is a Python
 library designed for the unsupervised keyword extraction from biomedical
 documents with the use of different algorithms, the classification of the
 keywords according to their semantic nature, and the extraction of is a
 relations among those keywords and with other terminologies. Author-email:
 Sergi Marsol
 gmail.com> License: MIT License Copyright (c) 2023 nlp4bia-bsc Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
```

### Comparing `keycare-0.0.2/README.md` & `keycare-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `keycare-0.0.2/keycare/categorizers/Categorizer.py` & `keycare-0.0.3/keycare/categorizers/Categorizer.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.2/keycare/categorizers/Clustering.py` & `keycare-0.0.3/keycare/categorizers/Clustering.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.2/keycare/categorizers/SetFitClassifier.py` & `keycare-0.0.3/keycare/categorizers/SetFitClassifier.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.2/keycare/categorizers/TransformersClassifier.py` & `keycare-0.0.3/keycare/categorizers/TransformersClassifier.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.2/keycare/extractors/Extractor.py` & `keycare-0.0.3/keycare/extractors/Extractor.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.2/keycare/extractors/KeyBertExtractor.py` & `keycare-0.0.3/keycare/extractors/KeyBertExtractor.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.2/keycare/extractors/RakeExtractor.py` & `keycare-0.0.3/keycare/extractors/RakeExtractor.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.2/keycare/extractors/TextRankExtractor.py` & `keycare-0.0.3/keycare/extractors/TextRankExtractor.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.2/keycare/extractors/YakeExtractor.py` & `keycare-0.0.3/keycare/extractors/YakeExtractor.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.2/keycare/keycare.egg-info/PKG-INFO` & `keycare-0.0.3/keycare/keycare.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycare
-Version: 0.0.2
+Version: 0.0.3
 Summary: KeyCARE is a Python library designed for the unsupervised keyword extraction from biomedical documents with the use of different algorithms, the classification of the keywords according to their semantic nature, and the extraction of is a relations among those keywords and with other terminologies.
 Author-email: Sergi Marsol <sergimarsolt@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 nlp4bia-bsc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: keycare Version: 0.0.2 Summary: KeyCARE is a Python
+Metadata-Version: 2.1 Name: keycare Version: 0.0.3 Summary: KeyCARE is a Python
 library designed for the unsupervised keyword extraction from biomedical
 documents with the use of different algorithms, the classification of the
 keywords according to their semantic nature, and the extraction of is a
 relations among those keywords and with other terminologies. Author-email:
 Sergi Marsol
 gmail.com> License: MIT License Copyright (c) 2023 nlp4bia-bsc Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
```

### Comparing `keycare-0.0.2/keycare/keycare.egg-info/SOURCES.txt` & `keycare-0.0.3/keycare/keycare.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,9 +17,10 @@
 keycare/keycare.egg-info/dependency_links.txt
 keycare/keycare.egg-info/requires.txt
 keycare/keycare.egg-info/top_level.txt
 keycare/relators/Relator.py
 keycare/relators/SetFitRelator.py
 keycare/relators/TransformersRelator.py
 keycare/relators/__init__.py
+keycare/tests/termextractor_pipeline.py
 keycare/utils/__init__.py
 keycare/utils/data_structures.py
```

### Comparing `keycare-0.0.2/keycare/relators/Relator.py` & `keycare-0.0.3/keycare/relators/Relator.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.2/keycare/relators/SetFitRelator.py` & `keycare-0.0.3/keycare/relators/SetFitRelator.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.2/keycare/relators/TransformersRelator.py` & `keycare-0.0.3/keycare/relators/TransformersRelator.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.2/keycare/utils/data_structures.py` & `keycare-0.0.3/keycare/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.2/pyproject.toml` & `keycare-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,18 @@
     "setuptools>=69.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["keycare"]
-exclude = ["tests"]
 
 [project]
 name = "keycare"
-version = "0.0.2"
+version = "0.0.3"
 description = "KeyCARE is a Python library designed for the unsupervised keyword extraction from biomedical documents with the use of different algorithms, the classification of the keywords according to their semantic nature, and the extraction of is a relations among those keywords and with other terminologies."
 readme = "README.md"
 authors = [{ name = "Sergi Marsol", email = "sergimarsolt@gmail.com" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 dependencies = [
     "datasets==2.14.4",
```


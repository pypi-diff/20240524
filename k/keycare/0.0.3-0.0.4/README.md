# Comparing `tmp/keycare-0.0.3.tar.gz` & `tmp/keycare-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycare-0.0.3.tar", last modified: Fri May 24 10:08:47 2024, max compression
+gzip compressed data, was "keycare-0.0.4.tar", last modified: Fri May 24 10:18:54 2024, max compression
```

## Comparing `keycare-0.0.3.tar` & `keycare-0.0.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:08:47.942385 keycare-0.0.3/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1068 2023-07-28 11:11:56.000000 keycare-0.0.3/LICENSE
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7593 2024-05-24 10:08:47.923662 keycare-0.0.3/PKG-INFO
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     4805 2024-05-24 09:25:31.000000 keycare-0.0.3/README.md
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:08:46.605544 keycare-0.0.3/keycare/
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:08:46.926806 keycare-0.0.3/keycare/categorizers/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     5858 2024-02-29 17:21:47.000000 keycare-0.0.3/keycare/categorizers/Categorizer.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     4395 2024-02-29 17:21:47.000000 keycare-0.0.3/keycare/categorizers/Clustering.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     5107 2024-05-22 17:26:21.000000 keycare-0.0.3/keycare/categorizers/SetFitClassifier.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7960 2024-05-22 17:26:43.000000 keycare-0.0.3/keycare/categorizers/TransformersClassifier.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.3/keycare/categorizers/__init__.py
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:08:47.237364 keycare-0.0.3/keycare/extractors/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7082 2024-02-29 17:21:47.000000 keycare-0.0.3/keycare/extractors/Extractor.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2909 2024-05-22 15:44:07.000000 keycare-0.0.3/keycare/extractors/KeyBertExtractor.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1706 2024-02-29 17:21:47.000000 keycare-0.0.3/keycare/extractors/RakeExtractor.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1631 2024-02-29 17:21:47.000000 keycare-0.0.3/keycare/extractors/TextRankExtractor.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1503 2024-02-29 17:21:47.000000 keycare-0.0.3/keycare/extractors/YakeExtractor.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.3/keycare/extractors/__init__.py
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:08:47.893554 keycare-0.0.3/keycare/keycare.egg-info/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7593 2024-05-24 10:08:46.000000 keycare-0.0.3/keycare/keycare.egg-info/PKG-INFO
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)      862 2024-05-24 10:08:46.000000 keycare-0.0.3/keycare/keycare.egg-info/SOURCES.txt
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)        1 2024-05-24 10:08:46.000000 keycare-0.0.3/keycare/keycare.egg-info/dependency_links.txt
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)      369 2024-05-24 10:08:46.000000 keycare-0.0.3/keycare/keycare.egg-info/requires.txt
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)       45 2024-05-24 10:08:46.000000 keycare-0.0.3/keycare/keycare.egg-info/top_level.txt
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:08:47.672159 keycare-0.0.3/keycare/relators/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)      517 2024-02-29 17:21:47.000000 keycare-0.0.3/keycare/relators/Relator.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2147 2024-05-22 17:27:08.000000 keycare-0.0.3/keycare/relators/SetFitRelator.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2596 2024-05-22 17:27:22.000000 keycare-0.0.3/keycare/relators/TransformersRelator.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.3/keycare/relators/__init__.py
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:08:47.732350 keycare-0.0.3/keycare/tests/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1495 2024-05-17 10:51:38.000000 keycare-0.0.3/keycare/tests/termextractor_pipeline.py
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:08:47.821586 keycare-0.0.3/keycare/utils/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.3/keycare/utils/__init__.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2355 2024-02-29 17:21:47.000000 keycare-0.0.3/keycare/utils/data_structures.py
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1599 2024-05-24 10:07:51.000000 keycare-0.0.3/pyproject.toml
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)       38 2024-05-24 10:08:47.945589 keycare-0.0.3/setup.cfg
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:18:54.919333 keycare-0.0.4/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1068 2023-07-28 11:11:56.000000 keycare-0.0.4/LICENSE
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7593 2024-05-24 10:18:54.897915 keycare-0.0.4/PKG-INFO
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     4805 2024-05-24 09:25:31.000000 keycare-0.0.4/README.md
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:18:53.744671 keycare-0.0.4/keycare/
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:18:54.026846 keycare-0.0.4/keycare/categorizers/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     5858 2024-02-29 17:21:47.000000 keycare-0.0.4/keycare/categorizers/Categorizer.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     4395 2024-02-29 17:21:47.000000 keycare-0.0.4/keycare/categorizers/Clustering.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     5107 2024-05-22 17:26:21.000000 keycare-0.0.4/keycare/categorizers/SetFitClassifier.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7960 2024-05-22 17:26:43.000000 keycare-0.0.4/keycare/categorizers/TransformersClassifier.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.4/keycare/categorizers/__init__.py
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:18:54.257126 keycare-0.0.4/keycare/extractors/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7082 2024-02-29 17:21:47.000000 keycare-0.0.4/keycare/extractors/Extractor.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2909 2024-05-22 15:44:07.000000 keycare-0.0.4/keycare/extractors/KeyBertExtractor.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1706 2024-02-29 17:21:47.000000 keycare-0.0.4/keycare/extractors/RakeExtractor.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1631 2024-02-29 17:21:47.000000 keycare-0.0.4/keycare/extractors/TextRankExtractor.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1503 2024-02-29 17:21:47.000000 keycare-0.0.4/keycare/extractors/YakeExtractor.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.4/keycare/extractors/__init__.py
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:18:54.871826 keycare-0.0.4/keycare/keycare.egg-info/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7593 2024-05-24 10:18:53.000000 keycare-0.0.4/keycare/keycare.egg-info/PKG-INFO
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)      862 2024-05-24 10:18:53.000000 keycare-0.0.4/keycare/keycare.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)        1 2024-05-24 10:18:53.000000 keycare-0.0.4/keycare/keycare.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)      369 2024-05-24 10:18:53.000000 keycare-0.0.4/keycare/keycare.egg-info/requires.txt
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)       45 2024-05-24 10:18:53.000000 keycare-0.0.4/keycare/keycare.egg-info/top_level.txt
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:18:54.702900 keycare-0.0.4/keycare/relators/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)      517 2024-02-29 17:21:47.000000 keycare-0.0.4/keycare/relators/Relator.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2147 2024-05-22 17:27:08.000000 keycare-0.0.4/keycare/relators/SetFitRelator.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2596 2024-05-22 17:27:22.000000 keycare-0.0.4/keycare/relators/TransformersRelator.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.4/keycare/relators/__init__.py
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:18:54.744318 keycare-0.0.4/keycare/tests/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1495 2024-05-17 10:51:38.000000 keycare-0.0.4/keycare/tests/termextractor_pipeline.py
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:18:54.818230 keycare-0.0.4/keycare/utils/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.4/keycare/utils/__init__.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2355 2024-02-29 17:21:47.000000 keycare-0.0.4/keycare/utils/data_structures.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1599 2024-05-24 10:17:19.000000 keycare-0.0.4/pyproject.toml
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)       38 2024-05-24 10:18:54.922243 keycare-0.0.4/setup.cfg
```

### Comparing `keycare-0.0.3/LICENSE` & `keycare-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `keycare-0.0.3/PKG-INFO` & `keycare-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycare
-Version: 0.0.3
+Version: 0.0.4
 Summary: KeyCARE is a Python library designed for the unsupervised keyword extraction from biomedical documents with the use of different algorithms, the classification of the keywords according to their semantic nature, and the extraction of is a relations among those keywords and with other terminologies.
 Author-email: Sergi Marsol <sergimarsolt@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 nlp4bia-bsc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: keycare Version: 0.0.3 Summary: KeyCARE is a Python
+Metadata-Version: 2.1 Name: keycare Version: 0.0.4 Summary: KeyCARE is a Python
 library designed for the unsupervised keyword extraction from biomedical
 documents with the use of different algorithms, the classification of the
 keywords according to their semantic nature, and the extraction of is a
 relations among those keywords and with other terminologies. Author-email:
 Sergi Marsol
 gmail.com> License: MIT License Copyright (c) 2023 nlp4bia-bsc Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
```

### Comparing `keycare-0.0.3/README.md` & `keycare-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `keycare-0.0.3/keycare/categorizers/Categorizer.py` & `keycare-0.0.4/keycare/categorizers/Categorizer.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.3/keycare/categorizers/Clustering.py` & `keycare-0.0.4/keycare/categorizers/Clustering.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.3/keycare/categorizers/SetFitClassifier.py` & `keycare-0.0.4/keycare/categorizers/SetFitClassifier.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.3/keycare/categorizers/TransformersClassifier.py` & `keycare-0.0.4/keycare/categorizers/TransformersClassifier.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.3/keycare/extractors/Extractor.py` & `keycare-0.0.4/keycare/extractors/Extractor.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.3/keycare/extractors/KeyBertExtractor.py` & `keycare-0.0.4/keycare/extractors/KeyBertExtractor.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.3/keycare/extractors/RakeExtractor.py` & `keycare-0.0.4/keycare/extractors/RakeExtractor.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.3/keycare/extractors/TextRankExtractor.py` & `keycare-0.0.4/keycare/extractors/TextRankExtractor.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.3/keycare/extractors/YakeExtractor.py` & `keycare-0.0.4/keycare/extractors/YakeExtractor.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.3/keycare/keycare.egg-info/PKG-INFO` & `keycare-0.0.4/keycare/keycare.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycare
-Version: 0.0.3
+Version: 0.0.4
 Summary: KeyCARE is a Python library designed for the unsupervised keyword extraction from biomedical documents with the use of different algorithms, the classification of the keywords according to their semantic nature, and the extraction of is a relations among those keywords and with other terminologies.
 Author-email: Sergi Marsol <sergimarsolt@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 nlp4bia-bsc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: keycare Version: 0.0.3 Summary: KeyCARE is a Python
+Metadata-Version: 2.1 Name: keycare Version: 0.0.4 Summary: KeyCARE is a Python
 library designed for the unsupervised keyword extraction from biomedical
 documents with the use of different algorithms, the classification of the
 keywords according to their semantic nature, and the extraction of is a
 relations among those keywords and with other terminologies. Author-email:
 Sergi Marsol
 gmail.com> License: MIT License Copyright (c) 2023 nlp4bia-bsc Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
```

### Comparing `keycare-0.0.3/keycare/keycare.egg-info/SOURCES.txt` & `keycare-0.0.4/keycare/keycare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keycare-0.0.3/keycare/relators/Relator.py` & `keycare-0.0.4/keycare/relators/Relator.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.3/keycare/relators/SetFitRelator.py` & `keycare-0.0.4/keycare/relators/SetFitRelator.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.3/keycare/relators/TransformersRelator.py` & `keycare-0.0.4/keycare/relators/TransformersRelator.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.3/keycare/tests/termextractor_pipeline.py` & `keycare-0.0.4/keycare/tests/termextractor_pipeline.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.3/keycare/utils/data_structures.py` & `keycare-0.0.4/keycare/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `keycare-0.0.3/pyproject.toml` & `keycare-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["keycare"]
 
 [project]
 name = "keycare"
-version = "0.0.3"
+version = "0.0.4"
 description = "KeyCARE is a Python library designed for the unsupervised keyword extraction from biomedical documents with the use of different algorithms, the classification of the keywords according to their semantic nature, and the extraction of is a relations among those keywords and with other terminologies."
 readme = "README.md"
 authors = [{ name = "Sergi Marsol", email = "sergimarsolt@gmail.com" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 dependencies = [
     "datasets==2.14.4",
```


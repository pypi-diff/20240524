# Comparing `tmp/keycare-0.0.1.tar.gz` & `tmp/keycare-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycare-0.0.1.tar", last modified: Wed May 22 20:16:40 2024, max compression
+gzip compressed data, was "keycare-0.0.2.tar", last modified: Fri May 24 10:02:57 2024, max compression
```

## Comparing `keycare-0.0.1.tar` & `keycare-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,34 @@
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 20:16:40.719228 keycare-0.0.1/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1068 2023-07-28 11:11:56.000000 keycare-0.0.1/LICENSE
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7485 2024-05-22 20:16:40.693906 keycare-0.0.1/PKG-INFO
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     4696 2024-02-29 17:21:47.000000 keycare-0.0.1/README.md
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 20:16:40.201526 keycare-0.0.1/keycare/
-drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 20:16:40.658007 keycare-0.0.1/keycare/keycare.egg-info/
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7485 2024-05-22 20:16:39.000000 keycare-0.0.1/keycare/keycare.egg-info/PKG-INFO
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)      226 2024-05-22 20:16:40.000000 keycare-0.0.1/keycare/keycare.egg-info/SOURCES.txt
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)        1 2024-05-22 20:16:39.000000 keycare-0.0.1/keycare/keycare.egg-info/dependency_links.txt
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)      369 2024-05-22 20:16:39.000000 keycare-0.0.1/keycare/keycare.egg-info/requires.txt
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)        1 2024-05-22 20:16:39.000000 keycare-0.0.1/keycare/keycare.egg-info/top_level.txt
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1634 2024-05-22 18:17:39.000000 keycare-0.0.1/pyproject.toml
--rwxrwxrwx   0 sergi     (1000) sergi     (1000)       38 2024-05-22 20:16:40.721385 keycare-0.0.1/setup.cfg
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:02:57.315379 keycare-0.0.2/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1068 2023-07-28 11:11:56.000000 keycare-0.0.2/LICENSE
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7593 2024-05-24 10:02:57.296131 keycare-0.0.2/PKG-INFO
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     4805 2024-05-24 09:25:31.000000 keycare-0.0.2/README.md
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:02:56.015001 keycare-0.0.2/keycare/
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:02:56.315141 keycare-0.0.2/keycare/categorizers/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     5858 2024-02-29 17:21:47.000000 keycare-0.0.2/keycare/categorizers/Categorizer.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     4395 2024-02-29 17:21:47.000000 keycare-0.0.2/keycare/categorizers/Clustering.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     5107 2024-05-22 17:26:21.000000 keycare-0.0.2/keycare/categorizers/SetFitClassifier.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7960 2024-05-22 17:26:43.000000 keycare-0.0.2/keycare/categorizers/TransformersClassifier.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.2/keycare/categorizers/__init__.py
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:02:56.611396 keycare-0.0.2/keycare/extractors/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7082 2024-02-29 17:21:47.000000 keycare-0.0.2/keycare/extractors/Extractor.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2909 2024-05-22 15:44:07.000000 keycare-0.0.2/keycare/extractors/KeyBertExtractor.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1706 2024-02-29 17:21:47.000000 keycare-0.0.2/keycare/extractors/RakeExtractor.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1631 2024-02-29 17:21:47.000000 keycare-0.0.2/keycare/extractors/TextRankExtractor.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1503 2024-02-29 17:21:47.000000 keycare-0.0.2/keycare/extractors/YakeExtractor.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.2/keycare/extractors/__init__.py
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:02:57.267686 keycare-0.0.2/keycare/keycare.egg-info/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     7593 2024-05-24 10:02:55.000000 keycare-0.0.2/keycare/keycare.egg-info/PKG-INFO
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)      822 2024-05-24 10:02:55.000000 keycare-0.0.2/keycare/keycare.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)        1 2024-05-24 10:02:55.000000 keycare-0.0.2/keycare/keycare.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)      369 2024-05-24 10:02:55.000000 keycare-0.0.2/keycare/keycare.egg-info/requires.txt
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)       39 2024-05-24 10:02:55.000000 keycare-0.0.2/keycare/keycare.egg-info/top_level.txt
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:02:57.101750 keycare-0.0.2/keycare/relators/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)      517 2024-02-29 17:21:47.000000 keycare-0.0.2/keycare/relators/Relator.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2147 2024-05-22 17:27:08.000000 keycare-0.0.2/keycare/relators/SetFitRelator.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2596 2024-05-22 17:27:22.000000 keycare-0.0.2/keycare/relators/TransformersRelator.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.2/keycare/relators/__init__.py
+drwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-24 10:02:57.200254 keycare-0.0.2/keycare/utils/
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)        0 2024-05-22 15:06:47.000000 keycare-0.0.2/keycare/utils/__init__.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     2355 2024-02-29 17:21:47.000000 keycare-0.0.2/keycare/utils/data_structures.py
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)     1620 2024-05-24 09:53:40.000000 keycare-0.0.2/pyproject.toml
+-rwxrwxrwx   0 sergi     (1000) sergi     (1000)       38 2024-05-24 10:02:57.315379 keycare-0.0.2/setup.cfg
```

### Comparing `keycare-0.0.1/LICENSE` & `keycare-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `keycare-0.0.1/PKG-INFO` & `keycare-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycare
-Version: 0.0.1
+Version: 0.0.2
 Summary: KeyCARE is a Python library designed for the unsupervised keyword extraction from biomedical documents with the use of different algorithms, the classification of the keywords according to their semantic nature, and the extraction of is a relations among those keywords and with other terminologies.
 Author-email: Sergi Marsol <sergimarsolt@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 nlp4bia-bsc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -109,44 +109,43 @@
 
 <a name="about"/></a>
 ## 1. About The Project
 [Back to ToC](#toc)
 KeyBERT provides a common interface for extracting, categorizing and associating terms extracted from a text: 
 
 1. **Keywords extraction**: KeyCARE implements several unsupervised term extraction techniques such as [*YAKE*](https://github.com/LIAAD/yake), [*RAKE*](https://pypi.org/project/rake-nltk/), [*TextRank*](https://pypi.org/project/pytextrank/) or [*KeyBERT*](https://github.com/MaartenGr/KeyBERT) to automatically extract key terms from a text.
-2. **Term categorization**: KeyCARE allows the application of term clustering techniques to group similar terms, as well as the training and application of supervised techniques to classify keywords into predefined categories. 
+2. **Term categorization**: KeyCARE allows the application of term clustering techniques to group similar terms, as well as the training and application of supervised techniques to classify keywords into predefined categories, including [SetFit]. 
 3. **Semantic relation classification**: Beyond the identification and categorization of terms, the library supports the use of neural classification models to extract the semantic relation between two terms by means of EXACT, BROAD, NARROW and NO_relation relationships, which allows interconnecting the extracted terms and can be used for terminological enrichment, among other tasks.
 
 <!-- GETTING STARTED -->
 <a name="gettingstarted"/></a>
 ## 2. Getting Started
 [Back to ToC](#toc)
 
 <a name="installation"/></a>
 ### 2.1. Installation 
 Installation can be done using pypi:
 
 ```sh
-   pip install keybert
+   pip install keycare
 ```
 
 <a name="usage"/></a>
 ### 2.2. Usage 
-La librería se construye sobre X objetos principales:
-
-
+The library is built on 3 main processes:
 
 #### Term Extraction
-
+...
 
 #### Term Categorization
 
 
 #### Relation Extraction
 
+For further information on the functioning of the library refer to the tutorials in the nbs folder.
 
 <!-- CONTRIBUTING -->
 <a name="contributing"/></a>
 ## 3. Contributing
 [Back to ToC](#toc)
 
 This library has been developed with Python 3.8.2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: keycare Version: 0.0.1 Summary: KeyCARE is a Python
+Metadata-Version: 2.1 Name: keycare Version: 0.0.2 Summary: KeyCARE is a Python
 library designed for the unsupervised keyword extraction from biomedical
 documents with the use of different algorithms, the classification of the
 keywords according to their semantic nature, and the extraction of is a
 relations among those keywords and with other terminologies. Author-email:
 Sergi Marsol
 gmail.com> License: MIT License Copyright (c) 2023 nlp4bia-bsc Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
@@ -47,32 +47,33 @@
 from a text: 1. **Keywords extraction**: KeyCARE implements several
 unsupervised term extraction techniques such as [*YAKE*](https://github.com/
 LIAAD/yake), [*RAKE*](https://pypi.org/project/rake-nltk/), [*TextRank*](https:
 //pypi.org/project/pytextrank/) or [*KeyBERT*](https://github.com/MaartenGr/
 KeyBERT) to automatically extract key terms from a text. 2. **Term
 categorization**: KeyCARE allows the application of term clustering techniques
 to group similar terms, as well as the training and application of supervised
-techniques to classify keywords into predefined categories. 3. **Semantic
-relation classification**: Beyond the identification and categorization of
-terms, the library supports the use of neural classification models to extract
-the semantic relation between two terms by means of EXACT, BROAD, NARROW and
-NO_relation relationships, which allows interconnecting the extracted terms and
-can be used for terminological enrichment, among other tasks. ## 2. Getting
-Started [Back to ToC](#toc) ### 2.1. Installation Installation can be done
-using pypi: ```sh pip install keybert ``` ### 2.2. Usage La librerÃ­a se
-construye sobre X objetos principales: #### Term Extraction #### Term
-Categorization #### Relation Extraction ## 3. Contributing [Back to ToC](#toc)
-This library has been developed with Python 3.8.2 Any contributions you make
-are **greatly appreciated**. For contributing: 1. Fork/Clone the Project in
-your system ```sh git clone https://github.com/nlp4bia-bsc/keycare.git ``` 2.
-Create a new virtual environment ```sh python3 -m venv .env_keycare ``` 3.
-Activate the new environment ```sh source .env_keycare/bin/activate ``` 4.
-Install the requirements ```sh pip install -r requirements.txt ``` 5. Create
-your Feature Branch (`git checkout -b feature/AmazingFeature`) 6. Update
-requirements file (`pip freeze > requirements.txt`) 7. Commit your Changes
-(`git commit -m 'Add some AmazingFeature'`) 8. Push to the Branch (`git push
-origin feature/AmazingFeature`) 9. Open a Pull Request from github. Follow
-[this tutorial](https://github.com/Kunena/Kunena-Forum/wiki/Create-a-new-
-branch-with-git-and-manage-branches) to create a branch. ## 4. License [Back to
-ToC](#toc) [Apache License, Version 2.0](https://www.apache.org/licenses/
-LICENSE-2.0) ## 5. References [Back to ToC](#toc) Please cite if you use the
-library in scientific works: > PAPER TO BE PUBLISHED
+techniques to classify keywords into predefined categories, including [SetFit].
+3. **Semantic relation classification**: Beyond the identification and
+categorization of terms, the library supports the use of neural classification
+models to extract the semantic relation between two terms by means of EXACT,
+BROAD, NARROW and NO_relation relationships, which allows interconnecting the
+extracted terms and can be used for terminological enrichment, among other
+tasks. ## 2. Getting Started [Back to ToC](#toc) ### 2.1. Installation
+Installation can be done using pypi: ```sh pip install keycare ``` ### 2.2.
+Usage The library is built on 3 main processes: #### Term Extraction ... ####
+Term Categorization #### Relation Extraction For further information on the
+functioning of the library refer to the tutorials in the nbs folder. ## 3.
+Contributing [Back to ToC](#toc) This library has been developed with Python
+3.8.2 Any contributions you make are **greatly appreciated**. For contributing:
+1. Fork/Clone the Project in your system ```sh git clone https://github.com/
+nlp4bia-bsc/keycare.git ``` 2. Create a new virtual environment ```sh python3 -
+m venv .env_keycare ``` 3. Activate the new environment ```sh source
+.env_keycare/bin/activate ``` 4. Install the requirements ```sh pip install -
+r requirements.txt ``` 5. Create your Feature Branch (`git checkout -b feature/
+AmazingFeature`) 6. Update requirements file (`pip freeze > requirements.txt`)
+7. Commit your Changes (`git commit -m 'Add some AmazingFeature'`) 8. Push to
+the Branch (`git push origin feature/AmazingFeature`) 9. Open a Pull Request
+from github. Follow [this tutorial](https://github.com/Kunena/Kunena-Forum/
+wiki/Create-a-new-branch-with-git-and-manage-branches) to create a branch. ##
+4. License [Back to ToC](#toc) [Apache License, Version 2.0](https://
+www.apache.org/licenses/LICENSE-2.0) ## 5. References [Back to ToC](#toc)
+Please cite if you use the library in scientific works: > PAPER TO BE PUBLISHED
```

### Comparing `keycare-0.0.1/README.md` & `keycare-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -51,44 +51,43 @@
 
 <a name="about"/></a>
 ## 1. About The Project
 [Back to ToC](#toc)
 KeyBERT provides a common interface for extracting, categorizing and associating terms extracted from a text: 
 
 1. **Keywords extraction**: KeyCARE implements several unsupervised term extraction techniques such as [*YAKE*](https://github.com/LIAAD/yake), [*RAKE*](https://pypi.org/project/rake-nltk/), [*TextRank*](https://pypi.org/project/pytextrank/) or [*KeyBERT*](https://github.com/MaartenGr/KeyBERT) to automatically extract key terms from a text.
-2. **Term categorization**: KeyCARE allows the application of term clustering techniques to group similar terms, as well as the training and application of supervised techniques to classify keywords into predefined categories. 
+2. **Term categorization**: KeyCARE allows the application of term clustering techniques to group similar terms, as well as the training and application of supervised techniques to classify keywords into predefined categories, including [SetFit]. 
 3. **Semantic relation classification**: Beyond the identification and categorization of terms, the library supports the use of neural classification models to extract the semantic relation between two terms by means of EXACT, BROAD, NARROW and NO_relation relationships, which allows interconnecting the extracted terms and can be used for terminological enrichment, among other tasks.
 
 <!-- GETTING STARTED -->
 <a name="gettingstarted"/></a>
 ## 2. Getting Started
 [Back to ToC](#toc)
 
 <a name="installation"/></a>
 ### 2.1. Installation 
 Installation can be done using pypi:
 
 ```sh
-   pip install keybert
+   pip install keycare
 ```
 
 <a name="usage"/></a>
 ### 2.2. Usage 
-La librería se construye sobre X objetos principales:
-
-
+The library is built on 3 main processes:
 
 #### Term Extraction
-
+...
 
 #### Term Categorization
 
 
 #### Relation Extraction
 
+For further information on the functioning of the library refer to the tutorials in the nbs folder.
 
 <!-- CONTRIBUTING -->
 <a name="contributing"/></a>
 ## 3. Contributing
 [Back to ToC](#toc)
 
 This library has been developed with Python 3.8.2
@@ -131,8 +130,8 @@
 
 <a name="references"/></a>
 ## 5. References
 [Back to ToC](#toc)
 
 Please cite if you use the library in scientific works: 
 
-> PAPER TO BE PUBLISHED
+> PAPER TO BE PUBLISHED
```

#### html2text {}

```diff
@@ -11,32 +11,33 @@
 from a text: 1. **Keywords extraction**: KeyCARE implements several
 unsupervised term extraction techniques such as [*YAKE*](https://github.com/
 LIAAD/yake), [*RAKE*](https://pypi.org/project/rake-nltk/), [*TextRank*](https:
 //pypi.org/project/pytextrank/) or [*KeyBERT*](https://github.com/MaartenGr/
 KeyBERT) to automatically extract key terms from a text. 2. **Term
 categorization**: KeyCARE allows the application of term clustering techniques
 to group similar terms, as well as the training and application of supervised
-techniques to classify keywords into predefined categories. 3. **Semantic
-relation classification**: Beyond the identification and categorization of
-terms, the library supports the use of neural classification models to extract
-the semantic relation between two terms by means of EXACT, BROAD, NARROW and
-NO_relation relationships, which allows interconnecting the extracted terms and
-can be used for terminological enrichment, among other tasks. ## 2. Getting
-Started [Back to ToC](#toc) ### 2.1. Installation Installation can be done
-using pypi: ```sh pip install keybert ``` ### 2.2. Usage La librerÃ­a se
-construye sobre X objetos principales: #### Term Extraction #### Term
-Categorization #### Relation Extraction ## 3. Contributing [Back to ToC](#toc)
-This library has been developed with Python 3.8.2 Any contributions you make
-are **greatly appreciated**. For contributing: 1. Fork/Clone the Project in
-your system ```sh git clone https://github.com/nlp4bia-bsc/keycare.git ``` 2.
-Create a new virtual environment ```sh python3 -m venv .env_keycare ``` 3.
-Activate the new environment ```sh source .env_keycare/bin/activate ``` 4.
-Install the requirements ```sh pip install -r requirements.txt ``` 5. Create
-your Feature Branch (`git checkout -b feature/AmazingFeature`) 6. Update
-requirements file (`pip freeze > requirements.txt`) 7. Commit your Changes
-(`git commit -m 'Add some AmazingFeature'`) 8. Push to the Branch (`git push
-origin feature/AmazingFeature`) 9. Open a Pull Request from github. Follow
-[this tutorial](https://github.com/Kunena/Kunena-Forum/wiki/Create-a-new-
-branch-with-git-and-manage-branches) to create a branch. ## 4. License [Back to
-ToC](#toc) [Apache License, Version 2.0](https://www.apache.org/licenses/
-LICENSE-2.0) ## 5. References [Back to ToC](#toc) Please cite if you use the
-library in scientific works: > PAPER TO BE PUBLISHED
+techniques to classify keywords into predefined categories, including [SetFit].
+3. **Semantic relation classification**: Beyond the identification and
+categorization of terms, the library supports the use of neural classification
+models to extract the semantic relation between two terms by means of EXACT,
+BROAD, NARROW and NO_relation relationships, which allows interconnecting the
+extracted terms and can be used for terminological enrichment, among other
+tasks. ## 2. Getting Started [Back to ToC](#toc) ### 2.1. Installation
+Installation can be done using pypi: ```sh pip install keycare ``` ### 2.2.
+Usage The library is built on 3 main processes: #### Term Extraction ... ####
+Term Categorization #### Relation Extraction For further information on the
+functioning of the library refer to the tutorials in the nbs folder. ## 3.
+Contributing [Back to ToC](#toc) This library has been developed with Python
+3.8.2 Any contributions you make are **greatly appreciated**. For contributing:
+1. Fork/Clone the Project in your system ```sh git clone https://github.com/
+nlp4bia-bsc/keycare.git ``` 2. Create a new virtual environment ```sh python3 -
+m venv .env_keycare ``` 3. Activate the new environment ```sh source
+.env_keycare/bin/activate ``` 4. Install the requirements ```sh pip install -
+r requirements.txt ``` 5. Create your Feature Branch (`git checkout -b feature/
+AmazingFeature`) 6. Update requirements file (`pip freeze > requirements.txt`)
+7. Commit your Changes (`git commit -m 'Add some AmazingFeature'`) 8. Push to
+the Branch (`git push origin feature/AmazingFeature`) 9. Open a Pull Request
+from github. Follow [this tutorial](https://github.com/Kunena/Kunena-Forum/
+wiki/Create-a-new-branch-with-git-and-manage-branches) to create a branch. ##
+4. License [Back to ToC](#toc) [Apache License, Version 2.0](https://
+www.apache.org/licenses/LICENSE-2.0) ## 5. References [Back to ToC](#toc)
+Please cite if you use the library in scientific works: > PAPER TO BE PUBLISHED
```

### Comparing `keycare-0.0.1/keycare/keycare.egg-info/PKG-INFO` & `keycare-0.0.2/keycare/keycare.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycare
-Version: 0.0.1
+Version: 0.0.2
 Summary: KeyCARE is a Python library designed for the unsupervised keyword extraction from biomedical documents with the use of different algorithms, the classification of the keywords according to their semantic nature, and the extraction of is a relations among those keywords and with other terminologies.
 Author-email: Sergi Marsol <sergimarsolt@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 nlp4bia-bsc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -109,44 +109,43 @@
 
 <a name="about"/></a>
 ## 1. About The Project
 [Back to ToC](#toc)
 KeyBERT provides a common interface for extracting, categorizing and associating terms extracted from a text: 
 
 1. **Keywords extraction**: KeyCARE implements several unsupervised term extraction techniques such as [*YAKE*](https://github.com/LIAAD/yake), [*RAKE*](https://pypi.org/project/rake-nltk/), [*TextRank*](https://pypi.org/project/pytextrank/) or [*KeyBERT*](https://github.com/MaartenGr/KeyBERT) to automatically extract key terms from a text.
-2. **Term categorization**: KeyCARE allows the application of term clustering techniques to group similar terms, as well as the training and application of supervised techniques to classify keywords into predefined categories. 
+2. **Term categorization**: KeyCARE allows the application of term clustering techniques to group similar terms, as well as the training and application of supervised techniques to classify keywords into predefined categories, including [SetFit]. 
 3. **Semantic relation classification**: Beyond the identification and categorization of terms, the library supports the use of neural classification models to extract the semantic relation between two terms by means of EXACT, BROAD, NARROW and NO_relation relationships, which allows interconnecting the extracted terms and can be used for terminological enrichment, among other tasks.
 
 <!-- GETTING STARTED -->
 <a name="gettingstarted"/></a>
 ## 2. Getting Started
 [Back to ToC](#toc)
 
 <a name="installation"/></a>
 ### 2.1. Installation 
 Installation can be done using pypi:
 
 ```sh
-   pip install keybert
+   pip install keycare
 ```
 
 <a name="usage"/></a>
 ### 2.2. Usage 
-La librería se construye sobre X objetos principales:
-
-
+The library is built on 3 main processes:
 
 #### Term Extraction
-
+...
 
 #### Term Categorization
 
 
 #### Relation Extraction
 
+For further information on the functioning of the library refer to the tutorials in the nbs folder.
 
 <!-- CONTRIBUTING -->
 <a name="contributing"/></a>
 ## 3. Contributing
 [Back to ToC](#toc)
 
 This library has been developed with Python 3.8.2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: keycare Version: 0.0.1 Summary: KeyCARE is a Python
+Metadata-Version: 2.1 Name: keycare Version: 0.0.2 Summary: KeyCARE is a Python
 library designed for the unsupervised keyword extraction from biomedical
 documents with the use of different algorithms, the classification of the
 keywords according to their semantic nature, and the extraction of is a
 relations among those keywords and with other terminologies. Author-email:
 Sergi Marsol
 gmail.com> License: MIT License Copyright (c) 2023 nlp4bia-bsc Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
@@ -47,32 +47,33 @@
 from a text: 1. **Keywords extraction**: KeyCARE implements several
 unsupervised term extraction techniques such as [*YAKE*](https://github.com/
 LIAAD/yake), [*RAKE*](https://pypi.org/project/rake-nltk/), [*TextRank*](https:
 //pypi.org/project/pytextrank/) or [*KeyBERT*](https://github.com/MaartenGr/
 KeyBERT) to automatically extract key terms from a text. 2. **Term
 categorization**: KeyCARE allows the application of term clustering techniques
 to group similar terms, as well as the training and application of supervised
-techniques to classify keywords into predefined categories. 3. **Semantic
-relation classification**: Beyond the identification and categorization of
-terms, the library supports the use of neural classification models to extract
-the semantic relation between two terms by means of EXACT, BROAD, NARROW and
-NO_relation relationships, which allows interconnecting the extracted terms and
-can be used for terminological enrichment, among other tasks. ## 2. Getting
-Started [Back to ToC](#toc) ### 2.1. Installation Installation can be done
-using pypi: ```sh pip install keybert ``` ### 2.2. Usage La librerÃ­a se
-construye sobre X objetos principales: #### Term Extraction #### Term
-Categorization #### Relation Extraction ## 3. Contributing [Back to ToC](#toc)
-This library has been developed with Python 3.8.2 Any contributions you make
-are **greatly appreciated**. For contributing: 1. Fork/Clone the Project in
-your system ```sh git clone https://github.com/nlp4bia-bsc/keycare.git ``` 2.
-Create a new virtual environment ```sh python3 -m venv .env_keycare ``` 3.
-Activate the new environment ```sh source .env_keycare/bin/activate ``` 4.
-Install the requirements ```sh pip install -r requirements.txt ``` 5. Create
-your Feature Branch (`git checkout -b feature/AmazingFeature`) 6. Update
-requirements file (`pip freeze > requirements.txt`) 7. Commit your Changes
-(`git commit -m 'Add some AmazingFeature'`) 8. Push to the Branch (`git push
-origin feature/AmazingFeature`) 9. Open a Pull Request from github. Follow
-[this tutorial](https://github.com/Kunena/Kunena-Forum/wiki/Create-a-new-
-branch-with-git-and-manage-branches) to create a branch. ## 4. License [Back to
-ToC](#toc) [Apache License, Version 2.0](https://www.apache.org/licenses/
-LICENSE-2.0) ## 5. References [Back to ToC](#toc) Please cite if you use the
-library in scientific works: > PAPER TO BE PUBLISHED
+techniques to classify keywords into predefined categories, including [SetFit].
+3. **Semantic relation classification**: Beyond the identification and
+categorization of terms, the library supports the use of neural classification
+models to extract the semantic relation between two terms by means of EXACT,
+BROAD, NARROW and NO_relation relationships, which allows interconnecting the
+extracted terms and can be used for terminological enrichment, among other
+tasks. ## 2. Getting Started [Back to ToC](#toc) ### 2.1. Installation
+Installation can be done using pypi: ```sh pip install keycare ``` ### 2.2.
+Usage The library is built on 3 main processes: #### Term Extraction ... ####
+Term Categorization #### Relation Extraction For further information on the
+functioning of the library refer to the tutorials in the nbs folder. ## 3.
+Contributing [Back to ToC](#toc) This library has been developed with Python
+3.8.2 Any contributions you make are **greatly appreciated**. For contributing:
+1. Fork/Clone the Project in your system ```sh git clone https://github.com/
+nlp4bia-bsc/keycare.git ``` 2. Create a new virtual environment ```sh python3 -
+m venv .env_keycare ``` 3. Activate the new environment ```sh source
+.env_keycare/bin/activate ``` 4. Install the requirements ```sh pip install -
+r requirements.txt ``` 5. Create your Feature Branch (`git checkout -b feature/
+AmazingFeature`) 6. Update requirements file (`pip freeze > requirements.txt`)
+7. Commit your Changes (`git commit -m 'Add some AmazingFeature'`) 8. Push to
+the Branch (`git push origin feature/AmazingFeature`) 9. Open a Pull Request
+from github. Follow [this tutorial](https://github.com/Kunena/Kunena-Forum/
+wiki/Create-a-new-branch-with-git-and-manage-branches) to create a branch. ##
+4. License [Back to ToC](#toc) [Apache License, Version 2.0](https://
+www.apache.org/licenses/LICENSE-2.0) ## 5. References [Back to ToC](#toc)
+Please cite if you use the library in scientific works: > PAPER TO BE PUBLISHED
```

### Comparing `keycare-0.0.1/pyproject.toml` & `keycare-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,19 @@
     "setuptools>=69.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["keycare"]
-include = []
 exclude = ["tests"]
 
 [project]
 name = "keycare"
-version = "0.0.1"
+version = "0.0.2"
 description = "KeyCARE is a Python library designed for the unsupervised keyword extraction from biomedical documents with the use of different algorithms, the classification of the keywords according to their semantic nature, and the extraction of is a relations among those keywords and with other terminologies."
 readme = "README.md"
 authors = [{ name = "Sergi Marsol", email = "sergimarsolt@gmail.com" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 dependencies = [
     "datasets==2.14.4",
```


# Comparing `tmp/preprocessinglib_tonga_gumustakim-0.4.tar.gz` & `tmp/preprocessinglib_tonga_gumustakim-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preprocessinglib_tonga_gumustakim-0.4.tar", last modified: Thu May 23 11:01:36 2024, max compression
+gzip compressed data, was "preprocessinglib_tonga_gumustakim-0.5.tar", last modified: Fri May 24 11:38:28 2024, max compression
```

## Comparing `preprocessinglib_tonga_gumustakim-0.4.tar` & `preprocessinglib_tonga_gumustakim-0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 11:01:36.134554 preprocessinglib_tonga_gumustakim-0.4/
--rw-rw-rw-   0        0        0     3230 2024-05-23 11:01:36.131906 preprocessinglib_tonga_gumustakim-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2546 2024-05-21 20:13:01.000000 preprocessinglib_tonga_gumustakim-0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 11:01:36.083415 preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim/
--rw-rw-rw-   0        0        0      664 2024-05-21 15:21:25.000000 preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim/CategoricalEncoder.py
--rw-rw-rw-   0        0        0      459 2024-05-21 15:31:42.000000 preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim/DataTypeConverter.py
--rw-rw-rw-   0        0        0      380 2024-05-21 17:04:39.000000 preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim/DateTimeHandler.py
--rw-rw-rw-   0        0        0      212 2024-05-21 15:39:43.000000 preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim/FeatureEngineer.py
--rw-rw-rw-   0        0        0      920 2024-05-21 15:41:03.000000 preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim/MissingValueHandler.py
--rw-rw-rw-   0        0        0      711 2024-05-21 16:01:47.000000 preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim/OutlierHandler.py
--rw-rw-rw-   0        0        0     1032 2024-05-23 10:59:37.000000 preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim/Scaler.py
--rw-rw-rw-   0        0        0     4903 2024-05-23 09:29:07.000000 preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim/TestDataPreprocessing.py
--rw-rw-rw-   0        0        0      665 2024-05-21 15:42:19.000000 preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim/TextCleaner.py
--rw-rw-rw-   0        0        0      255 2024-05-23 09:29:07.000000 preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:01:36.126840 preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim.egg-info/
--rw-rw-rw-   0        0        0     3230 2024-05-23 11:01:35.000000 preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      826 2024-05-23 11:01:35.000000 preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 11:01:35.000000 preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-23 11:01:35.000000 preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2024-05-23 11:01:35.000000 preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 11:01:36.134554 preprocessinglib_tonga_gumustakim-0.4/setup.cfg
--rw-rw-rw-   0        0        0      898 2024-05-23 11:01:03.000000 preprocessinglib_tonga_gumustakim-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 11:38:28.981406 preprocessinglib_tonga_gumustakim-0.5/
+-rw-rw-rw-   0        0        0     3252 2024-05-24 11:38:28.978945 preprocessinglib_tonga_gumustakim-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2546 2024-05-21 20:13:01.000000 preprocessinglib_tonga_gumustakim-0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 11:38:28.946925 preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim/
+-rw-rw-rw-   0        0        0      664 2024-05-21 15:21:25.000000 preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim/CategoricalEncoder.py
+-rw-rw-rw-   0        0        0      459 2024-05-21 15:31:42.000000 preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim/DataTypeConverter.py
+-rw-rw-rw-   0        0        0      380 2024-05-21 17:04:39.000000 preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim/DateTimeHandler.py
+-rw-rw-rw-   0        0        0      212 2024-05-21 15:39:43.000000 preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim/FeatureEngineer.py
+-rw-rw-rw-   0        0        0      920 2024-05-21 15:41:03.000000 preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim/MissingValueHandler.py
+-rw-rw-rw-   0        0        0      711 2024-05-21 16:01:47.000000 preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim/OutlierHandler.py
+-rw-rw-rw-   0        0        0      510 2024-05-21 15:31:42.000000 preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim/Scaler.py
+-rw-rw-rw-   0        0        0     6227 2024-05-24 11:03:06.000000 preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim/TestDataPreprocessing.py
+-rw-rw-rw-   0        0        0      807 2024-05-24 11:18:19.000000 preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim/TextCleaner.py
+-rw-rw-rw-   0        0        0      306 2024-05-24 08:54:56.000000 preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 11:38:28.975641 preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim.egg-info/
+-rw-rw-rw-   0        0        0     3252 2024-05-24 11:38:28.000000 preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      826 2024-05-24 11:38:28.000000 preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 11:38:28.000000 preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-24 11:38:28.000000 preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2024-05-24 11:38:28.000000 preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 11:38:28.982494 preprocessinglib_tonga_gumustakim-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      916 2024-05-24 11:30:18.000000 preprocessinglib_tonga_gumustakim-0.5/setup.py
```

### Comparing `preprocessinglib_tonga_gumustakim-0.4/PKG-INFO` & `preprocessinglib_tonga_gumustakim-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: preprocessinglib_tonga_gumustakim
-Version: 0.4
+Version: 0.5
 Summary: A comprehensive data preprocessing library for Python
 Home-page: https://github.com/Fzehzeh/mypreprocessinglib , https://github.com/ayserragm/mypreprocessinglib
 Author: Zehra Tonga-Ayse Serra Gumustakim
 Author-email: tongafatmazehra@gmail.com-ayseserra.gumustakim@stu.fsm.edu.tr 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
 Requires-Dist: nltk
+Requires-Dist: numpy
 
 PreprocessingLib
 PreprocessingLib is a Python library designed to facilitate data preprocessing steps. It provides various classes and functions to automate the process of cleaning, transforming, and engineering features in datasets.
 
 Features
 1. Missing Value Handling
 Detect missing values in a dataset.
```

### Comparing `preprocessinglib_tonga_gumustakim-0.4/README.md` & `preprocessinglib_tonga_gumustakim-0.5/README.md`

 * *Files identical despite different names*

### Comparing `preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim/CategoricalEncoder.py` & `preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim/CategoricalEncoder.py`

 * *Files identical despite different names*

### Comparing `preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim/MissingValueHandler.py` & `preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim/MissingValueHandler.py`

 * *Files identical despite different names*

### Comparing `preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim/OutlierHandler.py` & `preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim/OutlierHandler.py`

 * *Files identical despite different names*

### Comparing `preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim/TestDataPreprocessing.py` & `preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim/TestDataPreprocessing.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 import pandas as pd
 from preprocessinglib_tonga_gumustakim.MissingValueHandler import MissingValueHandler
 from preprocessinglib_tonga_gumustakim.FeatureEngineer import FeatureEngineer
 from preprocessinglib_tonga_gumustakim.DateTimeHandler import DateTimeHandler
 from preprocessinglib_tonga_gumustakim.DataTypeConverter import DataTypeConverter
 from preprocessinglib_tonga_gumustakim.CategoricalEncoder import CategoricalEncoder
 from preprocessinglib_tonga_gumustakim.OutlierHandler import OutlierHandler
-
-pd.set_option('display.max_columns', None)
+from preprocessinglib_tonga_gumustakim.TextCleaner import TextCleaner
+from preprocessinglib_tonga_gumustakim.Scaler import Scaler
 
 
 class TestDataPreprocessing(unittest.TestCase):
+    pd.set_option('display.max_columns', None)
+    data = pd.read_csv('C:/Users/EMRULLAH/Downloads/synthetic_sample_data_minimal.csv')
 
     @classmethod
     def setUpClass(cls):
-        filepath = r"C:\Users\EMRULLAH\Downloads\synthetic_sample_data.csv"
+        filepath = r"C:\Users\EMRULLAH\Downloads\synthetic_sample_data_minimal.csv"
         cls.data = pd.read_csv(filepath)
 
     def test_detect_missing_values(self):
         missing_handler = MissingValueHandler()
         result = missing_handler.detect_missing_values(self.data)
         expected_result = self.data.isnull().sum()
         self.assertTrue(result.equals(expected_result))
@@ -97,9 +99,42 @@
     def test_handle_outliers(self):
         outliers_removed_data = OutlierHandler.handle_outliers(self.data.select_dtypes(include=['number']),
                                                                method='drop')
         self.assertFalse(outliers_removed_data.isnull().values.any())
         print("Data after handling outliers:")
         print(outliers_removed_data.head())
 
+    def test_clean_text(self):
+        # Örnek bir metin oluştur
+        text_column = "Summary"
+
+        # Metni temizle
+        cleaned_text = TextCleaner.clean_text(self.data[text_column].values)
+
+        # Temizlenmiş metni kontrol et
+        print("Cleaned text:")
+        print(cleaned_text)
+
+    def test_standardize_data(self):
+        # Ölçeklendirme için bir veri seti seç
+        data_to_scale = self.data.select_dtypes(include=['number'])
+
+        # Veriyi standartlaştır
+        standardized_data = Scaler.standardize_data(data_to_scale)
+
+        # Standartlaştırılmış veriyi kontrol et
+        print("Standardized data:")
+        print(standardized_data.head())
+
+    def test_normalize_data(self):
+        # Ölçeklendirme için bir veri seti seç
+        data_to_scale = self.data.select_dtypes(include=['number'])
+
+        # Veriyi normalize et
+        normalized_data = Scaler.normalize_data(data_to_scale)
+
+        # Normalize edilmiş veriyi kontrol et
+        print("Normalized data:")
+        print(normalized_data.head())
+
     if __name__ == '__main__':
         unittest.main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim/TextCleaner.py` & `preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim/TextCleaner.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 from nltk.corpus import stopwords
 from nltk.tokenize import word_tokenize
 from nltk.stem import WordNetLemmatizer
 
 
 class TextCleaner:
     @staticmethod
-    def clean_text(text, tokenize=True):
-        text = text.lower()
-        text = text.translate(str.maketrans('', '', string.punctuation))
-        stop_words = set(stopwords.words('english'))
-        word_tokens = word_tokenize(text)
-
-        filtered_words = [word for word in word_tokens if word not in stop_words]
-        lemmatizer = WordNetLemmatizer()
-        cleaned_text = ' '.join([lemmatizer.lemmatize(word) for word in filtered_words])
-        return cleaned_text
+    def clean_text(text_array, tokenize=True):
+        cleaned_texts = []
+        for text in text_array:
+            text = text.lower()
+            text = text.translate(str.maketrans('', '', string.punctuation))
+            stop_words = set(stopwords.words('english'))
+            word_tokens = word_tokenize(text)
+            filtered_words = [word for word in word_tokens if word not in stop_words]
+            lemmatizer = WordNetLemmatizer()
+            cleaned_text = ' '.join([lemmatizer.lemmatize(word) for word in filtered_words])
+            cleaned_texts.append(cleaned_text)
+        return cleaned_texts
```

### Comparing `preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim.egg-info/PKG-INFO` & `preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: preprocessinglib_tonga_gumustakim
-Version: 0.4
+Version: 0.5
 Summary: A comprehensive data preprocessing library for Python
 Home-page: https://github.com/Fzehzeh/mypreprocessinglib , https://github.com/ayserragm/mypreprocessinglib
 Author: Zehra Tonga-Ayse Serra Gumustakim
 Author-email: tongafatmazehra@gmail.com-ayseserra.gumustakim@stu.fsm.edu.tr 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
 Requires-Dist: nltk
+Requires-Dist: numpy
 
 PreprocessingLib
 PreprocessingLib is a Python library designed to facilitate data preprocessing steps. It provides various classes and functions to automate the process of cleaning, transforming, and engineering features in datasets.
 
 Features
 1. Missing Value Handling
 Detect missing values in a dataset.
```

### Comparing `preprocessinglib_tonga_gumustakim-0.4/preprocessinglib_tonga_gumustakim.egg-info/SOURCES.txt` & `preprocessinglib_tonga_gumustakim-0.5/preprocessinglib_tonga_gumustakim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `preprocessinglib_tonga_gumustakim-0.4/setup.py` & `preprocessinglib_tonga_gumustakim-0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='preprocessinglib_tonga_gumustakim',
-    version='0.4',
+    version='0.5',
     packages=find_packages(),
     install_requires=[
         'pandas',
         'numpy',
         'scikit-learn',
-        'nltk'
+        'nltk',
+        'numpy'
     ],
     author='Zehra Tonga-Ayse Serra Gumustakim',
     author_email='tongafatmazehra@gmail.com-ayseserra.gumustakim@stu.fsm.edu.tr ',
     description='A comprehensive data preprocessing library for Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Fzehzeh/mypreprocessinglib , https://github.com/ayserragm/mypreprocessinglib',
```


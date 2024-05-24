# Comparing `tmp/SIST02_converter-0.1.2.tar.gz` & `tmp/SIST02-Converter-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SIST02_converter-0.1.2.tar", last modified: Fri May 24 09:16:07 2024, max compression
+gzip compressed data, was "SIST02-Converter-0.1.3.tar", last modified: Fri May 24 11:15:29 2024, max compression
```

## Comparing `SIST02_converter-0.1.2.tar` & `SIST02-Converter-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yasufumi   (501) staff       (20)        0 2024-05-24 09:16:07.115496 SIST02_converter-0.1.2/
--rw-r--r--   0 yasufumi   (501) staff       (20)     1353 2024-05-24 09:16:07.115348 SIST02_converter-0.1.2/PKG-INFO
--rw-r--r--   0 yasufumi   (501) staff       (20)     1144 2024-05-24 09:15:39.000000 SIST02_converter-0.1.2/README.md
-drwxr-xr-x   0 yasufumi   (501) staff       (20)        0 2024-05-24 09:16:07.114590 SIST02_converter-0.1.2/SIST02_converter/
--rw-r--r--   0 yasufumi   (501) staff       (20)     2122 2024-05-24 09:11:07.000000 SIST02_converter-0.1.2/SIST02_converter/SIST02_convert_URL.py
--rw-r--r--   0 yasufumi   (501) staff       (20)       43 2024-05-24 09:11:56.000000 SIST02_converter-0.1.2/SIST02_converter/__init__.py
-drwxr-xr-x   0 yasufumi   (501) staff       (20)        0 2024-05-24 09:16:07.115166 SIST02_converter-0.1.2/SIST02_converter.egg-info/
--rw-r--r--   0 yasufumi   (501) staff       (20)     1353 2024-05-24 09:16:07.000000 SIST02_converter-0.1.2/SIST02_converter.egg-info/PKG-INFO
--rw-r--r--   0 yasufumi   (501) staff       (20)      246 2024-05-24 09:16:07.000000 SIST02_converter-0.1.2/SIST02_converter.egg-info/SOURCES.txt
--rw-r--r--   0 yasufumi   (501) staff       (20)        1 2024-05-24 09:16:07.000000 SIST02_converter-0.1.2/SIST02_converter.egg-info/dependency_links.txt
--rw-r--r--   0 yasufumi   (501) staff       (20)       17 2024-05-24 09:16:07.000000 SIST02_converter-0.1.2/SIST02_converter.egg-info/top_level.txt
--rw-r--r--   0 yasufumi   (501) staff       (20)       38 2024-05-24 09:16:07.115550 SIST02_converter-0.1.2/setup.cfg
--rw-r--r--   0 yasufumi   (501) staff       (20)      541 2024-05-24 09:15:53.000000 SIST02_converter-0.1.2/setup.py
+drwxr-xr-x   0 yasufumi   (501) staff       (20)        0 2024-05-24 11:15:29.426913 SIST02-Converter-0.1.3/
+-rw-r--r--   0 yasufumi   (501) staff       (20)     1371 2024-05-24 11:15:29.426755 SIST02-Converter-0.1.3/PKG-INFO
+-rw-r--r--   0 yasufumi   (501) staff       (20)     1164 2024-05-24 11:15:00.000000 SIST02-Converter-0.1.3/README.md
+drwxr-xr-x   0 yasufumi   (501) staff       (20)        0 2024-05-24 11:15:29.425867 SIST02-Converter-0.1.3/SIST02_Converter.egg-info/
+-rw-r--r--   0 yasufumi   (501) staff       (20)     1371 2024-05-24 11:15:29.000000 SIST02-Converter-0.1.3/SIST02_Converter.egg-info/PKG-INFO
+-rw-r--r--   0 yasufumi   (501) staff       (20)      246 2024-05-24 11:15:29.000000 SIST02-Converter-0.1.3/SIST02_Converter.egg-info/SOURCES.txt
+-rw-r--r--   0 yasufumi   (501) staff       (20)        1 2024-05-24 11:15:29.000000 SIST02-Converter-0.1.3/SIST02_Converter.egg-info/dependency_links.txt
+-rw-r--r--   0 yasufumi   (501) staff       (20)       17 2024-05-24 11:15:29.000000 SIST02-Converter-0.1.3/SIST02_Converter.egg-info/top_level.txt
+drwxr-xr-x   0 yasufumi   (501) staff       (20)        0 2024-05-24 11:15:29.426399 SIST02-Converter-0.1.3/SIST02_converter/
+-rw-r--r--   0 yasufumi   (501) staff       (20)     2122 2024-05-24 09:11:07.000000 SIST02-Converter-0.1.3/SIST02_converter/SIST02_convert_URL.py
+-rw-r--r--   0 yasufumi   (501) staff       (20)       43 2024-05-24 09:11:56.000000 SIST02-Converter-0.1.3/SIST02_converter/__init__.py
+-rw-r--r--   0 yasufumi   (501) staff       (20)       38 2024-05-24 11:15:29.426972 SIST02-Converter-0.1.3/setup.cfg
+-rw-r--r--   0 yasufumi   (501) staff       (20)      539 2024-05-24 11:15:14.000000 SIST02-Converter-0.1.3/setup.py
```

### Comparing `SIST02_converter-0.1.2/PKG-INFO` & `SIST02-Converter-0.1.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,33 @@
-Metadata-Version: 2.1
-Name: SIST02_converter
-Version: 0.1.2
-Summary: Conversion of input URLs to SIST02 format.
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 ### パッケージについて
 
-ようこそ、**SIST02_converter** へ！
+ようこそ、**SIST02-converter** へ！
 
-**SIST02_converter** は、参考文献として使用したWebサイトをSIST02スタイルに変換する作業を簡略化することを目的とした Python ライブラリです。初心者から経験豊富な開発者まで、**SIST02_converter** は直感的なツールとユーティリティを提供し、Python プロジェクトのワークフローを支援します。
+**SIST02-converter** は、参考文献として使用したWebサイトをSIST02スタイルに変換する作業を簡略化することを目的とした Python ライブラリです。初心者から経験豊富な開発者まで、**SIST02-converter** は直感的なツールとユーティリティを提供し、Python プロジェクトのワークフローを支援します。
 
 ### 主な特徴
 
-- [入力されたURLからSIST02スタイルに変換したテキストを出力します]
+- 入力されたURLからSIST02スタイルに変換したテキストを出力します
 
 ### インストール
 
-pip を使用して **SIST02_converter** をインストールできます:
+pip を使用して **SIST02-converter** をインストールできます
 
 ```bash
-pip install SIST02_converter
+pip install SIST02-converter
 ```
 
 ### 使用法
 
-ここでは、**SIST02_converter** の使用方法の簡単な例を示します:
+ここでは、**SIST02-converter** の使用方法の簡単な例を示します
 
 ```python
 from SIST02_converter import Convert_URL
 
-text = Convert_URL('url')
+url = "https://example.com"
+text = Convert-URL(url)
 print(text)
 ```
 
 ### ライセンス
 
-**SIST02_converter** は [MIT ライセンス] の下でライセンスされています。これは、個人および商用のプロジェクトの両方で自由に使用できることを意味します。
-
+**SIST02_converter** は MIT ライセンス の下でライセンスされています。これは、個人および商用のプロジェクトの両方で自由に使用できることを意味します。
```

### Comparing `SIST02_converter-0.1.2/SIST02_converter/SIST02_convert_URL.py` & `SIST02-Converter-0.1.3/SIST02_converter/SIST02_convert_URL.py`

 * *Files identical despite different names*

### Comparing `SIST02_converter-0.1.2/SIST02_converter.egg-info/PKG-INFO` & `SIST02-Converter-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 Metadata-Version: 2.1
-Name: SIST02-converter
-Version: 0.1.2
-Summary: Conversion of input URLs to SIST02 format.
+Name: SIST02-Converter
+Version: 0.1.3
+Summary: Conversion of input URL to SIST02 style.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 ### パッケージについて
 
-ようこそ、**SIST02_converter** へ！
+ようこそ、**SIST02-converter** へ！
 
-**SIST02_converter** は、参考文献として使用したWebサイトをSIST02スタイルに変換する作業を簡略化することを目的とした Python ライブラリです。初心者から経験豊富な開発者まで、**SIST02_converter** は直感的なツールとユーティリティを提供し、Python プロジェクトのワークフローを支援します。
+**SIST02-converter** は、参考文献として使用したWebサイトをSIST02スタイルに変換する作業を簡略化することを目的とした Python ライブラリです。初心者から経験豊富な開発者まで、**SIST02-converter** は直感的なツールとユーティリティを提供し、Python プロジェクトのワークフローを支援します。
 
 ### 主な特徴
 
-- [入力されたURLからSIST02スタイルに変換したテキストを出力します]
+- 入力されたURLからSIST02スタイルに変換したテキストを出力します
 
 ### インストール
 
-pip を使用して **SIST02_converter** をインストールできます:
+pip を使用して **SIST02-converter** をインストールできます
 
 ```bash
-pip install SIST02_converter
+pip install SIST02-converter
 ```
 
 ### 使用法
 
-ここでは、**SIST02_converter** の使用方法の簡単な例を示します:
+ここでは、**SIST02-converter** の使用方法の簡単な例を示します
 
 ```python
 from SIST02_converter import Convert_URL
 
-text = Convert_URL('url')
+url = "https://example.com"
+text = Convert-URL(url)
 print(text)
 ```
 
 ### ライセンス
 
-**SIST02_converter** は [MIT ライセンス] の下でライセンスされています。これは、個人および商用のプロジェクトの両方で自由に使用できることを意味します。
+**SIST02_converter** は MIT ライセンス の下でライセンスされています。これは、個人および商用のプロジェクトの両方で自由に使用できることを意味します。
```

### Comparing `SIST02_converter-0.1.2/setup.py` & `SIST02-Converter-0.1.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent
 long_description = (here / "README.md").read_text(encoding="utf-8")
 setup(
-    name="SIST02_converter",
-    version="0.1.2",
+    name="SIST02-Converter",
+    version="0.1.3",
     LICENSE = 'MIT',
-    description="Conversion of input URLs to SIST02 format.",
+    description="Conversion of input URL to SIST02 style.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     CLASSIFIERS=[
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6'
     ],
```


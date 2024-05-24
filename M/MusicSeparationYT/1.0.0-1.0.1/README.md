# Comparing `tmp/musicseparationyt-1.0.0.tar.gz` & `tmp/musicseparationyt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicseparationyt-1.0.0.tar", last modified: Fri May 24 11:44:32 2024, max compression
+gzip compressed data, was "musicseparationyt-1.0.1.tar", last modified: Fri May 24 12:29:45 2024, max compression
```

## Comparing `musicseparationyt-1.0.0.tar` & `musicseparationyt-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-24 11:44:32.522786 musicseparationyt-1.0.0/
--rw-r--r--   0 yrry       (501) staff       (20)     1051 2024-05-24 09:16:34.000000 musicseparationyt-1.0.0/LICENSE
-drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-24 11:44:32.522294 musicseparationyt-1.0.0/MusicSeparationYT.egg-info/
--rw-r--r--   0 yrry       (501) staff       (20)      525 2024-05-24 11:44:32.000000 musicseparationyt-1.0.0/MusicSeparationYT.egg-info/PKG-INFO
--rw-r--r--   0 yrry       (501) staff       (20)      230 2024-05-24 11:44:32.000000 musicseparationyt-1.0.0/MusicSeparationYT.egg-info/SOURCES.txt
--rw-r--r--   0 yrry       (501) staff       (20)        1 2024-05-24 11:44:32.000000 musicseparationyt-1.0.0/MusicSeparationYT.egg-info/dependency_links.txt
--rw-r--r--   0 yrry       (501) staff       (20)       21 2024-05-24 11:44:32.000000 musicseparationyt-1.0.0/MusicSeparationYT.egg-info/requires.txt
--rw-r--r--   0 yrry       (501) staff       (20)        1 2024-05-24 11:44:32.000000 musicseparationyt-1.0.0/MusicSeparationYT.egg-info/top_level.txt
--rw-r--r--   0 yrry       (501) staff       (20)      525 2024-05-24 11:44:32.522569 musicseparationyt-1.0.0/PKG-INFO
--rw-r--r--   0 yrry       (501) staff       (20)       86 2024-05-24 11:29:39.000000 musicseparationyt-1.0.0/README.md
--rw-r--r--   0 yrry       (501) staff       (20)       38 2024-05-24 11:44:32.522840 musicseparationyt-1.0.0/setup.cfg
--rw-r--r--   0 yrry       (501) staff       (20)     1149 2024-05-24 11:44:30.000000 musicseparationyt-1.0.0/setup.py
+drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-24 12:29:45.997928 musicseparationyt-1.0.1/
+-rw-r--r--   0 yrry       (501) staff       (20)     1051 2024-05-24 09:16:34.000000 musicseparationyt-1.0.1/LICENSE
+drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-24 12:29:45.997366 musicseparationyt-1.0.1/MusicSeparationYT.egg-info/
+-rw-r--r--   0 yrry       (501) staff       (20)      563 2024-05-24 12:29:45.000000 musicseparationyt-1.0.1/MusicSeparationYT.egg-info/PKG-INFO
+-rw-r--r--   0 yrry       (501) staff       (20)      294 2024-05-24 12:29:45.000000 musicseparationyt-1.0.1/MusicSeparationYT.egg-info/SOURCES.txt
+-rw-r--r--   0 yrry       (501) staff       (20)        1 2024-05-24 12:29:45.000000 musicseparationyt-1.0.1/MusicSeparationYT.egg-info/dependency_links.txt
+-rw-r--r--   0 yrry       (501) staff       (20)       44 2024-05-24 12:29:45.000000 musicseparationyt-1.0.1/MusicSeparationYT.egg-info/requires.txt
+-rw-r--r--   0 yrry       (501) staff       (20)       22 2024-05-24 12:29:45.000000 musicseparationyt-1.0.1/MusicSeparationYT.egg-info/top_level.txt
+drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-24 12:29:45.997177 musicseparationyt-1.0.1/MusicSeparationYTMain/
+-rw-r--r--   0 yrry       (501) staff       (20)       68 2024-05-24 12:29:22.000000 musicseparationyt-1.0.1/MusicSeparationYTMain/__init__.py
+-rw-r--r--   0 yrry       (501) staff       (20)     1109 2024-05-24 12:25:08.000000 musicseparationyt-1.0.1/MusicSeparationYTMain/main.py
+-rw-r--r--   0 yrry       (501) staff       (20)      563 2024-05-24 12:29:45.997706 musicseparationyt-1.0.1/PKG-INFO
+-rw-r--r--   0 yrry       (501) staff       (20)       86 2024-05-24 11:51:34.000000 musicseparationyt-1.0.1/README.md
+-rw-r--r--   0 yrry       (501) staff       (20)       38 2024-05-24 12:29:45.997975 musicseparationyt-1.0.1/setup.cfg
+-rw-r--r--   0 yrry       (501) staff       (20)     1321 2024-05-24 12:29:37.000000 musicseparationyt-1.0.1/setup.py
```

### Comparing `musicseparationyt-1.0.0/LICENSE` & `musicseparationyt-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `musicseparationyt-1.0.0/setup.py` & `musicseparationyt-1.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 #!/usr/bin/env python3
 
+# from setuptools import setup, find_packages
 import setuptools
+# from setuptools import find_packages
 
 # パッケージの基本情報
 name = "MusicSeparationYT"  # パッケージ名
-version = "1.0.0"  # バージョン番号
+version = "1.0.1"  # バージョン番号
 description = "this tool music download and seprate"  # パッケージの説明
+long_description_content_type="text/markdown",
 author = "Y-Ryohei"  # 作者名
 author_email = ""  # 作者のメールアドレス
 url = "https://github.com/Y-Ryohei/MusicSeparationYT"  # リポジトリURL
 license = "MIT"  # ライセンス
 
 # インストールに必要な依存関係
 requirements = [
-  'pytube'
-  'moviepy',
-  'demucs',
+  'pytube==15.0.0',
+  'moviepy==1.0.3',
+  'demucs==4.0.3',
 ]
 
 # パッケージに含めるモジュール
-packages = [
-]
+# packages = find_packages(),
 
 # その他の情報
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.6",
@@ -37,10 +39,10 @@
     version=version,
     description=description,
     author=author,
     author_email=author_email,
     url=url,
     license=license,
     install_requires=requirements,
-    packages=packages,
+    # packages=packages,
     classifiers=classifiers,
 )
```


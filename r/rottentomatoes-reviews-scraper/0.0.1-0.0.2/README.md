# Comparing `tmp/rottentomatoes-reviews-scraper-0.0.1.tar.gz` & `tmp/rottentomatoes-reviews-scraper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rottentomatoes-reviews-scraper-0.0.1.tar", last modified: Fri May 24 09:15:27 2024, max compression
+gzip compressed data, was "rottentomatoes-reviews-scraper-0.0.2.tar", last modified: Fri May 24 09:19:28 2024, max compression
```

## Comparing `rottentomatoes-reviews-scraper-0.0.1.tar` & `rottentomatoes-reviews-scraper-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-24 09:15:27.771403 rottentomatoes-reviews-scraper-0.0.1/
--rw-r--r--   0 hwai12     (501) staff       (20)     2661 2024-05-24 09:15:27.771257 rottentomatoes-reviews-scraper-0.0.1/PKG-INFO
--rw-r--r--   0 hwai12     (501) staff       (20)     2106 2024-05-24 09:07:13.000000 rottentomatoes-reviews-scraper-0.0.1/README.md
--rw-r--r--   0 hwai12     (501) staff       (20)       38 2024-05-24 09:15:27.771454 rottentomatoes-reviews-scraper-0.0.1/setup.cfg
--rw-r--r--   0 hwai12     (501) staff       (20)      948 2024-05-24 09:15:06.000000 rottentomatoes-reviews-scraper-0.0.1/setup.py
-drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-24 09:15:27.769998 rottentomatoes-reviews-scraper-0.0.1/src/
-drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-24 09:15:27.771060 rottentomatoes-reviews-scraper-0.0.1/src/rottentomatoes_reviews_scraper.egg-info/
--rw-r--r--   0 hwai12     (501) staff       (20)     2661 2024-05-24 09:15:27.000000 rottentomatoes-reviews-scraper-0.0.1/src/rottentomatoes_reviews_scraper.egg-info/PKG-INFO
--rw-r--r--   0 hwai12     (501) staff       (20)      368 2024-05-24 09:15:27.000000 rottentomatoes-reviews-scraper-0.0.1/src/rottentomatoes_reviews_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 hwai12     (501) staff       (20)        1 2024-05-24 09:15:27.000000 rottentomatoes-reviews-scraper-0.0.1/src/rottentomatoes_reviews_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 hwai12     (501) staff       (20)       62 2024-05-24 09:15:27.000000 rottentomatoes-reviews-scraper-0.0.1/src/rottentomatoes_reviews_scraper.egg-info/entry_points.txt
--rw-r--r--   0 hwai12     (501) staff       (20)       25 2024-05-24 09:15:27.000000 rottentomatoes-reviews-scraper-0.0.1/src/rottentomatoes_reviews_scraper.egg-info/requires.txt
--rw-r--r--   0 hwai12     (501) staff       (20)        1 2024-05-24 09:15:27.000000 rottentomatoes-reviews-scraper-0.0.1/src/rottentomatoes_reviews_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-24 09:19:28.614057 rottentomatoes-reviews-scraper-0.0.2/
+-rw-r--r--   0 hwai12     (501) staff       (20)     2685 2024-05-24 09:19:28.613911 rottentomatoes-reviews-scraper-0.0.2/PKG-INFO
+-rw-r--r--   0 hwai12     (501) staff       (20)     2130 2024-05-24 09:18:21.000000 rottentomatoes-reviews-scraper-0.0.2/README.md
+-rw-r--r--   0 hwai12     (501) staff       (20)       38 2024-05-24 09:19:28.614110 rottentomatoes-reviews-scraper-0.0.2/setup.cfg
+-rw-r--r--   0 hwai12     (501) staff       (20)      948 2024-05-24 09:19:00.000000 rottentomatoes-reviews-scraper-0.0.2/setup.py
+drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-24 09:19:28.612687 rottentomatoes-reviews-scraper-0.0.2/src/
+drwxr-xr-x   0 hwai12     (501) staff       (20)        0 2024-05-24 09:19:28.613714 rottentomatoes-reviews-scraper-0.0.2/src/rottentomatoes_reviews_scraper.egg-info/
+-rw-r--r--   0 hwai12     (501) staff       (20)     2685 2024-05-24 09:19:28.000000 rottentomatoes-reviews-scraper-0.0.2/src/rottentomatoes_reviews_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 hwai12     (501) staff       (20)      368 2024-05-24 09:19:28.000000 rottentomatoes-reviews-scraper-0.0.2/src/rottentomatoes_reviews_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 hwai12     (501) staff       (20)        1 2024-05-24 09:19:28.000000 rottentomatoes-reviews-scraper-0.0.2/src/rottentomatoes_reviews_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 hwai12     (501) staff       (20)       62 2024-05-24 09:19:28.000000 rottentomatoes-reviews-scraper-0.0.2/src/rottentomatoes_reviews_scraper.egg-info/entry_points.txt
+-rw-r--r--   0 hwai12     (501) staff       (20)       25 2024-05-24 09:19:28.000000 rottentomatoes-reviews-scraper-0.0.2/src/rottentomatoes_reviews_scraper.egg-info/requires.txt
+-rw-r--r--   0 hwai12     (501) staff       (20)        1 2024-05-24 09:19:28.000000 rottentomatoes-reviews-scraper-0.0.2/src/rottentomatoes_reviews_scraper.egg-info/top_level.txt
```

### Comparing `rottentomatoes-reviews-scraper-0.0.1/PKG-INFO` & `rottentomatoes-reviews-scraper-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rottentomatoes-reviews-scraper
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package to scrape movie data from Rotten Tomatoes, including titles and reviews.
 Home-page: https://github.com/HwaI12/rottentomatoes-reviews-scraper
 Author: Fami Ishikawa
 Author-email: s2222061@stu.musashino-u.ac.jp
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -40,29 +40,29 @@
 ## Installation / インストール
 
 To install the package, use pip:
 
 パッケージをインストールするには、pipを使用します：
 
 ```sh
-pip install rottentomatoes-scraper
+pip install rottentomatoes-reviews-scraper
 ```
 
 ## Usage / 使い方
 
 After installing the package, you can use the command line interface to scrape data. Here is an example of how to use the package from the terminal:
 
 パッケージをインストールした後、コマンドラインインターフェースを使用してデータをスクレイピングできます。
 
 Set the number of movies to retrieve and the number of reviews to retrieve
 
 取得する映画数と取得するレビュー数を設定します。
 
 ```sh
-rottentomatoes-scraper --count_title 20 --count_review 20
+rottentomatoes-reviews-scraper --count_title 20 --count_review 20
 ```
 
 This command will first scrape 20 movie titles and then scrape 20 reviews for each of those movies.
 
 このコマンドは、最初に20の映画タイトルをスクレイピングし、その後各映画の20のレビューをスクレイピングします。
 
 ## Command Line Arguments / コマンドライン引数
@@ -76,10 +76,10 @@
 ## Example / 例
 
 Here is an example of how to run the scraper:
 
 スクレイパーを実行する例を以下に示します：
 
 ```sh
-rottentomatoes-scraper --count_title 20 --count_review 20
+rottentomatoes-reviews-scraper --count_title 20 --count_review 20
 ```
```

### Comparing `rottentomatoes-reviews-scraper-0.0.1/README.md` & `rottentomatoes-reviews-scraper-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -25,29 +25,29 @@
 ## Installation / インストール
 
 To install the package, use pip:
 
 パッケージをインストールするには、pipを使用します：
 
 ```sh
-pip install rottentomatoes-scraper
+pip install rottentomatoes-reviews-scraper
 ```
 
 ## Usage / 使い方
 
 After installing the package, you can use the command line interface to scrape data. Here is an example of how to use the package from the terminal:
 
 パッケージをインストールした後、コマンドラインインターフェースを使用してデータをスクレイピングできます。
 
 Set the number of movies to retrieve and the number of reviews to retrieve
 
 取得する映画数と取得するレビュー数を設定します。
 
 ```sh
-rottentomatoes-scraper --count_title 20 --count_review 20
+rottentomatoes-reviews-scraper --count_title 20 --count_review 20
 ```
 
 This command will first scrape 20 movie titles and then scrape 20 reviews for each of those movies.
 
 このコマンドは、最初に20の映画タイトルをスクレイピングし、その後各映画の20のレビューをスクレイピングします。
 
 ## Command Line Arguments / コマンドライン引数
@@ -61,9 +61,9 @@
 ## Example / 例
 
 Here is an example of how to run the scraper:
 
 スクレイパーを実行する例を以下に示します：
 
 ```sh
-rottentomatoes-scraper --count_title 20 --count_review 20
+rottentomatoes-reviews-scraper --count_title 20 --count_review 20
 ```
```

### Comparing `rottentomatoes-reviews-scraper-0.0.1/setup.py` & `rottentomatoes-reviews-scraper-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="rottentomatoes-reviews-scraper",
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         "requests",
         "pandas",
         "selenium"
     ],
```

### Comparing `rottentomatoes-reviews-scraper-0.0.1/src/rottentomatoes_reviews_scraper.egg-info/PKG-INFO` & `rottentomatoes-reviews-scraper-0.0.2/src/rottentomatoes_reviews_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rottentomatoes-reviews-scraper
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package to scrape movie data from Rotten Tomatoes, including titles and reviews.
 Home-page: https://github.com/HwaI12/rottentomatoes-reviews-scraper
 Author: Fami Ishikawa
 Author-email: s2222061@stu.musashino-u.ac.jp
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -40,29 +40,29 @@
 ## Installation / インストール
 
 To install the package, use pip:
 
 パッケージをインストールするには、pipを使用します：
 
 ```sh
-pip install rottentomatoes-scraper
+pip install rottentomatoes-reviews-scraper
 ```
 
 ## Usage / 使い方
 
 After installing the package, you can use the command line interface to scrape data. Here is an example of how to use the package from the terminal:
 
 パッケージをインストールした後、コマンドラインインターフェースを使用してデータをスクレイピングできます。
 
 Set the number of movies to retrieve and the number of reviews to retrieve
 
 取得する映画数と取得するレビュー数を設定します。
 
 ```sh
-rottentomatoes-scraper --count_title 20 --count_review 20
+rottentomatoes-reviews-scraper --count_title 20 --count_review 20
 ```
 
 This command will first scrape 20 movie titles and then scrape 20 reviews for each of those movies.
 
 このコマンドは、最初に20の映画タイトルをスクレイピングし、その後各映画の20のレビューをスクレイピングします。
 
 ## Command Line Arguments / コマンドライン引数
@@ -76,10 +76,10 @@
 ## Example / 例
 
 Here is an example of how to run the scraper:
 
 スクレイパーを実行する例を以下に示します：
 
 ```sh
-rottentomatoes-scraper --count_title 20 --count_review 20
+rottentomatoes-reviews-scraper --count_title 20 --count_review 20
 ```
```


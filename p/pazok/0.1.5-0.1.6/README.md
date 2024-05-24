# Comparing `tmp/pazok-0.1.5.tar.gz` & `tmp/pazok-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pazok-0.1.5.tar", last modified: Fri May 24 12:57:22 2024, max compression
+gzip compressed data, was "pazok-0.1.6.tar", last modified: Fri May 24 14:13:35 2024, max compression
```

## Comparing `pazok-0.1.5.tar` & `pazok-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 12:57:22.449213 pazok-0.1.5/
--rw-rw-rw-   0        0        0       29 2024-05-23 23:30:01.000000 pazok-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0     1141 2024-05-24 12:57:22.445229 pazok-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      717 2024-05-23 23:29:46.000000 pazok-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 12:57:22.415303 pazok-0.1.5/pazok/
--rw-rw-rw-   0        0        0      745 2024-05-24 12:54:44.000000 pazok-0.1.5/pazok/__init__.py
--rw-rw-rw-   0        0        0    44242 2024-05-24 12:54:23.000000 pazok-0.1.5/pazok/pazok.py
-drwxrwxrwx   0        0        0        0 2024-05-24 12:57:22.443227 pazok-0.1.5/pazok.egg-info/
--rw-rw-rw-   0        0        0     1141 2024-05-24 12:57:22.000000 pazok-0.1.5/pazok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-05-24 12:57:22.000000 pazok-0.1.5/pazok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 12:57:22.000000 pazok-0.1.5/pazok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-24 12:57:22.000000 pazok-0.1.5/pazok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 12:57:22.449213 pazok-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      552 2024-05-24 12:57:07.000000 pazok-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:13:35.606049 pazok-0.1.6/
+-rw-rw-rw-   0        0        0       29 2024-05-23 23:30:01.000000 pazok-0.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     1240 2024-05-24 14:13:35.606049 pazok-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      717 2024-05-23 23:29:46.000000 pazok-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 14:13:35.582066 pazok-0.1.6/pazok/
+-rw-rw-rw-   0        0        0      745 2024-05-24 12:54:44.000000 pazok-0.1.6/pazok/__init__.py
+-rw-rw-rw-   0        0        0    44242 2024-05-24 12:54:23.000000 pazok-0.1.6/pazok/pazok.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:13:35.606049 pazok-0.1.6/pazok.egg-info/
+-rw-rw-rw-   0        0        0     1240 2024-05-24 14:13:35.000000 pazok-0.1.6/pazok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2024-05-24 14:13:35.000000 pazok-0.1.6/pazok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 14:13:35.000000 pazok-0.1.6/pazok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-24 14:13:35.000000 pazok-0.1.6/pazok.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-24 14:13:35.000000 pazok-0.1.6/pazok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 14:13:35.606049 pazok-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      681 2024-05-24 14:12:56.000000 pazok-0.1.6/setup.py
```

### Comparing `pazok-0.1.5/PKG-INFO` & `pazok-0.1.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: pazok
-Version: 0.1.5
+Version: 0.1.6
 Summary: A short description of my package
 Author: b_azo
 Author-email: husseun.selt@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: requests
+Requires-Dist: fake_useragent
+Requires-Dist: PIL
+Requires-Dist: random
 
 <h1 align="center">pazok</h1>
 
 
 ### What is pazok?
 It is a python library that contains a set of ready-made codes that enable you to create the most wonderful designs and animations on the terminal.
```

#### html2text {}

```diff
@@ -1,12 +1,14 @@
-Metadata-Version: 2.1 Name: pazok Version: 0.1.5 Summary: A short description
+Metadata-Version: 2.1 Name: pazok Version: 0.1.6 Summary: A short description
 of my package Author: b_azo Author-email: husseun.selt@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE.txt
+Description-Content-Type: text/markdown License-File: LICENSE.txt Requires-
+Dist: requests Requires-Dist: fake_useragent Requires-Dist: PIL Requires-Dist:
+random
                               ************ ppaazzookk ************
 ### What is pazok? It is a python library that contains a set of ready-made
 codes that enable you to create the most wonderful designs and animations on
 the terminal. ### Support + python + termux ### Install Just write this code on
 terminal: ```shell pip3 install pazok ``` If you want to download the developer
 version then write on terminal this code ```shell pip3 install git+https://
 github.com/h98m/pazok ``` I don't recommend regular users to download the
```

### Comparing `pazok-0.1.5/README.md` & `pazok-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pazok-0.1.5/pazok/__init__.py` & `pazok-0.1.6/pazok/__init__.py`

 * *Files identical despite different names*

### Comparing `pazok-0.1.5/pazok/pazok.py` & `pazok-0.1.6/pazok/pazok.py`

 * *Files identical despite different names*

### Comparing `pazok-0.1.5/pazok.egg-info/PKG-INFO` & `pazok-0.1.6/pazok.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: pazok
-Version: 0.1.5
+Version: 0.1.6
 Summary: A short description of my package
 Author: b_azo
 Author-email: husseun.selt@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: requests
+Requires-Dist: fake_useragent
+Requires-Dist: PIL
+Requires-Dist: random
 
 <h1 align="center">pazok</h1>
 
 
 ### What is pazok?
 It is a python library that contains a set of ready-made codes that enable you to create the most wonderful designs and animations on the terminal.
```

#### html2text {}

```diff
@@ -1,12 +1,14 @@
-Metadata-Version: 2.1 Name: pazok Version: 0.1.5 Summary: A short description
+Metadata-Version: 2.1 Name: pazok Version: 0.1.6 Summary: A short description
 of my package Author: b_azo Author-email: husseun.selt@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE.txt
+Description-Content-Type: text/markdown License-File: LICENSE.txt Requires-
+Dist: requests Requires-Dist: fake_useragent Requires-Dist: PIL Requires-Dist:
+random
                               ************ ppaazzookk ************
 ### What is pazok? It is a python library that contains a set of ready-made
 codes that enable you to create the most wonderful designs and animations on
 the terminal. ### Support + python + termux ### Install Just write this code on
 terminal: ```shell pip3 install pazok ``` If you want to download the developer
 version then write on terminal this code ```shell pip3 install git+https://
 github.com/h98m/pazok ``` I don't recommend regular users to download the
```


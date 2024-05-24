# Comparing `tmp/oktmoparser-1.1.tar.gz` & `tmp/oktmoparser-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oktmoparser-1.1.tar", last modified: Fri May 24 06:12:33 2024, max compression
+gzip compressed data, was "oktmoparser-1.2.tar", last modified: Fri May 24 06:24:36 2024, max compression
```

## Comparing `oktmoparser-1.1.tar` & `oktmoparser-1.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 06:12:33.677003 oktmoparser-1.1/
--rw-rw-rw-   0        0        0     2169 2024-05-24 06:12:33.675989 oktmoparser-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1379 2024-05-24 05:51:05.000000 oktmoparser-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 06:12:33.651988 oktmoparser-1.1/oktmo-parser/
--rw-rw-rw-   0        0        0       29 2024-05-24 06:11:48.000000 oktmoparser-1.1/oktmo-parser/__init__.py
--rw-rw-rw-   0        0        0     2917 2024-05-24 04:20:54.000000 oktmoparser-1.1/oktmo-parser/oktmo.py
-drwxrwxrwx   0        0        0        0 2024-05-24 06:12:33.674990 oktmoparser-1.1/oktmoparser.egg-info/
--rw-rw-rw-   0        0        0     2169 2024-05-24 06:12:33.000000 oktmoparser-1.1/oktmoparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2024-05-24 06:12:33.000000 oktmoparser-1.1/oktmoparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 06:12:33.000000 oktmoparser-1.1/oktmoparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-24 06:12:33.000000 oktmoparser-1.1/oktmoparser.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-24 06:12:33.000000 oktmoparser-1.1/oktmoparser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-24 06:12:33.000000 oktmoparser-1.1/oktmoparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 06:12:33.678990 oktmoparser-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1028 2024-05-24 06:09:50.000000 oktmoparser-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:24:36.524614 oktmoparser-1.2/
+-rw-rw-rw-   0        0        0     2169 2024-05-24 06:24:36.524614 oktmoparser-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1379 2024-05-24 05:51:05.000000 oktmoparser-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 06:24:36.504613 oktmoparser-1.2/oktmo-parser/
+-rw-rw-rw-   0        0        0       20 2024-05-24 06:22:53.000000 oktmoparser-1.2/oktmo-parser/__init__.py
+-rw-rw-rw-   0        0        0     2917 2024-05-24 04:20:54.000000 oktmoparser-1.2/oktmo-parser/oktmo.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:24:36.523614 oktmoparser-1.2/oktmoparser.egg-info/
+-rw-rw-rw-   0        0        0     2169 2024-05-24 06:24:36.000000 oktmoparser-1.2/oktmoparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-05-24 06:24:36.000000 oktmoparser-1.2/oktmoparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 06:24:36.000000 oktmoparser-1.2/oktmoparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-24 06:24:36.000000 oktmoparser-1.2/oktmoparser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-24 06:24:36.000000 oktmoparser-1.2/oktmoparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 06:24:36.526611 oktmoparser-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      911 2024-05-24 06:24:13.000000 oktmoparser-1.2/setup.py
```

### Comparing `oktmoparser-1.1/PKG-INFO` & `oktmoparser-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oktmoparser
-Version: 1.1
+Version: 1.2
 Summary: Simple and useful parser that helps you get actual All-Russian Classifier of Municipal Territories (OKTMO)
 Home-page: https://github.com/letimvkocmoc/oktmo-parser
 Author: letimvkocmoc
 Author-email: letimvkocmoc@gmail.com
 Project-URL: GitGub, https://github.com/letimvkocmoc
 Keywords: oktmo parser municipal territory classifier
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `oktmoparser-1.1/README.md` & `oktmoparser-1.2/README.md`

 * *Files identical despite different names*

### Comparing `oktmoparser-1.1/oktmo-parser/oktmo.py` & `oktmoparser-1.2/oktmo-parser/oktmo.py`

 * *Files identical despite different names*

### Comparing `oktmoparser-1.1/oktmoparser.egg-info/PKG-INFO` & `oktmoparser-1.2/oktmoparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oktmoparser
-Version: 1.1
+Version: 1.2
 Summary: Simple and useful parser that helps you get actual All-Russian Classifier of Municipal Territories (OKTMO)
 Home-page: https://github.com/letimvkocmoc/oktmo-parser
 Author: letimvkocmoc
 Author-email: letimvkocmoc@gmail.com
 Project-URL: GitGub, https://github.com/letimvkocmoc
 Keywords: oktmo parser municipal territory classifier
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `oktmoparser-1.1/setup.py` & `oktmoparser-1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='oktmoparser',
-    version='1.1',
+    version='1.2',
     author='letimvkocmoc',
     author_email='letimvkocmoc@gmail.com',
     description='Simple and useful parser that helps you get actual All-Russian Classifier of Municipal Territories (OKTMO)',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/letimvkocmoc/oktmo-parser',
     classifiers=[
@@ -21,14 +21,9 @@
         'Operating System :: OS Independent'
     ],
     keywords='oktmo parser municipal territory classifier',
     project_urls={
         'GitGub': 'https://github.com/letimvkocmoc'
     },
     packages=find_packages(),
-    install_requires=['requests'],
-    entry_points={
-        'console_scripts': [
-            'oktmo-parser = oktmo_parser:main'
-        ]
-    }
+    install_requires=['requests']
 )
```


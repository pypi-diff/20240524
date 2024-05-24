# Comparing `tmp/scrathon_payments-0.2.0.tar.gz` & `tmp/scrathon_payments-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrathon_payments-0.2.0.tar", last modified: Thu May 23 09:22:27 2024, max compression
+gzip compressed data, was "scrathon_payments-0.2.1.tar", last modified: Fri May 24 07:19:15 2024, max compression
```

## Comparing `scrathon_payments-0.2.0.tar` & `scrathon_payments-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:22:27.448410 scrathon_payments-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-23 09:22:23.000000 scrathon_payments-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-23 09:22:27.448410 scrathon_payments-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-23 09:22:23.000000 scrathon_payments-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:22:27.444410 scrathon_payments-0.2.0/ScrathonPayments/
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-23 09:22:23.000000 scrathon_payments-0.2.0/ScrathonPayments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:22:27.448410 scrathon_payments-0.2.0/scrathon_payments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-23 09:22:27.000000 scrathon_payments-0.2.0/scrathon_payments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-23 09:22:27.000000 scrathon_payments-0.2.0/scrathon_payments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:22:27.000000 scrathon_payments-0.2.0/scrathon_payments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 09:22:27.000000 scrathon_payments-0.2.0/scrathon_payments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 09:22:27.000000 scrathon_payments-0.2.0/scrathon_payments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 09:22:27.448410 scrathon_payments-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-23 09:22:23.000000 scrathon_payments-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:19:15.259892 scrathon_payments-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-24 07:19:11.000000 scrathon_payments-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-24 07:19:15.259892 scrathon_payments-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-24 07:19:11.000000 scrathon_payments-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:19:15.259892 scrathon_payments-0.2.1/ScrathonPayments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-24 07:19:11.000000 scrathon_payments-0.2.1/ScrathonPayments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:19:15.259892 scrathon_payments-0.2.1/scrathon_payments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-24 07:19:15.000000 scrathon_payments-0.2.1/scrathon_payments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-24 07:19:15.000000 scrathon_payments-0.2.1/scrathon_payments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 07:19:15.000000 scrathon_payments-0.2.1/scrathon_payments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 07:19:15.000000 scrathon_payments-0.2.1/scrathon_payments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 07:19:15.000000 scrathon_payments-0.2.1/scrathon_payments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 07:19:15.259892 scrathon_payments-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-24 07:19:11.000000 scrathon_payments-0.2.1/setup.py
```

### Comparing `scrathon_payments-0.2.0/LICENSE` & `scrathon_payments-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrathon_payments-0.2.0/PKG-INFO` & `scrathon_payments-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrathon-payments
-Version: 0.2.0
+Version: 0.2.1
 Summary: API Wrapper for ScrathonPayments
 Home-page: https://github.com/Ryan-shamu-YT/ScrathonPayments
 Author: Ryan_shamu
 Author-email: Ryanshamu418@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scrathon_payments-0.2.0/README.md` & `scrathon_payments-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `scrathon_payments-0.2.0/ScrathonPayments/__init__.py` & `scrathon_payments-0.2.1/ScrathonPayments/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import scratchattach as scratch3
 import requests
 
-class Scrathon():
+class Scrathon:
 
-    def __init__(self, username):
+    def __init__(self, username, client: scratch3.CloudRequests):
+        self.client = client
         self.username = "None"
         try:
             scratch3.get_user(username)
             userexists = True
         except scratch3.exceptions.UserNotFound:
             userexists = False
         if userexists:
@@ -17,24 +18,25 @@
                 print("User {} did not use Scrathon before!".format(username))
         else:
             print("User {} does not exist on scratch!".format(username))
 
         if self.username != "None":
             print("Started Scrathon as {}! All funds earned will go to mentioned user".format(self.username))
 
-    def purchase(self, price, user):
-        request = requests.post("http://45.140.188.129:6623/transaction", json={
-            "price": price,
-            "buyer": user,
-            "seller": self.username
-        })
-
-        return request.json()
-    
-    def purchasecheck(self, price, user):
-        request = requests.post("http://45.140.188.129:6623/checkpurchase", json={
-            "price": price,
-            "buyer": user,
-            "seller": self.username
-        })
+        @client.request
+        def purchase(price):
+            request = requests.post("http://45.140.188.129:6623/transaction", json={
+                "price": price,
+                "buyer": client.get_requester(),
+                "seller": self.username
+            })
+
+            return request.json()
+        @client.request
+        def purchasecheck(price):
+            request = requests.post("http://45.140.188.129:6623/checkpurchase", json={
+                "price": price,
+                "buyer": client.get_requester(),
+                "seller": self.username
+            })
 
-        return request.json()
+            return request.json()
```

### Comparing `scrathon_payments-0.2.0/scrathon_payments.egg-info/PKG-INFO` & `scrathon_payments-0.2.1/scrathon_payments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrathon-payments
-Version: 0.2.0
+Version: 0.2.1
 Summary: API Wrapper for ScrathonPayments
 Home-page: https://github.com/Ryan-shamu-YT/ScrathonPayments
 Author: Ryan_shamu
 Author-email: Ryanshamu418@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scrathon_payments-0.2.0/setup.py` & `scrathon_payments-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='scrathon-payments',
-    version='0.2.0',
+    version='0.2.1',
     author='Ryan_shamu',
     author_email='Ryanshamu418@gmail.com',
     description='API Wrapper for ScrathonPayments',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Ryan-shamu-YT/ScrathonPayments',
     packages=find_packages(exclude=[]),
```


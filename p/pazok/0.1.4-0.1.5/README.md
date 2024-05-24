# Comparing `tmp/pazok-0.1.4.tar.gz` & `tmp/pazok-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pazok-0.1.4.tar", last modified: Fri May 24 12:09:35 2024, max compression
+gzip compressed data, was "pazok-0.1.5.tar", last modified: Fri May 24 12:57:22 2024, max compression
```

## Comparing `pazok-0.1.4.tar` & `pazok-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 12:09:35.506591 pazok-0.1.4/
--rw-rw-rw-   0        0        0       29 2024-05-23 23:30:01.000000 pazok-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1141 2024-05-24 12:09:35.503599 pazok-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      717 2024-05-23 23:29:46.000000 pazok-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 12:09:35.472683 pazok-0.1.4/pazok/
--rw-rw-rw-   0        0        0      723 2024-05-24 12:03:21.000000 pazok-0.1.4/pazok/__init__.py
--rw-rw-rw-   0        0        0    44251 2024-05-24 12:03:19.000000 pazok-0.1.4/pazok/pazok.py
-drwxrwxrwx   0        0        0        0 2024-05-24 12:09:35.499613 pazok-0.1.4/pazok.egg-info/
--rw-rw-rw-   0        0        0     1141 2024-05-24 12:09:35.000000 pazok-0.1.4/pazok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-05-24 12:09:35.000000 pazok-0.1.4/pazok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 12:09:35.000000 pazok-0.1.4/pazok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-24 12:09:35.000000 pazok-0.1.4/pazok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 12:09:35.506591 pazok-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      552 2024-05-24 12:09:20.000000 pazok-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 12:57:22.449213 pazok-0.1.5/
+-rw-rw-rw-   0        0        0       29 2024-05-23 23:30:01.000000 pazok-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     1141 2024-05-24 12:57:22.445229 pazok-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      717 2024-05-23 23:29:46.000000 pazok-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 12:57:22.415303 pazok-0.1.5/pazok/
+-rw-rw-rw-   0        0        0      745 2024-05-24 12:54:44.000000 pazok-0.1.5/pazok/__init__.py
+-rw-rw-rw-   0        0        0    44242 2024-05-24 12:54:23.000000 pazok-0.1.5/pazok/pazok.py
+drwxrwxrwx   0        0        0        0 2024-05-24 12:57:22.443227 pazok-0.1.5/pazok.egg-info/
+-rw-rw-rw-   0        0        0     1141 2024-05-24 12:57:22.000000 pazok-0.1.5/pazok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-05-24 12:57:22.000000 pazok-0.1.5/pazok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 12:57:22.000000 pazok-0.1.5/pazok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-24 12:57:22.000000 pazok-0.1.5/pazok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 12:57:22.449213 pazok-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      552 2024-05-24 12:57:07.000000 pazok-0.1.5/setup.py
```

### Comparing `pazok-0.1.4/PKG-INFO` & `pazok-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pazok
-Version: 0.1.4
+Version: 0.1.5
 Summary: A short description of my package
 Author: b_azo
 Author-email: husseun.selt@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pazok Version: 0.1.4 Summary: A short description
+Metadata-Version: 2.1 Name: pazok Version: 0.1.5 Summary: A short description
 of my package Author: b_azo Author-email: husseun.selt@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE.txt
                               ************ ppaazzookk ************
 ### What is pazok? It is a python library that contains a set of ready-made
 codes that enable you to create the most wonderful designs and animations on
```

### Comparing `pazok-0.1.4/README.md` & `pazok-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pazok-0.1.4/pazok/__init__.py` & `pazok-0.1.5/pazok/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 from .pazok import file_np
 from .pazok import log_in
 from .pazok import json_req
 from .pazok import cURL
 from .pazok import cook
 from .pazok import motifs
 from .pazok import info_motifs
-from .pazok import Hussein
+from .pazok import Hussein
+from .pazok import *
```

### Comparing `pazok-0.1.4/pazok/pazok.py` & `pazok-0.1.5/pazok/pazok.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,44 +194,43 @@
 #pazok.sb(اسم الداله, عدد الخيوط)
 
 
 #- - - - - - - - - - - - - - -- - - - - - -- - - - - #
 
 #ارسال تلي حديث
 
-def tele_ms(token, id, txt=None, file=None, img=None, button=None):
+def tele_ms(token, id, txt=None, file=None, img=None, buttons=None):
     if not token or not id or txt is None:
         raise ValueError("يرجى اضافة توكن وايدي ونص على الاقل")
     
     import telebot
     from telebot import types
     import requests
     import os
 
     bot = telebot.TeleBot(token)
     keyboard = types.InlineKeyboardMarkup()
-    if button:
-        for i in range(0, len(button), 2):
-            button_name = button[i]
-            button_url = button[i+1]
+    if buttons:
+        for i in range(0, len(buttons), 2):
+            button_name = buttons[i]
+            button_url = buttons[i + 1]
             button = types.InlineKeyboardButton(button_name, url=button_url)
             keyboard.add(button)
 
     def download_file_from_url(url):
         file_name = url.split('/')[-1]
         response = requests.get(url)
         with open(file_name, 'wb') as f:
             f.write(response.content)
         return file_name
 
     if file or img:
         if img:
             if img.startswith('http'):
                 bot.send_photo(id, photo=img, caption=txt, parse_mode='Markdown', reply_markup=keyboard)
-                
             else:
                 bot.send_photo(id, open(img, 'rb'), caption=txt, parse_mode='MarkdownV2', reply_markup=keyboard)
         
         if file:
             if file.startswith('http'):
                 file_path = download_file_from_url(file)
                 bot.send_document(id, open(file_path, 'rb'), caption=txt, parse_mode='MarkdownV2', reply_markup=keyboard)
@@ -239,14 +238,15 @@
             else:
                 bot.send_document(id, open(file, 'rb'), caption=txt, parse_mode='MarkdownV2', reply_markup=keyboard)
 
     elif txt:
         bot.send_message(id, txt, parse_mode='MarkdownV2', reply_markup=keyboard)
 
 
+
 #توكن
 #token=""
 #ايدي
 #id=""
 
 #يستقبل جميع تنسيقات النص
 #msg="hello"
```

### Comparing `pazok-0.1.4/pazok.egg-info/PKG-INFO` & `pazok-0.1.5/pazok.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pazok
-Version: 0.1.4
+Version: 0.1.5
 Summary: A short description of my package
 Author: b_azo
 Author-email: husseun.selt@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pazok Version: 0.1.4 Summary: A short description
+Metadata-Version: 2.1 Name: pazok Version: 0.1.5 Summary: A short description
 of my package Author: b_azo Author-email: husseun.selt@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE.txt
                               ************ ppaazzookk ************
 ### What is pazok? It is a python library that contains a set of ready-made
 codes that enable you to create the most wonderful designs and animations on
```

### Comparing `pazok-0.1.4/setup.py` & `pazok-0.1.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pazok',
-    version='0.1.4',
+    version='0.1.5',
     author='b_azo',
     author_email='husseun.selt@gmail.com',
     description='A short description of my package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
```


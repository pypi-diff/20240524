# Comparing `tmp/transitle-1.0.1.tar.gz` & `tmp/transitle-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transitle-1.0.1.tar", last modified: Wed Aug 30 14:24:34 2023, max compression
+gzip compressed data, was "transitle-1.1.0.tar", last modified: Fri May 24 11:26:22 2024, max compression
```

## Comparing `transitle-1.0.1.tar` & `transitle-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mesutgunes   (501) staff       (20)        0 2023-08-30 14:24:34.265812 transitle-1.0.1/
--rw-r--r--   0 mesutgunes   (501) staff       (20)    35149 2023-07-17 14:35:41.000000 transitle-1.0.1/LICENSE
--rw-r--r--   0 mesutgunes   (501) staff       (20)      527 2023-08-30 14:24:34.265574 transitle-1.0.1/PKG-INFO
--rw-r--r--   0 mesutgunes   (501) staff       (20)     2688 2023-07-18 12:37:13.000000 transitle-1.0.1/README.rst
--rw-r--r--   0 mesutgunes   (501) staff       (20)       38 2023-08-30 14:24:34.265863 transitle-1.0.1/setup.cfg
--rw-r--r--   0 mesutgunes   (501) staff       (20)     1285 2023-08-30 14:24:26.000000 transitle-1.0.1/setup.py
-drwxr-xr-x   0 mesutgunes   (501) staff       (20)        0 2023-08-30 14:24:34.261843 transitle-1.0.1/transitle/
--rw-r--r--   0 mesutgunes   (501) staff       (20)       60 2023-07-17 10:16:33.000000 transitle-1.0.1/transitle/__init__.py
--rw-r--r--   0 mesutgunes   (501) staff       (20)     1267 2023-08-30 13:04:29.000000 transitle-1.0.1/transitle/__main__.py
--rw-r--r--   0 mesutgunes   (501) staff       (20)     1130 2023-08-30 13:04:39.000000 transitle-1.0.1/transitle/translator.py
--rw-r--r--   0 mesutgunes   (501) staff       (20)     6005 2023-08-30 14:10:52.000000 transitle-1.0.1/transitle/ts.py
-drwxr-xr-x   0 mesutgunes   (501) staff       (20)        0 2023-08-30 14:24:34.265148 transitle-1.0.1/transitle.egg-info/
--rw-r--r--   0 mesutgunes   (501) staff       (20)      527 2023-08-30 14:24:34.000000 transitle-1.0.1/transitle.egg-info/PKG-INFO
--rw-r--r--   0 mesutgunes   (501) staff       (20)      311 2023-08-30 14:24:34.000000 transitle-1.0.1/transitle.egg-info/SOURCES.txt
--rw-r--r--   0 mesutgunes   (501) staff       (20)        1 2023-08-30 14:24:34.000000 transitle-1.0.1/transitle.egg-info/dependency_links.txt
--rw-r--r--   0 mesutgunes   (501) staff       (20)       47 2023-08-30 14:24:34.000000 transitle-1.0.1/transitle.egg-info/entry_points.txt
--rw-r--r--   0 mesutgunes   (501) staff       (20)       32 2023-08-30 14:24:34.000000 transitle-1.0.1/transitle.egg-info/requires.txt
--rw-r--r--   0 mesutgunes   (501) staff       (20)       10 2023-08-30 14:24:34.000000 transitle-1.0.1/transitle.egg-info/top_level.txt
+drwxr-xr-x   0 mesutgunes   (501) staff       (20)        0 2024-05-24 11:26:22.181828 transitle-1.1.0/
+-rw-r--r--   0 mesutgunes   (501) staff       (20)    35149 2024-05-16 13:31:48.000000 transitle-1.1.0/LICENSE
+-rw-r--r--   0 mesutgunes   (501) staff       (20)      658 2024-05-24 11:26:22.181579 transitle-1.1.0/PKG-INFO
+-rw-r--r--   0 mesutgunes   (501) staff       (20)     3358 2024-05-24 11:17:33.000000 transitle-1.1.0/README.rst
+-rw-r--r--   0 mesutgunes   (501) staff       (20)       38 2024-05-24 11:26:22.181868 transitle-1.1.0/setup.cfg
+-rw-r--r--   0 mesutgunes   (501) staff       (20)     1359 2024-05-24 11:26:17.000000 transitle-1.1.0/setup.py
+drwxr-xr-x   0 mesutgunes   (501) staff       (20)        0 2024-05-24 11:26:22.180414 transitle-1.1.0/transitle/
+-rw-r--r--   0 mesutgunes   (501) staff       (20)       60 2024-05-16 13:31:48.000000 transitle-1.1.0/transitle/__init__.py
+-rw-r--r--   0 mesutgunes   (501) staff       (20)     1374 2024-05-24 10:52:50.000000 transitle-1.1.0/transitle/__main__.py
+-rw-r--r--   0 mesutgunes   (501) staff       (20)     1332 2024-05-24 09:30:04.000000 transitle-1.1.0/transitle/translator.py
+-rw-r--r--   0 mesutgunes   (501) staff       (20)     7021 2024-05-24 09:42:58.000000 transitle-1.1.0/transitle/ts.py
+drwxr-xr-x   0 mesutgunes   (501) staff       (20)        0 2024-05-24 11:26:22.181349 transitle-1.1.0/transitle.egg-info/
+-rw-r--r--   0 mesutgunes   (501) staff       (20)      658 2024-05-24 11:26:22.000000 transitle-1.1.0/transitle.egg-info/PKG-INFO
+-rw-r--r--   0 mesutgunes   (501) staff       (20)      311 2024-05-24 11:26:22.000000 transitle-1.1.0/transitle.egg-info/SOURCES.txt
+-rw-r--r--   0 mesutgunes   (501) staff       (20)        1 2024-05-24 11:26:22.000000 transitle-1.1.0/transitle.egg-info/dependency_links.txt
+-rw-r--r--   0 mesutgunes   (501) staff       (20)       47 2024-05-24 11:26:22.000000 transitle-1.1.0/transitle.egg-info/entry_points.txt
+-rw-r--r--   0 mesutgunes   (501) staff       (20)       32 2024-05-24 11:26:22.000000 transitle-1.1.0/transitle.egg-info/requires.txt
+-rw-r--r--   0 mesutgunes   (501) staff       (20)       10 2024-05-24 11:26:22.000000 transitle-1.1.0/transitle.egg-info/top_level.txt
```

### Comparing `transitle-1.0.1/LICENSE` & `transitle-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `transitle-1.0.1/PKG-INFO` & `transitle-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Metadata-Version: 2.1
 Name: transitle
-Version: 1.0.1
-Summary: Translate subtitles in a folder flawlessly
+Version: 1.1.0
+Summary: AI-Based Subtitle translator. Translate subtitles in a folder flawlessly
 Home-page: https://github.com/gunesmes/subtitle_translator
 Author: Mesut Gunes
 Author-email: gunesmes@gmail.com
 License: LICENSE.md
 Requires-Python: >=3.0
 License-File: LICENSE
+Requires-Dist: googletranslate_python
+Requires-Dist: requests
 
-translate_subtitles allows you to translate subtitles in a directory flawlessly with your favorite translator. 
-        Translate bunch of subtitles from original language to desired language. This gives you a machine translated subtitle.
+
+    Transitle is a AI-based subtitle translator. It allows you to translate subtitles 
+    in a directory flawlessly with your favorite translator. Translate bunch of 
+    subtitlesfrom original language to desired language. This gives you a AI-based
+    translated subtitle.
```

### Comparing `transitle-1.0.1/README.rst` & `transitle-1.1.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,23 @@
-Translate Subtitles - transitle
+AI Based Subtitle Translator - transitle
 ===============================
 |PyPI latest| |PyPI Version| |PyPI License| |Docs|
 
-translate_subtitles allows you to translate subtitles in a directory
-flawlessly with your favorite translator. Translate bunch of subtitles
-from original language to desired language. This gives you a machine
-translated subtitle.
+Transitle is a AI-based subtitle translator. It allows you to translate subtitles 
+in a directory flawlessly with your favorite translator. Translate bunch of 
+subtitlesfrom original language to desired language. This gives you a AI-based
+translated subtitle. 
+
+Transitle also has support for using AI-based translator such as:
+ - [deepl](https://www.deepl.com/translator)
+ - [google](https://translate.google.com/)
+ - [mymemory](https://mymemory.ai/)
+ - [papago](https://papago.naver.com/)
+ - [qcri](https://mt.qcri.org/api/)
+
 
 ``pip install transitle``
 
 .. raw:: html
 
    <!---
    ![Subtitle Demo Gif](img/tty.gif)
@@ -20,14 +28,32 @@
 
 -  install the ``transitle`` via pip ``pip install transitle``
 -  you must have a valid subtitle in .srt format
 -  You can use Google translator or yandex
 -  For yandex you must have Yandex Translater API key. You can get it
    from here: http://api.yandex.com/key/keyslist.xml
 
+Translators
+-----------
+There buch of translators including AI-based translation `Deepl`. You can
+register and create a API token and then put it in the environment variables.
+Most of the toolings provide free limited translation.
+
+Alternative translators:
+ - google
+ - chatgpt
+ - microsoft
+ - pons
+ - linguee
+ - mymemory
+ - yandex
+ - papago
+ - deepl
+ - qcri
+
 Run as a CLI tooling
 --------------------
 
 .. code:: shell
 
    ➜  ~ pip install transitle
    ➜  ~ ts ~/Downloads/subtitles google en tr
@@ -36,15 +62,15 @@
    1
    00:00:09,750 --> 00:00:10,666
    <i>São Paulo,</i>
 
    2
    00:00:10,750 --> 00:00:13,166
    <i>neredeyse 13 milyon kişi.</i>
-
+   
 Use as a library
 ----------------
 
 .. code:: shell
 
    # translate subtitles in a path
    >>> from transitle import ts
```

### Comparing `transitle-1.0.1/setup.py` & `transitle-1.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,20 +14,24 @@
 # with codecs.open(os.path.join(pwd, 'CHANGELOG'), encoding='utf-8') as f:
 #     changelog = f.read()
 #     long_description += '\n\n{}'.format(changelog)
 
 
 setup(
     name = "transitle",
-    version = "1.0.1",
+    version = "1.1.0",
     author = "Mesut Gunes",
     author_email = "gunesmes@gmail.com" ,
-    description = "Translate subtitles in a folder flawlessly",
-    long_description = '''translate_subtitles allows you to translate subtitles in a directory flawlessly with your favorite translator. 
-        Translate bunch of subtitles from original language to desired language. This gives you a machine translated subtitle.
+    description = "AI-Based Subtitle translator. Translate subtitles in a folder flawlessly",
+    long_description = 
+    '''
+    Transitle is a AI-based subtitle translator. It allows you to translate subtitles 
+    in a directory flawlessly with your favorite translator. Translate bunch of 
+    subtitlesfrom original language to desired language. This gives you a AI-based
+    translated subtitle. 
     ''',
     license = "LICENSE.md",
     url = "https://github.com/gunesmes/subtitle_translator",
     packages = find_packages(include=('ts.*', 'transitle')),
     entry_points = {
         'console_scripts': ['ts = transitle.__main__:main']
     },
```

### Comparing `transitle-1.0.1/transitle/__main__.py` & `transitle-1.1.0/transitle/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         # file_dir = "/Users/mesutgunes/Projects/subtitle_translator"
         file_dir = args[0]
 
         # Google can only be choosen as translator. Later, Windows and Yandex can be added.
         translator = args[1]
 
         # set languages you want to translate
-        source_language = args[2]
-        target_language = args[3]
+        source_lang = args[2]
+        target_lang = args[3]
     except IndexError:
         print("Arguments Error! Please run the file with the following format:")
         print(
-            "\n   ts 'path/to/files' 'translator:google or yandex' 'source language' 'target language'\n   ts /Users/mesutgunes/Downloads/subtitles google pl tr\n")
+            "\n   ts 'path/to/files' 'translator' 'source language' 'target language'\n   ts /Users/mesutgunes/Downloads/subtitles google pl tr\n\nAlternative translators:\n - google\n - chatgpt\n - microsoft\n - pons\n - linguee\n - mymemory\n - yandex\n - papago\n - deepl\n - qcri\n")
         sys.exit(2)
 
-    ts(file_dir=file_dir, translator=translator, source_lang=source_language, target_lang=target_language)
+    ts(file_dir=file_dir, translator=translator, source_lang=source_lang, target_lang=target_lang)
```

### Comparing `transitle-1.0.1/transitle/translator.py` & `transitle-1.1.0/transitle/translator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 from datetime import datetime
 import os
-
+import pdb
 from transitle.ts import TranslateSubtitle
 
+out = '/out/'
 
 def ts(file_dir, translator, source_lang, target_lang):
     start_time = datetime.now()
     
-    # set directory
-    os.chdir(file_dir)
-    path = os.listdir(file_dir)
-
-    s = TranslateSubtitle()
+    # set absolute paths
+    abs_path = os.path.abspath(file_dir)
+    translation_path = abs_path + out
+
+    # change directory
+    os.chdir(abs_path)
+
+    ts = TranslateSubtitle(
+        abs_path=abs_path, 
+        out=translation_path, 
+        translator=translator,
+        source_lang=source_lang,
+        target_lang=target_lang
+        )
 
     # get the .srt files from the dir
-    files = list()
-    for item in path:
+    files = os.listdir(abs_path)
+    str_files = list()
+    for item in files:
         if item.rfind(".srt") != -1:
-            files.append(item)
+            str_files.append(item)
             continue
 
-    for file in files:
+    for file in str_files:
         print(f"\n - - - - - - - - Translating: {file} - - - - - - - - ")
-        subFile = os.path.dirname(os.path.abspath(file)) + "/" + file
 
         """
         this function translate a subtitle file from original language to desired  language
         
         fileName        : names of subtitles 
-        target_language : language you want to translate to
-        source_language : the language of the subtitle
+        target_lang     : language you want to translate to
+        source_lang     : the language of the subtitle
         translator      : Google (later Yandex, Microsoft)
         """
 
-        s.subtitle_translator(subFile, translator, source_lang, target_lang)
+        ts.subtitle_translator(file)
 
     end_time = datetime.now()
-    print('Duration: {}'.format(end_time - start_time))
+    print('Duration: {}'.format(end_time - start_time))
```

### Comparing `transitle-1.0.1/transitle.egg-info/PKG-INFO` & `transitle-1.1.0/transitle.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Metadata-Version: 2.1
 Name: transitle
-Version: 1.0.1
-Summary: Translate subtitles in a folder flawlessly
+Version: 1.1.0
+Summary: AI-Based Subtitle translator. Translate subtitles in a folder flawlessly
 Home-page: https://github.com/gunesmes/subtitle_translator
 Author: Mesut Gunes
 Author-email: gunesmes@gmail.com
 License: LICENSE.md
 Requires-Python: >=3.0
 License-File: LICENSE
+Requires-Dist: googletranslate_python
+Requires-Dist: requests
 
-translate_subtitles allows you to translate subtitles in a directory flawlessly with your favorite translator. 
-        Translate bunch of subtitles from original language to desired language. This gives you a machine translated subtitle.
+
+    Transitle is a AI-based subtitle translator. It allows you to translate subtitles 
+    in a directory flawlessly with your favorite translator. Translate bunch of 
+    subtitlesfrom original language to desired language. This gives you a AI-based
+    translated subtitle.
```


# Comparing `tmp/memory_game-0.1.tar.gz` & `tmp/memory_game-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memory_game-0.1.tar", last modified: Fri May 24 05:09:53 2024, max compression
+gzip compressed data, was "memory_game-0.2.tar", last modified: Fri May 24 06:38:16 2024, max compression
```

## Comparing `memory_game-0.1.tar` & `memory_game-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 oriidemitsuhiko   (501) staff       (20)        0 2024-05-24 05:09:53.452965 memory_game-0.1/
--rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)     1380 2024-05-21 07:01:36.000000 memory_game-0.1/LICENSE
--rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)       34 2024-05-22 01:41:19.000000 memory_game-0.1/MANIFEST.in
--rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)     1171 2024-05-24 05:09:53.452772 memory_game-0.1/PKG-INFO
--rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)      718 2024-05-21 07:01:35.000000 memory_game-0.1/README.md
-drwxr-xr-x   0 oriidemitsuhiko   (501) staff       (20)        0 2024-05-24 05:09:53.451511 memory_game-0.1/memory_game/
--rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)        0 2024-05-21 06:52:07.000000 memory_game-0.1/memory_game/__init__.py
--rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)     1867 2024-05-24 05:06:12.000000 memory_game-0.1/memory_game/game.py
-drwxr-xr-x   0 oriidemitsuhiko   (501) staff       (20)        0 2024-05-24 05:09:53.452502 memory_game-0.1/memory_game.egg-info/
--rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)     1171 2024-05-24 05:09:53.000000 memory_game-0.1/memory_game.egg-info/PKG-INFO
--rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)      260 2024-05-24 05:09:53.000000 memory_game-0.1/memory_game.egg-info/SOURCES.txt
--rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)        1 2024-05-24 05:09:53.000000 memory_game-0.1/memory_game.egg-info/dependency_links.txt
--rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)       54 2024-05-24 05:09:53.000000 memory_game-0.1/memory_game.egg-info/entry_points.txt
--rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)       12 2024-05-24 05:09:53.000000 memory_game-0.1/memory_game.egg-info/top_level.txt
--rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)       38 2024-05-24 05:09:53.453032 memory_game-0.1/setup.cfg
--rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)      733 2024-05-24 05:06:36.000000 memory_game-0.1/setup.py
+drwxr-xr-x   0 oriidemitsuhiko   (501) staff       (20)        0 2024-05-24 06:38:16.127831 memory_game-0.2/
+-rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)     1380 2024-05-21 07:01:36.000000 memory_game-0.2/LICENSE
+-rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)       34 2024-05-22 01:41:19.000000 memory_game-0.2/MANIFEST.in
+-rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)     1190 2024-05-24 06:38:16.127601 memory_game-0.2/PKG-INFO
+-rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)      718 2024-05-21 07:01:35.000000 memory_game-0.2/README.md
+drwxr-xr-x   0 oriidemitsuhiko   (501) staff       (20)        0 2024-05-24 06:38:16.126233 memory_game-0.2/memory_game/
+-rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)        0 2024-05-21 06:52:07.000000 memory_game-0.2/memory_game/__init__.py
+-rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)     1867 2024-05-24 05:06:12.000000 memory_game-0.2/memory_game/game.py
+drwxr-xr-x   0 oriidemitsuhiko   (501) staff       (20)        0 2024-05-24 06:38:16.127290 memory_game-0.2/memory_game.egg-info/
+-rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)     1190 2024-05-24 06:38:16.000000 memory_game-0.2/memory_game.egg-info/PKG-INFO
+-rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)      260 2024-05-24 06:38:16.000000 memory_game-0.2/memory_game.egg-info/SOURCES.txt
+-rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)        1 2024-05-24 06:38:16.000000 memory_game-0.2/memory_game.egg-info/dependency_links.txt
+-rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)       55 2024-05-24 06:38:16.000000 memory_game-0.2/memory_game.egg-info/entry_points.txt
+-rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)       12 2024-05-24 06:38:16.000000 memory_game-0.2/memory_game.egg-info/top_level.txt
+-rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)       38 2024-05-24 06:38:16.127907 memory_game-0.2/setup.cfg
+-rw-r--r--   0 oriidemitsuhiko   (501) staff       (20)      766 2024-05-24 05:14:48.000000 memory_game-0.2/setup.py
```

### Comparing `memory_game-0.1/LICENSE` & `memory_game-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `memory_game-0.1/PKG-INFO` & `memory_game-0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: memory_game
-Version: 0.1
+Version: 0.2
 Summary: A simple console-based memory game
 Home-page: https://github.com/yourusername/memory_game
 Author: Your Name
 Author-email: your.email@example.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -36,7 +37,8 @@
 
 ## How to play
 - The game board will be displayed with all cards hidden.
 - Enter the position of the first card to flip (e.g., 0 1 for the card at row 0, column 1).
 - Enter the position of the second card to flip.
 - If the cards match, they will stay revealed. If not, they will be hidden again.
 - The game ends when all pairs are matched.
+
```

### Comparing `memory_game-0.1/README.md` & `memory_game-0.2/README.md`

 * *Files identical despite different names*

### Comparing `memory_game-0.1/memory_game/game.py` & `memory_game-0.2/memory_game/game.py`

 * *Files identical despite different names*

### Comparing `memory_game-0.1/memory_game.egg-info/PKG-INFO` & `memory_game-0.2/memory_game.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: memory-game
-Version: 0.1
+Version: 0.2
 Summary: A simple console-based memory game
 Home-page: https://github.com/yourusername/memory_game
 Author: Your Name
 Author-email: your.email@example.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -36,7 +37,8 @@
 
 ## How to play
 - The game board will be displayed with all cards hidden.
 - Enter the position of the first card to flip (e.g., 0 1 for the card at row 0, column 1).
 - Enter the position of the second card to flip.
 - If the cards match, they will stay revealed. If not, they will be hidden again.
 - The game ends when all pairs are matched.
+
```

### Comparing `memory_game-0.1/setup.py` & `memory_game-0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='memory_game',
-    version='0.1',
+    version='0.2',  # バージョン番号を更新
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'memory_game=memory_game.game:main',
         ],
     },
     description='A simple console-based memory game',
@@ -19,8 +19,7 @@
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
 )
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


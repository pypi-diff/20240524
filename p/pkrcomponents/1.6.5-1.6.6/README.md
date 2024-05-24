# Comparing `tmp/pkrcomponents-1.6.5.tar.gz` & `tmp/pkrcomponents-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkrcomponents-1.6.5.tar", last modified: Fri May 24 02:54:11 2024, max compression
+gzip compressed data, was "pkrcomponents-1.6.6.tar", last modified: Fri May 24 21:11:42 2024, max compression
```

## Comparing `pkrcomponents-1.6.5.tar` & `pkrcomponents-1.6.6.tar`

### file list

```diff
@@ -1,69 +1,43 @@
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 02:54:09.019588 pkrcomponents-1.6.5/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 02:54:08.283221 pkrcomponents-1.6.5/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.6.5/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.6.5/LICENSE.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-14 20:27:30.000000 pkrcomponents-1.6.5/MANIFEST.in
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2024-05-24 02:54:09.015588 pkrcomponents-1.6.5/PKG-INFO
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      224 2024-05-24 00:25:51.000000 pkrcomponents-1.6.5/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/README.rst
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1040 2024-05-24 02:50:24.000000 pkrcomponents-1.6.5/coverage.txt
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 02:54:08.468843 pkrcomponents-1.6.5/pkrcomponents/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/pkrcomponents/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/pkrcomponents/_common.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1593 2024-05-24 00:57:29.000000 pkrcomponents-1.6.5/pkrcomponents/action.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7569 2024-05-24 00:57:29.000000 pkrcomponents-1.6.5/pkrcomponents/bitcard.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3948 2024-05-15 15:52:00.000000 pkrcomponents-1.6.5/pkrcomponents/board.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5296 2024-05-15 11:58:01.000000 pkrcomponents-1.6.5/pkrcomponents/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/pkrcomponents/constants.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/pkrcomponents/evaluator.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/pkrcomponents/hand.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.6.5/pkrcomponents/listings.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/pkrcomponents/lookup_table.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 02:54:08.495956 pkrcomponents-1.6.5/pkrcomponents/models/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 02:54:08.572024 pkrcomponents-1.6.5/pkrcomponents/models/actions/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.6.5/pkrcomponents/models/actions/move.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.6.5/pkrcomponents/models/actions/sequence.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.6.5/pkrcomponents/models/actions/street.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.6.5/pkrcomponents/models/amount.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 02:54:08.666993 pkrcomponents-1.6.5/pkrcomponents/models/cards/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.6.5/pkrcomponents/models/cards/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.6.5/pkrcomponents/models/cards/rank.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.6.5/pkrcomponents/models/cards/suit.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 02:54:08.691502 pkrcomponents-1.6.5/pkrcomponents/models/pots/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.6.5/pkrcomponents/models/pots/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4434 2024-05-15 18:17:46.000000 pkrcomponents-1.6.5/pkrcomponents/players.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      999 2024-05-15 15:52:00.000000 pkrcomponents-1.6.5/pkrcomponents/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    15964 2024-05-24 00:19:33.000000 pkrcomponents-1.6.5/pkrcomponents/table.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    12206 2024-05-24 00:59:50.000000 pkrcomponents-1.6.5/pkrcomponents/table_player.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    10193 2024-05-24 02:25:21.000000 pkrcomponents-1.6.5/pkrcomponents/tournament.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 02:54:09.007574 pkrcomponents-1.6.5/pkrcomponents.egg-info/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1336 2024-05-24 02:54:07.000000 pkrcomponents-1.6.5/pkrcomponents.egg-info/SOURCES.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/requirements.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-24 02:54:09.020591 pkrcomponents-1.6.5/setup.cfg
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1334 2024-05-12 18:14:33.000000 pkrcomponents-1.6.5/setup.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 02:54:08.994561 pkrcomponents-1.6.5/tests/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2140 2023-09-25 10:39:52.000000 pkrcomponents-1.6.5/tests/test_action.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1388 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_bitcard.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     6309 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_board.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1459 2024-05-24 02:25:34.000000 pkrcomponents-1.6.5/tests/test_buyin.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2017 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     6271 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_combo.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      250 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_combo_range.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      338 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_common.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      555 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_constants.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1455 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_deck.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1649 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_evaluator.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1041 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_general.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     6753 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_hand.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1787 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_level.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      659 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_listings.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      290 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_lookup_table.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2765 2024-05-24 02:41:12.000000 pkrcomponents-1.6.5/tests/test_payouts.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2962 2024-05-08 12:10:46.000000 pkrcomponents-1.6.5/tests/test_players.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      513 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2995 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_rank.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      808 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_shape.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1285 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_suit.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    12901 2024-05-24 00:57:29.000000 pkrcomponents-1.6.5/tests/test_table.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4222 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_table_player.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     6358 2024-05-24 02:50:09.000000 pkrcomponents-1.6.5/tests/test_tournament.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 21:11:42.845291 pkrcomponents-1.6.6/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 21:11:42.360716 pkrcomponents-1.6.6/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.6.6/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.6.6/LICENSE.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-24 19:24:47.000000 pkrcomponents-1.6.6/MANIFEST.in
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      951 2024-05-24 21:11:42.845291 pkrcomponents-1.6.6/PKG-INFO
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      224 2024-05-24 00:25:51.000000 pkrcomponents-1.6.6/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.6.6/README.rst
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1040 2024-05-24 21:09:31.000000 pkrcomponents-1.6.6/coverage.txt
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 21:11:42.594128 pkrcomponents-1.6.6/pkrcomponents/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.6.6/pkrcomponents/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.6.6/pkrcomponents/_common.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1593 2024-05-24 00:57:29.000000 pkrcomponents-1.6.6/pkrcomponents/action.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7569 2024-05-24 00:57:29.000000 pkrcomponents-1.6.6/pkrcomponents/bitcard.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3948 2024-05-15 15:52:00.000000 pkrcomponents-1.6.6/pkrcomponents/board.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5296 2024-05-15 11:58:01.000000 pkrcomponents-1.6.6/pkrcomponents/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.6.6/pkrcomponents/constants.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.6.6/pkrcomponents/evaluator.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.6.6/pkrcomponents/hand.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.6.6/pkrcomponents/listings.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.6.6/pkrcomponents/lookup_table.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 21:11:42.625456 pkrcomponents-1.6.6/pkrcomponents/models/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 21:11:42.704909 pkrcomponents-1.6.6/pkrcomponents/models/actions/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.6.6/pkrcomponents/models/actions/move.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.6.6/pkrcomponents/models/actions/sequence.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.6.6/pkrcomponents/models/actions/street.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.6.6/pkrcomponents/models/amount.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 21:11:42.798445 pkrcomponents-1.6.6/pkrcomponents/models/cards/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.6.6/pkrcomponents/models/cards/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.6.6/pkrcomponents/models/cards/rank.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.6.6/pkrcomponents/models/cards/suit.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 21:11:42.814040 pkrcomponents-1.6.6/pkrcomponents/models/pots/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.6.6/pkrcomponents/models/pots/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4434 2024-05-15 18:17:46.000000 pkrcomponents-1.6.6/pkrcomponents/players.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      999 2024-05-15 15:52:00.000000 pkrcomponents-1.6.6/pkrcomponents/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    15964 2024-05-24 00:19:33.000000 pkrcomponents-1.6.6/pkrcomponents/table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    12206 2024-05-24 00:59:50.000000 pkrcomponents-1.6.6/pkrcomponents/table_player.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    10341 2024-05-24 21:07:41.000000 pkrcomponents-1.6.6/pkrcomponents/tournament.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 21:11:42.829673 pkrcomponents-1.6.6/pkrcomponents.egg-info/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      797 2024-05-24 21:11:41.000000 pkrcomponents-1.6.6/pkrcomponents.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.6.6/requirements.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-24 21:11:42.845291 pkrcomponents-1.6.6/setup.cfg
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1385 2024-05-24 19:24:47.000000 pkrcomponents-1.6.6/setup.py
```

### Comparing `pkrcomponents-1.6.5/LICENSE.txt` & `pkrcomponents-1.6.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/MANIFEST.in` & `pkrcomponents-1.6.6/MANIFEST.in`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 global-include *.txt *.md *.py
 prune build
 prune dist
 prune pkrcomponents.egg-info
 prune venv
 prune docs
-prune Tests
+prune tests
 prune scripts
 
 global-exclude *.py[cod]  # Exclure les fichiers de bytecode Python
 global-exclude *.swp      # Exclure les fichiers swap de Vim
 global-exclude *.bak      # Exclure les fichiers de sauvegarde
 global-exclude *.tmp      # Exclure les fichiers temporaires
 global-exclude .DS_Store  # Exclure les fichiers système spécifiques à MacOS
```

### Comparing `pkrcomponents-1.6.5/PKG-INFO` & `pkrcomponents-1.6.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkrcomponents
-Version: 1.6.5
+Version: 1.6.6
 Summary: A Poker Package
 Home-page: https://github.com/manggy94/PokerComponents
 Author: Alexandre MANGWA
 Author-email: alex.mangwa@gmail.com
 License: MIT
 Keywords: poker pkrcomponents pkr
 Platform: UNKNOWN
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Natural Language :: French
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Games/Entertainment :: Board Games
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # A Package of poker components for python
 
 ## Description
 A python package for coding around poker.
 Made to create poker related objects
```

### Comparing `pkrcomponents-1.6.5/coverage.txt` & `pkrcomponents-1.6.6/coverage.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 pkrcomponents/hand.py             226      0   100%
 pkrcomponents/listings.py          16      0   100%
 pkrcomponents/lookup_table.py     112      0   100%
 pkrcomponents/players.py           96      7    93%
 pkrcomponents/pot.py               25      2    92%
 pkrcomponents/table.py            317     49    85%
 pkrcomponents/table_player.py     248     30    88%
-pkrcomponents/tournament.py       254      0   100%
+pkrcomponents/tournament.py       256      1    99%
 ---------------------------------------------------
-TOTAL                            1734     91    95%
+TOTAL                            1736     92    95%
```

### Comparing `pkrcomponents-1.6.5/pkrcomponents/_common.py` & `pkrcomponents-1.6.6/pkrcomponents/_common.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/pkrcomponents/action.py` & `pkrcomponents-1.6.6/pkrcomponents/action.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/pkrcomponents/bitcard.py` & `pkrcomponents-1.6.6/pkrcomponents/bitcard.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/pkrcomponents/board.py` & `pkrcomponents-1.6.6/pkrcomponents/board.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/pkrcomponents/card.py` & `pkrcomponents-1.6.6/pkrcomponents/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/pkrcomponents/constants.py` & `pkrcomponents-1.6.6/pkrcomponents/constants.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/pkrcomponents/evaluator.py` & `pkrcomponents-1.6.6/pkrcomponents/evaluator.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/pkrcomponents/hand.py` & `pkrcomponents-1.6.6/pkrcomponents/hand.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/pkrcomponents/listings.py` & `pkrcomponents-1.6.6/pkrcomponents/listings.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/pkrcomponents/lookup_table.py` & `pkrcomponents-1.6.6/pkrcomponents/lookup_table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/pkrcomponents/models/actions/move.py` & `pkrcomponents-1.6.6/pkrcomponents/models/actions/move.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/pkrcomponents/models/actions/street.py` & `pkrcomponents-1.6.6/pkrcomponents/models/actions/street.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/pkrcomponents/models/amount.py` & `pkrcomponents-1.6.6/pkrcomponents/models/amount.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/pkrcomponents/models/cards/card.py` & `pkrcomponents-1.6.6/pkrcomponents/models/cards/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/pkrcomponents/models/cards/rank.py` & `pkrcomponents-1.6.6/pkrcomponents/models/cards/rank.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/pkrcomponents/models/cards/suit.py` & `pkrcomponents-1.6.6/pkrcomponents/models/cards/suit.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/pkrcomponents/models/pots/pot.py` & `pkrcomponents-1.6.6/pkrcomponents/models/pots/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/pkrcomponents/players.py` & `pkrcomponents-1.6.6/pkrcomponents/players.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/pkrcomponents/pot.py` & `pkrcomponents-1.6.6/pkrcomponents/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/pkrcomponents/table.py` & `pkrcomponents-1.6.6/pkrcomponents/table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/pkrcomponents/table_player.py` & `pkrcomponents-1.6.6/pkrcomponents/table_player.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.5/pkrcomponents/tournament.py` & `pkrcomponents-1.6.6/pkrcomponents/tournament.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,17 @@
         ko = total * 0.45
         rake = total * 0.1
         return cls(freeze, ko, rake)
 
     def __str__(self):
         return f"Buy-in: {self.total}"
 
+    def __eq__(self, other):
+        return self.freeze_part == other.freeze_part and self.ko_part == other.ko_part and self.rake == other.rake
+
     def to_json(self):
         return {
             "freeze": self.freeze_part,
             "ko": self.ko_part,
             "rake": self.rake
         }
```

### Comparing `pkrcomponents-1.6.5/setup.py` & `pkrcomponents-1.6.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,17 +33,18 @@
 
 
 setup(
     name="pkrcomponents",
     version=get_version(),
     description="A Poker Package",
     long_description=Path("README.md").read_text(),
+    long_description_content_type="text/markdown",
     classifiers=classifiers,
     keywords="poker pkrcomponents pkr",
     author="Alexandre MANGWA",
     author_email="alex.mangwa@gmail.com",
     url="https://github.com/manggy94/PokerComponents",
     license="MIT",
-    packages=find_packages(exclude=["Tests", ".venv", "venv", "venv.*"]),
+    packages=find_packages(exclude=["tests", ".venv", "venv", "venv.*"]),
     install_requires=install_requires,
     tests_require=["pytest", "pytest-cov", "coverage", "coveralls"],
 )
```


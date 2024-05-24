# Comparing `tmp/pkrcomponents-1.6.4.tar.gz` & `tmp/pkrcomponents-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkrcomponents-1.6.4.tar", last modified: Wed May 15 19:36:49 2024, max compression
+gzip compressed data, was "pkrcomponents-1.6.5.tar", last modified: Fri May 24 02:54:11 2024, max compression
```

## Comparing `pkrcomponents-1.6.4.tar` & `pkrcomponents-1.6.5.tar`

### file list

```diff
@@ -1,48 +1,69 @@
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 19:36:49.296398 pkrcomponents-1.6.4/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 19:36:48.696828 pkrcomponents-1.6.4/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.6.4/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.6.4/LICENSE.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-14 20:27:30.000000 pkrcomponents-1.6.4/MANIFEST.in
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      704 2024-05-15 19:36:49.292314 pkrcomponents-1.6.4/PKG-INFO
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-04-16 08:43:13.000000 pkrcomponents-1.6.4/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.6.4/README.rst
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 19:36:48.963116 pkrcomponents-1.6.4/pkrcomponents/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.6.4/pkrcomponents/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.6.4/pkrcomponents/_common.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1507 2023-07-18 00:15:12.000000 pkrcomponents-1.6.4/pkrcomponents/action.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7279 2023-07-18 00:15:12.000000 pkrcomponents-1.6.4/pkrcomponents/bitcard.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3948 2024-05-15 15:52:00.000000 pkrcomponents-1.6.4/pkrcomponents/board.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5296 2024-05-15 11:58:01.000000 pkrcomponents-1.6.4/pkrcomponents/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.6.4/pkrcomponents/constants.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.6.4/pkrcomponents/evaluator.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.6.4/pkrcomponents/hand.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.6.4/pkrcomponents/listings.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.6.4/pkrcomponents/lookup_table.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 19:36:48.988766 pkrcomponents-1.6.4/pkrcomponents/models/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 19:36:49.075526 pkrcomponents-1.6.4/pkrcomponents/models/actions/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.6.4/pkrcomponents/models/actions/move.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.6.4/pkrcomponents/models/actions/sequence.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.6.4/pkrcomponents/models/actions/street.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.6.4/pkrcomponents/models/amount.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 19:36:49.161698 pkrcomponents-1.6.4/pkrcomponents/models/cards/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.6.4/pkrcomponents/models/cards/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.6.4/pkrcomponents/models/cards/rank.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.6.4/pkrcomponents/models/cards/suit.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 19:36:49.188207 pkrcomponents-1.6.4/pkrcomponents/models/pots/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.6.4/pkrcomponents/models/pots/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4434 2024-05-15 18:17:46.000000 pkrcomponents-1.6.4/pkrcomponents/players.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      999 2024-05-15 15:52:00.000000 pkrcomponents-1.6.4/pkrcomponents/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    15936 2024-05-15 19:34:36.000000 pkrcomponents-1.6.4/pkrcomponents/table.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    12178 2024-05-15 18:33:59.000000 pkrcomponents-1.6.4/pkrcomponents/table_player.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 19:36:48.619847 pkrcomponents-1.6.4/pkrcomponents/tests/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 19:36:49.237124 pkrcomponents-1.6.4/pkrcomponents/tests/actions/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 19:36:49.264527 pkrcomponents-1.6.4/pkrcomponents/tests/actions/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2023-11-10 19:00:33.000000 pkrcomponents-1.6.4/pkrcomponents/tests/actions/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3185 2023-11-10 19:03:11.000000 pkrcomponents-1.6.4/pkrcomponents/tests/actions/test_move.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1970 2023-11-10 19:18:13.000000 pkrcomponents-1.6.4/pkrcomponents/tests/actions/test_street.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7577 2024-05-15 07:44:35.000000 pkrcomponents-1.6.4/pkrcomponents/tournament.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 19:36:49.281877 pkrcomponents-1.6.4/pkrcomponents.egg-info/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      920 2024-05-15 19:36:47.000000 pkrcomponents-1.6.4/pkrcomponents.egg-info/SOURCES.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.6.4/requirements.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-15 19:36:49.297432 pkrcomponents-1.6.4/setup.cfg
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1334 2024-05-12 18:14:33.000000 pkrcomponents-1.6.4/setup.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 02:54:09.019588 pkrcomponents-1.6.5/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 02:54:08.283221 pkrcomponents-1.6.5/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.6.5/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.6.5/LICENSE.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-14 20:27:30.000000 pkrcomponents-1.6.5/MANIFEST.in
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2024-05-24 02:54:09.015588 pkrcomponents-1.6.5/PKG-INFO
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      224 2024-05-24 00:25:51.000000 pkrcomponents-1.6.5/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/README.rst
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1040 2024-05-24 02:50:24.000000 pkrcomponents-1.6.5/coverage.txt
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 02:54:08.468843 pkrcomponents-1.6.5/pkrcomponents/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/pkrcomponents/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/pkrcomponents/_common.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1593 2024-05-24 00:57:29.000000 pkrcomponents-1.6.5/pkrcomponents/action.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7569 2024-05-24 00:57:29.000000 pkrcomponents-1.6.5/pkrcomponents/bitcard.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3948 2024-05-15 15:52:00.000000 pkrcomponents-1.6.5/pkrcomponents/board.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5296 2024-05-15 11:58:01.000000 pkrcomponents-1.6.5/pkrcomponents/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/pkrcomponents/constants.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/pkrcomponents/evaluator.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/pkrcomponents/hand.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.6.5/pkrcomponents/listings.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/pkrcomponents/lookup_table.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 02:54:08.495956 pkrcomponents-1.6.5/pkrcomponents/models/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 02:54:08.572024 pkrcomponents-1.6.5/pkrcomponents/models/actions/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.6.5/pkrcomponents/models/actions/move.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.6.5/pkrcomponents/models/actions/sequence.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.6.5/pkrcomponents/models/actions/street.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.6.5/pkrcomponents/models/amount.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 02:54:08.666993 pkrcomponents-1.6.5/pkrcomponents/models/cards/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.6.5/pkrcomponents/models/cards/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.6.5/pkrcomponents/models/cards/rank.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.6.5/pkrcomponents/models/cards/suit.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 02:54:08.691502 pkrcomponents-1.6.5/pkrcomponents/models/pots/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.6.5/pkrcomponents/models/pots/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4434 2024-05-15 18:17:46.000000 pkrcomponents-1.6.5/pkrcomponents/players.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      999 2024-05-15 15:52:00.000000 pkrcomponents-1.6.5/pkrcomponents/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    15964 2024-05-24 00:19:33.000000 pkrcomponents-1.6.5/pkrcomponents/table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    12206 2024-05-24 00:59:50.000000 pkrcomponents-1.6.5/pkrcomponents/table_player.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    10193 2024-05-24 02:25:21.000000 pkrcomponents-1.6.5/pkrcomponents/tournament.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 02:54:09.007574 pkrcomponents-1.6.5/pkrcomponents.egg-info/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1336 2024-05-24 02:54:07.000000 pkrcomponents-1.6.5/pkrcomponents.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/requirements.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-24 02:54:09.020591 pkrcomponents-1.6.5/setup.cfg
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1334 2024-05-12 18:14:33.000000 pkrcomponents-1.6.5/setup.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 02:54:08.994561 pkrcomponents-1.6.5/tests/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2140 2023-09-25 10:39:52.000000 pkrcomponents-1.6.5/tests/test_action.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1388 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_bitcard.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     6309 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_board.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1459 2024-05-24 02:25:34.000000 pkrcomponents-1.6.5/tests/test_buyin.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2017 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     6271 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_combo.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      250 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_combo_range.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      338 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_common.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      555 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_constants.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1455 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_deck.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1649 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_evaluator.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1041 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_general.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     6753 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_hand.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1787 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_level.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      659 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_listings.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      290 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_lookup_table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2765 2024-05-24 02:41:12.000000 pkrcomponents-1.6.5/tests/test_payouts.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2962 2024-05-08 12:10:46.000000 pkrcomponents-1.6.5/tests/test_players.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      513 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2995 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_rank.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      808 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_shape.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1285 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_suit.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    12901 2024-05-24 00:57:29.000000 pkrcomponents-1.6.5/tests/test_table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4222 2023-07-18 00:15:12.000000 pkrcomponents-1.6.5/tests/test_table_player.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     6358 2024-05-24 02:50:09.000000 pkrcomponents-1.6.5/tests/test_tournament.py
```

### Comparing `pkrcomponents-1.6.4/LICENSE.txt` & `pkrcomponents-1.6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.4/MANIFEST.in` & `pkrcomponents-1.6.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.4/pkrcomponents/_common.py` & `pkrcomponents-1.6.5/pkrcomponents/_common.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.4/pkrcomponents/action.py` & `pkrcomponents-1.6.5/pkrcomponents/action.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     def __str__(self):
         return f"{self.player.name} does a {self.move} for {self.value}"
 
     @property
     def player(self):
         """
         Player involved in an action
+
+        Returns:
+            TablePlayer: The table_player involved in the action
         """
         return self._player
 
     @player.setter
     def player(self, player):
         """
         Player setter
```

### Comparing `pkrcomponents-1.6.4/pkrcomponents/bitcard.py` & `pkrcomponents-1.6.5/pkrcomponents/bitcard.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,30 +52,35 @@
         elif isinstance(card, Card):
             return BitCard.from_card(card)
         return BitCard.from_int(card)
 
     @classmethod
     def from_card(cls, card: Card) -> BitCard:
         """
-        Converts Card  to binary integer representation of card
-        example:
+        Converts Card to binary integer representation of card
         """
         rank_int = BitCard.char_to_int_rank[f"{card.rank}"]
         suit_int = BitCard.char_to_int_suit[f"{Card(card).suit}"]
         prime = BitCard.primes[rank_int]
         bit_rank = 1 << rank_int << 16
         rank = rank_int << 8
         suit = suit_int << 12
         card_int = bit_rank | suit | rank | prime
         return BitCard.from_int(card_int)
 
     @classmethod
     def from_string(cls, str_card) -> BitCard:
         """
-
+        Converts a string representation of a card to a 32-bit integer representation
+        Example:
+            "Kd" --> 134236965
+        Args:
+            str_card (str): A string representation of a card
+        Returns:
+            BitCard: The 32-bit int representing the card as described above
         """
         card = Card(str_card)
         return BitCard.from_card(card)
 
     @classmethod
     def from_int(cls, card_int: int) -> BitCard:
         """
```

### Comparing `pkrcomponents-1.6.4/pkrcomponents/board.py` & `pkrcomponents-1.6.5/pkrcomponents/board.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.4/pkrcomponents/card.py` & `pkrcomponents-1.6.5/pkrcomponents/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.4/pkrcomponents/constants.py` & `pkrcomponents-1.6.5/pkrcomponents/constants.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.4/pkrcomponents/evaluator.py` & `pkrcomponents-1.6.5/pkrcomponents/evaluator.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.4/pkrcomponents/hand.py` & `pkrcomponents-1.6.5/pkrcomponents/hand.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.4/pkrcomponents/listings.py` & `pkrcomponents-1.6.5/pkrcomponents/listings.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.4/pkrcomponents/lookup_table.py` & `pkrcomponents-1.6.5/pkrcomponents/lookup_table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.4/pkrcomponents/models/actions/move.py` & `pkrcomponents-1.6.5/pkrcomponents/models/actions/move.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.4/pkrcomponents/models/actions/street.py` & `pkrcomponents-1.6.5/pkrcomponents/models/actions/street.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.4/pkrcomponents/models/amount.py` & `pkrcomponents-1.6.5/pkrcomponents/models/amount.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.4/pkrcomponents/models/cards/card.py` & `pkrcomponents-1.6.5/pkrcomponents/models/cards/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.4/pkrcomponents/models/cards/rank.py` & `pkrcomponents-1.6.5/pkrcomponents/models/cards/rank.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.4/pkrcomponents/models/cards/suit.py` & `pkrcomponents-1.6.5/pkrcomponents/models/cards/suit.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.4/pkrcomponents/models/pots/pot.py` & `pkrcomponents-1.6.5/pkrcomponents/models/pots/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.4/pkrcomponents/players.py` & `pkrcomponents-1.6.5/pkrcomponents/players.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.4/pkrcomponents/pot.py` & `pkrcomponents-1.6.5/pkrcomponents/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.4/pkrcomponents/table.py` & `pkrcomponents-1.6.5/pkrcomponents/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         self._players = Players()
         self._pot = Pot()
         self._evaluator = Evaluator()
         self._is_mtt = False
         self._street = Street.PREFLOP
         self.max_players = max_players
         self._hand_has_started = False
+        self._cnt_bets = 0
 
     @property
     def board(self):
         """Returns the associated board """
         return self._board
 
     @property
```

### Comparing `pkrcomponents-1.6.4/pkrcomponents/table_player.py` & `pkrcomponents-1.6.5/pkrcomponents/table_player.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     _init_stack: float
     _combo: Combo or None
     _folded: bool
     _hero: bool
     _position: Position or None
     _table: Table
     _max_reward: float
-    _ko: float
+    _bounty: float
 
     def __init__(self, name: str = "Villain", seat=0, stack: float = 0):
         self.name = name
         self.seat = seat
         if stack < 0:
             raise ValueError("Init stack cannot be negative")
         else:
@@ -260,15 +260,15 @@
             self._table = table
             table.players.add_player(self)
             self.reset_street_status()
 
     def sit_out(self):
         """Removes player from the table"""
         self.reset_street_status()
-        self.table.remove_player(self)
+        self.table.players.remove_player(self)
         delattr(self, "_table")
 
     def pay(self, value):
         """Action of paying a value"""
         amount = self.max_bet(value)
         self.stack -= amount
         self.table.pot.add(amount)
@@ -372,15 +372,15 @@
         postflop_bets.append({"text": "All-in", "value": self.stack})
         if self.table.min_bet < self.stack:
             postflop_bets.append({"text": "Min Bet", "value": self.table.min_bet})
         postflop_bets = sorted(postflop_bets, key=lambda x: x.get("value"))
         return postflop_bets
 
     @property
-    def ko(self):
-        """Returns the knockout value"""
-        return self._ko
-
-    @ko.setter
-    def ko(self, value):
-        """Setter for knockout value"""
-        self._ko = value
+    def bounty(self):
+        """Returns the bounty value"""
+        return self._bounty
+
+    @bounty.setter
+    def bounty(self, value):
+        """Setter for bounty value"""
+        self._bounty = value
```

### Comparing `pkrcomponents-1.6.4/pkrcomponents/tournament.py` & `pkrcomponents-1.6.5/pkrcomponents/tournament.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,75 @@
 from pkrcomponents.constants import MoneyType
 
 
+class Buyin:
+    """
+    A class for the buy-in of a tournament
+    """
+    _freeze_part: float
+    _ko_part: float
+    _rake: float
+
+    def __init__(self, freeze: float, ko: float, rake: float):
+        self._freeze_part = freeze
+        self._ko_part = ko
+        self._rake = rake
+
+    @property
+    def freeze_part(self):
+        return self._freeze_part
+
+    @freeze_part.setter
+    def freeze_part(self, freeze):
+        if freeze < 0:
+            raise ValueError("Freeze part must be positive")
+        self._freeze_part = freeze
+
+    @property
+    def ko_part(self):
+        return self._ko_part
+
+    @ko_part.setter
+    def ko_part(self, ko):
+        if ko < 0:
+            raise ValueError("KO part must be positive")
+        self._ko_part = ko
+
+    @property
+    def rake(self):
+        return self._rake
+
+    @rake.setter
+    def rake(self, rake):
+        if rake < 0:
+            raise ValueError("Rake must be positive")
+        self._rake = rake
+
+    @property
+    def total(self):
+        return self.freeze_part + self.ko_part + self.rake
+
+    @classmethod
+    def from_total(cls, total: float):
+        freeze = total * 0.45
+        ko = total * 0.45
+        rake = total * 0.1
+        return cls(freeze, ko, rake)
+
+    def __str__(self):
+        return f"Buy-in: {self.total}"
+
+    def to_json(self):
+        return {
+            "freeze": self.freeze_part,
+            "ko": self.ko_part,
+            "rake": self.rake
+        }
+
+
 class Level:
     """Level of the tournament"""
 
     _level: int
     _sb: float
     _bb: float
     _ante: float
@@ -45,20 +110,20 @@
     def ante(self, ante):
         if ante < 0:
             raise ValueError("Ante must be positive")
         else:
             self._ante = ante
 
     @property
-    def level(self):
+    def level(self) -> int:
         return self._level
 
     @level.setter
     def level(self, level):
-        if level < 0 or type(level) != int:
+        if level < 0 or not isinstance(level, int):
             raise ValueError("Level must be a positive int")
         else:
             self._level = level
 
     def to_json(self):
         return {
             "level": self.level,
@@ -68,21 +133,44 @@
         }
 
 
 class Payout:
     """
     A class for a payout in a tournament
     """
+    _tier: int
+    _reward: float
+
     def __init__(self, tier: int, reward: float):
-        self.tier = tier
-        self.reward = reward
+        self._tier = tier
+        self._reward = reward
 
     def __str__(self):
         return f"Tier: {self.tier} - Reward: {self.reward}"
 
+    @property
+    def tier(self) -> int:
+        return self._tier
+
+    @tier.setter
+    def tier(self, tier):
+        if tier < 0 or not isinstance(tier, int):
+            raise ValueError("Tier must be a positive integer")
+        self._tier = tier
+
+    @property
+    def reward(self) -> float:
+        return self._reward
+
+    @reward.setter
+    def reward(self, reward):
+        if reward < 0 or not isinstance(reward, float):
+            raise ValueError("Reward must be positive")
+        self._reward = reward
+
 
 class Payouts(list):
     """
     A list of payouts
     """
 
     def add_payout(self, payout: Payout):
@@ -121,17 +209,17 @@
 
     def get_reward(self, rank: int) -> float:
         """
         A method to get the reward for a given finish rank
         """
         return self.get_payout(rank).reward
 
-    def get_prizepool(self) -> float:
+    def get_prize_pool(self) -> float:
         """
-        A method to get the total prizepool distributed via the payouts
+        A method to get the total prize pool distributed via the payouts
         """
         return sum(self.get_reward(rank) for rank in range(1, max(self.tiers)+1))
 
     @property
     def tiers(self):
         """
         A property to get the tiers of the payouts
@@ -146,33 +234,43 @@
         return [payout.reward for payout in self]
 
 
 class Tournament:
     """Class for played tournaments"""
     _id: str
     _name: str
-    _buyin: float
+    _buyin: Buyin
     _is_ko: bool = True
     _money_type: str = "real"
     _level: Level
     _payouts: Payouts
     _players_remaining: int
     _total_players: int
     _starting_stack: float
 
-    def __init__(self, ident: str = '0000', name: str = 'Kill The Fish', is_ko=True, buyin: float = 5.0,
-                 money_type: str = 'real', level: Level = Level(), starting_stack: float = 20000
+    def __init__(self,
+                 ident: str = '0000',
+                 name: str = 'Kill The Fish',
+                 is_ko=True,
+                 buyin: Buyin = Buyin(2.25, 2.25, 0.5),
+                 money_type: str = 'real',
+                 level: Level = Level(),
+                 starting_stack: float = 20000,
+                 total_players: int = None,
+                 players_remaining: int = None
                  ):
         self._id = ident
         self._name = name
         self._buyin = buyin
         self.money_type = money_type
         self._is_ko = is_ko
         self._level = level
         self._starting_stack = starting_stack
+        self._total_players = total_players
+        self._players_remaining = players_remaining
 
     @property
     def id(self):
         return self._id
 
     @id.setter
     def id(self, id_txt: str):
@@ -187,67 +285,78 @@
         self._name = name_txt
 
     @property
     def buyin(self):
         return self._buyin
 
     @buyin.setter
-    def buyin(self, amount):
-        self._buyin = max(0.0, float(amount))
+    def buyin(self, buyin: Buyin):
+        self._buyin = buyin
 
     @property
     def money_type(self):
         return self._money_type
 
     @money_type.setter
     def money_type(self, money_type):
         self._money_type = MoneyType(money_type)
 
     @property
-    def level(self):
+    def level(self) -> Level:
         return self._level
 
     @level.setter
     def level(self, level):
+
         self._level = level
 
     @property
     def is_ko(self):
         return self._is_ko
 
     @is_ko.setter
     def is_ko(self, is_ko):
         self._is_ko = bool(is_ko)
 
     @property
     def payouts(self):
         return self._payouts
 
+    @payouts.setter
+    def payouts(self, payouts):
+        self._payouts = payouts
+
     @property
     def total_players(self):
         return self._total_players
 
     @total_players.setter
     def total_players(self, total_players):
+        if total_players < 0 or not isinstance(total_players, int):
+            raise ValueError("Total players must be a positive integer")
         self._total_players = total_players
 
     @property
-    def players_remaining(self):
+    def players_remaining(self) -> int:
         return self._players_remaining
 
     @players_remaining.setter
     def players_remaining(self, players_remaining):
+        if players_remaining < 0 or players_remaining > self.total_players:
+            raise ValueError("Players remaining must be a positive integer and less than total players")
         self._players_remaining = players_remaining
 
     @property
     def starting_stack(self):
         return self._starting_stack
 
     @starting_stack.setter
     def starting_stack(self, starting_stack):
+        if starting_stack < 0:
+            raise ValueError("Starting stack must be positive")
         self._starting_stack = starting_stack
 
     @property
     def total_chips(self):
         return self.total_players * self.starting_stack
 
     @property
@@ -256,15 +365,15 @@
 
     @property
     def players_eliminated(self):
         return self.total_players - self.players_remaining
 
     @property
     def tournament_progression(self):
-        return self.players_eliminated / self.total_players - 1
+        return self.players_eliminated / (self.total_players - 1)
 
     @property
     def next_tier(self):
         return self.payouts.closest_payout(self.players_remaining).tier
 
     @property
     def next_reward(self):
@@ -278,28 +387,13 @@
         return f"Name: {self.name}\nId: {self.id}\nBuy-in: {self.buyin}\nMoney: {self.money_type}"
 
     def to_json(self):
         return {
             "level": self.level.to_json(),
             "id": self.id,
             "name": self.name,
-            "buy_in": self.buyin,
+            "buy_in": self.buyin.to_json(),
             "is_ko": self.is_ko,
             "money_type": self.money_type
         }
 
 
-
-
-if __name__ == "__main__":
-    p1 = Payout(1, 100.0)
-    p2 = Payout(2, 50.0)
-    p3 = Payout(3, 25.0)
-    p4 = Payout(6, 10.0)
-    p5 = Payout(12, 5.0)
-
-    payouts = Payouts([p1, p2, p3, p4, p5])
-
-
-    print(payouts.get_payout(15), payouts.get_reward(5))
-    print(payouts.get_prizepool())
-    print(payouts.closest_payout(7))
```

### Comparing `pkrcomponents-1.6.4/setup.py` & `pkrcomponents-1.6.5/setup.py`

 * *Files identical despite different names*


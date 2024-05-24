# Comparing `tmp/pokerkit-0.5.0a1.tar.gz` & `tmp/pokerkit-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokerkit-0.5.0a1.tar", last modified: Wed Apr 24 16:36:22 2024, max compression
+gzip compressed data, was "pokerkit-0.5.1.tar", last modified: Fri May 24 14:54:49 2024, max compression
```

## Comparing `pokerkit-0.5.0a1.tar` & `pokerkit-0.5.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-04-24 16:36:22.334641 pokerkit-0.5.0a1/
--rw-rw-r--   0 juho      (1000) juho      (1000)     1116 2024-04-11 09:02:36.000000 pokerkit-0.5.0a1/LICENSE
--rw-r--r--   0 juho      (1000) juho      (1000)    17204 2024-04-24 16:36:22.334641 pokerkit-0.5.0a1/PKG-INFO
--rw-rw-r--   0 juho      (1000) juho      (1000)    15530 2024-04-23 17:49:32.000000 pokerkit-0.5.0a1/README.rst
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-04-24 16:36:22.334641 pokerkit-0.5.0a1/pokerkit/
--rw-rw-r--   0 juho      (1000) juho      (1000)     4460 2024-04-20 15:21:12.000000 pokerkit-0.5.0a1/pokerkit/__init__.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    15073 2024-04-09 08:26:29.000000 pokerkit-0.5.0a1/pokerkit/analysis.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    73909 2024-04-24 16:25:13.000000 pokerkit-0.5.0a1/pokerkit/games.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    21443 2024-04-09 09:11:40.000000 pokerkit-0.5.0a1/pokerkit/hands.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    15305 2024-04-09 09:11:43.000000 pokerkit-0.5.0a1/pokerkit/lookups.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    28717 2024-04-09 08:58:34.000000 pokerkit-0.5.0a1/pokerkit/notation.py
--rw-rw-r--   0 juho      (1000) juho      (1000)        0 2024-03-03 02:45:25.000000 pokerkit-0.5.0a1/pokerkit/py.typed
--rw-rw-r--   0 juho      (1000) juho      (1000)   195732 2024-04-24 16:33:47.000000 pokerkit-0.5.0a1/pokerkit/state.py
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-04-24 16:36:22.334641 pokerkit-0.5.0a1/pokerkit/tests/
--rw-rw-r--   0 juho      (1000) juho      (1000)       88 2024-03-03 02:45:25.000000 pokerkit-0.5.0a1/pokerkit/tests/__init__.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    17128 2024-03-25 16:57:08.000000 pokerkit-0.5.0a1/pokerkit/tests/test_analysis.py
--rw-rw-r--   0 juho      (1000) juho      (1000)     6485 2024-04-23 17:51:34.000000 pokerkit-0.5.0a1/pokerkit/tests/test_games.py
--rw-rw-r--   0 juho      (1000) juho      (1000)     5331 2024-03-15 11:23:34.000000 pokerkit-0.5.0a1/pokerkit/tests/test_lookups.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    28167 2024-03-29 06:34:10.000000 pokerkit-0.5.0a1/pokerkit/tests/test_notation.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    35725 2024-04-23 17:51:05.000000 pokerkit-0.5.0a1/pokerkit/tests/test_papers.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    39414 2024-04-24 16:31:51.000000 pokerkit-0.5.0a1/pokerkit/tests/test_state.py
--rw-rw-r--   0 juho      (1000) juho      (1000)     2062 2024-04-23 17:51:13.000000 pokerkit-0.5.0a1/pokerkit/tests/test_utilities.py
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-04-24 16:36:22.334641 pokerkit-0.5.0a1/pokerkit/tests/test_wsop/
--rw-rw-r--   0 juho      (1000) juho      (1000)      141 2024-03-03 02:45:25.000000 pokerkit-0.5.0a1/pokerkit/tests/test_wsop/__init__.py
--rw-rw-r--   0 juho      (1000) juho      (1000)   193298 2024-04-16 23:01:37.000000 pokerkit-0.5.0a1/pokerkit/tests/test_wsop/test_2023_43_5.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    32968 2024-04-23 17:38:59.000000 pokerkit-0.5.0a1/pokerkit/tests/test_wsop/test_2023_54_4.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    20720 2024-04-24 16:31:35.000000 pokerkit-0.5.0a1/pokerkit/utilities.py
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-04-24 16:36:22.334641 pokerkit-0.5.0a1/pokerkit.egg-info/
--rw-r--r--   0 juho      (1000) juho      (1000)    17204 2024-04-24 16:36:22.000000 pokerkit-0.5.0a1/pokerkit.egg-info/PKG-INFO
--rw-rw-r--   0 juho      (1000) juho      (1000)      698 2024-04-24 16:36:22.000000 pokerkit-0.5.0a1/pokerkit.egg-info/SOURCES.txt
--rw-rw-r--   0 juho      (1000) juho      (1000)        1 2024-04-24 16:36:22.000000 pokerkit-0.5.0a1/pokerkit.egg-info/dependency_links.txt
--rw-rw-r--   0 juho      (1000) juho      (1000)        9 2024-04-24 16:36:22.000000 pokerkit-0.5.0a1/pokerkit.egg-info/top_level.txt
--rw-rw-r--   0 juho      (1000) juho      (1000)       38 2024-04-24 16:36:22.334641 pokerkit-0.5.0a1/setup.cfg
--rw-rw-r--   0 juho      (1000) juho      (1000)     2143 2024-04-24 16:33:25.000000 pokerkit-0.5.0a1/setup.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-05-24 14:54:49.909851 pokerkit-0.5.1/
+-rw-rw-r--   0 juho      (1000) juho      (1000)     1116 2024-04-26 03:43:03.000000 pokerkit-0.5.1/LICENSE
+-rw-r--r--   0 juho      (1000) juho      (1000)    17581 2024-05-24 14:54:49.909851 pokerkit-0.5.1/PKG-INFO
+-rw-rw-r--   0 juho      (1000) juho      (1000)    15909 2024-04-26 03:43:03.000000 pokerkit-0.5.1/README.rst
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-05-24 14:54:49.905851 pokerkit-0.5.1/pokerkit/
+-rw-rw-r--   0 juho      (1000) juho      (1000)     4460 2024-04-26 03:43:03.000000 pokerkit-0.5.1/pokerkit/__init__.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    15377 2024-05-24 14:48:46.000000 pokerkit-0.5.1/pokerkit/analysis.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    74000 2024-05-23 03:49:37.000000 pokerkit-0.5.1/pokerkit/games.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    21551 2024-04-26 03:43:03.000000 pokerkit-0.5.1/pokerkit/hands.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    15389 2024-04-26 03:43:03.000000 pokerkit-0.5.1/pokerkit/lookups.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    34328 2024-04-26 03:43:03.000000 pokerkit-0.5.1/pokerkit/notation.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)        0 2024-03-03 02:45:25.000000 pokerkit-0.5.1/pokerkit/py.typed
+-rw-rw-r--   0 juho      (1000) juho      (1000)   203233 2024-05-20 00:27:57.000000 pokerkit-0.5.1/pokerkit/state.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-05-24 14:54:49.909851 pokerkit-0.5.1/pokerkit/tests/
+-rw-rw-r--   0 juho      (1000) juho      (1000)       88 2024-03-03 02:45:25.000000 pokerkit-0.5.1/pokerkit/tests/__init__.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    17128 2024-04-26 03:42:57.000000 pokerkit-0.5.1/pokerkit/tests/test_analysis.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)     6485 2024-04-26 03:43:03.000000 pokerkit-0.5.1/pokerkit/tests/test_games.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)     5331 2024-04-26 03:42:57.000000 pokerkit-0.5.1/pokerkit/tests/test_lookups.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    28167 2024-04-26 03:42:57.000000 pokerkit-0.5.1/pokerkit/tests/test_notation.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    37063 2024-05-20 00:27:57.000000 pokerkit-0.5.1/pokerkit/tests/test_papers.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    39414 2024-04-26 03:43:03.000000 pokerkit-0.5.1/pokerkit/tests/test_state.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)     2062 2024-04-26 03:42:57.000000 pokerkit-0.5.1/pokerkit/tests/test_utilities.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-05-24 14:54:49.909851 pokerkit-0.5.1/pokerkit/tests/test_wsop/
+-rw-rw-r--   0 juho      (1000) juho      (1000)      141 2024-04-26 03:42:57.000000 pokerkit-0.5.1/pokerkit/tests/test_wsop/__init__.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)   193298 2024-04-26 03:42:57.000000 pokerkit-0.5.1/pokerkit/tests/test_wsop/test_2023_43_5.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    32968 2024-04-26 03:43:03.000000 pokerkit-0.5.1/pokerkit/tests/test_wsop/test_2023_54_4.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    21226 2024-04-26 03:43:03.000000 pokerkit-0.5.1/pokerkit/utilities.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-05-24 14:54:49.909851 pokerkit-0.5.1/pokerkit.egg-info/
+-rw-r--r--   0 juho      (1000) juho      (1000)    17581 2024-05-24 14:54:49.000000 pokerkit-0.5.1/pokerkit.egg-info/PKG-INFO
+-rw-rw-r--   0 juho      (1000) juho      (1000)      698 2024-05-24 14:54:49.000000 pokerkit-0.5.1/pokerkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 juho      (1000) juho      (1000)        1 2024-05-24 14:54:49.000000 pokerkit-0.5.1/pokerkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 juho      (1000) juho      (1000)        9 2024-05-24 14:54:49.000000 pokerkit-0.5.1/pokerkit.egg-info/top_level.txt
+-rw-rw-r--   0 juho      (1000) juho      (1000)       38 2024-05-24 14:54:49.909851 pokerkit-0.5.1/setup.cfg
+-rw-rw-r--   0 juho      (1000) juho      (1000)     2141 2024-05-24 14:52:05.000000 pokerkit-0.5.1/setup.py
```

### Comparing `pokerkit-0.5.0a1/LICENSE` & `pokerkit-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a1/PKG-INFO` & `pokerkit-0.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerkit
-Version: 0.5.0a1
+Version: 0.5.1
 Summary: An open-source Python library for poker game simulations, hand evaluations, and statistical analysis
 Home-page: https://github.com/uoftcprg/pokerkit
 Author: University of Toronto Computer Poker Student Research Group
 Author-email: uoftcprg@studentorg.utoronto.ca
 License: MIT
 Project-URL: Documentation, https://pokerkit.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/uoftcprg/pokerkit
@@ -61,16 +61,20 @@
 Multi-Runout in an All-In Situation
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Below shows the 4-runout hand between Phil Hellmuth and the Loose Cannon Ernest Wiggins.
 
 Link: https://youtu.be/cnjJv7x0HMY?si=4l05Ez7lQVczt8DI&t=638
 
+Note that the starting stacks for some players are set to be ``math.inf`` as they are not mentioned.
+
 .. code-block:: python
 
+   from math import inf
+
    from pokerkit import Automation, Mode, NoLimitTexasHoldem
 
    state = NoLimitTexasHoldem.create_state(
        # Automations
        (
            Automation.ANTE_POSTING,
            Automation.BET_COLLECTION,
@@ -80,15 +84,15 @@
            Automation.CHIPS_PUSHING,
            Automation.CHIPS_PULLING,
        ),
        False,  # Uniform antes?
        {-1: 600},  # Antes
        (200, 400, 800),  # Blinds or straddles
        400,  # Min-bet
-       (999999, 116400, 86900, 999999, 50000, 999999),  # Starting stacks
+       (inf, 116400, 86900, inf, 50000, inf),  # Starting stacks
        6,  # Number of players
        mode=Mode.CASH_GAME,
    )
 
 Below are the pre-flop dealings and actions.
 
 .. code-block:: python
@@ -167,25 +171,29 @@
    state.burn_card('??')
    state.deal_board('Kd')  # River
 
 Below are the final stacks.
 
 .. code-block:: python
 
-   print(state.stacks)  # [987399, 79400, 149700, 999999, 37400, 999399]
+   print(state.stacks)  # [inf, 79400, 149700, inf, 37400, inf]
 
 A Sample No-Limit Texas Hold'em Hand
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Below shows the first televised million-dollar pot between Tom Dwan and Phil Ivey.
 
 Link: https://youtu.be/GnxFohpljqM
 
+Note that the starting stack of Patrik Antonius is set to be ``math.inf`` as it is not mentioned.
+
 .. code-block:: python
 
+   from math import inf
+
    from pokerkit import Automation, NoLimitTexasHoldem
 
    state = NoLimitTexasHoldem.create_state(
        # Automations
        (
            Automation.ANTE_POSTING,
            Automation.BET_COLLECTION,
@@ -195,15 +203,15 @@
            Automation.CHIPS_PUSHING,
            Automation.CHIPS_PULLING,
        ),
        True,  # Uniform antes?
        500,  # Antes
        (1000, 2000),  # Blinds or straddles
        2000,  # Min-bet
-       (1125600, 2000000, 553500),  # Starting stacks
+       (1125600, inf, 553500),  # Starting stacks
        3,  # Number of players
    )
 
 Below are the pre-flop dealings and actions.
 
 .. code-block:: python
 
@@ -245,15 +253,15 @@
    state.burn_card('??')
    state.deal_board('Jh')
 
 Below are the final stacks.
 
 .. code-block:: python
 
-   print(state.stacks)  # [572100, 1997500, 1109500]
+   print(state.stacks)  # [572100, inf, 1109500]
 
 A Sample Short-Deck Hold'em Hand
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Below shows an all-in hand between Xuan and Phua.
 
 Link: https://youtu.be/QlgCcphLjaQ
@@ -495,16 +503,20 @@
 A Sample Badugi Hand
 ^^^^^^^^^^^^^^^^^^^^
 
 Below shows an example badugi hand from Wikipedia.
 
 Link: https://en.wikipedia.org/wiki/Badugi
 
+Note that the starting stacks are set to be ``math.inf`` as they are not mentioned.
+
 .. code-block:: python
 
+   from math import inf
+
    from pokerkit import Automation, FixedLimitBadugi
 
    state = FixedLimitBadugi.create_state(
        # Automations
        (
            Automation.ANTE_POSTING,
            Automation.BET_COLLECTION,
@@ -514,15 +526,15 @@
            Automation.CHIPS_PULLING,
        ),
        True,  # Uniform antes?
        0,  # Antes
        (1, 2),  # Blinds or straddles
        2,  # Small-bet
        4,  # Big-bet
-       200,  # Starting stacks
+       inf,  # Starting stacks
        4,  # Number of players
    )
 
 Below are the pre-flop dealings and actions.
 
 .. code-block:: python
 
@@ -590,15 +602,16 @@
    state.show_or_muck_hole_cards('2s4c6d9h')  # Alice
    state.show_or_muck_hole_cards('3s5d7c8h')  # Carol
 
 Below are the final stacks.
 
 .. code-block:: python
 
-   print(state.stacks)  # [196, 220, 200, 184]
+   print(state.stacks)  # [inf, inf, inf, inf]
+   print(state.payoffs)  # [-4, 20, 0, -16]
 
 Testing and Validation
 ----------------------
 
 PokerKit has extensive test coverage, passes mypy static type checking with strict mode, and has been validated through extensive use in real-life scenarios.
 
 Contributing
```

### Comparing `pokerkit-0.5.0a1/README.rst` & `pokerkit-0.5.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,20 @@
 Multi-Runout in an All-In Situation
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Below shows the 4-runout hand between Phil Hellmuth and the Loose Cannon Ernest Wiggins.
 
 Link: https://youtu.be/cnjJv7x0HMY?si=4l05Ez7lQVczt8DI&t=638
 
+Note that the starting stacks for some players are set to be ``math.inf`` as they are not mentioned.
+
 .. code-block:: python
 
+   from math import inf
+
    from pokerkit import Automation, Mode, NoLimitTexasHoldem
 
    state = NoLimitTexasHoldem.create_state(
        # Automations
        (
            Automation.ANTE_POSTING,
            Automation.BET_COLLECTION,
@@ -48,15 +52,15 @@
            Automation.CHIPS_PUSHING,
            Automation.CHIPS_PULLING,
        ),
        False,  # Uniform antes?
        {-1: 600},  # Antes
        (200, 400, 800),  # Blinds or straddles
        400,  # Min-bet
-       (999999, 116400, 86900, 999999, 50000, 999999),  # Starting stacks
+       (inf, 116400, 86900, inf, 50000, inf),  # Starting stacks
        6,  # Number of players
        mode=Mode.CASH_GAME,
    )
 
 Below are the pre-flop dealings and actions.
 
 .. code-block:: python
@@ -135,25 +139,29 @@
    state.burn_card('??')
    state.deal_board('Kd')  # River
 
 Below are the final stacks.
 
 .. code-block:: python
 
-   print(state.stacks)  # [987399, 79400, 149700, 999999, 37400, 999399]
+   print(state.stacks)  # [inf, 79400, 149700, inf, 37400, inf]
 
 A Sample No-Limit Texas Hold'em Hand
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Below shows the first televised million-dollar pot between Tom Dwan and Phil Ivey.
 
 Link: https://youtu.be/GnxFohpljqM
 
+Note that the starting stack of Patrik Antonius is set to be ``math.inf`` as it is not mentioned.
+
 .. code-block:: python
 
+   from math import inf
+
    from pokerkit import Automation, NoLimitTexasHoldem
 
    state = NoLimitTexasHoldem.create_state(
        # Automations
        (
            Automation.ANTE_POSTING,
            Automation.BET_COLLECTION,
@@ -163,15 +171,15 @@
            Automation.CHIPS_PUSHING,
            Automation.CHIPS_PULLING,
        ),
        True,  # Uniform antes?
        500,  # Antes
        (1000, 2000),  # Blinds or straddles
        2000,  # Min-bet
-       (1125600, 2000000, 553500),  # Starting stacks
+       (1125600, inf, 553500),  # Starting stacks
        3,  # Number of players
    )
 
 Below are the pre-flop dealings and actions.
 
 .. code-block:: python
 
@@ -213,15 +221,15 @@
    state.burn_card('??')
    state.deal_board('Jh')
 
 Below are the final stacks.
 
 .. code-block:: python
 
-   print(state.stacks)  # [572100, 1997500, 1109500]
+   print(state.stacks)  # [572100, inf, 1109500]
 
 A Sample Short-Deck Hold'em Hand
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Below shows an all-in hand between Xuan and Phua.
 
 Link: https://youtu.be/QlgCcphLjaQ
@@ -463,16 +471,20 @@
 A Sample Badugi Hand
 ^^^^^^^^^^^^^^^^^^^^
 
 Below shows an example badugi hand from Wikipedia.
 
 Link: https://en.wikipedia.org/wiki/Badugi
 
+Note that the starting stacks are set to be ``math.inf`` as they are not mentioned.
+
 .. code-block:: python
 
+   from math import inf
+
    from pokerkit import Automation, FixedLimitBadugi
 
    state = FixedLimitBadugi.create_state(
        # Automations
        (
            Automation.ANTE_POSTING,
            Automation.BET_COLLECTION,
@@ -482,15 +494,15 @@
            Automation.CHIPS_PULLING,
        ),
        True,  # Uniform antes?
        0,  # Antes
        (1, 2),  # Blinds or straddles
        2,  # Small-bet
        4,  # Big-bet
-       200,  # Starting stacks
+       inf,  # Starting stacks
        4,  # Number of players
    )
 
 Below are the pre-flop dealings and actions.
 
 .. code-block:: python
 
@@ -558,15 +570,16 @@
    state.show_or_muck_hole_cards('2s4c6d9h')  # Alice
    state.show_or_muck_hole_cards('3s5d7c8h')  # Carol
 
 Below are the final stacks.
 
 .. code-block:: python
 
-   print(state.stacks)  # [196, 220, 200, 184]
+   print(state.stacks)  # [inf, inf, inf, inf]
+   print(state.payoffs)  # [-4, 20, 0, -16]
 
 Testing and Validation
 ----------------------
 
 PokerKit has extensive test coverage, passes mypy static type checking with strict mode, and has been validated through extensive use in real-life scenarios.
 
 Contributing
```

### Comparing `pokerkit-0.5.0a1/pokerkit/__init__.py` & `pokerkit-0.5.1/pokerkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a1/pokerkit/analysis.py` & `pokerkit-0.5.1/pokerkit/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     chain,
     combinations,
     permutations,
     product,
     repeat,
     starmap,
 )
+from math import sqrt
 from operator import eq
 from random import choices, sample
 from statistics import mean, stdev
 from typing import Any
 
 from pokerkit.hands import Hand
 from pokerkit.notation import HandHistory
@@ -411,15 +412,18 @@
     )
 
     return equities[-1]
 
 
 @dataclass
 class Statistics:
-    """The class for player statistics."""
+    """The class for player statistics.
+
+    :param payoffs: The payoffs of each hand.
+    """
 
     payoffs: list[int]
     """The payoffs."""
 
     @classmethod
     def merge(cls, *statistics: Statistics) -> Statistics:
         """Merge the statistics.
@@ -432,26 +436,25 @@
         for sub_statistics in statistics:
             payoffs.extend(sub_statistics.payoffs)
 
         return Statistics(payoffs=payoffs)
 
     @classmethod
     def from_hand_history(cls, *hhs: HandHistory) -> dict[str, Statistics]:
-        """Obtain statistics for each position and players (if any) for a
-        hand history or hand histories.
+        """Obtain statistics for each position and players (if any) for
+        a hand history or hand histories.
 
         :param hh: The hand history/histories to analyze.
         :return: The hand history statistics.
         """
         statistics = defaultdict[str, list[Statistics]](list)
 
         for hh in hhs:
-            end_state = tuple(hh)[-1]
-
             if hh.finishing_stacks is None:
+                end_state = tuple(hh)[-1]
                 finishing_stacks = end_state.stacks
             else:
                 finishing_stacks = hh.finishing_stacks
 
             players: Any
 
             if hh.players is None:
@@ -495,10 +498,18 @@
         """
         return mean(self.payoffs)
 
     @property
     def payoff_stdev(self) -> float:
         """Return the payoff standard deviation.
 
-        :return: The payoff stdev.
+        :return: The payoff standard deviation.
         """
         return stdev(self.payoffs)
+
+    @property
+    def payoff_stderr(self) -> float:
+        """Return the payoff standard error.
+
+        :return: The payoff standard error.
+        """
+        return self.payoff_stdev / sqrt(self.sample_count)
```

### Comparing `pokerkit-0.5.0a1/pokerkit/games.py` & `pokerkit-0.5.1/pokerkit/games.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """:mod:`pokerkit.games` implements various poker game definitions.
 
 The classes here allow users to "save" certain configurations to create
-poker states in a simple manner. This is crucial, as poker states require
-tons of parameters to be specified.
+poker states in a simple manner. This is crucial, as poker states
+require tons of parameters to be specified.
 """
 
 from __future__ import annotations
 
 from abc import ABC
 from collections.abc import Callable
 from typing import ClassVar
@@ -201,16 +201,16 @@
             starting_board_count=self.starting_board_count,
             divmod=self.divmod,
             rake=self.rake,
         )
 
     @property
     def button_status(self) -> bool:
-        """Return whether this game is a button game (i.e. has a rotating
-        button).
+        """Return whether this game is a button game (i.e. has a
+        rotating button).
 
         We deem that a variant is a button game if it has betting round
         whose opener is decided based on position (not up card/hand like
         in stud).
 
         >>> game = NoLimitTexasHoldem((), True, 0, (1, 2), 2)
         >>> game.button_status
@@ -643,14 +643,15 @@
         """Create a no-limit Texas hold'em game.
 
         Below shows the 4-runout hand between Phil Hellmuth and the
         Loose Cannon Ernest Wiggins.
 
         Link: https://youtu.be/cnjJv7x0HMY?si=4l05Ez7lQVczt8DI&t=638
 
+        >>> from math import inf
         >>> from pokerkit import Automation, Mode, NoLimitTexasHoldem
         >>> state = NoLimitTexasHoldem.create_state(
         ...     (
         ...         Automation.ANTE_POSTING,
         ...         Automation.BET_COLLECTION,
         ...         Automation.BLIND_OR_STRADDLE_POSTING,
         ...         Automation.HOLE_CARDS_SHOWING_OR_MUCKING,
@@ -658,15 +659,15 @@
         ...         Automation.CHIPS_PUSHING,
         ...         Automation.CHIPS_PULLING,
         ...     ),
         ...     False,
         ...     {-1: 600},
         ...     (200, 400, 800),
         ...     400,
-        ...     (999999, 116400, 86900, 999999, 50000, 999999),
+        ...     (inf, 116400, 86900, inf, 50000, inf),
         ...     6,
         ...     mode=Mode.CASH_GAME,
         ... )
 
         Below are the pre-flop dealings and actions.
 
         >>> state.deal_hole('JsTh')  # Tony G  # doctest: +ELLIPSIS
@@ -779,15 +780,15 @@
         CardBurning(commentary=None, card=??)
         >>> state.deal_board('Kd')  # River
         BoardDealing(commentary=None, cards=(Kd,))
 
         Below are the final stacks.
 
         >>> state.stacks
-        [987399, 79400, 149700, 999999, 37400, 999399]
+        [inf, 79400, 149700, inf, 37400, inf]
 
         Below shows the first televised million dollar pot between
         Tom Dwan and Phil Ivey.
 
         Link: https://youtu.be/GnxFohpljqM
 
         >>> state = NoLimitTexasHoldem.create_state(
@@ -800,15 +801,15 @@
         ...         Automation.CHIPS_PUSHING,
         ...         Automation.CHIPS_PULLING,
         ...     ),
         ...     True,
         ...     500,
         ...     (1000, 2000),
         ...     2000,
-        ...     (1125600, 2000000, 553500),
+        ...     (1125600, inf, 553500),
         ...     3,
         ... )
 
         Below shows the pre-flop dealings and actions.
 
         >>> state.deal_hole('Ac2d')  # Ivey  # doctest: +ELLIPSIS
         HoleDealing(commentary=None, player_index=0, cards=(Ac, 2d), statuse...
@@ -864,15 +865,15 @@
         CardBurning(commentary=None, card=??)
         >>> state.deal_board('Jh')
         BoardDealing(commentary=None, cards=(Jh,))
 
         Below shows the final stacks.
 
         >>> state.stacks
-        [572100, 1997500, 1109500]
+        [572100, inf, 1109500]
 
         :param automations: The automations.
         :param ante_trimming_status: The ante trimming status.
         :param raw_antes: The antes.
         :param raw_blinds_or_straddles: The blinds or straddles.
         :param min_bet: The min bet.
         :param raw_starting_stacks: The starting stacks.
@@ -1204,16 +1205,16 @@
             player_count: int,
             *,
             mode: Mode = Mode.TOURNAMENT,
             starting_board_count: int = 1,
             divmod: Callable[[int, int], tuple[int, int]] = divmod,
             rake: Callable[[int, State], tuple[int, int]] = rake,
     ) -> State:
-        """Create a fixed-limit Omaha hold'em high/low-split eight or better
-        low game.
+        """Create a fixed-limit Omaha hold'em high/low-split eight or
+        better low game.
 
         :param automations: The automations.
         :param ante_trimming_status: The ante trimming status.
         :param raw_antes: The "raw" antes.
         :param raw_blinds_or_straddles: The "raw" blinds or straddles.
         :param small_bet: The small bet.
         :param big_bet: The big bet.
@@ -1893,29 +1894,30 @@
     ) -> State:
         """Create a fixed-limit badugi game.
 
         Below shows an example badugi hand from Wikipedia.
 
         Link: https://en.wikipedia.org/wiki/Badugi
 
+        >>> from math import inf
         >>> state = FixedLimitBadugi.create_state(
         ...     (
         ...         Automation.ANTE_POSTING,
         ...         Automation.BET_COLLECTION,
         ...         Automation.BLIND_OR_STRADDLE_POSTING,
         ...         Automation.HAND_KILLING,
         ...         Automation.CHIPS_PUSHING,
         ...         Automation.CHIPS_PULLING,
         ...     ),
         ...     True,
         ...     0,
         ...     (1, 2),
         ...     2,
         ...     4,
-        ...     200,
+        ...     inf,
         ...     4,
         ... )
 
         Below shows the pre-flop dealings and actions.
 
         >>> state.deal_hole('????????')  # Bob  # doctest: +ELLIPSIS
         HoleDealing(commentary=None, player_index=0, cards=(??, ??, ??, ??),...
@@ -2015,15 +2017,17 @@
         ...     '3s5d7c8h',
         ... )  # Carol  # doctest: +ELLIPSIS
         HoleCardsShowingOrMucking(commentary=None, player_index=1, hole_card...
 
         Below show the final stacks.
 
         >>> state.stacks
-        [196, 220, 200, 184]
+        [inf, inf, inf, inf]
+        >>> state.payoffs
+        [-4, 20, 0, -16]
 
         :param automations: The automations.
         :param ante_trimming_status: The ante trimming status.
         :param raw_antes: The "raw" antes.
         :param raw_blinds_or_straddles: The "raw" blinds or straddles.
         :param small_bet: The small bet.
         :param big_bet: The big bet.
```

### Comparing `pokerkit-0.5.0a1/pokerkit/hands.py` & `pokerkit-0.5.1/pokerkit/hands.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,17 @@
     TypeError: '<' not supported between instances of 'BadugiHand' and 'int'
 
     The hands are hashable.
 
     >>> h0 = ShortDeckHoldemHand('6s7s8s9sTs')
     >>> h1 = ShortDeckHoldemHand('7c8c9cTcJc')
     >>> hands = {h0, h1}
+
+    :param cards: The cards that form the hand.
+    :raises ValueError: If the cards form an invalid hand.
     """
 
     lookup: ClassVar[Lookup]
     """The hand lookup."""
     low: ClassVar[bool]
     """The low status."""
```

### Comparing `pokerkit-0.5.0a1/pokerkit/lookups.py` & `pokerkit-0.5.1/pokerkit/lookups.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,17 @@
     False
     >>> e1 == e2
     True
     >>> e0.index
     0
     >>> e0.label
     <Label.HIGH_CARD: 'High card'>
+
+    :param index: The index of the entry.
+    :param label: The label of the hand.
     """
 
     index: int
     """The index of the corresponding hand."""
     label: Label = field(compare=False)
     """The label of the corresponding hand."""
```

### Comparing `pokerkit-0.5.0a1/pokerkit/notation.py` & `pokerkit-0.5.1/pokerkit/notation.py`

 * *Files 26% similar despite different names*

```diff
@@ -41,14 +41,107 @@
     PotLimitOmahaHoldem,
 )
 from pokerkit.utilities import Card, divmod, parse_value, rake
 
 
 @dataclass
 class HandHistory(Iterable[State]):
+    """The class for hand histories.
+
+    :param variant: The variant name. For more information, please refer
+                    to :attr:`pokerkit.notation.HandHistory.variant`.
+    :param ante_trimming_status: The ante trimming status. For more
+                                 information, please refer to
+                                 :attr:`pokerkit.notation.HandHistory.ante_trimming_status`.
+    :param antes: The antes. For more information, please refer to
+                  :attr:`pokerkit.notation.HandHistory.antes`.
+    :param blinds_or_straddles: The blinds or straddles. For more
+                                information, please refer to
+                                :attr:`pokerkit.notation.HandHistory.blinds_or_straddles`.
+    :param bring_in: The bring-in. For more information, please refer to
+                     :attr:`pokerkit.notation.HandHistory.bring_in`.
+    :param small_bet: The small bet. For more information, please refer
+                      to
+                      :attr:`pokerkit.notation.HandHistory.small_bet`.
+    :param big_bet: The big bet. For more information, please refer to
+                    :attr:`pokerkit.notation.HandHistory.big_bet`.
+    :param min_bet: The minimum bet. For more information, please refer
+                    to :attr:`pokerkit.notation.HandHistory.min_bet`.
+    :param starting_stacks: The starting stacks. For more information,
+                            please refer to
+                            :attr:`pokerkit.notation.HandHistory.starting_stacks`.
+    :param actions: The actions. For more information, please refer to
+                    :attr:`pokerkit.notation.HandHistory.actions`.
+    :param author: The author. For more information, please refer to
+                   :attr:`pokerkit.notation.HandHistory.author`.
+    :param event: The event. For more information, please refer to
+                  :attr:`pokerkit.notation.HandHistory.event`.
+    :param url: The url. For more information, please refer to
+                :attr:`pokerkit.notation.HandHistory.url`.
+    :param address: The address. For more information, please refer to
+                    :attr:`pokerkit.notation.HandHistory.address`.
+    :param city: The city. For more information, please refer to
+                 :attr:`pokerkit.notation.HandHistory.city`.
+    :param region: The region. For more information, please refer to
+                   :attr:`pokerkit.notation.HandHistory.region`.
+    :param postal_code: The postal code. For more information, please
+                        refer to
+                        :attr:`pokerkit.notation.HandHistory.postal_code`.
+    :param country: The country. For more information, please refer to
+                    :attr:`pokerkit.notation.HandHistory.country`.
+    :param time: The time. For more information, please refer to
+                 :attr:`pokerkit.notation.HandHistory.time`.
+    :param time_zone: The time zone. For more information, please refer
+                      to
+                      :attr:`pokerkit.notation.HandHistory.time_zone`.
+    :param day: The day. For more information, please refer to
+                :attr:`pokerkit.notation.HandHistory.day`.
+    :param month: The month. For more information, please refer to
+                  :attr:`pokerkit.notation.HandHistory.month`.
+    :param year: The year. For more information, please refer to
+                 :attr:`pokerkit.notation.HandHistory.year`.
+    :param hand: The hand number. For more information, please refer to
+                 :attr:`pokerkit.notation.HandHistory.hand`.
+    :param level: The level. For more information, please refer to
+                  :attr:`pokerkit.notation.HandHistory.level`.
+    :param seats: The seat numbers. For more information, please refer
+                  to :attr:`pokerkit.notation.HandHistory.seats`.
+    :param seat_count: The number of seats. For more information, please
+                       refer to
+                       :attr:`pokerkit.notation.HandHistory.seat_count`.
+    :param table: The table number. For more information, please refer
+                  to :attr:`pokerkit.notation.HandHistory.table`.
+    :param players: The player names. For more information, please refer
+                    to :attr:`pokerkit.notation.HandHistory.players`.
+    :param finishing_stacks: The finishing stacks. For more information,
+                             please refer to
+                             :attr:`pokerkit.notation.HandHistory.finishing_stacks`.
+    :param currency: The currency. For more information, please refer to
+                     :attr:`pokerkit.notation.HandHistory.currency`.
+    :param time_limit: The time limit. For more information, please
+                       refer to
+                       :attr:`pokerkit.notation.HandHistory.time_limit`.
+    :param time_banks: The time banks. For more information, please
+                       refer to
+                       :attr:`pokerkit.notation.HandHistory.time_banks`.
+    :param user_defined_fields: The user-defined fields. For more
+                                information, please refer to
+                                :attr:`pokerkit.notation.HandHistory.user_defined_fields`.
+    :param automations: The automations. For more information, please
+                        refer to
+                        :attr:`pokerkit.notation.HandHistory.automations`.
+    :param divmod: The divmod function. For more information, please
+                   refer to :attr:`pokerkit.notation.HandHistory.divmod`.
+    :param rake: The rake function. For more information, please refer
+                 to :attr:`pokerkit.notation.HandHistory.rake`.
+    :param parse_value: The value parsing function. For more
+                        information, please refer to
+                        :attr:`pokerkit.notation.HandHistory.parse_value`.
+    """
+
     game_types: ClassVar[dict[str, type[Poker]]] = {
         'FT': FixedLimitTexasHoldem,
         'NT': NoLimitTexasHoldem,
         'NS': NoLimitShortDeckHoldem,
         'PO': PotLimitOmahaHoldem,
         'FO/8': FixedLimitOmahaHoldemHighLowSplitEightOrBetter,
         'F7S': FixedLimitSevenCardStud,
@@ -667,18 +760,15 @@
                     action = 'c'
                     actions += action
                 elif isinstance(operation, CompletionBettingOrRaisingTo):
                     match self.variant:
                         case 'FT':
                             action = 'r'
                         case 'NT':
-                            amount = (
-                                state.starting_stacks[operation.player_index]
-                                - state.stacks[operation.player_index]
-                            )
+                            amount = -state.payoffs[operation.player_index]
                             action = f'r{amount}'
                         case _:
                             raise AssertionError
 
                     actions += action
 
                 if (
@@ -767,18 +857,15 @@
                 index += 1
 
                 if isinstance(operation, Folding):
                     actions += 'f'
                 elif isinstance(operation, CheckingOrCalling):
                     actions += 'c'
                 elif isinstance(operation, CompletionBettingOrRaisingTo):
-                    amount = (
-                        state.starting_stacks[operation.player_index]
-                        - state.stacks[operation.player_index]
-                    )
+                    amount = -state.payoffs[operation.player_index]
                     actions += f'r{amount}'
                 elif isinstance(operation, HoleDealing):
                     for i, card in enumerate(operation.cards):
                         if not card.unknown_status:
                             raw_hole_cards[operation.player_index][i] = repr(
                                 card,
                             )
```

### Comparing `pokerkit-0.5.0a1/pokerkit/state.py` & `pokerkit-0.5.1/pokerkit/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,38 +191,80 @@
     ...     2,
     ...     None,
     ... )
     >>> street.card_burning_status
     False
     >>> street.hole_dealing_statuses
     (False, False)
+
+    :param card_burning_status: Whether to burn card (``True`` if this
+                                is so). For more information, please
+                                refer to
+                                :attr:`pokerkit.state.Street.card_burning_status`.
+    :param hole_dealing_statuses: The statuses of dealt hole cards. For
+                                  more information, please refer to
+                                  :attr:`pokerkit.state.Street.hole_dealing_statuses`.
+    :param board_dealing_count: The number of dealt board cards (``0``
+                                if none). For more information, please
+                                refer to
+                                :attr:`pokerkit.state.Street.board_dealing_count`.
+    :param draw_status: Whether to draw cards prior to betting (``True``
+                        if this is so). For more information, please
+                        refer to
+                        :attr:`pokerkit.state.Street.draw_status`.
+    :param opening: The opening. For more information, please refer to
+                    :attr:`pokerkit.state.Street.opening`.
+    :param min_completion_betting_or_raising_amount: The minimum
+                                                     completion,
+                                                     betting, or raising
+                                                     amount. For more
+                                                     information, please
+                                                     refer to
+                                                     :attr:`pokerkit.state.Street.min_completion_betting_or_raising_amount`.
+    :param max_completion_betting_or_raising_count: The maximum number
+                                                    of completions,
+                                                    bettings, or
+                                                    raisings. For more
+                                                    information, please
+                                                    refer to
+                                                    :attr:`pokerkit.state.Street.max_completion_betting_or_raising_count`.
+    :raises ValueError: If the arguments are invalid.
     """
 
     card_burning_status: bool
     """Whether to burn card (``True`` if this is so)."""
     hole_dealing_statuses: tuple[bool, ...]
     """The statuses of dealt hole cards.
 
     The length of this ``tuple`` denotes the number of hole cards dealt
     in the current street. Each item denotes whether to deal a card as
     an up card (``True``) or a down card (``False``).
+
+    If there is no board dealing and no drawing, this value should be
+    non-empty. If drawing, this should be left empty.
     """
     board_dealing_count: int
     """The number of dealt board cards (``0`` if none).
 
     This number of cards is dealt for each board (for multi-board
     games).
+
+    If there is no hole dealing and no drawing, this value should be
+    non-empty.
     """
     draw_status: bool
     """Whether to draw cards prior to betting (``True`` if this is so).
 
     This flag is mutually exclusive with the enabling of hole dealings.
     In other words, if this is ``True``,
     :attr:`pokerkit.state.Street.hole_dealing_statuses` should be
     ``()``.
+
+    If there is no hole dealing and no board dealing, this value should
+    be non-empty.
     """
     opening: Opening
     """The opening.
 
     It decides who acts first for each betting round.
     """
     min_completion_betting_or_raising_amount: int
@@ -370,23 +412,40 @@
     """The tournament poker state type."""
     CASH_GAME = 'Cash-game'
     """The cash-game poker state type."""
 
 
 @dataclass(frozen=True)
 class Pot:
-    """The class for pots."""
+    """The class for pots.
+
+
+    :param raked_amount: The raked amount. For more details, please
+                         refer to
+                         :attr:`pokerkit.state.Pot.raked_amount`.
+    :param unraked_amount: The unraked amount. For more details, please
+                           refer to
+                           :attr:`pokerkit.state.Pot.unraked_amount`.
+    :param player_indices: The player indices. For more details, please
+                           refer to
+                           :attr:`pokerkit.state.Pot.player_indices`.
+    :raises ValueError: If the arguments are invalid.
+    """
 
     raked_amount: int
     """The raked amount (from the original amount
     :attr:`pokerkit.state.Pot`).
+
+    This value must be non-negative.
     """
     unraked_amount: int
     """The unraked amount (remaining from the original amount
     :attr:`pokerkit.state.Pot`).
+
+    This vealue must be non-negative.
     """
     player_indices: tuple[int, ...]
     """The player indices of those who are eligible to win.
 
     This means A: they contributed to this pot and B: they are still
     active (in the hand).
     """
@@ -763,14 +822,54 @@
     >>> state.pull_chips(1)
     ChipsPulling(commentary=None, player_index=1, amount=3)
 
     The game has terminated.
 
     >>> state.status
     False
+
+    :param automations: The automations. For more details, please refer
+                        to :attr:`pokerkit.state.State.automations`.
+    :param deck: The deck. For more details, please refer to
+                 :attr:`pokerkit.state.State.deck`.
+    :param hand_types: The hand types. For more details, please refer to
+                       :attr:`pokerkit.state.State.hand_types`.
+    :param streets: The streets. For more details, please refer to
+                    :attr:`pokerkit.state.State.streets`.
+    :param betting_structure: The betting structure. For more details,
+                              please refer to
+                              :attr:`pokerkit.state.State.betting_structure`.
+    :param ante_trimming_status: The ante trimming status. For more
+                                 details, please refer to
+                                 :attr:`pokerkit.state.State.ante_trimming_status`.
+    :param raw_antes: The "raw" antes. For more details, please refer to
+                      :attr:`pokerkit.state.State.raw_antes`.
+    :param raw_blinds_or_straddles: The "raw" blinds/straddles. For more
+                                    details, please refer to
+                                    :attr:`pokerkit.state.State.raw_blinds_or_straddles`.
+    :param bring_in: The bring-in. For more details, please refer to
+                     :attr:`pokerkit.state.State.bring_in`.
+    :param raw_starting_stacks: The "raw" starting stacks. For more
+                                details, please refer to
+                                :attr:`pokerkit.state.State.raw_starting_stacks`.
+    :param player_count: The number of players. For more details, please
+                         refer to
+                         :attr:`pokerkit.state.State.player_count`.
+    :param mode: The mode. Defaults to tournament mode. For more
+                 details, please refer to
+                 :attr:`pokerkit.state.State.mode`.
+    :param starting_board_count: The number of boards at the start of
+                                 the game. For more details, please
+                                 refer to
+                                 :attr:`pokerkit.state.State.starting_board_count`.
+    :param divmod: The divmod function. For more details, please refer
+                   to :attr:`pokerkit.state.State.divmod`.
+    :param rake: The rake function. For more details, please refer to
+                 :attr:`pokerkit.state.State.rake`.
+    :raises ValueError: If the arguments are invalid.
     """
 
     __low_hand_opening_lookup = _LowHandOpeningLookup()
     __high_hand_opening_lookup = _HighHandOpeningLookup()
     automations: tuple[Automation, ...]
     """The automations.
 
@@ -793,14 +892,17 @@
     considered, through the use of multiple hand types.
     """
     streets: tuple[Street, ...]
     """The streets.
 
     Each street contains information about the corresponding betting
     round and corresponding dealing/draw stage before it occurs.
+
+    This attribute must be non-empty and its first item must be of
+    hole-dealing.
     """
     betting_structure: BettingStructure
     """The betting structure.
 
     This class attribute determines the betting limits of a particular
     game (e.g. no-limit, pot-limit, or fixed-limit).
     """
@@ -820,38 +922,57 @@
     can be supplied in many forms and will be "parsed" or "evaluated"
     further to convert them into a more ideal form.
 
     For instance, ``0`` will be interpreted as no ante for all players.
     Another value will be interpreted as that value as the antes for
     all. ``[0, 2]`` and ``{1: 2} will be considered as the big blind
     ante whereas ``{-1: 2}`` will be considered as the button ante.
+
+    All of its ante values must be non-negative.
     """
     raw_blinds_or_straddles: InitVar[ValuesLike]
     """The "raw" blinds or straddles.
 
     Just like for the antes, the blinds/straddles are also "interpreted"
     by PokerKit in the same fashion.
+
+    All of its blind/straddle values must be non-negative.
+
+    If the bring-in is non-zero, the all blind/straddle values must be
+    zero. If any of the bring-in is zero, there must be at least one
+    positive blind/straddle value.
     """
     bring_in: int
     """The bring-in.
 
     Some poker games do not have the bring-in, in which case ``0``
     should be its value.
+
+    This value must be non-negative. If all blind/straddle values are
+    zero, the bring-in must be positive. If any of the blind/straddle
+    values are non-zero, the bring-in must be zero.
+
+    It must be less than the min-bet.
     """
     raw_starting_stacks: InitVar[ValuesLike]
     """The "raw" starting stacks.
 
     Similar to "raw" antes and "raw" blinds/straddles, the starting
     stacks can be represented in different ways which PokerKit
     interprets when creating the games. Not all representations
     explicitly express the number of players and therefore this value is
     accepted as a separate parameter ``player_count``.
+
+    All items must be positive.
     """
     player_count: int
-    """The number of players."""
+    """The number of players.
+
+    This value must be at least ``2``.
+    """
     _: KW_ONLY
     mode: Mode = Mode.TOURNAMENT
     """The mode. Defaults to tournament mode.
 
     There are two modes available to be set: the tournament and
     cash-game mode. Tournaments use a stricter rule-set than typical
     cash-games. For more details, please consult
@@ -863,14 +984,16 @@
     For most poker games, it should be ``1``. Of course, for double
     board games, it should be ``2``. Triple/Quadruple/etc. board games
     are almost unheard of. Therefore, this value should mostly be ``1``
     or sometimes ``2``.
 
     The actual number of boards may change depending on the number of
     runouts (during all-ins).
+
+    This value must be positive.
     """
     divmod: Callable[[int, int], tuple[int, int]] = divmod
     """The divmod function. Defaults to PokerKit's that detects integral
     or real values automatically.
 
     This is used to denote how pots are divided up (for multiple boards,
     multiple winners, multiple hand types, etc.).
@@ -933,14 +1056,22 @@
     If the corresponding item is ``True`` one can say the player at that
     index is still "in the hand".
     """
     bets: list[int] = field(default_factory=list, init=False)
     """The player bets."""
     stacks: list[int] = field(default_factory=list, init=False)
     """The player stacks."""
+    payoffs: list[int] = field(default_factory=list, init=False)
+    """The player payoffs.
+
+    Note that a ``payoff = stack - starting_stack`` for each player.
+
+    Negated versions of these values can be thought of as contributions
+    to the hand by the individual players.
+    """
     hole_cards: list[list[Card]] = field(default_factory=list, init=False)
     """The player hole cards.
 
     In PokerKit, the concept of hole cards is slightly warped as it
     includes both up and down cards.
     """
     hole_card_statuses: list[list[bool]] = field(
@@ -1072,14 +1203,15 @@
 
         shuffle(self.deck_cards)
 
         for i in self.player_indices:
             self.statuses.append(True)
             self.bets.append(0)
             self.stacks.append(self.starting_stacks[i])
+            self.payoffs.append(0)
             self.hole_cards.append([])
             self.hole_card_statuses.append([])
 
         for _ in self.street_indices:
             self.discarded_cards.append([])
 
         self._setup_ante_posting()
@@ -2361,18 +2493,18 @@
         >>> tuple(state.pot_amounts)  # doctest: +ELLIPSIS
         ()
 
         Pre-flop.
 
         >>> state.complete_bet_or_raise_to(200)  # doctest: +ELLIPSIS
         CompletionBettingOrRaisingTo(commentary=None, player_index=2, amount...
-        >>> state.complete_bet_or_raise_to(1000)
+        >>> state.complete_bet_or_raise_to(1000)  # doctest: +ELLIPSIS
         Traceback (most recent call last):
             ...
-        ValueError: There is no reason to complete, bet, or raise.
+        ValueError: There is no reason to complete, bet, or raise since ever...
         >>> state.check_or_call()
         CheckingOrCalling(commentary=None, player_index=3, amount=200)
         >>> state.check_or_call()
         CheckingOrCalling(commentary=None, player_index=4, amount=200)
         >>> state.check_or_call()
         CheckingOrCalling(commentary=None, player_index=5, amount=100)
         >>> state.check_or_call()
@@ -2615,18 +2747,18 @@
         >>> tuple(state.pots)  # doctest: +ELLIPSIS
         ()
 
         Pre-flop.
 
         >>> state.complete_bet_or_raise_to(200)  # doctest: +ELLIPSIS
         CompletionBettingOrRaisingTo(commentary=None, player_index=2, amount...
-        >>> state.complete_bet_or_raise_to(1000)
+        >>> state.complete_bet_or_raise_to(1000)  # doctest: +ELLIPSIS
         Traceback (most recent call last):
             ...
-        ValueError: There is no reason to complete, bet, or raise.
+        ValueError: There is no reason to complete, bet, or raise since ever...
         >>> state.check_or_call()
         CheckingOrCalling(commentary=None, player_index=3, amount=200)
         >>> state.check_or_call()
         CheckingOrCalling(commentary=None, player_index=4, amount=200)
         >>> state.check_or_call()
         CheckingOrCalling(commentary=None, player_index=5, amount=100)
         >>> state.check_or_call()
@@ -2670,26 +2802,26 @@
 
         :return: The list of main and side pots (if any).
         """
         if self._pots is not None:
             yield from self._pots
 
             return
-        elif sum(self.stacks) + sum(self.bets) == sum(self.starting_stacks):
+        elif sum(self.payoffs) == -sum(self.bets):
             return
 
-        contributions = list(self.starting_stacks)
-        pending_contributions = list(self.starting_stacks)
+        contributions = []
+        pending_contributions = []
         amount = 0
 
         for i in self.player_indices:
-            assert self.stacks[i] <= self.starting_stacks[i]
+            assert self.payoffs[i] <= 0
 
-            contributions[i] -= self.bets[i] + self.stacks[i]
-            pending_contributions[i] -= self.stacks[i]
+            contributions.append(-self.payoffs[i] - self.bets[i])
+            pending_contributions.append(-self.payoffs[i])
 
         if not self.ante_trimming_status:
             amount = 0
 
             for i in self.player_indices:
                 ante = self.get_effective_ante(i)
                 amount += ante
@@ -2938,14 +3070,15 @@
         assert self.ante_posting_statuses[player_index]
         assert not self.bets[player_index]
         assert 0 < amount <= self.stacks[player_index]
 
         self.ante_posting_statuses[player_index] = False
         self.bets[player_index] = amount
         self.stacks[player_index] -= amount
+        self.payoffs[player_index] -= amount
 
         operation = AntePosting(player_index, amount, commentary=commentary)
 
         self._update_ante_posting(operation)
 
         return operation
 
@@ -3074,15 +3207,17 @@
         if self.street is not None or self.ante_trimming_status:
             bet_cutoff = sorted(self.bets)[-2]
 
             for i in player_indices:
                 if self.bets[i] > bet_cutoff:
                     assert self.statuses[i]
 
-                    self.stacks[i] += self.bets[i] - bet_cutoff
+                    overbet = self.bets[i] - bet_cutoff
+                    self.stacks[i] += overbet
+                    self.payoffs[i] += overbet
                     bets[i] = bet_cutoff
 
         for i in player_indices:
             self.bets[i] = 0
 
         operation = BetCollection(tuple(bets), commentary=commentary)
 
@@ -3297,14 +3432,15 @@
         assert self.blind_or_straddle_posting_statuses[player_index]
         assert not self.bets[player_index]
         assert 0 < amount <= self.stacks[player_index]
 
         self.blind_or_straddle_posting_statuses[player_index] = False
         self.bets[player_index] = amount
         self.stacks[player_index] -= amount
+        self.payoffs[player_index] -= amount
 
         operation = BlindOrStraddlePosting(
             player_index,
             amount,
             commentary=commentary,
         )
 
@@ -4353,16 +4489,17 @@
 
         amount = self.checking_or_calling_amount
         player_index = self._pop_actor_index()
 
         assert self.stacks[player_index]
         assert amount is not None
 
-        self.stacks[player_index] -= amount
         self.bets[player_index] += amount
+        self.stacks[player_index] -= amount
+        self.payoffs[player_index] -= amount
 
         operation = CheckingOrCalling(
             player_index,
             amount,
             commentary=commentary,
         )
 
@@ -4440,16 +4577,17 @@
         assert self.stacks[player_index]
         assert amount is not None
         assert not any(self.bets)
         assert self.bring_in
         assert self.completion_status
         assert self.actor_indices
 
-        self.stacks[player_index] -= amount
         self.bets[player_index] += amount
+        self.stacks[player_index] -= amount
+        self.payoffs[player_index] -= amount
         self.bring_in_status = False
 
         operation = BringInPosting(player_index, amount, commentary=commentary)
 
         self._update_betting(operation)
 
         return operation
@@ -4564,25 +4702,36 @@
 
         assert player_index is not None
 
         if (
                 self.stacks[player_index]
                 <= max(self.bets) - self.bets[player_index]
         ):
-            raise ValueError('There are not enough chips in stack.')
+            raise ValueError(
+                (
+                    'The player is already covered by a previous bet/raise.'
+                    ' You most likely want to just call here with'
+                    ' ``pokerkit.state.State.check_or_call()``.'
+                ),
+            )
 
         for i in self.player_indices:
             if (
                     i != player_index
                     and self.statuses[i]
                     and self.stacks[i] + self.bets[i] > max(self.bets)
             ):
                 break
         else:
-            raise ValueError('There is no reason to complete, bet, or raise.')
+            raise ValueError(
+                (
+                    'There is no reason to complete, bet, or raise since every'
+                    ' other player has either folded or gone all-in.'
+                ),
+            )
 
     def verify_completion_betting_or_raising_to(
             self,
             amount: int | None = None,
     ) -> int:
         """Verify the completion, betting, or raising to.
 
@@ -4756,16 +4905,18 @@
         :raises ValueError: If the completion, betting, or raising
                             cannot be done.
         """
         amount = self.verify_completion_betting_or_raising_to(amount)
         player_index = self._pop_actor_index()
 
         completion_betting_or_raising_amount = amount - max(self.bets)
-        self.stacks[player_index] -= amount - self.bets[player_index]
+        delta = amount - self.bets[player_index]
         self.bets[player_index] = amount
+        self.stacks[player_index] -= delta
+        self.payoffs[player_index] -= delta
         self.bring_in_status = False
         self.completion_status = False
         self.actor_indices = deque(self.player_indices)
         self.opener_index = player_index
         self.completion_betting_or_raising_amount = max(
             self.completion_betting_or_raising_amount,
             completion_betting_or_raising_amount,
@@ -5981,14 +6132,15 @@
         :return: The chips pulling.
         :raises ValueError: If the chips pulling cannot be done.
         """
         player_index = self.verify_chips_pulling(player_index)
         amount = self.bets[player_index]
 
         self.stacks[player_index] += amount
+        self.payoffs[player_index] += amount
         self.bets[player_index] = 0
         self.chips_pulling_statuses[player_index] = False
 
         operation = ChipsPulling(player_index, amount, commentary=commentary)
 
         self._update_chips_pulling(operation)
```

### Comparing `pokerkit-0.5.0a1/pokerkit/tests/test_analysis.py` & `pokerkit-0.5.1/pokerkit/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a1/pokerkit/tests/test_games.py` & `pokerkit-0.5.1/pokerkit/tests/test_games.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a1/pokerkit/tests/test_lookups.py` & `pokerkit-0.5.1/pokerkit/tests/test_lookups.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a1/pokerkit/tests/test_notation.py` & `pokerkit-0.5.1/pokerkit/tests/test_notation.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a1/pokerkit/tests/test_papers.py` & `pokerkit-0.5.1/pokerkit/tests/test_papers.py`

 * *Files 4% similar despite different names*

```diff
@@ -709,17 +709,23 @@
         self.assertEqual(new_state.stacks, [196, 220, 200, 184])
         self.assertEqual(new_state.operations, state.operations)
         self.assertEqual(s, hh.dumps())
 
 
 class READMETestCase(TestCase):
     def test_hellmuth_wiggins(self) -> None:
-        # The 4-runout hand between Phil Hellmuth and the Loose Cannon Ernest
-        # Wiggins.
+        # The 4-runout hand between Phil Hellmuth and the Loose Cannon
+        # Ernest Wiggins.
+        #
         # Link: https://youtu.be/cnjJv7x0HMY?si=4l05Ez7lQVczt8DI&t=638
+        #
+        # Note that the starting stacks for some players are set to be
+        # ``math.inf`` as they are not mentioned.
+
+        from math import inf
 
         from pokerkit import Automation, Mode, NoLimitTexasHoldem
 
         # Set up the game.
 
         state = NoLimitTexasHoldem.create_state(
             # Automations
@@ -732,15 +738,15 @@
                 Automation.CHIPS_PUSHING,
                 Automation.CHIPS_PULLING,
             ),
             False,  # Uniform antes?
             {-1: 600},  # Antes
             (200, 400, 800),  # Blinds or straddles
             400,  # Min-bet
-            (999999, 116400, 86900, 999999, 50000, 999999),  # Starting stacks
+            (inf, 116400, 86900, inf, 50000, inf),  # type: ignore[arg-type]  # Starting stacks  # noqa: E501
             6,  # Number of players
             mode=Mode.CASH_GAME,
         )
 
         # Below are the pre-flop dealings and actions.
 
         state.deal_hole('JsTh')  # Tony G
@@ -803,45 +809,51 @@
         state.burn_card('??')
         state.deal_board('Qc')  # Turn
         state.burn_card('??')
         state.deal_board('Kd')  # River
 
         # Below are the final stacks.
 
-        # print(state.stacks)  # [987399, 79400, 149700, 999999, 37400, 999399]
+        # print(state.stacks)  # [inf, 79400, 149700, inf, 37400, inf]
 
         self.assertEqual(
             state.stacks,
-            [987399, 79400, 149700, 999999, 37400, 999399],
+            [inf, 79400, 149700, inf, 37400, inf],
         )
 
     def test_dwan_ivey(self) -> None:
-        # Below shows the first televised million-dollar pot between Tom Dwan
-        # and Phil Ivey.
+        # Below shows the first televised million-dollar pot between Tom
+        # Dwan and Phil Ivey.
         #
         # Link: https://youtu.be/GnxFohpljqM
+        #
+        # Note that the starting stack of Patrik Antonius is set to be
+        # ``math.inf`` as it is not mentioned.
+
+        from math import inf
 
         from pokerkit import Automation, NoLimitTexasHoldem
 
         state = NoLimitTexasHoldem.create_state(
+            # Automations
             (
                 Automation.ANTE_POSTING,
                 Automation.BET_COLLECTION,
                 Automation.BLIND_OR_STRADDLE_POSTING,
                 Automation.HOLE_CARDS_SHOWING_OR_MUCKING,
                 Automation.HAND_KILLING,
                 Automation.CHIPS_PUSHING,
                 Automation.CHIPS_PULLING,
             ),
-            True,
-            500,
-            (1000, 2000),
-            2000,
-            (1125600, 2000000, 553500),
-            3,
+            True,  # Uniform antes?
+            500,  # Antes
+            (1000, 2000),  # Blinds or straddles
+            2000,  # Min-bet
+            (1125600, inf, 553500),  # type: ignore[arg-type]  # Starting stacks  # noqa: E501
+            3,  # Number of players
         )
 
         # Below are the pre-flop dealings and actions.
 
         state.deal_hole('Ac2d')  # Ivey
         state.deal_hole('????')  # Antonius
         state.deal_hole('7h6h')  # Dwan
@@ -872,41 +884,42 @@
         # Below is the river dealing.
 
         state.burn_card('??')
         state.deal_board('Jh')
 
         # Below are the final stacks.
 
-        # print(state.stacks)  # [572100, 1997500, 1109500]
+        # print(state.stacks)  # [572100, inf, 1109500]
 
-        self.assertEqual(state.stacks, [572100, 1997500, 1109500])
+        self.assertEqual(state.stacks, [572100, inf, 1109500])
 
     def test_phua_xuan(self) -> None:
         # Below shows an all-in hand between Xuan and Phua.
         #
         # Link: https://youtu.be/QlgCcphLjaQ
 
         from pokerkit import Automation, NoLimitShortDeckHoldem
 
         state = NoLimitShortDeckHoldem.create_state(
+            # Automations
             (
                 Automation.ANTE_POSTING,
                 Automation.BET_COLLECTION,
                 Automation.BLIND_OR_STRADDLE_POSTING,
                 Automation.HOLE_CARDS_SHOWING_OR_MUCKING,
                 Automation.HAND_KILLING,
                 Automation.CHIPS_PUSHING,
                 Automation.CHIPS_PULLING,
             ),
-            True,
-            3000,
-            {-1: 3000},
-            3000,
-            (495000, 232000, 362000, 403000, 301000, 204000),
-            6,
+            True,  # Uniform antes?
+            3000,  # Antes
+            {-1: 3000},  # Blinds or straddles
+            3000,  # Min-bet
+            (495000, 232000, 362000, 403000, 301000, 204000),  # Starting stacks  # noqa: E501
+            6,  # Number of players
         )
 
         # Below are the pre-flop dealings and actions.
 
         state.deal_hole('Th8h')  # Badziakouski
         state.deal_hole('QsJd')  # Zhong
         state.deal_hole('QhQd')  # Xuan
@@ -945,37 +958,38 @@
 
         self.assertEqual(
             state.stacks,
             [489000, 226000, 684000, 400000, 0, 198000],
         )
 
     def test_antonius_blom(self) -> None:
-        # Below shows the largest online poker pot ever played between Patrik
-        # Antonius and Viktor Blom.
+        # Below shows the largest online poker pot ever played between
+        # Patrik Antonius and Viktor Blom.
         #
         # Link: https://youtu.be/UMBm66Id2AA
 
         from pokerkit import Automation, PotLimitOmahaHoldem
 
         state = PotLimitOmahaHoldem.create_state(
+            # Automations
             (
                 Automation.ANTE_POSTING,
                 Automation.BET_COLLECTION,
                 Automation.BLIND_OR_STRADDLE_POSTING,
                 Automation.HOLE_CARDS_SHOWING_OR_MUCKING,
                 Automation.HAND_KILLING,
                 Automation.CHIPS_PUSHING,
                 Automation.CHIPS_PULLING,
             ),
-            True,
-            0,
-            (500, 1000),
-            2000,
-            (1259450.25, 678473.5),  # type: ignore[arg-type]
-            2,
+            True,  # Uniform antes?
+            0,  # Antes
+            (500, 1000),  # Blinds or straddles
+            1000,  # Min-bet
+            (1259450.25, 678473.5),  # type: ignore[arg-type]  # Starting stacks  # noqa: E501
+            2,  # Number of players
         )
 
         # Below are the pre-flop dealings and actions.
 
         state.deal_hole('Ah3sKsKh')  # Antonius
         state.deal_hole('6d9s7d8h')  # Blom
 
@@ -1018,30 +1032,31 @@
 
         from pokerkit import (
             Automation,
             FixedLimitDeuceToSevenLowballTripleDraw,
         )
 
         state = FixedLimitDeuceToSevenLowballTripleDraw.create_state(
+            # Automations
             (
                 Automation.ANTE_POSTING,
                 Automation.BET_COLLECTION,
                 Automation.BLIND_OR_STRADDLE_POSTING,
                 Automation.HOLE_CARDS_SHOWING_OR_MUCKING,
                 Automation.HAND_KILLING,
                 Automation.CHIPS_PUSHING,
                 Automation.CHIPS_PULLING,
             ),
-            True,
-            0,
-            (75000, 150000),
-            150000,
-            300000,
-            (1180000, 4340000, 5910000, 10765000),
-            4,
+            True,  # Uniform antes?
+            0,  # Antes
+            (75000, 150000),  # Blinds or straddles
+            150000,  # Small-bet
+            300000,  # Big-bet
+            (1180000, 4340000, 5910000, 10765000),  # Starting stacks
+            4,  # Number of players
         )
 
         # Below are the pre-flop dealings and actions.
 
         state.deal_hole('7h6c4c3d2c')  # Yockey
         state.deal_hole('??????????')  # Hui
         state.deal_hole('??????????')  # Esposito
@@ -1089,33 +1104,39 @@
 
         self.assertEqual(state.stacks, [0, 4190000, 5910000, 12095000])
 
     def test_alice_carol(self) -> None:
         # Below shows an example badugi hand from Wikipedia.
         #
         # Link: https://en.wikipedia.org/wiki/Badugi
+        #
+        # Note that the starting stacks are set to be ``math.inf`` as
+        # they are not mentioned.
+
+        from math import inf
 
         from pokerkit import Automation, FixedLimitBadugi
 
         state = FixedLimitBadugi.create_state(
+            # Automations
             (
                 Automation.ANTE_POSTING,
                 Automation.BET_COLLECTION,
                 Automation.BLIND_OR_STRADDLE_POSTING,
                 Automation.HAND_KILLING,
                 Automation.CHIPS_PUSHING,
                 Automation.CHIPS_PULLING,
             ),
-            True,
-            0,
-            (1, 2),
-            2,
-            4,
-            200,
-            4,
+            True,  # Uniform antes?
+            0,  # Antes
+            (1, 2),  # Blinds or straddles
+            2,  # Small-bet
+            4,  # Big-bet
+            inf,  # type: ignore[arg-type]  # Starting stacks
+            4,  # Number of players
         )
 
         # Below are the pre-flop dealings and actions.
 
         state.deal_hole('????????')  # Bob
         state.deal_hole('????????')  # Carol
         state.deal_hole('????????')  # Ted
@@ -1170,14 +1191,16 @@
         # Below is the showdown.
 
         state.show_or_muck_hole_cards('2s4c6d9h')  # Alice
         state.show_or_muck_hole_cards('3s5d7c8h')  # Carol
 
         # Below are the final stacks.
 
-        # print(state.stacks)  # [196, 220, 200, 184]
+        # print(state.stacks)  # [inf, inf, inf, inf]
+        # print(state.payoffs)  # [-4, 20, 0, -16]
 
-        self.assertEqual(state.stacks, [196, 220, 200, 184])
+        self.assertEqual(state.stacks, [inf, inf, inf, inf])
+        self.assertEqual(state.payoffs, [-4, 20, 0, -16])
 
 
 if __name__ == '__main__':
     main()  # pragma: no cover
```

### Comparing `pokerkit-0.5.0a1/pokerkit/tests/test_state.py` & `pokerkit-0.5.1/pokerkit/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a1/pokerkit/tests/test_utilities.py` & `pokerkit-0.5.1/pokerkit/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a1/pokerkit/tests/test_wsop/test_2023_43_5.py` & `pokerkit-0.5.1/pokerkit/tests/test_wsop/test_2023_43_5.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a1/pokerkit/tests/test_wsop/test_2023_54_4.py` & `pokerkit-0.5.1/pokerkit/tests/test_wsop/test_2023_54_4.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a1/pokerkit/utilities.py` & `pokerkit-0.5.1/pokerkit/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,20 +229,25 @@
     dataclasses.FrozenInstanceError: cannot assign to field 'rank'
 
     The card is also hashable.
 
     >>> from collections.abc import Hashable
     >>> isinstance(card, Hashable)
     True
+
+    :param rank: The rank. For more details, please refer to
+                 :attr:`pokerkit.utilities.Card.rank`.
+    :param suit: The suit. For more details, please refer to
+                 :attr:`pokerkit.utilities.Card.suit`.
     """
 
     rank: Rank
-    """The rank."""
+    """The rank of the card."""
     suit: Suit
-    """The suit."""
+    """The suit of the card."""
 
     @classmethod
     def get_ranks(cls, cards: CardsLike) -> Iterator[Rank]:
         """Return an iterator of the ranks of each card.
 
         >>> Card.get_ranks('2sKh')  # doctest: +ELLIPSIS
         <generator object Card.get_ranks at 0x...>
@@ -413,14 +418,21 @@
         return f'{self.rank}{self.suit}'
 
     def __str__(self) -> str:
         return f'{self.rank.name} OF {self.suit.name}S ({repr(self)})'
 
     @property
     def unknown_status(self) -> bool:
+        """Return the unknown-ness of the card.
+
+        A card is "unknown" if both or either one of its rank or suit is
+        unknown.
+
+        :return: The unknown-ness of the card.
+        """
         return self.rank == Rank.UNKNOWN or self.suit == Suit.UNKNOWN
 
 
 CardsLike = Iterable[Card] | Card | str
 
 
 @unique
@@ -593,14 +605,15 @@
     Traceback (most recent call last):
         ...
     ValueError: The values None are invalid.
 
     :param values: The values.
     :param count: The number of values.
     :return: The cleaned integers.
+    :raises ValueError: If the values are invalid.
     """
     if isinstance(values, int | float):
         values = (values,) * count
     elif isinstance(values, Mapping):
         parsed_values = [0] * count
 
         for key, value in values.items():
@@ -666,15 +679,15 @@
         *,
         percentage: float = 0,
         cap: float = inf,
         no_flop_no_drop: bool = False,
 ) -> tuple[int, int]:
     """Rake the amount.
 
-    Note that the percentage value are expected to be within range
+    Note that the percentage value is expected to be within range
     [``0``, ``1``]. For instance, ``0.1`` represents 10%.
 
     >>> rake(100)
     (0, 100)
     >>> rake(1000, percentage=0.1)
     (100, 900)
     >>> rake(10, percentage=0.11)
```

### Comparing `pokerkit-0.5.0a1/pokerkit.egg-info/PKG-INFO` & `pokerkit-0.5.1/pokerkit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerkit
-Version: 0.5.0a1
+Version: 0.5.1
 Summary: An open-source Python library for poker game simulations, hand evaluations, and statistical analysis
 Home-page: https://github.com/uoftcprg/pokerkit
 Author: University of Toronto Computer Poker Student Research Group
 Author-email: uoftcprg@studentorg.utoronto.ca
 License: MIT
 Project-URL: Documentation, https://pokerkit.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/uoftcprg/pokerkit
@@ -61,16 +61,20 @@
 Multi-Runout in an All-In Situation
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Below shows the 4-runout hand between Phil Hellmuth and the Loose Cannon Ernest Wiggins.
 
 Link: https://youtu.be/cnjJv7x0HMY?si=4l05Ez7lQVczt8DI&t=638
 
+Note that the starting stacks for some players are set to be ``math.inf`` as they are not mentioned.
+
 .. code-block:: python
 
+   from math import inf
+
    from pokerkit import Automation, Mode, NoLimitTexasHoldem
 
    state = NoLimitTexasHoldem.create_state(
        # Automations
        (
            Automation.ANTE_POSTING,
            Automation.BET_COLLECTION,
@@ -80,15 +84,15 @@
            Automation.CHIPS_PUSHING,
            Automation.CHIPS_PULLING,
        ),
        False,  # Uniform antes?
        {-1: 600},  # Antes
        (200, 400, 800),  # Blinds or straddles
        400,  # Min-bet
-       (999999, 116400, 86900, 999999, 50000, 999999),  # Starting stacks
+       (inf, 116400, 86900, inf, 50000, inf),  # Starting stacks
        6,  # Number of players
        mode=Mode.CASH_GAME,
    )
 
 Below are the pre-flop dealings and actions.
 
 .. code-block:: python
@@ -167,25 +171,29 @@
    state.burn_card('??')
    state.deal_board('Kd')  # River
 
 Below are the final stacks.
 
 .. code-block:: python
 
-   print(state.stacks)  # [987399, 79400, 149700, 999999, 37400, 999399]
+   print(state.stacks)  # [inf, 79400, 149700, inf, 37400, inf]
 
 A Sample No-Limit Texas Hold'em Hand
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Below shows the first televised million-dollar pot between Tom Dwan and Phil Ivey.
 
 Link: https://youtu.be/GnxFohpljqM
 
+Note that the starting stack of Patrik Antonius is set to be ``math.inf`` as it is not mentioned.
+
 .. code-block:: python
 
+   from math import inf
+
    from pokerkit import Automation, NoLimitTexasHoldem
 
    state = NoLimitTexasHoldem.create_state(
        # Automations
        (
            Automation.ANTE_POSTING,
            Automation.BET_COLLECTION,
@@ -195,15 +203,15 @@
            Automation.CHIPS_PUSHING,
            Automation.CHIPS_PULLING,
        ),
        True,  # Uniform antes?
        500,  # Antes
        (1000, 2000),  # Blinds or straddles
        2000,  # Min-bet
-       (1125600, 2000000, 553500),  # Starting stacks
+       (1125600, inf, 553500),  # Starting stacks
        3,  # Number of players
    )
 
 Below are the pre-flop dealings and actions.
 
 .. code-block:: python
 
@@ -245,15 +253,15 @@
    state.burn_card('??')
    state.deal_board('Jh')
 
 Below are the final stacks.
 
 .. code-block:: python
 
-   print(state.stacks)  # [572100, 1997500, 1109500]
+   print(state.stacks)  # [572100, inf, 1109500]
 
 A Sample Short-Deck Hold'em Hand
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Below shows an all-in hand between Xuan and Phua.
 
 Link: https://youtu.be/QlgCcphLjaQ
@@ -495,16 +503,20 @@
 A Sample Badugi Hand
 ^^^^^^^^^^^^^^^^^^^^
 
 Below shows an example badugi hand from Wikipedia.
 
 Link: https://en.wikipedia.org/wiki/Badugi
 
+Note that the starting stacks are set to be ``math.inf`` as they are not mentioned.
+
 .. code-block:: python
 
+   from math import inf
+
    from pokerkit import Automation, FixedLimitBadugi
 
    state = FixedLimitBadugi.create_state(
        # Automations
        (
            Automation.ANTE_POSTING,
            Automation.BET_COLLECTION,
@@ -514,15 +526,15 @@
            Automation.CHIPS_PULLING,
        ),
        True,  # Uniform antes?
        0,  # Antes
        (1, 2),  # Blinds or straddles
        2,  # Small-bet
        4,  # Big-bet
-       200,  # Starting stacks
+       inf,  # Starting stacks
        4,  # Number of players
    )
 
 Below are the pre-flop dealings and actions.
 
 .. code-block:: python
 
@@ -590,15 +602,16 @@
    state.show_or_muck_hole_cards('2s4c6d9h')  # Alice
    state.show_or_muck_hole_cards('3s5d7c8h')  # Carol
 
 Below are the final stacks.
 
 .. code-block:: python
 
-   print(state.stacks)  # [196, 220, 200, 184]
+   print(state.stacks)  # [inf, inf, inf, inf]
+   print(state.payoffs)  # [-4, 20, 0, -16]
 
 Testing and Validation
 ----------------------
 
 PokerKit has extensive test coverage, passes mypy static type checking with strict mode, and has been validated through extensive use in real-life scenarios.
 
 Contributing
```

### Comparing `pokerkit-0.5.0a1/pokerkit.egg-info/SOURCES.txt` & `pokerkit-0.5.1/pokerkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pokerkit-0.5.0a1/setup.py` & `pokerkit-0.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 from setuptools import find_packages, setup
 
 setup(
     name='pokerkit',
-    version='0.5.0a1',
+    version='0.5.1',
     description='An open-source Python library for poker game simulations, hand evaluations, and statistical analysis',
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
     url='https://github.com/uoftcprg/pokerkit',
     author='University of Toronto Computer Poker Student Research Group',
     author_email='uoftcprg@studentorg.utoronto.ca',
     license='MIT',
```


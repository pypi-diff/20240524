# Comparing `tmp/fasttyper-2.4.1.tar.gz` & `tmp/fasttyper-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasttyper-2.4.1.tar", last modified: Sat Dec  3 15:06:55 2022, max compression
+gzip compressed data, was "fasttyper-2.4.2.tar", last modified: Fri May 24 11:56:08 2024, max compression
```

## Comparing `fasttyper-2.4.1.tar` & `fasttyper-2.4.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 doman      (501) staff       (20)        0 2022-12-03 15:06:55.942876 fasttyper-2.4.1/
--rw-r--r--   0 doman      (501) staff       (20)    35149 2022-12-01 21:04:45.000000 fasttyper-2.4.1/LICENSE
--rw-r--r--   0 doman      (501) staff       (20)     7633 2022-12-03 15:06:55.942933 fasttyper-2.4.1/PKG-INFO
--rw-r--r--   0 doman      (501) staff       (20)     7166 2022-12-03 14:56:21.000000 fasttyper-2.4.1/README.md
-drwxr-xr-x   0 doman      (501) staff       (20)        0 2022-12-03 15:06:55.942010 fasttyper-2.4.1/fasttyper/
--rw-r--r--   0 doman      (501) staff       (20)        0 2022-12-01 21:04:45.000000 fasttyper-2.4.1/fasttyper/__init__.py
--rw-r--r--   0 doman      (501) staff       (20)      744 2022-12-01 21:04:45.000000 fasttyper-2.4.1/fasttyper/__main__.py
--rw-r--r--   0 doman      (501) staff       (20)     1241 2022-12-01 21:04:45.000000 fasttyper-2.4.1/fasttyper/application.py
--rw-r--r--   0 doman      (501) staff       (20)     4262 2022-12-01 21:04:45.000000 fasttyper-2.4.1/fasttyper/buffer.py
--rw-r--r--   0 doman      (501) staff       (20)     2334 2022-12-03 14:47:34.000000 fasttyper-2.4.1/fasttyper/cli.py
--rw-r--r--   0 doman      (501) staff       (20)    12002 2022-12-01 21:04:45.000000 fasttyper-2.4.1/fasttyper/components.py
--rw-r--r--   0 doman      (501) staff       (20)     1519 2022-12-03 14:50:24.000000 fasttyper-2.4.1/fasttyper/config.py
--rw-r--r--   0 doman      (501) staff       (20)     2023 2022-12-01 21:04:45.000000 fasttyper-2.4.1/fasttyper/interface.py
--rw-r--r--   0 doman      (501) staff       (20)     1869 2022-12-01 21:04:45.000000 fasttyper-2.4.1/fasttyper/listener.py
--rw-r--r--   0 doman      (501) staff       (20)     4794 2022-12-03 15:05:50.000000 fasttyper-2.4.1/fasttyper/runner.py
--rw-r--r--   0 doman      (501) staff       (20)     4743 2022-12-01 21:04:45.000000 fasttyper-2.4.1/fasttyper/stats.py
-drwxr-xr-x   0 doman      (501) staff       (20)        0 2022-12-03 15:06:55.942752 fasttyper-2.4.1/fasttyper.egg-info/
--rw-r--r--   0 doman      (501) staff       (20)     7633 2022-12-03 15:06:55.000000 fasttyper-2.4.1/fasttyper.egg-info/PKG-INFO
--rw-r--r--   0 doman      (501) staff       (20)      470 2022-12-03 15:06:55.000000 fasttyper-2.4.1/fasttyper.egg-info/SOURCES.txt
--rw-r--r--   0 doman      (501) staff       (20)        1 2022-12-03 15:06:55.000000 fasttyper-2.4.1/fasttyper.egg-info/dependency_links.txt
--rw-r--r--   0 doman      (501) staff       (20)       54 2022-12-03 15:06:55.000000 fasttyper-2.4.1/fasttyper.egg-info/entry_points.txt
--rw-r--r--   0 doman      (501) staff       (20)       89 2022-12-03 15:06:55.000000 fasttyper-2.4.1/fasttyper.egg-info/requires.txt
--rw-r--r--   0 doman      (501) staff       (20)       10 2022-12-03 15:06:55.000000 fasttyper-2.4.1/fasttyper.egg-info/top_level.txt
--rw-r--r--   0 doman      (501) staff       (20)      100 2022-12-03 15:06:55.943137 fasttyper-2.4.1/setup.cfg
--rw-r--r--   0 doman      (501) staff       (20)      958 2022-12-03 15:06:34.000000 fasttyper-2.4.1/setup.py
+drwxr-xr-x   0 doman      (501) staff       (20)        0 2024-05-24 11:56:08.552328 fasttyper-2.4.2/
+-rw-r--r--   0 doman      (501) staff       (20)    35149 2024-05-24 11:48:30.000000 fasttyper-2.4.2/LICENSE
+-rw-r--r--   0 doman      (501) staff       (20)     8297 2024-05-24 11:56:08.552231 fasttyper-2.4.2/PKG-INFO
+-rw-r--r--   0 doman      (501) staff       (20)     7699 2024-05-24 11:48:30.000000 fasttyper-2.4.2/README.md
+drwxr-xr-x   0 doman      (501) staff       (20)        0 2024-05-24 11:56:08.550984 fasttyper-2.4.2/fasttyper/
+-rw-r--r--   0 doman      (501) staff       (20)        0 2024-05-24 11:48:30.000000 fasttyper-2.4.2/fasttyper/__init__.py
+-rw-r--r--   0 doman      (501) staff       (20)      744 2024-05-24 11:48:30.000000 fasttyper-2.4.2/fasttyper/__main__.py
+-rw-r--r--   0 doman      (501) staff       (20)     1241 2024-05-24 11:48:30.000000 fasttyper-2.4.2/fasttyper/application.py
+-rw-r--r--   0 doman      (501) staff       (20)     4262 2024-05-24 11:48:30.000000 fasttyper-2.4.2/fasttyper/buffer.py
+-rw-r--r--   0 doman      (501) staff       (20)     2334 2024-05-24 11:48:30.000000 fasttyper-2.4.2/fasttyper/cli.py
+-rw-r--r--   0 doman      (501) staff       (20)    12002 2024-05-24 11:48:30.000000 fasttyper-2.4.2/fasttyper/components.py
+-rw-r--r--   0 doman      (501) staff       (20)     1519 2024-05-24 11:48:30.000000 fasttyper-2.4.2/fasttyper/config.py
+-rw-r--r--   0 doman      (501) staff       (20)     2023 2024-05-24 11:48:30.000000 fasttyper-2.4.2/fasttyper/interface.py
+-rw-r--r--   0 doman      (501) staff       (20)     1869 2024-05-24 11:48:30.000000 fasttyper-2.4.2/fasttyper/listener.py
+-rw-r--r--   0 doman      (501) staff       (20)     4794 2024-05-24 11:48:30.000000 fasttyper-2.4.2/fasttyper/runner.py
+-rw-r--r--   0 doman      (501) staff       (20)     4743 2024-05-24 11:48:30.000000 fasttyper-2.4.2/fasttyper/stats.py
+drwxr-xr-x   0 doman      (501) staff       (20)        0 2024-05-24 11:56:08.552014 fasttyper-2.4.2/fasttyper.egg-info/
+-rw-r--r--   0 doman      (501) staff       (20)     8297 2024-05-24 11:56:08.000000 fasttyper-2.4.2/fasttyper.egg-info/PKG-INFO
+-rw-r--r--   0 doman      (501) staff       (20)      470 2024-05-24 11:56:08.000000 fasttyper-2.4.2/fasttyper.egg-info/SOURCES.txt
+-rw-r--r--   0 doman      (501) staff       (20)        1 2024-05-24 11:56:08.000000 fasttyper-2.4.2/fasttyper.egg-info/dependency_links.txt
+-rw-r--r--   0 doman      (501) staff       (20)       54 2024-05-24 11:56:08.000000 fasttyper-2.4.2/fasttyper.egg-info/entry_points.txt
+-rw-r--r--   0 doman      (501) staff       (20)       89 2024-05-24 11:56:08.000000 fasttyper-2.4.2/fasttyper.egg-info/requires.txt
+-rw-r--r--   0 doman      (501) staff       (20)       10 2024-05-24 11:56:08.000000 fasttyper-2.4.2/fasttyper.egg-info/top_level.txt
+-rw-r--r--   0 doman      (501) staff       (20)      100 2024-05-24 11:56:08.552509 fasttyper-2.4.2/setup.cfg
+-rw-r--r--   0 doman      (501) staff       (20)      958 2024-05-24 11:51:03.000000 fasttyper-2.4.2/setup.py
```

### Comparing `fasttyper-2.4.1/LICENSE` & `fasttyper-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fasttyper-2.4.1/PKG-INFO` & `fasttyper-2.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,57 @@
-Metadata-Version: 2.1
-Name: fasttyper
-Version: 2.4.1
-Summary: Minimalistic typing exercise
-Home-page: https://github.com/ickyicky/fasttyper
-Author: Piotr Domanski
-Author-email: pi.domanski@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # fasttyper
 [![](https://github.com/ickyicky/fasttyper/blob/main/doc/demo.gif?raw=true)](https://github.com/ickyicky/fasttyper)
 
 # About
 
-_Fasttyper_ is minimalistic typing test based on user provided exercising text. It supports both reading from text files and stdin supporting wide range of usecases. The goal was to create it as simple as it can be, without any additional bloatware functionalities. That means that _Fasttyper_ doesn't come with build in test generator and you have to provide your own scripts generating tests. Some examples of such scrips are providen in [Usage section](#usage).
+_Fasttyper_ is minimalistic typing test based on user provided exercising text. It supports both reading from text files and stdin supporting wide range of usecases. The goal was to create it as simple as it can be, without any additional bloatware functionalities. That means that _Fasttyper_ doesn't come with build in test generator and you have to provide your own scripts generating tests. Some examples of such scripts are provided in [Usage section](#usage).
+
+# Table of contents
+
+  - [fasttyper](#fasttyper)
+  - [About](#about)
+  - [Installation](#installation)
+  - [Usage](#usage)
+  - [Running next test and stopping application](#running-next-test-and-stopping-application)
+  - [Configuring](#configuring)
+  - [Usage as module, piping stuff, custom scripts etc](#usage-as-module,-piping-stuff,-custom-scripts-etc)
+  - [When backspace does wierd shiet](#when-backspace-does-wierd-shiet)
+  - [Hiding cursor](#hiding-cursor)
+    - [Example scripts](#example-scripts)
 
 # Installation
 
-_Fasttyper_ is currently maintained on [PyPi](https://pypi.org/) Python Package Index. To install package simpply use:
+_Fasttyper_ is currently maintained on [PyPi](https://pypi.org/) Python Package Index. To install package simply use:
 
 `python3 -m pip install fasttyper`
 
 # Usage
 
 With installation of fasttyper you should have new executable - `fasttyper`. It takes two optional positional arguments, amount of words and language (like in [Monkeytype's](https://github.com/Miodec/monkeytype): english, english_1k etc). Default amount of words is 25 and language is english. To run fasttyper simply call:
 
 ```bash
 fasttyper
 ```
 
-from command line. There are some avalibe options:
+from command line. There are some available options:
 
 ```
 usage: fasttyper [-h] [--config FILE] [--unclutter-backspace] [--no-cursor] [amount] [language]
 
 positional arguments:
   amount                Amount of words
   language              Language
 
 options:
   -h, --help            show this help message and exit
   --config FILE, -c FILE
                         configuration file
   --unclutter-backspace, -b
                         unclutter backspace, when it raises ctrl+backspace instead
-  --no-cursor, -n       disable cursos
+  --no-cursor, -n       disable cursors
 ```
 
 I personally use alias:
 
 ```
 alias ff='fasttyper -n`
 ```
@@ -105,28 +104,28 @@
     "amount": 25,
     "language": "english",
     "no_cursor": False,
     "unclutter_backspace": False,
 }
 ```
 
-Fasttyper by default looks for config file in: `$HOME/.config/fasttyper/config.json`. You can provide different location for config file with `--config` argument, for example: `--config=~/.fasttyper.json`. Config has to be a json dict. Avalibe keys:
+Fasttyper by default looks for config file in: `$HOME/.config/fasttyper/config.json`. You can provide different location for config file with `--config` argument, for example: `--config=~/.fasttyper.json`. Config has to be a json dict. Available keys:
 
 - **user_input_valid_color** - integer, terminal color for valid text, by default it is 3
 - **user_input_invalid_color** - integer, terminal color for invalid text, by default it is 2
 - **reference_text_color** - integer, terminal color for reference text, by default it is 8
 - **stats_color** - integer, terminal color for stats text, by default it is 5
 - **summary_datafile** - datafile storing all stats, by default it is ~/.cache/fasttyper/datafile.csv
 - **top_margin_percentage** - integer, percentage of screen used for top margin, by default 30
 - **left_margin_percentage** - integer, percentage of screen used for left (and right) margin, by default 10
 - **lines_on_screen** - integer, number of lines to display on screen, by default 3
 
 Also there are keys that override fault parameters for CLI args, like: amount and language will override Your default settings for runner, same goes for punctuation, sentence_mode etc.
 
-Example config file with all default values in avalibe [here](https://github.com/ickyicky/fasttyper/blob/main/doc/example_config.json).
+Example config file with all default values in available [here](https://github.com/ickyicky/fasttyper/blob/main/doc/example_config.json).
 
 Other example config files:
 
 ```json
 {"top_margin_percentage": 40, "left_margin_percentage": 25}
 ```
 
@@ -146,21 +145,21 @@
 
 `python3 -m fasttyper example_text.txt`
 
 Program also allows user to pipe text into it. Keep in mind, it only supports spaces and new line characters, so you won't be able to table tabs. For example, you can run _Fasttyper_ on fortune generated quote changing tabulators to spaces with sed:
 
 `furtune | python3 -m fasttyper`
 
-or if you want to randomize words from given file with shuf on for example all disctionaries in system:
+or if you want to randomize words from given file with shuf on for example all dictionaries in system:
 
 `shuf -n5 /usr/share/dict/* | python -m fasttyper`
 
 You can use another similar projects set of words as well, for example to create test with 20 random words from [Monkeytype's](https://github.com/Miodec/monkeytype) english 100 dictionary use:
 
-`curl -s https://raw.githubusercontent.com/Miodec/monkeytype/master/static/languages/english.json | python3 -c "import sys, json; print('\n'.join(json.load(sys.stdin)['words']))" | shuf -n20 | python3 -m fasttyper`
+`curl -s https://raw.githubusercontent.com/monkeytypegame/monkeytype/master/frontend/static/languages/english.json | python3 -c "import sys, json; print('\n'.join(json.load(sys.stdin)['words']))" | shuf -n20 | python3 -m fasttyper`
 
 To exit you can either finish test, use `KeyboardInterrupt` (CTRL+C) or tap **tab**. After you finish test, there will be summary printed, use enter to exit from it.
 
 # When backspace does wierd shiet
 
 Some terminal emulators send different values for key presses of backspace and ctrl+backspace. To fix it, simply add `b` flag like that: `python3 -m fasttyper -b`.
 
@@ -182,10 +181,10 @@
 	do
 		shuf -n $amount $sfile | python3 -m fasttyper || break
 	done
 }
 ```
 `ff 50 english_1k`
 
-This shell function shuffles N words from cached word list, and if given word list doesnt exist it download's it. It runs in loop, but does exit from it if you exit fasttyper with CTRL+C.
+This shell function shuffles N words from cached word list, and if given word list doesn't exist it download's it. It runs in loop, but does exit from it if you exit fasttyper with CTRL+C.
 
-The above script is avalible for download from doc folder.
+The above script is available for download from doc folder.
```

### Comparing `fasttyper-2.4.1/README.md` & `fasttyper-2.4.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,74 @@
+Metadata-Version: 2.1
+Name: fasttyper
+Version: 2.4.2
+Summary: Minimalistic typing exercise
+Home-page: https://github.com/ickyicky/fasttyper
+Author: Piotr Domanski
+Author-email: pi.domanski@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: readchar
+Requires-Dist: requests
+Requires-Dist: windows-curses; sys_platform == "win32" or sys_platform == "cygwin"
+
 # fasttyper
 [![](https://github.com/ickyicky/fasttyper/blob/main/doc/demo.gif?raw=true)](https://github.com/ickyicky/fasttyper)
 
 # About
 
-_Fasttyper_ is minimalistic typing test based on user provided exercising text. It supports both reading from text files and stdin supporting wide range of usecases. The goal was to create it as simple as it can be, without any additional bloatware functionalities. That means that _Fasttyper_ doesn't come with build in test generator and you have to provide your own scripts generating tests. Some examples of such scrips are providen in [Usage section](#usage).
+_Fasttyper_ is minimalistic typing test based on user provided exercising text. It supports both reading from text files and stdin supporting wide range of usecases. The goal was to create it as simple as it can be, without any additional bloatware functionalities. That means that _Fasttyper_ doesn't come with build in test generator and you have to provide your own scripts generating tests. Some examples of such scripts are provided in [Usage section](#usage).
+
+# Table of contents
+
+  - [fasttyper](#fasttyper)
+  - [About](#about)
+  - [Installation](#installation)
+  - [Usage](#usage)
+  - [Running next test and stopping application](#running-next-test-and-stopping-application)
+  - [Configuring](#configuring)
+  - [Usage as module, piping stuff, custom scripts etc](#usage-as-module,-piping-stuff,-custom-scripts-etc)
+  - [When backspace does wierd shiet](#when-backspace-does-wierd-shiet)
+  - [Hiding cursor](#hiding-cursor)
+    - [Example scripts](#example-scripts)
 
 # Installation
 
-_Fasttyper_ is currently maintained on [PyPi](https://pypi.org/) Python Package Index. To install package simpply use:
+_Fasttyper_ is currently maintained on [PyPi](https://pypi.org/) Python Package Index. To install package simply use:
 
 `python3 -m pip install fasttyper`
 
 # Usage
 
 With installation of fasttyper you should have new executable - `fasttyper`. It takes two optional positional arguments, amount of words and language (like in [Monkeytype's](https://github.com/Miodec/monkeytype): english, english_1k etc). Default amount of words is 25 and language is english. To run fasttyper simply call:
 
 ```bash
 fasttyper
 ```
 
-from command line. There are some avalibe options:
+from command line. There are some available options:
 
 ```
 usage: fasttyper [-h] [--config FILE] [--unclutter-backspace] [--no-cursor] [amount] [language]
 
 positional arguments:
   amount                Amount of words
   language              Language
 
 options:
   -h, --help            show this help message and exit
   --config FILE, -c FILE
                         configuration file
   --unclutter-backspace, -b
                         unclutter backspace, when it raises ctrl+backspace instead
-  --no-cursor, -n       disable cursos
+  --no-cursor, -n       disable cursors
 ```
 
 I personally use alias:
 
 ```
 alias ff='fasttyper -n`
 ```
@@ -91,28 +121,28 @@
     "amount": 25,
     "language": "english",
     "no_cursor": False,
     "unclutter_backspace": False,
 }
 ```
 
-Fasttyper by default looks for config file in: `$HOME/.config/fasttyper/config.json`. You can provide different location for config file with `--config` argument, for example: `--config=~/.fasttyper.json`. Config has to be a json dict. Avalibe keys:
+Fasttyper by default looks for config file in: `$HOME/.config/fasttyper/config.json`. You can provide different location for config file with `--config` argument, for example: `--config=~/.fasttyper.json`. Config has to be a json dict. Available keys:
 
 - **user_input_valid_color** - integer, terminal color for valid text, by default it is 3
 - **user_input_invalid_color** - integer, terminal color for invalid text, by default it is 2
 - **reference_text_color** - integer, terminal color for reference text, by default it is 8
 - **stats_color** - integer, terminal color for stats text, by default it is 5
 - **summary_datafile** - datafile storing all stats, by default it is ~/.cache/fasttyper/datafile.csv
 - **top_margin_percentage** - integer, percentage of screen used for top margin, by default 30
 - **left_margin_percentage** - integer, percentage of screen used for left (and right) margin, by default 10
 - **lines_on_screen** - integer, number of lines to display on screen, by default 3
 
 Also there are keys that override fault parameters for CLI args, like: amount and language will override Your default settings for runner, same goes for punctuation, sentence_mode etc.
 
-Example config file with all default values in avalibe [here](https://github.com/ickyicky/fasttyper/blob/main/doc/example_config.json).
+Example config file with all default values in available [here](https://github.com/ickyicky/fasttyper/blob/main/doc/example_config.json).
 
 Other example config files:
 
 ```json
 {"top_margin_percentage": 40, "left_margin_percentage": 25}
 ```
 
@@ -132,21 +162,21 @@
 
 `python3 -m fasttyper example_text.txt`
 
 Program also allows user to pipe text into it. Keep in mind, it only supports spaces and new line characters, so you won't be able to table tabs. For example, you can run _Fasttyper_ on fortune generated quote changing tabulators to spaces with sed:
 
 `furtune | python3 -m fasttyper`
 
-or if you want to randomize words from given file with shuf on for example all disctionaries in system:
+or if you want to randomize words from given file with shuf on for example all dictionaries in system:
 
 `shuf -n5 /usr/share/dict/* | python -m fasttyper`
 
 You can use another similar projects set of words as well, for example to create test with 20 random words from [Monkeytype's](https://github.com/Miodec/monkeytype) english 100 dictionary use:
 
-`curl -s https://raw.githubusercontent.com/Miodec/monkeytype/master/static/languages/english.json | python3 -c "import sys, json; print('\n'.join(json.load(sys.stdin)['words']))" | shuf -n20 | python3 -m fasttyper`
+`curl -s https://raw.githubusercontent.com/monkeytypegame/monkeytype/master/frontend/static/languages/english.json | python3 -c "import sys, json; print('\n'.join(json.load(sys.stdin)['words']))" | shuf -n20 | python3 -m fasttyper`
 
 To exit you can either finish test, use `KeyboardInterrupt` (CTRL+C) or tap **tab**. After you finish test, there will be summary printed, use enter to exit from it.
 
 # When backspace does wierd shiet
 
 Some terminal emulators send different values for key presses of backspace and ctrl+backspace. To fix it, simply add `b` flag like that: `python3 -m fasttyper -b`.
 
@@ -168,10 +198,10 @@
 	do
 		shuf -n $amount $sfile | python3 -m fasttyper || break
 	done
 }
 ```
 `ff 50 english_1k`
 
-This shell function shuffles N words from cached word list, and if given word list doesnt exist it download's it. It runs in loop, but does exit from it if you exit fasttyper with CTRL+C.
+This shell function shuffles N words from cached word list, and if given word list doesn't exist it download's it. It runs in loop, but does exit from it if you exit fasttyper with CTRL+C.
 
-The above script is avalible for download from doc folder.
+The above script is available for download from doc folder.
```

### Comparing `fasttyper-2.4.1/fasttyper/__main__.py` & `fasttyper-2.4.2/fasttyper/__main__.py`

 * *Files identical despite different names*

### Comparing `fasttyper-2.4.1/fasttyper/application.py` & `fasttyper-2.4.2/fasttyper/application.py`

 * *Files identical despite different names*

### Comparing `fasttyper-2.4.1/fasttyper/buffer.py` & `fasttyper-2.4.2/fasttyper/buffer.py`

 * *Files identical despite different names*

### Comparing `fasttyper-2.4.1/fasttyper/cli.py` & `fasttyper-2.4.2/fasttyper/cli.py`

 * *Files identical despite different names*

### Comparing `fasttyper-2.4.1/fasttyper/components.py` & `fasttyper-2.4.2/fasttyper/components.py`

 * *Files identical despite different names*

### Comparing `fasttyper-2.4.1/fasttyper/config.py` & `fasttyper-2.4.2/fasttyper/config.py`

 * *Files identical despite different names*

### Comparing `fasttyper-2.4.1/fasttyper/interface.py` & `fasttyper-2.4.2/fasttyper/interface.py`

 * *Files identical despite different names*

### Comparing `fasttyper-2.4.1/fasttyper/listener.py` & `fasttyper-2.4.2/fasttyper/listener.py`

 * *Files identical despite different names*

### Comparing `fasttyper-2.4.1/fasttyper/runner.py` & `fasttyper-2.4.2/fasttyper/runner.py`

 * *Files identical despite different names*

### Comparing `fasttyper-2.4.1/fasttyper/stats.py` & `fasttyper-2.4.2/fasttyper/stats.py`

 * *Files identical despite different names*

### Comparing `fasttyper-2.4.1/fasttyper.egg-info/PKG-INFO` & `fasttyper-2.4.2/fasttyper.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,58 +1,74 @@
 Metadata-Version: 2.1
 Name: fasttyper
-Version: 2.4.1
+Version: 2.4.2
 Summary: Minimalistic typing exercise
 Home-page: https://github.com/ickyicky/fasttyper
 Author: Piotr Domanski
 Author-email: pi.domanski@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: readchar
+Requires-Dist: requests
+Requires-Dist: windows-curses; sys_platform == "win32" or sys_platform == "cygwin"
 
 # fasttyper
 [![](https://github.com/ickyicky/fasttyper/blob/main/doc/demo.gif?raw=true)](https://github.com/ickyicky/fasttyper)
 
 # About
 
-_Fasttyper_ is minimalistic typing test based on user provided exercising text. It supports both reading from text files and stdin supporting wide range of usecases. The goal was to create it as simple as it can be, without any additional bloatware functionalities. That means that _Fasttyper_ doesn't come with build in test generator and you have to provide your own scripts generating tests. Some examples of such scrips are providen in [Usage section](#usage).
+_Fasttyper_ is minimalistic typing test based on user provided exercising text. It supports both reading from text files and stdin supporting wide range of usecases. The goal was to create it as simple as it can be, without any additional bloatware functionalities. That means that _Fasttyper_ doesn't come with build in test generator and you have to provide your own scripts generating tests. Some examples of such scripts are provided in [Usage section](#usage).
+
+# Table of contents
+
+  - [fasttyper](#fasttyper)
+  - [About](#about)
+  - [Installation](#installation)
+  - [Usage](#usage)
+  - [Running next test and stopping application](#running-next-test-and-stopping-application)
+  - [Configuring](#configuring)
+  - [Usage as module, piping stuff, custom scripts etc](#usage-as-module,-piping-stuff,-custom-scripts-etc)
+  - [When backspace does wierd shiet](#when-backspace-does-wierd-shiet)
+  - [Hiding cursor](#hiding-cursor)
+    - [Example scripts](#example-scripts)
 
 # Installation
 
-_Fasttyper_ is currently maintained on [PyPi](https://pypi.org/) Python Package Index. To install package simpply use:
+_Fasttyper_ is currently maintained on [PyPi](https://pypi.org/) Python Package Index. To install package simply use:
 
 `python3 -m pip install fasttyper`
 
 # Usage
 
 With installation of fasttyper you should have new executable - `fasttyper`. It takes two optional positional arguments, amount of words and language (like in [Monkeytype's](https://github.com/Miodec/monkeytype): english, english_1k etc). Default amount of words is 25 and language is english. To run fasttyper simply call:
 
 ```bash
 fasttyper
 ```
 
-from command line. There are some avalibe options:
+from command line. There are some available options:
 
 ```
 usage: fasttyper [-h] [--config FILE] [--unclutter-backspace] [--no-cursor] [amount] [language]
 
 positional arguments:
   amount                Amount of words
   language              Language
 
 options:
   -h, --help            show this help message and exit
   --config FILE, -c FILE
                         configuration file
   --unclutter-backspace, -b
                         unclutter backspace, when it raises ctrl+backspace instead
-  --no-cursor, -n       disable cursos
+  --no-cursor, -n       disable cursors
 ```
 
 I personally use alias:
 
 ```
 alias ff='fasttyper -n`
 ```
@@ -105,28 +121,28 @@
     "amount": 25,
     "language": "english",
     "no_cursor": False,
     "unclutter_backspace": False,
 }
 ```
 
-Fasttyper by default looks for config file in: `$HOME/.config/fasttyper/config.json`. You can provide different location for config file with `--config` argument, for example: `--config=~/.fasttyper.json`. Config has to be a json dict. Avalibe keys:
+Fasttyper by default looks for config file in: `$HOME/.config/fasttyper/config.json`. You can provide different location for config file with `--config` argument, for example: `--config=~/.fasttyper.json`. Config has to be a json dict. Available keys:
 
 - **user_input_valid_color** - integer, terminal color for valid text, by default it is 3
 - **user_input_invalid_color** - integer, terminal color for invalid text, by default it is 2
 - **reference_text_color** - integer, terminal color for reference text, by default it is 8
 - **stats_color** - integer, terminal color for stats text, by default it is 5
 - **summary_datafile** - datafile storing all stats, by default it is ~/.cache/fasttyper/datafile.csv
 - **top_margin_percentage** - integer, percentage of screen used for top margin, by default 30
 - **left_margin_percentage** - integer, percentage of screen used for left (and right) margin, by default 10
 - **lines_on_screen** - integer, number of lines to display on screen, by default 3
 
 Also there are keys that override fault parameters for CLI args, like: amount and language will override Your default settings for runner, same goes for punctuation, sentence_mode etc.
 
-Example config file with all default values in avalibe [here](https://github.com/ickyicky/fasttyper/blob/main/doc/example_config.json).
+Example config file with all default values in available [here](https://github.com/ickyicky/fasttyper/blob/main/doc/example_config.json).
 
 Other example config files:
 
 ```json
 {"top_margin_percentage": 40, "left_margin_percentage": 25}
 ```
 
@@ -146,21 +162,21 @@
 
 `python3 -m fasttyper example_text.txt`
 
 Program also allows user to pipe text into it. Keep in mind, it only supports spaces and new line characters, so you won't be able to table tabs. For example, you can run _Fasttyper_ on fortune generated quote changing tabulators to spaces with sed:
 
 `furtune | python3 -m fasttyper`
 
-or if you want to randomize words from given file with shuf on for example all disctionaries in system:
+or if you want to randomize words from given file with shuf on for example all dictionaries in system:
 
 `shuf -n5 /usr/share/dict/* | python -m fasttyper`
 
 You can use another similar projects set of words as well, for example to create test with 20 random words from [Monkeytype's](https://github.com/Miodec/monkeytype) english 100 dictionary use:
 
-`curl -s https://raw.githubusercontent.com/Miodec/monkeytype/master/static/languages/english.json | python3 -c "import sys, json; print('\n'.join(json.load(sys.stdin)['words']))" | shuf -n20 | python3 -m fasttyper`
+`curl -s https://raw.githubusercontent.com/monkeytypegame/monkeytype/master/frontend/static/languages/english.json | python3 -c "import sys, json; print('\n'.join(json.load(sys.stdin)['words']))" | shuf -n20 | python3 -m fasttyper`
 
 To exit you can either finish test, use `KeyboardInterrupt` (CTRL+C) or tap **tab**. After you finish test, there will be summary printed, use enter to exit from it.
 
 # When backspace does wierd shiet
 
 Some terminal emulators send different values for key presses of backspace and ctrl+backspace. To fix it, simply add `b` flag like that: `python3 -m fasttyper -b`.
 
@@ -182,10 +198,10 @@
 	do
 		shuf -n $amount $sfile | python3 -m fasttyper || break
 	done
 }
 ```
 `ff 50 english_1k`
 
-This shell function shuffles N words from cached word list, and if given word list doesnt exist it download's it. It runs in loop, but does exit from it if you exit fasttyper with CTRL+C.
+This shell function shuffles N words from cached word list, and if given word list doesn't exist it download's it. It runs in loop, but does exit from it if you exit fasttyper with CTRL+C.
 
-The above script is avalible for download from doc folder.
+The above script is available for download from doc folder.
```

### Comparing `fasttyper-2.4.1/setup.py` & `fasttyper-2.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read().splitlines()
 
 
 setup(
     name="fasttyper",
-    version="2.4.1",
+    version="2.4.2",
     author="Piotr Domanski",
     author_email="pi.domanski@gmail.com",
     description="Minimalistic typing exercise",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ickyicky/fasttyper",
     classifiers=[
```


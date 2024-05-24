# Comparing `tmp/fuzzylogic-1.2.0.tar.gz` & `tmp/fuzzylogic-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fuzzylogic-1.2.0.tar", last modified: Fri Feb 11 13:43:00 2022, max compression
+gzip compressed data, was "fuzzylogic-1.4.0.tar", last modified: Fri May 24 09:51:17 2024, max compression
```

## Comparing `fuzzylogic-1.2.0.tar` & `fuzzylogic-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxrwx---   0 root         (0) vboxsf     (998)        0 2022-02-11 13:43:01.684413 fuzzylogic-1.2.0/
--rwxrwx---   0 root         (0) vboxsf     (998)     1097 2021-04-23 10:07:34.000000 fuzzylogic-1.2.0/LICENSE
--rwxrwx---   0 root         (0) vboxsf     (998)     5738 2022-02-11 13:43:01.682460 fuzzylogic-1.2.0/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (998)     4809 2022-02-10 09:28:58.000000 fuzzylogic-1.2.0/README.md
--rwxrwx---   0 root         (0) vboxsf     (998)       38 2022-02-11 13:43:01.684413 fuzzylogic-1.2.0/setup.cfg
--rwxrwx---   0 root         (0) vboxsf     (998)     1434 2022-02-11 11:06:16.000000 fuzzylogic-1.2.0/setup.py
-drwxrwx---   0 root         (0) vboxsf     (998)        0 2022-02-11 13:43:01.533455 fuzzylogic-1.2.0/src/
-drwxrwx---   0 root         (0) vboxsf     (998)        0 2022-02-11 13:43:01.636057 fuzzylogic-1.2.0/src/fuzzylogic/
--rwxrwx---   0 root         (0) vboxsf     (998)       25 2022-02-10 09:39:18.000000 fuzzylogic-1.2.0/src/fuzzylogic/__init__.py
--rwxrwx---   0 root         (0) vboxsf     (998)    18443 2022-02-11 12:45:43.000000 fuzzylogic-1.2.0/src/fuzzylogic/classes.py
--rwxrwx---   0 root         (0) vboxsf     (998)     4990 2021-04-05 22:24:56.000000 fuzzylogic-1.2.0/src/fuzzylogic/combinators.py
--rwxrwx---   0 root         (0) vboxsf     (998)    12892 2021-02-19 14:25:01.000000 fuzzylogic-1.2.0/src/fuzzylogic/functions.py
--rwxrwx---   0 root         (0) vboxsf     (998)     1214 2021-04-05 22:54:39.000000 fuzzylogic-1.2.0/src/fuzzylogic/hedges.py
--rwxrwx---   0 root         (0) vboxsf     (998)     2252 2021-10-01 10:07:03.000000 fuzzylogic-1.2.0/src/fuzzylogic/rules.py
--rwxrwx---   0 root         (0) vboxsf     (998)      714 2017-03-17 18:30:30.000000 fuzzylogic-1.2.0/src/fuzzylogic/truth.py
-drwxrwx---   0 root         (0) vboxsf     (998)        0 2022-02-11 13:43:01.678555 fuzzylogic-1.2.0/src/fuzzylogic.egg-info/
--rwxrwx---   0 root         (0) vboxsf     (998)     5738 2022-02-11 13:43:00.000000 fuzzylogic-1.2.0/src/fuzzylogic.egg-info/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (998)      399 2022-02-11 13:43:00.000000 fuzzylogic-1.2.0/src/fuzzylogic.egg-info/SOURCES.txt
--rwxrwx---   0 root         (0) vboxsf     (998)        1 2022-02-11 13:43:00.000000 fuzzylogic-1.2.0/src/fuzzylogic.egg-info/dependency_links.txt
--rwxrwx---   0 root         (0) vboxsf     (998)        1 2021-10-01 10:18:36.000000 fuzzylogic-1.2.0/src/fuzzylogic.egg-info/not-zip-safe
--rwxrwx---   0 root         (0) vboxsf     (998)       11 2022-02-11 13:43:00.000000 fuzzylogic-1.2.0/src/fuzzylogic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 09:51:17.848665 fuzzylogic-1.4.0/
+-rw-rw-rw-   0        0        0     1097 2022-04-27 16:13:47.000000 fuzzylogic-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0     6023 2024-05-24 09:51:17.832666 fuzzylogic-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4992 2023-06-27 12:15:37.000000 fuzzylogic-1.4.0/README.md
+-rw-rw-rw-   0        0        0     1216 2023-09-18 09:22:03.000000 fuzzylogic-1.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-24 09:51:17.849666 fuzzylogic-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1430 2024-05-24 09:42:13.000000 fuzzylogic-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:51:17.392666 fuzzylogic-1.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-24 09:51:17.524665 fuzzylogic-1.4.0/src/fuzzylogic/
+-rw-rw-rw-   0        0        0       25 2024-05-23 15:27:17.000000 fuzzylogic-1.4.0/src/fuzzylogic/__init__.py
+-rw-rw-rw-   0        0        0    18769 2024-05-24 09:41:00.000000 fuzzylogic-1.4.0/src/fuzzylogic/classes.py
+-rw-rw-rw-   0        0        0     6600 2024-05-24 09:40:34.000000 fuzzylogic-1.4.0/src/fuzzylogic/combinators.py
+-rw-rw-rw-   0        0        0    14581 2024-05-24 08:59:26.000000 fuzzylogic-1.4.0/src/fuzzylogic/functions.py
+-rw-rw-rw-   0        0        0     1214 2021-04-05 22:54:39.000000 fuzzylogic-1.4.0/src/fuzzylogic/hedges.py
+-rw-rw-rw-   0        0        0     2226 2023-06-27 12:44:21.000000 fuzzylogic-1.4.0/src/fuzzylogic/rules.py
+-rw-rw-rw-   0        0        0      714 2017-03-17 18:30:30.000000 fuzzylogic-1.4.0/src/fuzzylogic/truth.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:51:17.823666 fuzzylogic-1.4.0/src/fuzzylogic.egg-info/
+-rw-rw-rw-   0        0        0     6023 2024-05-24 09:51:16.000000 fuzzylogic-1.4.0/src/fuzzylogic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2024-05-24 09:51:16.000000 fuzzylogic-1.4.0/src/fuzzylogic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 09:51:16.000000 fuzzylogic-1.4.0/src/fuzzylogic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2021-10-01 10:18:36.000000 fuzzylogic-1.4.0/src/fuzzylogic.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-24 09:51:16.000000 fuzzylogic-1.4.0/src/fuzzylogic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 09:51:17.802667 fuzzylogic-1.4.0/tests/
+-rw-rw-rw-   0        0        0     1700 2022-04-30 18:08:47.000000 fuzzylogic-1.4.0/tests/test_caro.py
+-rw-rw-rw-   0        0        0     2514 2021-10-01 10:04:15.000000 fuzzylogic-1.4.0/tests/test_functionality.py
+-rw-rw-rw-   0        0        0    17033 2023-06-27 12:15:32.000000 fuzzylogic-1.4.0/tests/test_units.py
```

### Comparing `fuzzylogic-1.2.0/LICENSE` & `fuzzylogic-1.4.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2017-2021 Anselm Kiefner
+Copyright (c) 2017-2022 Anselm Kiefner
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `fuzzylogic-1.2.0/PKG-INFO` & `fuzzylogic-1.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,67 @@
-Metadata-Version: 2.1
-Name: fuzzylogic
-Version: 1.2.0
-Summary: Fuzzy Logic for Python 3
-Home-page: https://github.com/amogorkon/fuzzylogic
-Author: Anselm Kiefner
-Author-email: fuzzylogic-pypi@anselm.kiefner.de
-License: MIT
-Keywords: fuzzy logic
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Manufacturing
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Fuzzy Logic for Python 3
-
-[![license](https://img.shields.io/github/license/amogorkon/fuzzylogic)](https://github.com/amogorkon/fuzzylogic/blob/master/LICENSE)
-[![stars](https://img.shields.io/github/stars/amogorkon/fuzzylogic?style=plastic)](https://github.com/amogorkon/fuzzylogic/stargazers)
-[![forks](https://img.shields.io/github/forks/amogorkon/fuzzylogic?style=plastic)](https://github.com/amogorkon/fuzzylogic/network/members)
-[![Downloads](https://pepy.tech/badge/fuzzylogic)](https://pepy.tech/project/fuzzylogic)
-
-
-This is the fourth time I rebuilt this library from scratch to find the sweet spot between ease of use (beautiful is better than ugly!), testability (simple is better than complex!) and potential for performance optimization (practicality beats purity!). 
-
-### Why a new library?
-The first time I was confronted with fuzzy logic, I fell in love with the concept, but after reading books and checking out libraries etc. I found it frustrating how most people make fuzzy logic appear complicated, hard to handle and incorporate in code.
-Sure, there are frameworks that allow modelling of functions via GUI, but that's not a solution for a coder, right? Then there's a ton of mathematical research and other cruft that no normal person has time and patience to work through before trying to explore and applying things. Coming from this direction, there are also a number of script-ish (DSL) language frameworks that try to make the IF THEN ELSE pattern work (which I also tried in python, but gave it up because it just looks ugly).
-And yes, it's also possible to implement the whole thing completely in a functional style, but you really don't want to work with a recursive structure of 7+ steps by hand, trying not to miss a (..) along the way.
-Finally, most education on the subject emphasize sets and membership functions, but fail to mention the importance of the domain (or "universe of discourse"). It's easy to miss this point if you get lost with set operations and membership values, which are actually not that difficult once you can *play* and *explore* how these things look and work!
-
-### The Idea
-So, the idea is to have three parts that work together: domains, sets and rules. Each of these classes wrap additional logic around basic building blocks - Set gives logical operations to simple functions, Domain gives additional logic to numpy arrays and groups Sets together while Rule combines different Domains. You start modelling your system by defining your domain of interest. Then you think about where your interesting points are in that domain and look for a function that might do what you want. In general, fuzzy.functions map any value to [0,1], that's all. Simply wrap the function in a Set and assign it to the domain in question. Once assigned, you can plot that set and see if it actually looks how you imagined. Now that you have one or more sets, you also can start to combine them with set operations &, |, ~, etc. It's fairly straight forward.
-Finally, use the Rules to map input domain to output domain to actually control stuff.
-### Warning: Magic
-To make it possible to write fuzzy logic in the most pythonic and simplest way imaginable, it was necessary to employ some magic tricks that normally are discouraged, but at least there's no black magic involved (aka meta-programming etc.), so things are easy to debug if there is a problem. Most notably:
-* all functions are recursive closures (which makes it kinda hard to serialize things, if you really want to do that)
-* The main classes use a lot of dunder methods to implement their logic, which can be a bit daunting at first glance
-* Domain and Set uses an assignment trick to make it possible to instantiate Set() without passing domain and name over and over (yet still be explicit, just not the way one would normally expect). This also allows to call sets as Domain.attributes, which also normally shouldn't be possible (since they are technically not attributes). However, this allows interesting things like dangling sets (sets without domains) that can be freely combined with other sets to avoid cluttering of domain-namespaces and just have the resulting set assigned to a domain to work with.
-
-# Installation
-Just enter 
-`python -m pip install fuzzylogic`
-in a commandline prompt and you should be good to go!
-
-It's even more fun to experiment with it in jupyter lab ( https://jupyter.org/ ) :-)
-
-# Check out the Showcase!
-For complete examples and documentation how to work with fuzzylogic, check out https://github.com/amogorkon/fuzzylogic/blob/master/docs/Showcase.ipynb !
-
-Have fun!
-
-# Office Hours
-You can also contact me one-on-one! Please follow https://calendly.com/amogorkon/officehours to set up a meeting :-)
-
--- Anselm Kiefner
-
-
+Metadata-Version: 2.1
+Name: fuzzylogic
+Version: 1.4.0
+Summary: Fuzzy Logic for Python 3
+Home-page: https://github.com/amogorkon/fuzzylogic
+Author: Anselm Kiefner
+Author-email: fuzzylogic-pypi@anselm.kiefner.de
+License: MIT
+Keywords: fuzzy logic
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Manufacturing
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Requires-Python: >=3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Fuzzy Logic for Python 3
+
+[![license](https://img.shields.io/github/license/amogorkon/fuzzylogic)](https://github.com/amogorkon/fuzzylogic/blob/master/LICENSE)
+[![stars](https://img.shields.io/github/stars/amogorkon/fuzzylogic?style=plastic)](https://github.com/amogorkon/fuzzylogic/stargazers)
+[![forks](https://img.shields.io/github/forks/amogorkon/fuzzylogic?style=plastic)](https://github.com/amogorkon/fuzzylogic/network/members)
+[![Downloads](https://pepy.tech/badge/fuzzylogic)](https://pepy.tech/project/fuzzylogic)
+
+
+This is the fourth time I rebuilt this library from scratch to find the sweet spot between ease of use (beautiful is better than ugly!), testability (simple is better than complex!) and potential for performance optimization (practicality beats purity!). 
+
+### Why a new library?
+The first time I was confronted with fuzzy logic, I fell in love with the concept, but after reading books and checking out libraries etc. I found it frustrating how most people make fuzzy logic appear complicated, hard to handle and incorporate in code.
+Sure, there are frameworks that allow modelling of functions via GUI, but that's not a solution for a coder, right? Then there's a ton of mathematical research and other cruft that no normal person has time and patience to work through before trying to explore and applying things. Coming from this direction, there are also a number of script-ish (DSL) language frameworks that try to make the IF THEN ELSE pattern work (which I also tried in python, but gave it up because it just looks ugly).
+And yes, it's also possible to implement the whole thing completely in a functional style, but you really don't want to work with a recursive structure of 7+ steps by hand, trying not to miss a (..) along the way.
+Finally, most education on the subject emphasize sets and membership functions, but fail to mention the importance of the domain (or "universe of discourse"). It's easy to miss this point if you get lost with set operations and membership values, which are actually not that difficult once you can *play* and *explore* how these things look and work!
+
+### The Idea
+So, the idea is to have three parts that work together: domains, sets and rules. Each of these classes wrap additional logic around basic building blocks - Set gives logical operations to simple functions, Domain gives additional logic to numpy arrays and groups Sets together while Rule combines different Domains. You start modelling your system by defining your domain of interest. Then you think about where your interesting points are in that domain and look for a function that might do what you want. In general, fuzzy.functions map any value to [0,1], that's all. Simply wrap the function in a Set and assign it to the domain in question. Once assigned, you can plot that set and see if it actually looks how you imagined. Now that you have one or more sets, you also can start to combine them with set operations &, |, ~, etc. It's fairly straight forward.
+Finally, use the Rules to map input domain to output domain to actually control stuff.
+### Warning: Magic
+To make it possible to write fuzzy logic in the most pythonic and simplest way imaginable, it was necessary to employ some magic tricks that normally are discouraged, but at least there's no black magic involved (aka meta-programming etc.), so things are easy to debug if there is a problem. Most notably:
+* all functions are recursive closures (which makes it kinda hard to serialize things, if you really want to do that)
+* The main classes use a lot of dunder methods to implement their logic, which can be a bit daunting at first glance
+* Domain and Set uses an assignment trick to make it possible to instantiate Set() without passing domain and name over and over (yet still be explicit, just not the way one would normally expect). This also allows to call sets as Domain.attributes, which also normally shouldn't be possible (since they are technically not attributes). However, this allows interesting things like dangling sets (sets without domains) that can be freely combined with other sets to avoid cluttering of domain-namespaces and just have the resulting set assigned to a domain to work with.
+
+# Installation
+Just enter 
+`python -m pip install fuzzylogic`
+in a commandline prompt and you should be good to go!
+
+It's even more fun to experiment with it in [Jupyter Lab](https://jupyter.org) :-)
+
+# Documentation
+Thanks to [Atul Kushwaha](https://github.com/coderatul), we now have an amazing [documentation](https://fuzzylogic.readthedocs.io/en/latest/) including our [Showcase](https://github.com/amogorkon/fuzzylogic/blob/master/docs/Showcase.ipynb) - check it out!
+
+# Office Hours
+You can also contact me one-on-one! Please follow https://calendly.com/amogorkon/officehours to set up a meeting :-)
+
+# Office Hours
+You can also contact me one-on-one! Check my [office hours](https://calendly.com/amogorkon/officehours) to set up a meeting :-)
+
+-- Anselm Kiefner
```

### Comparing `fuzzylogic-1.2.0/README.md` & `fuzzylogic-1.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-# Fuzzy Logic for Python 3
-
-[![license](https://img.shields.io/github/license/amogorkon/fuzzylogic)](https://github.com/amogorkon/fuzzylogic/blob/master/LICENSE)
-[![stars](https://img.shields.io/github/stars/amogorkon/fuzzylogic?style=plastic)](https://github.com/amogorkon/fuzzylogic/stargazers)
-[![forks](https://img.shields.io/github/forks/amogorkon/fuzzylogic?style=plastic)](https://github.com/amogorkon/fuzzylogic/network/members)
-[![Downloads](https://pepy.tech/badge/fuzzylogic)](https://pepy.tech/project/fuzzylogic)
-
-
-This is the fourth time I rebuilt this library from scratch to find the sweet spot between ease of use (beautiful is better than ugly!), testability (simple is better than complex!) and potential for performance optimization (practicality beats purity!). 
-
-### Why a new library?
-The first time I was confronted with fuzzy logic, I fell in love with the concept, but after reading books and checking out libraries etc. I found it frustrating how most people make fuzzy logic appear complicated, hard to handle and incorporate in code.
-Sure, there are frameworks that allow modelling of functions via GUI, but that's not a solution for a coder, right? Then there's a ton of mathematical research and other cruft that no normal person has time and patience to work through before trying to explore and applying things. Coming from this direction, there are also a number of script-ish (DSL) language frameworks that try to make the IF THEN ELSE pattern work (which I also tried in python, but gave it up because it just looks ugly).
-And yes, it's also possible to implement the whole thing completely in a functional style, but you really don't want to work with a recursive structure of 7+ steps by hand, trying not to miss a (..) along the way.
-Finally, most education on the subject emphasize sets and membership functions, but fail to mention the importance of the domain (or "universe of discourse"). It's easy to miss this point if you get lost with set operations and membership values, which are actually not that difficult once you can *play* and *explore* how these things look and work!
-
-### The Idea
-So, the idea is to have three parts that work together: domains, sets and rules. Each of these classes wrap additional logic around basic building blocks - Set gives logical operations to simple functions, Domain gives additional logic to numpy arrays and groups Sets together while Rule combines different Domains. You start modelling your system by defining your domain of interest. Then you think about where your interesting points are in that domain and look for a function that might do what you want. In general, fuzzy.functions map any value to [0,1], that's all. Simply wrap the function in a Set and assign it to the domain in question. Once assigned, you can plot that set and see if it actually looks how you imagined. Now that you have one or more sets, you also can start to combine them with set operations &, |, ~, etc. It's fairly straight forward.
-Finally, use the Rules to map input domain to output domain to actually control stuff.
-### Warning: Magic
-To make it possible to write fuzzy logic in the most pythonic and simplest way imaginable, it was necessary to employ some magic tricks that normally are discouraged, but at least there's no black magic involved (aka meta-programming etc.), so things are easy to debug if there is a problem. Most notably:
-* all functions are recursive closures (which makes it kinda hard to serialize things, if you really want to do that)
-* The main classes use a lot of dunder methods to implement their logic, which can be a bit daunting at first glance
-* Domain and Set uses an assignment trick to make it possible to instantiate Set() without passing domain and name over and over (yet still be explicit, just not the way one would normally expect). This also allows to call sets as Domain.attributes, which also normally shouldn't be possible (since they are technically not attributes). However, this allows interesting things like dangling sets (sets without domains) that can be freely combined with other sets to avoid cluttering of domain-namespaces and just have the resulting set assigned to a domain to work with.
-
-# Installation
-Just enter 
-`python -m pip install fuzzylogic`
-in a commandline prompt and you should be good to go!
-
-It's even more fun to experiment with it in jupyter lab ( https://jupyter.org/ ) :-)
-
-# Check out the Showcase!
-For complete examples and documentation how to work with fuzzylogic, check out https://github.com/amogorkon/fuzzylogic/blob/master/docs/Showcase.ipynb !
-
-Have fun!
-
-# Office Hours
-You can also contact me one-on-one! Please follow https://calendly.com/amogorkon/officehours to set up a meeting :-)
-
--- Anselm Kiefner
+# Fuzzy Logic for Python 3
+
+[![license](https://img.shields.io/github/license/amogorkon/fuzzylogic)](https://github.com/amogorkon/fuzzylogic/blob/master/LICENSE)
+[![stars](https://img.shields.io/github/stars/amogorkon/fuzzylogic?style=plastic)](https://github.com/amogorkon/fuzzylogic/stargazers)
+[![forks](https://img.shields.io/github/forks/amogorkon/fuzzylogic?style=plastic)](https://github.com/amogorkon/fuzzylogic/network/members)
+[![Downloads](https://pepy.tech/badge/fuzzylogic)](https://pepy.tech/project/fuzzylogic)
+
+
+This is the fourth time I rebuilt this library from scratch to find the sweet spot between ease of use (beautiful is better than ugly!), testability (simple is better than complex!) and potential for performance optimization (practicality beats purity!). 
+
+### Why a new library?
+The first time I was confronted with fuzzy logic, I fell in love with the concept, but after reading books and checking out libraries etc. I found it frustrating how most people make fuzzy logic appear complicated, hard to handle and incorporate in code.
+Sure, there are frameworks that allow modelling of functions via GUI, but that's not a solution for a coder, right? Then there's a ton of mathematical research and other cruft that no normal person has time and patience to work through before trying to explore and applying things. Coming from this direction, there are also a number of script-ish (DSL) language frameworks that try to make the IF THEN ELSE pattern work (which I also tried in python, but gave it up because it just looks ugly).
+And yes, it's also possible to implement the whole thing completely in a functional style, but you really don't want to work with a recursive structure of 7+ steps by hand, trying not to miss a (..) along the way.
+Finally, most education on the subject emphasize sets and membership functions, but fail to mention the importance of the domain (or "universe of discourse"). It's easy to miss this point if you get lost with set operations and membership values, which are actually not that difficult once you can *play* and *explore* how these things look and work!
+
+### The Idea
+So, the idea is to have three parts that work together: domains, sets and rules. Each of these classes wrap additional logic around basic building blocks - Set gives logical operations to simple functions, Domain gives additional logic to numpy arrays and groups Sets together while Rule combines different Domains. You start modelling your system by defining your domain of interest. Then you think about where your interesting points are in that domain and look for a function that might do what you want. In general, fuzzy.functions map any value to [0,1], that's all. Simply wrap the function in a Set and assign it to the domain in question. Once assigned, you can plot that set and see if it actually looks how you imagined. Now that you have one or more sets, you also can start to combine them with set operations &, |, ~, etc. It's fairly straight forward.
+Finally, use the Rules to map input domain to output domain to actually control stuff.
+### Warning: Magic
+To make it possible to write fuzzy logic in the most pythonic and simplest way imaginable, it was necessary to employ some magic tricks that normally are discouraged, but at least there's no black magic involved (aka meta-programming etc.), so things are easy to debug if there is a problem. Most notably:
+* all functions are recursive closures (which makes it kinda hard to serialize things, if you really want to do that)
+* The main classes use a lot of dunder methods to implement their logic, which can be a bit daunting at first glance
+* Domain and Set uses an assignment trick to make it possible to instantiate Set() without passing domain and name over and over (yet still be explicit, just not the way one would normally expect). This also allows to call sets as Domain.attributes, which also normally shouldn't be possible (since they are technically not attributes). However, this allows interesting things like dangling sets (sets without domains) that can be freely combined with other sets to avoid cluttering of domain-namespaces and just have the resulting set assigned to a domain to work with.
+
+# Installation
+Just enter 
+`python -m pip install fuzzylogic`
+in a commandline prompt and you should be good to go!
+
+It's even more fun to experiment with it in [Jupyter Lab](https://jupyter.org) :-)
+
+# Documentation
+Thanks to [Atul Kushwaha](https://github.com/coderatul), we now have an amazing [documentation](https://fuzzylogic.readthedocs.io/en/latest/) including our [Showcase](https://github.com/amogorkon/fuzzylogic/blob/master/docs/Showcase.ipynb) - check it out!
+
+# Office Hours
+You can also contact me one-on-one! Please follow https://calendly.com/amogorkon/officehours to set up a meeting :-)
+
+# Office Hours
+You can also contact me one-on-one! Check my [office hours](https://calendly.com/amogorkon/officehours) to set up a meeting :-)
+
+-- Anselm Kiefner
```

### Comparing `fuzzylogic-1.2.0/setup.py` & `fuzzylogic-1.4.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 import os
+import pathlib
 import sys
 
+from setuptools import find_packages, setup
+
 here = os.path.abspath(os.path.dirname(__file__))
 src = os.path.join(here, "src/fuzzylogic")
 sys.path.append(src)
 
-from setuptools import find_packages, setup
-
-meta = {
-    "name": "fuzzylogic",
-    "description": "Fuzzy Logic for Python 3",
-    "license": "MIT",
-    "url": "https://github.com/amogorkon/fuzzylogic",
-    "version": "1.2.0",
-    "author": "Anselm Kiefner",
-    "author_email": "fuzzylogic-pypi@anselm.kiefner.de",
-    "python_requires": ">=3.7",
-    "keywords": [
-        "fuzzy logic",
-    ],
-    "classifiers": [
-        "Development Status :: 4 - Beta",
-        "Intended Audience :: Developers",
-        "Intended Audience :: Education",
-        "Intended Audience :: Manufacturing",
-        "Intended Audience :: Science/Research",
-        "Natural Language :: English",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3 :: Only",
-        "Topic :: Scientific/Engineering :: Artificial Intelligence",
-        "Topic :: Scientific/Engineering :: Mathematics",
-        "Topic :: Scientific/Engineering :: Information Analysis",
-    ],
-}
-
 
-with open("README.md") as f:
-    LONG_DESCRIPTION = f.read()
+__license__ = "MIT"
+__version__ = "1.4.0"
+__author__ = "Anselm Kiefner"
+__contact__ = "fuzzylogic-pypi@anselm.kiefner.de"
+
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Education",
+    "Intended Audience :: Manufacturing",
+    "Intended Audience :: Science/Research",
+    "Natural Language :: English",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3 :: Only",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+    "Topic :: Scientific/Engineering :: Mathematics",
+    "Topic :: Scientific/Engineering :: Information Analysis",
+]
 
 setup(
     packages=find_packages(where="src"),
     package_dir={"": "src"},
-    long_description=LONG_DESCRIPTION,
+    long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     zip_safe=False,
-    **meta
+    name="fuzzylogic",
+    description="Fuzzy Logic for Python 3",
+    license=__license__,
+    url="https://github.com/amogorkon/fuzzylogic",
+    version=__version__,
+    author=__author__,
+    author_email=__contact__,
+    python_requires=">=3.12",
+    keywords="fuzzy logic",
+    classifiers=classifiers,
 )
```

### Comparing `fuzzylogic-1.2.0/src/fuzzylogic/classes.py` & `fuzzylogic-1.4.0/src/fuzzylogic/classes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,480 +1,498 @@
-"""
-Domain, Set and Rule classes for fuzzy logic.
-
-Primary abstractions for recursive functions and arrays, 
-adding logical operaitons for easier handling.
-"""
-
-from logging import warn
-
-import matplotlib.pyplot as plt
-import numpy as np
-
-from .combinators import MAX, MIN, bounded_sum, product, simple_disjoint_sum
-from .functions import inv, normalize
-
-
-class FuzzyWarning(UserWarning):
-    """Extra Exception so that user code can filter exceptions specific to this lib."""
-
-    pass
-
-
-class Domain:
-    """
-    A domain is a 'measurable' dimension of 'real' values like temperature.
-
-    There must be a lower and upper limit and a resolution (the size of steps)
-    specified.
-
-    Fuzzysets are defined within one such domain and are only meaningful
-    while considered within their domain ('apples and bananas').
-    To operate with sets across domains, there needs to be a mapping.
-
-    The sets are accessed as attributes of the domain like
-    >>> temp = Domain('temperature', 0, 100)
-    >>> temp.hot = Set(lambda x: 0)
-    >>> temp.hot(5)
-    0
-
-    It is possible now to call derived sets without assignment first!
-    >>> from .hedges import very
-    >>> (very(~temp.hot) | ~very(temp.hot))(2)
-    1
-
-    You MUST NOT add arbitrary attributes to an *instance* of Domain - you can
-    however subclass or modify the class itself. If you REALLY have to add attributes,
-    make sure to "whitelist" it in __slots__ first.
-
-    Use the Domain by calling it with the value in question. This returns a
-    dictionary with the degrees of membership per set. You MAY override __call__
-    in a subclass to enable concurrent evaluation for performance improvement.
-    """
-
-    __slots__ = ["_name", "_low", "_high", "_res", "_sets"]
-
-    def __init__(self, name, low, high, *, res=1, sets: dict = None):
-        """Define a domain."""
-        assert low < high, "higher bound must be greater than lower."
-        assert res > 0, "resolution can't be negative or zero"
-        self._name = name
-        self._high = high
-        self._low = low
-        self._res = res
-        self._sets = {} if sets is None else sets  # Name: Set(Function())
-
-    def __call__(self, X):
-        """Pass a value to all sets of the domain and return a dict with results."""
-        if isinstance(X, np.ndarray):
-            if any(not (self._low <= x <= self._high) for x in X):
-                raise FuzzyWarning("Value in array is outside of defined range!")
-            res = {}
-            for s in self._sets.values():
-                vector = np.vectorize(s.func, otypes=[float])
-                res[s] = vector(X)
-            return res
-        if not (self._low <= X <= self._high):
-            warn(f"{X} is outside of domain!")
-        return {s: s.func(X) for name, s in self._sets.items()}
-
-    def __str__(self):
-        """Return a string to print()."""
-        return self._name
-
-    def __repr__(self):
-        """Return a string so that eval(repr(Domain)) == Domain."""
-        return f"Domain('{self._name}', {self._low}, {self._high}, res={self._res}, sets={self._sets})"
-
-    def __eq__(self, other):
-        """Test equality of two domains."""
-        return all(
-            [
-                self._name == other._name,
-                self._low == other._low,
-                self._high == other._high,
-                self._res == other._res,
-                self._sets == other._sets,
-            ]
-        )
-
-    def __hash__(self):
-        return id(self)
-
-    def __getattr__(self, name):
-        """Get the value of an attribute. Is called after __getattribute__ is called with an AttributeError."""
-        if name in self._sets:
-            return self._sets[name]
-        else:
-            raise AttributeError(f"{name} is not a set or attribute")
-
-    def __setattr__(self, name, value):
-        """Define a set within a domain or assign a value to a domain attribute."""
-        # It's a domain attr
-        if name in self.__slots__:
-            object.__setattr__(self, name, value)
-        # We've got a fuzzyset
-        else:
-            assert str.isidentifier(name), f"{name} must be an identifier."
-            if not isinstance(value, Set):
-                # Often useful to just assign a function for simple sets..
-                value = Set(value)
-            # However, we need the abstraction if we want to use Superfuzzysets (derived sets).
-            self._sets[name] = value
-            value.domain = self
-            value.name = name
-
-    def __delattr__(self, name):
-        """Delete a fuzzy set from the domain."""
-        if name in self._sets:
-            del self._sets[name]
-        else:
-            raise FuzzyWarning("Trying to delete a regular attr, this needs extra care.")
-
-    @property
-    def range(self):
-        """Return an arange object with the domain's specifics.
-
-        This is used to conveniently iterate over all possible values
-        for plotting etc.
-
-        High upper bound is INCLUDED unlike range.
-        """
-        return np.arange(self._low, self._high + self._res, self._res)
-
-    def min(self, x):
-        """Standard way to get the min over all membership funcs.
-
-        It's not just more convenient but also faster than
-        to calculate all results, construct a dict, unpack the dict
-        and calculate the min from that.
-        """
-        return min(f(x) for f in self._sets.values())
-
-    def max(self, x):
-        """Standard way to get the max over all membership funcs."""
-        return max(f(x) for f in self._sets.values())
-
-
-class Set:
-    """
-    A fuzzyset defines a 'region' within a domain.
-
-    The associated membership function defines 'how much' a given value is
-    inside this region - how 'true' the value is.
-
-    Sets and functions MUST NOT be mixed because functions don't have
-    the methods of the sets needed for the logic.
-
-    Sets that are returned from one of the operations are 'derived sets' or
-    'Superfuzzysets' according to Zadeh.
-
-    Note that most checks are merely assertions that can be optimized away.
-    DO NOT RELY on these checks and use tests to make sure that only valid calls are made.
-
-    This class uses the classical MIN/MAX operators for AND/OR. To use different operators, simply subclass and
-    replace the __and__ and __or__ functions. However, be careful not to mix the classes logically,
-    since it might be confusing which operator will be used (left/right binding).
-
-    """
-
-    name = None  # these are set on assignment to the domain! DO NOT MODIFY
-    domain = None
-
-    def __init__(self, func: callable, *, name=None, domain=None):
-        self.func = func
-        self.domain = domain
-        self.name = name
-        self.__center_of_gravity = None
-
-    def __call__(self, x):
-        return self.func(x)
-
-    def __invert__(self):
-        """Return a new set with 1 - function."""
-        return Set(inv(self.func), domain=self.domain)
-
-    def __neg__(self):
-        """Synonyme for invert."""
-        return Set(inv(self.func), domain=self.domain)
-
-    def __and__(self, other):
-        """Return a new set with modified function."""
-        assert self.domain == other.domain
-        return Set(MIN(self.func, other.func), domain=self.domain)
-
-    def __or__(self, other):
-        """Return a new set with modified function."""
-        assert self.domain == other.domain
-        return Set(MAX(self.func, other.func), domain=self.domain)
-
-    def __mul__(self, other):
-        """Return a new set with modified function."""
-        assert self.domain == other.domain
-        return Set(product(self.func, other.func), domain=self.domain)
-
-    def __add__(self, other):
-        """Return a new set with modified function."""
-        assert self.domain == other.domain
-        return Set(bounded_sum(self.func, other.func), domain=self.domain)
-
-    def __xor__(self, other):
-        """Return a new set with modified function."""
-        assert self.domain == other.domain
-        return Set(simple_disjoint_sum(self.func, other.func), domain=self.domain)
-
-    def __pow__(self, power):
-        """Return a new set with modified function."""
-        # FYI: pow is used with hedges
-        return Set(lambda x: pow(self.func(x), power), domain=self.domain)
-
-    def __eq__(self, other):
-        """A set is equal with another if both return the same values over the same range."""
-        if self.domain is None or other.domain is None:
-            # It would require complete AST analysis to check whether both Sets
-            # represent the same recursive functions -
-            # additionally, there are infinitely many mathematically equivalent
-            # functions that don't have the same bytecode...
-            raise FuzzyWarning("Impossible to determine.")
-        else:
-            # however, if domains ARE assigned (whether or not it's the same domain),
-            # we simply can check if they map to the same values
-            return np.array_equal(self.array(), other.array())
-
-    def __le__(self, other):
-        """If this <= other, it means this is a subset of the other."""
-        assert self.domain == other.domain
-        if self.domain is None or other.domain is None:
-            raise FuzzyWarning("Can't compare without Domains.")
-        return all(np.less_equal(self.array(), other.array()))
-
-    def __lt__(self, other):
-        """If this < other, it means this is a proper subset of the other."""
-        assert self.domain == other.domain
-        if self.domain is None or other.domain is None:
-            raise FuzzyWarning("Can't compare without Domains.")
-        return all(np.less(self.array(), other.array()))
-
-    def __ge__(self, other):
-        """If this >= other, it means this is a superset of the other."""
-        assert self.domain == other.domain
-        if self.domain is None or other.domain is None:
-            raise FuzzyWarning("Can't compare without Domains.")
-        return all(np.greater_equal(self.array(), other.array()))
-
-    def __gt__(self, other):
-        """If this > other, it means this is a proper superset of the other."""
-        assert self.domain == other.domain
-        if self.domain is None or other.domain is None:
-            raise FuzzyWarning("Can't compare without Domains.")
-        return all(np.greater(self.array(), other.array()))
-
-    def __len__(self):
-        """Number of membership values in the set, defined by bounds and resolution of domain."""
-        if self.domain is None:
-            raise FuzzyWarning("No domain.")
-        return len(self.array())
-
-    @property
-    def cardinality(self):
-        """The sum of all values in the set."""
-        if self.domain is None:
-            raise FuzzyWarning("No domain.")
-        return sum(self.array())
-
-    @property
-    def relative_cardinality(self):
-        """Relative cardinality is the sum of all membership values by number of all values."""
-        if self.domain is None:
-            raise FuzzyWarning("No domain.")
-        if len(self) == 0:
-            # this is highly unlikely and only possible with res=inf but still..
-            raise FuzzyWarning("The domain has no element.")
-        return self.cardinality() / len(self)
-
-    def concentrated(self):
-        """
-        Alternative to hedge "very".
-
-        Returns a new set that has a reduced amount of values the set includes and to dampen the
-        membership of many values.
-        """
-        return Set(lambda x: self.func(x) ** 2, domain=self.domain)
-
-    def intensified(self):
-        """
-        Alternative to hedges.
-
-        Returns a new set where the membership of values are increased that
-        already strongly belong to the set and dampened the rest.
-        """
-
-        def f(x):
-            if x < 0.5:
-                return 2 * self.func(x) ** 2
-            else:
-                return 1 - 2 * (1 - self.func(x) ** 2)
-
-        return Set(f, domain=self.domain)
-
-    def dilated(self):
-        """Expand the set with more values and already included values are enhanced."""
-        return Set(lambda x: self.func(x) ** 1.0 / 2.0, domain=self.domain)
-
-    def multiplied(self, n):
-        """Multiply with a constant factor, changing all membership values."""
-        return Set(lambda x: self.func(x) * n, domain=self)
-
-    def plot(self):
-        """Graph the set in the given domain."""
-        if self.domain is None:
-            raise FuzzyWarning("No domain assigned, cannot plot.")
-        R = self.domain.range
-        V = [self.func(x) for x in R]
-        plt.plot(R, V)
-
-    def array(self):
-        """Return an array of all values for this set within the given domain."""
-        if self.domain is None:
-            raise FuzzyWarning("No domain assigned.")
-        return np.fromiter((self.func(x) for x in self.domain.range), float)
-
-    @property
-    def center_of_gravity(self):
-        """Return the center of gravity for this distribution, within the given domain."""
-        if self.__center_of_gravity is not None:
-            return self.__center_of_gravity
-
-        weights = self.array()
-        if sum(weights) == 0:
-            return 0
-        cog = np.average(np.arange(len(weights)), weights=weights)
-        self.__center_of_gravity = cog
-        return cog
-
-    def __repr__(self):
-        """
-        Return a string representation of the Set that reconstructs the set with eval().
-
-        *******
-        Current implementation does NOT work correctly.
-
-        This is harder than expected since all functions are (recursive!) closures which
-        can't simply be pickled. If this functionality really is needed, all functions
-        would have to be peppered with closure-returning overhead such as
-
-        def create_closure_and_function(*args):
-            func = None
-            def create_function_closure():
-                return func
-
-            closure = create_function_closure.__closure__
-            func = types.FunctionType(*args[:-1] + [closure])
-            return func
-        """
-        return f"Set({self.func})"
-
-    def __str__(self):
-        """Return a string for print()."""
-        if self.name is None and self.domain is None:
-            return f"dangling Set({self.func})"
-        else:
-            return f"{self.domain._name}.{self.name}"
-
-    def normalized(self):
-        """Return a set that is normalized *for this domain* with 1 as max."""
-        if self.domain is None:
-            raise FuzzyWarning("Can't normalize without domain.")
-        return Set(normalize(max(self.array()), self.func), domain=self.domain)
-
-    def __hash__(self):
-        return id(self)
-
-
-class Rule:
-    """
-    A collection of bound sets that span a multi-dimensional space of their respective domains.
-    """
-
-    def __init__(self, conditions, func=None):
-        self.conditions = {frozenset(C): O for C, O, in conditions.items()}
-        self.func = func
-
-    def __add__(self, other):
-        assert isinstance(other, Rule)
-        return Rule({**self.conditions, **other.conditions})
-
-    def __radd__(self, other):
-        assert isinstance(other, (Rule, int))
-        # we're using sum(..)
-        if isinstance(other, int):
-            return self
-        return Rule({**self.conditions, **other.conditions})
-
-    def __or__(self, other):
-        assert isinstance(other, Rule)
-        return Rule({**self.conditions, **other.conditions})
-
-    def __eq__(self, other):
-        return self.conditions == other.conditions
-
-    def __getitem__(self, key):
-        return self.conditions[frozenset(key)]
-
-    def __call__(self, args: "dict[Domain, float]", method="cog"):
-        """Calculate the infered value based on different methods.
-        Default is center of gravity (cog).
-        """
-        assert len(args) == max(
-            len(c) for c in self.conditions.keys()
-        ), "Number of values must correspond to the number of domains defined as conditions!"
-        assert isinstance(args, dict), "Please make sure to pass in the values as a dictionary."
-        if method == "cog":
-            assert (
-                len({C.domain for C in self.conditions.values()}) == 1
-            ), "For CoG, all conditions must have the same target domain."
-            actual_values = {f: f(args[f.domain]) for S in self.conditions.keys() for f in S}
-
-            weights = []
-            for K, v in self.conditions.items():
-                x = min((actual_values[k] for k in K if k in actual_values), default=0)
-                if x > 0:
-                    weights.append((v, x))
-
-            if not weights:
-                return None
-            target_domain = list(self.conditions.values())[0].domain
-            index = sum(v.center_of_gravity * x for v, x in weights) / sum(x for v, x in weights)
-            return (target_domain._high - target_domain._low) / len(
-                target_domain.range
-            ) * index + target_domain._low
-
-
-def rule_from_table(table: str, references: dict):
-    """Turn a (2D) string table into a Rule of fuzzy sets.
-
-    ATTENTION: This will eval() all strings in the table.
-    This can pose a potential security risk if the table originates from an untrusted source.
-
-    Using a table will considerably reduce the amount of required text to describe all rules,
-    but there are two critical drawbacks: Tables are limited to 2 input variables (2D) and they are strings,
-    with no IDE support. It is strongly recommended to check the Rule output for consistency.
-    For example, a trailing "." will result in a SyntaxError when eval()ed.
-    """
-    import io
-    from itertools import product
-
-    import pandas as pd
-
-    df = pd.read_table(io.StringIO(table), delim_whitespace=True)
-    D = {}
-    for x, y in product(range(len(df.index)), range(len(df.columns))):
-        D[(eval(df.index[x].strip(), references), eval(df.columns[y].strip(), references))] = eval(
-            df.iloc[x, y], references
-        )
-    return Rule(D)
-
-
-if __name__ == "__main__":
-    import doctest
-
-    doctest.testmod()
+"""
+Domain, Set and Rule classes for fuzzy logic.
+
+Primary abstractions for recursive functions and arrays,
+adding logical operaitons for easier handling.
+"""
+
+from typing import Callable
+
+import matplotlib.pyplot as plt
+import numpy as np
+
+from .combinators import MAX, MIN, bounded_sum, product, simple_disjoint_sum
+from .functions import inv, normalize
+
+
+class FuzzyWarning(UserWarning):
+    """Extra Exception so that user code can filter exceptions specific to this lib."""
+
+    pass
+
+
+class Domain:
+    """
+    A domain is a 'measurable' dimension of 'real' values like temperature.
+
+    There must be a lower and upper limit and a resolution (the size of steps)
+    specified.
+
+    Fuzzysets are defined within one such domain and are only meaningful
+    while considered within their domain ('apples and bananas').
+    To operate with sets across domains, there needs to be a mapping.
+
+    The sets are accessed as attributes of the domain like
+    >>> temp = Domain('temperature', 0, 100)
+    >>> temp.hot = Set(lambda x: 0)
+    >>> temp.hot(5)
+    0
+
+    It is possible now to call derived sets without assignment first!
+    >>> from .hedges import very
+    >>> (very(~temp.hot) | ~very(temp.hot))(2)
+    1
+
+    You MUST NOT add arbitrary attributes to an *instance* of Domain - you can
+    however subclass or modify the class itself. If you REALLY have to add attributes,
+    make sure to "whitelist" it in __slots__ first.
+
+    Use the Domain by calling it with the value in question. This returns a
+    dictionary with the degrees of membership per set. You MAY override __call__
+    in a subclass to enable concurrent evaluation for performance improvement.
+    """
+
+    __slots__ = ["_name", "_low", "_high", "_res", "_sets"]
+
+    def __init__(
+        self,
+        name: str,
+        low: float | int,
+        high: float | int,
+        res: float | int = 1,
+        sets: dict | None = None,
+    ) -> None:
+        """Define a domain."""
+        assert low < high, "higher bound must be greater than lower."
+        assert res > 0, "resolution can't be negative or zero"
+        self._name = name
+        self._high = high
+        self._low = low
+        self._res = res
+        self._sets = {} if sets is None else sets  # Name: Set(Function())
+
+    def __call__(self, x):
+        """Pass a value to all sets of the domain and return a dict with results."""
+        if not (self._low <= x <= self._high):
+            raise FuzzyWarning(f"{x} is outside of domain!")
+        return {name: s.func(x) for name, s in self._sets.items()}
+
+    def __str__(self):
+        """Return a string to print()."""
+        return self._name
+
+    def __repr__(self):
+        """Return a string so that eval(repr(Domain)) == Domain."""
+        return f"Domain('{self._name}', {self._low}, {self._high}, res={self._res}, sets={self._sets})"
+
+    def __eq__(self, other):
+        """Test equality of two domains."""
+        return all(
+            [
+                self._name == other._name,
+                self._low == other._low,
+                self._high == other._high,
+                self._res == other._res,
+                self._sets == other._sets,
+            ]
+        )
+
+    def __hash__(self):
+        return id(self)
+
+    def __getattr__(self, name):
+        """Get the value of an attribute. Called after __getattribute__ is called with an AttributeError."""
+        if name in self._sets:
+            return self._sets[name]
+        else:
+            raise AttributeError(f"{name} is not a set or attribute")
+
+    def __setattr__(self, name, value):
+        """Define a set within a domain or assign a value to a domain attribute."""
+        # It's a domain attr
+        if name in self.__slots__:
+            object.__setattr__(self, name, value)
+        # We've got a fuzzyset
+        else:
+            assert str.isidentifier(name), f"{name} must be an identifier."
+            if not isinstance(value, Set):
+                # Often useful to just assign a function for simple sets..
+                value = Set(value)
+            # However, we need the abstraction if we want to use Superfuzzysets (derived sets).
+            self._sets[name] = value
+            value.domain = self
+            value.name = name
+
+    def __delattr__(self, name):
+        """Delete a fuzzy set from the domain."""
+        if name in self._sets:
+            del self._sets[name]
+        else:
+            raise FuzzyWarning("Trying to delete a regular attr, this needs extra care.")
+
+    @property
+    def range(self):
+        """Return an arange object with the domain's specifics.
+
+        This is used to conveniently iterate over all possible values
+        for plotting etc.
+
+        High upper bound is INCLUDED unlike range.
+        """
+        if int(self._res) == self._res:
+            return np.arange(self._low, self._high + self._res, int(self._res))
+        else:
+            return np.linspace(self._low, self._high, int((self._high - self._low) / self._res) + 1)
+
+    def min(self, x):
+        """Standard way to get the min over all membership funcs.
+
+        It's not just more convenient but also faster than
+        to calculate all results, construct a dict, unpack the dict
+        and calculate the min from that.
+        """
+        return min((f(x) for f in self._sets.values()), default=0)
+
+    def max(self, x):
+        """Standard way to get the max over all membership funcs."""
+        return max((f(x) for f in self._sets.values()), default=0)
+
+
+class Set:
+    """
+    A fuzzyset defines a 'region' within a domain.
+
+    The associated membership function defines 'how much' a given value is
+    inside this region - how 'true' the value is.
+
+    Sets and functions MUST NOT be mixed because functions don't have
+    the methods of the sets needed for the logic.
+
+    Sets that are returned from one of the operations are 'derived sets' or
+    'Superfuzzysets' according to Zadeh.
+
+    Note that most checks are merely assertions that can be optimized away.
+    DO NOT RELY on these checks and use tests to make sure that only valid calls are made.
+
+    This class uses the classical MIN/MAX operators for AND/OR. To use different operators, simply subclass &
+    replace the __and__ and __or__ functions. However, be careful not to mix the classes logically,
+    since it might be confusing which operator will be used (left/right binding).
+
+    """
+
+    name = None  # these are set on assignment to the domain! DO NOT MODIFY
+    domain = None
+
+    def __init__(self, func: Callable, *, name: str | None = None, domain: Domain | None = None):
+        self.func = func
+        self.domain = domain
+        self.name = name
+        self.__center_of_gravity = None
+
+    def __call__(self, x):
+        return self.func(x)
+
+    def __invert__(self):
+        """Return a new set with 1 - function."""
+        return Set(inv(self.func), domain=self.domain)
+
+    def __neg__(self):
+        """Synonyme for invert."""
+        return Set(inv(self.func), domain=self.domain)
+
+    def __and__(self, other):
+        """Return a new set with modified function."""
+        assert self.domain == other.domain
+        return Set(MIN(self.func, other.func), domain=self.domain)
+
+    def __or__(self, other):
+        """Return a new set with modified function."""
+        assert self.domain == other.domain
+        return Set(MAX(self.func, other.func), domain=self.domain)
+
+    def __mul__(self, other):
+        """Return a new set with modified function."""
+        assert self.domain == other.domain
+        return Set(product(self.func, other.func), domain=self.domain)
+
+    def __add__(self, other):
+        """Return a new set with modified function."""
+        assert self.domain == other.domain
+        return Set(bounded_sum(self.func, other.func), domain=self.domain)
+
+    def __xor__(self, other):
+        """Return a new set with modified function."""
+        assert self.domain == other.domain
+        return Set(simple_disjoint_sum(self.func, other.func), domain=self.domain)
+
+    def __pow__(self, power):
+        """Return a new set with modified function."""
+        # FYI: pow is used with hedges
+        return Set(lambda x: pow(self.func(x), power), domain=self.domain)
+
+    def __eq__(self, other):
+        """A set is equal with another if both return the same values over the same range."""
+        if self.domain is None or other.domain is None:
+            # It would require complete AST analysis to check whether both Sets
+            # represent the same recursive functions -
+            # additionally, there are infinitely many mathematically equivalent
+            # functions that don't have the same bytecode...
+            raise FuzzyWarning("Impossible to determine.")
+        else:
+            # however, if domains ARE assigned (whether or not it's the same domain),
+            # we simply can check if they map to the same values
+            return np.array_equal(self.array(), other.array())
+
+    def __le__(self, other):
+        """If this <= other, it means this is a subset of the other."""
+        assert self.domain == other.domain
+        if self.domain is None or other.domain is None:
+            raise FuzzyWarning("Can't compare without Domains.")
+        return all(np.less_equal(self.array(), other.array()))
+
+    def __lt__(self, other):
+        """If this < other, it means this is a proper subset of the other."""
+        assert self.domain == other.domain
+        if self.domain is None or other.domain is None:
+            raise FuzzyWarning("Can't compare without Domains.")
+        return all(np.less(self.array(), other.array()))
+
+    def __ge__(self, other):
+        """If this >= other, it means this is a superset of the other."""
+        assert self.domain == other.domain
+        if self.domain is None or other.domain is None:
+            raise FuzzyWarning("Can't compare without Domains.")
+        return all(np.greater_equal(self.array(), other.array()))
+
+    def __gt__(self, other):
+        """If this > other, it means this is a proper superset of the other."""
+        assert self.domain == other.domain
+        if self.domain is None or other.domain is None:
+            raise FuzzyWarning("Can't compare without Domains.")
+        return all(np.greater(self.array(), other.array()))
+
+    def __len__(self):
+        """Number of membership values in the set, defined by bounds and resolution of domain."""
+        if self.domain is None:
+            raise FuzzyWarning("No domain.")
+        return len(self.array())
+
+    @property
+    def cardinality(self):
+        """The sum of all values in the set."""
+        if self.domain is None:
+            raise FuzzyWarning("No domain.")
+        return sum(self.array())
+
+    @property
+    def relative_cardinality(self):
+        """Relative cardinality is the sum of all membership values by number of all values."""
+        if self.domain is None:
+            raise FuzzyWarning("No domain.")
+        if len(self) == 0:
+            # this is highly unlikely and only possible with res=inf but still..
+            raise FuzzyWarning("The domain has no element.")
+        return self.cardinality / len(self)
+
+    def concentrated(self):
+        """
+        Alternative to hedge "very".
+
+        Returns a new set that has a reduced amount of values the set includes and to dampen the
+        membership of many values.
+        """
+        return Set(lambda x: self.func(x) ** 2, domain=self.domain)
+
+    def intensified(self):
+        """
+        Alternative to hedges.
+
+        Returns a new set where the membership of values are increased that
+        already strongly belong to the set and dampened the rest.
+        """
+
+        def f(x):
+            return 2 * self.func(x) ** 2 if x < 0.5 else 1 - 2 * (1 - self.func(x) ** 2)
+
+        return Set(f, domain=self.domain)
+
+    def dilated(self):
+        """Expand the set with more values and already included values are enhanced."""
+        return Set(lambda x: self.func(x) ** 1.0 / 2.0, domain=self.domain)
+
+    def multiplied(self, n):
+        """Multiply with a constant factor, changing all membership values."""
+        return Set(lambda x: self.func(x) * n, domain=self.domain)
+
+    def plot(self):
+        """Graph the set in the given domain."""
+        if self.domain is None:
+            raise FuzzyWarning("No domain assigned, cannot plot.")
+        R = self.domain.range
+        V = [self.func(x) for x in R]
+        plt.plot(R, V)
+
+    def array(self):
+        """Return an array of all values for this set within the given domain."""
+        if self.domain is None:
+            raise FuzzyWarning("No domain assigned.")
+        return np.fromiter((self.func(x) for x in self.domain.range), float)
+
+    def center_of_gravity(self):
+        """Return the center of gravity for this distribution, within the given domain."""
+
+        assert self.domain is not None, "No center of gravity with no domain."
+        weights = self.array()
+        if sum(weights) == 0:
+            return 0
+        cog = np.average(self.domain.range, weights=weights)
+        self.__center_of_gravity = cog
+        return cog
+
+    def __repr__(self):
+        """
+        Return a string representation of the Set that reconstructs the set with eval().
+
+        *******
+        Current implementation does NOT work correctly.
+
+        This is harder than expected since all functions are (recursive!) closures which
+        can't simply be pickled. If this functionality really is needed, all functions
+        would have to be peppered with closure-returning overhead such as
+
+        def create_closure_and_function(*args):
+            func = None
+            def create_function_closure():
+                return func
+
+            closure = create_function_closure.__closure__
+            func = types.FunctionType(*args[:-1] + [closure])
+            return func
+        """
+        return f"Set({self.func})"
+
+    def __str__(self):
+        """Return a string for print()."""
+        if self.domain is not None:
+            return f"{self.domain._name}.{self.name}"
+        if self.name is None:
+            return f"dangling Set({self.func})"
+        else:
+            return f"dangling Set({self.name}"
+
+    def normalized(self):
+        """Return a set that is normalized *for this domain* with 1 as max."""
+        if self.domain is None:
+            raise FuzzyWarning("Can't normalize without domain.")
+        return Set(normalize(max(self.array()), self.func), domain=self.domain)
+
+    def __hash__(self):
+        return id(self)
+
+
+class Rule:
+    """
+    A collection of bound sets that span a multi-dimensional space of their respective domains.
+    """
+
+    def __init__(self, conditions, func=None):
+        print("ohalala")
+        self.conditions = {frozenset(C): oth for C, oth in conditions.items()}
+        self.func = func
+
+    def __add__(self, other):
+        assert isinstance(other, Rule)
+        return Rule({**self.conditions, **other.conditions})
+
+    def __radd__(self, other):
+        assert isinstance(other, (Rule, int))
+        # we're using sum(..)
+        if isinstance(other, int):
+            return self
+        return Rule({**self.conditions, **other.conditions})
+
+    def __or__(self, other):
+        assert isinstance(other, Rule)
+        return Rule({**self.conditions, **other.conditions})
+
+    def __eq__(self, other):
+        return self.conditions == other.conditions
+
+    def __getitem__(self, key):
+        return self.conditions[frozenset(key)]
+
+    def __call__(self, args: "dict[Domain, float]", method="cog"):
+        """Calculate the infered value based on different methods.
+        Default is center of gravity (cog).
+        """
+        assert len(args) == max(
+            len(c) for c in self.conditions.keys()
+        ), "Number of values must correspond to the number of domains defined as conditions!"
+        assert isinstance(args, dict), "Please make sure to pass in the values as a dictionary."
+        match method:
+            case "cog":
+                assert (
+                    len({C.domain for C in self.conditions.values()}) == 1
+                ), "For CoG, all conditions must have the same target domain."
+                actual_values = {f: f(args[f.domain]) for S in self.conditions.keys() for f in S}
+
+                weights = []
+                for K, v in self.conditions.items():
+                    x = min((actual_values[k] for k in K if k in actual_values), default=0)
+                    if x > 0:
+                        weights.append((v, x))
+
+                if not weights:
+                    return None
+                target_domain = list(self.conditions.values())[0].domain
+                index = sum(v.center_of_gravity * x for v, x in weights) / sum(x for v, x in weights)
+                return (target_domain._high - target_domain._low) / len(
+                    target_domain.range
+                ) * index + target_domain._low
+
+            case "centroid":
+                raise NotImplementedError("Centroid method not implemented yet.")
+            case "bisector":
+                raise NotImplementedError("Bisector method not implemented yet.")
+            case "mom":
+                raise NotImplementedError("Middle of max method not implemented yet.")
+            case "som":
+                raise NotImplementedError("Smallest of max method not implemented yet.")
+            case "lom":
+                raise NotImplementedError("Largest of max method not implemented yet.")
+            case _:
+                raise ValueError("Invalid method.")
+
+
+def rule_from_table(table: str, references: dict):
+    """Turn a (2D) string table into a Rule of fuzzy sets.
+
+    ATTENTION: This will eval() all strings in the table.
+    This can pose a potential security risk if the table originates from an untrusted source.
+
+    Using a table will considerably reduce the amount of required text to describe all rules,
+    but there are two critical drawbacks: Tables are limited to 2 input variables (2D) and they are strings,
+    with no IDE support. It is strongly recommended to check the Rule output for consistency.
+    For example, a trailing "." will result in a SyntaxError when eval()ed.
+    """
+    import io
+    from itertools import product
+    from typing import Any
+
+    import pandas as pd
+
+    df = pd.read_table(io.StringIO(table), sep=r"\s+")
+
+    D: dict[tuple[Any, Any], Any] = {
+        (
+            eval(df.index[x].strip(), references),  # type: ignore
+            eval(df.columns[y].strip(), references),  # type: ignore
+        ): eval(df.iloc[x, y], references)  # type: ignore
+        for x, y in product(range(len(df.index)), range(len(df.columns)))
+    }
+    return Rule(D)
+
+
+if __name__ == "__main__":
+    import doctest
+
+    doctest.testmod()
```

### Comparing `fuzzylogic-1.2.0/src/fuzzylogic/functions.py` & `fuzzylogic-1.4.0/src/fuzzylogic/functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-
 """
 General-purpose functions that map R -> [0,1].
 
-These functions work as closures. 
+These functions work as closures.
 The inner function uses the variables of the outer function.
 
 These functions work in two steps: prime and call.
 In the first step the function is constructed, initialized and
 constants pre-evaluated. In the second step the actual value
 is passed into the function, using the arguments of the first step.
 
@@ -23,119 +22,154 @@
 The intervals with max(m) are called "height"
 The intervals  m != 1 and m != 0 are called 'boundary'.
 The intervals with m == 0 are called 'unsupported', short no_m
 
 In a fuzzy set with one and only one m == 1, this element is called 'prototype'.
 """
 
-
+from collections.abc import Callable
 from math import exp, isinf, isnan, log
+from typing import Any, Optional
+
+try:
+    raise ImportError
+    # from numba import njit # still not ready for prime time :(
+
+except ImportError:
+
+    def njit(func: Callable) -> Callable:
+        return func
+
 
 #####################
 # SPECIAL FUNCTIONS #
 #####################
 
-def inv(g):
+type number = int | float
+
+
+def inv(g: Callable[[number], number]) -> Callable:
     """Invert the given function within the unit-interval.
-    
+
     For sets, the ~ operator uses this. It is equivalent to the TRUTH value of FALSE.
     """
-    def f(x):
-        return 1 - g(x)
+
+    def f(x: number) -> float:
+        return float(1 - g(x))
+
     return f
 
 
-def noop():
+def noop() -> Callable:
     """Do nothing and return the value as is.
-    
+
     Useful for testing.
     """
-    def f(x):
+
+    def f(x: number) -> number:
         return x
+
     return f
 
-def constant(c):
+
+def constant(c: number) -> Callable:
     """Return always the same value, no matter the input.
-    
+
     Useful for testing.
     >>> f = constant(1)
     >>> f(0)
     1
     """
-    def f(_):
+
+    def f(_: Any) -> number:
         return c
+
     return f
 
 
-def alpha(*, floor=0, ceiling=1, func,  
-          floor_clip=None, ceiling_clip=None):
+def alpha(
+    *,
+    floor: number = 0,
+    ceiling: number = 1,
+    func: Callable,
+    floor_clip: Optional[number] = None,
+    ceiling_clip: Optional[number] = None,
+):
     """Clip a function's values.
-    
+
     This is used to either cut off the upper or lower part of a graph.
     Actually, this is more like a hedge but doesn't make sense for sets.
     """
-    assert floor <= ceiling
-    assert 0 <= floor
-    assert ceiling <= 1
-    
+    assert floor <= ceiling, breakpoint()
+    assert 0 <= floor, breakpoint()
+    assert ceiling <= 1, breakpoint()
+
     floor_clip = floor if floor_clip is None else floor_clip
     ceiling_clip = ceiling if ceiling_clip is None else ceiling_clip
-    
-    #assert 0 <= floor_clip <= ceiling_clip <= 1, "%s <= %s"%(floor_clip, ceiling_clip)
-    
-    def f(x):
+    # assert 0 <= floor_clip <= ceiling_clip <= 1, "%s <= %s"%(floor_clip, ceiling_clip)
+
+    def f(x: number) -> float:
         m = func(x)
         if m >= ceiling:
             return ceiling_clip
         elif m <= floor:
             return floor_clip
-        else: 
+        else:
             return m
+
     return f
 
-def normalize(height, func):
+
+def normalize(height: number, func: Callable) -> Callable:
     """Map [0,1] to [0,1] so that max(array) == 1."""
     assert 0 < height <= 1
-    
-    def f(x):
+
+    def f(x: number) -> float:
         return func(x) / height
+
     return f
 
-def moderate(func):
+
+def moderate(func: Callable) -> Callable:
     """Map [0,1] -> [0,1] with bias towards 0.5.
 
     For instance this is needed to dampen extremes.
     """
-    def f(x):
-        return 1/2 + 4 * (func(x) - 1/2)**3
+
+    def f(x: number) -> float:
+        return 1 / 2 + 4 * (func(x) - 1 / 2) ** 3
+
     return f
-    
+
+
 ########################
 # MEMBERSHIP FUNCTIONS #
 ########################
 
-def singleton(p, *, no_m=0, c_m=1):
+
+def singleton(p: number, *, no_m: number = 0, c_m: number = 1):
     """A single spike.
-    
+
     >>> f = singleton(2)
     >>> f(1)
     0
     >>> f(2)
     1
     """
     assert 0 <= no_m < c_m <= 1
 
-    def f(x):
+    def f(x: number) -> number:
         return c_m if x == p else no_m
+
     return f
 
 
-def linear(m:float=0, b:float=0) -> callable:
+def linear(m: number = 0, b: number = 0) -> Callable:
     """A textbook linear function with y-axis section and gradient.
-    
+
     f(x) = m*x + b
     BUT CLIPPED.
 
     >>> f = linear(1, -1)
     >>> f(-2)   # should be -3 but clipped
     0
     >>> f(0)    # should be -1 but clipped
@@ -145,37 +179,68 @@
     >>> f(1.5)
     0.5
     >>> f(2)
     1
     >>> f(3)    # should be 2 but clipped
     1
     """
-    def f(x) -> float:
+
+    def f(x: number) -> number:
         y = m * x + b
         if y <= 0:
             return 0
         elif y >= 1:
             return 1
         else:
             return y
+
+    return f
+
+
+def step(limit: number, /, *, left: number = 0, right: number = 1, at_lmt: number | None = None) -> Callable:
+    """A step function.
+
+    Coming from left, the function returns the *left* argument.
+    At the limit, it returns *at_lmt* or the average of left and right.
+    After the limit, it returns the *right* argument.
+    >>> f = step(2)
+    >>> f(1)
+    0
+    >>> f(2)
+    0.5
+    >>> f(3)
+    1
+    """
+    assert 0 <= left <= 1 and 0 <= right <= 1
+
+    def f(x: number) -> number:
+        if x < limit:
+            return left
+        elif x > limit:
+            return right
+        else:
+            return at_lmt if at_lmt is not None else (left + right) / 2
+
     return f
 
 
-def bounded_linear(low, high, *, c_m=1, no_m=0, inverse=False):
+def bounded_linear(
+    low: number, high: number, *, c_m: number = 1, no_m: number = 0, inverse=False
+) -> Callable:
     """Variant of the linear function with gradient being determined by bounds.
 
     The bounds determine minimum and maximum value-mappings,
     but also the gradient. As [0, 1] must be the bounds for y-values,
     left and right bounds specify 2 points on the graph, for which the formula
     f(x) = y = (y2 - y1) / (x2 - x1) * (x - x1) + y1 = (y2 - y1) / (x2 - x1) *
                                                                 (x - x2) + y2
 
     (right_y - left_y) / ((right - left) * (x - self.left) + left_y)
     works.
-    
+
     >>> f = bounded_linear(2, 3)
     >>> f(1)
     0.0
     >>> f(2)
     0.0
     >>> f(2.5)
     0.5
@@ -185,199 +250,198 @@
     1.0
     """
     assert low < high, "low must be less than high"
     assert c_m > no_m, "core_m must be greater than unsupported_m"
 
     if inverse:
         c_m, no_m = no_m, c_m
-    
+
     gradient = (c_m - no_m) / (high - low)
-    
+
     # special cases found by hypothesis
-    
-    def g_0(_):
+
+    def g_0(_: Any) -> float:
         return (c_m + no_m) / 2
-    
+
     if gradient == 0:
         return g_0
-    
-    def g_inf(x):
+
+    def g_inf(x: number) -> float:
         asymptode = (high + low) / 2
         if x < asymptode:
             return no_m
         elif x > asymptode:
             return c_m
         else:
             return (c_m + no_m) / 2
-    
+
     if isinf(gradient):
         return g_inf
-    
-    def f(x):
+
+    def f(x: number) -> float:
         y = gradient * (x - low) + no_m
         if y < 0:
-            return 0.
-        if y > 1:
-            return 1.
-        return y
+            return 0.0
+        return 1.0 if y > 1 else y
+
     return f
 
 
-def R(low, high):
+def R(low: number, high: number) -> Callable:
     """Simple alternative for bounded_linear().
-    
+
     THIS FUNCTION ONLY CAN HAVE A POSITIVE SLOPE -
     USE THE S() FUNCTION FOR NEGATIVE SLOPE.
     """
     assert low < high, f"{low} >? {high}"
 
-    def f(x):
+    def f(x: number) -> float:
         if x < low or isinf(high - low):
             return 0
         elif low <= x <= high:
             return (x - low) / (high - low)
         else:
             return 1
+
     return f
 
-def S(low, high):
+
+def S(low: number, high: number) -> Callable:
     """Simple alternative for bounded_linear.
-    
+
     THIS FUNCTION ONLY CAN HAVE A NEGATIVE SLOPE -
     USE THE R() FUNCTION FOR POSITIVE SLOPE.
     """
     assert low < high, f"{low}, {high}"
 
-    def f(x):
+    def f(x: number) -> float:
         if x <= low:
             return 1
         elif low < x < high:
             # factorized to avoid nan
-            return high / (high - low) - x / (high - low) 
+            return high / (high - low) - x / (high - low)
         else:
             return 0
+
     return f
 
 
-def rectangular(low:float, high:float, *, c_m:float=1, no_m:float=0) -> callable:
+def rectangular(low: number, high: number, *, c_m: number = 1, no_m: number = 0) -> Callable:
     """Basic rectangular function that returns the core_y for the core else 0.
-    
+
         ______
         |    |
     ____|    |___
     """
-    assert low < high, f'{low}, {high}'
+    assert low < high, f"{low}, {high}"
 
-    def f(x:float) -> float:
-        if x < low or high < x:
-            return no_m
-        else:
-            return c_m
+    def f(x: number) -> number:
+        return no_m if x < low or high < x else c_m
 
     return f
 
 
-def triangular(low, high, *, c=None, c_m=1, no_m=0):
+def triangular(low: number, high: number, *, c: number | None = None, c_m: number = 1, no_m: number = 0):
     r"""Basic triangular norm as combination of two linear functions.
 
          /\
     ____/  \___
 
     """
-    assert low < high, 'low must be less than high.'
+    assert low < high, "low must be less than high."
     assert no_m < c_m
-    
-    c = c if c is not None else (low + high) / 2.
+
+    c = c if c is not None else (low + high) / 2.0
     assert low < c < high, "peak must be inbetween"
-    
+
     left_slope = bounded_linear(low, c, no_m=0, c_m=c_m)
     right_slope = inv(bounded_linear(c, high, no_m=0, c_m=c_m))
 
-    def f(x):
+    def f(x: number) -> number:
         return left_slope(x) if x <= c else right_slope(x)
+
     return f
 
 
-def trapezoid(low, c_low, c_high, high, *, c_m=1, no_m=0):
+def trapezoid(low: number, c_low: number, c_high: number, high: number, *, c_m: number = 1, no_m: number = 0):
     r"""Combination of rectangular and triangular, for convenience.
-    
+
           ____
          /    \
     ____/      \___
 
     """
     assert low < c_low <= c_high < high
-    assert 0 <= no_m < c_m <= 1 
+    assert 0 <= no_m < c_m <= 1
 
     left_slope = bounded_linear(low, c_low, c_m=c_m, no_m=no_m)
-    right_slope = bounded_linear(c_high, high, c_m=c_m, no_m=no_m,
-                                inverse=True)
+    right_slope = bounded_linear(c_high, high, c_m=c_m, no_m=no_m, inverse=True)
 
-    def f(x):
+    def f(x: number) -> number:
         if x < low or high < x:
             return no_m
         elif x < c_low:
             return left_slope(x)
         elif x > c_high:
             return right_slope(x)
         else:
             return c_m
 
     return f
 
 
-def sigmoid(L, k, x0):
+def sigmoid(L: number, k: number, x0: number = 0):
     """Special logistic function.
 
     http://en.wikipedia.org/wiki/Logistic_function
 
     f(x) = L / (1 + e^(-k*(x-x0)))
     with
     x0 = x-value of the midpoint
     L = the curve's maximum value
     k = steepness
     """
     # need to be really careful here, otherwise we end up in nanland
-    assert 0 < L <= 1, 'L invalid.'
+    assert 0 < L <= 1, "L invalid."
 
-    def f(x):
-        if isnan(k*x):
+    def f(x: number) -> float:
+        if isnan(k * x):
             # e^(0*inf) = 1
-            o = 1.
+            o = 1.0
         else:
             try:
-                o = exp(-k*(x - x0))
+                o = exp(-k * (x - x0))
             except OverflowError:
                 o = float("inf")
         return L / (1 + o)
 
     return f
 
 
-def bounded_sigmoid(low, high, inverse=False):
+def bounded_sigmoid(low: number, high: number, inverse=False):
     """
     Calculate a weight based on the sigmoid function.
 
     Specify the lower limit where f(x) = 0.1 and the
     upper with f(x) = 0.9 and calculate the steepness and elasticity
     based on these. We don't need the general logistic function as we
     operate on [0,1].
-    
+
     core idea:
-    f(x) = 1. / (1. + exp(x * (4. * log(3)) / (low - high)) * 
+    f(x) = 1. / (1. + exp(x * (4. * log(3)) / (low - high)) *
                 9 * exp(low * -(4. * log(3)) / (low - high)))
-    
-    How I got this? IIRC I was playing around with linear equations and 
+
+    How I got this? IIRC I was playing around with linear equations and
     boundary conditions of sigmoid funcs on wolframalpha..
-    
+
     previously factored to:
     k = -(4. * log(3)) / (low - high)
     o = 9 * exp(low * k)
     return 1 / (1 + exp(-k * x) * o)
-    
+
     vars
     ----
     low: x-value with f(x) = 0.1
     for x < low: m -> 0
     high: x-value with f(x) = 0.9
     for x > high: m -> 1
 
@@ -387,67 +451,70 @@
     >>> round(f(1), 2)
     0.9
     >>> round(f(100000), 2)
     1.0
     >>> round(f(-100000), 2)
     0.0
     """
-    assert low < high, 'low must be less than high'
-    
+    assert low < high, "low must be less than high"
+
     if inverse:
         low, high = high, low
-    
-    k = (4. * log(3)) / (low - high)
+
+    k = (4.0 * log(3)) / (low - high)
     try:
         # if high - low underflows to 0..
         if isinf(k):
-            p = 0.
+            p = 0.0
         # just in case k -> 0 and low -> inf
         elif isnan(-k * low):
-            p = 1.
+            p = 1.0
         else:
             p = exp(-k * low)
     except OverflowError:
         p = float("inf")
-    
-    def f(x):
+
+    def f(x: number) -> float:
         try:
             # e^(0*inf) = 1 for both -inf and +inf
-            if (isinf(k) and x == 0) or (k == 0 and isinf(x)):
-                q = 1.
-            else: q = exp(x * k)
+            q = 1.0 if (isinf(k) and x == 0) or (k == 0 and isinf(x)) else exp(x * k)
         except OverflowError:
             q = float("inf")
-        
+
         # e^(inf)*e^(-inf) = 1
         r = p * q
         if isnan(r):
             r = 1
         return 1 / (1 + 9 * r)
+
     return f
 
-def bounded_exponential(k=0.1, limit=1):
+
+def bounded_exponential(k: number = 0.1, limit: number = 1):
     """Function that goes through the origin and approaches a limit.
     k determines the steepness. The function defined for [0, +inf).
     Useful for things that can't be below 0 but may not have a limit like temperature
     or time, so values are always defined.
     f(x)=limit-limit/e^(k*x)
 
     Again: This function assumes x >= 0, there are no checks for this assumption!
     """
     assert limit > 0
     assert k > 0
-    def f(x):
-        try: 
-            return limit - limit/exp(k*x)
+
+    def f(x: number) -> float:
+        try:
+            return limit - limit / exp(k * x)
         except OverflowError:
-            return limit
+            return float(limit)
+
     return f
 
-def simple_sigmoid(k=0.229756):
+
+def simple_sigmoid(k: number = 0.229756):
     """Sigmoid variant with only one parameter (steepness).
 
     The midpoint is 0.
     The slope is positive for positive k and negative k.
     f(x) is within [0,1] for any real k and x.
     >>> f = simple_sigmoid()
     >>> round(f(-1000), 2)
@@ -457,75 +524,76 @@
     >>> round(f(1000), 2)
     1.0
     >>> round(f(-20), 2)
     0.01
     >>> round(f(20), 2)
     0.99
     """
-    def f(x):
-        # yay for limits..
-        if (isinf(x) and k == 0):
-            return 1/2
-        else:
-            try:
-                return 1 / (1 + exp(x * -k))
-            except OverflowError:
-                return 0.
+
+    def f(x: number) -> float:
+        if isinf(x) and k == 0:
+            return 1 / 2
+        try:
+            return 1 / (1 + exp(x * -k))
+        except OverflowError:
+            return 0.0
+
     return f
 
 
-def triangular_sigmoid(low, high, c=None):
+def triangular_sigmoid(low: number, high: number, c: number | None = None):
     """Version of triangular using sigmoids instead of linear.
-    
+
     THIS FUNCTION PEAKS AT 0.9
 
     >>> g = triangular_sigmoid(2, 4)
     >>> g(2)
     0.1
     >>> round(g(3), 2)
     0.9
     """
     assert low < high, "low must be less than high"
-    c = c if c is not None else (low + high) / 2.
+    c = c if c is not None else (low + high) / 2.0
     assert low < c < high, "c must be inbetween"
 
     left_slope = bounded_sigmoid(low, c)
+    "float"
     right_slope = inv(bounded_sigmoid(c, high))
+    "float"
 
-    def f(x):
-        if x <= c:
-            return left_slope(x)
-        else:
-            return right_slope(x)
+    def f(x: number) -> float:
+        return left_slope(x) if x <= c else right_slope(x)
 
     return f
 
 
-def gauss(c, b, *, c_m=1):
+def gauss(c: number, b: number, *, c_m: number = 1) -> Callable:
     """Defined by ae^(-b(x-x0)^2), a gaussian distribution.
-    
+
     Basically a triangular sigmoid function, it comes close to human perception.
 
     vars
     ----
     c_m (a)
         defines the maximum y-value of the graph
     b
         defines the steepness
     c (x0)
         defines the symmetry center/peak of the graph
     """
     assert 0 < c_m <= 1
     assert 0 < b, "b must be greater than 0"
 
-    def f(x):
+    def f(x: number) -> float:
         try:
-            o = (x - c)**2
+            o = (x - c) ** 2
         except OverflowError:
             return 0
         return c_m * exp(-b * o)
+
     return f
 
 
 if __name__ == "__main__":
     import doctest
+
     doctest.testmod()
```

### Comparing `fuzzylogic-1.2.0/src/fuzzylogic/hedges.py` & `fuzzylogic-1.4.0/src/fuzzylogic/hedges.py`

 * *Files identical despite different names*

### Comparing `fuzzylogic-1.2.0/src/fuzzylogic/rules.py` & `fuzzylogic-1.4.0/src/fuzzylogic/rules.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Functions to evaluate, infer and defuzzify."""
 
 from math import isinf
 
-from .classes import Domain, Set
+from .classes import Domain
 
 
 def round_partial(value, res):
     """
     Round any value to any arbitrary precision.
 
     >>> round_partial(0.405, 0.02)
@@ -23,17 +23,15 @@
     7.75
     >>> round_partial(987654321, 100)
     987654300
     >>> round_partial(3.14, 0)
     3.14
     """
     # backed up by wolframalpha
-    if res == 0 or isinf(res):
-        return value
-    return round(value / res) * res
+    return value if res == 0 or isinf(res) else round(value / res) * res
 
 
 def rescale(out_min, out_max, *, in_min=0, in_max=1):
     """Scale from one domain to another.
 
     Tests only cover scaling from [0,1] (with default in_min, in_max!)
     to R.
@@ -60,26 +58,26 @@
 
     def f(x):
         return (n - a * x - o + b * x) / m
 
     return f
 
 
-def weighted_sum(*, weights: dict, target_d: Domain) -> float:
+def weighted_sum(*, weights: dict, target_d: Domain):
     """Used for weighted decision trees and such.
 
     Parametrize with dict of factorname -> weight and domain of results.
     Call with a dict of factorname -> [0, 1]
 
     There SHOULD be the same number of items (with the same names!)
     of weights and factors, but it doesn't have to be - however
     set(factors.names) <= set(weights.names) - in other words:
     there MUST be at least as many items in weights as factors.
     """
-    assert sum(w for w in weights.values()) == 1
+    assert sum(weights.values()) == 1, breakpoint()
 
     rsc = rescale(target_d._low, target_d._high)
 
     def f(memberships):
         result = sum(r * weights[n] for n, r in memberships.items())
         return round_partial(rsc(result), target_d._res)
```

### Comparing `fuzzylogic-1.2.0/src/fuzzylogic/truth.py` & `fuzzylogic-1.4.0/src/fuzzylogic/truth.py`

 * *Files identical despite different names*

### Comparing `fuzzylogic-1.2.0/src/fuzzylogic.egg-info/PKG-INFO` & `fuzzylogic-1.4.0/src/fuzzylogic.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,67 @@
-Metadata-Version: 2.1
-Name: fuzzylogic
-Version: 1.2.0
-Summary: Fuzzy Logic for Python 3
-Home-page: https://github.com/amogorkon/fuzzylogic
-Author: Anselm Kiefner
-Author-email: fuzzylogic-pypi@anselm.kiefner.de
-License: MIT
-Keywords: fuzzy logic
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Manufacturing
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Fuzzy Logic for Python 3
-
-[![license](https://img.shields.io/github/license/amogorkon/fuzzylogic)](https://github.com/amogorkon/fuzzylogic/blob/master/LICENSE)
-[![stars](https://img.shields.io/github/stars/amogorkon/fuzzylogic?style=plastic)](https://github.com/amogorkon/fuzzylogic/stargazers)
-[![forks](https://img.shields.io/github/forks/amogorkon/fuzzylogic?style=plastic)](https://github.com/amogorkon/fuzzylogic/network/members)
-[![Downloads](https://pepy.tech/badge/fuzzylogic)](https://pepy.tech/project/fuzzylogic)
-
-
-This is the fourth time I rebuilt this library from scratch to find the sweet spot between ease of use (beautiful is better than ugly!), testability (simple is better than complex!) and potential for performance optimization (practicality beats purity!). 
-
-### Why a new library?
-The first time I was confronted with fuzzy logic, I fell in love with the concept, but after reading books and checking out libraries etc. I found it frustrating how most people make fuzzy logic appear complicated, hard to handle and incorporate in code.
-Sure, there are frameworks that allow modelling of functions via GUI, but that's not a solution for a coder, right? Then there's a ton of mathematical research and other cruft that no normal person has time and patience to work through before trying to explore and applying things. Coming from this direction, there are also a number of script-ish (DSL) language frameworks that try to make the IF THEN ELSE pattern work (which I also tried in python, but gave it up because it just looks ugly).
-And yes, it's also possible to implement the whole thing completely in a functional style, but you really don't want to work with a recursive structure of 7+ steps by hand, trying not to miss a (..) along the way.
-Finally, most education on the subject emphasize sets and membership functions, but fail to mention the importance of the domain (or "universe of discourse"). It's easy to miss this point if you get lost with set operations and membership values, which are actually not that difficult once you can *play* and *explore* how these things look and work!
-
-### The Idea
-So, the idea is to have three parts that work together: domains, sets and rules. Each of these classes wrap additional logic around basic building blocks - Set gives logical operations to simple functions, Domain gives additional logic to numpy arrays and groups Sets together while Rule combines different Domains. You start modelling your system by defining your domain of interest. Then you think about where your interesting points are in that domain and look for a function that might do what you want. In general, fuzzy.functions map any value to [0,1], that's all. Simply wrap the function in a Set and assign it to the domain in question. Once assigned, you can plot that set and see if it actually looks how you imagined. Now that you have one or more sets, you also can start to combine them with set operations &, |, ~, etc. It's fairly straight forward.
-Finally, use the Rules to map input domain to output domain to actually control stuff.
-### Warning: Magic
-To make it possible to write fuzzy logic in the most pythonic and simplest way imaginable, it was necessary to employ some magic tricks that normally are discouraged, but at least there's no black magic involved (aka meta-programming etc.), so things are easy to debug if there is a problem. Most notably:
-* all functions are recursive closures (which makes it kinda hard to serialize things, if you really want to do that)
-* The main classes use a lot of dunder methods to implement their logic, which can be a bit daunting at first glance
-* Domain and Set uses an assignment trick to make it possible to instantiate Set() without passing domain and name over and over (yet still be explicit, just not the way one would normally expect). This also allows to call sets as Domain.attributes, which also normally shouldn't be possible (since they are technically not attributes). However, this allows interesting things like dangling sets (sets without domains) that can be freely combined with other sets to avoid cluttering of domain-namespaces and just have the resulting set assigned to a domain to work with.
-
-# Installation
-Just enter 
-`python -m pip install fuzzylogic`
-in a commandline prompt and you should be good to go!
-
-It's even more fun to experiment with it in jupyter lab ( https://jupyter.org/ ) :-)
-
-# Check out the Showcase!
-For complete examples and documentation how to work with fuzzylogic, check out https://github.com/amogorkon/fuzzylogic/blob/master/docs/Showcase.ipynb !
-
-Have fun!
-
-# Office Hours
-You can also contact me one-on-one! Please follow https://calendly.com/amogorkon/officehours to set up a meeting :-)
-
--- Anselm Kiefner
-
-
+Metadata-Version: 2.1
+Name: fuzzylogic
+Version: 1.4.0
+Summary: Fuzzy Logic for Python 3
+Home-page: https://github.com/amogorkon/fuzzylogic
+Author: Anselm Kiefner
+Author-email: fuzzylogic-pypi@anselm.kiefner.de
+License: MIT
+Keywords: fuzzy logic
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Manufacturing
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Requires-Python: >=3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Fuzzy Logic for Python 3
+
+[![license](https://img.shields.io/github/license/amogorkon/fuzzylogic)](https://github.com/amogorkon/fuzzylogic/blob/master/LICENSE)
+[![stars](https://img.shields.io/github/stars/amogorkon/fuzzylogic?style=plastic)](https://github.com/amogorkon/fuzzylogic/stargazers)
+[![forks](https://img.shields.io/github/forks/amogorkon/fuzzylogic?style=plastic)](https://github.com/amogorkon/fuzzylogic/network/members)
+[![Downloads](https://pepy.tech/badge/fuzzylogic)](https://pepy.tech/project/fuzzylogic)
+
+
+This is the fourth time I rebuilt this library from scratch to find the sweet spot between ease of use (beautiful is better than ugly!), testability (simple is better than complex!) and potential for performance optimization (practicality beats purity!). 
+
+### Why a new library?
+The first time I was confronted with fuzzy logic, I fell in love with the concept, but after reading books and checking out libraries etc. I found it frustrating how most people make fuzzy logic appear complicated, hard to handle and incorporate in code.
+Sure, there are frameworks that allow modelling of functions via GUI, but that's not a solution for a coder, right? Then there's a ton of mathematical research and other cruft that no normal person has time and patience to work through before trying to explore and applying things. Coming from this direction, there are also a number of script-ish (DSL) language frameworks that try to make the IF THEN ELSE pattern work (which I also tried in python, but gave it up because it just looks ugly).
+And yes, it's also possible to implement the whole thing completely in a functional style, but you really don't want to work with a recursive structure of 7+ steps by hand, trying not to miss a (..) along the way.
+Finally, most education on the subject emphasize sets and membership functions, but fail to mention the importance of the domain (or "universe of discourse"). It's easy to miss this point if you get lost with set operations and membership values, which are actually not that difficult once you can *play* and *explore* how these things look and work!
+
+### The Idea
+So, the idea is to have three parts that work together: domains, sets and rules. Each of these classes wrap additional logic around basic building blocks - Set gives logical operations to simple functions, Domain gives additional logic to numpy arrays and groups Sets together while Rule combines different Domains. You start modelling your system by defining your domain of interest. Then you think about where your interesting points are in that domain and look for a function that might do what you want. In general, fuzzy.functions map any value to [0,1], that's all. Simply wrap the function in a Set and assign it to the domain in question. Once assigned, you can plot that set and see if it actually looks how you imagined. Now that you have one or more sets, you also can start to combine them with set operations &, |, ~, etc. It's fairly straight forward.
+Finally, use the Rules to map input domain to output domain to actually control stuff.
+### Warning: Magic
+To make it possible to write fuzzy logic in the most pythonic and simplest way imaginable, it was necessary to employ some magic tricks that normally are discouraged, but at least there's no black magic involved (aka meta-programming etc.), so things are easy to debug if there is a problem. Most notably:
+* all functions are recursive closures (which makes it kinda hard to serialize things, if you really want to do that)
+* The main classes use a lot of dunder methods to implement their logic, which can be a bit daunting at first glance
+* Domain and Set uses an assignment trick to make it possible to instantiate Set() without passing domain and name over and over (yet still be explicit, just not the way one would normally expect). This also allows to call sets as Domain.attributes, which also normally shouldn't be possible (since they are technically not attributes). However, this allows interesting things like dangling sets (sets without domains) that can be freely combined with other sets to avoid cluttering of domain-namespaces and just have the resulting set assigned to a domain to work with.
+
+# Installation
+Just enter 
+`python -m pip install fuzzylogic`
+in a commandline prompt and you should be good to go!
+
+It's even more fun to experiment with it in [Jupyter Lab](https://jupyter.org) :-)
+
+# Documentation
+Thanks to [Atul Kushwaha](https://github.com/coderatul), we now have an amazing [documentation](https://fuzzylogic.readthedocs.io/en/latest/) including our [Showcase](https://github.com/amogorkon/fuzzylogic/blob/master/docs/Showcase.ipynb) - check it out!
+
+# Office Hours
+You can also contact me one-on-one! Please follow https://calendly.com/amogorkon/officehours to set up a meeting :-)
+
+# Office Hours
+You can also contact me one-on-one! Check my [office hours](https://calendly.com/amogorkon/officehours) to set up a meeting :-)
+
+-- Anselm Kiefner
```


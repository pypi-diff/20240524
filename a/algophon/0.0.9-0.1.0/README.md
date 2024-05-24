# Comparing `tmp/algophon-0.0.9.tar.gz` & `tmp/algophon-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algophon-0.0.9.tar", last modified: Mon May  6 15:46:32 2024, max compression
+gzip compressed data, was "algophon-0.1.0.tar", last modified: Fri May 24 00:10:47 2024, max compression
```

## Comparing `algophon-0.0.9.tar` & `algophon-0.1.0.tar`

### file list

```diff
@@ -1,33 +1,46 @@
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-06 15:46:32.514066 algophon-0.0.9/
--rw-r--r--   0 u6052607   (503) staff       (20)    11357 2024-04-18 14:18:03.000000 algophon-0.0.9/LICENSE
--rw-r--r--   0 u6052607   (503) staff       (20)     9638 2024-05-06 15:46:32.513321 algophon-0.0.9/PKG-INFO
--rw-r--r--   0 u6052607   (503) staff       (20)     9006 2024-04-19 00:09:14.000000 algophon-0.0.9/README.md
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-06 15:46:32.473955 algophon-0.0.9/algophon/
--rw-r--r--   0 u6052607   (503) staff       (20)      245 2024-05-05 22:24:11.000000 algophon-0.0.9/algophon/__init__.py
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-06 15:46:32.487633 algophon-0.0.9/algophon/distance/
--rw-r--r--   0 u6052607   (503) staff       (20)        0 2024-05-05 22:11:24.000000 algophon-0.0.9/algophon/distance/__init__.py
--rw-r--r--   0 u6052607   (503) staff       (20)     5222 2024-05-06 15:22:54.000000 algophon-0.0.9/algophon/distance/edit_distance.py
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-06 15:46:32.493350 algophon-0.0.9/algophon/ipa/
--rw-r--r--   0 u6052607   (503) staff       (20)       32 2024-04-19 13:49:06.000000 algophon-0.0.9/algophon/ipa/__init__.py
--rw-r--r--   0 u6052607   (503) staff       (20)     3081 2024-05-03 14:26:54.000000 algophon-0.0.9/algophon/ipa/convert.py
--rw-r--r--   0 u6052607   (503) staff       (20)   350576 2024-04-25 00:16:18.000000 algophon-0.0.9/algophon/ipa.txt
--rw-r--r--   0 u6052607   (503) staff       (20)     1006 2024-04-19 00:08:37.000000 algophon-0.0.9/algophon/natclass.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1173 2024-04-18 18:31:25.000000 algophon-0.0.9/algophon/seg.py
--rw-r--r--   0 u6052607   (503) staff       (20)     5850 2024-04-25 00:03:43.000000 algophon-0.0.9/algophon/seginv.py
--rw-r--r--   0 u6052607   (503) staff       (20)     5780 2024-05-06 15:42:02.000000 algophon-0.0.9/algophon/segstr.py
--rw-r--r--   0 u6052607   (503) staff       (20)      178 2024-04-25 00:14:05.000000 algophon-0.0.9/algophon/symbols.py
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-06 15:46:32.512549 algophon-0.0.9/algophon.egg-info/
--rw-r--r--   0 u6052607   (503) staff       (20)     9638 2024-05-06 15:46:32.000000 algophon-0.0.9/algophon.egg-info/PKG-INFO
--rw-r--r--   0 u6052607   (503) staff       (20)      560 2024-05-06 15:46:32.000000 algophon-0.0.9/algophon.egg-info/SOURCES.txt
--rw-r--r--   0 u6052607   (503) staff       (20)        1 2024-05-06 15:46:32.000000 algophon-0.0.9/algophon.egg-info/dependency_links.txt
--rw-r--r--   0 u6052607   (503) staff       (20)       12 2024-05-06 15:46:32.000000 algophon-0.0.9/algophon.egg-info/requires.txt
--rw-r--r--   0 u6052607   (503) staff       (20)        9 2024-05-06 15:46:32.000000 algophon-0.0.9/algophon.egg-info/top_level.txt
--rw-r--r--   0 u6052607   (503) staff       (20)      829 2024-05-06 15:45:42.000000 algophon-0.0.9/pyproject.toml
--rw-r--r--   0 u6052607   (503) staff       (20)       38 2024-05-06 15:46:32.514159 algophon-0.0.9/setup.cfg
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-06 15:46:32.511666 algophon-0.0.9/tests/
--rw-r--r--   0 u6052607   (503) staff       (20)     1240 2024-05-05 22:45:04.000000 algophon-0.0.9/tests/test_distance.py
--rw-r--r--   0 u6052607   (503) staff       (20)      860 2024-04-19 00:19:07.000000 algophon-0.0.9/tests/test_natclass.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1273 2024-04-18 23:49:35.000000 algophon-0.0.9/tests/test_seg.py
--rw-r--r--   0 u6052607   (503) staff       (20)     2746 2024-04-24 23:34:28.000000 algophon-0.0.9/tests/test_seginv.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1941 2024-04-24 23:29:27.000000 algophon-0.0.9/tests/test_segstr.py
--rw-r--r--   0 u6052607   (503) staff       (20)      884 2024-05-05 22:29:23.000000 algophon-0.0.9/tests/tester.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-24 00:10:47.826599 algophon-0.1.0/
+-rw-r--r--   0 u6052607   (503) staff       (20)    11357 2024-04-18 14:18:03.000000 algophon-0.1.0/LICENSE
+-rw-r--r--   0 u6052607   (503) staff       (20)    10227 2024-05-24 00:10:47.825284 algophon-0.1.0/PKG-INFO
+-rw-r--r--   0 u6052607   (503) staff       (20)     9596 2024-05-24 00:09:59.000000 algophon-0.1.0/README.md
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-24 00:10:47.738799 algophon-0.1.0/algophon/
+-rw-r--r--   0 u6052607   (503) staff       (20)      245 2024-05-05 22:24:11.000000 algophon-0.1.0/algophon/__init__.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-24 00:10:47.756923 algophon-0.1.0/algophon/distance/
+-rw-r--r--   0 u6052607   (503) staff       (20)        0 2024-05-05 22:11:24.000000 algophon-0.1.0/algophon/distance/__init__.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     5222 2024-05-06 15:22:54.000000 algophon-0.1.0/algophon/distance/edit_distance.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-24 00:10:47.762670 algophon-0.1.0/algophon/ipa/
+-rw-r--r--   0 u6052607   (503) staff       (20)       32 2024-04-19 13:49:06.000000 algophon-0.1.0/algophon/ipa/__init__.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     3081 2024-05-03 14:26:54.000000 algophon-0.1.0/algophon/ipa/convert.py
+-rw-r--r--   0 u6052607   (503) staff       (20)   350576 2024-04-25 00:16:18.000000 algophon-0.1.0/algophon/ipa.txt
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-24 00:10:47.763248 algophon-0.1.0/algophon/models/
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-24 00:10:47.778672 algophon-0.1.0/algophon/models/D2L/
+-rw-r--r--   0 u6052607   (503) staff       (20)      179 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/models/D2L/__init__.py
+-rw-r--r--   0 u6052607   (503) staff       (20)    13761 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/models/D2L/d2l.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1854 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/models/D2L/discrepancy.py
+-rw-r--r--   0 u6052607   (503) staff       (20)    10969 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/models/D2L/rule.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     3205 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/models/D2L/tier.py
+-rw-r--r--   0 u6052607   (503) staff       (20)        0 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/models/__init__.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1006 2024-04-19 00:08:37.000000 algophon-0.1.0/algophon/natclass.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1779 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/seg.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     8023 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/seginv.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     5780 2024-05-06 15:42:02.000000 algophon-0.1.0/algophon/segstr.py
+-rw-r--r--   0 u6052607   (503) staff       (20)      250 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/symbols.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-24 00:10:47.789201 algophon-0.1.0/algophon/utils/
+-rw-r--r--   0 u6052607   (503) staff       (20)       36 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/utils/__init__.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1114 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/utils/utils.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-24 00:10:47.823174 algophon-0.1.0/algophon.egg-info/
+-rw-r--r--   0 u6052607   (503) staff       (20)    10227 2024-05-24 00:10:47.000000 algophon-0.1.0/algophon.egg-info/PKG-INFO
+-rw-r--r--   0 u6052607   (503) staff       (20)      827 2024-05-24 00:10:47.000000 algophon-0.1.0/algophon.egg-info/SOURCES.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)        1 2024-05-24 00:10:47.000000 algophon-0.1.0/algophon.egg-info/dependency_links.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)       12 2024-05-24 00:10:47.000000 algophon-0.1.0/algophon.egg-info/requires.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)        9 2024-05-24 00:10:47.000000 algophon-0.1.0/algophon.egg-info/top_level.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)      829 2024-05-24 00:09:59.000000 algophon-0.1.0/pyproject.toml
+-rw-r--r--   0 u6052607   (503) staff       (20)       38 2024-05-24 00:10:47.826659 algophon-0.1.0/setup.cfg
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-24 00:10:47.821769 algophon-0.1.0/tests/
+-rw-r--r--   0 u6052607   (503) staff       (20)    29575 2024-05-24 00:09:59.000000 algophon-0.1.0/tests/test_d2l.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1240 2024-05-05 22:45:04.000000 algophon-0.1.0/tests/test_distance.py
+-rw-r--r--   0 u6052607   (503) staff       (20)      860 2024-04-19 00:19:07.000000 algophon-0.1.0/tests/test_natclass.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     2123 2024-05-24 00:09:59.000000 algophon-0.1.0/tests/test_seg.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     4553 2024-05-24 00:09:59.000000 algophon-0.1.0/tests/test_seginv.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1941 2024-04-24 23:29:27.000000 algophon-0.1.0/tests/test_segstr.py
+-rw-r--r--   0 u6052607   (503) staff       (20)      645 2024-05-24 00:09:59.000000 algophon-0.1.0/tests/test_utils.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1132 2024-05-24 00:09:59.000000 algophon-0.1.0/tests/tester.py
```

### Comparing `algophon-0.0.9/LICENSE` & `algophon-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `algophon-0.0.9/PKG-INFO` & `algophon-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,104 +1,88 @@
-Metadata-Version: 2.1
-Name: algophon
-Version: 0.0.9
-Summary: Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)
-Author: Caleb Belth
-License: Apache 2.0
-Project-URL: Homepage, https://github.com/cbelth/algophon
-Keywords: computational linguistics,phonology,morphology,natural language processing
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy>=1.24
-
 # algophon
 
 **Code for working on computational phonology and morphology in Python.** 
 
 The project is based on code developed by [Caleb Belth](https://cbelth.github.io/) during the course of his PhD; the title of his [dissertation](https://cbelth.github.io/public/assets/documents/belth_dissertation.pdf), *Towards an Algorithmic Account of Phonological Rules and Representations*, serves as the origin for the repository's name *algophon*.
 
-This is a <span style="color:orange">work in progress</span>. The pypi distribution and documentation will be updated as the project progresses! The initial plan for the project is to include:
+This is a <span style="color:orange">work in progress</span>. The PyPI distribution and documentation will be updated as the project progresses! The initial plan for the project is to include:
 1. Handy tools for working with strings of phonological segments.
 2. Implementations of computational learning models.
 
 Item (1) will be implemented first.
 
 **Suggestions are welcome!**
 
 ## Install
 
-```
+```bash
 pip install algophon
 ```
 
 ## Working With Strings of Segments
 
 The code at the top level of the package provides some nice functionality for easily working with strings of phonological segments.
 
 The following examples assume you have imported the appropriate classes:
 
-```python
+```pycon
 >>> from algophon import Seg, SegInv, SegStr, NatClass
 ```
 
 ### Segments: `Seg`
 
 **A class to represent a phonological segment.**
 
 You are unlikely to be creating `Seg` objects yourself very often. They will usually be constructed internally by other parts of the package (in particular, see `SegInv` and `SegStr`). However, if you ever need to, creating a `Seg` object requires the following arguments:
 - `ipa`: a `str` IPA symbol
 - `features` (optional): a `dict` of features mapping to their corresponding values
 
-```python
+```pycon
 >>> seg = Seg(ipa='i', features={'syl': '+', 'voi': '+', 'stri': '0'})
 ```
 
 What is important to know is how `Seg` objects behave, and why they are handy.
 
 <span style="color:green">**First**</span>, in the important respects `Seg` behaves like the `str` IPA segment used to create it.
 
 If you `print` a `Seg` object, it will print its IPA:
 
-```python
+```pycon
 >>> print(seg)
 i
 ```
 
 If you compare a `Seg` object to a `str`, it will behave like it is the IPA symbol:
 
-```python
+```pycon
 >>> print(seg == 'i')
 True
 >>> print(seg == 'e')
 False
 ```
 
 A `Seg` object hashes to the same value as its IPA symbol:
 
-```python
+```pycon
 >>> print(len({seg, 'i'}))
 1
 >>> print('i' in {seg}, seg in {'i'})
 True True
 ```
 
 <span style="color:green">**Second**</span>, in the important respects `Seg` behaves like a feature bundle (see also the other classes, where other benefits will become clear).
 
-```python
+```pycon
 >>> print(seg.features['syl'])
 +
 ```
 
-<span style="color:green">**Third**</span>, `Seg` handles IPA symbols that are longer than one unicode char.
+<span style="color:green">**Third**</span>, `Seg` handles IPA symbols that are longer than one Unicode char.
 
-```python
+```pycon
 >>> tsh = Seg(ipa='t͡ʃ')
 >>> print(tsh)
 t͡ʃ
 >>> print(len(tsh))
 1
 >>> from algophon.symbols import LONG # see description of symbols below
 >>> long_i = Seg(ipa=f'i{LONG}')
@@ -115,50 +99,50 @@
 A `SegInv` object is a collection of `Seg` objects. A `SegInv` requires no arguments to construct, though it provides two optional arguments:
 - `ipa_file_path`: a `str` pointing to a file of segment-feature mappings.
 - `sep`: a `str` specifying the column separator of the `ipa_file_path` file.
 
 By default, `SegInv` uses [Panphon](https://github.com/dmort27/panphon) (Mortensen et. al., 2016) features. The optional parameters allow you to use your own features. The file at `ipa_file_path` must be formatted like this:
 - The first row must be a header of feature names, separated by the `sep` (by default, `\t`)
 - The first column must contain the segment IPAs (the header row can have anything, e.g., `SEG`)
-- The remaining columns (non first row) must contain the feature values.
+- The remaining columns (non-first row) must contain the feature values.
 
 When a `SegInv` object is created, it is empty:
 
-```python
+```pycon
 >>> seginv = SegInv()
 >>> seginv
 SegInv of size 0
 ```
 
 You can add segments by the `add`, `add_segments`, and `add_segments_by_str` methods:
 
-```python
+```pycon
 >>> seginv.add('i')
 >>> print(seginv.segs)
 {i}
 >>> seginv.add_segs({'p', 'b', 't', 'd'})
 >>> print(seginv.segs)
 {b, t, d, i, p}
 >>> seginv.add_segs_by_str('eː n t j ə') # segments in str must be space-separated
 >>> print(seginv.segs)
 {b, t, d, i, j, n, p, ə, eː}
 ```
 
-The reason that `add_segs_by_str` requires the segments be space-separated is because not all IPA symbols are only one char (e.g., `'eː'`). Moreover, this is consistent with the [Sigmorphon](https://github.com/sigmorphon) challenges data format commonly used in morphophonology tasks.
+The reason that `add_segs_by_str` requires the segments to be space-separated is because not all IPA symbols are only one char (e.g., `'eː'`). Moreover, this is consistent with the [Sigmorphon](https://github.com/sigmorphon) challenges data format commonly used in morphophonology tasks.
 
 These `add*` methods automatically create `Seg` objects and assign them `features` based on either Panphon (default) or the `ipa_file_path` file.
 
-```python
+```pycon
 >>> print(seginv['eː'].features)
 {'syl': '+', 'son': '+', 'cons': '-', 'cont': '+', 'delrel': '-', 'lat': '-', 'nas': '-', 'strid': '0', 'voi': '+', 'sg': '-', 'cg': '-', 'ant': '0', 'cor': '-', 'distr': '0', 'lab': '-', 'hi': '-', 'lo': '-', 'back': '-', 'round': '-', 'velaric': '-', 'tense': '+', 'long': '+', 'hitone': '0', 'hireg': '0'}
 ```
 
 This also demonstrates that `seginv` operates like a dictionary in that you can retrieve and check the existence of segments by their IPA.
 
-```python
+```pycon
 >>> 'eː' in seginv
 True
 ```
 
 ### Strings of Segments: `SegStr`
 
 **A class to represent a sequence of phonological segments (Seg objects).**
@@ -168,31 +152,31 @@
 Creating a `SegStr` object requires the following arguments:
   - `segs`: a collection of segments, which can be in any of the following formats:
     - str of IPA symbols, where each symbol is separated by a space ' ' (**most common**)
     - list of IPA symbols
     - list of Seg objects
   - `seginv`: a `SegInv` object
 
-```python
+```pycon
 >>> seginv = SegInv() # init SegInv
 >>> seq = SegStr('eː n t j ə', seginv)
 >>> print(seq)
 eːntjə
 ```
 
 Creating the `SegStr` object automatically adds the segments in the object to the `SegInv` object.
 
-```python
+```pycon
 >>> print(seginv.segs)
 {ə, t, n, j, eː}
 ```
 
-For clean visuzliation, `SegStr` displays the sequence of segments without spaces, as `print(seq)` shows above. But internally a `SegStr` object knows what the segments are:
+For clean visualization, `SegStr` displays the sequence of segments without spaces, as `print(seq)` shows above. But internally a `SegStr` object knows what the segments are:
 
-```python
+```pycon
 >>> print(len(seq))
 5
 >>> seq[0]
 eː
 >>> type(seq[0]) # indexing returns a Seg object
 <class 'algophon.seg.Seg'>
 >>> seq[-2:]
@@ -201,72 +185,72 @@
 <class 'algophon.segstr.SegStr'>
 >>> seq[-2:] == 'j ə' # comparison to str objects works as expected
 True
 >>> seq[-2:] == 'ə n'
 False
 ```
 
-`SegStr` also implements equivalents of useful str methods.
+`SegStr` also implements equivalents of useful `str` methods.
 
-```python
+```pycon
 >>> seq.endswith('j ə')
 True
 >>> dim_sufx = seq[-2:]
 >>> seq.endswith(dim_sufx)
 True
 >>> seq.startswith(seq[:-2])
 True
 ```
 
 A `SegStr` object hashes to the value of its (space-separated) string:
 
-```python
+```pycon
 >>> len({seq, 'eː n t j ə'})
 1
 >>> seq in {'eː n t j ə'}
 True
 ```
 
 ### Natural Class: `NatClass`
 
 **A class to represent a Natural class, in the sense of sets of segments represented intensionally as conjunctions of features.**
 
-```python
+```pycon
 >>> son = NatClass(feats={'+son'}, seginv=seginv)
 >>> son
 [+son]
 >>> 'ə' in son
 True
 >>> 'n' in son
 True
 >>> 't' in son
 False
 ```
 
 The class also allows you to get the natural class's extension and the extension's complement, relative to the `SegInv` (in our example, only `{ə, t, n, j, eː}` are in `seginv`):
 
-```python
+```pycon
 >>> son.extension()
 {eː, j, ə, n}
 >>> son.extension_complement()
 {t}
 ```
 
 You can also retrieve an extension (complement) directly from a `SegInv` object without creating a `NatClass` obj:
 
-```python
+```pycon
 >>> seginv.extension({'+syl'})
 {ə, eː}
 >>> seginv.extension_complement({'+syl'})
 {j, t, n}
 ```
 
 ### Symbols: The `symbols` module
 
-The `symbols` module (techincally just a file...) contains a number of constant variables that store some useful symbols:
+The `symbols` module (technically just a file...) contains a number of constant variables that store some useful symbols:
 
 ```python
 LWB = '⋊'
 RWB = '⋉'
 SYL_BOUNDARY = '.'
 PRIMARY_STRESS = 'ˈ'
 SEC_STRESS = 'ˌ'
@@ -275,24 +259,51 @@
 UNDERSPECIFIED = '0'
 UNK = '?'
 NEG = '¬'
 ```
 
 These can be accessed like this:
 
-```python
+```pycon
 >>> from algophon.symbols import *
 >>> NASALIZED
 '̃'
 >>> f'i{LONG}'
 iː
 ```
 
 ## Learning Models
 
+### D2L
+
+An implementation of the model "Distant to Local" from the following paper:
+
+```
+@article{belth2024tiers,
+    title={A Learning-Based Account of Phonological Tiers},
+    author={Belth, Caleb},
+    journal={Linguistic Inquiry},
+    year={2024},
+    publisher={MIT Press},
+    url = {https://doi.org/10.1162/ling\_a\_00530},
+}
+```
+
+Please see the models [README](https://github.com/cbelth/algophon/blob/main/algophon/models/README.md) for details.
+
+### PLP
+
+<span style="color:orange">Work in Progress</span>
+
+### Miaseg
+
+<span style="color:orange">Work in Progress</span>
+
+### Other Models
+
 <span style="color:orange">Work in Progress</span>
 
 ## Citation
 
 If you use this package in your research, you can use the following citation:
 
 ```bibtex
```

### Comparing `algophon-0.0.9/README.md` & `algophon-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,88 +1,104 @@
+Metadata-Version: 2.1
+Name: algophon
+Version: 0.1.0
+Summary: Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)
+Author: Caleb Belth
+License: Apache 2.0
+Project-URL: Homepage, https://github.com/cbelth/algophon
+Keywords: computational linguistics,phonology,morphology,natural language processing
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.24
+
 # algophon
 
 **Code for working on computational phonology and morphology in Python.** 
 
 The project is based on code developed by [Caleb Belth](https://cbelth.github.io/) during the course of his PhD; the title of his [dissertation](https://cbelth.github.io/public/assets/documents/belth_dissertation.pdf), *Towards an Algorithmic Account of Phonological Rules and Representations*, serves as the origin for the repository's name *algophon*.
 
-This is a <span style="color:orange">work in progress</span>. The pypi distribution and documentation will be updated as the project progresses! The initial plan for the project is to include:
+This is a <span style="color:orange">work in progress</span>. The PyPI distribution and documentation will be updated as the project progresses! The initial plan for the project is to include:
 1. Handy tools for working with strings of phonological segments.
 2. Implementations of computational learning models.
 
 Item (1) will be implemented first.
 
 **Suggestions are welcome!**
 
 ## Install
 
-```
+```bash
 pip install algophon
 ```
 
 ## Working With Strings of Segments
 
 The code at the top level of the package provides some nice functionality for easily working with strings of phonological segments.
 
 The following examples assume you have imported the appropriate classes:
 
-```python
+```pycon
 >>> from algophon import Seg, SegInv, SegStr, NatClass
 ```
 
 ### Segments: `Seg`
 
 **A class to represent a phonological segment.**
 
 You are unlikely to be creating `Seg` objects yourself very often. They will usually be constructed internally by other parts of the package (in particular, see `SegInv` and `SegStr`). However, if you ever need to, creating a `Seg` object requires the following arguments:
 - `ipa`: a `str` IPA symbol
 - `features` (optional): a `dict` of features mapping to their corresponding values
 
-```python
+```pycon
 >>> seg = Seg(ipa='i', features={'syl': '+', 'voi': '+', 'stri': '0'})
 ```
 
 What is important to know is how `Seg` objects behave, and why they are handy.
 
 <span style="color:green">**First**</span>, in the important respects `Seg` behaves like the `str` IPA segment used to create it.
 
 If you `print` a `Seg` object, it will print its IPA:
 
-```python
+```pycon
 >>> print(seg)
 i
 ```
 
 If you compare a `Seg` object to a `str`, it will behave like it is the IPA symbol:
 
-```python
+```pycon
 >>> print(seg == 'i')
 True
 >>> print(seg == 'e')
 False
 ```
 
 A `Seg` object hashes to the same value as its IPA symbol:
 
-```python
+```pycon
 >>> print(len({seg, 'i'}))
 1
 >>> print('i' in {seg}, seg in {'i'})
 True True
 ```
 
 <span style="color:green">**Second**</span>, in the important respects `Seg` behaves like a feature bundle (see also the other classes, where other benefits will become clear).
 
-```python
+```pycon
 >>> print(seg.features['syl'])
 +
 ```
 
-<span style="color:green">**Third**</span>, `Seg` handles IPA symbols that are longer than one unicode char.
+<span style="color:green">**Third**</span>, `Seg` handles IPA symbols that are longer than one Unicode char.
 
-```python
+```pycon
 >>> tsh = Seg(ipa='t͡ʃ')
 >>> print(tsh)
 t͡ʃ
 >>> print(len(tsh))
 1
 >>> from algophon.symbols import LONG # see description of symbols below
 >>> long_i = Seg(ipa=f'i{LONG}')
@@ -99,50 +115,50 @@
 A `SegInv` object is a collection of `Seg` objects. A `SegInv` requires no arguments to construct, though it provides two optional arguments:
 - `ipa_file_path`: a `str` pointing to a file of segment-feature mappings.
 - `sep`: a `str` specifying the column separator of the `ipa_file_path` file.
 
 By default, `SegInv` uses [Panphon](https://github.com/dmort27/panphon) (Mortensen et. al., 2016) features. The optional parameters allow you to use your own features. The file at `ipa_file_path` must be formatted like this:
 - The first row must be a header of feature names, separated by the `sep` (by default, `\t`)
 - The first column must contain the segment IPAs (the header row can have anything, e.g., `SEG`)
-- The remaining columns (non first row) must contain the feature values.
+- The remaining columns (non-first row) must contain the feature values.
 
 When a `SegInv` object is created, it is empty:
 
-```python
+```pycon
 >>> seginv = SegInv()
 >>> seginv
 SegInv of size 0
 ```
 
 You can add segments by the `add`, `add_segments`, and `add_segments_by_str` methods:
 
-```python
+```pycon
 >>> seginv.add('i')
 >>> print(seginv.segs)
 {i}
 >>> seginv.add_segs({'p', 'b', 't', 'd'})
 >>> print(seginv.segs)
 {b, t, d, i, p}
 >>> seginv.add_segs_by_str('eː n t j ə') # segments in str must be space-separated
 >>> print(seginv.segs)
 {b, t, d, i, j, n, p, ə, eː}
 ```
 
-The reason that `add_segs_by_str` requires the segments be space-separated is because not all IPA symbols are only one char (e.g., `'eː'`). Moreover, this is consistent with the [Sigmorphon](https://github.com/sigmorphon) challenges data format commonly used in morphophonology tasks.
+The reason that `add_segs_by_str` requires the segments to be space-separated is because not all IPA symbols are only one char (e.g., `'eː'`). Moreover, this is consistent with the [Sigmorphon](https://github.com/sigmorphon) challenges data format commonly used in morphophonology tasks.
 
 These `add*` methods automatically create `Seg` objects and assign them `features` based on either Panphon (default) or the `ipa_file_path` file.
 
-```python
+```pycon
 >>> print(seginv['eː'].features)
 {'syl': '+', 'son': '+', 'cons': '-', 'cont': '+', 'delrel': '-', 'lat': '-', 'nas': '-', 'strid': '0', 'voi': '+', 'sg': '-', 'cg': '-', 'ant': '0', 'cor': '-', 'distr': '0', 'lab': '-', 'hi': '-', 'lo': '-', 'back': '-', 'round': '-', 'velaric': '-', 'tense': '+', 'long': '+', 'hitone': '0', 'hireg': '0'}
 ```
 
 This also demonstrates that `seginv` operates like a dictionary in that you can retrieve and check the existence of segments by their IPA.
 
-```python
+```pycon
 >>> 'eː' in seginv
 True
 ```
 
 ### Strings of Segments: `SegStr`
 
 **A class to represent a sequence of phonological segments (Seg objects).**
@@ -152,31 +168,31 @@
 Creating a `SegStr` object requires the following arguments:
   - `segs`: a collection of segments, which can be in any of the following formats:
     - str of IPA symbols, where each symbol is separated by a space ' ' (**most common**)
     - list of IPA symbols
     - list of Seg objects
   - `seginv`: a `SegInv` object
 
-```python
+```pycon
 >>> seginv = SegInv() # init SegInv
 >>> seq = SegStr('eː n t j ə', seginv)
 >>> print(seq)
 eːntjə
 ```
 
 Creating the `SegStr` object automatically adds the segments in the object to the `SegInv` object.
 
-```python
+```pycon
 >>> print(seginv.segs)
 {ə, t, n, j, eː}
 ```
 
-For clean visuzliation, `SegStr` displays the sequence of segments without spaces, as `print(seq)` shows above. But internally a `SegStr` object knows what the segments are:
+For clean visualization, `SegStr` displays the sequence of segments without spaces, as `print(seq)` shows above. But internally a `SegStr` object knows what the segments are:
 
-```python
+```pycon
 >>> print(len(seq))
 5
 >>> seq[0]
 eː
 >>> type(seq[0]) # indexing returns a Seg object
 <class 'algophon.seg.Seg'>
 >>> seq[-2:]
@@ -185,72 +201,72 @@
 <class 'algophon.segstr.SegStr'>
 >>> seq[-2:] == 'j ə' # comparison to str objects works as expected
 True
 >>> seq[-2:] == 'ə n'
 False
 ```
 
-`SegStr` also implements equivalents of useful str methods.
+`SegStr` also implements equivalents of useful `str` methods.
 
-```python
+```pycon
 >>> seq.endswith('j ə')
 True
 >>> dim_sufx = seq[-2:]
 >>> seq.endswith(dim_sufx)
 True
 >>> seq.startswith(seq[:-2])
 True
 ```
 
 A `SegStr` object hashes to the value of its (space-separated) string:
 
-```python
+```pycon
 >>> len({seq, 'eː n t j ə'})
 1
 >>> seq in {'eː n t j ə'}
 True
 ```
 
 ### Natural Class: `NatClass`
 
 **A class to represent a Natural class, in the sense of sets of segments represented intensionally as conjunctions of features.**
 
-```python
+```pycon
 >>> son = NatClass(feats={'+son'}, seginv=seginv)
 >>> son
 [+son]
 >>> 'ə' in son
 True
 >>> 'n' in son
 True
 >>> 't' in son
 False
 ```
 
 The class also allows you to get the natural class's extension and the extension's complement, relative to the `SegInv` (in our example, only `{ə, t, n, j, eː}` are in `seginv`):
 
-```python
+```pycon
 >>> son.extension()
 {eː, j, ə, n}
 >>> son.extension_complement()
 {t}
 ```
 
 You can also retrieve an extension (complement) directly from a `SegInv` object without creating a `NatClass` obj:
 
-```python
+```pycon
 >>> seginv.extension({'+syl'})
 {ə, eː}
 >>> seginv.extension_complement({'+syl'})
 {j, t, n}
 ```
 
 ### Symbols: The `symbols` module
 
-The `symbols` module (techincally just a file...) contains a number of constant variables that store some useful symbols:
+The `symbols` module (technically just a file...) contains a number of constant variables that store some useful symbols:
 
 ```python
 LWB = '⋊'
 RWB = '⋉'
 SYL_BOUNDARY = '.'
 PRIMARY_STRESS = 'ˈ'
 SEC_STRESS = 'ˌ'
@@ -259,24 +275,51 @@
 UNDERSPECIFIED = '0'
 UNK = '?'
 NEG = '¬'
 ```
 
 These can be accessed like this:
 
-```python
+```pycon
 >>> from algophon.symbols import *
 >>> NASALIZED
 '̃'
 >>> f'i{LONG}'
 iː
 ```
 
 ## Learning Models
 
+### D2L
+
+An implementation of the model "Distant to Local" from the following paper:
+
+```
+@article{belth2024tiers,
+    title={A Learning-Based Account of Phonological Tiers},
+    author={Belth, Caleb},
+    journal={Linguistic Inquiry},
+    year={2024},
+    publisher={MIT Press},
+    url = {https://doi.org/10.1162/ling\_a\_00530},
+}
+```
+
+Please see the models [README](https://github.com/cbelth/algophon/blob/main/algophon/models/README.md) for details.
+
+### PLP
+
+<span style="color:orange">Work in Progress</span>
+
+### Miaseg
+
+<span style="color:orange">Work in Progress</span>
+
+### Other Models
+
 <span style="color:orange">Work in Progress</span>
 
 ## Citation
 
 If you use this package in your research, you can use the following citation:
 
 ```bibtex
@@ -286,8 +329,8 @@
   year={2023},
   school={{University of Michigan}}
 }
 ```
 
 ## References
 
-- Mortensen, D. R., Littell, P., Bharadwaj, A., Goyal, K., Dyer, C., & Levin, L. (2016, December). Panphon: A resource for mapping IPA segments to articulatory feature vectors. In Proceedings of COLING 2016, the 26th International Conference on Computational Linguistics: Technical Papers (pp. 3475-3484).
+- Mortensen, D. R., Littell, P., Bharadwaj, A., Goyal, K., Dyer, C., & Levin, L. (2016, December). Panphon: A resource for mapping IPA segments to articulatory feature vectors. In Proceedings of COLING 2016, the 26th International Conference on Computational Linguistics: Technical Papers (pp. 3475-3484).
```

### Comparing `algophon-0.0.9/algophon/distance/edit_distance.py` & `algophon-0.1.0/algophon/distance/edit_distance.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.9/algophon/ipa/convert.py` & `algophon-0.1.0/algophon/ipa/convert.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.9/algophon/ipa.txt` & `algophon-0.1.0/algophon/ipa.txt`

 * *Files identical despite different names*

### Comparing `algophon-0.0.9/algophon/natclass.py` & `algophon-0.1.0/algophon/natclass.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.9/algophon/seginv.py` & `algophon-0.1.0/algophon/seginv.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,45 @@
+from typing import Union
+
 from algophon.seg import Seg
 from algophon.natclass import NatClass
-from algophon.symbols import UNDERSPECIFIED
+from algophon.symbols import UNDERSPECIFIED, BOUNDARIES
 
 import pkgutil
 
 class SegInv:
     '''
     A class representing an inventory of phonological segments (Seg objects).
     '''
     def __init__(self, 
-                 ipa_file_path: str=None, 
+                 add_boundary_symbols: bool=False,
+                 ipa_file_path: Union[None, str]=None, 
                  sep: str='\t'
-        ):
+        ) -> object:
+        '''
+        :add_boundary_symbols: (Optional; default False) if True, adds boundary symbols (e.g., syllabe boundaries) as Seg objects
+        :ipa_file_path: (Optional; default None) if a str path is passed, the features are used from there
+            - Default of None uses Panphon (https://github.com/dmort27/panphon) features
+        :sep: (Optional; default '\t') the char separating columns in :ipa_file_path:
+            - Only used if :ipa_file_path: is also passed
+        '''
         self._ipa_source = f'Panphon (https://github.com/dmort27/panphon)' if ipa_file_path is None else ipa_file_path
+        self._add_boundary_symbols = add_boundary_symbols
         self.ipa_file_path = ipa_file_path # uses Panphon features (https://github.com/dmort27/panphon) by default
         self.sep = sep
 
-        # load the _seg_to_feat_vec map
-        self._load_seg_to_feat_dict()
-
         # stores the Seg objects in the SegInv
         self.segs = set()
-
         # maps ipa symbols to their Seg object in the SegInv
         self._ipa_to_seg = dict()
 
+        # load the _seg_to_feat_vec map
+        self._load_seg_to_feat_dict()
+
+
     def __str__(self) -> str:
         return f'SegInv of size {len(self)}'
     
     def __repr__(self) -> str:
         return self.__str__()
     
     def __len__(self) -> int:
@@ -70,20 +81,29 @@
                 lines = f.readlines()
         for i, line in enumerate(lines): # iterate over lines
             line = line.strip().split(self.sep)
             seg, feats = line[0], line[1:] # extract the IPA segment and its features
             if i == 0: # extract the header
                 self.feature_space = feats
             else: # add the segment to the dict
+                if self._add_boundary_symbols:
+                    feats += ['-', '-', '-', '-', '-']
                 self._seg_to_feat_vec[seg] = feats
 
         if self.ipa_file_path is None:
             # make ord('g') == 103 and ord('ɡ') == 609 the same, since panphon only as 609
             self._seg_to_feat_vec['g'] = self._seg_to_feat_vec['ɡ']
 
+        if self._add_boundary_symbols: # add boundary symbols
+            self.feature_space += ['B', 'LWB', 'RWB', 'SYLB', 'MORPHB']
+            for boundary_feat, symbol in zip(['LWB', 'RWB', 'SYLB', 'MORPHB'], 
+                                             BOUNDARIES):
+                feats = dict((feat, UNDERSPECIFIED if feat not in {'B', 'LWB', 'RWB', 'SYLB', 'MORPHB'} else '+' if feat in {'B', boundary_feat} else '-') for feat in self.feature_space)
+                self.add_custom(symbol=symbol, features=feats)
+
     def add(self, ipa_seg: str) -> None:
         '''
         :ipa_seg: an IPA segment in str form
 
         :return: None
         '''
         if ipa_seg in self:
@@ -120,14 +140,33 @@
         :seg: an IPA segment in str form or a Seg object
 
         :return: the Seg object corresponding to the IPA seg
         '''
         self.add(f'{seg}')
         return self[seg]
     
+    def add_custom(self, symbol: str, features: dict) -> None:
+        '''
+        Adds a custom symbol (i.e., not one in the IPA inventory used to create the SegInv).
+        Useful for abstract segments like /S/ for {[s], [ʃ]}.
+
+        :symbol: A str to use as a symbol shorthand for the Seg
+        :features: a dictionary feature -> value mapping
+            - Features must exactly match those in self.feature_space
+
+        :return: None
+        '''
+        if symbol in self._seg_to_feat_vec:
+            raise ValueError(f'The symbol "{symbol}" is already a symbol in the IPA data from {self._ipa_source}.')
+        if set(features.keys()) != set(self.feature_space):
+            raise ValueError('The features do not match those in the feature space.')
+        seg = Seg(ipa=symbol, features=features)
+        self.segs.add(seg)
+        self._ipa_to_seg[symbol] = seg
+    
     def extension(self, nat_class) -> set:
         '''
         :nat_class: a set of features or a NatClass object
 
         :return: the extension of the :nat_class:
         '''
         if type(nat_class) is set:
```

### Comparing `algophon-0.0.9/algophon/segstr.py` & `algophon-0.1.0/algophon/segstr.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.9/algophon.egg-info/PKG-INFO` & `algophon-0.1.0/algophon.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algophon
-Version: 0.0.9
+Version: 0.1.0
 Summary: Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)
 Author: Caleb Belth
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/cbelth/algophon
 Keywords: computational linguistics,phonology,morphology,natural language processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,89 +16,89 @@
 
 # algophon
 
 **Code for working on computational phonology and morphology in Python.** 
 
 The project is based on code developed by [Caleb Belth](https://cbelth.github.io/) during the course of his PhD; the title of his [dissertation](https://cbelth.github.io/public/assets/documents/belth_dissertation.pdf), *Towards an Algorithmic Account of Phonological Rules and Representations*, serves as the origin for the repository's name *algophon*.
 
-This is a <span style="color:orange">work in progress</span>. The pypi distribution and documentation will be updated as the project progresses! The initial plan for the project is to include:
+This is a <span style="color:orange">work in progress</span>. The PyPI distribution and documentation will be updated as the project progresses! The initial plan for the project is to include:
 1. Handy tools for working with strings of phonological segments.
 2. Implementations of computational learning models.
 
 Item (1) will be implemented first.
 
 **Suggestions are welcome!**
 
 ## Install
 
-```
+```bash
 pip install algophon
 ```
 
 ## Working With Strings of Segments
 
 The code at the top level of the package provides some nice functionality for easily working with strings of phonological segments.
 
 The following examples assume you have imported the appropriate classes:
 
-```python
+```pycon
 >>> from algophon import Seg, SegInv, SegStr, NatClass
 ```
 
 ### Segments: `Seg`
 
 **A class to represent a phonological segment.**
 
 You are unlikely to be creating `Seg` objects yourself very often. They will usually be constructed internally by other parts of the package (in particular, see `SegInv` and `SegStr`). However, if you ever need to, creating a `Seg` object requires the following arguments:
 - `ipa`: a `str` IPA symbol
 - `features` (optional): a `dict` of features mapping to their corresponding values
 
-```python
+```pycon
 >>> seg = Seg(ipa='i', features={'syl': '+', 'voi': '+', 'stri': '0'})
 ```
 
 What is important to know is how `Seg` objects behave, and why they are handy.
 
 <span style="color:green">**First**</span>, in the important respects `Seg` behaves like the `str` IPA segment used to create it.
 
 If you `print` a `Seg` object, it will print its IPA:
 
-```python
+```pycon
 >>> print(seg)
 i
 ```
 
 If you compare a `Seg` object to a `str`, it will behave like it is the IPA symbol:
 
-```python
+```pycon
 >>> print(seg == 'i')
 True
 >>> print(seg == 'e')
 False
 ```
 
 A `Seg` object hashes to the same value as its IPA symbol:
 
-```python
+```pycon
 >>> print(len({seg, 'i'}))
 1
 >>> print('i' in {seg}, seg in {'i'})
 True True
 ```
 
 <span style="color:green">**Second**</span>, in the important respects `Seg` behaves like a feature bundle (see also the other classes, where other benefits will become clear).
 
-```python
+```pycon
 >>> print(seg.features['syl'])
 +
 ```
 
-<span style="color:green">**Third**</span>, `Seg` handles IPA symbols that are longer than one unicode char.
+<span style="color:green">**Third**</span>, `Seg` handles IPA symbols that are longer than one Unicode char.
 
-```python
+```pycon
 >>> tsh = Seg(ipa='t͡ʃ')
 >>> print(tsh)
 t͡ʃ
 >>> print(len(tsh))
 1
 >>> from algophon.symbols import LONG # see description of symbols below
 >>> long_i = Seg(ipa=f'i{LONG}')
@@ -115,50 +115,50 @@
 A `SegInv` object is a collection of `Seg` objects. A `SegInv` requires no arguments to construct, though it provides two optional arguments:
 - `ipa_file_path`: a `str` pointing to a file of segment-feature mappings.
 - `sep`: a `str` specifying the column separator of the `ipa_file_path` file.
 
 By default, `SegInv` uses [Panphon](https://github.com/dmort27/panphon) (Mortensen et. al., 2016) features. The optional parameters allow you to use your own features. The file at `ipa_file_path` must be formatted like this:
 - The first row must be a header of feature names, separated by the `sep` (by default, `\t`)
 - The first column must contain the segment IPAs (the header row can have anything, e.g., `SEG`)
-- The remaining columns (non first row) must contain the feature values.
+- The remaining columns (non-first row) must contain the feature values.
 
 When a `SegInv` object is created, it is empty:
 
-```python
+```pycon
 >>> seginv = SegInv()
 >>> seginv
 SegInv of size 0
 ```
 
 You can add segments by the `add`, `add_segments`, and `add_segments_by_str` methods:
 
-```python
+```pycon
 >>> seginv.add('i')
 >>> print(seginv.segs)
 {i}
 >>> seginv.add_segs({'p', 'b', 't', 'd'})
 >>> print(seginv.segs)
 {b, t, d, i, p}
 >>> seginv.add_segs_by_str('eː n t j ə') # segments in str must be space-separated
 >>> print(seginv.segs)
 {b, t, d, i, j, n, p, ə, eː}
 ```
 
-The reason that `add_segs_by_str` requires the segments be space-separated is because not all IPA symbols are only one char (e.g., `'eː'`). Moreover, this is consistent with the [Sigmorphon](https://github.com/sigmorphon) challenges data format commonly used in morphophonology tasks.
+The reason that `add_segs_by_str` requires the segments to be space-separated is because not all IPA symbols are only one char (e.g., `'eː'`). Moreover, this is consistent with the [Sigmorphon](https://github.com/sigmorphon) challenges data format commonly used in morphophonology tasks.
 
 These `add*` methods automatically create `Seg` objects and assign them `features` based on either Panphon (default) or the `ipa_file_path` file.
 
-```python
+```pycon
 >>> print(seginv['eː'].features)
 {'syl': '+', 'son': '+', 'cons': '-', 'cont': '+', 'delrel': '-', 'lat': '-', 'nas': '-', 'strid': '0', 'voi': '+', 'sg': '-', 'cg': '-', 'ant': '0', 'cor': '-', 'distr': '0', 'lab': '-', 'hi': '-', 'lo': '-', 'back': '-', 'round': '-', 'velaric': '-', 'tense': '+', 'long': '+', 'hitone': '0', 'hireg': '0'}
 ```
 
 This also demonstrates that `seginv` operates like a dictionary in that you can retrieve and check the existence of segments by their IPA.
 
-```python
+```pycon
 >>> 'eː' in seginv
 True
 ```
 
 ### Strings of Segments: `SegStr`
 
 **A class to represent a sequence of phonological segments (Seg objects).**
@@ -168,31 +168,31 @@
 Creating a `SegStr` object requires the following arguments:
   - `segs`: a collection of segments, which can be in any of the following formats:
     - str of IPA symbols, where each symbol is separated by a space ' ' (**most common**)
     - list of IPA symbols
     - list of Seg objects
   - `seginv`: a `SegInv` object
 
-```python
+```pycon
 >>> seginv = SegInv() # init SegInv
 >>> seq = SegStr('eː n t j ə', seginv)
 >>> print(seq)
 eːntjə
 ```
 
 Creating the `SegStr` object automatically adds the segments in the object to the `SegInv` object.
 
-```python
+```pycon
 >>> print(seginv.segs)
 {ə, t, n, j, eː}
 ```
 
-For clean visuzliation, `SegStr` displays the sequence of segments without spaces, as `print(seq)` shows above. But internally a `SegStr` object knows what the segments are:
+For clean visualization, `SegStr` displays the sequence of segments without spaces, as `print(seq)` shows above. But internally a `SegStr` object knows what the segments are:
 
-```python
+```pycon
 >>> print(len(seq))
 5
 >>> seq[0]
 eː
 >>> type(seq[0]) # indexing returns a Seg object
 <class 'algophon.seg.Seg'>
 >>> seq[-2:]
@@ -201,72 +201,72 @@
 <class 'algophon.segstr.SegStr'>
 >>> seq[-2:] == 'j ə' # comparison to str objects works as expected
 True
 >>> seq[-2:] == 'ə n'
 False
 ```
 
-`SegStr` also implements equivalents of useful str methods.
+`SegStr` also implements equivalents of useful `str` methods.
 
-```python
+```pycon
 >>> seq.endswith('j ə')
 True
 >>> dim_sufx = seq[-2:]
 >>> seq.endswith(dim_sufx)
 True
 >>> seq.startswith(seq[:-2])
 True
 ```
 
 A `SegStr` object hashes to the value of its (space-separated) string:
 
-```python
+```pycon
 >>> len({seq, 'eː n t j ə'})
 1
 >>> seq in {'eː n t j ə'}
 True
 ```
 
 ### Natural Class: `NatClass`
 
 **A class to represent a Natural class, in the sense of sets of segments represented intensionally as conjunctions of features.**
 
-```python
+```pycon
 >>> son = NatClass(feats={'+son'}, seginv=seginv)
 >>> son
 [+son]
 >>> 'ə' in son
 True
 >>> 'n' in son
 True
 >>> 't' in son
 False
 ```
 
 The class also allows you to get the natural class's extension and the extension's complement, relative to the `SegInv` (in our example, only `{ə, t, n, j, eː}` are in `seginv`):
 
-```python
+```pycon
 >>> son.extension()
 {eː, j, ə, n}
 >>> son.extension_complement()
 {t}
 ```
 
 You can also retrieve an extension (complement) directly from a `SegInv` object without creating a `NatClass` obj:
 
-```python
+```pycon
 >>> seginv.extension({'+syl'})
 {ə, eː}
 >>> seginv.extension_complement({'+syl'})
 {j, t, n}
 ```
 
 ### Symbols: The `symbols` module
 
-The `symbols` module (techincally just a file...) contains a number of constant variables that store some useful symbols:
+The `symbols` module (technically just a file...) contains a number of constant variables that store some useful symbols:
 
 ```python
 LWB = '⋊'
 RWB = '⋉'
 SYL_BOUNDARY = '.'
 PRIMARY_STRESS = 'ˈ'
 SEC_STRESS = 'ˌ'
@@ -275,24 +275,51 @@
 UNDERSPECIFIED = '0'
 UNK = '?'
 NEG = '¬'
 ```
 
 These can be accessed like this:
 
-```python
+```pycon
 >>> from algophon.symbols import *
 >>> NASALIZED
 '̃'
 >>> f'i{LONG}'
 iː
 ```
 
 ## Learning Models
 
+### D2L
+
+An implementation of the model "Distant to Local" from the following paper:
+
+```
+@article{belth2024tiers,
+    title={A Learning-Based Account of Phonological Tiers},
+    author={Belth, Caleb},
+    journal={Linguistic Inquiry},
+    year={2024},
+    publisher={MIT Press},
+    url = {https://doi.org/10.1162/ling\_a\_00530},
+}
+```
+
+Please see the models [README](https://github.com/cbelth/algophon/blob/main/algophon/models/README.md) for details.
+
+### PLP
+
+<span style="color:orange">Work in Progress</span>
+
+### Miaseg
+
+<span style="color:orange">Work in Progress</span>
+
+### Other Models
+
 <span style="color:orange">Work in Progress</span>
 
 ## Citation
 
 If you use this package in your research, you can use the following citation:
 
 ```bibtex
```

### Comparing `algophon-0.0.9/algophon.egg-info/SOURCES.txt` & `algophon-0.1.0/algophon.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -13,13 +13,23 @@
 algophon.egg-info/dependency_links.txt
 algophon.egg-info/requires.txt
 algophon.egg-info/top_level.txt
 algophon/distance/__init__.py
 algophon/distance/edit_distance.py
 algophon/ipa/__init__.py
 algophon/ipa/convert.py
+algophon/models/__init__.py
+algophon/models/D2L/__init__.py
+algophon/models/D2L/d2l.py
+algophon/models/D2L/discrepancy.py
+algophon/models/D2L/rule.py
+algophon/models/D2L/tier.py
+algophon/utils/__init__.py
+algophon/utils/utils.py
+tests/test_d2l.py
 tests/test_distance.py
 tests/test_natclass.py
 tests/test_seg.py
 tests/test_seginv.py
 tests/test_segstr.py
+tests/test_utils.py
 tests/tester.py
```

### Comparing `algophon-0.0.9/pyproject.toml` & `algophon-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "algophon"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
     { name = "Caleb Belth" },
 ]
 description = "Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "Apache 2.0" }
```

### Comparing `algophon-0.0.9/tests/test_distance.py` & `algophon-0.1.0/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.9/tests/test_natclass.py` & `algophon-0.1.0/tests/test_natclass.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.9/tests/test_seginv.py` & `algophon-0.1.0/tests/test_seginv.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,34 @@
 import unittest
 import sys
 sys.path.append('../')
 from algophon.seginv import SegInv
+from algophon.symbols import UNDERSPECIFIED, LWB
 
 class TestSegInv(unittest.TestCase):
     def test_init(self):
         seginv = SegInv()
         assert(seginv is not None)
 
+    def test_init_boundary(self):
+        seginv = SegInv(add_boundary_symbols=True)
+        assert(len(seginv) == 4)
+        assert(seginv.feature_space[-5:] == ['B', 'LWB', 'RWB', 'SYLB', 'MORPHB'])
+        assert(seginv[LWB].features['B'] == '+')
+        assert(seginv[LWB].features['syl'] == UNDERSPECIFIED)
+        assert(seginv[LWB].features['LWB'] == '+')
+        assert(seginv[LWB].features['RWB'] == '-')
+
+        seginv.add('i')
+        assert(seginv['i'].features['B'] == '-')
+        assert(seginv['i'].features['syl'] == '+')
+        assert(seginv['i'].features['LWB'] == '-')
+        assert(seginv['i'].features['RWB'] == '-')
+
+
     def test_add(self):
         seginv = SegInv()
         
         seginv.add('i')
         assert(len(seginv) == 1)
         assert(seginv.segs == {'i'}) 
 
@@ -19,14 +36,42 @@
         assert(len(seginv) == 5)
         assert(seginv.segs == {'i', 'p', 'b', 't', 'd'}) 
 
         seginv.add_segs_by_str('eː n t j ə')
         assert(len(seginv) == 9)
         assert(seginv.segs == {'i', 'p', 'b', 't', 'd', 'eː', 'n', 'j', 'ə'}) 
 
+    def test_add_custom(self):
+        seginv = SegInv()
+
+        seginv.add('s')
+        seginv.add('ʃ')
+
+        shared_feats = set(feat[1:] for feat in seginv.feature_intersection({'s', 'ʃ'}, exclude_underspecified=False))
+        feat_diff = set(seginv.feature_space).difference(shared_feats)
+        features = dict((feat, val if feat not in feat_diff else UNDERSPECIFIED) for feat, val in seginv['s'].features.items())
+
+        seginv.add_custom(symbol='S', features=features)
+        assert('S' in seginv)
+        assert(seginv['S'].features == features)
+
+        try:
+            seginv.add_custom(symbol='V', features={'voi': '+'})
+            assert(False)
+        except ValueError as e:
+            assert(True)
+            assert(e.__str__() == 'The features do not match those in the feature space.')
+
+        try:
+            seginv.add_custom(symbol='s', features=features)
+            assert(False)
+        except ValueError as e:
+            assert(True)
+            assert(e.__str__() == 'The symbol "s" is already a symbol in the IPA data from Panphon (https://github.com/dmort27/panphon).')
+
     def test_get(self):
         seginv = SegInv()
         seginv.add('eː')
         assert(seginv['eː'].features == {'syl': '+', 'son': '+', 'cons': '-', 'cont': '+', 'delrel': '-', 'lat': '-', 'nas': '-', 
                                          'strid': '0', 'voi': '+', 'sg': '-', 'cg': '-', 'ant': '0', 'cor': '-', 'distr': '0', 'lab': '-',
                                          'hi': '-', 'lo': '-', 'back': '-', 'round': '-', 'velaric': '-', 'tense': '+', 'long': '+', 
                                          'hitone': '0', 'hireg': '0'})
```

### Comparing `algophon-0.0.9/tests/test_segstr.py` & `algophon-0.1.0/tests/test_segstr.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.9/tests/tester.py` & `algophon-0.1.0/tests/tester.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import unittest
 from test_seg import TestSeg
 from test_seginv import TestSegInv
 from test_segstr import TestSegStr
 from test_natclass import TestNatClass
 from test_distance import TestDistance
+from test_utils import TestUtils
+from test_d2l import TestD2L
 
 '''
 A script to run all the test cases.
 '''
 # load test suites
 test_seg_suite = unittest.TestLoader().loadTestsFromTestCase(TestSeg)
 test_seginv_suite = unittest.TestLoader().loadTestsFromTestCase(TestSegInv)
 test_segstr_suite = unittest.TestLoader().loadTestsFromTestCase(TestSegStr)
 test_natclass_suite = unittest.TestLoader().loadTestsFromTestCase(TestNatClass)
 test_distance_suite = unittest.TestLoader().loadTestsFromTestCase(TestDistance)
+test_utils_suite = unittest.TestLoader().loadTestsFromTestCase(TestUtils)
+test_d2l_suite = unittest.TestLoader().loadTestsFromTestCase(TestD2L)
 # combine the test suites
 suites = unittest.TestSuite([
     test_seg_suite,
     test_seginv_suite,
     test_segstr_suite,
     test_natclass_suite,
-    test_distance_suite
+    test_distance_suite,
+    test_utils_suite,
+    test_d2l_suite
 ])
 # run the test suites
 unittest.TextTestRunner(verbosity=2).run(suites)
```


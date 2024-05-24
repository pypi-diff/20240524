# Comparing `tmp/itertree-1.0.5.tar.gz` & `tmp/itertree-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itertree-1.0.5.tar", last modified: Sat Jul  1 07:40:22 2023, max compression
+gzip compressed data, was "itertree-1.1.2.tar", last modified: Fri May 24 10:42:51 2024, max compression
```

## Comparing `itertree-1.0.5.tar` & `itertree-1.1.2.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 07:40:22.044827 itertree-1.0.5/
--rw-rw-rw-   0        0        0     1443 2023-06-22 21:06:01.000000 itertree-1.0.5/LICENSE
--rw-rw-rw-   0        0        0    17295 2023-07-01 07:40:22.045860 itertree-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    16683 2023-07-01 07:38:07.000000 itertree-1.0.5/README.md
--rw-rw-rw-   0        0        0      108 2021-03-31 14:04:49.000000 itertree-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      733 2023-07-01 07:40:22.046766 itertree-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      402 2023-07-01 07:38:07.000000 itertree-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 07:40:21.974606 itertree-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-01 07:40:21.997598 itertree-1.0.5/src/itertree/
--rw-rw-rw-   0        0        0     2452 2023-07-01 07:38:07.000000 itertree-1.0.5/src/itertree/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 07:40:22.015598 itertree-1.0.5/src/itertree/examples/
--rw-rw-rw-   0        0        0        0 2021-03-15 06:47:19.000000 itertree-1.0.5/src/itertree/examples/__init__.py
--rw-rw-rw-   0        0        0    19734 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/examples/calendar_example.py
--rw-rw-rw-   0        0        0     9669 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/examples/itree_data_models.py
--rw-rw-rw-   0        0        0    37511 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/examples/itree_docu_examples.py
--rw-rw-rw-   0        0        0     4376 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/examples/itree_link_example1.py
--rw-rw-rw-   0        0        0     4643 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/examples/itree_usage_example1.py
--rw-rw-rw-   0        0        0     5654 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/examples/itree_usage_example2.py
--rw-rw-rw-   0        0        0    58456 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_data.py
--rw-rw-rw-   0        0        0    23415 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_filters.py
--rw-rw-rw-   0        0        0    48086 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_getitem.py
--rw-rw-rw-   0        0        0    12135 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_helpers.py
--rw-rw-rw-   0        0        0    47842 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_indepth.py
--rw-rw-rw-   0        0        0   146925 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_main.py
--rw-rw-rw-   0        0        0    86824 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_mathsets.py
--rw-rw-rw-   0        0        0    37511 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_private.py
-drwxrwxrwx   0        0        0        0 2023-07-01 07:40:22.023599 itertree-1.0.5/src/itertree/itree_serializer/
--rw-rw-rw-   0        0        0        0 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_serializer/__init__.py
--rw-rw-rw-   0        0        0     7505 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_serializer/itree_json_converter.py
--rw-rw-rw-   0        0        0    20518 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_serializer/itree_json_serialize.py
--rw-rw-rw-   0        0        0     5304 2023-07-01 07:26:51.000000 itertree-1.0.5/src/itertree/itree_serializer/itree_render_dot.py
--rw-rw-rw-   0        0        0     6730 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_serializer/itree_renderer.py
-drwxrwxrwx   0        0        0        0 2023-07-01 07:40:22.004598 itertree-1.0.5/src/itertree.egg-info/
--rw-rw-rw-   0        0        0    17295 2023-07-01 07:40:21.000000 itertree-1.0.5/src/itertree.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1359 2023-07-01 07:40:21.000000 itertree-1.0.5/src/itertree.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 07:40:21.000000 itertree-1.0.5/src/itertree.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-01 07:40:21.000000 itertree-1.0.5/src/itertree.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-01 07:40:22.042837 itertree-1.0.5/tests/
--rw-rw-rw-   0        0        0    80119 2023-06-28 17:06:04.000000 itertree-1.0.5/tests/test_itertree_base1.py
--rw-rw-rw-   0        0        0    31107 2023-06-27 18:42:24.000000 itertree-1.0.5/tests/test_itertree_base_old.py
--rw-rw-rw-   0        0        0     4280 2023-06-12 06:06:03.000000 itertree-1.0.5/tests/test_itertree_examples.py
--rw-rw-rw-   0        0        0    10143 2023-06-26 20:21:06.000000 itertree-1.0.5/tests/test_itertree_flags.py
--rw-rw-rw-   0        0        0    16705 2023-06-27 18:42:24.000000 itertree-1.0.5/tests/test_itertree_full_feature_trees.py
--rw-rw-rw-   0        0        0    19598 2023-02-20 15:28:39.000000 itertree-1.0.5/tests/test_itertree_intervals.py
--rw-rw-rw-   0        0        0    59084 2023-06-26 20:21:06.000000 itertree-1.0.5/tests/test_itertree_iter.py
--rw-rw-rw-   0        0        0    19816 2023-06-27 18:42:24.000000 itertree-1.0.5/tests/test_itertree_links.py
--rw-rw-rw-   0        0        0    59933 2023-02-19 17:40:31.000000 itertree-1.0.5/tests/test_itertree_mathsets.py
--rw-rw-rw-   0        0        0    11308 2023-06-27 18:42:24.000000 itertree-1.0.5/tests/test_itertree_serialize.py
--rw-rw-rw-   0        0        0    19651 2023-03-01 21:50:32.000000 itertree-1.0.5/tests/test_itertree_value_models.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:42:51.971150 itertree-1.1.2/
+-rw-rw-rw-   0        0        0     1443 2023-06-22 21:06:01.000000 itertree-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0    15396 2024-05-24 10:42:51.970149 itertree-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    14784 2024-05-24 10:42:40.000000 itertree-1.1.2/README.md
+-rw-rw-rw-   0        0        0      108 2021-03-31 14:04:49.000000 itertree-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      733 2024-05-24 10:42:51.972145 itertree-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      402 2024-05-24 10:37:39.000000 itertree-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:42:51.897145 itertree-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-24 10:42:51.920138 itertree-1.1.2/src/itertree/
+-rw-rw-rw-   0        0        0     2474 2024-05-24 10:37:39.000000 itertree-1.1.2/src/itertree/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:42:51.938147 itertree-1.1.2/src/itertree/examples/
+-rw-rw-rw-   0        0        0        0 2021-03-15 06:47:19.000000 itertree-1.1.2/src/itertree/examples/__init__.py
+-rw-rw-rw-   0        0        0    19734 2023-06-29 16:45:55.000000 itertree-1.1.2/src/itertree/examples/calendar_example.py
+-rw-rw-rw-   0        0        0     9669 2023-06-29 16:45:55.000000 itertree-1.1.2/src/itertree/examples/itree_data_models.py
+-rw-rw-rw-   0        0        0    37511 2023-06-29 16:45:55.000000 itertree-1.1.2/src/itertree/examples/itree_docu_examples.py
+-rw-rw-rw-   0        0        0     9248 2023-07-29 20:03:26.000000 itertree-1.1.2/src/itertree/examples/itree_like_anytree.py
+-rw-rw-rw-   0        0        0     4376 2023-06-29 16:45:55.000000 itertree-1.1.2/src/itertree/examples/itree_link_example1.py
+-rw-rw-rw-   0        0        0     4643 2023-06-29 16:45:55.000000 itertree-1.1.2/src/itertree/examples/itree_usage_example1.py
+-rw-rw-rw-   0        0        0     5654 2023-06-29 16:45:55.000000 itertree-1.1.2/src/itertree/examples/itree_usage_example2.py
+-rw-rw-rw-   0        0        0    58456 2023-06-29 16:45:55.000000 itertree-1.1.2/src/itertree/itree_data.py
+-rw-rw-rw-   0        0        0    23415 2023-06-29 16:45:55.000000 itertree-1.1.2/src/itertree/itree_filters.py
+-rw-rw-rw-   0        0        0    49237 2023-08-21 09:11:48.000000 itertree-1.1.2/src/itertree/itree_getitem.py
+-rw-rw-rw-   0        0        0    14262 2023-11-13 14:21:30.000000 itertree-1.1.2/src/itertree/itree_helpers.py
+-rw-rw-rw-   0        0        0    50984 2023-11-26 16:07:32.000000 itertree-1.1.2/src/itertree/itree_indepth.py
+-rw-rw-rw-   0        0        0   152269 2023-11-26 10:43:00.000000 itertree-1.1.2/src/itertree/itree_main.py
+-rw-rw-rw-   0        0        0    86824 2023-06-29 16:45:55.000000 itertree-1.1.2/src/itertree/itree_mathsets.py
+-rw-rw-rw-   0        0        0    37505 2023-07-31 17:56:52.000000 itertree-1.1.2/src/itertree/itree_private.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:42:51.946148 itertree-1.1.2/src/itertree/itree_serializer/
+-rw-rw-rw-   0        0        0        0 2023-06-29 16:45:55.000000 itertree-1.1.2/src/itertree/itree_serializer/__init__.py
+-rw-rw-rw-   0        0        0     7505 2023-06-29 16:45:55.000000 itertree-1.1.2/src/itertree/itree_serializer/itree_json_converter.py
+-rw-rw-rw-   0        0        0    21060 2023-07-31 17:56:52.000000 itertree-1.1.2/src/itertree/itree_serializer/itree_json_serialize.py
+-rw-rw-rw-   0        0        0     5304 2023-07-01 07:26:51.000000 itertree-1.1.2/src/itertree/itree_serializer/itree_render_dot.py
+-rw-rw-rw-   0        0        0     6759 2023-07-31 17:40:50.000000 itertree-1.1.2/src/itertree/itree_serializer/itree_renderer.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:42:51.968154 itertree-1.1.2/src/itertree.egg-info/
+-rw-rw-rw-   0        0        0    15396 2024-05-24 10:42:51.000000 itertree-1.1.2/src/itertree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1431 2024-05-24 10:42:51.000000 itertree-1.1.2/src/itertree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 10:42:51.000000 itertree-1.1.2/src/itertree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-24 10:42:51.000000 itertree-1.1.2/src/itertree.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 10:42:51.966150 itertree-1.1.2/tests/
+-rw-rw-rw-   0        0        0    82107 2024-02-16 15:50:19.000000 itertree-1.1.2/tests/test_itertree_base1.py
+-rw-rw-rw-   0        0        0    31107 2023-06-27 18:42:24.000000 itertree-1.1.2/tests/test_itertree_base_old.py
+-rw-rw-rw-   0        0        0    10143 2023-06-26 20:21:06.000000 itertree-1.1.2/tests/test_itertree_flags.py
+-rw-rw-rw-   0        0        0    16705 2023-06-27 18:42:24.000000 itertree-1.1.2/tests/test_itertree_full_feature_trees.py
+-rw-rw-rw-   0        0        0     4462 2023-12-03 21:27:00.000000 itertree-1.1.2/tests/test_itertree_helpers.py
+-rw-rw-rw-   0        0        0    19598 2023-02-20 15:28:39.000000 itertree-1.1.2/tests/test_itertree_intervals.py
+-rw-rw-rw-   0        0        0    59082 2023-08-04 06:33:13.000000 itertree-1.1.2/tests/test_itertree_iter.py
+-rw-rw-rw-   0        0        0    76965 2023-11-13 16:41:42.000000 itertree-1.1.2/tests/test_itertree_iter2.py
+-rw-rw-rw-   0        0        0    19816 2023-06-27 18:42:24.000000 itertree-1.1.2/tests/test_itertree_links.py
+-rw-rw-rw-   0        0        0    59933 2023-02-19 17:40:31.000000 itertree-1.1.2/tests/test_itertree_mathsets.py
+-rw-rw-rw-   0        0        0    11308 2023-06-27 18:42:24.000000 itertree-1.1.2/tests/test_itertree_serialize.py
+-rw-rw-rw-   0        0        0    19651 2023-03-01 21:50:32.000000 itertree-1.1.2/tests/test_itertree_value_models.py
```

### Comparing `itertree-1.0.5/LICENSE` & `itertree-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `itertree-1.0.5/PKG-INFO` & `itertree-1.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 Metadata-Version: 2.1
 Name: itertree
-Version: 1.0.5
+Version: 1.1.2
 Summary: Python tree structure for data storage and iterations
 Home-page: https://github.com/BR1py/itertree
 Author: B_R
 Author-email: br_development@posteo.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BR1py/itertree/issues
 Project-URL: Documentation, https://readthedocs.org/projects/itertree/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![Static Badge](https://img.shields.io/badge/itertree-https%3A%2F%2Fgithub.com%2FBR1py%2Fitertree-blue?logo=github)](https://github.com/BR1py/itertree)
+[![PyPI](https://img.shields.io/pypi/v/itertree)](https://pypi.org/project/itertree)
+![Static Badge](https://img.shields.io/badge/python-%3E%3D3.4-green)
+[![Static Badge](https://img.shields.io/badge/licence-MIT(hpp)-green)](https://github.com/BR1py/itertree/blob/main/LICENSE)
+[![Static Badge](https://img.shields.io/badge/documenation-https%3A%2F%2Fitertree.readthedocs.io%2Fen%2Flatest%2F-yellow?logo=readthedocs)](https://itertree.readthedocs.io/en/latest/)
+![GitHub Release 1.1.2 - Published_At](https://img.shields.io/github/release-date/Br1py/itertree)
+
+
 # itertree python package
 
 
 ## Welcome to itertree python package
 
-Release 1.0.5   - fully released
+Release 1.1.2  -  released
 
 * Do you have to store data in a tree like structure?
 * Do you need good performance and a reach feature set in the tree object?
 * You like to serialize and store the structure in files?
 * And is it helpful for you if you can link subtrees from other trees and add local items in this "inherited" parts?
 
 Please give itertree package a try!
@@ -110,14 +118,20 @@
     iTree('sub', value={'mykey': 3})
     >>> # Show tree content:
     >>> root.render()
     iTree('root', value={'mykey': 0})
      > iTree('sub', value={'mykey': 1})
      > iTree('sub', value={'mykey': 2})
      > iTree('sub', value={'mykey': 3})
+    >>> # Address item via tag-index-pair (key):
+    >>> root['sub', 1]
+    iTree('sub', value={'mykey': 2})
+    >>> # Address item via absolute-index and check stored value:
+    >>> root[1].value
+    {'mykey': 2}
    
 
 ## First steps
 
 All important classes of the package are published by the package `__init__.py` file so that the functionality of
 itertree can be reached by importing:
 
@@ -302,54 +316,7 @@
     >>> first_item = next(iter(root.deep)) # create an iterator from the generator object
     >>> fifth_item = list(root.deep)[4]  # and this is slower as:
     >>> import itertools
     >>> fifth_item = next(itertools.islice(root.deep, 4, None))
   
 
     
-## iterators vs. lists
-
-We named the package itertree because when ever a iTree operation delivers multiple items the result will be an
-iterator (and not a list what the user might expect).
-
-Iterators are very powerful objects especially if you have a huge number of items to be iterated over.
-Iterators can be created very fast and they can be combined. So you can create very effective filter functions. It's
-recommended to have a look in the powerful itertools and more_itertools packages to combine it with itertree
-
-The main idea is to combine all the filtering and iterator options together before you start the final iteration
-(consume the iterator), which might at least end up in the expected list. By this mechanism we do at least only one
-unique iteration over the items and we must not do multiple typecasts and re-iterations in between even when we
-combine multiple filters.
-
-If the user really wants to create a list he can easy cast the iterator by using the `list()` statement:
-
-    >>> myresultlist=list(root.iter_all()) #  this is quick even for huge number of items
-    >>> first_item=list(root.iter_all())[0] # Anyway this is much slower than:
-    >>> first_item=next(root.iter_all())
-    >>> fifth_item=list(root.iter_all())[4] # and this is much slower than:
-    >>> import itertools
-    >>> fifth_item=next(itertools.isslice(root.iter_all(),4,None))
-    
-
-As it is shown in the performance test the operation `list()` is very quick (less then 0.5 s on 1 million items
-(depending on you PC)). And using the index access afterwards is a very good readable code. But as shown here there
-are quicker solutions available on iterators only.
-
-But we see also two downsides related to iterators:
-
-* The StopIteration exception must be handled in case of empty iterators. To make the handling a bit easier iTree
-  delivers in most cases an empty list if we have no match. But in some cases (e.g. filter operations) the user
-  will get an empty iterator and not the empty list. In itree_helpers the user can find a check
-  function for empty iterators that might help in this case: `is_iterator_empty(my_iterator)`.
-
-* The user must also consider that an iterator can be consumed only one time. To reuse an iterator multiple times
-  you may have a look on `itertools.tee()`.
-
-To summarize this chapter: 
-
-We decided that the iTree methods should deliver only iterators (and not lists). This is made to give the user
-the possibility to utilize the whole iterator power afterwards. If he really needs a list (in most cases for
-index access) he can cast the iterator easy and quick via the `list()` statement. But if iTree would directly
-deliver lists by default we would have a performance drop in all itertree filter functions which is not
-acceptable from our point of view.
-
-
```

### Comparing `itertree-1.0.5/README.md` & `itertree-1.1.2/src/itertree.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,38 @@
+Metadata-Version: 2.1
+Name: itertree
+Version: 1.1.2
+Summary: Python tree structure for data storage and iterations
+Home-page: https://github.com/BR1py/itertree
+Author: B_R
+Author-email: br_development@posteo.org
+License: MIT
+Project-URL: Bug Tracker, https://github.com/BR1py/itertree/issues
+Project-URL: Documentation, https://readthedocs.org/projects/itertree/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Static Badge](https://img.shields.io/badge/itertree-https%3A%2F%2Fgithub.com%2FBR1py%2Fitertree-blue?logo=github)](https://github.com/BR1py/itertree)
+[![PyPI](https://img.shields.io/pypi/v/itertree)](https://pypi.org/project/itertree)
+![Static Badge](https://img.shields.io/badge/python-%3E%3D3.4-green)
+[![Static Badge](https://img.shields.io/badge/licence-MIT(hpp)-green)](https://github.com/BR1py/itertree/blob/main/LICENSE)
+[![Static Badge](https://img.shields.io/badge/documenation-https%3A%2F%2Fitertree.readthedocs.io%2Fen%2Flatest%2F-yellow?logo=readthedocs)](https://itertree.readthedocs.io/en/latest/)
+![GitHub Release 1.1.2 - Published_At](https://img.shields.io/github/release-date/Br1py/itertree)
+
+
 # itertree python package
 
 
 ## Welcome to itertree python package
 
-Release 1.0.5   - fully released
+Release 1.1.2  -  released
 
 * Do you have to store data in a tree like structure?
 * Do you need good performance and a reach feature set in the tree object?
 * You like to serialize and store the structure in files?
 * And is it helpful for you if you can link subtrees from other trees and add local items in this "inherited" parts?
 
 Please give itertree package a try!
@@ -93,14 +118,20 @@
     iTree('sub', value={'mykey': 3})
     >>> # Show tree content:
     >>> root.render()
     iTree('root', value={'mykey': 0})
      > iTree('sub', value={'mykey': 1})
      > iTree('sub', value={'mykey': 2})
      > iTree('sub', value={'mykey': 3})
+    >>> # Address item via tag-index-pair (key):
+    >>> root['sub', 1]
+    iTree('sub', value={'mykey': 2})
+    >>> # Address item via absolute-index and check stored value:
+    >>> root[1].value
+    {'mykey': 2}
    
 
 ## First steps
 
 All important classes of the package are published by the package `__init__.py` file so that the functionality of
 itertree can be reached by importing:
 
@@ -285,54 +316,7 @@
     >>> first_item = next(iter(root.deep)) # create an iterator from the generator object
     >>> fifth_item = list(root.deep)[4]  # and this is slower as:
     >>> import itertools
     >>> fifth_item = next(itertools.islice(root.deep, 4, None))
   
 
     
-## iterators vs. lists
-
-We named the package itertree because when ever a iTree operation delivers multiple items the result will be an
-iterator (and not a list what the user might expect).
-
-Iterators are very powerful objects especially if you have a huge number of items to be iterated over.
-Iterators can be created very fast and they can be combined. So you can create very effective filter functions. It's
-recommended to have a look in the powerful itertools and more_itertools packages to combine it with itertree
-
-The main idea is to combine all the filtering and iterator options together before you start the final iteration
-(consume the iterator), which might at least end up in the expected list. By this mechanism we do at least only one
-unique iteration over the items and we must not do multiple typecasts and re-iterations in between even when we
-combine multiple filters.
-
-If the user really wants to create a list he can easy cast the iterator by using the `list()` statement:
-
-    >>> myresultlist=list(root.iter_all()) #  this is quick even for huge number of items
-    >>> first_item=list(root.iter_all())[0] # Anyway this is much slower than:
-    >>> first_item=next(root.iter_all())
-    >>> fifth_item=list(root.iter_all())[4] # and this is much slower than:
-    >>> import itertools
-    >>> fifth_item=next(itertools.isslice(root.iter_all(),4,None))
-    
-
-As it is shown in the performance test the operation `list()` is very quick (less then 0.5 s on 1 million items
-(depending on you PC)). And using the index access afterwards is a very good readable code. But as shown here there
-are quicker solutions available on iterators only.
-
-But we see also two downsides related to iterators:
-
-* The StopIteration exception must be handled in case of empty iterators. To make the handling a bit easier iTree
-  delivers in most cases an empty list if we have no match. But in some cases (e.g. filter operations) the user
-  will get an empty iterator and not the empty list. In itree_helpers the user can find a check
-  function for empty iterators that might help in this case: `is_iterator_empty(my_iterator)`.
-
-* The user must also consider that an iterator can be consumed only one time. To reuse an iterator multiple times
-  you may have a look on `itertools.tee()`.
-
-To summarize this chapter: 
-
-We decided that the iTree methods should deliver only iterators (and not lists). This is made to give the user
-the possibility to utilize the whole iterator power afterwards. If he really needs a list (in most cases for
-index access) he can cast the iterator easy and quick via the `list()` statement. But if iTree would directly
-deliver lists by default we would have a performance drop in all itertree filter functions which is not
-acceptable from our point of view.
-
-
```

### Comparing `itertree-1.0.5/setup.cfg` & `itertree-1.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 7465 7274 7265 652d 425f 520d   = itertree-B_R.
-00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e35  .version = 1.0.5
+00000020: 0a76 6572 7369 6f6e 203d 2031 2e31 2e32  .version = 1.1.2
 00000030: 0d0a 6175 7468 6f72 203d 2042 2e52 2e0d  ..author = B.R..
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 6272 5f64 6576 656c 6f70 6d65 6e74 4070  br_development@p
 00000060: 6f73 7465 6f2e 6f72 670d 0a64 6573 6372  osteo.org..descr
 00000070: 6970 7469 6f6e 203d 2041 2070 6163 6b61  iption = A packa
 00000080: 6765 2066 6f72 2063 7265 6174 696e 6720  ge for creating 
 00000090: 7472 6565 2073 7472 7563 7475 7265 7320  tree structures
```

### Comparing `itertree-1.0.5/src/itertree/__init__.py` & `itertree-1.1.2/src/itertree/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,20 +34,22 @@
 
 This part of code contains the initialization and publishing of the iTree related classes of the itertree package.
 """
 
 from __future__ import absolute_import
 
 __package__ = 'itertree'
-__version__ = '1.0.5'
+__version__ = '1.1.2'
 __licence__ = 'MIT incl. human protect patch'
 __author__ = 'B.R.'
 __url__ = 'https://github.com/BR1py/itertree'
 __description__ = 'Python tree structure for data storage and iterations'
 
-from .itree_helpers import iTLink, NoTag, NoKey, NoValue, Tag, iTFLAG, getter_to_list,INF,INF_PLUS,INF_MINUS,Any,TagIdx
+from .itree_helpers import iTLink, NoTag, NoKey, NoValue, Tag, \
+    iTFLAG, getter_to_list, INF, INF_PLUS, INF_MINUS, Any, TagIdx, ITER
 from .itree_main import iTree
 
 from . import itree_data as Data
 from . import itree_filters as Filters
 from .itree_serializer.itree_render_dot import _iTreeRenderDot
-iTreeRenderDot=_iTreeRenderDot().renders
+
+iTreeRenderDot = _iTreeRenderDot().renders
```

### Comparing `itertree-1.0.5/src/itertree/examples/calendar_example.py` & `itertree-1.1.2/src/itertree/examples/calendar_example.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.5/src/itertree/examples/itree_data_models.py` & `itertree-1.1.2/src/itertree/examples/itree_data_models.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.5/src/itertree/examples/itree_docu_examples.py` & `itertree-1.1.2/src/itertree/examples/itree_docu_examples.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.5/src/itertree/examples/itree_link_example1.py` & `itertree-1.1.2/src/itertree/examples/itree_link_example1.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.5/src/itertree/examples/itree_usage_example1.py` & `itertree-1.1.2/src/itertree/examples/itree_usage_example1.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.5/src/itertree/examples/itree_usage_example2.py` & `itertree-1.1.2/src/itertree/examples/itree_usage_example2.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.5/src/itertree/itree_data.py` & `itertree-1.1.2/src/itertree/itree_data.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.5/src/itertree/itree_filters.py` & `itertree-1.1.2/src/itertree/itree_filters.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.5/src/itertree/itree_getitem.py` & `itertree-1.1.2/src/itertree/itree_getitem.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,22 +111,22 @@
                         except:
                             raise ValueError('Given target {} is invalid'.format(repr(target)))  # from e
                 except IndexError:
                     try:
                         return False,itree._getitem_fam(target)
                     except:
                         raise IndexError(
-                            'Given family-idx of target {} not found in iTree'.format(repr(target)))  # from e
+                            'Given family-idx of target {} not found'.format(repr(target)))  # from e
                 except:
                     try:
                         return False,itree._getitem_fam(target)
                     except:
                         if 'fam_idx' in locals():
                             raise KeyError(
-                                'Given target {} invalid or not found in iTree'.format(repr(target)))  # from e
+                                'Given target {} invalid or not found'.format(repr(target)))  # from e
                         else:
                             raise ValueError('Given target {} is invalid'.format(repr(target)))  # from e
             elif t is int:
                 # absolute index or absolute index-slice
                 try:
                     return True,itree.getitem_by_idx(target)
                 except IndexError:
@@ -187,15 +187,15 @@
                                 target(c)
                             except Exception:
                                 raise TypeError('lambda: raised an exception in filter-calculation, the %i. child %s'
                                                 ' is incompatible with the calculation' % (c.idx, str(c)))
             result=itree._get_fam(target)
             if result is not None:
                 return False, result[:]
-        raise KeyError('Given target: %s not found in iTree!' % repr(target))
+        raise KeyError('Given target: %s not found' % repr(target))
 
     def __call__(self, target=NoTarget, *target_path, default=Exception,target_type=None):
         """
         Call via **iTree().get()**
         
         Main get method for items that supports in-depth level-wise access too.
 
@@ -568,15 +568,15 @@
                 r = self.getitem_by_idx(idx)
                 for i in idx_path:
                     r = r.getitem_by_idx(i)
                 return r
             else:
                 return self.getitem_by_idx(idx)
         except AttributeError:
-            return self._raise_exception(IndexError('No child in iTree %s' % (self._itree))) if default is Exception else default
+            return self._raise_exception(IndexError('Empty item, no child in %s' % str(self._itree))) if default is Exception else default
         except Exception as e:
             return self._raise_exception(e) if default is Exception else default
 
     def by_idx_slice(self, idx_slice, *idx_slice_path, default=Exception):
         """
         Call via **iTree().get.by_idx_slice()**
 
@@ -610,19 +610,19 @@
             r = self.getitem_by_idx(idx_slice)
             if idx_slice_path:
                 for i_s in idx_slice_path:
                     r2 = []
                     for item in r:
                         r2.extend(item.getitem_by_idx(i_s))
                     if not r2:
-                        raise IndexError(' No matching items found in iTree')
+                        raise IndexError(' No matching items found')
                     r = r2
                 return r
             else:
-                return r if r else self._raise_exception(IndexError(' No matching items found in iTree'))
+                return r if r else self._raise_exception(IndexError(' No matching items found'))
         except Exception as e:
              return self._raise_exception(e) if default is Exception else default
 
     def by_idx_list(self, idx_list, *idx_list_path, default=Exception):
         """
         Call via **iTree().get.by_idx_list()**
 
@@ -662,21 +662,21 @@
                             if BLIST_ACTIVE:
                                 [r2.extend(list(item.getitem_by_idx(self.NoneSlice))) for item in r]
                             else:
                                 [r2.extend(list(item)) for item in r]
                         else:
                             r2 = [item.getitem_by_idx(i) for item in r for i in i_l if i < len(item)]
                         if not r2:
-                            raise KeyError(' No matching items found in iTree')
+                            raise KeyError(' No matching items found')
                         r = r2
                     return r
                 else:
                     return r
             else:
-                raise IndexError('No child in iTree %s' % (itree))
+                raise IndexError('No child in %s' % str(itree))
         except Exception as e:
             return self._raise_exception(e) if default is Exception else default
 
     def by_tag_idx(self, tag_idx, *tag_idx_path, default=Exception):
         """
         Call via **iTree().get.by_tag_idx()**
 
@@ -710,15 +710,15 @@
                 for t, i in tag_idx_path:
                     r = r._getitem_fam(t)[i]
                 return r
             else:
                 return self._getitem_fam(tag)[fam_idx]
         except AttributeError:
             if default is Exception:
-                raise KeyError('No child in iTree %s' % (self._itree))
+                raise KeyError('No child in %s' % str(self._itree))
             else:
                 return default
         except Exception as e:
             return self._raise_exception(e) if default is Exception else default
 
     def by_tag_idx_slice(self, tag_idx_slice, *tag_idx_slice_path, default=Exception):
         """
@@ -756,19 +756,19 @@
                             family = self._getitem_fam(t)
                             if len(family) > s:
                                 result = family[s]
                                 if hasattr(result, '_itree_prt_idx'):
                                     result = [result]
                                 r2.extend(result)
                     if not r2:
-                        raise KeyError(' No matching items found in iTree')
+                        raise KeyError(' No matching items found')
                     r = r2
                 return r
             else:
-                return r if r else self._raise_exception(KeyError(' No matching items found in iTree'))
+                return r if r else self._raise_exception(KeyError(' No matching items found'))
         except Exception as e:
             return self._raise_exception(e) if default is Exception else default
 
     def by_tag_idx_list(self, tag_idx_list, *tag_idx_list_path, default=Exception):
         """
         Call via **iTree().get.by_tag_idx_list()**
 
@@ -809,15 +809,15 @@
                             family = self._getitem_fam(t)
                             if il is ...:
                                 r2.extend(family)
                             else:
                                 if len(family) > il:
                                     r2.append(family[il])
                     if not r2:
-                        raise KeyError(' No matching items found in iTree')
+                        raise KeyError(' No matching items found')
                     r = r2
                 return r
             else:
                 return r
         except Exception as e:
             return self._raise_exception(e) if default is Exception else default
 
@@ -851,21 +851,21 @@
                 r = self._getitem_fam(tag)
                 r2 = []
                 for t in tag_path:
                     for item in r:
                         if item._contains_fam(t):
                             r2.extend(item._getitem_fam(t))
                 if not r2:
-                    raise KeyError('Given tag_path %s has no match in iTree' % repr([tag] + tag_path))
+                    raise KeyError('Given tag_path %s has no match' % repr([tag] + tag_path))
                 return r2
             else:
                 return self._getitem_fam(tag)[:]
         except AttributeError:
             if default is Exception:
-                raise KeyError('No child in targeted iTree?')
+                raise KeyError('No child in targeted item?')
             else:
                 return default
         except Exception as e:
             return self._raise_exception(e) if default is Exception else default
 
     def by_tags(self, tags, *tags_path, default=Exception):
         """
@@ -915,20 +915,20 @@
                         except TypeError:
                             iterator = [tag]
                         for t in iterator:
                             for item in r:
                                 if item._contains_fam(t):
                                     r2.extend(item._getitem_fam(t))
                     if not r2:
-                        raise KeyError('Given tag_path *%s has no match in iTree' % repr((tags,) + tuple(tags_path)))
+                        raise KeyError('Given tag_path *%s has no match' % repr((tags,) + tuple(tags_path)))
                     return r2
                 else:
                     return r
             else:
-                raise KeyError('No child in iTree %s' % (itree))
+                raise KeyError('No child in %s' % str(itree))
         except Exception as e:
             return self._raise_exception(e) if default is Exception else default
 
     def by_level_filter(self, filter_method, *filter_method_path, default=Exception):
         """
         Call via **iTree().get.by_level_filters()**
 
@@ -961,18 +961,47 @@
                 r = filter(filter_method,itree)
                 if filter_method_path:
                     r2 = []
                     for f in filter_method_path:
                         for item in r:
                             r2.extend(filter(f,item))
                     if not r2:
-                        raise KeyError('Given filter_method_path has no match in iTree')
+                        raise KeyError('Given filter_method_path has no match')
                     return r2
                 else:
                     return list(r)
             else:
-                raise KeyError('No child in iTree %s' % (itree))
+                raise KeyError('No child in %s' % str(itree))
         except Exception as e:
             return self._raise_exception(e) if default is Exception else default
 
     def _raise_exception(self,exception):
         raise exception
+
+    def same_index_children(self,idx,incl_self=False):
+        """
+        method delivers the deepest item in the tree targeted by the given index.
+        E.g. if 0 is given the method extracts from the given item the first child,
+        from the child the first sub-child,...until the first item has no more child (empty item).
+        The chain of children with the index will be delivered as result.
+
+        In case the calling item (self has no children an empty list will be delivered.
+
+        :type idx: int
+        :param idx: index of chain of children to be extracted from the tree (negative values are accepted too)
+        :type incl_self: bool
+        :param incl_self: True - the calling item will be included as firat element in the list of children
+                          False - only children not the calling item is included in the return list
+        :return: chain of children with the given index
+        """
+        item=self._itree
+        if incl_self:
+            items = [item]
+        else:
+            items=[]
+        while item:
+            try:
+                item=item.getitem_by_idx(idx)
+            except IndexError:
+                break
+            items.append(item)
+        return items
```

### Comparing `itertree-1.0.5/src/itertree/itree_helpers.py` & `itertree-1.1.2/src/itertree/itree_helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -151,26 +151,26 @@
 
     def get_init_args(self):
         if self._link_item is None:
             return (self._file_path, self._target_path)
         else:
             return (self._file_path, self._target_path, self._link_item)
 
-    def get_target_tree(self, self_itree, source_dir=None):
+    def get_target_tree(self, ABSOLUTE, source_dir=None):
         if self._file_path:
             if os.path.isabs(self._file_path) or not source_dir:
                 file_path = self._file_path
             else:
                 file_path = os.path.join(source_dir, self._file_path)
             if not os.path.exists(file_path):
                 raise FileNotFoundError('Related source-file %s of the iTLink object not found!' % file_path)
-            result_tree = self_itree.load(file_path, load_links=True)
+            result_tree = ABSOLUTE.load(file_path, load_links=True)
             self._file_crc = self._get_file_crc(file_path)
         else:
-            result_tree = self_itree.root
+            result_tree = ABSOLUTE.root
         if self._target_path:
             if type(self._target_path) is str:
                 self._target_path=[self._target_path]
             if self._target_path[0]==result_tree.tag and Tag(self._target_path[0]) not in result_tree:
                 self._target_path=self._target_path[1:]
             if self._target_path:
                 result_tree = result_tree.get(*self._target_path)
@@ -260,14 +260,17 @@
         if self._link_item is not None:
             return 'iTLink(file_path=%s, target_path=%s,link_item=%s)' % (
                 repr(self._file_path), repr(self._target_path), repr(self._link_item),)
 
         return 'iTLink(file_path=%s, target_path=%s)' % (
             repr(self._file_path), repr(self._target_path),)
 
+ORDER_PRE=1
+ORDER_POST=0
+ORDER_LEVEL=2
 
 class iTFLAG():
     """
     public flags for setting the `iTree behavior during `__init__()`
     """
     READ_ONLY_TREE = 0b1
     READ_ONLY_VALUE = 0b10
@@ -385,7 +388,58 @@
     :rtype: list
     :return: result list
     """
     if hasattr(get_result, '_itree_prt_idx'):
         return [get_result]
     else:
         return list(get_result)
+
+class ITER():
+    """
+    iter options for deep iterators
+    """
+    DOWN=0b1 #gives iteration direction top-> down (default)
+    UP=DOWN <<1 # gives iteration direction bottom-> up
+    # in case DOWN adn UP is in we use UP;
+    # Both flags are just in because of downward compatibility
+    REVERSE=UP<<1 # switches item iteration direction to high index -> low index
+    SELF=REVERSE<<1 # include the calling object in the iteration (only if target matches)
+    FILTER_ANY= SELF<<1 # Use build in filtering instead of hierarchical filtering (only in iter())
+    MULTIPLE=FILTER_ANY<<1 # allows multiple matches of items in an iteration
+
+    @staticmethod
+    def get_option_str(option):
+        """
+        calculates a string representing the options used in given option
+        :para option: integer containing the option-bits
+        :return:
+        """
+        options=[]
+        if option & ITER.DOWN:
+            options.append('DOWN')
+        if option&ITER.UP:
+            options.append('UP')
+        if option&ITER.REVERSE:
+            options.append('REVERSE')
+        if option&ITER.SELF:
+            options.append('SELF')
+        if option&ITER.FILTER_ANY:
+            options.append('FILTER_ANY')
+        if option & ITER.MULTIPLE:
+            options.append('MULTIPLE')
+
+        invalid=option&~(ITER.UP | ITER.REVERSE | ITER.SELF |ITER.FILTER_ANY |ITER.MULTIPLE)
+        if invalid:
+            options.append('%s'%bin(invalid))
+        return ' | '.join(options)
+
+    @staticmethod
+    def valid_option(option,expected_option=DOWN |UP | REVERSE | SELF |FILTER_ANY  |MULTIPLE):
+        """
+        checks if given option is valid
+        :para option: integer containing the options-bits
+        :para expected_option: integer containing the full set of possible option-bits
+        :return: None or string for exception containing the invalid flags used
+        """
+        invalid=option&(~expected_option)
+        if invalid:
+            return 'Invalid iteration option(s) given: %s'%ITER.get_option_str(invalid)
```

### Comparing `itertree-1.0.5/src/itertree/itree_main.py` & `itertree-1.1.2/src/itertree/itree_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     Hashable = None
     Iterable = None
     Callable = None
     Union = None
     Optional = None
 
 from .itree_helpers import itree_list, TagIdx, NoTarget, iTFLAG, iTLink, _iTFLAG, NoTag, \
-    NoValue, INF,BLIST_SWITCH
+    NoValue, INF,BLIST_SWITCH,ITER
 from .itree_serializer.itree_renderer import iTreeRender
 from .itree_serializer.itree_json_serialize import iTStdJSONSerializer2
 from .itree_indepth import _iTreeIndepthTree
 from .itree_getitem import _iTreeGetitem
 from .itree_private import _iTreePrivate
 
 class iTree(_iTreePrivate):
@@ -320,14 +320,32 @@
         :rtype: Union[iTree, None]
         :return: iTree parent-object or None (in case no parent exists)
         """
         # Implementation state: ready, tested, doc ok
         return self._itree_prt_idx[0] if self._itree_prt_idx else None
 
     @property
+    def ancestors(self):
+        """
+        Property delivers current items parents list up to the oot.
+        In case item has no parent an empty list will be delivered
+
+        :rtype: list
+        :return: list of all ancestors
+        """
+        ancestors = []
+        p = self.parent
+        while p != None:
+            ancestors.append(p)
+            p = p.parent
+        # switch order to root->down
+        ancestors.reverse()
+        return ancestors
+
+    @property
     def is_root(self):
         """
         Is this item a root-item (has no parent)?
 
         :rtype: bool
         :return:
                 * *True* - is root
@@ -404,24 +422,24 @@
                 if siblings[i] is self:
                     parent_list[1] = i
                     return i
             if abs_idx < size / 2:
                 # start -> end
                 i = 0
                 for item in siblings:
-                    item._itree_prt_idx.__setitem__(1, i)
+                    item._itree_prt_idx.__setitem__(1, i) # update items idx cache
                     if item is self:
                         return i
                     i = i + 1
                 raise IndexError('Internal error for this iTree we found no related index in the parent-object!')
             else:
                 # end -> start
                 for i in range((size - 1), -1, -1):
                     item = siblings[i]
-                    item._itree_prt_idx.__setitem__(1, i)
+                    item._itree_prt_idx.__setitem__(1, i) #update item idx cache
                     if item is self:
                         return i
                 raise IndexError('Internal error for this iTree we found no related index in the parent-object!')
 
     @property
     def idx_path(self):
         """
@@ -582,14 +600,29 @@
         if self._itree_prt_idx is None:
             return None
         idx = self.idx + 1
         sl = self._itree_prt_idx[0]._items
         return sl.__getitem__(idx) if idx < sl.__len__() else None
 
     @property
+    def siblings(self):
+        """
+        Property delivers all siblings of the item. Iterates over all children of the parent and skips the item itself
+            * In case of no siblings an empty list is delivered.
+            * In case of an unique sibling a list with the unique sibling is delivered
+            * In case of multiple siblings a generator (iterator) over all siblings is delivered
+        :rtype Union(list,generator)
+        :return: iterable over the siblings
+        """
+        if self._itree_prt_idx is None:
+            return []
+        parent=self._itree_prt_idx[0]
+        return [i for i in parent if i is not self]
+
+    @property
     def level(self):
         """
         Delivers the distance (number of levels) to the root-item of the tree. Or in other words how
         deep in tree the item is positioned.
         In case item has no parent (is a root-item) this method will deliver 0.
 
         :rtype: int
@@ -629,14 +662,100 @@
                 break
             else:
                 max_depth += 1
             items = new_items
         return max_depth - 1
 
     @property
+    def negative_levels(self):
+        """
+        The property delivers a list of all bottom->up levels of the item. Because any branch might have
+        different depth
+        each item can have multiple negative levels. If the item has np children an empty list will be delivered.
+
+        ..note:: To check for a specific negative_level it's recommended to use the quicker `has_inverted_level()`
+                 method.
+
+        :rtype: list
+        :return: list of negative levels
+        """
+        self_level = self.level
+        return [(self_level-leave.level) for leave in self.deep.siblings(-1, ITER.INNER)]
+
+    def equal_negative_level(self,target_level):
+        """
+        The method checks if this item matches to the given target_level (bottom->up level).
+        The bottom up level is counted from the bottom of the tree upwards. The sub-tree of the item might
+        have different depths in the different branches. Therefore each item might have multiple inverted_levels.
+
+        :type target_level: int
+        :param target_level: The given level can be a positive or negative number (method considers the
+                             absolute level value)
+        :return: True - The given target-level is a valid bottom->up distance for this item
+                 False - This item has no matching bottom->up distance
+        """
+        target_level=abs(target_level)
+        self_level=self.level
+        for leave in self.deep.siblings(-1,ITER.INNER):
+            if leave.level-self_level==target_level:
+                return True
+        return False
+
+    def in_negative_level(self, target_level,equal=False,any=False):
+        """
+        The method checks if this item is greater or equal to the given target_level (bottom->up level).
+        The bottom up level is counted from the bottom of the tree upwards. The sub-tree of the item might
+        have different depths in the different branches. Therefor each item might have multiple inverted_levels.
+
+        :type target_level: int
+        :param target_level: The given level can be a positive or negative number
+                             (A given zero makes no sense and function will deliver False)
+
+        :type equal: bool
+        :param equal: Flag if the in means upon the given negative level (False) or
+                      upon or equal to given negative level (True) - default is False
+        :param any: Check if the item is upon the given negative level for all containing children (True)
+                    not just one (False - default)
+
+        :return: True - The given target-level is a valid bottom->up distance for this item
+                 False - This item has no matching bottom->up distance
+        """
+        target_level = abs(target_level)
+        if self:
+            if any:
+                if equal:
+                    self_level = self.level
+                    for leave in self.deep.siblings(-1, ITER.INNER):
+                        if leave.level - self_level < target_level:
+                            return False
+                    else:
+                        return True
+                else:
+                    self_level = self.level
+                    for leave in self.deep.siblings(-1, ITER.INNER):
+                        if leave.level - self_level <= target_level:
+                            return False
+                    else:
+                        return True
+            else:
+                if equal:
+                    self_level = self.level
+                    for leave in self.deep.siblings(-1, ITER.INNER):
+                        if leave.level - self_level >= target_level:
+                            return True
+                else:
+                    self_level = self.level
+                    for leave in self.deep.siblings(-1, ITER.INNER):
+                        if leave.level - self_level > target_level:
+                            return True
+        elif equal and target_level==1:
+            return True
+        return False
+
+    @property
     def tag_number(self):
         """
         property contains the number of tags (families) the itree contains
         :return: integer
         """
         if self:
             return len(self._families)
@@ -816,15 +935,15 @@
                       have a `iTValueModel` already as value it is placed inside the model.
 
         :rtype: object
         :return: old value object that was stored in iTree before
         """
         # Implementation state: ready, tested, doc ok
         if self._flags & self._IS_VALUE_PROTECTED:
-            raise PermissionError('iTree value is read only')
+            raise PermissionError('%s value is read only'%self.__class__.__name__)
         old_value = self._value
         # do we have a model?
         if (
                 hasattr(old_value, 'is_iTValueModel')
                 and hasattr(value, 'is_iTValueModel')
                 or not hasattr(old_value, 'is_iTValueModel')
         ):
@@ -872,15 +991,15 @@
 
 
         :rtype: object
         :return: old value object that was stored in iTree before
         """
         # Implementation state: ready, tested, doc ok
         if self._flags & self._IS_VALUE_PROTECTED:
-            raise PermissionError('iTree value is read only')
+            raise PermissionError('%s value is read only'%self.__class__.__name__)
         old_value = self._value
         try:
             old_value = old_value[key]
         except KeyError:
             old_value[key] = value
             return NoValue
         except TypeError:
@@ -955,15 +1074,15 @@
         This method will always delete the whole object stored in `iTree` even `iTValueModel`-objects are deleted. To
         delete the value content of a model `mytree.value.clear()` or 'set_value(NoValue)' might be used.
 
         :return: deleted value
         """
         # Implementation state: ready, tested, doc ok
         if self._flags & self._READ_ONLY_VALUE:
-            raise PermissionError('iTree value is read only')
+            raise PermissionError('%s value is read only'%self.__class__.__name__)
         old_value, self._value = self._value, NoValue
         return old_value
 
     def del_key_value(self, key):
         """
         If no parameter is given deletes the full value-object stored in ´iTree´ (store ´NoValue´ ).
 
@@ -982,15 +1101,15 @@
         :type key: Optional[Hashable,int]
         :param key: Optional key or index to exchange just sub-items in the value
 
         :return: deleted value
         """
         # Implementation state: ready, tested, doc ok
         if self._flags & self._READ_ONLY_VALUE:
-            raise PermissionError('iTree value is read only')
+            raise PermissionError('%s value is read only'%self.__class__.__name__)
         return self._value.pop(key)
 
     @property
     def coupled_object(self):
         """
         The `iTree`-object can be coupled with another Python-object. The pointer to the object is stored and can be
         reached via this property. (E.g. this can be helpful when connecting the `iTree` with a visual item
@@ -1059,19 +1178,19 @@
                 if hasattr(item, '_itree_prt_idx') and item.flags & (
                         self._LINKED | self._LINK_ROOT | self._PLACEHOLDER):
                     raise TypeError('Linked items cannot be appended to linked item as local item')
             else:
                 self._raise_read_only_exception(self)
         try:
             if item._itree_prt_idx is not None:
-                raise RecursionError('Given item has already a parent iTree!')
+                raise RecursionError('Given item has already a parent')
             tag = item._tag
         except AttributeError:
             # implicit definition of iTree:
-            item = iTree(value=item)
+            item = self.__class__(value=item)
             tag = NoTag
         # return self._append_item(self,item)
         # Just for performance we keep the code for append here and do not use the helper
         abs_idx = len(self)  # after tests here the len() is quicker (not understood why)
         if abs_idx:
             self._items.append(item)
             # append item to family
@@ -1158,18 +1277,18 @@
                         self._raise_read_only_exception(self)
                 elif self._link.is_loaded and NoTag in self._link._tags:
                     self._raise_read_only_exception(self)
             else:
                 self._raise_read_only_exception(self)
         try:
             if item._itree_prt_idx is not None:
-                raise RecursionError('Given item has already a parent iTree!')
+                raise RecursionError('Given item has already a parent')
         except AttributeError:
             # implicit definition of iTree:
-            item = iTree(value=item)
+            item = self.__class__(value=item)
         if self:
             return self._append_item_left(self, item)
         else:
             return self._append_item(self, item)
 
     def insert(self, target, item=NoValue):
         """
@@ -1218,29 +1337,29 @@
                         self._raise_read_only_exception(self)
                 elif self._link.is_loaded and NoTag in self._link._tags:
                     self._raise_read_only_exception(self)
             else:
                 self._raise_read_only_exception(self)
         try:
             if item._itree_prt_idx is not None:
-                raise RecursionError('Given item has already a parent iTree!')
+                raise RecursionError('Given item has already a parent')
         except AttributeError:
             # implicit definition of iTree:
-            item = iTree(value=item)
+            item = self.__class__(value=item)
         if self:
             sl = self._items
             size = sl.__len__()
             if size == 0 and target != 0:
-                raise KeyError('iTree is empty no valid target given!')
+                raise KeyError('%s is empty no valid target given!'%self.__class__.__name__)
             # absolute index of the target
             if type(target) is int:  # is already the absolute index!
                 abs_idx = size + target if target < 0 else target
             elif hasattr(target, '_itree_prt_idx'):
                 if target._itree_prt_idx is not self:
-                    raise ValueError('Given target is not part of the iTree')
+                    raise ValueError('Given target is not part of the %s'%self.__class__.__name__)
                 abs_idx = target.idx
             else:
                 abs_idx = self.__getitem__(target).idx
             if abs_idx == 0:
                 return self._append_item_left(self, item)
             # insert in list
             sl.insert(abs_idx, item)
@@ -1296,15 +1415,15 @@
                     flag_mask = self._LINKED | self._LINK_ROOT | self._PLACEHOLDER
                     error = any(
                         hasattr(i, '_itree_prt_idx') and i.flags & flag_mask
                         for i in check_items
                     )
                     if error:
                         raise PermissionError(
-                            'It is not allowed to append linked items in an already linked item iTree')
+                            'It is not allowed to append linked items in an already linked item')
             else:
                 self._raise_read_only_exception(self)
         return self._items.extend(_iTreePrivate._iter_extend(self, items))
 
     def extendleft(self, items):
         """
         Multy item append on left hand-side (at the beginning) of the ´iTree´.
@@ -1441,20 +1560,20 @@
 
         # prepare new item
         if hasattr(value, '_itree_prt_idx'):
             parent_list = value._itree_prt_idx
             if parent_list is not None:
                 if parent_list[0] == self:
                     # reorder operation!
-                    value = self._iter_copy(value, iTree._get_args_skip_subtree)
+                    value = self._iter_copy(value, self.__class__._get_args_skip_subtree)
                 else:
-                    raise RecursionError('Given item has already a parent iTree!')
+                    raise RecursionError('Given item has already a parent')
         else:
             # implicit iTree definition
-            value = iTree(value=value)
+            value = self.__class__(value=value)
 
         if target is ...:  # Ellipsis is used for single append
             if self:
                 tag = value.tag
                 if tag in self._families:
                     # delete family
                     self.__delitem__(tag)
@@ -1529,15 +1648,15 @@
                        * key - key-tuple (family_tag, family_index) pair
                        * item - `iTree`-item that is already a children (future successor)
                        * None - if `None` is given we will move the item to the last position in the ´iTree´-object
 
         :return: self (with updated indexes)
         """
         if self._itree_prt_idx is None:
-            raise LookupError('This item is not a children of a iTree!')
+            raise LookupError('This item is not a children of a %s'%self.__class__.__name__)
         parent = self._itree_prt_idx[0]
         flags = parent._flags
         if flags & self._IS_TREE_PROTECTED:
             if parent.is_link_root:
                 if parent._link.is_loaded and self.tag in parent._link._tags:
                     self._raise_read_only_exception(self)
             else:
@@ -1893,38 +2012,38 @@
         :return: removed item(s) (parent will be set to None) - in case of multiple removes the
                  method delivers a list no iterator because anyway a list is created
         """
         if hasattr(item, '_itree_prt_idx'):
             if item._itree_prt_idx is not None and item._itree_prt_idx[0] is self:
                 return self.__delitem__(item.idx)
             else:
-                raise ValueError('Given iTree object is not a child of this iTree-object')
+                raise ValueError('Given item object is not a child of this %s-object'%self.__class__.__name__)
         try:
             is_link_root = self.is_link_root and self.is_link_loaded
             item_list = list(
                 item)  # we consume the iterator here because we need it multiple times we used list to reverse later on
             for i in item_list:  # check if the items in the iterator are valid for the operation
                 try:
                     if i._itree_prt_idx[0] is not self:
                         raise AttributeError()
                     if is_link_root and (i.is_linked or i.is_placeholder):
                         self._raise_read_only_exception(self)
                     continue
                 except AttributeError as e:
                     raise ValueError(
-                        'The object %r is not a child of this iTree-object'
-                        % repr(i)
+                        'The object %r is not a child of this %s-object'
+                        % (repr(i),self.__class__.__name__)
                     ) from e
             for i in reversed(item_list):  # we see advantage for most cases if we remove in reversed order
                 self.__delitem__(i.idx)
             return item_list
         except (PermissionError, ValueError):
             raise
         except:
-            raise TypeError('As item parameter we expect an iTree child or a Iterable of children')
+            raise TypeError('As item parameter we expect a tree child or an iterable of children')
 
     # *** getters: *****************************************************************************************************
 
     def __getitem__(self, target):
         """
         Main common get method for children (first level items).
 
@@ -1985,22 +2104,22 @@
                         except:
                             raise ValueError('Given target {} is invalid'.format(repr(target)))  # from e
                 except IndexError:
                     try:
                         return list(self._getitem_fam(target))
                     except:
                         raise IndexError(
-                            'Given family-idx of target {} not found in iTree'.format(repr(target)))  # from e
+                            'Given family-idx of target {} not found'.format(repr(target)))  # from e
                 except:
                     try:
                         return list(self._getitem_fam(target))
                     except:
                         if 'fam_idx' in locals():
                             raise KeyError(
-                                'Given target {} invalid or not found in iTree'.format(repr(target)))  # from e
+                                'Given target {} invalid or not found'.format(repr(target)))  # from e
                         else:
                             raise ValueError('Given target {} is invalid'.format(repr(target)))  # from e
             elif t is int or t is slice:
                 # absolute index or absolute index-slice
                 try:
                     return self.getitem_by_idx(target)
                 except IndexError:
@@ -2051,24 +2170,19 @@
                                 target(c)
                             except Exception:
                                 raise TypeError('lambda: raised an exception in filter-calculation, the %i. child %s'
                                                 ' is incompatible with the calculation' % (c.idx, str(c)))
             result= self._get_fam(target)
             if result is not None:
                 return result[:] # slice is quicker then copy
-        raise KeyError('Given target: %s not found in iTree!' % repr(target))
+        raise KeyError('Given target: %s not found' % repr(target))
 
     # *** math operations and operations creating new/copied representations *******************************************
 
-    def __reversed__(self):
-        return self.__class__(self._tag,
-                              value=copy.copy(self._value),
-                              subtree=[i.__copy__() for i in reversed(list(self._items.__iter__()))],
-                              # here we create a recursion -> subtree is copied!!
-                              )
+    #use def __reverse__() from super class
 
     def __mul__(self, factor):
         """
         Multiplication function a iTree is multiplied (copies) and put in a new iTree:
 
         my_single_item=iTree('multi')
         multi=my_single_item*1000
@@ -2089,23 +2203,23 @@
         if hasattr(factor, '_itree_prt_idx'):
             if self.is_link_root:
                 raise TypeError('__mul__() on link-root items is not supported')
             subtree = chain.from_iterable(
                 product((i.copy() for i in self), (i.copy() for i in factor)))
         else:
             subtree = repeat(self.copy(), factor)
-        return iTree(self._tag, copy.copy(self._value), subtree, None, self._flags)
+        return self.__class__(self._tag, copy.copy(self._value), subtree, None, self._flags)
 
     def __rmul__(self, other):
         if hasattr(other, '_itree_prt_idx'):
             subtree = chain.from_iterable(
                 product((i.copy() for i in self), (i.copy() for i in other)))
         else:
             subtree = repeat(self.copy(), other)
-        return iTree(NoTag, NoValue, subtree)
+        return self.__class__(NoTag, NoValue, subtree)
 
     def __sub__(self, other):
         """
         To subtract two iTree objects we copy the self-object and we iterate over the other object items.
         In case a matching key is found in self the item will be deleted in the copy.
 
         :param other:
@@ -2157,19 +2271,19 @@
 
         :param other: iTree object that should be added
         :return: New iTree object containing copies of all children
         """
         if hasattr(other, '_itree_prt_idx'):
             if self.is_link_root:
                 raise TypeError('__add__() on link-root items is not supported')
-            return iTree(copy.copy(self._tag), copy.copy(self._value),
+            return self.__class__(copy.copy(self._tag), copy.copy(self._value),
                          subtree=chain((item.__copy__() for item in self),
                                        (item.__copy__() for item in other)), flags=self._flags)
         else:
-            raise TypeError('Added item is not of type iTree')
+            raise TypeError('Added item is not an instance of iTree')
 
     def __copy__(self):
         """
         create a copy of this item
 
         The difference in between copy and deepcopy for iTree is just that we do in deepcopy a copy
         of all data items too. In copy we just copy the iTData object not the items itself, they stay as pointers
@@ -2179,63 +2293,63 @@
         do a copy of all sub-items (in-depth). It's not possible to copy just the top-level element only.
 
         The function is used internally in extend operations too. And we can see (profiler) that
         improvements in this method have big impact.
 
         :return: copied iTree object
         """
-        return self._iter_copy(self, iTree._get_copy_args)
+        return self._iter_copy(self, self.__class__._get_copy_args)
 
     def copy_keep_value(self):
         """
         Create a copy of this item.
 
         The difference in between normal `copy()` and this method is that the value objects are
         completely untouched in this operation (for immutable objects there is no difference
         in between the two copy operations).
 
         :return: copied iTree object
         """
-        return self._iter_copy(self, iTree._get_args_skip_subtree)
+        return self._iter_copy(self, self.__class__._get_args_skip_subtree)
 
     def copy(self, *args, **kwargs):
         """
         create a copy of this item
 
         The difference in between `copy()` and `deepcopy()` for `iTree` is just that we do in `deepcopy()` a deepcopy
         of all value items. In `copy()` we just copy the value object not the items inside, the pointers
         to the original objects are kept (for immutable objects there is no difference).
 
         :return: copied iTree object
         """
-        return self._iter_copy(self, iTree._get_copy_args)
+        return self._iter_copy(self, self.__class__._get_copy_args)
 
     def __deepcopy__(self, *args, **kwargs):
         """
         create a deepcopy of this item
 
         The difference in between `copy()` and `deepcopy()` for `iTree` is just that we do in `deepcopy()` a deepcopy
         of all value items. In `copy()` we just copy the value object not the items inside, the pointers
         to the original objects are kept (for immutable objects there is no difference).
 
         :return: deep copied new iTree object
         """
-        return self._iter_copy(self, iTree._get_deepcopy_args)
+        return self._iter_copy(self, self.__class__._get_deepcopy_args)
 
     def deepcopy(self, *args, **kwargs):
         """
         create a deepcopy of this item
 
         The difference in between `copy()` and `deepcopy()` for `iTree` is just that we do in `deepcopy()` a deepcopy
         of all value items. In `copy()` we just copy the value object not the items inside, the pointers
         to the original objects are kept (for immutable objects there is no difference).
 
         :return: deep copied new iTree object
         """
-        return self._iter_copy(self, iTree._get_deepcopy_args)
+        return self._iter_copy(self, self.__class__._get_deepcopy_args)
 
     # *** size & comparisons *******************************************************************************************
 
     # __len__() of the super-class blist is not overloaded!
 
     def filtered_len(self, filter_method):
         """
@@ -2308,15 +2422,15 @@
                 * True - matching child is found
                 * False - no matching item found
         """
         if hasattr(item, '_itree_prt_idx'):
             p = item._itree_prt_idx
             return p is not None and p[0] is self
         else:
-            raise TypeError('Given item is not of type iTree')
+            raise TypeError('Given item is not an instance of iTree')
 
     def __eq__(self, other):
 
         """
         compares if the tag, value and children content of another item matches with this item
 
         .. note::
@@ -2496,31 +2610,31 @@
                 if not hasattr(start, '_itree_prt_idx'):
                     start = self.get.single(start)
                 try:
                     first_item = next(dropwhile(lambda i: i is not start, iterator))
                     if first_item == item:
                         return first_item.idx
                 except StopIteration:
-                    raise IndexError('No matching item found in iTree')
+                    raise IndexError('No matching item found')
             if stop is not None:
                 if not hasattr(stop, '_itree_prt_idx'):
                     stop = self.get.single(stop)
                 try:
                     item = next(dropwhile(lambda i: i is not stop and i != item, iterator))
                     if item is not stop:
                         return item.idx
                     raise StopIteration
                 except StopIteration:
-                    raise IndexError('No matching item found in iTree')
+                    raise IndexError('No matching item found')
             else:
                 try:
                     item = next(dropwhile(lambda i: i != item, iterator))
                     return item.idx
                 except StopIteration:
-                    raise IndexError('No matching item found in iTree')
+                    raise IndexError('No matching item found')
 
     def __hash__(self):
         """
         The hash operation is available
 
         .. node::As for the `==` operator we do not consider, parent, coupled items or flags properties of the object
 
@@ -2583,20 +2697,18 @@
                             of this object for matches (see :ref:`filter_method <filter_method>`)
 
                             If `None` is given filtering is inactive.
 
         :rtype: Iterator
         :return: iterator over the values stored in the children
         """
-        if filter_method:
-            for item in filter(filter_method, self):
-                yield item._value
+        if filter_method is None:
+            return (i._value for i in self)
         else:
-            for item in self:
-                yield item.value
+            return (i._value for i in filter(filter_method,self))
 
     def items(self, filter_method=None, values_only=False):
         """
         Iterates over all children and deliver the children
         item-tuples (key,item) or (key,value). As key we use the unique tag-idx: (tag-family,family-index).
 
         The function is comparable with dicts `items()` function.
@@ -2747,15 +2859,15 @@
         Create representation string from which the object can be theoretically be reconstructed via `eval()`
         (might not work in case of
         value-objects that do not have a working `__repr()` method)
 
         :rtype: str
         :return: representation string
         """
-        out = ['iTree(']
+        out = ['%s('%self.__class__.__name__]
         if self._tag is not NoTag:
             out.append(repr(self._tag))
             out.append(', ')
         if self._value is not NoValue:
             out.append('value=')
             out.append(repr(self._value))
             out.append(', ')
@@ -2795,15 +2907,15 @@
         """
         String repr of the item stripping the subtree to the first and last element only and giving ".." inbetween
 
         For full representation-string use `repr()`.
 
         :return: shorten representation string
         """
-        out = ['iTree(']
+        out = ['%s('%self.__class__.__name__]
         if self._tag is not NoTag:
             out.append(repr(self._tag))
             out.append(', ')
         if self._value is not NoValue:
             out.append('value=')
             out.append(repr(self._value))
             out.append(', ')
@@ -2895,15 +3007,15 @@
         print(
             self.renders(filter_method, enumerate, renderer=iTreeRender).encode(
                 errors='replace').decode(
                 'utf8')[:-1])
 
     # for pickle
     def __reduce__(self):
-        return iTree, tuple(self.get_init_args())
+        return self.__class__, tuple(self.get_init_args())
 
     def get_init_args(self, filter_method=None, _subtree_not_none=True):
         """
         Method creates list of arguments that can be used as a pointer to create an equal instance of an iTree object.
         This is a method is used in most cases for internal functionalities (especially copy()).
 
         :type filter_method: Union[Callable,None]
@@ -2960,15 +3072,15 @@
 
         :param itree_serializer: optional user defined serializer for iTree objects
 
         :return: iTree object loaded from file
         """
         serializer_obj = getattr(self, '__itree_serializer', None)
         if serializer_obj is None or type(serializer_obj) != itree_serializer:
-            self.__itree_serializer = serializer_obj = itree_serializer(iTree)
+            self.__itree_serializer = serializer_obj = itree_serializer(self.__class__)
 
         return serializer_obj.loads(data_str, check_hash=check_hash, load_links=load_links)
 
     def load(self, file_path, check_hash=True, load_links=True,
              itree_serializer=iTStdJSONSerializer2):
         """
         create an iTree object by loading from a file
@@ -2985,15 +3097,15 @@
 
         :param itree_serializer: optional user defined serializer for iTree objects
 
         :return: iTree object loaded from file
         """
         serializer_obj = getattr(self, '__itree_serializer', None)
         if serializer_obj is None or type(serializer_obj) != itree_serializer:
-            self.__itree_serializer = serializer_obj = itree_serializer(iTree)
+            self.__itree_serializer = serializer_obj = itree_serializer(self.__class__)
 
         return serializer_obj.load(file_path, check_hash=check_hash, load_links=load_links)
 
     def dumps(self, calc_hash=False, filter_method=None,
               itree_serializer=iTStdJSONSerializer2):
 
         """
@@ -3003,15 +3115,15 @@
 
         :param itree_serializer: optional user defined serializer for iTree objects
 
         :return: serialized string (JSON in case of default serializer)
         """
         serializer_obj = getattr(self, '__itree_serializer', None)
         if serializer_obj is None or type(serializer_obj) != itree_serializer:
-            self.__itree_serializer = serializer_obj = itree_serializer(iTree)
+            self.__itree_serializer = serializer_obj = itree_serializer(self.__class__)
         return serializer_obj.dumps(self, calc_hash=calc_hash, filter_method=filter_method)
 
     def dump(self, target_path, pack=True, calc_hash=True, overwrite=False,
              filter_method=None,
              itree_serializer=iTStdJSONSerializer2):
         """
         serializes the iTree object to JSON (default serializer) and store it in a file
@@ -3023,15 +3135,15 @@
 
         :param itree_serializer: optional user defined serializer for iTree obbjects
 
         :return: True if file is stored successful
         """
         serializer_obj = getattr(self, '__itree_serializer', None)
         if serializer_obj is None or type(serializer_obj) != itree_serializer:
-            self.__itree_serializer = serializer_obj = itree_serializer(iTree)
+            self.__itree_serializer = serializer_obj = itree_serializer(self.__class__)
         return serializer_obj.dump(self,
                                    target_path,
                                    pack=pack,
                                    calc_hash=calc_hash,
                                    overwrite=overwrite,
                                    filter_method=filter_method)
 
@@ -3057,15 +3169,15 @@
         """
         If the item is local and covers a linked item the property is True
 
         :rtype: bool
         :return: True/False
 
         """
-        return hasattr(self, '_link') and self._link and (type(self._link._link_item) is iTree)
+        return hasattr(self, '_link') and self._link and (hasattr(self._link._link_item,'_itree_prt_idx'))
 
     @property
     def is_linked(self):
         """
         In contrast to iTreeLinked class this is False
 
         :rtype: bool
@@ -3077,15 +3189,15 @@
     @property
     def is_link_loaded(self):
         if hasattr(self, '_link'):
             return self._link.is_loaded
         else:
             # we return False in case we have no link_roots inside the subtree
             return any(
-                i.is_link_loaded for i in filter(iTree._filter_linked_roots, self.deep))
+                i.is_link_loaded for i in filter(self.__class__._filter_linked_roots, self.deep))
 
     @property
     def link_root(self):
         """
         delivers the highest level item that is linked
         in case item is not linked it delivers itself
 
@@ -3247,15 +3359,15 @@
                     link_handler.set_tags_and_keys(tags, keys)
                     link_handler.set_loaded(load_item.tag, load_item.value)
                     return True
                 else:
                     return False
         else:
             loaded = False
-            for i in filter(iTree._filter_linked_roots, self.deep):
+            for i in filter(self.__class__._filter_linked_roots, self.deep):
                 if i.load_links(force=force, delete_invalid_items=delete_invalid_items, _depth=(_depth + 1)):
                     loaded = True
             return loaded
 
     def make_local(self, copy_subtree=True):
         """
         make the current linked object a local object
@@ -3279,18 +3391,18 @@
         parent._getitem_fam(tag)[f_idx] = local_item
         local_item._itree_prt_idx = [parent, abs_idx, f_idx]
         return local_item
 
     # *** unsupported methode (overload super() methods with exceptions ************************************************
 
     def __isub__(self, other):
-        raise TypeError('iTree: unsupported operand or function')
+        raise TypeError('Unsupported operand or function')
 
     def __imul__(self, other):
-        raise TypeError('iTree: unsupported operand or function')
+        raise TypeError('Unsupported operand or function')
 
     # *** helpers ******************************************************************************************************
 
     # property for debugging
     @property
     def _debug_children_list(self):
         """
```

### Comparing `itertree-1.0.5/src/itertree/itree_mathsets.py` & `itertree-1.1.2/src/itertree/itree_mathsets.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.5/src/itertree/itree_private.py` & `itertree-1.1.2/src/itertree/itree_private.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
             return True
         except Exception:
             return False
 
 
     @staticmethod
     def _raise_read_only_exception(itree_item):
-        raise PermissionError('The iTree item (%s) is read_only (linked or read_only flag)!' % repr(itree_item))
+        raise PermissionError('The item (%s) is read_only (linked or read_only flag)!' % repr(itree_item))
 
     @staticmethod
     def _raise_exception(exception):
         raise exception
 
     # --- flags related helpers ----------------------------------------------------------------
     # private helpers for setting flags
```

### Comparing `itertree-1.0.5/src/itertree/itree_serializer/itree_json_converter.py` & `itertree-1.1.2/src/itertree/itree_serializer/itree_json_converter.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.5/src/itertree/itree_serializer/itree_json_serialize.py` & `itertree-1.1.2/src/itertree/itree_serializer/itree_json_serialize.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,168 +35,174 @@
 This part of code contains the standard iTree serializers (JSON and rendering)
 """
 
 from __future__ import absolute_import
 
 import gzip
 import hashlib
-from collections import OrderedDict,deque
+from collections import OrderedDict, deque
 
 # For serializing we (try) to import some modules:
 
-IS_ORJSON=False
+IS_ORJSON = False
 DECODE = False
 try:
     import rapidjson
 except:
     rapidjson = None
 
 try:
     import orjson as JSON
-    IS_ORJSON=True
+
+    IS_ORJSON = True
     # orjson is much faster than standard json but might not be available
     import json
 
 except:
     import json as JSON
 
-    test=bytes(JSON.dumps({'test':'123','HASH':hashlib.sha1(b'asjhdahsdh').hexdigest()}).encode('utf8', errors='backslashreplace'))
+    test = bytes(JSON.dumps({'test': '123', 'HASH': hashlib.sha1(b'asjhdahsdh').hexdigest()}).encode('utf8',
+                                                                                                     errors='backslashreplace'))
     try:
         JSON.loads(test)
     except TypeError:
-        DECODE=True
+        DECODE = True
+
 
 class np():
     class nparray():
         pass
+
+
 try:
     import numpy as np
+
     # only needed in case of numpy arrays in data
     # for serializing the data
     np_loaded = True
 except ImportError:
     np_loaded = False
 
 from ..itree_helpers import *
 
 DT_SERIALIZE_VERSION = "2.0.0"
 DT_SERIALIZE_MAJOR_VERSION = "2.0"
 
+
 class iTStdJSONSerializer2(object):
     """
     This is the standard serializer for DataTree which translates the structure
     into the JSON format.
     Users might implement their own serializers using the interface methods defined
     in this serializer
     """
-    not_linked_filter=lambda i: not i.is_linked
+    not_linked_filter = lambda i: not i.is_linked
 
     ALL_TYPE = 0
-    BYTE_TYPE=1
-    STR_TYPE=2
-    DICT_TYPE=3
-    ITER_TYPE=4
+    BYTE_TYPE = 1
+    STR_TYPE = 2
+    DICT_TYPE = 3
+    ITER_TYPE = 4
     NP_TYPE = 5
     IT_TYPE = 6
     IT_LINK_TYPE = 7
     IT_CONST_TYPE = 8
 
-    NO_VALUE=0
-    NO_TAG=1
+    NO_VALUE = 0
+    NO_TAG = 1
     ANY = 2
-    NO_KEY=3
+    NO_KEY = 3
 
-    TRANSLATE_OBJ2KEY={NoKey:NO_KEY,
-                       Any:ANY,
-                       NoTag:NO_TAG,
-                       NoValue:NO_VALUE}
-
-    TRANSLATE_KEY2OBJ = {NO_KEY:NoKey ,
-                         ANY:Any ,
-                         NO_TAG:NoTag ,
-                         NO_VALUE:NoValue }
+    TRANSLATE_OBJ2KEY = {NoKey: NO_KEY,
+                         Any: ANY,
+                         NoTag: NO_TAG,
+                         NoValue: NO_VALUE}
+
+    TRANSLATE_KEY2OBJ = {NO_KEY: NoKey,
+                         ANY: Any,
+                         NO_TAG: NoTag,
+                         NO_VALUE: NoValue}
 
     CONVERT_MAP = {
         float: lambda self, o: [o, self.ALL_TYPE],
         int: lambda self, o: [o, self.ALL_TYPE],
         str: lambda self, o: [o, self.ALL_TYPE],
         tuple: lambda self, o: [[self.convert_to_json_item(i) for i in o],
                                 self.ITER_TYPE,
                                 o.__class__.__name__],
-        type: lambda self, o: [self.TRANSLATE_OBJ2KEY[o],self.IT_CONST_TYPE],
+        type: lambda self, o: [self.TRANSLATE_OBJ2KEY[o], self.IT_CONST_TYPE],
         bytes: lambda self, o: [list(o), self.BYTE_TYPE],
         list: lambda self, o: [[self.convert_to_json_item(i) for i in o],
                                self.ITER_TYPE,
                                o.__class__.__name__],
         deque: lambda self, o: [[self.convert_to_json_item(i) for i in o],
                                 self.ITER_TYPE,
                                 o.__class__.__name__],
         set: lambda self, o: [[self.convert_to_json_item(i) for i in o],
                               self.ITER_TYPE,
                               o.__class__.__name__],
         dict: lambda self, o: [[(self.convert_to_json_item(k),
-                               self.convert_to_json_item(v)) for k, v in o.items()],
+                                 self.convert_to_json_item(v)) for k, v in o.items()],
                                self.DICT_TYPE, o.__class__.__name__],
         OrderedDict: lambda self, o: [[(self.convert_to_json_item(k),
-                                     self.convert_to_json_item(v)) for k, v in o.items()],
-                                     self.DICT_TYPE, o.__class__.__name__],
-       }
+                                        self.convert_to_json_item(v)) for k, v in o.items()],
+                                      self.DICT_TYPE, o.__class__.__name__],
+    }
 
     CONVERT_FROM_JSON_MAP = {
         ALL_TYPE: lambda self, o: o[0],
-        BYTE_TYPE: lambda self, o: b''.join([i.to_bytes(1,'little') for i in o[0]]),
-        DICT_TYPE: lambda self,o: eval(o[2])([(self.convert_from_json_obj(k),self.convert_from_json_obj(v)) for k,v in o[0]]),
-        ITER_TYPE: lambda self,o: eval(o[2])([self.convert_from_json_obj(v) for v in o[0]]),
-        NP_TYPE: lambda self,o: self.convert_numpy(o[0],o[3],o[4]),
-        IT_CONST_TYPE: lambda self,o: self.TRANSLATE_KEY2OBJ[o[0]],
-        IT_TYPE: lambda self,o: self.convert_it_type(o)
-        }
+        BYTE_TYPE: lambda self, o: b''.join([i.to_bytes(1, 'little') for i in o[0]]),
+        DICT_TYPE: lambda self, o: eval(o[2])(
+            [(self.convert_from_json_obj(k), self.convert_from_json_obj(v)) for k, v in o[0]]),
+        ITER_TYPE: lambda self, o: eval(o[2])([self.convert_from_json_obj(v) for v in o[0]]),
+        NP_TYPE: lambda self, o: self.convert_numpy(o[0], o[3], o[4]),
+        IT_CONST_TYPE: lambda self, o: self.TRANSLATE_KEY2OBJ[o[0]],
+        IT_TYPE: lambda self, o: self.convert_it_type(o)
+    }
 
     if np_loaded:
-        CONVERT_MAP[np.ndarray]= lambda self,o: [[int(i) for i in o.tobytes()],
-                                                 self.NP_TYPE,
-                                                 o.__class__.__name__,
-                                                 str(o.dtype),
-                                                 list(o.shape)]
+        CONVERT_MAP[np.ndarray] = lambda self, o: [[int(i) for i in o.tobytes()],
+                                                   self.NP_TYPE,
+                                                   o.__class__.__name__,
+                                                   str(o.dtype),
+                                                   list(o.shape)]
 
     def __init__(self, itree_class):
-        self.itree_class=itree_class
+        self.itree_class = itree_class
         self.json = JSON
 
-        #from ..itree_main import iTree
-
-    def convert_to_json_item(self,o):
+    def convert_to_json_item(self, o):
         try:
-            t=type(o)
-            cm=self.CONVERT_MAP
+            t = type(o)
+            cm = self.CONVERT_MAP
             if t in cm:
-                return cm[t](self,o)
+                return cm[t](self, o)
             elif hasattr(o, 'get_init_args'):
                 return [self.convert_to_json_item(o.get_init_args()), self.IT_TYPE,
-                                          o.__class__.__name__,
-                                          o.__class__.__module__]
-            elif hasattr(o,'__iter__') or hasattr(o,'__next__') : # This is an iterable
+                        o.__class__.__name__,
+                        o.__class__.__module__]
+            elif hasattr(o, '__iter__') or hasattr(o, '__next__'):  # This is an iterable
                 convert_to_json_item = self.convert_to_json_item
                 if hasattr(o, 'items') and callable(o.items):  # dict indication
                     return [[(convert_to_json_item(k), convert_to_json_item(v)) for k, v in o.items()],
                             self.DICT_TYPE, o.__class__.__name__]
                 else:
-                    return [[convert_to_json_item(i) for i in o],self.ITER_TYPE,o.__class__.__name__]
+                    return [[convert_to_json_item(i) for i in o], self.ITER_TYPE, o.__class__.__name__]
             else:
-                return [o,self.ALL_TYPE]
+                return [o, self.ALL_TYPE]
         except:
             print('Issue in converting item {}'.format(o))
             raise
 
-    def convert_numpy(self,data,dtype,shape):
+    def convert_numpy(self, data, dtype, shape):
         raw_bytes = np.array(data, dtype=np.uint8)
         flat_array = np.frombuffer(raw_bytes, dtype)
         return flat_array.reshape(shape)
 
-    def convert_it_type(self,o):
+    def convert_it_type(self, o):
         class_name = o[2]
         object_class = None
         try:
             object_class = eval(class_name)
         except:
             pass
         if object_class is None:
@@ -221,45 +227,45 @@
                     except:
                         pass
         if object_class is None:
             raise TypeError('Target-Object: %s.%s could not be created, '
                             'ensure related import (from xxx import yyy is available' % (module_name, class_name))
         return object_class(*self.convert_from_json_obj(o[0]))
 
-    def convert_from_json_obj(self,json_obj):
+    def convert_from_json_obj(self, json_obj):
 
         try:
             try:
                 t = json_obj[1]
             except:
                 return json_obj
-            return self.CONVERT_FROM_JSON_MAP[t](self,json_obj)
+            return self.CONVERT_FROM_JSON_MAP[t](self, json_obj)
         except Exception as e:
             args = list(e.args)
             args[0] = 'Issue in object %s; \n%s' % (repr(json_obj), args[0])
             e.args = tuple(args)
             raise
 
-    def convert_single_itree_to_json_obj(self,depth,itree,fidx):
-        convert_to_json_item=self.convert_to_json_item
-        data=[depth,fidx]
+    def convert_single_itree_to_json_obj(self, depth, itree, fidx):
+        convert_to_json_item = self.convert_to_json_item
+        data = [depth, fidx]
         data.extend(convert_to_json_item(arg) for arg in itree.__class__._get_args_skip_subtree(itree))
         try:
-            return b' '*2*depth+JSON.dumps(data)
+            return b' ' * 2 * depth + JSON.dumps(data)
         except TypeError as e:
-            raise TypeError('%s -> %s'%(str(e),str((itree))))
+            raise TypeError('%s -> %s' % (str(e), str((itree))))
 
-    def convert_single_itree_to_json_obj2(self,depth,itree,fidx):
-        convert_to_json_item=self.convert_to_json_item
-        data=[depth,fidx]
+    def convert_single_itree_to_json_obj2(self, depth, itree, fidx):
+        convert_to_json_item = self.convert_to_json_item
+        data = [depth, fidx]
         data.extend(convert_to_json_item(arg) for arg in itree.__class__._get_args_skip_subtree(itree))
         try:
-            return b' '*2*depth+bytes(JSON.dumps(data, indent=2).encode('utf8', errors='backslashreplace'))
+            return b' ' * 2 * depth + bytes(JSON.dumps(data, indent=2).encode('utf8', errors='backslashreplace'))
         except TypeError as e:
-            raise TypeError('%s -> %s'%(str(e),str((itree))))
+            raise TypeError('%s -> %s' % (str(e), str((itree))))
 
     def dumps(self, o, add_header=False, calc_hash=False, filter_method=None):
         """
         In JSON the iTree object is represented in the following form
         Item-> dict with all properties (Special keys used)
         Tree structure is stored in list
 
@@ -269,39 +275,46 @@
         :param calc_hash: True - A sha1 hash is calculated over the data section of iTree and added in the header
                           False - no hash will be calculated
 
         :rtype: tuple
         :return: hash,string containing the serialized data -> if no hash calculation requested hash will be None
         """
         if IS_ORJSON:
-            convert=self.convert_single_itree_to_json_obj
+            convert = self.convert_single_itree_to_json_obj
         else:
             convert = self.convert_single_itree_to_json_obj2
 
         if filter_method:
-            tree_json = [convert(d, i, fidx) for d, fidx, i in o.__class__._iter_deep_locals_add_placeholders_filtered(o,filter_method)]
+            tree_json = [convert(d, i, fidx) for d, fidx, i in
+                         o.__class__._iter_deep_locals_add_placeholders_filtered(o, filter_method)]
         else:
-            tree_json = [convert(d,i,fidx) for d,fidx,i in o.__class__._iter_deep_locals_add_placeholders(o)]
-        dt_str=b'[\n'+convert(0,o,0)+b',\n'+b',\n'.join(tree_json)+b'\n]'
+            tree_json = [convert(d, i, fidx) for d, fidx, i in o.__class__._iter_deep_locals_add_placeholders(o)]
+        dt_str = b'[\n' + convert(0, o, 0) + b',\n' + b',\n'.join(tree_json) + b'\n]'
         if calc_hash:
             data_hash = hashlib.sha256(dt_str).hexdigest()
         if add_header:
-            header_dict = {'TYPE': 'itertree.iTree', 'VERSION': DT_SERIALIZE_VERSION}
+            class_name = self.itree_class.__name__
+            if class_name == 'iTree':
+                full_name = 'itertree.iTree'
+            else:
+                module = self.itree_class.__module__
+                full_name = module + '.' + class_name
+            header_dict = {'TYPE': full_name, 'VERSION': DT_SERIALIZE_VERSION}
             if calc_hash:
                 header_dict['HASH'] = data_hash
             if IS_ORJSON:
                 header_str = JSON.dumps(header_dict)
             else:
-                header_str = bytes(JSON.dumps(header_dict,indent=2).encode('utf8', errors='backslashreplace'))
-            dt_str = b'[\n'+header_str+b',\n'+dt_str+b']'
+                header_str = bytes(JSON.dumps(header_dict, indent=2).encode('utf8', errors='backslashreplace'))
+            dt_str = b'[\n' + header_str + b',\n' + dt_str + b']'
         if calc_hash:
-            return data_hash,dt_str
+            return data_hash, dt_str
         return dt_str
 
-    def dump(self, o, file_path, pack=True, calc_hash=True, overwrite=False,filter_method=None):
+    def dump(self, o, file_path, pack=True, calc_hash=True, overwrite=False, filter_method=None):
         """
         Serialize iTree object into a file
 
         :param o: iTree object to be serialized
         :param file_path: target file path where to store the data in
         :param pack: True - gzip the data, False - do not zip
         :param overwrite: True - an existing fie will be overwritten
@@ -315,64 +328,66 @@
             is_hdl = False
             if os.path.exists(file_path):
                 if not overwrite:
                     raise FileExistsError('Error file "%s" exists already' % file_path)
                 if os.path.isdir(file_path):
                     raise FileExistsError('Error dir with name "%s" exists already' % file_path)
         if calc_hash:
-            data_hash,data = self.dumps(o, add_header=True,calc_hash=calc_hash,filter_method=filter_method)
+            data_hash, data = self.dumps(o, add_header=True, calc_hash=calc_hash, filter_method=filter_method)
         else:
             data = self.dumps(o, add_header=True, calc_hash=calc_hash, filter_method=filter_method)
         if pack:
             data = gzip.compress(data)
         if is_hdl:
             file_path.write(data)
         else:
             with open(file_path, 'wb') as fh:
                 fh.write(data)
         return data_hash if calc_hash else True
 
-    def create_itree_from_raw(self,raw_o):
-        convert_from_json_obj=self.convert_from_json_obj
-        itree_class=self.itree_class
-        #root=itree_class(*[convert_from_json_obj(arg)  for arg in raw_o[2:]])
-        level_datas=[[]]
+    def create_itree_from_raw(self, raw_o):
+        convert_from_json_obj = self.convert_from_json_obj
+        itree_class = self.itree_class
+        # root=itree_class(*[convert_from_json_obj(arg)  for arg in raw_o[2:]])
+        level_datas = [[]]
         for item_data in raw_o:
             try:
-                depth=item_data[0]
-                s=len(level_datas)-1
-                if depth==s:
+                depth = item_data[0]
+                s = len(level_datas) - 1
+                if depth == s:
                     level_datas[depth].append(item_data)
-                elif depth==s+1:
+                elif depth == s + 1:
                     level_datas.append([item_data])
-                elif depth<s:
-                    for _ in range(s-depth):
-                        main_args=level_datas[-2][-1]
-                        if len(main_args)>2:
-                            a=1
+                elif depth < s:
+                    for _ in range(s - depth):
+                        main_args = level_datas[-2][-1]
+                        if len(main_args) > 2:
+                            a = 1
                         if type(main_args) is not list:
-                            raise SyntaxError('Something wrong in structure in between {} and {}'.format(main_args,item_data))
-                        it = itree_class(convert_from_json_obj(main_args[2]), # tag
-                                         convert_from_json_obj(main_args[3]), # value
+                            raise SyntaxError(
+                                'Something wrong in structure in between {} and {}'.format(main_args, item_data))
+                        it = itree_class(convert_from_json_obj(main_args[2]),  # tag
+                                         convert_from_json_obj(main_args[3]),  # value
                                          # subtree:
                                          (itree_class(*[convert_from_json_obj(arg)
                                                         for arg in args[2:]])
-                                         if type(args) is list else args for args in level_datas[-1]),
+                                          if type(args) is list else args for args in level_datas[-1]),
                                          # additional arguments
                                          *[convert_from_json_obj(arg) for arg in main_args[5:]])
                         del level_datas[-1]
-                        level_datas[-1][-1]=it
+                        level_datas[-1][-1] = it
                     level_datas[-1].append(item_data)
                 else:
-                    raise SyntaxError('During build of iTree from serialized data '
-                                      'an implausible depth step upwards was found in item: {}'.format(str(item_data)))
+                    raise SyntaxError('During build of {} from serialized data '
+                                      'an implausible depth step upwards was found in item: {}'.format(
+                                       self.itree_class.__name__, str(item_data)))
             except:
                 print('Issue in {}'.format(item_data))
                 raise
-        for _ in range(len(level_datas)-1):
+        for _ in range(len(level_datas) - 1):
             main_args = level_datas[-2][-1]
             if type(main_args) is not list:
                 raise SyntaxError('Something wrong in structure in {}'.format(main_args))
             it = itree_class(convert_from_json_obj(main_args[2]),  # tag
                              convert_from_json_obj(main_args[3]),  # value
                              # subtree:
                              (itree_class(*[convert_from_json_obj(arg)
@@ -381,32 +396,32 @@
                              # additional arguments
                              *[convert_from_json_obj(arg) for arg in main_args[5:]])
             del level_datas[-1]
             level_datas[-1][-1] = it
 
         return it
 
-    def create_itree_from_raw2(self,raw_o):
-        convert_from_json_obj=self.obj_serializer.convert_from_json_obj
-        itree_class=self.itree_class
-        _,args=raw_o.pop(-1)
-        new_itree=itree_class(*[convert_from_json_obj(arg)  for arg in args])
-        last_kp=1
-        last_item=new_itree
-        for kp,args in raw_o:
-            if kp!=last_kp:
-                last_kp=kp
-                new_index=[-1]*(kp-1)
+    def create_itree_from_raw2(self, raw_o):
+        convert_from_json_obj = self.obj_serializer.convert_from_json_obj
+        itree_class = self.itree_class
+        _, args = raw_o.pop(-1)
+        new_itree = itree_class(*[convert_from_json_obj(arg) for arg in args])
+        last_kp = 1
+        last_item = new_itree
+        for kp, args in raw_o:
+            if kp != last_kp:
+                last_kp = kp
+                new_index = [-1] * (kp - 1)
                 last_item = new_itree.getitem_deep(new_index)
-                #for _ in range((kp-1)):
+                # for _ in range((kp-1)):
                 #    last_item=last_item[-1]
             last_item._append(itree_class(*[convert_from_json_obj(arg) for arg in args]))
         return new_itree
 
-    def loads(self, source_str, check_hash=True, load_links=True,_source=None):
+    def loads(self, source_str, check_hash=True, load_links=True, _source=None):
         """
         create an iTree object by loading from a string.
 
         :param source_str: source string that contains the iTree information
         :param check_hash: True the hash of the file will be checked and the loading will be stopped if it doesn't match
                            False - do not check the iTree hash
         :param load_links: True - linked iTree objects will be loaded
@@ -416,35 +431,32 @@
         """
         if DECODE:
             raw_o = JSON.loads(source_str.decode('utf-8'))
         else:
             raw_o = JSON.loads(source_str)
         if type(raw_o) is not list:
             raise SyntaxError('Unknown input file format')
-        if len(raw_o)==2 and type(raw_o[0]) is dict:
+        if len(raw_o) == 2 and type(raw_o[0]) is dict:
             # header found
-            header_dict,tree_data=raw_o
-            if header_dict['TYPE'] != 'itertree.iTree':
-                raise SyntaxError('Unknown file format')
-            version=header_dict['VERSION']
-            i=version.rindex('.')
+            header_dict, tree_data = raw_o
+            version = header_dict['VERSION']
+            i = version.rindex('.')
             if version[:i] != DT_SERIALIZE_MAJOR_VERSION:
-                raise SyntaxError('Wrong version of DataTree data please convert first!')
+                raise SyntaxError('Wrong version of serialization file please convert first!')
             if check_hash and ('HASH' in header_dict):
-                i=source_str.find(b'},\n')+3
+                i = source_str.find(b'},\n') + 3
                 if hashlib.sha256(source_str[i:-1]).hexdigest() != header_dict['HASH']:
-                    raise PermissionError('Given DataTree data is corrupted (wrong hash)!')
+                    raise PermissionError('Given tree data is corrupted (wrong hash)!')
         else:
-            tree_data=raw_o
-        new_tree=self.create_itree_from_raw(tree_data)
+            tree_data = raw_o
+        new_tree = self.create_itree_from_raw(tree_data)
         if load_links:
             new_tree.load_links()
         return new_tree
 
-
     def load(self, file_path, check_hash=True, load_links=True):
         """
         create an iTree object by loading from a file
 
         :param file_path: file path to the file that contains the iTree information
         :param check_hash: True the hash of the file will be checked and the loading will be stopped if it doesn't match
                            False - do not check the iTree hash
@@ -462,13 +474,11 @@
         try:
             data = gzip.decompress(data)
         except OSError:
             # we might have an already unzipped file!
             pass
         # data=data.decode(decode)
         try:
-            file_path=os.path.abspath(file_path)
+            file_path = os.path.abspath(file_path)
         except:
             pass
-        return self.loads(data, check_hash, load_links,file_path)
-
-
+        return self.loads(data, check_hash, load_links, file_path)
```

### Comparing `itertree-1.0.5/src/itertree/itree_serializer/itree_render_dot.py` & `itertree-1.1.2/src/itertree/itree_serializer/itree_render_dot.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.5/src/itertree/itree_serializer/itree_renderer.py` & `itertree-1.1.2/src/itertree/itree_serializer/itree_renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         :param enumerate: add enumeration before the items
 
          :return: string containing the pretty print output
          """
         return self._render_main(itree_object,filter_method,enumerate,False)
 
     def _build_item_str(self,itree_object,enum_cnt=None):
-        out = ['iTree(']
+        out = ['%s('%itree_object.__class__.__name__]
         if itree_object._tag != NoTag:
             out.append(repr(itree_object._tag))
             out.append(', ')
         if itree_object._value != NoValue:
             out.append('value=')
             out.append(repr(itree_object._value))
             out.append(', ')
```

### Comparing `itertree-1.0.5/src/itertree.egg-info/PKG-INFO` & `itertree-1.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,21 @@
-Metadata-Version: 2.1
-Name: itertree
-Version: 1.0.5
-Summary: Python tree structure for data storage and iterations
-Home-page: https://github.com/BR1py/itertree
-Author: B_R
-Author-email: br_development@posteo.org
-License: MIT
-Project-URL: Bug Tracker, https://github.com/BR1py/itertree/issues
-Project-URL: Documentation, https://readthedocs.org/projects/itertree/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.4
-Description-Content-Type: text/markdown
-License-File: LICENSE
+[![Static Badge](https://img.shields.io/badge/itertree-https%3A%2F%2Fgithub.com%2FBR1py%2Fitertree-blue?logo=github)](https://github.com/BR1py/itertree)
+[![PyPI](https://img.shields.io/pypi/v/itertree)](https://pypi.org/project/itertree)
+![Static Badge](https://img.shields.io/badge/python-%3E%3D3.4-green)
+[![Static Badge](https://img.shields.io/badge/licence-MIT(hpp)-green)](https://github.com/BR1py/itertree/blob/main/LICENSE)
+[![Static Badge](https://img.shields.io/badge/documenation-https%3A%2F%2Fitertree.readthedocs.io%2Fen%2Flatest%2F-yellow?logo=readthedocs)](https://itertree.readthedocs.io/en/latest/)
+![GitHub Release 1.1.2 - Published_At](https://img.shields.io/github/release-date/Br1py/itertree)
+
 
 # itertree python package
 
 
 ## Welcome to itertree python package
 
-Release 1.0.5   - fully released
+Release 1.1.2  -  released
 
 * Do you have to store data in a tree like structure?
 * Do you need good performance and a reach feature set in the tree object?
 * You like to serialize and store the structure in files?
 * And is it helpful for you if you can link subtrees from other trees and add local items in this "inherited" parts?
 
 Please give itertree package a try!
@@ -110,14 +101,20 @@
     iTree('sub', value={'mykey': 3})
     >>> # Show tree content:
     >>> root.render()
     iTree('root', value={'mykey': 0})
      > iTree('sub', value={'mykey': 1})
      > iTree('sub', value={'mykey': 2})
      > iTree('sub', value={'mykey': 3})
+    >>> # Address item via tag-index-pair (key):
+    >>> root['sub', 1]
+    iTree('sub', value={'mykey': 2})
+    >>> # Address item via absolute-index and check stored value:
+    >>> root[1].value
+    {'mykey': 2}
    
 
 ## First steps
 
 All important classes of the package are published by the package `__init__.py` file so that the functionality of
 itertree can be reached by importing:
 
@@ -302,54 +299,7 @@
     >>> first_item = next(iter(root.deep)) # create an iterator from the generator object
     >>> fifth_item = list(root.deep)[4]  # and this is slower as:
     >>> import itertools
     >>> fifth_item = next(itertools.islice(root.deep, 4, None))
   
 
     
-## iterators vs. lists
-
-We named the package itertree because when ever a iTree operation delivers multiple items the result will be an
-iterator (and not a list what the user might expect).
-
-Iterators are very powerful objects especially if you have a huge number of items to be iterated over.
-Iterators can be created very fast and they can be combined. So you can create very effective filter functions. It's
-recommended to have a look in the powerful itertools and more_itertools packages to combine it with itertree
-
-The main idea is to combine all the filtering and iterator options together before you start the final iteration
-(consume the iterator), which might at least end up in the expected list. By this mechanism we do at least only one
-unique iteration over the items and we must not do multiple typecasts and re-iterations in between even when we
-combine multiple filters.
-
-If the user really wants to create a list he can easy cast the iterator by using the `list()` statement:
-
-    >>> myresultlist=list(root.iter_all()) #  this is quick even for huge number of items
-    >>> first_item=list(root.iter_all())[0] # Anyway this is much slower than:
-    >>> first_item=next(root.iter_all())
-    >>> fifth_item=list(root.iter_all())[4] # and this is much slower than:
-    >>> import itertools
-    >>> fifth_item=next(itertools.isslice(root.iter_all(),4,None))
-    
-
-As it is shown in the performance test the operation `list()` is very quick (less then 0.5 s on 1 million items
-(depending on you PC)). And using the index access afterwards is a very good readable code. But as shown here there
-are quicker solutions available on iterators only.
-
-But we see also two downsides related to iterators:
-
-* The StopIteration exception must be handled in case of empty iterators. To make the handling a bit easier iTree
-  delivers in most cases an empty list if we have no match. But in some cases (e.g. filter operations) the user
-  will get an empty iterator and not the empty list. In itree_helpers the user can find a check
-  function for empty iterators that might help in this case: `is_iterator_empty(my_iterator)`.
-
-* The user must also consider that an iterator can be consumed only one time. To reuse an iterator multiple times
-  you may have a look on `itertools.tee()`.
-
-To summarize this chapter: 
-
-We decided that the iTree methods should deliver only iterators (and not lists). This is made to give the user
-the possibility to utilize the whole iterator power afterwards. If he really needs a list (in most cases for
-index access) he can cast the iterator easy and quick via the `list()` statement. But if iTree would directly
-deliver lists by default we would have a performance drop in all itertree filter functions which is not
-acceptable from our point of view.
-
-
```

### Comparing `itertree-1.0.5/src/itertree.egg-info/SOURCES.txt` & `itertree-1.1.2/src/itertree.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,26 +16,28 @@
 src/itertree.egg-info/SOURCES.txt
 src/itertree.egg-info/dependency_links.txt
 src/itertree.egg-info/top_level.txt
 src/itertree/examples/__init__.py
 src/itertree/examples/calendar_example.py
 src/itertree/examples/itree_data_models.py
 src/itertree/examples/itree_docu_examples.py
+src/itertree/examples/itree_like_anytree.py
 src/itertree/examples/itree_link_example1.py
 src/itertree/examples/itree_usage_example1.py
 src/itertree/examples/itree_usage_example2.py
 src/itertree/itree_serializer/__init__.py
 src/itertree/itree_serializer/itree_json_converter.py
 src/itertree/itree_serializer/itree_json_serialize.py
 src/itertree/itree_serializer/itree_render_dot.py
 src/itertree/itree_serializer/itree_renderer.py
 tests/test_itertree_base1.py
 tests/test_itertree_base_old.py
-tests/test_itertree_examples.py
 tests/test_itertree_flags.py
 tests/test_itertree_full_feature_trees.py
+tests/test_itertree_helpers.py
 tests/test_itertree_intervals.py
 tests/test_itertree_iter.py
+tests/test_itertree_iter2.py
 tests/test_itertree_links.py
 tests/test_itertree_mathsets.py
 tests/test_itertree_serialize.py
 tests/test_itertree_value_models.py
```

### Comparing `itertree-1.0.5/tests/test_itertree_base1.py` & `itertree-1.1.2/tests/test_itertree_base1.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,15 +320,15 @@
         assert new_item.tag_idx[1] == tag_idx_old_new[1] + 1
 
         # appendleft() should be quicker then insert(0,..)
         testtree = iTree()
         t1 = calc_timeit(lambda: testtree.appendleft(iTree()), number=100)
         testtree = iTree()
         t2 = calc_timeit(lambda: testtree.insert(0, iTree()), number=100)
-        if BLIST_ACTIVE:
+        if BLIST_ACTIVE and False: #  we skip the test it fails on newer python versions
             assert t1 < t2
 
         # extend list
         l = len(itree)
         itree.extend([iTree('new2') for i in range(5)])
         assert len(itree) == l + 5
         assert itree[-1].tag_idx[1] == 4
@@ -1421,25 +1421,31 @@
         c_ti = c.tag_idx
         assert c_ti[1] == 2
         d_ti = d.tag_idx
         assert d_ti[1] == 3
 
         old_itree = itree_root.copy()
         # reversed
-        new_reveresed = reversed(itree_root)
+        new_reversed = list(reversed(itree_root))
+
+        assert itree_root[0].tag_idx == a_ti
+        assert itree_root[1].tag_idx == b_ti
+        assert itree_root[-2].tag_idx == c_ti
+        assert itree_root[-1].tag_idx == d_ti
 
-        assert new_reveresed[0].tag_idx == a_ti
-        assert new_reveresed[1].tag_idx == b_ti
-        assert new_reveresed[-2].tag_idx == c_ti
-        assert new_reveresed[-1].tag_idx == d_ti
+        assert new_reversed[-1].tag_idx == a_ti
+        assert new_reversed[-2].tag_idx == b_ti
+        assert new_reversed[1].tag_idx == c_ti
+        assert new_reversed[0].tag_idx == d_ti
 
         # reverse
         itree_root.reverse()
 
-        assert itree_root == new_reveresed
+        for i,ii in zip(itree_root,new_reversed):
+            assert i is ii
 
         assert itree_root[0] is d
         assert itree_root[1] is c
         assert itree_root[-2] is b
         assert itree_root[-1] is a
 
         assert itree_root[0].tag_idx == a_ti
@@ -1640,14 +1646,68 @@
         # self and other have equal but not same coupled object
         coupled_obj3 = {1: 1}
         new_itree2.set_coupled_object(coupled_obj3)
         assert not itree_root[1].equal(new_itree2, check_coupled=True)
 
         print('\nRESULT OF TEST: iTree properties-> PASS')
 
+    def test6b_iTree_properties(self):
+        if not 6 in TEST_SELECTION:
+            return
+        print('\nRESULT OF TEST: iTree properties(b)')
+        # build a small tree
+        itree_root = iTree(1, 1)
+        itree_root += iTree(1.0, 2)
+        itree_root += iTree(1.1, 3)
+        itree_root += iTree(1.2, 4)
+        itree_root += iTree(1.3, 5)
+
+        itree_root[0] += iTree(1.00, 6)
+        itree_root[0] += iTree(1.01, 7)
+        itree_root[0] += iTree(1.02, 8)
+        itree_root[0] += iTree(1.03, 9)
+
+        itree_root[1] += iTree(1.10, 6)
+        itree_root[1] += iTree(1.12, 7)
+        itree_root[1] += iTree(1.13, 8)
+        itree_root[1] += iTree(1.14, 9)
+
+        itree_root[2] += iTree(1.20, 6)
+        itree_root[2] += iTree(1.22, 7)
+        itree_root[2] += iTree(1.23, 8)
+        itree_root[2] += iTree(1.24, 9)
+
+        itree_root[3] += iTree(1.30, 6)
+        itree_root[3] += iTree(1.32, 7)
+        itree_root[3] += iTree(1.33, 8)
+        itree_root[3] += iTree(1.34, 9)
+        itree_root[3] += iTree(1.34, 10)
+
+        #ancestors
+
+        low_level_item=itree_root[1].append(iTree('sub')).append(iTree('subsub'))
+        a=low_level_item.ancestors
+        assert len(a)==3
+        assert a[0] == itree_root
+        assert a[1]==itree_root[1]
+        assert a[2]==itree_root[1][-1]
+
+        #siblings
+
+        s=list(itree_root[1].siblings)
+        s2=list(itree_root)
+        assert len(s)+1==len(s2)
+        i=0
+        for item in s2:
+            if item is not itree_root[1]:
+                assert item==s[i]
+                i += 1
+
+        print('\nRESULT OF TEST: iTree properties(b) -> PASS')
+
     def test7_iTree_internals_methods(self):
         if not 7 in TEST_SELECTION:
             return
         print('\nRESULT OF TEST: iTree internals')
 
         # _value_equal
         root = iTree()
@@ -1807,34 +1867,34 @@
         print('\nRESULT OF TEST: iTree other methods')
         largetree, size = self.large_itree([10000, 2], ['tag_it'], 'cnt')
 
         # do some tests on count and len
         assert len(largetree) == 10000
         assert len(largetree.deep) == size
 
-        myfilter = lambda i: i.value <= 100
+        myfilter = lambda i: type(i.value) is int and i.value <= 100
         for i in largetree:
             if i.value > 100:
                 break
         assert largetree.filtered_len(myfilter) == i.idx
         myfilter = lambda i: i.value > 100
         assert largetree.filtered_len(myfilter) == len(largetree) - i.idx
         myfilter = lambda i: False
         assert largetree.filtered_len(myfilter) == 0
         myfilter = lambda i: True
         assert largetree.filtered_len(myfilter) == len(largetree)
 
         # do some tests on count_deep
         assert len(largetree.deep) == size
-        myfilter = lambda i: i.value <= 1000
+        myfilter = lambda i: type(i.value) is int and i.value <= 1000
         assert sum(1 for _ in filter(myfilter, largetree.deep)) == 1000
         assert largetree.deep.filtered_len(myfilter, True) == 1000
         assert largetree.deep.filtered_len(myfilter, False) == 1000
 
-        myfilter = lambda i: i.value > 1000
+        myfilter = lambda i: type(i.value) is int and i.value > 1000
         assert largetree.deep.filtered_len(myfilter, True) == size - 1001 - 1
         assert largetree.deep.filtered_len(myfilter, False) == size - 1000
         assert sum(1 for _ in filter(myfilter, largetree.deep)) == size - 1000
         myfilter = lambda i: False
         assert largetree.deep.filtered_len(myfilter, True) == 0
         assert largetree.deep.filtered_len(myfilter, False) == 0
         assert sum(1 for _ in filter(myfilter, largetree.deep)) == 0
```

### Comparing `itertree-1.0.5/tests/test_itertree_base_old.py` & `itertree-1.1.2/tests/test_itertree_base_old.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.5/tests/test_itertree_flags.py` & `itertree-1.1.2/tests/test_itertree_flags.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.5/tests/test_itertree_full_feature_trees.py` & `itertree-1.1.2/tests/test_itertree_full_feature_trees.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.5/tests/test_itertree_intervals.py` & `itertree-1.1.2/tests/test_itertree_intervals.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.5/tests/test_itertree_iter.py` & `itertree-1.1.2/tests/test_itertree_iter.py`

 * *Files 0% similar despite different names*

```diff
@@ -929,18 +929,16 @@
         t = calc_timeit(lambda: list(i for i in iter_method(test_filter,up_to_low=True)), number=timeit_number)
         print('%s(test_filter) -> iteration-time over %s items: %es' % (method_name, s, t))
 
         s = len(list(i for i in filter(test_filter_outside,iter_method(up_to_low=True))))
         t = calc_timeit(lambda: list(i for i in filter(test_filter_outside,iter_method(up_to_low=True))), number=timeit_number)
         print('filter(test_filter,%s()) -> iteration-time over %s items: %es' % (method_name, s, t))
 
-
         print('\nRESULT OF TEST: iTree deep key_paths iterators -> PASS')
 
-
     def test2_iTree_unit_filters(self):
         # filters are tested in a special test
         if not 2 in TEST_SELECTION:
             return
         print('\nRESULT OF TEST: iTree unit test filters')
         # iTFilter class
```

### Comparing `itertree-1.0.5/tests/test_itertree_links.py` & `itertree-1.1.2/tests/test_itertree_links.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.5/tests/test_itertree_mathsets.py` & `itertree-1.1.2/tests/test_itertree_mathsets.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.5/tests/test_itertree_serialize.py` & `itertree-1.1.2/tests/test_itertree_serialize.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.5/tests/test_itertree_value_models.py` & `itertree-1.1.2/tests/test_itertree_value_models.py`

 * *Files identical despite different names*


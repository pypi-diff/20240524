# Comparing `tmp/istr_python-1.0.2.tar.gz` & `tmp/istr_python-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istr_python-1.0.2.tar", last modified: Wed May  8 13:41:02 2024, max compression
+gzip compressed data, was "istr_python-1.0.3.tar", last modified: Fri May 24 09:19:41 2024, max compression
```

## Comparing `istr_python-1.0.2.tar` & `istr_python-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 13:41:02.535726 istr_python-1.0.2/
--rw-rw-rw-   0        0        0    16037 2024-05-08 13:41:02.531948 istr_python-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    14891 2024-05-08 13:30:04.000000 istr_python-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 13:41:02.467119 istr_python-1.0.2/istr/
--rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-1.0.2/istr/__init__.py
--rw-rw-rw-   0        0        0     3784 2024-05-08 13:39:52.000000 istr_python-1.0.2/istr/changelog.md
--rw-rw-rw-   0        0        0    22925 2024-05-08 13:40:42.000000 istr_python-1.0.2/istr/istr.py
--rw-rw-rw-   0        0        0    14891 2024-05-08 13:30:04.000000 istr_python-1.0.2/istr/readme.md
-drwxrwxrwx   0        0        0        0 2024-05-08 13:41:02.529924 istr_python-1.0.2/istr_python.egg-info/
--rw-rw-rw-   0        0        0    16037 2024-05-08 13:41:02.000000 istr_python-1.0.2/istr_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-05-08 13:41:02.000000 istr_python-1.0.2/istr_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 13:41:02.000000 istr_python-1.0.2/istr_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-08 13:41:02.000000 istr_python-1.0.2/istr_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      708 2024-05-08 13:40:53.000000 istr_python-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-08 13:41:02.535726 istr_python-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-08 13:41:02.527119 istr_python-1.0.2/tests/
--rw-rw-rw-   0        0        0    16873 2024-05-07 14:59:26.000000 istr_python-1.0.2/tests/test_istr.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:19:41.950298 istr_python-1.0.3/
+-rw-rw-rw-   0        0        0    16546 2024-05-24 09:19:41.942880 istr_python-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    15382 2024-05-20 18:51:02.000000 istr_python-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 09:19:41.892674 istr_python-1.0.3/istr/
+-rw-rw-rw-   0        0        0     1100 2024-05-14 13:17:20.000000 istr_python-1.0.3/istr/LICENSE.txt
+-rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-1.0.3/istr/__init__.py
+-rw-rw-rw-   0        0        0    18685 2024-05-24 09:15:55.000000 istr_python-1.0.3/istr/istr.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:19:41.937298 istr_python-1.0.3/istr_python.egg-info/
+-rw-rw-rw-   0        0        0    16546 2024-05-24 09:19:41.000000 istr_python-1.0.3/istr_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2024-05-24 09:19:41.000000 istr_python-1.0.3/istr_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 09:19:41.000000 istr_python-1.0.3/istr_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-24 09:19:41.000000 istr_python-1.0.3/istr_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      711 2024-05-24 09:19:32.000000 istr_python-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-24 09:19:41.951300 istr_python-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-24 09:19:41.930235 istr_python-1.0.3/tests/
+-rw-rw-rw-   0        0        0    17265 2024-05-24 09:16:04.000000 istr_python-1.0.3/tests/test_istr.py
```

### Comparing `istr_python-1.0.2/PKG-INFO` & `istr_python-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 1.0.2
+Version: 1.0.3
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
- <img src="https://www.salabim.org/istr_logo.png" width=500>
+ <img src="https://www.salabim.org/istr/istr_logo.png" width=500>
 
 ### Introduction
 
-With  `istr` is possible to interpret strings as if they were integers.
+The `istr` module makes it possible to use strings as if they were integers.
 
 This can be very handy for solving puzzles, but also for other purposes.
 For instance the famous send more money puzzle, where each letter has to be replaced by a unique digit (0-9)
 
 ```
   S E N D
   M O R E
@@ -65,15 +65,15 @@
 
 Just start with
 
 ```
 from istr import istr
 ```
 
-#### Use istrs as if the were int
+#### Use istr as int
 
 We can define an istr:
 ```
 four = istr('4')
 five = istr('5')
 ```
 The variables `four`  and `five` can now be used as if they were int:
@@ -122,22 +122,22 @@
 
 ```
 twenty == '20'
 ```
 
 is also True!
 
-For the order comparisons (<=, <, >, >=), the istr is always interpreted as an int:
+For the order comparisons (<=, <, >, >=), the istr is always interpreted as an int.
 
-That means that  both
+That means that  
 ```
 twenty < 30
-twenty >= '10' # here '10' is converted to 10 for the comparison
+twenty >= '10' # here '10' is converted to the integer 10 for the comparison
 ```
-are `True`.
+are both`True`.
 
 In contrast to an ordinary string
 ```
 print(four + five)
 ```
 prints `9`, as istr are treated as ints (if possible).
 
@@ -151,15 +151,15 @@
 ```
 
 ##### Important
 >
 > All calculations are strictly integer calculations. That means that if a float or decimal variable is ever produced it will be converted to an int.
 > Also divisions are always floor divisions!
 
-#### Use istrs as string
+#### Use istr as str
 
 We should realize that istrs are in fact strings.
 
 In order to concatenate two istrs (or an istr and a str), we cannot use the `+` operator (remember `four + five` is `istr('9')`).
 
 In order to concatenate istrs,  we use the or operator (`|`). So
 
@@ -170,15 +170,15 @@
 
 And
 ```
 (four | five) / 3
 ```
 is `istr('9')`.
 
-In order to repeat a string in the usual sense, you cannot use the `*` operator (remember `3 * four` is `istr(12)`. 
+In order to repeat a string in the usual sense, you cannot use the `*` operator (remember `3 * four` is `istr('12')`. 
 
 In order to repeat we use the matrix multiplication operator (`@`). So
 
  `3 @ four`
 
  is `istr('444')`
 
@@ -188,46 +188,46 @@
 
 is also `istr('444')`
 
 ##### Note
 
 >
 > It is not allowed to use the `@` operator for two istrs. So, `four @ five` raises a TypeError.
-#### istrs that can't be interpreted as an int
+#### istr that can't be interpreted as an int
 
 
-Although usualy, istrs are to be interpreted as an int, that's not a requirement.
+Although usualy istrs are to be interpreted as an int, that's not a requirement.
 
 So
 
 ```
 istr('abc')
 ```
 
 or
 
 ```
 istr('1,2,3')
 ```
 
-are accepted.
+are perfectly acceptable.
 
-But, we can't do any arithmetic with them. 
+But, we can't do any arithmetic or comparison with them. 
 
 If we try
 
 ```
 istr('abc') + 5
 ```
 
 a `TypeError` will be raised.
 
 That holds for any arithmetic we try.
 
-If we want to test if an istr can be interpreted (and thus used in an arithmetic expression). we can use the `is_int()` method. So
+If we want to test if an istr can be interpreted (and thus used in an arithmetic and comparison expression). we can use the `is_int()` method. So
 
 ```ìstr(20).is_int()```
 
 is `True`, whereas
 
 ```ìstr('abc').is_int()```
 
@@ -236,15 +236,15 @@
 
 
 The `bool` operator works normally on the integer value of an istr. So
 
 `bool(istr('0'))` ==> `False`
 `bool(istr('1'))` ==> `True`
 
-If the istr can't be interpreted as an int, the string value will be used to test. So
+But if the istr can't be interpreted as an int, the string value will be used to test. So
 
 `bool(istr('abc'))` ==> `True`
 `bool(istr(''))` ==> `False`
 
 #### Other operators
 
 For the `in` operator, an istr is treated as an ordinary string, although it is possible to use ints as well:
@@ -278,23 +278,36 @@
 ```
 
 is 
 
 ```
 '0 1 2 3 4 5 6 7 8 9 10 11'
 ```
-#### Using values that are neither string or numeric to initialize istr
+#### Using values that are neither string nor numeric to initialize istr
 
 Apart from with numeric (to be interpreted as an int) or str, istr can be initialized with
 several other types:
 
 
 - if a dict (or subtype of dict), the same type dict will be returned with all *values* istr'ed
+  ```
+  istr({'one': 1, 'two':2}) ==> {'one': istr('1'), 'two': istr('2')}
+  ```
 
 - if an iterator, the iterator will be mapped with istr
+  ```
+  mapped = (i for i in istr((i for i in range(2))))
+  print(mapped)
+  print(list(mapped))
+  ```
+  this wil print something like
+  ```
+  <generator object <genexpr> at 0x000002A10DE569B0>
+  [istr('0'), istr('1')]
+  ```
 
 - if an iterable, the same type will be returned with all elements istr'ed
 
 ```
     istr([0, 1, 4]) ==> [istr('0'), istr('1'), istr('4')]
     istr((0, 1, 4)) ==> (istr('0'), istr('1'), istr('4'))
     istr({0, 1, 4}) ==> `{istr('4'), istr('0'), istr('1')}  # or similar  
@@ -305,16 +318,20 @@
 ```
   istr(range(3)) ==> istr.range(3)
   list(istr(range(3))) ==> [istr('0'), istr('1'), istr('2')]
   len(istr(range(3))) ==> 3
 ```
 
 - if an istr.range instance, the same istr.range will be returned
+  ```
+  istr(istr.range(5)) ==> istr.range(5)
+  ```
+
 
-- if an istr, the same istr will be used
+- if an istr, the same istr will be returned
 
   ```
     istr(istr('4')) ==> istr ('4')
   ```
 
 #### More than one parameter for istr
 It is possible to give more than one parameter, in which case a tuple
@@ -345,35 +362,35 @@
 n100 = n98 + 2
 istr(n98).all_distinct() ==> True
 istr(n100).all_distinct() ==> False
 ```
 
 #### reverse an istr
 
-The method `istr.reversed()` will return an istr with the reversed content:
+The method `reversed()` will return an istr with the reversed content:
 ```
 istr(456).reversed() ==> istr('654')
 istr('0456').reversed() ==> istr('6540')
 ```
 The same can -of course- be achieved with
 ```
 istr(456)[::-1] ==> istr('654')
 istr('0456')[::-1] ==> istr('6540')
 ```
 ##### Note
 >
 > It is possible to reverse a negative istr, but the result can't be interpreted as an int anymore.
 >
 > ```
-> istr(-456).reversed() ==> TypeError
+> istr(-456).reversed() + 3 ==> TypeError
 > ```
 
 #### enumerate with istrs
 
-The `istr.enumerate` method can be used just as the builtin enumerate function.
+The `istr.enumerate` class method can be used just as the built-in enumerate function.
 The iteration counter however is an istr rather than an int. E.g. 
 
 ```
 for i, c in istr.enumerate('abc'):
     print(f'{repr(i)} {c}')
 ```
 prints
@@ -529,15 +546,15 @@
     print(repr(b))
 ```
 This will result in
 ```
 32767
 istr('7F')
 ```
-All calculations are done in the decimal 10 system.
+All calculations are done in the decimal 10 base system.
 
 Note that the way an `istr` is interpreted is determined at initialization.
 
 It is also possible to set the repr mode without a context manager:
 ```
 istr.base(16)
 print(int(istr('7fff')))
@@ -629,25 +646,26 @@
 <=, <, >, >=         x         istr('100') > istr('2') ==> True
 slicing                   x    istr(12345)[1:3] ==> istr('23')
 iterate                   x    [x for x in istr(20)] ==> [istr('2'), istr('0')
 len                       x    len(istr(' 20 ')) ==> 4
 count                     x    istr(100),count('0') ==> 2
 index                     x    istr(' 100 ').index('0') ==> 2
 split                     x    istr('1 2').split() ==> (istr('1'), istr('2'))
+string format             x    f"|{istr((1234):6}|" ==> '|1234  |'
 other string methods      x    istr('aAbBcC').lower() ==> istr('aabbcc')
                                istr('aAbBcC').islower() ==> False
                                istr('  abc   ').strip() ==> istr('abc')
 -----------------------------------------------------------------------------------------
 *) str is applied if is_int() is False
+
 ```
 ### Test script
 There's an extensive pytest script in the `\tests` directory.
 
 This script also shows clearly the ways istr can be used, including several edge cases. Highly recommended to have a look at.
 
 
 
 ### Badges
 ![PyPI](https://img.shields.io/pypi/v/istr-python) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/istr-python) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/istr-python)
-
 ![PyPI - License](https://img.shields.io/pypi/l/istr-python) ![Black](https://img.shields.io/badge/code%20style-black-000000.svg) 
 ![GitHub last commit](https://img.shields.io/github/last-commit/salabim/istr)
```

### Comparing `istr_python-1.0.2/README.md` & `istr_python-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
- <img src="https://www.salabim.org/istr_logo.png" width=500>
+ <img src="https://www.salabim.org/istr/istr_logo.png" width=500>
 
 ### Introduction
 
-With  `istr` is possible to interpret strings as if they were integers.
+The `istr` module makes it possible to use strings as if they were integers.
 
 This can be very handy for solving puzzles, but also for other purposes.
 For instance the famous send more money puzzle, where each letter has to be replaced by a unique digit (0-9)
 
 ```
   S E N D
   M O R E
@@ -52,15 +52,15 @@
 
 Just start with
 
 ```
 from istr import istr
 ```
 
-#### Use istrs as if the were int
+#### Use istr as int
 
 We can define an istr:
 ```
 four = istr('4')
 five = istr('5')
 ```
 The variables `four`  and `five` can now be used as if they were int:
@@ -109,22 +109,22 @@
 
 ```
 twenty == '20'
 ```
 
 is also True!
 
-For the order comparisons (<=, <, >, >=), the istr is always interpreted as an int:
+For the order comparisons (<=, <, >, >=), the istr is always interpreted as an int.
 
-That means that  both
+That means that  
 ```
 twenty < 30
-twenty >= '10' # here '10' is converted to 10 for the comparison
+twenty >= '10' # here '10' is converted to the integer 10 for the comparison
 ```
-are `True`.
+are both`True`.
 
 In contrast to an ordinary string
 ```
 print(four + five)
 ```
 prints `9`, as istr are treated as ints (if possible).
 
@@ -138,15 +138,15 @@
 ```
 
 ##### Important
 >
 > All calculations are strictly integer calculations. That means that if a float or decimal variable is ever produced it will be converted to an int.
 > Also divisions are always floor divisions!
 
-#### Use istrs as string
+#### Use istr as str
 
 We should realize that istrs are in fact strings.
 
 In order to concatenate two istrs (or an istr and a str), we cannot use the `+` operator (remember `four + five` is `istr('9')`).
 
 In order to concatenate istrs,  we use the or operator (`|`). So
 
@@ -157,15 +157,15 @@
 
 And
 ```
 (four | five) / 3
 ```
 is `istr('9')`.
 
-In order to repeat a string in the usual sense, you cannot use the `*` operator (remember `3 * four` is `istr(12)`. 
+In order to repeat a string in the usual sense, you cannot use the `*` operator (remember `3 * four` is `istr('12')`. 
 
 In order to repeat we use the matrix multiplication operator (`@`). So
 
  `3 @ four`
 
  is `istr('444')`
 
@@ -175,46 +175,46 @@
 
 is also `istr('444')`
 
 ##### Note
 
 >
 > It is not allowed to use the `@` operator for two istrs. So, `four @ five` raises a TypeError.
-#### istrs that can't be interpreted as an int
+#### istr that can't be interpreted as an int
 
 
-Although usualy, istrs are to be interpreted as an int, that's not a requirement.
+Although usualy istrs are to be interpreted as an int, that's not a requirement.
 
 So
 
 ```
 istr('abc')
 ```
 
 or
 
 ```
 istr('1,2,3')
 ```
 
-are accepted.
+are perfectly acceptable.
 
-But, we can't do any arithmetic with them. 
+But, we can't do any arithmetic or comparison with them. 
 
 If we try
 
 ```
 istr('abc') + 5
 ```
 
 a `TypeError` will be raised.
 
 That holds for any arithmetic we try.
 
-If we want to test if an istr can be interpreted (and thus used in an arithmetic expression). we can use the `is_int()` method. So
+If we want to test if an istr can be interpreted (and thus used in an arithmetic and comparison expression). we can use the `is_int()` method. So
 
 ```ìstr(20).is_int()```
 
 is `True`, whereas
 
 ```ìstr('abc').is_int()```
 
@@ -223,15 +223,15 @@
 
 
 The `bool` operator works normally on the integer value of an istr. So
 
 `bool(istr('0'))` ==> `False`
 `bool(istr('1'))` ==> `True`
 
-If the istr can't be interpreted as an int, the string value will be used to test. So
+But if the istr can't be interpreted as an int, the string value will be used to test. So
 
 `bool(istr('abc'))` ==> `True`
 `bool(istr(''))` ==> `False`
 
 #### Other operators
 
 For the `in` operator, an istr is treated as an ordinary string, although it is possible to use ints as well:
@@ -265,23 +265,36 @@
 ```
 
 is 
 
 ```
 '0 1 2 3 4 5 6 7 8 9 10 11'
 ```
-#### Using values that are neither string or numeric to initialize istr
+#### Using values that are neither string nor numeric to initialize istr
 
 Apart from with numeric (to be interpreted as an int) or str, istr can be initialized with
 several other types:
 
 
 - if a dict (or subtype of dict), the same type dict will be returned with all *values* istr'ed
+  ```
+  istr({'one': 1, 'two':2}) ==> {'one': istr('1'), 'two': istr('2')}
+  ```
 
 - if an iterator, the iterator will be mapped with istr
+  ```
+  mapped = (i for i in istr((i for i in range(2))))
+  print(mapped)
+  print(list(mapped))
+  ```
+  this wil print something like
+  ```
+  <generator object <genexpr> at 0x000002A10DE569B0>
+  [istr('0'), istr('1')]
+  ```
 
 - if an iterable, the same type will be returned with all elements istr'ed
 
 ```
     istr([0, 1, 4]) ==> [istr('0'), istr('1'), istr('4')]
     istr((0, 1, 4)) ==> (istr('0'), istr('1'), istr('4'))
     istr({0, 1, 4}) ==> `{istr('4'), istr('0'), istr('1')}  # or similar  
@@ -292,16 +305,20 @@
 ```
   istr(range(3)) ==> istr.range(3)
   list(istr(range(3))) ==> [istr('0'), istr('1'), istr('2')]
   len(istr(range(3))) ==> 3
 ```
 
 - if an istr.range instance, the same istr.range will be returned
+  ```
+  istr(istr.range(5)) ==> istr.range(5)
+  ```
+
 
-- if an istr, the same istr will be used
+- if an istr, the same istr will be returned
 
   ```
     istr(istr('4')) ==> istr ('4')
   ```
 
 #### More than one parameter for istr
 It is possible to give more than one parameter, in which case a tuple
@@ -332,35 +349,35 @@
 n100 = n98 + 2
 istr(n98).all_distinct() ==> True
 istr(n100).all_distinct() ==> False
 ```
 
 #### reverse an istr
 
-The method `istr.reversed()` will return an istr with the reversed content:
+The method `reversed()` will return an istr with the reversed content:
 ```
 istr(456).reversed() ==> istr('654')
 istr('0456').reversed() ==> istr('6540')
 ```
 The same can -of course- be achieved with
 ```
 istr(456)[::-1] ==> istr('654')
 istr('0456')[::-1] ==> istr('6540')
 ```
 ##### Note
 >
 > It is possible to reverse a negative istr, but the result can't be interpreted as an int anymore.
 >
 > ```
-> istr(-456).reversed() ==> TypeError
+> istr(-456).reversed() + 3 ==> TypeError
 > ```
 
 #### enumerate with istrs
 
-The `istr.enumerate` method can be used just as the builtin enumerate function.
+The `istr.enumerate` class method can be used just as the built-in enumerate function.
 The iteration counter however is an istr rather than an int. E.g. 
 
 ```
 for i, c in istr.enumerate('abc'):
     print(f'{repr(i)} {c}')
 ```
 prints
@@ -516,15 +533,15 @@
     print(repr(b))
 ```
 This will result in
 ```
 32767
 istr('7F')
 ```
-All calculations are done in the decimal 10 system.
+All calculations are done in the decimal 10 base system.
 
 Note that the way an `istr` is interpreted is determined at initialization.
 
 It is also possible to set the repr mode without a context manager:
 ```
 istr.base(16)
 print(int(istr('7fff')))
@@ -616,25 +633,26 @@
 <=, <, >, >=         x         istr('100') > istr('2') ==> True
 slicing                   x    istr(12345)[1:3] ==> istr('23')
 iterate                   x    [x for x in istr(20)] ==> [istr('2'), istr('0')
 len                       x    len(istr(' 20 ')) ==> 4
 count                     x    istr(100),count('0') ==> 2
 index                     x    istr(' 100 ').index('0') ==> 2
 split                     x    istr('1 2').split() ==> (istr('1'), istr('2'))
+string format             x    f"|{istr((1234):6}|" ==> '|1234  |'
 other string methods      x    istr('aAbBcC').lower() ==> istr('aabbcc')
                                istr('aAbBcC').islower() ==> False
                                istr('  abc   ').strip() ==> istr('abc')
 -----------------------------------------------------------------------------------------
 *) str is applied if is_int() is False
+
 ```
 ### Test script
 There's an extensive pytest script in the `\tests` directory.
 
 This script also shows clearly the ways istr can be used, including several edge cases. Highly recommended to have a look at.
 
 
 
 ### Badges
 ![PyPI](https://img.shields.io/pypi/v/istr-python) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/istr-python) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/istr-python)
-
 ![PyPI - License](https://img.shields.io/pypi/l/istr-python) ![Black](https://img.shields.io/badge/code%20style-black-000000.svg) 
 ![GitHub last commit](https://img.shields.io/github/last-commit/salabim/istr)
```

### Comparing `istr_python-1.0.2/istr_python.egg-info/PKG-INFO` & `istr_python-1.0.3/istr_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 1.0.2
+Version: 1.0.3
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
- <img src="https://www.salabim.org/istr_logo.png" width=500>
+ <img src="https://www.salabim.org/istr/istr_logo.png" width=500>
 
 ### Introduction
 
-With  `istr` is possible to interpret strings as if they were integers.
+The `istr` module makes it possible to use strings as if they were integers.
 
 This can be very handy for solving puzzles, but also for other purposes.
 For instance the famous send more money puzzle, where each letter has to be replaced by a unique digit (0-9)
 
 ```
   S E N D
   M O R E
@@ -65,15 +65,15 @@
 
 Just start with
 
 ```
 from istr import istr
 ```
 
-#### Use istrs as if the were int
+#### Use istr as int
 
 We can define an istr:
 ```
 four = istr('4')
 five = istr('5')
 ```
 The variables `four`  and `five` can now be used as if they were int:
@@ -122,22 +122,22 @@
 
 ```
 twenty == '20'
 ```
 
 is also True!
 
-For the order comparisons (<=, <, >, >=), the istr is always interpreted as an int:
+For the order comparisons (<=, <, >, >=), the istr is always interpreted as an int.
 
-That means that  both
+That means that  
 ```
 twenty < 30
-twenty >= '10' # here '10' is converted to 10 for the comparison
+twenty >= '10' # here '10' is converted to the integer 10 for the comparison
 ```
-are `True`.
+are both`True`.
 
 In contrast to an ordinary string
 ```
 print(four + five)
 ```
 prints `9`, as istr are treated as ints (if possible).
 
@@ -151,15 +151,15 @@
 ```
 
 ##### Important
 >
 > All calculations are strictly integer calculations. That means that if a float or decimal variable is ever produced it will be converted to an int.
 > Also divisions are always floor divisions!
 
-#### Use istrs as string
+#### Use istr as str
 
 We should realize that istrs are in fact strings.
 
 In order to concatenate two istrs (or an istr and a str), we cannot use the `+` operator (remember `four + five` is `istr('9')`).
 
 In order to concatenate istrs,  we use the or operator (`|`). So
 
@@ -170,15 +170,15 @@
 
 And
 ```
 (four | five) / 3
 ```
 is `istr('9')`.
 
-In order to repeat a string in the usual sense, you cannot use the `*` operator (remember `3 * four` is `istr(12)`. 
+In order to repeat a string in the usual sense, you cannot use the `*` operator (remember `3 * four` is `istr('12')`. 
 
 In order to repeat we use the matrix multiplication operator (`@`). So
 
  `3 @ four`
 
  is `istr('444')`
 
@@ -188,46 +188,46 @@
 
 is also `istr('444')`
 
 ##### Note
 
 >
 > It is not allowed to use the `@` operator for two istrs. So, `four @ five` raises a TypeError.
-#### istrs that can't be interpreted as an int
+#### istr that can't be interpreted as an int
 
 
-Although usualy, istrs are to be interpreted as an int, that's not a requirement.
+Although usualy istrs are to be interpreted as an int, that's not a requirement.
 
 So
 
 ```
 istr('abc')
 ```
 
 or
 
 ```
 istr('1,2,3')
 ```
 
-are accepted.
+are perfectly acceptable.
 
-But, we can't do any arithmetic with them. 
+But, we can't do any arithmetic or comparison with them. 
 
 If we try
 
 ```
 istr('abc') + 5
 ```
 
 a `TypeError` will be raised.
 
 That holds for any arithmetic we try.
 
-If we want to test if an istr can be interpreted (and thus used in an arithmetic expression). we can use the `is_int()` method. So
+If we want to test if an istr can be interpreted (and thus used in an arithmetic and comparison expression). we can use the `is_int()` method. So
 
 ```ìstr(20).is_int()```
 
 is `True`, whereas
 
 ```ìstr('abc').is_int()```
 
@@ -236,15 +236,15 @@
 
 
 The `bool` operator works normally on the integer value of an istr. So
 
 `bool(istr('0'))` ==> `False`
 `bool(istr('1'))` ==> `True`
 
-If the istr can't be interpreted as an int, the string value will be used to test. So
+But if the istr can't be interpreted as an int, the string value will be used to test. So
 
 `bool(istr('abc'))` ==> `True`
 `bool(istr(''))` ==> `False`
 
 #### Other operators
 
 For the `in` operator, an istr is treated as an ordinary string, although it is possible to use ints as well:
@@ -278,23 +278,36 @@
 ```
 
 is 
 
 ```
 '0 1 2 3 4 5 6 7 8 9 10 11'
 ```
-#### Using values that are neither string or numeric to initialize istr
+#### Using values that are neither string nor numeric to initialize istr
 
 Apart from with numeric (to be interpreted as an int) or str, istr can be initialized with
 several other types:
 
 
 - if a dict (or subtype of dict), the same type dict will be returned with all *values* istr'ed
+  ```
+  istr({'one': 1, 'two':2}) ==> {'one': istr('1'), 'two': istr('2')}
+  ```
 
 - if an iterator, the iterator will be mapped with istr
+  ```
+  mapped = (i for i in istr((i for i in range(2))))
+  print(mapped)
+  print(list(mapped))
+  ```
+  this wil print something like
+  ```
+  <generator object <genexpr> at 0x000002A10DE569B0>
+  [istr('0'), istr('1')]
+  ```
 
 - if an iterable, the same type will be returned with all elements istr'ed
 
 ```
     istr([0, 1, 4]) ==> [istr('0'), istr('1'), istr('4')]
     istr((0, 1, 4)) ==> (istr('0'), istr('1'), istr('4'))
     istr({0, 1, 4}) ==> `{istr('4'), istr('0'), istr('1')}  # or similar  
@@ -305,16 +318,20 @@
 ```
   istr(range(3)) ==> istr.range(3)
   list(istr(range(3))) ==> [istr('0'), istr('1'), istr('2')]
   len(istr(range(3))) ==> 3
 ```
 
 - if an istr.range instance, the same istr.range will be returned
+  ```
+  istr(istr.range(5)) ==> istr.range(5)
+  ```
+
 
-- if an istr, the same istr will be used
+- if an istr, the same istr will be returned
 
   ```
     istr(istr('4')) ==> istr ('4')
   ```
 
 #### More than one parameter for istr
 It is possible to give more than one parameter, in which case a tuple
@@ -345,35 +362,35 @@
 n100 = n98 + 2
 istr(n98).all_distinct() ==> True
 istr(n100).all_distinct() ==> False
 ```
 
 #### reverse an istr
 
-The method `istr.reversed()` will return an istr with the reversed content:
+The method `reversed()` will return an istr with the reversed content:
 ```
 istr(456).reversed() ==> istr('654')
 istr('0456').reversed() ==> istr('6540')
 ```
 The same can -of course- be achieved with
 ```
 istr(456)[::-1] ==> istr('654')
 istr('0456')[::-1] ==> istr('6540')
 ```
 ##### Note
 >
 > It is possible to reverse a negative istr, but the result can't be interpreted as an int anymore.
 >
 > ```
-> istr(-456).reversed() ==> TypeError
+> istr(-456).reversed() + 3 ==> TypeError
 > ```
 
 #### enumerate with istrs
 
-The `istr.enumerate` method can be used just as the builtin enumerate function.
+The `istr.enumerate` class method can be used just as the built-in enumerate function.
 The iteration counter however is an istr rather than an int. E.g. 
 
 ```
 for i, c in istr.enumerate('abc'):
     print(f'{repr(i)} {c}')
 ```
 prints
@@ -529,15 +546,15 @@
     print(repr(b))
 ```
 This will result in
 ```
 32767
 istr('7F')
 ```
-All calculations are done in the decimal 10 system.
+All calculations are done in the decimal 10 base system.
 
 Note that the way an `istr` is interpreted is determined at initialization.
 
 It is also possible to set the repr mode without a context manager:
 ```
 istr.base(16)
 print(int(istr('7fff')))
@@ -629,25 +646,26 @@
 <=, <, >, >=         x         istr('100') > istr('2') ==> True
 slicing                   x    istr(12345)[1:3] ==> istr('23')
 iterate                   x    [x for x in istr(20)] ==> [istr('2'), istr('0')
 len                       x    len(istr(' 20 ')) ==> 4
 count                     x    istr(100),count('0') ==> 2
 index                     x    istr(' 100 ').index('0') ==> 2
 split                     x    istr('1 2').split() ==> (istr('1'), istr('2'))
+string format             x    f"|{istr((1234):6}|" ==> '|1234  |'
 other string methods      x    istr('aAbBcC').lower() ==> istr('aabbcc')
                                istr('aAbBcC').islower() ==> False
                                istr('  abc   ').strip() ==> istr('abc')
 -----------------------------------------------------------------------------------------
 *) str is applied if is_int() is False
+
 ```
 ### Test script
 There's an extensive pytest script in the `\tests` directory.
 
 This script also shows clearly the ways istr can be used, including several edge cases. Highly recommended to have a look at.
 
 
 
 ### Badges
 ![PyPI](https://img.shields.io/pypi/v/istr-python) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/istr-python) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/istr-python)
-
 ![PyPI - License](https://img.shields.io/pypi/l/istr-python) ![Black](https://img.shields.io/badge/code%20style-black-000000.svg) 
 ![GitHub last commit](https://img.shields.io/github/last-commit/salabim/istr)
```

### Comparing `istr_python-1.0.2/pyproject.toml` & `istr_python-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "istr-python"
 authors = [
     {name = "Ruud van der Ham", email = "rt.van.der.ham@gmail.com"}
 ]
 description = "istr - strings you can count on"
-version = "1.0.2"
+version = "1.0.3"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
@@ -22,8 +22,9 @@
 Homepage = "https://github.com/salabim/istr"
 Repository = "https://github.com/salabim/istr"
 
 [tool.setuptools]
 packages = ["istr"]
 
 [tool.setuptools.package-data]
-"*" = ["*.md"]
+"*" = ["*.txt"]
+
```

### Comparing `istr_python-1.0.2/tests/test_istr.py` & `istr_python-1.0.3/tests/test_istr.py`

 * *Files 6% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         assert istr("") == ""
 
 
 def test_divmod():
     assert divmod(eleven, three) == (istr(3), istr(2))
     assert divmod(11, three) == (istr(3), istr(2))
     assert divmod(eleven, 3) == (istr(3), istr(2))
-    assert divmod(11, 3) == (3, 2)
+    assert divmod(11, 3) == (3, 2)  # just for reference
 
 
 def test_iter():
     assert [x for x in istr.range(3)] == [istr(0), istr(1), istr(2)]
 
 
 def test_reversed():
@@ -282,17 +282,14 @@
     istr.int_format("03")
     assert istr.int_format() == "03"
     assert istr("  8 ") == "  8 "
     istr.int_format("")
     assert istr(" 8 ") == " 8 "
 
 
-#    assert repr(istr('a')) == "istr('a')"
-
-
 def test_range_int_format():
     r = istr.range(11)
     assert repr(r) == "istr.range(0, 11)"
     assert " ".join(r) == "0 1 2 3 4 5 6 7 8 9 10"
     r = istr.range(11)
     with istr.int_format("02"):
         assert " ".join(r) == "00 01 02 03 04 05 06 07 08 09 10"
@@ -323,14 +320,26 @@
 
     s = istr("").join(istr(("", "", "6")))
     assert s == "6"
     assert s == 6
     assert type(s) == istr
 
 
+def test_or():
+    assert (eleven | twelve).equals(istr("1112"))
+    assert ("11" | twelve).equals(istr("1112"))
+    assert (eleven | "12").equals(istr("1112"))
+    with pytest.raises(TypeError):
+        11 | twelve
+    with pytest.raises(TypeError, match=re.escape("unsupported operand type(s) for |: 11 and istr('12')")):
+        11 | twelve
+    with pytest.raises(TypeError, match=re.escape("unsupported operand type(s) for |: istr('11') and 12")):
+        eleven | 12
+
+
 def test_matmul():
     assert (five @ 3).equals(istr("555"))
     assert (3 @ five).equals(istr("555"))
 
     with pytest.raises(TypeError):
         three @ five
     with pytest.raises(TypeError):
@@ -365,17 +374,17 @@
         math.ceil(istr("a"))
     with pytest.raises(TypeError, match=re.escape(f"unsupported operand for abs: istr('a')")):
         abs(istr("a"))
     with pytest.raises(TypeError, match=re.escape(f"unsupported operand for +: istr('a')")):
         +istr("a")
     with pytest.raises(TypeError, match=re.escape(f"unsupported operand for -: istr('a')")):
         -istr("a")
-    with pytest.raises(TypeError, match=re.escape(f"unsupported operand for is_odd: istr('a')")):
+    with pytest.raises(TypeError):
         istr("a").is_odd()
-    with pytest.raises(TypeError, match=re.escape(f"unsupported operand for is_even: istr('a')")):
+    with pytest.raises(TypeError):
         istr("a").is_even()
     assert istr(1).is_int()
     assert not istr("a").is_int()
 
     with pytest.raises(TypeError, match=f"istr"):
         istr("a") + 1
     with pytest.raises(TypeError, match=f"istr"):
@@ -384,14 +393,17 @@
     with pytest.raises(TypeError, match=f"istr"):
         with istr.repr_mode("str"):  # error message should not use the standard repr
             istr("a") + 1
 
 
 def test_str():
     assert repr(str(five)) == "'5'"
+    assert f"|{istr(1234):6}|" == "|1234  |"
+    with pytest.raises(ValueError):
+        f"{istr(1234):d}"
 
 
 def test_bool():
     assert bool(istr(0)) is False
     assert bool(istr(1)) is True
     assert bool(istr("0")) is False
     assert bool(istr("a")) is True
@@ -402,39 +414,39 @@
     assert math.trunc(one).equals(istr("1"))
     assert math.ceil(one).equals(istr("1"))
     assert math.floor(one).equals(istr("1"))
     assert round(one).equals(istr("1"))
 
 
 def test_data_structures():
-    assert repr(istr(list(range(1, 4)))) == "[istr('1'), istr('2'), istr('3')]"
-    assert repr(istr(tuple(range(1, 4)))) == "(istr('1'), istr('2'), istr('3'))"
+    assert istr(list(range(1, 4))) == [istr("1"), istr("2"), istr("3")]
+    assert istr(tuple(range(1, 4))) == (istr("1"), istr("2"), istr("3"))
     assert istr(set(range(1, 4))) == {istr(1), istr(2), istr(3)}
 
-    assert repr(list(istr(range(1, 4)))) == "[istr('1'), istr('2'), istr('3')]"
+    assert list(istr(range(1, 4))) == [istr("1"), istr("2"), istr("3")]
 
-    assert repr(list(istr.enumerate("abc"))) == "[(istr('0'), 'a'), (istr('1'), 'b'), (istr('2'), 'c')]"
-    assert repr(list(istr.enumerate("abc", 1))) == "[(istr('1'), 'a'), (istr('2'), 'b'), (istr('3'), 'c')]"
+    assert list(istr.enumerate("abc")) == [(istr("0"), "a"), (istr("1"), "b"), (istr("2"), "c")]
+    assert list(istr.enumerate("abc", 1)) == [(istr("1"), "a"), (istr("2"), "b"), (istr("3"), "c")]
 
-    assert repr(istr(dict(zero=0, one=1, two=4))) == "{'zero': istr('0'), 'one': istr('1'), 'two': istr('4')}"
+    assert istr(dict(zero=0, one=1, two=4)) == {"zero": istr("0"), "one": istr("1"), "two": istr("4")}
 
 
 def test_indexing():
     a = istr(12345)
     assert a[0].equals(istr(1))
     assert a[:2].equals(istr(12))
     assert a[::-1].equals(istr(54321))
     assert a[-2:].equals(istr(45))
 
 
 def test_reverse():
     a = istr(12345)
-    assert a.reversed(), same(istr(54321))
-    a = istr(-120)
-    assert a.reversed(), same(istr("-210"))
+    assert a.reversed().equals(istr(54321))
+    a = istr(-123)
+    assert a.reversed().equals(istr("321-"))
 
 
 def test_edge_cases():
     with pytest.raises(TypeError):
         istr(istr)
     assert istr(istr(one)).equals(istr("1"))
     with pytest.raises(TypeError):
@@ -466,16 +478,16 @@
     with istr.repr_mode("str"):
         hundred = istr(100)
     assert repr(hundred) == "'100'"
     hundred = istr(100)
     assert repr(hundred) == "istr('100')"
 
     with istr.repr_mode("int"):
-        a = istr("a")
-    assert repr(a) == "nan"
+        a = istr("abc")
+    assert repr(a) == "?"
 
     assert istr.repr_mode() == "istr"
 
     with pytest.raises(TypeError):
         istr.repr_mode("no")
 
 
@@ -544,35 +556,37 @@
     assert istr.digits().equals(istr("0123456789"))
     assert istr.digits("").equals(istr("0123456789"))
     assert istr.digits("1").equals(istr("1"))
     assert istr.digits("3-").equals(istr("3456789"))
     assert istr.digits("-3").equals(istr("0123"))
     assert istr.digits("1-4", "6", "8-9").equals(istr("1234689"))
     assert istr.digits("1", "1-2", "1-3").equals(istr("112123"))
-    a= istr.digits("a")
+    a = istr.digits("a")
     assert a.equals(istr("A"))
     assert not a.is_int()
-    with istr.base(36): 
-        a=istr.digits("a")
+    with istr.base(36):
+        a = istr.digits("a")
         assert a == 10
-        assert a =="A"
+        assert a == "A"
         assert istr.digits("-a").equals(istr("0123456789A"))
         assert istr.digits("x-").equals(istr("XYZ"))
         assert istr.digits("B-d").equals(istr("BCD"))
         assert istr.digits("-").equals(istr("0123456789"))
     with istr.base(16):
         ef = istr.digits("e-f")
-        assert (ef+1).equals(istr("F0"))
+        assert (ef + 1).equals(istr("F0"))
         assert ef == 239
 
+
 def test_all_distinct():
     assert istr("abcdef").all_distinct()
     assert not istr("aabcdef").all_distinct()
     assert istr("").all_distinct()
 
+
 def test_subclassing():
     class jstr(istr):
         ...
 
     assert jstr(5).equals(jstr(5))
     assert repr(jstr(*range(3))) == "(jstr('0'), jstr('1'), jstr('2'))"
```


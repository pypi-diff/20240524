# Comparing `tmp/PyKCS11-1.5.8.tar.gz` & `tmp/PyKCS11-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyKCS11-1.5.8.tar", last modified: Fri May 15 13:51:30 2020, max compression
+gzip compressed data, was "dist/PyKCS11-1.5.9.tar", last modified: Fri Jul 31 13:34:14 2020, max compression
```

## Comparing `PyKCS11-1.5.8.tar` & `PyKCS11-1.5.9.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2020-05-15 13:51:30.000000 PyKCS11-1.5.8/
--rw-r--r--   0 rousseau   (501) staff       (20)    17987 2019-01-22 20:49:24.000000 PyKCS11-1.5.8/COPYING
--rw-r--r--   0 rousseau   (501) staff       (20)     7589 2020-05-15 13:33:12.000000 PyKCS11-1.5.8/Changes.txt
--rw-r--r--   0 rousseau   (501) staff       (20)      238 2020-05-04 15:34:43.000000 PyKCS11-1.5.8/MANIFEST.in
--rw-r--r--   0 rousseau   (501) staff       (20)     1223 2020-03-30 07:07:51.000000 PyKCS11-1.5.8/Makefile
--rw-r--r--   0 rousseau   (501) staff       (20)      505 2019-01-22 20:49:24.000000 PyKCS11-1.5.8/Makefile.win32
--rw-r--r--   0 rousseau   (501) staff       (20)     1374 2020-05-15 13:51:30.000000 PyKCS11-1.5.8/PKG-INFO
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2020-05-15 13:51:30.000000 PyKCS11-1.5.8/PyKCS11/
--rw-r--r--   0 rousseau   (501) staff       (20)    53170 2020-05-15 13:32:01.000000 PyKCS11-1.5.8/PyKCS11/__init__.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2020-05-15 13:51:30.000000 PyKCS11-1.5.8/PyKCS11.egg-info/
--rw-r--r--   0 rousseau   (501) staff       (20)     1374 2020-05-15 13:51:30.000000 PyKCS11-1.5.8/PyKCS11.egg-info/PKG-INFO
--rw-r--r--   0 rousseau   (501) staff       (20)     1490 2020-05-15 13:51:30.000000 PyKCS11-1.5.8/PyKCS11.egg-info/SOURCES.txt
--rw-r--r--   0 rousseau   (501) staff       (20)        1 2020-05-15 13:51:30.000000 PyKCS11-1.5.8/PyKCS11.egg-info/dependency_links.txt
--rw-r--r--   0 rousseau   (501) staff       (20)        8 2020-05-15 13:51:30.000000 PyKCS11-1.5.8/PyKCS11.egg-info/top_level.txt
--rw-r--r--   0 rousseau   (501) staff       (20)     2188 2019-01-22 20:57:15.000000 PyKCS11-1.5.8/README.md
--rw-r--r--   0 rousseau   (501) staff       (20)       30 2019-04-17 13:45:32.000000 PyKCS11-1.5.8/dev-requirements.txt
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2020-05-15 13:51:30.000000 PyKCS11-1.5.8/docs/
--rw-r--r--   0 rousseau   (501) staff       (20)      604 2019-01-22 20:57:15.000000 PyKCS11-1.5.8/docs/Makefile
--rw-r--r--   0 rousseau   (501) staff       (20)       94 2019-01-22 20:57:15.000000 PyKCS11-1.5.8/docs/api.rst
--rw-r--r--   0 rousseau   (501) staff       (20)     5182 2019-01-22 20:57:15.000000 PyKCS11-1.5.8/docs/conf.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)      254 2019-01-22 20:57:15.000000 PyKCS11-1.5.8/docs/generate.sh
--rw-r--r--   0 rousseau   (501) staff       (20)      910 2019-01-22 20:57:15.000000 PyKCS11-1.5.8/docs/index.rst
--rw-r--r--   0 rousseau   (501) staff       (20)      725 2019-01-22 20:57:15.000000 PyKCS11-1.5.8/docs/license.rst
--rw-r--r--   0 rousseau   (501) staff       (20)      735 2019-01-22 20:57:15.000000 PyKCS11-1.5.8/docs/samples.rst
--rw-r--r--   0 rousseau   (501) staff       (20)     2801 2019-01-22 20:49:24.000000 PyKCS11-1.5.8/pykcs11.rc
--rw-r--r--   0 rousseau   (501) staff       (20)      401 2019-01-22 20:49:24.000000 PyKCS11-1.5.8/resource.h
--rwxr-xr-x   0 rousseau   (501) staff       (20)     1484 2020-02-09 20:22:18.000000 PyKCS11-1.5.8/run_test.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2020-05-15 13:51:30.000000 PyKCS11-1.5.8/samples/
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2020-05-15 13:51:30.000000 PyKCS11-1.5.8/samples/LowLevel/
--rwxr-xr-x   0 rousseau   (501) staff       (20)     3997 2019-01-22 20:57:15.000000 PyKCS11-1.5.8/samples/LowLevel/InitTokenPin.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     6173 2019-01-22 20:57:15.000000 PyKCS11-1.5.8/samples/LowLevel/dumpit.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     2082 2019-01-22 20:57:15.000000 PyKCS11-1.5.8/samples/LowLevel/rand.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     4619 2019-01-22 20:57:15.000000 PyKCS11-1.5.8/samples/LowLevel/test.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     4806 2019-01-22 20:57:15.000000 PyKCS11-1.5.8/samples/LowLevel/test1.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     1296 2019-01-22 20:49:24.000000 PyKCS11-1.5.8/samples/destroy_by_ID.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)    11887 2019-01-22 20:57:15.000000 PyKCS11-1.5.8/samples/dumpit.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     2337 2019-04-17 13:45:32.000000 PyKCS11-1.5.8/samples/ec_generate.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     1923 2019-04-17 13:45:32.000000 PyKCS11-1.5.8/samples/ec_signature.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     1611 2019-01-22 20:49:24.000000 PyKCS11-1.5.8/samples/encrypt.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     2794 2019-05-15 07:03:16.000000 PyKCS11-1.5.8/samples/events.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     1826 2019-01-22 20:57:15.000000 PyKCS11-1.5.8/samples/generate.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     4896 2019-01-22 20:57:15.000000 PyKCS11-1.5.8/samples/genkeypair_import_cert.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     5216 2019-01-22 20:57:15.000000 PyKCS11-1.5.8/samples/getinfo.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     1467 2019-01-22 20:49:24.000000 PyKCS11-1.5.8/samples/modulus.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     2023 2019-01-22 20:57:15.000000 PyKCS11-1.5.8/samples/rsa_encrypt.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     1769 2019-01-22 20:57:15.000000 PyKCS11-1.5.8/samples/signature.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     1125 2019-01-22 20:49:24.000000 PyKCS11-1.5.8/samples/unblock.py
--rw-r--r--   0 rousseau   (501) staff       (20)       38 2020-05-15 13:51:30.000000 PyKCS11-1.5.8/setup.cfg
--rwxr-xr-x   0 rousseau   (501) staff       (20)     3337 2020-05-15 13:30:56.000000 PyKCS11-1.5.8/setup.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2020-05-15 13:51:30.000000 PyKCS11-1.5.8/src/
--rw-r--r--   0 rousseau   (501) staff       (20)     8196 2020-05-15 13:39:51.000000 PyKCS11-1.5.8/src/.DS_Store
--rw-r--r--   0 rousseau   (501) staff       (20)    78160 2020-05-15 13:51:21.000000 PyKCS11-1.5.8/src/LowLevel.py
--rw-r--r--   0 rousseau   (501) staff       (20)     5800 2020-05-04 15:34:43.000000 PyKCS11-1.5.8/src/ck_attribute_smart.cpp
--rw-r--r--   0 rousseau   (501) staff       (20)     1985 2019-04-17 14:59:52.000000 PyKCS11-1.5.8/src/ck_attribute_smart.h
--rw-r--r--   0 rousseau   (501) staff       (20)     2208 2019-01-22 20:57:15.000000 PyKCS11-1.5.8/src/dyn_generic.h
--rw-r--r--   0 rousseau   (501) staff       (20)     1815 2019-01-22 20:49:24.000000 PyKCS11-1.5.8/src/dyn_unix.c
--rw-r--r--   0 rousseau   (501) staff       (20)     2081 2019-01-22 20:57:15.000000 PyKCS11-1.5.8/src/dyn_win32.c
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2020-05-15 13:51:30.000000 PyKCS11-1.5.8/src/opensc/
--rw-r--r--   0 rousseau   (501) staff       (20)     6148 2020-05-15 12:44:34.000000 PyKCS11-1.5.8/src/opensc/.DS_Store
--rw-r--r--   0 rousseau   (501) staff       (20)    43553 2020-05-14 15:35:18.000000 PyKCS11-1.5.8/src/opensc/pkcs11.h
--rw-r--r--   0 rousseau   (501) staff       (20)    24503 2019-10-06 20:08:47.000000 PyKCS11-1.5.8/src/pkcs11lib.cpp
--rw-r--r--   0 rousseau   (501) staff       (20)     7053 2019-10-06 20:08:47.000000 PyKCS11-1.5.8/src/pkcs11lib.h
--rw-r--r--   0 rousseau   (501) staff       (20)     1097 2019-01-22 20:49:24.000000 PyKCS11-1.5.8/src/pykcs11.cpp
--rw-r--r--   0 rousseau   (501) staff       (20)      795 2019-01-22 20:49:24.000000 PyKCS11-1.5.8/src/pykcs11.h
--rw-r--r--   0 rousseau   (501) staff       (20)    49449 2020-05-15 13:29:10.000000 PyKCS11-1.5.8/src/pykcs11.i
--rw-r--r--   0 rousseau   (501) staff       (20)     1423 2019-01-22 20:49:24.000000 PyKCS11-1.5.8/src/pykcs11string.cpp
--rw-r--r--   0 rousseau   (501) staff       (20)     1111 2019-01-22 20:49:24.000000 PyKCS11-1.5.8/src/pykcs11string.h
--rw-r--r--   0 rousseau   (501) staff       (20)     1066 2019-01-22 20:49:24.000000 PyKCS11-1.5.8/src/stdafx.cpp
--rw-r--r--   0 rousseau   (501) staff       (20)     1294 2019-01-22 20:49:24.000000 PyKCS11-1.5.8/src/stdafx.h
--rw-r--r--   0 rousseau   (501) staff       (20)     2428 2019-01-22 20:49:24.000000 PyKCS11-1.5.8/src/utility.cpp
--rw-r--r--   0 rousseau   (501) staff       (20)     1301 2019-01-22 20:49:24.000000 PyKCS11-1.5.8/src/utility.h
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2020-05-15 13:51:30.000000 PyKCS11-1.5.8/test/
--rw-r--r--   0 rousseau   (501) staff       (20)      560 2019-04-17 13:45:32.000000 PyKCS11-1.5.8/test/test_CK.py
--rw-r--r--   0 rousseau   (501) staff       (20)     4784 2019-10-06 20:11:49.000000 PyKCS11-1.5.8/test/test_LowLevel.py
--rw-r--r--   0 rousseau   (501) staff       (20)     6353 2020-05-04 15:34:43.000000 PyKCS11-1.5.8/test/test_asymetric.py
--rw-r--r--   0 rousseau   (501) staff       (20)     3323 2019-04-17 13:45:32.000000 PyKCS11-1.5.8/test/test_asymetric_ECC.py
--rw-r--r--   0 rousseau   (501) staff       (20)     2938 2019-04-17 13:45:32.000000 PyKCS11-1.5.8/test/test_asymetric_gost.py
--rw-r--r--   0 rousseau   (501) staff       (20)     2446 2019-10-06 20:09:11.000000 PyKCS11-1.5.8/test/test_ckbytelist.py
--rw-r--r--   0 rousseau   (501) staff       (20)     1062 2019-04-17 13:45:32.000000 PyKCS11-1.5.8/test/test_digest.py
--rw-r--r--   0 rousseau   (501) staff       (20)     1424 2019-04-17 13:45:32.000000 PyKCS11-1.5.8/test/test_exception.py
--rw-r--r--   0 rousseau   (501) staff       (20)     1676 2019-04-17 13:45:32.000000 PyKCS11-1.5.8/test/test_info.py
--rw-r--r--   0 rousseau   (501) staff       (20)     2675 2019-04-17 13:45:32.000000 PyKCS11-1.5.8/test/test_init.py
--rw-r--r--   0 rousseau   (501) staff       (20)     1292 2019-10-06 20:09:11.000000 PyKCS11-1.5.8/test/test_load.py
--rw-r--r--   0 rousseau   (501) staff       (20)     2623 2019-04-17 13:45:32.000000 PyKCS11-1.5.8/test/test_objects.py
--rw-r--r--   0 rousseau   (501) staff       (20)     1833 2019-10-06 20:09:11.000000 PyKCS11-1.5.8/test/test_pin.py
--rw-r--r--   0 rousseau   (501) staff       (20)      724 2019-04-17 13:45:32.000000 PyKCS11-1.5.8/test/test_random.py
--rw-r--r--   0 rousseau   (501) staff       (20)     4026 2020-05-04 15:34:43.000000 PyKCS11-1.5.8/test/test_symetric.py
--rw-r--r--   0 rousseau   (501) staff       (20)    11767 2020-05-04 15:34:43.000000 PyKCS11-1.5.8/test/test_wrap.py
--rw-r--r--   0 rousseau   (501) staff       (20)      488 2020-05-15 13:50:46.000000 PyKCS11-1.5.8/tox.ini
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2020-07-31 13:34:14.589751 PyKCS11-1.5.9/
+-rw-r--r--   0 rousseau   (501) staff       (20)    17987 2019-01-22 20:49:24.000000 PyKCS11-1.5.9/COPYING
+-rw-r--r--   0 rousseau   (501) staff       (20)     7751 2020-07-31 13:31:10.000000 PyKCS11-1.5.9/Changes.txt
+-rw-r--r--   0 rousseau   (501) staff       (20)      238 2020-05-04 15:34:43.000000 PyKCS11-1.5.9/MANIFEST.in
+-rw-r--r--   0 rousseau   (501) staff       (20)     1223 2020-03-30 07:07:51.000000 PyKCS11-1.5.9/Makefile
+-rw-r--r--   0 rousseau   (501) staff       (20)      505 2019-01-22 20:49:24.000000 PyKCS11-1.5.9/Makefile.win32
+-rw-r--r--   0 rousseau   (501) staff       (20)     1374 2020-07-31 13:34:14.589525 PyKCS11-1.5.9/PKG-INFO
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2020-07-31 13:34:14.575007 PyKCS11-1.5.9/PyKCS11/
+-rw-r--r--   0 rousseau   (501) staff       (20)    53170 2020-05-15 13:32:01.000000 PyKCS11-1.5.9/PyKCS11/__init__.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2020-07-31 13:34:14.575936 PyKCS11-1.5.9/PyKCS11.egg-info/
+-rw-r--r--   0 rousseau   (501) staff       (20)     1374 2020-07-31 13:34:14.000000 PyKCS11-1.5.9/PyKCS11.egg-info/PKG-INFO
+-rw-r--r--   0 rousseau   (501) staff       (20)     1490 2020-07-31 13:34:14.000000 PyKCS11-1.5.9/PyKCS11.egg-info/SOURCES.txt
+-rw-r--r--   0 rousseau   (501) staff       (20)        1 2020-07-31 13:34:14.000000 PyKCS11-1.5.9/PyKCS11.egg-info/dependency_links.txt
+-rw-r--r--   0 rousseau   (501) staff       (20)        8 2020-07-31 13:34:14.000000 PyKCS11-1.5.9/PyKCS11.egg-info/top_level.txt
+-rw-r--r--   0 rousseau   (501) staff       (20)     2188 2019-01-22 20:57:15.000000 PyKCS11-1.5.9/README.md
+-rw-r--r--   0 rousseau   (501) staff       (20)       30 2019-04-17 13:45:32.000000 PyKCS11-1.5.9/dev-requirements.txt
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2020-07-31 13:34:14.577523 PyKCS11-1.5.9/docs/
+-rw-r--r--   0 rousseau   (501) staff       (20)      604 2019-01-22 20:57:15.000000 PyKCS11-1.5.9/docs/Makefile
+-rw-r--r--   0 rousseau   (501) staff       (20)       94 2019-01-22 20:57:15.000000 PyKCS11-1.5.9/docs/api.rst
+-rw-r--r--   0 rousseau   (501) staff       (20)     5182 2019-01-22 20:57:15.000000 PyKCS11-1.5.9/docs/conf.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)      254 2019-01-22 20:57:15.000000 PyKCS11-1.5.9/docs/generate.sh
+-rw-r--r--   0 rousseau   (501) staff       (20)      910 2019-01-22 20:57:15.000000 PyKCS11-1.5.9/docs/index.rst
+-rw-r--r--   0 rousseau   (501) staff       (20)      725 2019-01-22 20:57:15.000000 PyKCS11-1.5.9/docs/license.rst
+-rw-r--r--   0 rousseau   (501) staff       (20)      735 2019-01-22 20:57:15.000000 PyKCS11-1.5.9/docs/samples.rst
+-rw-r--r--   0 rousseau   (501) staff       (20)     2801 2019-01-22 20:49:24.000000 PyKCS11-1.5.9/pykcs11.rc
+-rw-r--r--   0 rousseau   (501) staff       (20)      401 2019-01-22 20:49:24.000000 PyKCS11-1.5.9/resource.h
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     1484 2020-02-09 20:22:18.000000 PyKCS11-1.5.9/run_test.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2020-07-31 13:34:14.580306 PyKCS11-1.5.9/samples/
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2020-07-31 13:34:14.581388 PyKCS11-1.5.9/samples/LowLevel/
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     3997 2019-01-22 20:57:15.000000 PyKCS11-1.5.9/samples/LowLevel/InitTokenPin.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     6173 2019-01-22 20:57:15.000000 PyKCS11-1.5.9/samples/LowLevel/dumpit.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     2082 2019-01-22 20:57:15.000000 PyKCS11-1.5.9/samples/LowLevel/rand.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     4619 2019-01-22 20:57:15.000000 PyKCS11-1.5.9/samples/LowLevel/test.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     4806 2019-01-22 20:57:15.000000 PyKCS11-1.5.9/samples/LowLevel/test1.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     1296 2019-01-22 20:49:24.000000 PyKCS11-1.5.9/samples/destroy_by_ID.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)    11887 2019-01-22 20:57:15.000000 PyKCS11-1.5.9/samples/dumpit.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     2337 2019-04-17 13:45:32.000000 PyKCS11-1.5.9/samples/ec_generate.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     1923 2019-04-17 13:45:32.000000 PyKCS11-1.5.9/samples/ec_signature.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     1611 2019-01-22 20:49:24.000000 PyKCS11-1.5.9/samples/encrypt.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     2794 2019-05-15 07:03:16.000000 PyKCS11-1.5.9/samples/events.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     1826 2019-01-22 20:57:15.000000 PyKCS11-1.5.9/samples/generate.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     4896 2019-01-22 20:57:15.000000 PyKCS11-1.5.9/samples/genkeypair_import_cert.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     5216 2019-01-22 20:57:15.000000 PyKCS11-1.5.9/samples/getinfo.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     1467 2019-01-22 20:49:24.000000 PyKCS11-1.5.9/samples/modulus.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     2023 2019-01-22 20:57:15.000000 PyKCS11-1.5.9/samples/rsa_encrypt.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     1769 2019-01-22 20:57:15.000000 PyKCS11-1.5.9/samples/signature.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     1125 2019-01-22 20:49:24.000000 PyKCS11-1.5.9/samples/unblock.py
+-rw-r--r--   0 rousseau   (501) staff       (20)       38 2020-07-31 13:34:14.589815 PyKCS11-1.5.9/setup.cfg
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     3337 2020-07-31 13:31:10.000000 PyKCS11-1.5.9/setup.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2020-07-31 13:34:14.585501 PyKCS11-1.5.9/src/
+-rw-r--r--   0 rousseau   (501) staff       (20)     8196 2020-05-20 11:41:31.000000 PyKCS11-1.5.9/src/.DS_Store
+-rw-r--r--   0 rousseau   (501) staff       (20)    78160 2020-07-31 13:33:52.000000 PyKCS11-1.5.9/src/LowLevel.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     5800 2020-05-04 15:34:43.000000 PyKCS11-1.5.9/src/ck_attribute_smart.cpp
+-rw-r--r--   0 rousseau   (501) staff       (20)     1985 2019-04-17 14:59:52.000000 PyKCS11-1.5.9/src/ck_attribute_smart.h
+-rw-r--r--   0 rousseau   (501) staff       (20)     2208 2019-01-22 20:57:15.000000 PyKCS11-1.5.9/src/dyn_generic.h
+-rw-r--r--   0 rousseau   (501) staff       (20)     1815 2019-01-22 20:49:24.000000 PyKCS11-1.5.9/src/dyn_unix.c
+-rw-r--r--   0 rousseau   (501) staff       (20)     2081 2019-01-22 20:57:15.000000 PyKCS11-1.5.9/src/dyn_win32.c
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2020-07-31 13:34:14.585913 PyKCS11-1.5.9/src/opensc/
+-rw-r--r--   0 rousseau   (501) staff       (20)     6148 2020-05-15 12:44:34.000000 PyKCS11-1.5.9/src/opensc/.DS_Store
+-rw-r--r--   0 rousseau   (501) staff       (20)    43553 2020-05-14 15:35:18.000000 PyKCS11-1.5.9/src/opensc/pkcs11.h
+-rw-r--r--   0 rousseau   (501) staff       (20)    24646 2020-07-30 20:10:17.000000 PyKCS11-1.5.9/src/pkcs11lib.cpp
+-rw-r--r--   0 rousseau   (501) staff       (20)     7053 2019-10-06 20:08:47.000000 PyKCS11-1.5.9/src/pkcs11lib.h
+-rw-r--r--   0 rousseau   (501) staff       (20)     1097 2019-01-22 20:49:24.000000 PyKCS11-1.5.9/src/pykcs11.cpp
+-rw-r--r--   0 rousseau   (501) staff       (20)      795 2019-01-22 20:49:24.000000 PyKCS11-1.5.9/src/pykcs11.h
+-rw-r--r--   0 rousseau   (501) staff       (20)    49449 2020-07-30 20:09:39.000000 PyKCS11-1.5.9/src/pykcs11.i
+-rw-r--r--   0 rousseau   (501) staff       (20)     1423 2019-01-22 20:49:24.000000 PyKCS11-1.5.9/src/pykcs11string.cpp
+-rw-r--r--   0 rousseau   (501) staff       (20)     1111 2019-01-22 20:49:24.000000 PyKCS11-1.5.9/src/pykcs11string.h
+-rw-r--r--   0 rousseau   (501) staff       (20)     1066 2019-01-22 20:49:24.000000 PyKCS11-1.5.9/src/stdafx.cpp
+-rw-r--r--   0 rousseau   (501) staff       (20)     1294 2019-01-22 20:49:24.000000 PyKCS11-1.5.9/src/stdafx.h
+-rw-r--r--   0 rousseau   (501) staff       (20)     2428 2019-01-22 20:49:24.000000 PyKCS11-1.5.9/src/utility.cpp
+-rw-r--r--   0 rousseau   (501) staff       (20)     1301 2019-01-22 20:49:24.000000 PyKCS11-1.5.9/src/utility.h
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2020-07-31 13:34:14.589225 PyKCS11-1.5.9/test/
+-rw-r--r--   0 rousseau   (501) staff       (20)      560 2019-04-17 13:45:32.000000 PyKCS11-1.5.9/test/test_CK.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     4784 2019-10-06 20:11:49.000000 PyKCS11-1.5.9/test/test_LowLevel.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     6353 2020-05-04 15:34:43.000000 PyKCS11-1.5.9/test/test_asymetric.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     3323 2019-04-17 13:45:32.000000 PyKCS11-1.5.9/test/test_asymetric_ECC.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     2938 2019-04-17 13:45:32.000000 PyKCS11-1.5.9/test/test_asymetric_gost.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     2446 2019-10-06 20:09:11.000000 PyKCS11-1.5.9/test/test_ckbytelist.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     1062 2019-04-17 13:45:32.000000 PyKCS11-1.5.9/test/test_digest.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     1424 2019-04-17 13:45:32.000000 PyKCS11-1.5.9/test/test_exception.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     1676 2019-04-17 13:45:32.000000 PyKCS11-1.5.9/test/test_info.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     2675 2019-04-17 13:45:32.000000 PyKCS11-1.5.9/test/test_init.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     1292 2019-10-06 20:09:11.000000 PyKCS11-1.5.9/test/test_load.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     2623 2019-04-17 13:45:32.000000 PyKCS11-1.5.9/test/test_objects.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     1833 2019-10-06 20:09:11.000000 PyKCS11-1.5.9/test/test_pin.py
+-rw-r--r--   0 rousseau   (501) staff       (20)      724 2019-04-17 13:45:32.000000 PyKCS11-1.5.9/test/test_random.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     4026 2020-05-04 15:34:43.000000 PyKCS11-1.5.9/test/test_symetric.py
+-rw-r--r--   0 rousseau   (501) staff       (20)    11767 2020-05-04 15:34:43.000000 PyKCS11-1.5.9/test/test_wrap.py
+-rw-r--r--   0 rousseau   (501) staff       (20)      488 2020-07-30 20:09:39.000000 PyKCS11-1.5.9/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PyKCS11-1.5.8/COPYING` & `PyKCS11-1.5.9/COPYING`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/Changes.txt` & `PyKCS11-1.5.9/Changes.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 History
 =======
 
+1.5.9 - July 2020, Ludovic Rousseau
+  - call C_GetSlotList() with a NULL parameter to correctly initialize
+	some PKCS#11 lib conforming to PKCS#11 version 2.40.
+
 1.5.8 - May 2020, Ludovic Rousseau
   - CKA_ALWAYS_AUTHENTICATE is boolean
   - CKM_VENDOR_DEFINED_...
    . Fix name: use CKM_ instead of CKR_ prefix
    . Use an explicit hex prefix: CKM_VENDOR_DEFINED_0x45
   - Add missing CKM_*, CKA_*, CKF_*, CKD_*, CKK_*, CKN_*, CKO_*, CKR_*
 	from PKCS#11 v3.0
```

### Comparing `PyKCS11-1.5.8/Makefile` & `PyKCS11-1.5.9/Makefile`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/PKG-INFO` & `PyKCS11-1.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: PyKCS11
-Version: 1.5.8
+Version: 1.5.9
 Summary: A Full PKCS#11 wrapper for Python
 Home-page: https://github.com/LudovicRousseau/PyKCS11
 Author: Giuseppe Amato (Midori)
 Author-email: paipai@tiscali.it
 Maintainer: Ludovic Rousseau
 Maintainer-email: ludovic.rousseau@free.fr
 License: GPL
```

### Comparing `PyKCS11-1.5.8/PyKCS11/__init__.py` & `PyKCS11-1.5.9/PyKCS11/__init__.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/PyKCS11.egg-info/PKG-INFO` & `PyKCS11-1.5.9/PyKCS11.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: PyKCS11
-Version: 1.5.8
+Version: 1.5.9
 Summary: A Full PKCS#11 wrapper for Python
 Home-page: https://github.com/LudovicRousseau/PyKCS11
 Author: Giuseppe Amato (Midori)
 Author-email: paipai@tiscali.it
 Maintainer: Ludovic Rousseau
 Maintainer-email: ludovic.rousseau@free.fr
 License: GPL
```

### Comparing `PyKCS11-1.5.8/PyKCS11.egg-info/SOURCES.txt` & `PyKCS11-1.5.9/PyKCS11.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/README.md` & `PyKCS11-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/docs/Makefile` & `PyKCS11-1.5.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/docs/conf.py` & `PyKCS11-1.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/docs/index.rst` & `PyKCS11-1.5.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/docs/license.rst` & `PyKCS11-1.5.9/docs/license.rst`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/docs/samples.rst` & `PyKCS11-1.5.9/docs/samples.rst`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/pykcs11.rc` & `PyKCS11-1.5.9/pykcs11.rc`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/run_test.py` & `PyKCS11-1.5.9/run_test.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/samples/LowLevel/InitTokenPin.py` & `PyKCS11-1.5.9/samples/LowLevel/InitTokenPin.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/samples/LowLevel/dumpit.py` & `PyKCS11-1.5.9/samples/LowLevel/dumpit.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/samples/LowLevel/rand.py` & `PyKCS11-1.5.9/samples/LowLevel/rand.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/samples/LowLevel/test.py` & `PyKCS11-1.5.9/samples/LowLevel/test.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/samples/LowLevel/test1.py` & `PyKCS11-1.5.9/samples/LowLevel/test1.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/samples/destroy_by_ID.py` & `PyKCS11-1.5.9/samples/destroy_by_ID.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/samples/dumpit.py` & `PyKCS11-1.5.9/samples/dumpit.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/samples/ec_generate.py` & `PyKCS11-1.5.9/samples/ec_generate.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/samples/ec_signature.py` & `PyKCS11-1.5.9/samples/ec_signature.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/samples/encrypt.py` & `PyKCS11-1.5.9/samples/encrypt.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/samples/events.py` & `PyKCS11-1.5.9/samples/events.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/samples/generate.py` & `PyKCS11-1.5.9/samples/generate.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/samples/genkeypair_import_cert.py` & `PyKCS11-1.5.9/samples/genkeypair_import_cert.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/samples/getinfo.py` & `PyKCS11-1.5.9/samples/getinfo.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/samples/modulus.py` & `PyKCS11-1.5.9/samples/modulus.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/samples/rsa_encrypt.py` & `PyKCS11-1.5.9/samples/rsa_encrypt.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/samples/signature.py` & `PyKCS11-1.5.9/samples/signature.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/samples/unblock.py` & `PyKCS11-1.5.9/samples/unblock.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/setup.py` & `PyKCS11-1.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         copy_file("src/LowLevel.py", "PyKCS11")
         self.run_command("build_py")
         build.run(self)
 
 
 setup(
     name="PyKCS11",
-    version="1.5.8",
+    version="1.5.9",
     description="A Full PKCS#11 wrapper for Python",
     keywords="crypto,pki,pkcs11,c++",
     classifiers=classifiers,
     platforms="Win32 Unix",
     long_description=description,
     author="Giuseppe Amato (Midori)",
     author_email="paipai@tiscali.it",
```

### Comparing `PyKCS11-1.5.8/src/.DS_Store` & `PyKCS11-1.5.9/src/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 1800 0000 0800  ....Bud1........
 00000010: 0000 1800 0000 100b 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0017  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0016  ................
 00000050: 0000 0001 0000 1000 0074 0074 0072 0069  .........t.t.r.i
 00000060: 0062 0075 0000 0000 0000 0000 0000 0000  .b.u............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -250,102 +250,102 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0000 0000 0017 0000 0016  ................
+00001000: 0000 0000 0000 0000 0000 0016 0000 0016  ................
 00001010: 0063 006b 005f 0061 0074 0074 0072 0069  .c.k._.a.t.t.r.i
 00001020: 0062 0075 0074 0065 005f 0073 006d 0061  .b.u.t.e._.s.m.a
 00001030: 0072 0074 002e 0063 0070 0070 496c 6f63  .r.t...c.p.pIloc
 00001040: 626c 6f62 0000 0010 0000 0039 0000 0028  blob.......9...(
 00001050: ffff ffff ffff 0000 0000 0014 0063 006b  .............c.k
 00001060: 005f 0061 0074 0074 0072 0069 0062 0075  ._.a.t.t.r.i.b.u
 00001070: 0074 0065 005f 0073 006d 0061 0072 0074  .t.e._.s.m.a.r.t
 00001080: 002e 0068 496c 6f63 626c 6f62 0000 0010  ...hIlocblob....
 00001090: 0000 00a3 0000 0028 ffff ffff ffff 0000  .......(........
-000010a0: 0000 0003 0064 0065 0076 496c 6f63 626c  .....d.e.vIlocbl
-000010b0: 6f62 0000 0010 0000 02b5 0000 0108 ffff  ob..............
-000010c0: ffff ffff 0000 0000 000d 0064 0079 006e  ...........d.y.n
-000010d0: 005f 0067 0065 006e 0065 0072 0069 0063  ._.g.e.n.e.r.i.c
-000010e0: 002e 0068 496c 6f63 626c 6f62 0000 0010  ...hIlocblob....
-000010f0: 0000 010d 0000 0028 ffff ffff ffff 0000  .......(........
-00001100: 0000 000a 0064 0079 006e 005f 0075 006e  .....d.y.n._.u.n
-00001110: 0069 0078 002e 0063 496c 6f63 626c 6f62  .i.x...cIlocblob
-00001120: 0000 0010 0000 0177 0000 0028 ffff ffff  .......w...(....
-00001130: ffff 0000 0000 000b 0064 0079 006e 005f  .........d.y.n._
-00001140: 0077 0069 006e 0033 0032 002e 0063 496c  .w.i.n.3.2...cIl
-00001150: 6f63 626c 6f62 0000 0010 0000 01e1 0000  ocblob..........
-00001160: 0028 ffff ffff ffff 0000 0000 000b 004c  .(.............L
-00001170: 006f 0077 004c 0065 0076 0065 006c 002e  .o.w.L.e.v.e.l..
-00001180: 0070 0079 496c 6f63 626c 6f62 0000 0010  .p.yIlocblob....
-00001190: 0000 024b 0000 0028 ffff ffff ffff 0000  ...K...(........
-000011a0: 0000 0006 006f 0070 0065 006e 0073 0063  .....o.p.e.n.s.c
-000011b0: 496c 6f63 626c 6f62 0000 0010 0000 02b5  Ilocblob........
-000011c0: 0000 0028 ffff ffff ffff 0000 0000 0006  ...(............
-000011d0: 006f 0070 0065 006e 0073 0063 6277 7370  .o.p.e.n.s.cbwsp
-000011e0: 626c 6f62 0000 00cb 6270 6c69 7374 3030  blob....bplist00
-000011f0: d701 0203 0405 0607 0809 0908 090d 095d  ...............]
-00001200: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
-00001210: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
-00001220: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
-00001230: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
-00001240: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
-00001250: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00001260: 7208 0909 0809 5f10 1a7b 7b31 3034 392c  r....._..{{1049,
-00001270: 2033 3537 7d2c 207b 3130 3233 2c20 3931   357}, {1023, 91
-00001280: 377d 7d09 0817 2531 3d49 606d 797a 7b7c  7}}...%1=I`myz{|
-00001290: 7d7e 9b00 0000 0000 0001 0100 0000 0000  }~..............
-000012a0: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
-000012b0: 0000 9c00 0000 0600 6f00 7000 6500 6e00  ........o.p.e.n.
-000012c0: 7300 6366 6473 6362 6f6f 6c01 0000 0006  s.cfdscbool.....
-000012d0: 006f 0070 0065 006e 0073 0063 7653 726e  .o.p.e.n.s.cvSrn
-000012e0: 6c6f 6e67 0000 0001 0000 000d 0070 006b  long.........p.k
-000012f0: 0063 0073 0031 0031 006c 0069 0062 002e  .c.s.1.1.l.i.b..
-00001300: 0063 0070 0070 496c 6f63 626c 6f62 0000  .c.p.pIlocblob..
-00001310: 0010 0000 0039 0000 0098 ffff ffff ffff  .....9..........
-00001320: 0000 0000 000b 0070 006b 0063 0073 0031  .......p.k.c.s.1
-00001330: 0031 006c 0069 0062 002e 0068 496c 6f63  .1.l.i.b...hIloc
-00001340: 626c 6f62 0000 0010 0000 00a3 0000 0098  blob............
-00001350: ffff ffff ffff 0000 0000 000b 0070 0079  .............p.y
-00001360: 006b 0063 0073 0031 0031 002e 0063 0070  .k.c.s.1.1...c.p
-00001370: 0070 496c 6f63 626c 6f62 0000 0010 0000  .pIlocblob......
-00001380: 0177 0000 0098 ffff ffff ffff 0000 0000  .w..............
-00001390: 0009 0070 0079 006b 0063 0073 0031 0031  ...p.y.k.c.s.1.1
-000013a0: 002e 0068 496c 6f63 626c 6f62 0000 0010  ...hIlocblob....
-000013b0: 0000 01e1 0000 0098 ffff ffff ffff 0000  ................
-000013c0: 0000 0009 0070 0079 006b 0063 0073 0031  .....p.y.k.c.s.1
-000013d0: 0031 002e 0069 496c 6f63 626c 6f62 0000  .1...iIlocblob..
-000013e0: 0010 0000 024b 0000 0098 ffff ffff ffff  .....K..........
-000013f0: 0000 0000 0010 0070 0079 006b 0063 0073  .......p.y.k.c.s
-00001400: 0031 0031 005f 0077 0072 0061 0070 002e  .1.1._.w.r.a.p..
-00001410: 0063 0070 0070 496c 6f63 626c 6f62 0000  .c.p.pIlocblob..
-00001420: 0010 0000 010d 0000 0098 ffff ffff ffff  ................
-00001430: 0000 0000 0011 0070 0079 006b 0063 0073  .......p.y.k.c.s
-00001440: 0031 0031 0073 0074 0072 0069 006e 0067  .1.1.s.t.r.i.n.g
-00001450: 002e 0063 0070 0070 496c 6f63 626c 6f62  ...c.p.pIlocblob
-00001460: 0000 0010 0000 02b5 0000 0098 ffff ffff  ................
-00001470: ffff 0000 0000 000f 0070 0079 006b 0063  .........p.y.k.c
-00001480: 0073 0031 0031 0073 0074 0072 0069 006e  .s.1.1.s.t.r.i.n
-00001490: 0067 002e 0068 496c 6f63 626c 6f62 0000  .g...hIlocblob..
-000014a0: 0010 0000 0039 0000 0108 ffff ffff ffff  .....9..........
-000014b0: 0000 0000 000a 0073 0074 0064 0061 0066  .......s.t.d.a.f
-000014c0: 0078 002e 0063 0070 0070 496c 6f63 626c  .x...c.p.pIlocbl
-000014d0: 6f62 0000 0010 0000 00a3 0000 0108 ffff  ob..............
-000014e0: ffff ffff 0000 0000 0008 0073 0074 0064  ...........s.t.d
-000014f0: 0061 0066 0078 002e 0068 496c 6f63 626c  .a.f.x...hIlocbl
-00001500: 6f62 0000 0010 0000 010d 0000 0108 ffff  ob..............
-00001510: ffff ffff 0000 0000 000b 0075 0074 0069  ...........u.t.i
-00001520: 006c 0069 0074 0079 002e 0063 0070 0070  .l.i.t.y...c.p.p
-00001530: 496c 6f63 626c 6f62 0000 0010 0000 0177  Ilocblob.......w
-00001540: 0000 0108 ffff ffff ffff 0000 0000 0009  ................
-00001550: 0075 0074 0069 006c 0069 0074 0079 002e  .u.t.i.l.i.t.y..
-00001560: 0068 496c 6f63 626c 6f62 0000 0010 0000  .hIlocblob......
-00001570: 01e1 0000 0108 ffff ffff ffff 0000 0000  ................
+000010a0: 0000 000d 0064 0079 006e 005f 0067 0065  .....d.y.n._.g.e
+000010b0: 006e 0065 0072 0069 0063 002e 0068 496c  .n.e.r.i.c...hIl
+000010c0: 6f63 626c 6f62 0000 0010 0000 010d 0000  ocblob..........
+000010d0: 0028 ffff ffff ffff 0000 0000 000a 0064  .(.............d
+000010e0: 0079 006e 005f 0075 006e 0069 0078 002e  .y.n._.u.n.i.x..
+000010f0: 0063 496c 6f63 626c 6f62 0000 0010 0000  .cIlocblob......
+00001100: 0177 0000 0028 ffff ffff ffff 0000 0000  .w...(..........
+00001110: 000b 0064 0079 006e 005f 0077 0069 006e  ...d.y.n._.w.i.n
+00001120: 0033 0032 002e 0063 496c 6f63 626c 6f62  .3.2...cIlocblob
+00001130: 0000 0010 0000 01e1 0000 0028 ffff ffff  ...........(....
+00001140: ffff 0000 0000 000b 004c 006f 0077 004c  .........L.o.w.L
+00001150: 0065 0076 0065 006c 002e 0070 0079 496c  .e.v.e.l...p.yIl
+00001160: 6f63 626c 6f62 0000 0010 0000 024b 0000  ocblob.......K..
+00001170: 0028 ffff ffff ffff 0000 0000 0006 006f  .(.............o
+00001180: 0070 0065 006e 0073 0063 496c 6f63 626c  .p.e.n.s.cIlocbl
+00001190: 6f62 0000 0010 0000 02b5 0000 0028 ffff  ob...........(..
+000011a0: ffff ffff 0000 0000 0006 006f 0070 0065  ...........o.p.e
+000011b0: 006e 0073 0063 6277 7370 626c 6f62 0000  .n.s.cbwspblob..
+000011c0: 00cb 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
+000011d0: 0607 0809 0908 090d 095d 5368 6f77 5374  .........]ShowSt
+000011e0: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
+000011f0: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
+00001200: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
+00001210: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
+00001220: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
+00001230: 5368 6f77 5369 6465 6261 7208 0909 0809  ShowSidebar.....
+00001240: 5f10 1a7b 7b31 3034 392c 2033 3537 7d2c  _..{{1049, 357},
+00001250: 207b 3130 3233 2c20 3931 377d 7d09 0817   {1023, 917}}...
+00001260: 2531 3d49 606d 797a 7b7c 7d7e 9b00 0000  %1=I`myz{|}~....
+00001270: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
+00001280: 0000 0000 0000 0000 0000 0000 9c00 0000  ................
+00001290: 0600 6f00 7000 6500 6e00 7300 6366 6473  ..o.p.e.n.s.cfds
+000012a0: 6362 6f6f 6c01 0000 0006 006f 0070 0065  cbool......o.p.e
+000012b0: 006e 0073 0063 7653 726e 6c6f 6e67 0000  .n.s.cvSrnlong..
+000012c0: 0001 0000 000d 0070 006b 0063 0073 0031  .......p.k.c.s.1
+000012d0: 0031 006c 0069 0062 002e 0063 0070 0070  .1.l.i.b...c.p.p
+000012e0: 496c 6f63 626c 6f62 0000 0010 0000 0039  Ilocblob.......9
+000012f0: 0000 0098 ffff ffff ffff 0000 0000 000b  ................
+00001300: 0070 006b 0063 0073 0031 0031 006c 0069  .p.k.c.s.1.1.l.i
+00001310: 0062 002e 0068 496c 6f63 626c 6f62 0000  .b...hIlocblob..
+00001320: 0010 0000 00a3 0000 0098 ffff ffff ffff  ................
+00001330: 0000 0000 000b 0070 0079 006b 0063 0073  .......p.y.k.c.s
+00001340: 0031 0031 002e 0063 0070 0070 496c 6f63  .1.1...c.p.pIloc
+00001350: 626c 6f62 0000 0010 0000 0177 0000 0098  blob.......w....
+00001360: ffff ffff ffff 0000 0000 0009 0070 0079  .............p.y
+00001370: 006b 0063 0073 0031 0031 002e 0068 496c  .k.c.s.1.1...hIl
+00001380: 6f63 626c 6f62 0000 0010 0000 01e1 0000  ocblob..........
+00001390: 0098 ffff ffff ffff 0000 0000 0009 0070  ...............p
+000013a0: 0079 006b 0063 0073 0031 0031 002e 0069  .y.k.c.s.1.1...i
+000013b0: 496c 6f63 626c 6f62 0000 0010 0000 024b  Ilocblob.......K
+000013c0: 0000 0098 ffff ffff ffff 0000 0000 0010  ................
+000013d0: 0070 0079 006b 0063 0073 0031 0031 005f  .p.y.k.c.s.1.1._
+000013e0: 0077 0072 0061 0070 002e 0063 0070 0070  .w.r.a.p...c.p.p
+000013f0: 496c 6f63 626c 6f62 0000 0010 0000 010d  Ilocblob........
+00001400: 0000 0098 ffff ffff ffff 0000 0000 0011  ................
+00001410: 0070 0079 006b 0063 0073 0031 0031 0073  .p.y.k.c.s.1.1.s
+00001420: 0074 0072 0069 006e 0067 002e 0063 0070  .t.r.i.n.g...c.p
+00001430: 0070 496c 6f63 626c 6f62 0000 0010 0000  .pIlocblob......
+00001440: 02b5 0000 0098 ffff ffff ffff 0000 0000  ................
+00001450: 000f 0070 0079 006b 0063 0073 0031 0031  ...p.y.k.c.s.1.1
+00001460: 0073 0074 0072 0069 006e 0067 002e 0068  .s.t.r.i.n.g...h
+00001470: 496c 6f63 626c 6f62 0000 0010 0000 0039  Ilocblob.......9
+00001480: 0000 0108 ffff ffff ffff 0000 0000 000a  ................
+00001490: 0073 0074 0064 0061 0066 0078 002e 0063  .s.t.d.a.f.x...c
+000014a0: 0070 0070 496c 6f63 626c 6f62 0000 0010  .p.pIlocblob....
+000014b0: 0000 00a3 0000 0108 ffff ffff ffff 0000  ................
+000014c0: 0000 0008 0073 0074 0064 0061 0066 0078  .....s.t.d.a.f.x
+000014d0: 002e 0068 496c 6f63 626c 6f62 0000 0010  ...hIlocblob....
+000014e0: 0000 010d 0000 0108 ffff ffff ffff 0000  ................
+000014f0: 0000 000b 0075 0074 0069 006c 0069 0074  .....u.t.i.l.i.t
+00001500: 0079 002e 0063 0070 0070 496c 6f63 626c  .y...c.p.pIlocbl
+00001510: 6f62 0000 0010 0000 0177 0000 0108 ffff  ob.......w......
+00001520: ffff ffff 0000 0000 0009 0075 0074 0069  ...........u.t.i
+00001530: 006c 0069 0074 0079 002e 0068 496c 6f63  .l.i.t.y...hIloc
+00001540: 626c 6f62 0000 0010 0000 01e1 0000 0108  blob............
+00001550: ffff ffff ffff 0000 0000 0000 0000 0000  ................
+00001560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -457,23 +457,23 @@
 00001c80: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001c90: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 00001ca0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 00001cb0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
 00001cc0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
 00001cd0: 0000 0000 0104 0000 0000 0000 0108 0000  ................
 00001ce0: 0000 0000 0110 0000 0000 0000 0120 0000  ............. ..
-00001cf0: 0000 0000 0140 0000 0000 0000 0063 626c  .....@.......cbl
-00001d00: 6f62 0000 0010 0000 010d 0000 0108 ffff  ob..............
-00001d10: ffff ffff 0000 0000 000b 0075 0074 0069  ...........u.t.i
-00001d20: 006c 0069 0074 0079 002e 0063 0070 0070  .l.i.t.y...c.p.p
-00001d30: 496c 6f63 626c 6f62 0000 0010 0000 0177  Ilocblob.......w
-00001d40: 0000 0108 ffff ffff ffff 0000 0000 0009  ................
-00001d50: 0075 0074 0069 006c 0069 0074 0079 002e  .u.t.i.l.i.t.y..
-00001d60: 0068 496c 6f63 626c 6f62 0000 0010 0000  .hIlocblob......
-00001d70: 01e1 0000 0108 ffff ffff ffff 0000 0000  ................
+00001cf0: 0000 0000 0140 0000 0000 0000 0069 0074  .....@.......i.t
+00001d00: 0079 002e 0063 0070 0070 496c 6f63 626c  .y...c.p.pIlocbl
+00001d10: 6f62 0000 0010 0000 0177 0000 0108 ffff  ob.......w......
+00001d20: ffff ffff 0000 0000 0009 0075 0074 0069  ...........u.t.i
+00001d30: 006c 0069 0074 0079 002e 0068 496c 6f63  .l.i.t.y...hIloc
+00001d40: 626c 6f62 0000 0010 0000 01e1 0000 0108  blob............
+00001d50: ffff ffff ffff 0000 0000 0000 0000 0000  ................
+00001d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `PyKCS11-1.5.8/src/LowLevel.py` & `PyKCS11-1.5.9/src/LowLevel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file was automatically generated by SWIG (http://www.swig.org).
-# Version 4.0.1
+# Version 4.0.2
 #
 # Do not make changes to this file unless you know what you are doing--modify
 # the SWIG interface file instead.
 
 from sys import version_info as _swig_python_version_info
 if _swig_python_version_info < (2, 7, 0):
     raise RuntimeError("Python 2.7 or later required")
```

### Comparing `PyKCS11-1.5.8/src/ck_attribute_smart.cpp` & `PyKCS11-1.5.9/src/ck_attribute_smart.cpp`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/src/ck_attribute_smart.h` & `PyKCS11-1.5.9/src/ck_attribute_smart.h`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/src/dyn_generic.h` & `PyKCS11-1.5.9/src/dyn_generic.h`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/src/dyn_unix.c` & `PyKCS11-1.5.9/src/dyn_unix.c`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/src/dyn_win32.c` & `PyKCS11-1.5.9/src/dyn_win32.c`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/src/opensc/.DS_Store` & `PyKCS11-1.5.9/src/opensc/.DS_Store`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/src/opensc/pkcs11.h` & `PyKCS11-1.5.9/src/opensc/pkcs11.h`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/src/pkcs11lib.cpp` & `PyKCS11-1.5.9/src/pkcs11lib.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -130,20 +130,27 @@
 	unsigned char tokenPresent,
 	vector<long>& slotList)
 {
 	CPKCS11LIB_PROLOGUE(C_GetSlotList);
 
 	CK_ULONG i;
 	slotList.clear();
-	CK_SLOT_ID ck_slotList[1024];
-	CK_ULONG ulSlotCount = sizeof(ck_slotList)/sizeof(ck_slotList[0]);
-	rv = m_pFunc->C_GetSlotList(tokenPresent, ck_slotList, &ulSlotCount);
+	CK_ULONG ulSlotCount;
+	rv = m_pFunc->C_GetSlotList(tokenPresent, NULL, &ulSlotCount);
 	if (CKR_OK == rv)
-		for(i=0; i<ulSlotCount; i++)
-			slotList.push_back(ck_slotList[i]);
+	{
+		CK_SLOT_ID_PTR ck_slotList;
+		ck_slotList = (CK_SLOT_ID_PTR)malloc(ulSlotCount * sizeof(CK_SLOT_ID));
+		rv = m_pFunc->C_GetSlotList(tokenPresent, ck_slotList, &ulSlotCount);
+		if (CKR_OK == rv)
+			for(i=0; i<ulSlotCount; i++)
+				slotList.push_back(ck_slotList[i]);
+
+		free(ck_slotList);
+	}
 
 	CPKCS11LIB_EPILOGUE;
 	return rv;
 }
 
 CK_RV CPKCS11Lib::C_GetSlotInfo(
 	CK_SLOT_ID slotID,
```

### Comparing `PyKCS11-1.5.8/src/pkcs11lib.h` & `PyKCS11-1.5.9/src/pkcs11lib.h`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/src/pykcs11.cpp` & `PyKCS11-1.5.9/src/pykcs11.cpp`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/src/pykcs11.h` & `PyKCS11-1.5.9/src/pykcs11.h`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/src/pykcs11.i` & `PyKCS11-1.5.9/src/pykcs11.i`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/src/pykcs11string.cpp` & `PyKCS11-1.5.9/src/pykcs11string.cpp`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/src/pykcs11string.h` & `PyKCS11-1.5.9/src/pykcs11string.h`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/src/stdafx.cpp` & `PyKCS11-1.5.9/src/stdafx.cpp`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/src/stdafx.h` & `PyKCS11-1.5.9/src/stdafx.h`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/src/utility.cpp` & `PyKCS11-1.5.9/src/utility.cpp`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/src/utility.h` & `PyKCS11-1.5.9/src/utility.h`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/test/test_CK.py` & `PyKCS11-1.5.9/test/test_CK.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/test/test_LowLevel.py` & `PyKCS11-1.5.9/test/test_LowLevel.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/test/test_asymetric.py` & `PyKCS11-1.5.9/test/test_asymetric.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/test/test_asymetric_ECC.py` & `PyKCS11-1.5.9/test/test_asymetric_ECC.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/test/test_asymetric_gost.py` & `PyKCS11-1.5.9/test/test_asymetric_gost.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/test/test_ckbytelist.py` & `PyKCS11-1.5.9/test/test_ckbytelist.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/test/test_digest.py` & `PyKCS11-1.5.9/test/test_digest.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/test/test_exception.py` & `PyKCS11-1.5.9/test/test_exception.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/test/test_info.py` & `PyKCS11-1.5.9/test/test_info.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/test/test_init.py` & `PyKCS11-1.5.9/test/test_init.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/test/test_load.py` & `PyKCS11-1.5.9/test/test_load.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/test/test_objects.py` & `PyKCS11-1.5.9/test/test_objects.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/test/test_pin.py` & `PyKCS11-1.5.9/test/test_pin.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/test/test_random.py` & `PyKCS11-1.5.9/test/test_random.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/test/test_symetric.py` & `PyKCS11-1.5.9/test/test_symetric.py`

 * *Files identical despite different names*

### Comparing `PyKCS11-1.5.8/test/test_wrap.py` & `PyKCS11-1.5.9/test/test_wrap.py`

 * *Files identical despite different names*


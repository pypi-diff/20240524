# Comparing `tmp/nuclia.plone-1.0a3.tar.gz` & `tmp/nuclia.plone-1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuclia.plone-1.0a3.tar", last modified: Mon Oct 10 15:49:08 2022, max compression
+gzip compressed data, was "nuclia.plone-1.0b1.tar", last modified: Fri May 24 08:12:10 2024, max compression
```

## Comparing `nuclia.plone-1.0a3.tar` & `nuclia.plone-1.0b1.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2022-10-10 15:49:08.786229 nuclia.plone-1.0a3/
--rw-r--r--   0 ebr        (501) staff       (20)      251 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/CHANGES.rst
--rw-r--r--   0 ebr        (501) staff       (20)       64 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/CONTRIBUTORS.rst
--rw-r--r--   0 ebr        (501) staff       (20)     1338 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/DEVELOP.rst
--rw-r--r--   0 ebr        (501) staff       (20)    18092 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/LICENSE.GPL
--rw-r--r--   0 ebr        (501) staff       (20)      656 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/LICENSE.rst
--rw-r--r--   0 ebr        (501) staff       (20)       63 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/MANIFEST.in
--rw-r--r--   0 ebr        (501) staff       (20)     2594 2022-10-10 15:49:08.786369 nuclia.plone-1.0a3/PKG-INFO
--rw-r--r--   0 ebr        (501) staff       (20)     1228 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/README.md
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2022-10-10 15:49:08.770178 nuclia.plone-1.0a3/docs/
--rw-r--r--   0 ebr        (501) staff       (20)     7911 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/docs/conf.py
--rw-r--r--   0 ebr        (501) staff       (20)       59 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/docs/index.rst
--rw-r--r--   0 ebr        (501) staff       (20)      334 2022-10-10 15:49:08.786918 nuclia.plone-1.0a3/setup.cfg
--rw-r--r--   0 ebr        (501) staff       (20)     2397 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/setup.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2022-10-10 15:49:08.750894 nuclia.plone-1.0a3/src/
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2022-10-10 15:49:08.770856 nuclia.plone-1.0a3/src/nuclia/
--rw-r--r--   0 ebr        (501) staff       (20)       80 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2022-10-10 15:49:08.777082 nuclia.plone-1.0a3/src/nuclia/plone/
--rw-r--r--   0 ebr        (501) staff       (20)      719 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2022-10-10 15:49:08.779629 nuclia.plone-1.0a3/src/nuclia/plone/browser/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/browser/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      623 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/browser/configure.zcml
--rw-r--r--   0 ebr        (501) staff       (20)     2478 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/browser/extract.py
--rw-r--r--   0 ebr        (501) staff       (20)      713 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/browser/search.pt
--rw-r--r--   0 ebr        (501) staff       (20)      934 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/browser/search.py
--rw-r--r--   0 ebr        (501) staff       (20)     2178 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/configure.zcml
--rw-r--r--   0 ebr        (501) staff       (20)     5332 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/events.py
--rw-r--r--   0 ebr        (501) staff       (20)      261 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/interfaces.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2022-10-10 15:49:08.781589 nuclia.plone-1.0a3/src/nuclia/plone/locales/
--rw-r--r--   0 ebr        (501) staff       (20)      611 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/locales/README.rst
--rw-r--r--   0 ebr        (501) staff       (20)        0 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/locales/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2022-10-10 15:49:08.751667 nuclia.plone-1.0a3/src/nuclia/plone/locales/en/
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2022-10-10 15:49:08.781973 nuclia.plone-1.0a3/src/nuclia/plone/locales/en/LC_MESSAGES/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/locales/en/LC_MESSAGES/nuclia.plone.po
--rw-r--r--   0 ebr        (501) staff       (20)        0 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/locales/nuclia.plone.pot
--rw-r--r--   0 ebr        (501) staff       (20)     1740 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/locales/update.py
--rwxr-xr-x   0 ebr        (501) staff       (20)      473 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/locales/update.sh
--rw-r--r--   0 ebr        (501) staff       (20)      260 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/permissions.zcml
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2022-10-10 15:49:08.752163 nuclia.plone-1.0a3/src/nuclia/plone/profiles/
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2022-10-10 15:49:08.784517 nuclia.plone-1.0a3/src/nuclia/plone/profiles/default/
--rw-r--r--   0 ebr        (501) staff       (20)     1486 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/profiles/default/actions.xml
--rw-r--r--   0 ebr        (501) staff       (20)      162 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/profiles/default/browserlayer.xml
--rw-r--r--   0 ebr        (501) staff       (20)      105 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/profiles/default/catalog.xml
--rw-r--r--   0 ebr        (501) staff       (20)      514 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/profiles/default/controlpanel.xml
--rw-r--r--   0 ebr        (501) staff       (20)      195 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/profiles/default/metadata.xml
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2022-10-10 15:49:08.784837 nuclia.plone-1.0a3/src/nuclia/plone/profiles/default/registry/
--rw-r--r--   0 ebr        (501) staff       (20)      376 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/profiles/default/registry/main.xml
--rw-r--r--   0 ebr        (501) staff       (20)      118 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/profiles/default/rolemap.xml
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2022-10-10 15:49:08.785107 nuclia.plone-1.0a3/src/nuclia/plone/profiles/uninstall/
--rw-r--r--   0 ebr        (501) staff       (20)      122 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 ebr        (501) staff       (20)      967 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/settings.py
--rw-r--r--   0 ebr        (501) staff       (20)      775 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/setuphandlers.py
--rw-r--r--   0 ebr        (501) staff       (20)     1408 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/testing.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2022-10-10 15:49:08.785764 nuclia.plone-1.0a3/src/nuclia/plone/tests/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/tests/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2022-10-10 15:49:08.786001 nuclia.plone-1.0a3/src/nuclia/plone/tests/robot/
--rw-r--r--   0 ebr        (501) staff       (20)     1979 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/tests/robot/test_example.robot
--rw-r--r--   0 ebr        (501) staff       (20)      872 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/tests/test_robot.py
--rw-r--r--   0 ebr        (501) staff       (20)     2355 2022-10-10 15:49:02.000000 nuclia.plone-1.0a3/src/nuclia/plone/tests/test_setup.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2022-10-10 15:49:08.774031 nuclia.plone-1.0a3/src/nuclia.plone.egg-info/
--rw-r--r--   0 ebr        (501) staff       (20)     2594 2022-10-10 15:49:06.000000 nuclia.plone-1.0a3/src/nuclia.plone.egg-info/PKG-INFO
--rw-r--r--   0 ebr        (501) staff       (20)     1703 2022-10-10 15:49:08.000000 nuclia.plone-1.0a3/src/nuclia.plone.egg-info/SOURCES.txt
--rw-r--r--   0 ebr        (501) staff       (20)        1 2022-10-10 15:49:06.000000 nuclia.plone-1.0a3/src/nuclia.plone.egg-info/dependency_links.txt
--rw-r--r--   0 ebr        (501) staff       (20)      117 2022-10-10 15:49:07.000000 nuclia.plone-1.0a3/src/nuclia.plone.egg-info/entry_points.txt
--rw-r--r--   0 ebr        (501) staff       (20)        7 2022-10-10 15:49:07.000000 nuclia.plone-1.0a3/src/nuclia.plone.egg-info/namespace_packages.txt
--rw-r--r--   0 ebr        (501) staff       (20)        1 2022-10-10 15:49:06.000000 nuclia.plone-1.0a3/src/nuclia.plone.egg-info/not-zip-safe
--rw-r--r--   0 ebr        (501) staff       (20)      159 2022-10-10 15:49:07.000000 nuclia.plone-1.0a3/src/nuclia.plone.egg-info/requires.txt
--rw-r--r--   0 ebr        (501) staff       (20)        7 2022-10-10 15:49:07.000000 nuclia.plone-1.0a3/src/nuclia.plone.egg-info/top_level.txt
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-24 08:12:10.443643 nuclia.plone-1.0b1/
+-rw-r--r--   0 ebr        (501) staff       (20)      524 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/CHANGES.rst
+-rw-r--r--   0 ebr        (501) staff       (20)       64 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/CONTRIBUTORS.rst
+-rw-r--r--   0 ebr        (501) staff       (20)     1338 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/DEVELOP.rst
+-rw-r--r--   0 ebr        (501) staff       (20)    18092 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/LICENSE.GPL
+-rw-r--r--   0 ebr        (501) staff       (20)      656 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/LICENSE.rst
+-rw-r--r--   0 ebr        (501) staff       (20)       63 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/MANIFEST.in
+-rw-r--r--   0 ebr        (501) staff       (20)     3384 2024-05-24 08:12:10.443828 nuclia.plone-1.0b1/PKG-INFO
+-rw-r--r--   0 ebr        (501) staff       (20)     1745 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/README.md
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-24 08:12:10.423493 nuclia.plone-1.0b1/docs/
+-rw-r--r--   0 ebr        (501) staff       (20)     7911 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/docs/conf.py
+-rw-r--r--   0 ebr        (501) staff       (20)       59 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/docs/index.rst
+-rw-r--r--   0 ebr        (501) staff       (20)      334 2024-05-24 08:12:10.444562 nuclia.plone-1.0b1/setup.cfg
+-rw-r--r--   0 ebr        (501) staff       (20)     2397 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/setup.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-24 08:12:10.416646 nuclia.plone-1.0b1/src/
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-24 08:12:10.423945 nuclia.plone-1.0b1/src/nuclia/
+-rw-r--r--   0 ebr        (501) staff       (20)       80 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-24 08:12:10.431978 nuclia.plone-1.0b1/src/nuclia/plone/
+-rw-r--r--   0 ebr        (501) staff       (20)     1420 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-24 08:12:10.434841 nuclia.plone-1.0b1/src/nuclia/plone/browser/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/browser/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      455 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/browser/configure.zcml
+-rw-r--r--   0 ebr        (501) staff       (20)      678 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/browser/reindex.pt
+-rw-r--r--   0 ebr        (501) staff       (20)      911 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/browser/reindex.py
+-rw-r--r--   0 ebr        (501) staff       (20)      604 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/browser/search.pt
+-rw-r--r--   0 ebr        (501) staff       (20)      919 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/browser/search.py
+-rw-r--r--   0 ebr        (501) staff       (20)     2176 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/configure.zcml
+-rw-r--r--   0 ebr        (501) staff       (20)      752 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/events.py
+-rw-r--r--   0 ebr        (501) staff       (20)      261 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/interfaces.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-24 08:12:10.436995 nuclia.plone-1.0b1/src/nuclia/plone/locales/
+-rw-r--r--   0 ebr        (501) staff       (20)      611 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/locales/README.rst
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/locales/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-24 08:12:10.417461 nuclia.plone-1.0b1/src/nuclia/plone/locales/en/
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-24 08:12:10.437529 nuclia.plone-1.0b1/src/nuclia/plone/locales/en/LC_MESSAGES/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/locales/en/LC_MESSAGES/nuclia.plone.po
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/locales/nuclia.plone.pot
+-rw-r--r--   0 ebr        (501) staff       (20)     1740 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/locales/update.py
+-rwxr-xr-x   0 ebr        (501) staff       (20)      473 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/locales/update.sh
+-rw-r--r--   0 ebr        (501) staff       (20)     5988 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/nuclia_api.py
+-rw-r--r--   0 ebr        (501) staff       (20)      260 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/permissions.zcml
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-24 08:12:10.418184 nuclia.plone-1.0b1/src/nuclia/plone/profiles/
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-24 08:12:10.440462 nuclia.plone-1.0b1/src/nuclia/plone/profiles/default/
+-rw-r--r--   0 ebr        (501) staff       (20)      861 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/profiles/default/actions.xml
+-rw-r--r--   0 ebr        (501) staff       (20)      162 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/profiles/default/browserlayer.xml
+-rw-r--r--   0 ebr        (501) staff       (20)      105 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/profiles/default/catalog.xml
+-rw-r--r--   0 ebr        (501) staff       (20)      514 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/profiles/default/controlpanel.xml
+-rw-r--r--   0 ebr        (501) staff       (20)      195 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/profiles/default/metadata.xml
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-24 08:12:10.440880 nuclia.plone-1.0b1/src/nuclia/plone/profiles/default/registry/
+-rw-r--r--   0 ebr        (501) staff       (20)      374 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/profiles/default/registry/main.xml
+-rw-r--r--   0 ebr        (501) staff       (20)      118 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/profiles/default/rolemap.xml
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-24 08:12:10.441439 nuclia.plone-1.0b1/src/nuclia/plone/profiles/uninstall/
+-rw-r--r--   0 ebr        (501) staff       (20)      122 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 ebr        (501) staff       (20)     2632 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/settings.py
+-rw-r--r--   0 ebr        (501) staff       (20)      775 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/setuphandlers.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1408 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/testing.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-24 08:12:10.442844 nuclia.plone-1.0b1/src/nuclia/plone/tests/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/tests/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-24 08:12:10.443300 nuclia.plone-1.0b1/src/nuclia/plone/tests/robot/
+-rw-r--r--   0 ebr        (501) staff       (20)     1979 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/tests/robot/test_example.robot
+-rw-r--r--   0 ebr        (501) staff       (20)      872 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/tests/test_robot.py
+-rw-r--r--   0 ebr        (501) staff       (20)     2355 2024-05-24 08:12:06.000000 nuclia.plone-1.0b1/src/nuclia/plone/tests/test_setup.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2024-05-24 08:12:10.427585 nuclia.plone-1.0b1/src/nuclia.plone.egg-info/
+-rw-r--r--   0 ebr        (501) staff       (20)     3384 2024-05-24 08:12:09.000000 nuclia.plone-1.0b1/src/nuclia.plone.egg-info/PKG-INFO
+-rw-r--r--   0 ebr        (501) staff       (20)     1770 2024-05-24 08:12:10.000000 nuclia.plone-1.0b1/src/nuclia.plone.egg-info/SOURCES.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        1 2024-05-24 08:12:09.000000 nuclia.plone-1.0b1/src/nuclia.plone.egg-info/dependency_links.txt
+-rw-r--r--   0 ebr        (501) staff       (20)      117 2024-05-24 08:12:09.000000 nuclia.plone-1.0b1/src/nuclia.plone.egg-info/entry_points.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        7 2024-05-24 08:12:09.000000 nuclia.plone-1.0b1/src/nuclia.plone.egg-info/namespace_packages.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        1 2024-05-24 08:12:09.000000 nuclia.plone-1.0b1/src/nuclia.plone.egg-info/not-zip-safe
+-rw-r--r--   0 ebr        (501) staff       (20)      159 2024-05-24 08:12:09.000000 nuclia.plone-1.0b1/src/nuclia.plone.egg-info/requires.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        7 2024-05-24 08:12:09.000000 nuclia.plone-1.0b1/src/nuclia.plone.egg-info/top_level.txt
```

### Comparing `nuclia.plone-1.0a3/DEVELOP.rst` & `nuclia.plone-1.0b1/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `nuclia.plone-1.0a3/LICENSE.GPL` & `nuclia.plone-1.0b1/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `nuclia.plone-1.0a3/LICENSE.rst` & `nuclia.plone-1.0b1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `nuclia.plone-1.0a3/PKG-INFO` & `nuclia.plone-1.0b1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nuclia.plone
-Version: 1.0a3
+Version: 1.0b1
 Summary: Integrate Nuclia search in Plone
 Home-page: https://github.com/nuclia/nuclia.plone
 Author: Eric BREHAULT
 Author-email: ebrehault@gmail.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/nuclia.plone
 Project-URL: Source, https://github.com/nuclia/nuclia.plone
 Project-URL: Tracker, https://github.com/nuclia/nuclia.plone/issues
 Keywords: Python Plone CMS
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
-Classifier: Framework :: Plone :: 5.2
+Classifier: Framework :: Plone :: 5.1
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -42,35 +42,53 @@
 
 Restart Plone.
 
 Go to Site Setup / Add-ons and install `nuclia.plone`.
 
 Go to Nuclia settings, and enter the following:
 
-- Knowledge box ID: you have a default knowledge box created with your Nuclia account, go to [Nuclia dashboard](https://nuclia.cloud/), the knowledge box ID is indicated on the home page in the **Nuclia APi endpoint**
-- API key: see [how to get an API key](https://docs.nuclia.dev/docs/quick-start/push#get-a-service-access-token)
-- Region: this the geographical region your knowledge box is attached to (at the moment only `europe-1` is supported)
-- Widget ID: see [how to create a widget](https://docs.nuclia.dev/docs/quick-start/search#add-a-search-widget-to-your-website)
+- Knowledge box ID: you have a default knowledge box created with your Nuclia account, go to [Nuclia dashboard](https://nuclia.cloud/), the knowledge box ID is indicated on the home page in the **Nuclia APi endpoint**.
+- API key: see [how to get an API key](https://docs.nuclia.dev/docs/guides/getting-started/quick-start/push#get-an-api-key).
+- Region: this the geographical region your knowledge box is attached to.
+- Widget snippet: see [how to create a widget](https://docs.nuclia.dev/docs/guides/getting-started/quick-start/search#add-a-search-widget-to-your-website).
+- File attribute: the attribute of the content that contains the file to index. Default is `file`.
+- Metadata mapping: Nuclia allows to store the following metadata: `title`, `summary`, `tags`, `contributors`, `created`, `modified`. You can map Plone content fields to these metadata fields. If the field belongs to the parent node, use the following format: `parent/field_name`.
+- Workflow states: you can choose which workflow states trigger indexing in Nuclia. Default is `published`.
 
 ## Usage
 
-Everytime a `File` or a `Link` content is created, it is indexed in Nuclia.
+Everytime a content having a file is created or modified (and if it is in the appropriate workflow state).
 
 The Nuclia search widget is visible on the `/@@nuclia-search` view.
 
 
 Contributors
 ============
 
 - Eric BREHAULT, ebrehault@gmail.com
 
 
 Changelog
 =========
 
+1.0b1 (2024-05-24)
+------------------
+
+- Allow to re-index all files
+  [ebrehault]
+
+- Support different field name for the file content, and allow to map metadata fields
+  [ebrehault]
+
+- Compliancy with Plone 5.1
+  [ebrehault]
+
+- Allow to re-index all files
+  [ebrehault]
+
 
 1.0a3 (2022-10-10)
 ------------------
 
 - Fix project metadata.
   [ebrehault]
```

### Comparing `nuclia.plone-1.0a3/docs/conf.py` & `nuclia.plone-1.0b1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nuclia.plone-1.0a3/setup.py` & `nuclia.plone-1.0b1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,23 +10,23 @@
     open('CONTRIBUTORS.rst').read(),
     open('CHANGES.rst').read(),
 ])
 
 
 setup(
     name='nuclia.plone',
-    version='1.0a3',
+    version='1.0b1',
     description="Integrate Nuclia search in Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
-        "Framework :: Plone :: 5.2",
+        "Framework :: Plone :: 5.1",
         "Framework :: Plone :: 6.0",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
@@ -48,15 +48,15 @@
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.7",
     install_requires=[
         'setuptools',
         # -*- Extra requirements: -*-
         'z3c.jbot',
-        'plone.api>=1.8.4',
+        'plone.api>=1.8.2',
         'plone.app.dexterity',
     ],
     extras_require={
         'test': [
             'plone.app.testing',
             # Plone KGS does not use this version, because it would break
             # Remove if your package shall be part of coredev.
```

### Comparing `nuclia.plone-1.0a3/src/nuclia/plone/browser/search.py` & `nuclia.plone-1.0b1/src/nuclia/plone/browser/search.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from plone import api
 from Products.Five.browser import BrowserView
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 
 class SearchWidget(BrowserView):
-    """ Render the search widget)
+    """ Render the search widget
     """
     index = ViewPageTemplateFile("search.pt")
     _kbid = None
     _region = None
     _widget = None
 
     @property
@@ -19,14 +19,14 @@
     @property
     def region(self):
         if not self._region:
             self._region = api.portal.get_registry_record('nuclia.region', default='europe-1')
         return self._region
 
     @property
-    def widget_id(self):
+    def widget(self):
         if not self._widget:
-            self._widget = api.portal.get_registry_record('nuclia.widgetId', default='dashboard')
+            self._widget = api.portal.get_registry_record('nuclia.widget', default='')
         return self._widget
 
     def __call__(self):
         return self.index()
```

### Comparing `nuclia.plone-1.0a3/src/nuclia/plone/configure.zcml` & `nuclia.plone-1.0b1/src/nuclia/plone/configure.zcml`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
   <utility
       factory=".setuphandlers.HiddenProfiles"
       name="nuclia.plone-hiddenprofiles"
       />
 
   <subscriber
     for="Products.CMFCore.interfaces.IContentish
-         zope.lifecycleevent.IObjectCreatedEvent"
+         zope.lifecycleevent.IObjectAddedEvent"
     handler=".events.on_create"
     />
   <subscriber
     for="Products.CMFCore.interfaces.IContentish
          zope.lifecycleevent.IObjectModifiedEvent"
     handler=".events.on_modify"
     />
```

### Comparing `nuclia.plone-1.0a3/src/nuclia/plone/events.py` & `nuclia.plone-1.0b1/src/nuclia/plone/nuclia_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,158 +1,172 @@
-from nuclia.plone import FIELD_ID_ANNOTATION, MD5_ANNOTATION, UID_ANNOTATION, logger, get_kb_path, get_headers
+from nuclia.plone import MD5_ANNOTATION, get_field_mapping, logger, get_kb_path, get_headers
 import requests
 import hashlib
 from base64 import b64encode
 from plone import api
 from zope.annotation.interfaces import IAnnotations
 
+def get_attribute_value(object, attr, default=None):
+    if attr.startswith('parent/'):
+        return get_attribute_value(object.getParentNode(), attr[7:], default)
+    return getattr(object, attr, default)
+
+def flatten_tags(object, attrs):
+    tags = []
+    for attr in attrs:
+        value = get_attribute_value(object, attr, None)
+        if value:
+            if isinstance(value, (list, tuple)):
+                tags.extend(["{attr}/{v}".format(attr=attr, v=v) for v in value if v])
+            else:
+                tags.append("{attr}/{value}".format(attr=attr, value=value))
+    return tags
+
+def get_date(object, field):
+    date = get_attribute_value(object, field, None)
+    if not date:
+        return None
+    return date.strftime('%Y-%m-%dT%H:%M:%S.%fZ')
 
-def on_create(object, event):
-    if is_public(object):
-        upload_to_new_resource(object)
-
-def on_modify(object, event):
-    if not is_public(object):
-        return
-    annotations = IAnnotations(object)
-    resource = annotations.get(UID_ANNOTATION)
-    if not resource:
-        upload_to_new_resource(object)
-    else:
-        update_resource(object)
-
-def on_delete(object, event):
-    if is_public(object):
-        unindex_object(object)
-
-def on_state_change(object, event):
-    if is_public(object):
-        upload_to_new_resource(object)
-    else:
-        unindex_object(object)
+def get_data(object):
+    mapping = get_field_mapping()
+    return {
+        'file': get_attribute_value(object, mapping['file'], None),
+        'title': get_attribute_value(object, mapping['title'], None),
+        'summary': get_attribute_value(object, mapping['summary'], None),
+        'tags': flatten_tags(object, mapping['tags']),
+        'created': get_date(object, mapping['created']),
+        'modified': get_date(object, mapping['modified']),
+        'collaborators': get_attribute_value(object, mapping['collaborators'], None),
+    }
+    
 
 def upload_to_new_resource(object):
-    file = getattr(object, 'file', None)
-    remoteUrl = getattr(object, 'remoteUrl', None)
+    data = get_data(object)
+    file = data.get('file', None)
     annotations = IAnnotations(object)
     if file:
-        response = upload_file(f"{get_kb_path()}/upload", file)
-        if response:
-            resource = response.json()['uuid']
-            annotations[UID_ANNOTATION] = resource
-            field = response.json()['field_id']
-            annotations[FIELD_ID_ANNOTATION] = field
-            annotations[MD5_ANNOTATION] = hashlib.md5(file.data).hexdigest()
-    elif remoteUrl:
+        uuid = api.content.get_uuid(obj=object)
         response = requests.post(
-            f"{get_kb_path()}/resources",
+            "{path}/resources".format(path=get_kb_path()),
             headers=get_headers(),
             json={
-                "links": {"link": { "uri": remoteUrl }},
-                "title": object.title,
-                "icon": 'application/stf-link',
+                "slug": uuid,
+                "title": data.get('title', None),
+                "summary": data.get('summary', None),
+                "origin": {
+                    "created": data.get('created', None),
+                    "modified": data.get('modified', None),
+                    "collaborators": data.get('collaborators', None),
+                    "tags": data.get('tags', None),
+                    "url": object.absolute_url(),
+                    "path": object.absolute_url_path(),
+                }
             },
         )
         if not response.ok:
-            logger.error(f'Error creating link resource')
-            logger.error(response.text)
-        else:
-            resource = response.json()['uuid']
-            annotations[UID_ANNOTATION] = resource
+            if response.status_code == 409:
+                update_resource(object)
+                return
+            else:
+                logger.error('Error creating resource')
+                logger.error(response.text)
+                return
+        response = upload_file(uuid, file)
+        if response:
+            annotations[MD5_ANNOTATION] = hashlib.md5(file.data).hexdigest()
 
-def upload_file(path, file):
+def upload_file(uuid, file):
     filename = getattr(file, "filename", None)
     if not filename:
         return
     content_type = file.contentType
     headers = get_headers()
     headers.update({
         "content-type": content_type,
-        "x-filename": b64encode(filename.encode('ascii')).decode('ascii'),
+        "x-filename": b64encode(filename.encode()).decode(),
     })
     response = requests.post(
-        path,
+        "{path}/slug/{uuid}/file/file/upload".format(path=get_kb_path(), uuid=uuid),
         headers=headers,
         data=file.data,
         verify=False,
     )
     if not response.ok:
-        logger.error(f'Error uploading file')
+        logger.error('Error uploading file')
         logger.error(response.text)
         return None
     else:
         return response
 
 def update_resource(object):
     annotations = IAnnotations(object)
-    file = getattr(object, 'file', None)
-    remoteUrl = getattr(object, 'remoteUrl', None)
-    if not file and not remoteUrl:
+    data = get_data(object)
+    file = data.get('file', None)
+    must_update_file = True
+    if not file:
         return
-    resource = annotations.get(UID_ANNOTATION)
-    data = {}
-    if resource:
-        response = requests.get(
-            f"{get_kb_path()}/resource/{resource}?show=basic&show=values&show=extracted&extracted=file&extracted=link",
-            headers=get_headers()
-        )
-        if not response.ok:
-            logger.error(f'Error getting resource')
+    uuid = api.content.get_uuid(obj=object)
+    fields = {}
+    response = requests.get(
+        "{path}/slug/{uuid}?show=basic&show=values&show=extracted&extracted=file".format(path=get_kb_path(), uuid=uuid),
+        headers=get_headers()
+    )
+    if not response.ok:
+        if response.status_code == 404:
+            upload_to_new_resource(object)
+            return
+        else:
+            logger.error('Error getting resource')
             logger.error(response.text)
-        data = response.json()['data']
-    files = data.get('files', None)
-    links = data.get('links', None)
-    field_id = annotations.get(FIELD_ID_ANNOTATION, None)
-    if files and field_id and field_id in files:
+            return
+    fields = response.json()['data']
+    files = fields.get('files', None)
+    if files and 'file' in files:
         previous_md5 = annotations.get(MD5_ANNOTATION, None)
         current_md5 = hashlib.md5(file.data).hexdigest()
         if previous_md5 == current_md5:
-            return
+            must_update_file = False
         else:
-            delete_field(resource, 'file', field_id, annotations)
-    if links and 'link' in links and links['link']['value']['uri'] != remoteUrl:
-        delete_field(resource, 'link', 'link', annotations)
+            delete_file_field(uuid)
 
-    if file:
-        response = upload_file(f"{get_kb_path()}/resource/{resource}/file/file1/upload", file)
+    if must_update_file:
+        response = upload_file(uuid, file)
         if response:
-            field = response.json()['field_id'].split('/')[-1]
-            annotations[FIELD_ID_ANNOTATION] = field
             annotations[MD5_ANNOTATION] = hashlib.md5(file.data).hexdigest()
-    if remoteUrl:
-        response = requests.patch(
-            f"{get_kb_path()}/resource/{resource}",
-            headers=get_headers(),
-            json={
-                "links": {"link": { "uri": remoteUrl }},
-                "title": object.title,
-            },
-        )
-        if not response.ok:
-            logger.error(f'Error updating link')
-            logger.error(response.text)
+    
+    data = get_data(object)
+    response = requests.patch(
+        "{path}/slug/{uuid}".format(path=get_kb_path(), uuid=uuid),
+        headers=get_headers(),
+        json={
+            "title": data.get('title', None),
+            "summary": data.get('summary', None),
+            "origin": {
+                "created": data.get('created', None),
+                "modified": data.get('modified', None),
+                "collaborators": data.get('collaborators', None),
+                "tags": data.get('tags', None),
+                "url": object.absolute_url(),
+                "path": object.absolute_url_path(),
+            }
+        },
+    )
 
 def unindex_object(object):
-    annotations = IAnnotations(object)
-    resource = annotations.get(UID_ANNOTATION)
-    if resource:
-        response = requests.delete(
-            f"{get_kb_path()}/resource/{resource}",
-            headers=get_headers()
-        )
-        if not response.ok:
-            logger.error(f'Error deleting resource')
-            logger.error(response.text)
-
-def delete_field(resource, field_type, field_id, annotations):
+    uuid = api.content.get_uuid(obj=object)
     response = requests.delete(
-        f"{get_kb_path()}/resource/{resource}/{field_type}/{field_id}",
+        "{path}/slug/{uuid}".format(path=get_kb_path(), uuid=uuid),
         headers=get_headers()
     )
     if not response.ok:
-        logger.error(f'Error deleting field')
+        logger.error('Error deleting resource')
         logger.error(response.text)
-    else:
-        del annotations[FIELD_ID_ANNOTATION]
 
-def is_public(object):
-    return api.content.get_state(obj=object, default='published') == 'published'
+def delete_file_field(resource):
+    response = requests.delete(
+        "{path}/slug/{resource}/file/file".format(path=get_kb_path(), resource=resource),
+        headers=get_headers()
+    )
+    if not response.ok:
+        logger.error('Error deleting field')
+        logger.error(response.text)
```

### Comparing `nuclia.plone-1.0a3/src/nuclia/plone/locales/README.rst` & `nuclia.plone-1.0b1/src/nuclia/plone/locales/README.rst`

 * *Files identical despite different names*

### Comparing `nuclia.plone-1.0a3/src/nuclia/plone/locales/update.py` & `nuclia.plone-1.0b1/src/nuclia/plone/locales/update.py`

 * *Files identical despite different names*

### Comparing `nuclia.plone-1.0a3/src/nuclia/plone/profiles/default/actions.xml` & `nuclia.plone-1.0b1/src/nuclia/plone/profiles/default/actions.xml`

 * *Files 18% similar despite different names*

#### Comparing `nuclia.plone-1.0a3/src/nuclia/plone/profiles/default/actions.xml` & `nuclia.plone-1.0b1/src/nuclia/plone/profiles/default/actions.xml`

```diff
@@ -1,32 +1,19 @@
 <?xml version="1.0" encoding="utf-8"?>
 <object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="portal_actions" meta_type="Plone Actions Tool">
   <action-provider name="portal_workflow"/>
   <action-provider name="portal_types"/>
   <action-provider name="portal_actions"/>
   <object name="object_buttons" meta_type="CMF Action Category">
-    <object name="nuclia_extract_text" meta_type="CMF Action" i18n:domain="plone">
-      <property name="title" i18n:translate="">Extract text</property>
-      <property name="url_expr">string:$object_url/nuclia-extract-text</property>
+    <object name="nuclia_reindex" meta_type="CMF Action" i18n:domain="plone">
+      <property name="title" i18n:translate="">Re-index files in Nuclia</property>
+      <property name="url_expr">string:$object_url/nuclia-reindex</property>
       <property name="link_target"/>
       <property name="icon_expr"/>
       <property name="permissions">
         <element value="View"/>
         <element value="Modify portal content"/>
       </property>
       <property name="visible">True</property>
     </object>
-    <object name="nuclia_extract_keywords" meta_type="CMF Action" i18n:domain="plone">
-      <property name="title" i18n:translate="">Extract keywords</property>
-      <property name="description" i18n:translate="">None</property>
-      <property name="url_expr">string:$object_url/nuclia-extract-keywords</property>
-      <property name="link_target"/>
-      <property name="icon_expr"/>
-      <property name="available_expr"/>
-      <property name="permissions">
-        <element value="Modify portal content"/>
-        <element value="View"/>
-      </property>
-      <property name="visible">True</property>
-    </object>
   </object>
 </object>
```

### Comparing `nuclia.plone-1.0a3/src/nuclia/plone/profiles/default/controlpanel.xml` & `nuclia.plone-1.0b1/src/nuclia/plone/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `nuclia.plone-1.0a3/src/nuclia/plone/setuphandlers.py` & `nuclia.plone-1.0b1/src/nuclia/plone/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `nuclia.plone-1.0a3/src/nuclia/plone/testing.py` & `nuclia.plone-1.0b1/src/nuclia/plone/testing.py`

 * *Files identical despite different names*

### Comparing `nuclia.plone-1.0a3/src/nuclia/plone/tests/robot/test_example.robot` & `nuclia.plone-1.0b1/src/nuclia/plone/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `nuclia.plone-1.0a3/src/nuclia/plone/tests/test_robot.py` & `nuclia.plone-1.0b1/src/nuclia/plone/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `nuclia.plone-1.0a3/src/nuclia/plone/tests/test_setup.py` & `nuclia.plone-1.0b1/src/nuclia/plone/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `nuclia.plone-1.0a3/src/nuclia.plone.egg-info/PKG-INFO` & `nuclia.plone-1.0b1/src/nuclia.plone.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nuclia.plone
-Version: 1.0a3
+Version: 1.0b1
 Summary: Integrate Nuclia search in Plone
 Home-page: https://github.com/nuclia/nuclia.plone
 Author: Eric BREHAULT
 Author-email: ebrehault@gmail.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/nuclia.plone
 Project-URL: Source, https://github.com/nuclia/nuclia.plone
 Project-URL: Tracker, https://github.com/nuclia/nuclia.plone/issues
 Keywords: Python Plone CMS
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
-Classifier: Framework :: Plone :: 5.2
+Classifier: Framework :: Plone :: 5.1
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -42,35 +42,53 @@
 
 Restart Plone.
 
 Go to Site Setup / Add-ons and install `nuclia.plone`.
 
 Go to Nuclia settings, and enter the following:
 
-- Knowledge box ID: you have a default knowledge box created with your Nuclia account, go to [Nuclia dashboard](https://nuclia.cloud/), the knowledge box ID is indicated on the home page in the **Nuclia APi endpoint**
-- API key: see [how to get an API key](https://docs.nuclia.dev/docs/quick-start/push#get-a-service-access-token)
-- Region: this the geographical region your knowledge box is attached to (at the moment only `europe-1` is supported)
-- Widget ID: see [how to create a widget](https://docs.nuclia.dev/docs/quick-start/search#add-a-search-widget-to-your-website)
+- Knowledge box ID: you have a default knowledge box created with your Nuclia account, go to [Nuclia dashboard](https://nuclia.cloud/), the knowledge box ID is indicated on the home page in the **Nuclia APi endpoint**.
+- API key: see [how to get an API key](https://docs.nuclia.dev/docs/guides/getting-started/quick-start/push#get-an-api-key).
+- Region: this the geographical region your knowledge box is attached to.
+- Widget snippet: see [how to create a widget](https://docs.nuclia.dev/docs/guides/getting-started/quick-start/search#add-a-search-widget-to-your-website).
+- File attribute: the attribute of the content that contains the file to index. Default is `file`.
+- Metadata mapping: Nuclia allows to store the following metadata: `title`, `summary`, `tags`, `contributors`, `created`, `modified`. You can map Plone content fields to these metadata fields. If the field belongs to the parent node, use the following format: `parent/field_name`.
+- Workflow states: you can choose which workflow states trigger indexing in Nuclia. Default is `published`.
 
 ## Usage
 
-Everytime a `File` or a `Link` content is created, it is indexed in Nuclia.
+Everytime a content having a file is created or modified (and if it is in the appropriate workflow state).
 
 The Nuclia search widget is visible on the `/@@nuclia-search` view.
 
 
 Contributors
 ============
 
 - Eric BREHAULT, ebrehault@gmail.com
 
 
 Changelog
 =========
 
+1.0b1 (2024-05-24)
+------------------
+
+- Allow to re-index all files
+  [ebrehault]
+
+- Support different field name for the file content, and allow to map metadata fields
+  [ebrehault]
+
+- Compliancy with Plone 5.1
+  [ebrehault]
+
+- Allow to re-index all files
+  [ebrehault]
+
 
 1.0a3 (2022-10-10)
 ------------------
 
 - Fix project metadata.
   [ebrehault]
```

### Comparing `nuclia.plone-1.0a3/src/nuclia.plone.egg-info/SOURCES.txt` & `nuclia.plone-1.0b1/src/nuclia.plone.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,23 @@
 src/nuclia.plone.egg-info/not-zip-safe
 src/nuclia.plone.egg-info/requires.txt
 src/nuclia.plone.egg-info/top_level.txt
 src/nuclia/plone/__init__.py
 src/nuclia/plone/configure.zcml
 src/nuclia/plone/events.py
 src/nuclia/plone/interfaces.py
+src/nuclia/plone/nuclia_api.py
 src/nuclia/plone/permissions.zcml
 src/nuclia/plone/settings.py
 src/nuclia/plone/setuphandlers.py
 src/nuclia/plone/testing.py
 src/nuclia/plone/browser/__init__.py
 src/nuclia/plone/browser/configure.zcml
-src/nuclia/plone/browser/extract.py
+src/nuclia/plone/browser/reindex.pt
+src/nuclia/plone/browser/reindex.py
 src/nuclia/plone/browser/search.pt
 src/nuclia/plone/browser/search.py
 src/nuclia/plone/locales/README.rst
 src/nuclia/plone/locales/__init__.py
 src/nuclia/plone/locales/nuclia.plone.pot
 src/nuclia/plone/locales/update.py
 src/nuclia/plone/locales/update.sh
```


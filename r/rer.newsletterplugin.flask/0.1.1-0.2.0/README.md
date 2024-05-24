# Comparing `tmp/rer.newsletterplugin.flask-0.1.1.tar.gz` & `tmp/rer.newsletterplugin.flask-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rer.newsletterplugin.flask-0.1.1.tar", last modified: Sat May  4 20:44:15 2024, max compression
+gzip compressed data, was "rer.newsletterplugin.flask-0.2.0.tar", last modified: Fri May 24 14:32:28 2024, max compression
```

## Comparing `rer.newsletterplugin.flask-0.1.1.tar` & `rer.newsletterplugin.flask-0.2.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.453294 rer.newsletterplugin.flask-0.1.1/
--rw-r--r--   0 cekk       (501) staff       (20)     1926 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/.gitlab-ci.yml
--rw-r--r--   0 cekk       (501) staff       (20)     1213 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/.travis.yml
--rw-r--r--   0 cekk       (501) staff       (20)      171 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/CHANGES.rst
--rw-r--r--   0 cekk       (501) staff       (20)       62 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/CONTRIBUTORS.rst
--rw-r--r--   0 cekk       (501) staff       (20)      586 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/DEVELOP.rst
--rw-r--r--   0 cekk       (501) staff       (20)    18092 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      666 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/LICENSE.rst
--rw-r--r--   0 cekk       (501) staff       (20)      102 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)     4116 2024-05-04 20:44:15.453361 rer.newsletterplugin.flask-0.1.1/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     2600 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)       27 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/constraints.txt
--rw-r--r--   0 cekk       (501) staff       (20)      105 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/constraints_plone51.txt
--rw-r--r--   0 cekk       (501) staff       (20)      105 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/constraints_plone52.txt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.446434 rer.newsletterplugin.flask-0.1.1/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     7913 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/docs/conf.py
--rw-r--r--   0 cekk       (501) staff       (20)      101 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/docs/index.rst
--rw-r--r--   0 cekk       (501) staff       (20)    32560 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/docs/rer-logo.png
--rw-r--r--   0 cekk       (501) staff       (20)     1835 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/publiccode.yml
--rw-r--r--   0 cekk       (501) staff       (20)       50 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/requirements.txt
--rw-r--r--   0 cekk       (501) staff       (20)      321 2024-05-04 20:44:15.453689 rer.newsletterplugin.flask-0.1.1/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     2831 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.442757 rer.newsletterplugin.flask-0.1.1/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.446594 rer.newsletterplugin.flask-0.1.1/src/rer/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.447884 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.448663 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/
--rw-r--r--   0 cekk       (501) staff       (20)      215 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.449049 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/adapter/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/adapter/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      446 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/adapter/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     7054 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/adapter/flask_adapter.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.449433 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/browser/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/browser/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      568 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/browser/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      807 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/browser/sendmessageview.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.449689 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/browser/templates/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/browser/templates/.gitkeep
--rw-r--r--   0 cekk       (501) staff       (20)     1366 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/browser/templates/sendmessageview.pt
--rw-r--r--   0 cekk       (501) staff       (20)     1475 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      806 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/interfaces.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.450333 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/
--rw-r--r--   0 cekk       (501) staff       (20)      611 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.443347 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/en/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.450616 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/en/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)      458 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/en/LC_MESSAGES/rer.newsletterplugin.flask.mo
--rw-r--r--   0 cekk       (501) staff       (20)     1819 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/en/LC_MESSAGES/rer.newsletterplugin.flask.po
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.443473 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/it/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.450897 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     1118 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/it/LC_MESSAGES/rer.newsletterplugin.flask.mo
--rw-r--r--   0 cekk       (501) staff       (20)     2306 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/it/LC_MESSAGES/rer.newsletterplugin.flask.po
--rw-r--r--   0 cekk       (501) staff       (20)     1951 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/rer.newsletterplugin.flask.pot
--rw-r--r--   0 cekk       (501) staff       (20)     1599 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/update.py
--rwxr-xr-x   0 cekk       (501) staff       (20)      515 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/update.sh
--rw-r--r--   0 cekk       (501) staff       (20)      260 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/permissions.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.443683 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.451575 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      203 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      105 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/profiles/default/catalog.xml
--rw-r--r--   0 cekk       (501) staff       (20)      182 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/profiles/default/metadata.xml
--rw-r--r--   0 cekk       (501) staff       (20)      242 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/profiles/default/registry.xml
--rw-r--r--   0 cekk       (501) staff       (20)      118 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/profiles/default/rolemap.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.451859 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      136 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      255 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/profiles/uninstall/registry.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.452119 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/services/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/services/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      199 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/services/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.452492 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/services/send_complete/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/services/send_complete/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      350 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/services/send_complete/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     2444 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/services/send_complete/post.py
--rw-r--r--   0 cekk       (501) staff       (20)      627 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/setuphandlers.py
--rw-r--r--   0 cekk       (501) staff       (20)     2626 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.453157 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/tests/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     2603 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/tests/test_send_adapter.py
--rw-r--r--   0 cekk       (501) staff       (20)     3362 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/tests/test_send_complete.py
--rw-r--r--   0 cekk       (501) staff       (20)     5887 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/tests/test_send_to_queue.py
--rw-r--r--   0 cekk       (501) staff       (20)     2624 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/tests/test_setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-04 20:44:15.447717 rer.newsletterplugin.flask-0.1.1/src/rer.newsletterplugin.flask.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)     4116 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer.newsletterplugin.flask.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     3118 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer.newsletterplugin.flask.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer.newsletterplugin.flask.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)      131 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer.newsletterplugin.flask.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)       25 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer.newsletterplugin.flask.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer.newsletterplugin.flask.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      226 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer.newsletterplugin.flask.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)        4 2024-05-04 20:44:15.000000 rer.newsletterplugin.flask-0.1.1/src/rer.newsletterplugin.flask.egg-info/top_level.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.345919 rer.newsletterplugin.flask-0.2.0/
+-rw-r--r--   0 cekk       (501) staff       (20)     1926 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/.gitlab-ci.yml
+-rw-r--r--   0 cekk       (501) staff       (20)     1213 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/.travis.yml
+-rw-r--r--   0 cekk       (501) staff       (20)      240 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       62 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      586 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/DEVELOP.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      666 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      102 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)     4185 2024-05-24 14:32:28.345976 rer.newsletterplugin.flask-0.2.0/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     2600 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       27 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/constraints.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/constraints_plone51.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/constraints_plone52.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.339592 rer.newsletterplugin.flask-0.2.0/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     7913 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/docs/conf.py
+-rw-r--r--   0 cekk       (501) staff       (20)      101 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/docs/index.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    32560 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/docs/rer-logo.png
+-rw-r--r--   0 cekk       (501) staff       (20)     1835 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/publiccode.yml
+-rw-r--r--   0 cekk       (501) staff       (20)       50 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/requirements.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      321 2024-05-24 14:32:28.346264 rer.newsletterplugin.flask-0.2.0/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     2831 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.336417 rer.newsletterplugin.flask-0.2.0/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.339727 rer.newsletterplugin.flask-0.2.0/src/rer/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.340829 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.341559 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/
+-rw-r--r--   0 cekk       (501) staff       (20)      215 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.341910 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/adapter/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/adapter/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      446 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/adapter/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     7448 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/adapter/flask_adapter.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.342269 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      568 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      807 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/browser/sendmessageview.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.342501 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/browser/templates/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/browser/templates/.gitkeep
+-rw-r--r--   0 cekk       (501) staff       (20)     1366 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/browser/templates/sendmessageview.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     1475 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      806 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.343105 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      611 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/locales/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/locales/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.336950 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/locales/en/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.343361 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/locales/en/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)      458 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/locales/en/LC_MESSAGES/rer.newsletterplugin.flask.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     1819 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/locales/en/LC_MESSAGES/rer.newsletterplugin.flask.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.337068 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.343615 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     1118 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/locales/it/LC_MESSAGES/rer.newsletterplugin.flask.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     2306 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/locales/it/LC_MESSAGES/rer.newsletterplugin.flask.po
+-rw-r--r--   0 cekk       (501) staff       (20)     1951 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/locales/rer.newsletterplugin.flask.pot
+-rw-r--r--   0 cekk       (501) staff       (20)     1599 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/locales/update.py
+-rwxr-xr-x   0 cekk       (501) staff       (20)      515 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/locales/update.sh
+-rw-r--r--   0 cekk       (501) staff       (20)      260 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/permissions.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.337255 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.344217 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      203 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/profiles/default/catalog.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      182 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/profiles/default/metadata.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      242 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/profiles/default/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      118 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/profiles/default/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.344463 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      136 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      255 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/profiles/uninstall/registry.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.344680 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/services/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/services/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      199 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/services/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.345030 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/services/send_complete/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/services/send_complete/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      350 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/services/send_complete/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     2444 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/services/send_complete/post.py
+-rw-r--r--   0 cekk       (501) staff       (20)      627 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2626 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.345770 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/tests/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2603 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/tests/test_send_adapter.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3362 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/tests/test_send_complete.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5887 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/tests/test_send_to_queue.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2624 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/tests/test_setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-24 14:32:28.340706 rer.newsletterplugin.flask-0.2.0/src/rer.newsletterplugin.flask.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)     4185 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer.newsletterplugin.flask.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     3118 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer.newsletterplugin.flask.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer.newsletterplugin.flask.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      131 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer.newsletterplugin.flask.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       25 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer.newsletterplugin.flask.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer.newsletterplugin.flask.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      226 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer.newsletterplugin.flask.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        4 2024-05-24 14:32:28.000000 rer.newsletterplugin.flask-0.2.0/src/rer.newsletterplugin.flask.egg-info/top_level.txt
```

### Comparing `rer.newsletterplugin.flask-0.1.1/.gitlab-ci.yml` & `rer.newsletterplugin.flask-0.2.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/.travis.yml` & `rer.newsletterplugin.flask-0.2.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/DEVELOP.rst` & `rer.newsletterplugin.flask-0.2.0/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/LICENSE.GPL` & `rer.newsletterplugin.flask-0.2.0/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/LICENSE.rst` & `rer.newsletterplugin.flask-0.2.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/PKG-INFO` & `rer.newsletterplugin.flask-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rer.newsletterplugin.flask
-Version: 0.1.1
+Version: 0.2.0
 Summary: Add-on per Plone collegato a rer.newsletter per inviare le mail usando un servizio Flask
 Home-page: https://github.com/collective/rer.newsletterplugin.flask
 Author: RedTurtle
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/rer.newsletterplugin.flask
 Project-URL: Source, https://github.com/collective/rer.newsletterplugin.flask
@@ -122,14 +122,19 @@
 
 - RedTurtle, sviluppo@redturtle.it
 
 
 Changelog
 =========
 
+0.2.0 (2024-05-24)
+------------------
+
+- Fix volto support.
+  [cekk]
 
 0.1.1 (2024-05-04)
 ------------------
 
 - Fix python version for Plone6.
   [cekk]
```

### Comparing `rer.newsletterplugin.flask-0.1.1/README.rst` & `rer.newsletterplugin.flask-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/docs/conf.py` & `rer.newsletterplugin.flask-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/docs/rer-logo.png` & `rer.newsletterplugin.flask-0.2.0/docs/rer-logo.png`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/publiccode.yml` & `rer.newsletterplugin.flask-0.2.0/publiccode.yml`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/setup.py` & `rer.newsletterplugin.flask-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="rer.newsletterplugin.flask",
-    version="0.1.1",
+    version="0.2.0",
     description="Add-on per Plone collegato a rer.newsletter per inviare le mail usando un servizio Flask",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/adapter/flask_adapter.py` & `rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/adapter/flask_adapter.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,68 +18,63 @@
 from requests.exceptions import ConnectionError
 from requests.exceptions import Timeout
 
 import json
 import re
 import requests
 
-SUBSCRIBERS_KEY = 'rer.newsletter.subscribers'
-HISTORY_KEY = 'rer.newsletter.channel.history'
+SUBSCRIBERS_KEY = "rer.newsletter.subscribers"
+HISTORY_KEY = "rer.newsletter.channel.history"
 
 
 @implementer(IChannelSender)
 class FlaskAdapter(BaseAdapter):
-    """ Adapter per l'invio delle newsletter fuori da
-    """
+    """Adapter per l'invio delle newsletter fuori da"""
 
     def __init__(self, context, request):
         self.context = context
         self.request = request
 
     def sendMessage(self, message):
-        logger.debug(
-            'adapter: sendMessage %s %s', self.context.title, message.title
-        )
+        logger.debug("adapter: sendMessage %s %s", self.context.title, message.title)
         queue_endpoint = api.portal.get_registry_record(
-            'queue_endpoint',
+            "queue_endpoint",
             interface=INewsletterPluginFlaskSettings,
-            default=u'',
+            default="",
         )
         if not queue_endpoint:
             api.portal.show_message(
                 message=_(
-                    u'endpoint_not_set',
-                    default=u'Queue endpoint not set. Please set it in site controlpanel.',  # noqa
+                    "endpoint_not_set",
+                    default="Queue endpoint not set. Please set it in site controlpanel.",  # noqa
                 ),
                 request=self.context.REQUEST,
-                type='error',
+                type="error",
             )
             return NOK
         # Costruzione del messaggio: body, subject, destinatari, ...
         subscribers = self.get_annotations_for_channel(key=SUBSCRIBERS_KEY)
         recipients = []
         for user in subscribers.keys():
-            if subscribers[user]['is_active']:
-                recipients.append(subscribers[user]['email'])
+            if subscribers[user]["is_active"]:
+                recipients.append(subscribers[user]["email"])
 
         if not recipients:
             api.portal.show_message(
                 message=_(
-                    u'recipients_empty',
-                    default=u'There are 0 subscribers to this channel.',
+                    "recipients_empty",
+                    default="There are 0 subscribers to this channel.",
                 ),
                 request=self.context.REQUEST,
-                type='error',
+                type="error",
             )
             return NOK
 
         nl_subject = (
-            ' - ' + self.context.subject_email
-            if self.context.subject_email
-            else u''
+            " - " + self.context.subject_email if self.context.subject_email else ""
         )
 
         sender = (
             self.context.sender_name
             and formataddr(  # noqa
                 (self.context.sender_name, self.context.sender_email)
             )
@@ -89,20 +84,20 @@
 
         send_uid = self.set_start_send_infos(message=message)
 
         # Preparazione della request con il vero payload e l'header
         body = self.prepare_body(message=message)
         headers = {"Content-Type": "application/json"}
         payload = {
-            'channel_url': self.convert_url(self.context.absolute_url()),
-            'subscribers': recipients,
-            'subject': subject,
-            'mfrom': sender,
-            'text': body.getData(),
-            'send_uid': send_uid,
+            "channel_url": self.convert_url(self.context.absolute_url()),
+            "subscribers": recipients,
+            "subject": subject,
+            "mfrom": sender,
+            "text": body.getData(),
+            "send_uid": send_uid,
         }
         try:
             response = requests.post(
                 queue_endpoint, data=json.dumps(payload), headers=headers
             )
         except (ConnectionError, Timeout) as e:
             logger.exception(e)
@@ -117,24 +112,35 @@
                 )
             )
             return UNHANDLED
 
         return OK
 
     def convert_url(self, url):
-        source_link = api.portal.get_registry_record(
-            'source_link', ISettingsSchema
-        )
+
+        # If volto frontend_domain is set, use it as destination link
+        try:
+            destination_link = api.portal.get_registry_record(
+                "volto.frontend_domain", default=""
+            )
+            if destination_link.endswith("/"):
+                destination_link = destination_link[:-1]
+            destination_link += "/++api++"
+        except KeyError:
+            destination_link = ""
+        if not destination_link:
+            # otherwise, use the newsletter one
+            destination_link = api.portal.get_registry_record(
+                "destination_link", ISettingsSchema
+            )
+
+        source_link = api.portal.get_registry_record("source_link", ISettingsSchema)
         if not source_link:
             source_link = api.portal.get().absolute_url()
 
-        destination_link = api.portal.get_registry_record(
-            'destination_link', ISettingsSchema
-        )
-
         # non è questo il modo migliore per fare il replace...
         # 1. non serve usare re.sub ma basta il replace di string
         # 2. forse sarebbe più corretto usare un metodo di lxml
         if source_link and destination_link:
             return re.sub(source_link, destination_link, url)
         return url
 
@@ -142,54 +148,52 @@
         res = super(FlaskAdapter, self).set_end_send_infos(
             send_uid=send_uid, completed=completed
         )
         self._sendNotification(status=completed, send_uid=send_uid)
         return res
 
     def _sendNotification(self, status, send_uid):
-        """ send notification to user when asynch call is finished """
+        """send notification to user when asynch call is finished"""
         portal = api.portal.get()
         channel = self.context
         details = self.get_annotations_for_channel(key=HISTORY_KEY)
-        send_info = [x for x in details if x['uid'] == send_uid][0]
+        send_info = [x for x in details if x["uid"] == send_uid][0]
 
         if channel.sender_email:
             message_template = None
             if status:
                 message_template = self.context.restrictedTraverse(
-                    '@@{0}'.format('asynch_send_success')
+                    "@@{0}".format("asynch_send_success")
                 )
             else:
                 message_template = self.context.restrictedTraverse(
-                    '@@{0}'.format('asynch_send_fail')
+                    "@@{0}".format("asynch_send_fail")
                 )
             parameters = {
-                'header': channel.header.output if channel.header else u'',
-                'footer': channel.footer.output if channel.footer else u'',
-                'style': channel.css_style if channel.css_style else u'',
-                'portal_name': portal.title,
-                'channel_name': channel.title,
-                'subscribers': send_info.get('subscribers', ''),
-                'message_title': send_info.get('message', ''),
+                "header": channel.header.output if channel.header else "",
+                "footer": channel.footer.output if channel.footer else "",
+                "style": channel.css_style if channel.css_style else "",
+                "portal_name": portal.title,
+                "channel_name": channel.title,
+                "subscribers": send_info.get("subscribers", ""),
+                "message_title": send_info.get("message", ""),
             }
             mail_text = message_template(**parameters)
-            mail_text = portal.portal_transforms.convertTo(
-                'text/mail', mail_text
-            )
+            mail_text = portal.portal_transforms.convertTo("text/mail", mail_text)
 
-            subject = u'Risultato invio di {0} del {1} del '.format(
-                send_info.get('message', ''), channel.title
-            ) + u'portale {0}'.format(get_site_title())
+            subject = "Risultato invio di {0} del {1} del ".format(
+                send_info.get("message", ""), channel.title
+            ) + "portale {0}".format(get_site_title())
 
             sender = compose_sender(self.context)
 
-            mail_host = api.portal.get_tool(name='MailHost')
+            mail_host = api.portal.get_tool(name="MailHost")
             mail_host.send(
                 mail_text.getData(),
                 mto=channel.sender_email,
                 mfrom=sender,
                 subject=subject,
-                charset='utf-8',
-                msg_type='text/html',
+                charset="utf-8",
+                msg_type="text/html",
             )
         else:
-            logger.exception('Non è stato impostato l\'indirizzo del mittente')
+            logger.exception("Non è stato impostato l'indirizzo del mittente")
```

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/browser/configure.zcml` & `rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/browser/sendmessageview.py` & `rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/browser/sendmessageview.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/browser/templates/sendmessageview.pt` & `rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/browser/templates/sendmessageview.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/configure.zcml` & `rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/interfaces.py` & `rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/interfaces.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/README.rst` & `rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/locales/README.rst`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/en/LC_MESSAGES/rer.newsletterplugin.flask.po` & `rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/locales/en/LC_MESSAGES/rer.newsletterplugin.flask.po`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/it/LC_MESSAGES/rer.newsletterplugin.flask.mo` & `rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/locales/it/LC_MESSAGES/rer.newsletterplugin.flask.mo`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/it/LC_MESSAGES/rer.newsletterplugin.flask.po` & `rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/locales/it/LC_MESSAGES/rer.newsletterplugin.flask.po`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/rer.newsletterplugin.flask.pot` & `rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/locales/rer.newsletterplugin.flask.pot`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/update.py` & `rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/locales/update.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/locales/update.sh` & `rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/locales/update.sh`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/services/send_complete/post.py` & `rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/services/send_complete/post.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/setuphandlers.py` & `rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/testing.py` & `rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/testing.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/tests/test_send_adapter.py` & `rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/tests/test_send_adapter.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/tests/test_send_complete.py` & `rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/tests/test_send_complete.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/tests/test_send_to_queue.py` & `rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/tests/test_send_to_queue.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer/newsletterplugin/flask/tests/test_setup.py` & `rer.newsletterplugin.flask-0.2.0/src/rer/newsletterplugin/flask/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer.newsletterplugin.flask.egg-info/PKG-INFO` & `rer.newsletterplugin.flask-0.2.0/src/rer.newsletterplugin.flask.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rer.newsletterplugin.flask
-Version: 0.1.1
+Version: 0.2.0
 Summary: Add-on per Plone collegato a rer.newsletter per inviare le mail usando un servizio Flask
 Home-page: https://github.com/collective/rer.newsletterplugin.flask
 Author: RedTurtle
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/rer.newsletterplugin.flask
 Project-URL: Source, https://github.com/collective/rer.newsletterplugin.flask
@@ -122,14 +122,19 @@
 
 - RedTurtle, sviluppo@redturtle.it
 
 
 Changelog
 =========
 
+0.2.0 (2024-05-24)
+------------------
+
+- Fix volto support.
+  [cekk]
 
 0.1.1 (2024-05-04)
 ------------------
 
 - Fix python version for Plone6.
   [cekk]
```

### Comparing `rer.newsletterplugin.flask-0.1.1/src/rer.newsletterplugin.flask.egg-info/SOURCES.txt` & `rer.newsletterplugin.flask-0.2.0/src/rer.newsletterplugin.flask.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/Products.MeetingNamur-4.2.0rc3.tar.gz` & `tmp/Products.MeetingNamur-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Products.MeetingNamur-4.2.0rc3.tar", last modified: Thu Sep 28 08:15:28 2023, max compression
+gzip compressed data, was "Products.MeetingNamur-4.2.1.tar", last modified: Fri May 24 14:19:16 2024, max compression
```

## Comparing `Products.MeetingNamur-4.2.0rc3.tar` & `Products.MeetingNamur-4.2.1.tar`

### file list

```diff
@@ -1,189 +1,190 @@
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.957358 Products.MeetingNamur-4.2.0rc3/
--rw-rw-r--   0 adu       (1000) adu       (1000)     5544 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/CHANGES.rst
--rw-rw-r--   0 adu       (1000) adu       (1000)      679 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/MANIFEST.in
--rw-rw-r--   0 adu       (1000) adu       (1000)     6216 2023-09-28 08:15:28.957358 Products.MeetingNamur-4.2.0rc3/PKG-INFO
--rw-rw-r--   0 adu       (1000) adu       (1000)      148 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/README.rst
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/docs/
--rw-rw-r--   0 adu       (1000) adu       (1000)    18092 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/docs/LICENSE.GPL
--rw-rw-r--   0 adu       (1000) adu       (1000)      731 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/docs/LICENSE.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)       38 2023-09-28 08:15:28.957358 Products.MeetingNamur-4.2.0rc3/setup.cfg
--rw-rw-r--   0 adu       (1000) adu       (1000)     1465 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/setup.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/src/
--rw-rw-r--   0 adu       (1000) adu       (1000)       76 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/EXTERNALS.txt
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/src/Products/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/Extensions/
--rw-rw-r--   0 adu       (1000) adu       (1000)       26 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/Extensions/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      964 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/README.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)     1751 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)    31247 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/adapters.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/browser/
--rw-rw-r--   0 adu       (1000) adu       (1000)       22 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/browser/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      562 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/browser/configure.zcml
--rw-rw-r--   0 adu       (1000) adu       (1000)     6239 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/browser/itemcertifiedsignatures.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      120 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/browser/overrides.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/browser/templates/
--rw-rw-r--   0 adu       (1000) adu       (1000)       73 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/browser/templates/display_certified_signatures.pt
--rw-rw-r--   0 adu       (1000) adu       (1000)     3116 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/config.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     3773 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/configure.zcml
--rw-rw-r--   0 adu       (1000) adu       (1000)     1361 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/events.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      674 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/events.zcml
--rw-rw-r--   0 adu       (1000) adu       (1000)     4083 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/interfaces.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/
--rw-rw-r--   0 adu       (1000) adu       (1000)     5058 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/PloneMeeting.pot
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.937356 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/de/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/de/LC_MESSAGES/
--rw-rw-r--   0 adu       (1000) adu       (1000)     5541 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/de/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     1666 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.actionspanel.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     1860 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     3371 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/de/LC_MESSAGES/plone.po
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.937356 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/en/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/en/LC_MESSAGES/
--rw-rw-r--   0 adu       (1000) adu       (1000)     5498 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/en/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     1661 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.actionspanel.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     1893 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     3234 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/en/LC_MESSAGES/plone.po
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.937356 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/es/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/es/LC_MESSAGES/
--rw-rw-r--   0 adu       (1000) adu       (1000)     5772 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/es/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     1890 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.actionspanel.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     1860 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     3663 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/es/LC_MESSAGES/plone.po
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.937356 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/fr/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 adu       (1000) adu       (1000)     8489 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     2299 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.actionspanel.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     2397 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     4133 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     1400 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/imio.actionspanel.pot
--rw-rw-r--   0 adu       (1000) adu       (1000)     1721 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/imio.history.pot
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.937356 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/nl/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/
--rw-rw-r--   0 adu       (1000) adu       (1000)     5412 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     1575 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.actionspanel.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     1860 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     3287 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/plone.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     2850 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/plone.pot
--rwxrwxr-x   0 adu       (1000) adu       (1000)      307 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/sync_pos.sh
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/migrations/
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/migrations/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     5060 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/migrations/migrate_to_4200.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      976 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/migrations/migrate_to_4_1.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/model/
--rw-rw-r--   0 adu       (1000) adu       (1000)       23 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/model/__init__.py
--rwxrwxr-x   0 adu       (1000) adu       (1000)      305 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/model/generate.sh
--rw-rw-r--   0 adu       (1000) adu       (1000)     4280 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/model/pm_updates.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      405 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/overrides.zcml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/__init__.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/
--rw-rw-r--   0 adu       (1000) adu       (1000)      177 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/MeetingNamur_marker.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      709 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/cssregistry.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)     1421 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/import_steps.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      423 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/jsregistry.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      104 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/metadata.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      600 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/rolemap.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      890 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/skins.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      167 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/toolset.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.937356 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/workflows/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/workflows/meetingitemnamur_workflow/
--rw-rw-r--   0 adu       (1000) adu       (1000)    58818 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/workflows/meetingitemnamur_workflow/definition.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/workflows/meetingnamur_workflow/
--rw-rw-r--   0 adu       (1000) adu       (1000)    10860 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/workflows/meetingnamur_workflow/definition.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      885 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/workflows.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/
--rw-rw-r--   0 adu       (1000) adu       (1000)      177 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/MeetingNamur_examples_fr_marker.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/__init__.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.953358 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/
--rw-rw-r--   0 adu       (1000) adu       (1000)     3352 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/attach.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      630 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/budget.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      492 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/budgetAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)     1032 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.gif
--rw-rw-r--   0 adu       (1000) adu       (1000)      731 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/decisionAnnex.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      742 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/financialAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/itemAnnex.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      761 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/legalAdvice.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      332 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/legalAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      885 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/negative.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      305 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/nil.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      880 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/overheadAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)     1147 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/positive.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      355 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/remarks.png
--rw-rw-r--   0 adu       (1000) adu       (1000)     1663 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/import_data.py
--rwxrwxr-x   0 adu       (1000) adu       (1000)      898 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/import_steps.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.953358 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/templates/
--rwxrwxr-x   0 adu       (1000) adu       (1000)   104980 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/templates/Agenda.odt
--rwxrwxr-x   0 adu       (1000) adu       (1000)    37100 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/templates/Decisions.odt
--rwxrwxr-x   0 adu       (1000) adu       (1000)    34356 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/templates/Item.odt
--rwxrwxr-x   0 adu       (1000) adu       (1000)      167 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/toolset.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.953358 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/
--rw-rw-r--   0 adu       (1000) adu       (1000)      177 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/MeetingNamur_tests_marker.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/__init__.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.953358 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/images/
--rw-rw-r--   0 adu       (1000) adu       (1000)     3352 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/images/attach.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      630 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/images/budget.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      492 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/images/budgetAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      731 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/images/cahier.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/images/decisionAnnex.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      742 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/images/financialAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/images/itemAnnex.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      332 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/images/legalAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      411 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/images/negative.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      880 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/images/overheadAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)     1147 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/images/positive.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      355 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/images/remarks.png
--rw-rw-r--   0 adu       (1000) adu       (1000)     1585 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/import_data.py
--rwxrwxr-x   0 adu       (1000) adu       (1000)      327 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/import_steps.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      171 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/metadata.xml
--rwxrwxr-x   0 adu       (1000) adu       (1000)      167 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/toolset.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)     1269 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles.zcml
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/refresh.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)     4488 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/setuphandlers.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/skins/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.953358 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/skins/meetingnamur_images/
--rw-rw-r--   0 adu       (1000) adu       (1000)      657 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/skins/meetingnamur_images/isConfidentialYes.png
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.953358 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/skins/meetingnamur_styles/
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/skins/meetingnamur_styles/meetingnamur.css
--rw-rw-r--   0 adu       (1000) adu       (1000)      348 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/skins/meetingnamur_styles/readme.txt
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.953358 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/skins/meetingnamur_templates/
--rw-rw-r--   0 adu       (1000) adu       (1000)    11157 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_edit.pt
--rw-rw-r--   0 adu       (1000) adu       (1000)    42870 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_view.pt
--rw-rw-r--   0 adu       (1000) adu       (1000)     1102 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/testing.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      597 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/testing.zcml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.957358 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/
--rwxrwxr-x   0 adu       (1000) adu       (1000)     1610 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/MeetingNamurTestCase.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1292 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1243 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/helpers.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     9893 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testAdvices.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     3710 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testAnnexes.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1326 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testChangeItemOrderView.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1217 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testColumns.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1342 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testContacts.py
--rwxrwxr-x   0 adu       (1000) adu       (1000)     3088 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testCustomMeeting.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     5114 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testCustomMeetingItem.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1250 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testFaceted.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      507 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testMeeting.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1303 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testMeetingCategory.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1445 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testMeetingConfig.py
--rwxrwxr-x   0 adu       (1000) adu       (1000)     7541 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testMeetingItem.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1263 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testPortlets.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     2204 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testSearches.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1254 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testSetup.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1307 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testToolPloneMeeting.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1207 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testUtils.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1266 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testValidators.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      442 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testViews.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     3458 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testWFAdaptations.py
--rwxrwxr-x   0 adu       (1000) adu       (1000)     6685 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testWorkflows.py
--rw-rw-r--   0 adu       (1000) adu       (1000)        8 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/version.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)       56 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products/__init__.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-09-28 08:15:28.945357 Products.MeetingNamur-4.2.0rc3/src/Products.MeetingNamur.egg-info/
--rw-rw-r--   0 adu       (1000) adu       (1000)     6216 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products.MeetingNamur.egg-info/PKG-INFO
--rw-rw-r--   0 adu       (1000) adu       (1000)     8265 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products.MeetingNamur.egg-info/SOURCES.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        1 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products.MeetingNamur.egg-info/dependency_links.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        9 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products.MeetingNamur.egg-info/namespace_packages.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        1 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products.MeetingNamur.egg-info/not-zip-safe
--rw-rw-r--   0 adu       (1000) adu       (1000)      284 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products.MeetingNamur.egg-info/requires.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        9 2023-09-28 08:15:28.000000 Products.MeetingNamur-4.2.0rc3/src/Products.MeetingNamur.egg-info/top_level.txt
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.775189 Products.MeetingNamur-4.2.1/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5787 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/CHANGES.rst
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      679 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/MANIFEST.in
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     6436 2024-05-24 14:19:16.775189 Products.MeetingNamur-4.2.1/PKG-INFO
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      148 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/README.rst
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.771190 Products.MeetingNamur-4.2.1/docs/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    18092 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/docs/LICENSE.GPL
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      731 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/docs/LICENSE.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       38 2024-05-24 14:19:16.775189 Products.MeetingNamur-4.2.1/setup.cfg
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1462 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/setup.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.771190 Products.MeetingNamur-4.2.1/src/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       76 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/EXTERNALS.txt
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.771190 Products.MeetingNamur-4.2.1/src/Products/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.772189 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.772189 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/Extensions/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       26 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/Extensions/__init__.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      964 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/README.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1751 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/__init__.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    31393 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/adapters.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.772189 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/browser/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       22 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/browser/__init__.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      562 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/browser/configure.zcml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     6239 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/browser/itemcertifiedsignatures.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      120 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/browser/overrides.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.772189 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/browser/templates/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       73 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/browser/templates/display_certified_signatures.pt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3116 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/config.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3773 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/configure.zcml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1361 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/events.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      674 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/events.zcml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4083 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/interfaces.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.772189 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5058 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/PloneMeeting.pot
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.770190 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/de/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.772189 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5541 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/PloneMeeting.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1666 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.actionspanel.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1860 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.history.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3371 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/plone.po
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.770190 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/en/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.772189 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5498 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/PloneMeeting.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1661 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.actionspanel.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1893 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.history.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3234 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/plone.po
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.770190 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/es/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.772189 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5772 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/PloneMeeting.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1890 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.actionspanel.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1860 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.history.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3663 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/plone.po
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.770190 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/fr/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.772189 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     8489 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/PloneMeeting.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2299 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.actionspanel.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2397 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.history.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4133 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/plone.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1400 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/imio.actionspanel.pot
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1721 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/imio.history.pot
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.770190 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/nl/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.772189 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5412 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/PloneMeeting.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1575 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.actionspanel.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1860 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.history.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3287 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/plone.po
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2850 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/plone.pot
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      307 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/sync_pos.sh
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.773190 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/migrations/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/migrations/__init__.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5062 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/migrations/migrate_to_4200.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2240 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/migrations/migrate_to_4201.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      976 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/migrations/migrate_to_4_1.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.773190 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/model/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       23 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/model/__init__.py
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      305 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/model/generate.sh
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4279 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/model/pm_updates.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      405 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/overrides.zcml
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.773190 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/__init__.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.773190 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      177 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/MeetingNamur_marker.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/__init__.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      709 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/cssregistry.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1421 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/import_steps.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      423 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/jsregistry.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      104 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/metadata.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      600 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/rolemap.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      890 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/skins.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      167 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/toolset.xml
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.770190 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/workflows/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.773190 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/workflows/meetingitemnamur_workflow/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    58818 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/workflows/meetingitemnamur_workflow/definition.xml
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.773190 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/workflows/meetingnamur_workflow/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    10860 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/workflows/meetingnamur_workflow/definition.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      885 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/workflows.xml
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.773190 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      177 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/MeetingNamur_examples_fr_marker.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/__init__.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.774190 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3352 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/attach.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      630 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/budget.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      492 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/budgetAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1032 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.gif
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      731 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      216 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/decisionAnnex.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      742 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/financialAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      216 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/itemAnnex.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      761 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/legalAdvice.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      332 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/legalAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      885 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/negative.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      305 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/nil.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      880 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/overheadAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1147 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/positive.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      355 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/remarks.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1663 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/import_data.py
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      898 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/import_steps.xml
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.774190 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/templates/
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)   104980 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/templates/Agenda.odt
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)    37100 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/templates/Decisions.odt
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)    34356 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/templates/Item.odt
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      167 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/toolset.xml
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.774190 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      177 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/MeetingNamur_tests_marker.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/__init__.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.774190 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/images/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3352 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/images/attach.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      630 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/images/budget.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      492 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/images/budgetAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      731 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/images/cahier.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      216 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/images/decisionAnnex.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      742 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/images/financialAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      216 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/images/itemAnnex.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      332 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/images/legalAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      411 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/images/negative.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      880 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/images/overheadAnalysis.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1147 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/images/positive.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      355 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/images/remarks.png
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1585 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/import_data.py
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      327 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/import_steps.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      171 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/metadata.xml
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)      167 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/toolset.xml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1537 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles.zcml
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/refresh.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4488 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/setuphandlers.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.771190 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/skins/
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.774190 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/skins/meetingnamur_images/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      657 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/skins/meetingnamur_images/isConfidentialYes.png
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.774190 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/skins/meetingnamur_styles/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/skins/meetingnamur_styles/meetingnamur.css
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      348 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/skins/meetingnamur_styles/readme.txt
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.774190 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/skins/meetingnamur_templates/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    11157 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_edit.pt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    42870 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_view.pt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1102 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/testing.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      597 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/testing.zcml
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.775189 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)     1610 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/MeetingNamurTestCase.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1292 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/__init__.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1243 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/helpers.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     9893 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testAdvices.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3710 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testAnnexes.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1326 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testChangeItemOrderView.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1217 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testColumns.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1342 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testContacts.py
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)     3088 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testCustomMeeting.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5160 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testCustomMeetingItem.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1250 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testFaceted.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      507 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testMeeting.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1303 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testMeetingCategory.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1445 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testMeetingConfig.py
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)     7626 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testMeetingItem.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1263 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testPortlets.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2204 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testSearches.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1254 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testSetup.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1307 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testToolPloneMeeting.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1207 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testUtils.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1266 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testValidators.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      442 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testViews.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     2265 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testWFAdaptations.py
+-rwxr-xr-x   0 duchenean  (1000) duchenean  (1000)     6685 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testWorkflows.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        8 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/version.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       56 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products/__init__.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 14:19:16.771190 Products.MeetingNamur-4.2.1/src/Products.MeetingNamur.egg-info/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     6436 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products.MeetingNamur.egg-info/PKG-INFO
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     8321 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products.MeetingNamur.egg-info/SOURCES.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        1 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products.MeetingNamur.egg-info/dependency_links.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        9 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products.MeetingNamur.egg-info/namespace_packages.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        1 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products.MeetingNamur.egg-info/not-zip-safe
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      271 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products.MeetingNamur.egg-info/requires.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        9 2024-05-24 14:19:16.000000 Products.MeetingNamur-4.2.1/src/Products.MeetingNamur.egg-info/top_level.txt
```

### Comparing `Products.MeetingNamur-4.2.0rc3/CHANGES.rst` & `Products.MeetingNamur-4.2.1/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,29 @@
 Products.MeetingNamur Changelog
 ===============================
 
 Older versions than 3.0 can be found at http://svn.communesplone.org/svn/communesplone/MeetingNamur/tags/
 The Products.MeetingNamur version must be the same as the Products.PloneMeeting version
 
+4.2.1 (2024-05-24)
+------------------
+
+- Cleanup.
+  [gbastien]
+- Migrate `MeetingItem.grpBudgetInfos` to use orgs UIDs.
+  [aduchene]
+
+
+4.2.0 (2024-03-11)
+------------------
+
+- Fixed `MeetingItem.customshowDuplicateItemAction`.
+  [aduchene]
+
+
 4.2.0rc3 (2023-09-28)
 ---------------------
 
 - In `CustomNamurMeetingItem._initDecisionFieldIfEmpty` removed parameter
   `keepWithNext=False` when calling `MeetingItem.getDecision` as it does not
   exist anymore.
   [gbastien]
@@ -17,14 +33,15 @@
 - Fixed `meetingitem_view.pt` as `MeetingItem.isCopiesEnabled` was removed and
   field `MeetingItem.copyGroups` is now an optional field managed by
   `MeetingConfig.usedItemAttributes`.
   [gbastien]
 - `meetingnamur.css` is now completely empty.
   [gbastien]
 
+
 4.2.0rc2 (2023-07-04)
 ---------------------
 
 - Adapt vocabulary and i18n.
   [aduchene]
```

### Comparing `Products.MeetingNamur-4.2.0rc3/MANIFEST.in` & `Products.MeetingNamur-4.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/PKG-INFO` & `Products.MeetingNamur-4.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,50 @@
 Metadata-Version: 2.1
 Name: Products.MeetingNamur
-Version: 4.2.0rc3
+Version: 4.2.1
 Summary: PloneMeeting profile for city of Namur
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: Andre Nuyens
 Author-email: andre.nuyens@imio.be
 License: GPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 4.3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
-Provides-Extra: templates
 Provides-Extra: test
+Provides-Extra: templates
 
 ========================
 Products.MeetingNamur
 ========================
 
 'Products.MeetingNamur' is a custom profile for 'Products.MeetingCommunes'.
 Products.MeetingNamur Changelog
 ===============================
 
 Older versions than 3.0 can be found at http://svn.communesplone.org/svn/communesplone/MeetingNamur/tags/
 The Products.MeetingNamur version must be the same as the Products.PloneMeeting version
 
+4.2.1 (2024-05-24)
+------------------
+
+- Cleanup.
+  [gbastien]
+- Migrate `MeetingItem.grpBudgetInfos` to use orgs UIDs.
+  [aduchene]
+
+
+4.2.0 (2024-03-11)
+------------------
+
+- Fixed `MeetingItem.customshowDuplicateItemAction`.
+  [aduchene]
+
+
 4.2.0rc3 (2023-09-28)
 ---------------------
 
 - In `CustomNamurMeetingItem._initDecisionFieldIfEmpty` removed parameter
   `keepWithNext=False` when calling `MeetingItem.getDecision` as it does not
   exist anymore.
   [gbastien]
@@ -39,14 +54,15 @@
 - Fixed `meetingitem_view.pt` as `MeetingItem.isCopiesEnabled` was removed and
   field `MeetingItem.copyGroups` is now an optional field managed by
   `MeetingConfig.usedItemAttributes`.
   [gbastien]
 - `meetingnamur.css` is now completely empty.
   [gbastien]
 
+
 4.2.0rc2 (2023-07-04)
 ---------------------
 
 - Adapt vocabulary and i18n.
   [aduchene]
 
 
@@ -181,9 +197,7 @@
 - Migrated to Plone 4 (use PloneMeeting 3.x, see PloneMeeting's HISTORY.txt for full changes list)
 
 2.1.3 (2012-09-19)
 ------------------
 - Added possibility to give, modify and view an advice on created item
 - Added possibility to define a decision of replacement when an item is delayed
 - Added new workflow adaptation to add publish state with hidden decision for no meeting-manager
-
-
```

### Comparing `Products.MeetingNamur-4.2.0rc3/docs/LICENSE.GPL` & `Products.MeetingNamur-4.2.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/docs/LICENSE.txt` & `Products.MeetingNamur-4.2.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/setup.py` & `Products.MeetingNamur-4.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import os
 
 
-version = '4.2.0rc3'
+version = '4.2.1'
 
 setup(name='Products.MeetingNamur',
       version=version,
       description="PloneMeeting profile for city of Namur",
       long_description=open("README.rst").read() + "\n" + open("CHANGES.rst").read(),
       classifiers=[
         "Environment :: Web Environment",
```

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/README.txt` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/README.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/__init__.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/adapters.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 # -*- coding: utf-8 -*-
 
 from AccessControl import ClassSecurityInfo
 from AccessControl.class_init import InitializeClass
-from Products.MeetingNamur.config import WriteDecisionProject
-from Products.PloneMeeting.model.adaptations import WF_APPLIED
 from collective.contact.plonegroup.utils import get_organizations
 from collective.contact.plonegroup.utils import get_plone_group_id
 from imio.helpers.cache import get_plone_groups_for_user
 from imio.helpers.xhtml import xhtmlContentIsEmpty
 from plone import api
 from Products.Archetypes.atapi import DisplayList
 from Products.CMFCore.utils import getToolByName
-from Products.MeetingCommunes.adapters import CustomMeeting, CustomMeetingConfig
+from Products.MeetingCommunes.adapters import CustomMeeting
+from Products.MeetingCommunes.adapters import CustomMeetingConfig
 from Products.MeetingCommunes.adapters import CustomMeetingItem
 from Products.MeetingCommunes.adapters import CustomToolPloneMeeting
 from Products.MeetingCommunes.adapters import MeetingCommunesWorkflowActions
 from Products.MeetingCommunes.adapters import MeetingCommunesWorkflowConditions
 from Products.MeetingCommunes.adapters import MeetingItemCommunesWorkflowActions
 from Products.MeetingCommunes.adapters import MeetingItemCommunesWorkflowConditions
+from Products.MeetingNamur.config import WriteDecisionProject
 from Products.MeetingNamur.interfaces import IMeetingItemNamurCollegeWorkflowActions
 from Products.MeetingNamur.interfaces import IMeetingItemNamurCollegeWorkflowConditions
 from Products.MeetingNamur.interfaces import IMeetingItemNamurCouncilWorkflowActions
 from Products.MeetingNamur.interfaces import IMeetingItemNamurCouncilWorkflowConditions
 from Products.MeetingNamur.interfaces import IMeetingItemNamurWorkflowActions
 from Products.MeetingNamur.interfaces import IMeetingItemNamurWorkflowConditions
 from Products.MeetingNamur.interfaces import IMeetingNamurCollegeWorkflowActions
 from Products.MeetingNamur.interfaces import IMeetingNamurCollegeWorkflowConditions
 from Products.MeetingNamur.interfaces import IMeetingNamurCouncilWorkflowActions
 from Products.MeetingNamur.interfaces import IMeetingNamurCouncilWorkflowConditions
 from Products.MeetingNamur.interfaces import IMeetingNamurWorkflowActions
 from Products.MeetingNamur.interfaces import IMeetingNamurWorkflowConditions
 from Products.PloneMeeting.adapters import ItemPrettyLinkAdapter
-from Products.PloneMeeting.interfaces import IMeetingCustom, IMeetingConfigCustom
+from Products.PloneMeeting.config import MEETING_REMOVE_MOG_WFA
+from Products.PloneMeeting.interfaces import IMeetingConfigCustom
+from Products.PloneMeeting.interfaces import IMeetingCustom
 from Products.PloneMeeting.interfaces import IMeetingItemCustom
 from Products.PloneMeeting.interfaces import IToolPloneMeetingCustom
 from Products.PloneMeeting.MeetingConfig import MeetingConfig
 from Products.PloneMeeting.MeetingItem import MeetingItem
 from Products.PloneMeeting.MeetingItem import MeetingItemWorkflowActions
-from Products.PloneMeeting.utils import sendMail, org_id_to_uid
+from Products.PloneMeeting.model.adaptations import WF_APPLIED
+from Products.PloneMeeting.utils import org_id_to_uid
+from Products.PloneMeeting.utils import sendMail
 from zope.i18n import translate
 from zope.interface import implements
 
 
 customWfAdaptations = (
     'item_validation_shortcuts',
     'item_validation_no_validate_shortcuts',
     'only_creator_may_delete',
-    'meeting_remove_global_access',
     'meetingmanager_correct_closed_meeting',
     # first define meeting workflow state removal
     'no_freeze',
     'no_publication',
     'no_decide',
     # then define added item decided states
     'accepted_but_modified',
@@ -70,14 +73,16 @@
     'accepted_out_of_meeting',
     'accepted_out_of_meeting_and_duplicated',
     'accepted_out_of_meeting_emergency',
     'accepted_out_of_meeting_emergency_and_duplicated',
     'transfered',
     'transfered_and_duplicated',
     'namur_meetingmanager_may_not_edit_decision_project',
+    MEETING_REMOVE_MOG_WFA
+
 )
 MeetingConfig.wfAdaptations = customWfAdaptations
 
 
 class CustomNamurMeetingConfig(CustomMeetingConfig):
     implements(IMeetingConfigCustom)
     security = ClassSecurityInfo()
@@ -320,15 +325,15 @@
 
     def listGrpBudgetInfosAdviser(self):
         """Returns a list of groups that can be selected on an item to modify budgetInfos field.
         acronym group start with DGF"""
         res = []
         orgs = get_organizations(not_empty_suffix='budgetimpactreviewers')
         for group in orgs:
-            res.append((group.id, group.getProperty('title')))
+            res.append((group.UID(), group.getProperty('title')))
         return DisplayList(tuple(res))
 
     MeetingItem.listGrpBudgetInfosAdviser = listGrpBudgetInfosAdviser
 
     security.declarePublic('updateMeetingBudgetImpactReviewerRole')
 
     def updateMeetingBudgetImpactReviewerRole(self):
@@ -340,16 +345,15 @@
         grp_uids = []
         if item.query_state() in ('presented', 'itemfrozen', 'accepted', 'delayed', 'accepted_but_modified',
                                   'pre_accepted', 'refused'):
             # add new MeetingBudgetImpactReviewerRole
             for grpBudgetInfo in item.grpBudgetInfos:
                 # for each group_budgetimpactreviewers add new local roles
                 if grpBudgetInfo:
-                    grp_role = '%s_budgetimpactreviewers' % grpBudgetInfo
-                    grp_uid = org_id_to_uid(grp_role)
+                    grp_uid = '%s_budgetimpactreviewers' % grpBudgetInfo
                     grp_uids.append(grp_uid)
                     item.manage_addLocalRoles(grp_uid, ('Reader', 'MeetingBudgetImpactReviewer',))
         # suppress old unused group_budgetimpactreviewers
         toRemove = []
         for user, roles in item.get_local_roles():
             if user.endswith('_budgetimpactreviewers') and user not in grp_uids:
                 toRemove.append(user)
@@ -394,15 +398,15 @@
         # - the user is creator in some group;
         # - the user must be able to see the item if it is private.
         # The user will duplicate the item in his own folder.
         tool = api.portal.get_tool('portal_plonemeeting')
         item = self.getSelf()
         cfg = tool.getMeetingConfig(self)
         ignoreDuplicateButton = item.query_state() == 'pre_accepted'
-        if not cfg.getEnableItemDuplication() or \
+        if 'duplication' not in cfg.getEnabledItemActions() or \
                 self.isDefinedInTool() or \
                 not tool.userIsAmong(['creators']) or \
                 not self.adapted().isPrivacyViewable() or ignoreDuplicateButton:
             return False
         return True
 
     MeetingItem.__pm_old_showDuplicateItemAction = MeetingItem.showDuplicateItemAction
```

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/browser/configure.zcml` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/browser/itemcertifiedsignatures.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/browser/itemcertifiedsignatures.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/config.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/config.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/configure.zcml` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/events.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/events.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/events.zcml` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/events.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/interfaces.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/interfaces.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/PloneMeeting.pot` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/PloneMeeting.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/de/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.history.po` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/de/LC_MESSAGES/plone.po` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/de/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/en/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.history.po` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/en/LC_MESSAGES/plone.po` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/es/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.history.po` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/es/LC_MESSAGES/plone.po` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/es/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.history.po` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/plone.po` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/imio.actionspanel.pot` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/imio.actionspanel.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/imio.history.pot` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/imio.history.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.history.po` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/plone.po` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/nl/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/locales/plone.pot` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/migrations/migrate_to_4200.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/migrations/migrate_to_4200.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from DateTime import DateTime
 from plone import api
 from Products.MeetingCommunes.migrations.migrate_to_4200 import Migrate_To_4200 as MCMigrate_To_4200
+
 import logging
 
+
 logger = logging.getLogger('MeetingNamur')
 
 
 class Migrate_To_4200(MCMigrate_To_4200):
 
     def _fixUsedWFs(self):
         """meetingseraing_workflow/meetingitemseraing_workflow do not exist anymore,
```

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/migrations/migrate_to_4_1.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/migrations/migrate_to_4_1.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/model/pm_updates.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/model/pm_updates.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from Products.Archetypes.atapi import StringField
 from Products.Archetypes.atapi import TextAreaWidget
 from Products.Archetypes.atapi import TextField
 from Products.PloneMeeting.config import registerClasses
 from Products.PloneMeeting.MeetingItem import MeetingItem
 
 
-
 def update_item_schema(baseSchema):
     specificSchema = Schema((
 
         StringField(
             name='grpBudgetInfos',
             widget=MultiSelectionWidget(
                 description="GrpBudgetInfos",
```

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/cssregistry.xml` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/cssregistry.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/import_steps.xml` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/rolemap.xml` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/skins.xml` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/skins.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/workflows/meetingitemnamur_workflow/definition.xml` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/workflows/meetingitemnamur_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/workflows/meetingnamur_workflow/definition.xml` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/workflows/meetingnamur_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/default/workflows.xml` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/attach.png` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/budget.png` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.gif` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.png` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/financialAnalysis.png` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/legalAdvice.png` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/negative.png` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/overheadAnalysis.png` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/images/positive.png` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/import_data.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/import_steps.xml` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/templates/Agenda.odt` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/templates/Agenda.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/templates/Decisions.odt` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/templates/Decisions.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/examples_fr/templates/Item.odt` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/examples_fr/templates/Item.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/images/attach.png` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/images/budget.png` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/images/cahier.png` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/images/financialAnalysis.png` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/images/overheadAnalysis.png` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/images/positive.png` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles/testing/import_data.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles/testing/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/profiles.zcml` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/profiles.zcml`

 * *Files 5% similar despite different names*

```diff
@@ -31,8 +31,16 @@
         title="Go to MeetingNamur 4.2"
         description=""
         source="4.1"
         destination="4200"
         handler="Products.MeetingNamur.migrations.migrate_to_4200.migrate"
         profile="Products.MeetingNamur:default"/>
 
+    <genericsetup:upgradeStep
+        title="Go to MeetingNamur 4201"
+        description=""
+        source="4200"
+        destination="4201"
+        handler="Products.MeetingNamur.migrations.migrate_to_4201.migrate"
+        profile="Products.MeetingNamur:default"/>
+
 </configure>
```

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/setuphandlers.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/skins/meetingnamur_images/isConfidentialYes.png` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/skins/meetingnamur_images/isConfidentialYes.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_edit.pt` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_edit.pt`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_view.pt` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/skins/meetingnamur_templates/meetingitem_view.pt`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/testing.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/testing.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/testing.zcml` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/testing.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/MeetingNamurTestCase.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/MeetingNamurTestCase.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 # 02110-1301, USA.
 #
 
 from Products.MeetingCommunes.tests.MeetingCommunesTestCase import MeetingCommunesTestCase
-
 from Products.MeetingNamur.testing import MNA_TESTING_PROFILE_FUNCTIONAL
 from Products.MeetingNamur.tests.helpers import MeetingNamurTestingHelpers
 
+
 class MeetingNamurTestCase(MeetingCommunesTestCase, MeetingNamurTestingHelpers):
     """Base class for defining MeetingNamur test cases."""
 
     layer = MNA_TESTING_PROFILE_FUNCTIONAL
     subproductIgnoredTestFiles = ['testPerformances.py',
                                   'testVotes.py',
                                   'test_robot.py']
```

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/__init__.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/helpers.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testAdvices.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testAdvices.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testAnnexes.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testAnnexes.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testChangeItemOrderView.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testChangeItemOrderView.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testColumns.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testColumns.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testContacts.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testContacts.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testCustomMeeting.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testCustomMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testCustomMeetingItem.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testCustomMeetingItem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
+from AccessControl import Unauthorized
 from datetime import datetime
 from datetime import timedelta
-
-from AccessControl import Unauthorized
 from Products.MeetingCommunes.tests.testCustomMeetingItem import testCustomMeetingItem as mctcmi
 from Products.MeetingNamur.tests.MeetingNamurTestCase import MeetingNamurTestCase
 from Products.PloneMeeting.utils import org_id_to_uid
 
 
 class testCustomMeetingItem(MeetingNamurTestCase, mctcmi):
     """
@@ -18,21 +17,22 @@
         and state is, at least "itemFrozen". Retrieve role for other grp_budgetimpactreviewers
         """
         self.changeUser('pmManager')
         m = self._createMeetingWithItems()
         self.do(m, 'freeze')
         item = m.get_items()[0]
         # no MeetingBudgetImpactReviewer in rôle
-        developers_budgetimpactreviewers_uid = org_id_to_uid("developers_budgetimpactreviewers")
+        developers_uid = org_id_to_uid("developers")
+        developers_budgetimpactreviewers_uid = developers_uid + "_budgetimpactreviewers"
         vendors_budgetimpactreviewers_uid = org_id_to_uid("vendors_budgetimpactreviewers")
         self.assertFalse((developers_budgetimpactreviewers_uid, (
             'Reader', 'MeetingBudgetImpactReviewer')) in item.get_local_roles())
         self.assertFalse((vendors_budgetimpactreviewers_uid, (
             'Reader', 'MeetingBudgetImpactReviewer')) in item.get_local_roles())
-        item.setGrpBudgetInfos(('developers',))
+        item.setGrpBudgetInfos((developers_uid,))
         item.update_local_roles()
         # MeetingBudgetImpactReviewer role define for finance (only)
         self.assertTrue((developers_budgetimpactreviewers_uid, (
             'Reader', 'MeetingBudgetImpactReviewer')) in item.get_local_roles())
         self.assertFalse((vendors_budgetimpactreviewers_uid, (
             'Reader', 'MeetingBudgetImpactReviewer')) in item.get_local_roles())
```

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testFaceted.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testFaceted.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testMeetingCategory.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testMeetingCategory.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testMeetingConfig.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testMeetingConfig.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testMeetingItem.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testMeetingItem.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 # GNU General Public License (GPL)
 #
 
 from Products.MeetingCommunes.tests.testMeetingItem import testMeetingItem as mctmi
 from Products.MeetingNamur.tests.MeetingNamurTestCase import MeetingNamurTestCase
+from Products.PloneMeeting.config import EXECUTE_EXPR_VALUE
 from Products.PloneMeeting.utils import get_annexes
 from Products.PloneMeeting.utils import ON_TRANSITION_TRANSFORM_TAL_EXPR_ERROR
 from Products.statusmessages.interfaces import IStatusMessage
 
 
 class testMeetingItem(MeetingNamurTestCase, mctmi):
     """
@@ -93,27 +94,28 @@
         item3.setDescription('<p>My original description.</p>')
         self.do(item3, 'accept')
         self.assertTrue(item3.Description() == '<p>My new description.</p>')
         # if ever an error occurs with the TAL expression, the transition
         # is made but the rich text is not changed and a portal_message is displayed
         self.meetingConfig.setOnTransitionFieldTransforms(
             ({'transition': 'accept',
-              'field_name': 'MeetingItem.decision',
-              'tal_expression': 'some_wrong_tal_expression'},))
+              'field_name': EXECUTE_EXPR_VALUE,
+              'tal_expression': 'python: wrong_expression'},))
         item4 = meeting.get_items()[3]
         item4.setDecision('<p>My decision that will not be touched.</p>')
         self.do(item4, 'accept')
         # transition was triggered
         self.assertTrue(item4.query_state() == 'accepted')
         # original decision was not touched
         self.assertTrue(item4.getDecision(keepWithNext=False) == '<p>My decision that will not be touched.</p>')
         # a portal_message is displayed to the user that triggered the transition
         messages = IStatusMessage(self.request).show()
-        self.assertTrue(messages[-1].message == ON_TRANSITION_TRANSFORM_TAL_EXPR_ERROR % (
-            'decision', "'some_wrong_tal_expression'"))
+        self.assertEqual(
+            messages[-1].message, ON_TRANSITION_TRANSFORM_TAL_EXPR_ERROR %
+            (EXECUTE_EXPR_VALUE, "name 'wrong_expression' is not defined"))
 
     def test_pm_DuplicatedItemDoesNotKeepDecisionAnnexes(self):
         """When an item is duplicated using the 'duplicate and keep link',
            decision annexes are not kept."""
         self.changeUser('pmCreator1')
         item = self.create('MeetingItem')
         self.addAnnex(item)
```

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testPortlets.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testPortlets.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testSearches.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testSearches.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testSetup.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testSetup.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testToolPloneMeeting.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testToolPloneMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testUtils.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testUtils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testValidators.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testValidators.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testWFAdaptations.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testWFAdaptations.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,60 @@
 # -*- coding: utf-8 -*-
 #
-# File: testWFAdaptations.py
-#
-# Copyright (c) 2013 by Imio.be
-#
 # GNU General Public License (GPL)
 #
-# This program is free software; you can redistribute it and/or
-# modify it under the terms of the GNU General Public License
-# as published by the Free Software Foundation; either version 2
-# of the License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
-# 02110-1301, USA.
-#
 
-from datetime import datetime
-from Products.CMFCore.permissions import DeleteObjects
+from imio.helpers.content import get_vocab_values
 from Products.MeetingCommunes.tests.testWFAdaptations import testWFAdaptations as mctwfa
 from Products.MeetingNamur.tests.MeetingNamurTestCase import MeetingNamurTestCase
-from Products.PloneMeeting.tests.PloneMeetingTestCase import pm_logger
+from Products.PloneMeeting.config import MEETING_REMOVE_MOG_WFA
 
 
 class testWFAdaptations(MeetingNamurTestCase, mctwfa):
     '''Tests various aspects of votes management.'''
 
     def test_pm_WFA_availableWFAdaptations(self):
         '''Most of wfAdaptations makes no sense, just make sure most are disabled.'''
-        self.assertEquals(set(self.meetingConfig.listWorkflowAdaptations()),
-                          {'item_validation_shortcuts',
-                           'item_validation_no_validate_shortcuts',
-                           'only_creator_may_delete',
-                           'meeting_remove_global_access',
-                           'meetingmanager_correct_closed_meeting',
-                           'no_freeze',
-                           'no_publication',
-                           'no_decide',
-                           'accepted_but_modified',
-                           'postpone_next_meeting',
-                           'mark_not_applicable',
-                           'removed',
-                           'removed_and_duplicated',
-                           'refused',
-                           'delayed',
-                           'pre_accepted',
-                           'reviewers_take_back_validated_item',
-                           'presented_item_back_to_itemcreated',
-                           'presented_item_back_to_proposed',
-                           'return_to_proposing_group',
-                           'return_to_proposing_group_with_last_validation',
-                           'return_to_proposing_group_with_all_validations',
-                           'accepted_out_of_meeting',
-                           'accepted_out_of_meeting_and_duplicated',
-                           'accepted_out_of_meeting_emergency',
-                           'accepted_out_of_meeting_emergency_and_duplicated',
-                           'transfered',
-                           'transfered_and_duplicated',
-                           'namur_meetingmanager_may_not_edit_decision_project'
-                           })
+        self.assertEqual(
+            sorted(get_vocab_values(self.meetingConfig, 'WorkflowAdaptations')),
+            ['accepted_but_modified',
+             'accepted_out_of_meeting',
+             'accepted_out_of_meeting_and_duplicated',
+             'accepted_out_of_meeting_emergency',
+             'accepted_out_of_meeting_emergency_and_duplicated',
+             'delayed',
+             'item_validation_no_validate_shortcuts',
+             'item_validation_shortcuts',
+             'mark_not_applicable',
+             MEETING_REMOVE_MOG_WFA,
+             'meetingmanager_correct_closed_meeting',
+             # custom WFA
+             'namur_meetingmanager_may_not_edit_decision_project',
+             'no_decide',
+             'no_freeze',
+             'no_publication',
+             'only_creator_may_delete',
+             'postpone_next_meeting',
+             'pre_accepted',
+             'presented_item_back_to_itemcreated',
+             'presented_item_back_to_proposed',
+             'refused',
+             'removed',
+             'removed_and_duplicated',
+             'return_to_proposing_group',
+             'return_to_proposing_group_with_all_validations',
+             'return_to_proposing_group_with_last_validation',
+             'reviewers_take_back_validated_item',
+             'transfered',
+             'transfered_and_duplicated']
+        )
 
     def test_pm_Validate_workflowAdaptations_dependencies(self):
         '''Not all WFA are available yet...'''
         pass
 
 
-
 def test_suite():
     from unittest import TestSuite, makeSuite
     suite = TestSuite()
     suite.addTest(makeSuite(testWFAdaptations, prefix='test_pm_'))
     return suite
```

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products/MeetingNamur/tests/testWorkflows.py` & `Products.MeetingNamur-4.2.1/src/Products/MeetingNamur/tests/testWorkflows.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products.MeetingNamur.egg-info/PKG-INFO` & `Products.MeetingNamur-4.2.1/src/Products.MeetingNamur.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,50 @@
 Metadata-Version: 2.1
 Name: Products.MeetingNamur
-Version: 4.2.0rc3
+Version: 4.2.1
 Summary: PloneMeeting profile for city of Namur
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: Andre Nuyens
 Author-email: andre.nuyens@imio.be
 License: GPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 4.3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
-Provides-Extra: templates
 Provides-Extra: test
+Provides-Extra: templates
 
 ========================
 Products.MeetingNamur
 ========================
 
 'Products.MeetingNamur' is a custom profile for 'Products.MeetingCommunes'.
 Products.MeetingNamur Changelog
 ===============================
 
 Older versions than 3.0 can be found at http://svn.communesplone.org/svn/communesplone/MeetingNamur/tags/
 The Products.MeetingNamur version must be the same as the Products.PloneMeeting version
 
+4.2.1 (2024-05-24)
+------------------
+
+- Cleanup.
+  [gbastien]
+- Migrate `MeetingItem.grpBudgetInfos` to use orgs UIDs.
+  [aduchene]
+
+
+4.2.0 (2024-03-11)
+------------------
+
+- Fixed `MeetingItem.customshowDuplicateItemAction`.
+  [aduchene]
+
+
 4.2.0rc3 (2023-09-28)
 ---------------------
 
 - In `CustomNamurMeetingItem._initDecisionFieldIfEmpty` removed parameter
   `keepWithNext=False` when calling `MeetingItem.getDecision` as it does not
   exist anymore.
   [gbastien]
@@ -39,14 +54,15 @@
 - Fixed `meetingitem_view.pt` as `MeetingItem.isCopiesEnabled` was removed and
   field `MeetingItem.copyGroups` is now an optional field managed by
   `MeetingConfig.usedItemAttributes`.
   [gbastien]
 - `meetingnamur.css` is now completely empty.
   [gbastien]
 
+
 4.2.0rc2 (2023-07-04)
 ---------------------
 
 - Adapt vocabulary and i18n.
   [aduchene]
 
 
@@ -181,9 +197,7 @@
 - Migrated to Plone 4 (use PloneMeeting 3.x, see PloneMeeting's HISTORY.txt for full changes list)
 
 2.1.3 (2012-09-19)
 ------------------
 - Added possibility to give, modify and view an advice on created item
 - Added possibility to define a decision of replacement when an item is delayed
 - Added new workflow adaptation to add publish state with hidden decision for no meeting-manager
-
-
```

### Comparing `Products.MeetingNamur-4.2.0rc3/src/Products.MeetingNamur.egg-info/SOURCES.txt` & `Products.MeetingNamur-4.2.1/src/Products.MeetingNamur.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 src/Products/MeetingNamur/locales/fr/LC_MESSAGES/plone.po
 src/Products/MeetingNamur/locales/nl/LC_MESSAGES/PloneMeeting.po
 src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.actionspanel.po
 src/Products/MeetingNamur/locales/nl/LC_MESSAGES/imio.history.po
 src/Products/MeetingNamur/locales/nl/LC_MESSAGES/plone.po
 src/Products/MeetingNamur/migrations/__init__.py
 src/Products/MeetingNamur/migrations/migrate_to_4200.py
+src/Products/MeetingNamur/migrations/migrate_to_4201.py
 src/Products/MeetingNamur/migrations/migrate_to_4_1.py
 src/Products/MeetingNamur/model/__init__.py
 src/Products/MeetingNamur/model/generate.sh
 src/Products/MeetingNamur/model/pm_updates.py
 src/Products/MeetingNamur/profiles/__init__.py
 src/Products/MeetingNamur/profiles/default/MeetingNamur_marker.txt
 src/Products/MeetingNamur/profiles/default/__init__.py
```


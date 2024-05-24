# Comparing `tmp/pretix-sepadebit-2.4.2.tar.gz` & `tmp/pretix_sepadebit-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-sepadebit-2.4.2.tar", last modified: Tue Nov 28 17:11:19 2023, max compression
+gzip compressed data, was "pretix_sepadebit-2.5.0.tar", last modified: Fri May 24 08:27:58 2024, max compression
```

## Comparing `pretix-sepadebit-2.4.2.tar` & `pretix_sepadebit-2.5.0.tar`

### file list

```diff
@@ -1,135 +1,138 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.908714 pretix-sepadebit-2.4.2/
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2072 2023-11-28 17:11:19.908714 pretix-sepadebit-2.4.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      908 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.896714 pretix-sepadebit-2.4.2/pretix_sepadebit/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/apps.py
--rw-rw-rw-   0 root         (0) root         (0)   109251 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/bicdata.py
--rw-rw-rw-   0 root         (0) root         (0)     2593 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/exporters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.896714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.872713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/ar/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.896714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/ar/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15987 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.872713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/ca/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.896714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/ca/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16372 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.872713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/cs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.896714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/cs/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15998 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.872713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/da/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.896714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/da/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16052 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.872713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.896714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    23675 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-28 17:10:50.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    23684 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)    15738 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/django.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.872713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/el/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/el/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15713 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.872713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16269 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.872713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/fi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/fi/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16075 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.872713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    25198 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.872713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/hr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/hr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15713 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.872713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/it/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/it/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16030 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.876713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15713 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.876713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/lv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/lv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16132 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.876713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/nl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    24121 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.892713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/nl_BE/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/nl_BE/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15716 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/nl_BE/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.892713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/nl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/nl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    24357 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/nl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.892713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/pl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/pl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16628 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.892713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/pl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/pl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15722 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/pl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.892713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/pt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/pt/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15713 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.892713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/pt_BR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/pt_BR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16025 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.892713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15713 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.892713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/si/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/si/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15963 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/si/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.892713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/sl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/sl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15950 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.892713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/sv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/sv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16039 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.892713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/uk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.900714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/uk/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16095 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.892713 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.904714 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16063 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.904714 pretix-sepadebit-2.4.2/pretix_sepadebit/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1802 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/migrations/0002_auto_20170530_1527.py
--rw-rw-rw-   0 root         (0) root         (0)      958 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/migrations/0003_sepaexportorder_payment.py
--rw-rw-rw-   0 root         (0) root         (0)      407 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/migrations/0004_sepaexport_testmode.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/migrations/0005_auto_20190429_0811.py
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/migrations/0006_sepaexport_currency.py
--rw-rw-rw-   0 root         (0) root         (0)     2806 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/migrations/0007_sepaduedate.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/migrations/0008_alter_sepaduedate_payment.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-28 17:10:50.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/models.py
--rw-rw-rw-   0 root         (0) root         (0)    19528 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/payment.py
--rw-rw-rw-   0 root         (0) root         (0)     9441 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.892713 pretix-sepadebit-2.4.2/pretix_sepadebit/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.904714 pretix-sepadebit-2.4.2/pretix_sepadebit/static/pretix_sepadebit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-28 17:10:50.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/static/pretix_sepadebit/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.892713 pretix-sepadebit-2.4.2/pretix_sepadebit/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.908714 pretix-sepadebit-2.4.2/pretix_sepadebit/templates/pretix_sepadebit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-28 17:10:50.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/templates/pretix_sepadebit/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     1551 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)     1476 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1670 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/templates/pretix_sepadebit/control.html
--rw-rw-rw-   0 root         (0) root         (0)     5782 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/templates/pretix_sepadebit/export.html
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/templates/pretix_sepadebit/mail.txt
--rw-rw-rw-   0 root         (0) root         (0)     3400 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/templates/pretix_sepadebit/orders.html
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/templates/pretix_sepadebit/pending.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.908714 pretix-sepadebit-2.4.2/pretix_sepadebit/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-28 17:10:50.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10539 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/tests/test_payment.py
--rw-rw-rw-   0 root         (0) root         (0)      938 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    12651 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pretix_sepadebit/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:11:19.908714 pretix-sepadebit-2.4.2/pretix_sepadebit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2072 2023-11-28 17:11:19.000000 pretix-sepadebit-2.4.2/pretix_sepadebit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3070 2023-11-28 17:11:19.000000 pretix-sepadebit-2.4.2/pretix_sepadebit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-28 17:11:19.000000 pretix-sepadebit-2.4.2/pretix_sepadebit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      137 2023-11-28 17:11:19.000000 pretix-sepadebit-2.4.2/pretix_sepadebit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-11-28 17:11:19.000000 pretix-sepadebit-2.4.2/pretix_sepadebit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-11-28 17:11:19.000000 pretix-sepadebit-2.4.2/pretix_sepadebit.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1011 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      817 2023-11-28 17:11:19.908714 pretix-sepadebit-2.4.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-11-28 17:03:08.000000 pretix-sepadebit-2.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.636288 pretix_sepadebit-2.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      135 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2072 2024-05-24 08:27:58.636288 pretix_sepadebit-2.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      908 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.628288 pretix_sepadebit-2.5.0/pretix_sepadebit/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      608 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)   109251 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/bicdata.py
+-rw-rw-rw-   0 root         (0) root         (0)     2593 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/exporters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.628288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.620288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/ar/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.628288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/ar/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16318 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.620288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/ca/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.628288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/ca/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16703 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.620288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/cs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.628288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/cs/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16329 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.620288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/da/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.628288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/da/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16383 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.620288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.628288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    24170 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.628288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.628288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    24180 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)    16069 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/django.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.620288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/el/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.628288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/el/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16044 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.620288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.628288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16600 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.620288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/fi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.628288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/fi/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16406 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.620288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.632288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    25925 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.620288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/hr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.632288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/hr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16044 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.620288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/it/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.632288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/it/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16361 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.620288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/ja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.632288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16044 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.620288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/lv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.632288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/lv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16463 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.620288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/nl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.632288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    24781 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.624288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/nl_BE/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.632288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/nl_BE/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16069 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/nl_BE/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.624288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/nl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.632288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/nl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    25017 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/nl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.624288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/pl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.632288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/pl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16959 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.624288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/pl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.632288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/pl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16053 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/pl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.624288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/pt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.632288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/pt/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16044 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.624288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/pt_BR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.632288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/pt_BR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16356 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.624288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.632288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16044 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.624288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/si/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.632288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/si/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16294 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/si/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.624288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/sk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.632288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/sk/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16044 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.624288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/sl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.632288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/sl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16281 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.624288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/sv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.632288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/sv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16370 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.624288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/uk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.632288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/uk/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16531 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.624288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.632288 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16394 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.636288 pretix_sepadebit-2.5.0/pretix_sepadebit/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/migrations/0002_auto_20170530_1527.py
+-rw-rw-rw-   0 root         (0) root         (0)      958 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/migrations/0003_sepaexportorder_payment.py
+-rw-rw-rw-   0 root         (0) root         (0)      407 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/migrations/0004_sepaexport_testmode.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/migrations/0005_auto_20190429_0811.py
+-rw-rw-rw-   0 root         (0) root         (0)      240 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/migrations/0006_sepaexport_currency.py
+-rw-rw-rw-   0 root         (0) root         (0)     2806 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/migrations/0007_sepaduedate.py
+-rw-rw-rw-   0 root         (0) root         (0)      588 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/migrations/0008_alter_sepaduedate_payment.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    19652 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)     9441 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.624288 pretix_sepadebit-2.5.0/pretix_sepadebit/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.636288 pretix_sepadebit-2.5.0/pretix_sepadebit/static/pretix_sepadebit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/static/pretix_sepadebit/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.624288 pretix_sepadebit-2.5.0/pretix_sepadebit/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.636288 pretix_sepadebit-2.5.0/pretix_sepadebit/templates/pretix_sepadebit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/templates/pretix_sepadebit/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     1551 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)     1476 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/templates/pretix_sepadebit/control.html
+-rw-rw-rw-   0 root         (0) root         (0)     5782 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/templates/pretix_sepadebit/export.html
+-rw-rw-rw-   0 root         (0) root         (0)      465 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/templates/pretix_sepadebit/mail.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3400 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/templates/pretix_sepadebit/orders.html
+-rw-rw-rw-   0 root         (0) root         (0)      174 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/templates/pretix_sepadebit/pending.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.636288 pretix_sepadebit-2.5.0/pretix_sepadebit/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10539 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/tests/test_payment.py
+-rw-rw-rw-   0 root         (0) root         (0)      938 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    12651 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pretix_sepadebit/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:58.636288 pretix_sepadebit-2.5.0/pretix_sepadebit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2072 2024-05-24 08:27:58.000000 pretix_sepadebit-2.5.0/pretix_sepadebit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3119 2024-05-24 08:27:58.000000 pretix_sepadebit-2.5.0/pretix_sepadebit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 08:27:58.000000 pretix_sepadebit-2.5.0/pretix_sepadebit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      137 2024-05-24 08:27:58.000000 pretix_sepadebit-2.5.0/pretix_sepadebit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2024-05-24 08:27:58.000000 pretix_sepadebit-2.5.0/pretix_sepadebit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-24 08:27:58.000000 pretix_sepadebit-2.5.0/pretix_sepadebit.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      817 2024-05-24 08:27:58.636288 pretix_sepadebit-2.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-24 08:27:27.000000 pretix_sepadebit-2.5.0/setup.py
```

### Comparing `pretix-sepadebit-2.4.2/LICENSE` & `pretix_sepadebit-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/PKG-INFO` & `pretix_sepadebit-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-sepadebit
-Version: 2.4.2
+Version: 2.5.0
 Summary: This plugin adds SEPA direct debit support to pretix
 Author-email: pretix team <support@pretix.eu>
 Maintainer-email: pretix team <support@pretix.eu>
 License: Copyright 2017 Raphael Michel
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
```

### Comparing `pretix-sepadebit-2.4.2/README.rst` & `pretix_sepadebit-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/apps.py` & `pretix_sepadebit-2.5.0/pretix_sepadebit/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/bicdata.py` & `pretix_sepadebit-2.5.0/pretix_sepadebit/bicdata.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/exporters.py` & `pretix_sepadebit-2.5.0/pretix_sepadebit/exporters.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/ar/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/ar/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
 "PO-Revision-Date: 2019-11-22 17:00+0000\n"
 "Last-Translator: Raphael Michel <michel@rami.io>\n"
 "Language-Team: Arabic <https://translate.pretix.eu/projects/pretix/pretix-"
 "plugin-sepadebit/ar/>\n"
 "Language: ar\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -24,279 +24,291 @@
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
 msgctxt "export_category"
 msgid "Order data"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr ""
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -435,18 +447,14 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr ""
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
 msgstr ""
@@ -468,14 +476,21 @@
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr ""
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/ca/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/uk/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,299 +3,312 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: 2020-12-15 21:00+0000\n"
-"Last-Translator: albert <albert.serra.monner@gmail.com>\n"
-"Language-Team: Catalan <https://translate.pretix.eu/projects/pretix/pretix-"
-"plugin-sepadebit/ca/>\n"
-"Language: ca\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
+"PO-Revision-Date: 2024-05-23 05:00+0000\n"
+"Last-Translator: Serhii Horichenko <m@sgg.im>\n"
+"Language-Team: Ukrainian <https://translate.pretix.eu/projects/pretix/"
+"pretix-plugin-sepadebit/uk/>\n"
+"Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 3.10.3\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 5.5.5\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
-msgstr ""
+msgstr "Прямий дебет SEPA"
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
 msgctxt "export_category"
 msgid "Order data"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
-msgid "Order code"
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:40
+msgid "Order code"
+msgstr "Код замовлення"
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
-msgstr ""
+msgstr "Сума оплати"
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
-msgstr ""
+msgstr "Доступні символи заповнення: {list}"
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr "IBAN"
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
-msgstr "BIC"
+msgstr ""
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -386,48 +399,44 @@
 
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:38
 msgid "Due date"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:10
 msgid "In test mode, your exports will only contain test mode orders."
-msgstr "En mode de prova, les exportacions només contindran comandes de prova."
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:14
 msgid ""
 "If you want, you can now also create SEPA debit files for multiple events "
 "combined."
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:17
 msgid "Go to organizer-level exports"
-msgstr "Anar a les exportacions de nivell organitzador"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:24
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:33
 msgid ""
 "Refunds for SEPA debit transactions are grouped with bank transfer refunds."
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:27
-#, fuzzy
-#| msgid "Go to organizer-level exports"
 msgid "Go to refund exports"
-msgstr "Anar a les exportacions de nivell organitzador"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:36
-#, fuzzy
-#| msgid "Go to organizer-level exports"
 msgid "Go to organizer-level refund exports"
-msgstr "Anar a les exportacions de nivell organitzador"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:44
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:65
 msgid "Create new export file"
-msgstr "Crear un nou fitxer d'exportació"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:48
 #, python-format
 msgid ""
 "<strong>%(num_new)s</strong> SEPA debit orders have been placed and are not "
 "yet exported as Sepa XML."
 msgstr ""
@@ -438,30 +447,26 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr "Data d'exportació"
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
-msgstr "Número de comandes"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
-msgstr ""
+msgstr "Загальна сума"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:89
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:19
 msgid "TEST MODE"
-msgstr ""
+msgstr "ТЕСТОВИЙ РЕЖИМ"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:103
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:110
 msgid "Orders"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:106
@@ -469,15 +474,22 @@
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:11
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:15
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
-msgstr "Encara no s'han creat exportacions."
+msgstr ""
+
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
@@ -495,15 +507,15 @@
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:32
 msgid "Order"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:33
 msgid "Payment"
-msgstr ""
+msgstr "Оплата"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:34
 msgid "Mandate date"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:35
 msgid "Associated invoices"
@@ -518,15 +530,15 @@
 "The SEPA direct debit failed to be completed. Please contact the organizer "
 "of the event as soon as possible!"
 msgstr ""
 
 #: pretix_sepadebit/views.py:100
 #, python-brace-format
 msgid "Event ticket {event}-{code}"
-msgstr "Tiquet per l'acte {event}-{code}"
+msgstr "Квиток на подію {event}-{code}"
 
 #: pretix_sepadebit/views.py:137
 msgid ""
 "The generated file did not validate for the following reasons. Please "
 "contact pretix support for more information.\n"
 "{}"
 msgstr ""
@@ -539,8 +551,8 @@
 
 #: pretix_sepadebit/views.py:150
 msgid "A new export file has been created."
 msgstr ""
 
 #: pretix_sepadebit/views.py:152
 msgid "No valid orders have been found."
-msgstr "No s'han trobat comandes vàlides."
+msgstr ""
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/cs/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/cs/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
 "PO-Revision-Date: 2023-09-15 17:00+0000\n"
 "Last-Translator: Michael <michael.happl@gmx.at>\n"
-"Language-Team: Czech <https://translate.pretix.eu/projects/pretix/"
-"pretix-plugin-sepadebit/cs/>\n"
+"Language-Team: Czech <https://translate.pretix.eu/projects/pretix/pretix-"
+"plugin-sepadebit/cs/>\n"
 "Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
 "X-Generator: Weblate 5.0.1\n"
 
@@ -23,279 +23,291 @@
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
 msgctxt "export_category"
 msgid "Order data"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
 msgstr "Datum objednávky"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr "Částka platby"
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr "Dostupné zástupné symboly: {list}"
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr "Majitel účtu"
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr "IBAN"
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr "BIC"
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -434,18 +446,14 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr ""
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
 msgstr ""
@@ -467,14 +475,21 @@
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr ""
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/da/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/fi/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,301 +3,313 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: 2018-03-20 21:00+0000\n"
-"Last-Translator: Mikkel Ricky <rimi@aarhus.dk>\n"
-"Language-Team: Danish <https://translate.pretix.eu/projects/pretix/pretix-"
-"plugin-sepadebit/da/>\n"
-"Language: da\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
+"PO-Revision-Date: 2021-01-07 03:00+0000\n"
+"Last-Translator: Jaakko Rinta-Filppula <jaakko@r-f.fi>\n"
+"Language-Team: Finnish <https://translate.pretix.eu/projects/pretix/pretix-"
+"plugin-sepadebit/fi/>\n"
+"Language: fi\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 2.19.1\n"
+"X-Generator: Weblate 3.10.3\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
 #, fuzzy
 #| msgid "Order date"
 msgctxt "export_category"
 msgid "Order data"
-msgstr "Bestillingsdato"
+msgstr "Tilauksen päivämäärä"
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr "Vie päivämäärä"
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
-msgstr "Bestillingskode"
+msgstr "Tilauskoodi"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
-msgstr "Bestillingsdato"
+msgstr "Tilauksen päivämäärä"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
-msgstr "Fakturaer"
+msgstr "Laskut"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr ""
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
-msgstr "Kontoejer"
+msgstr ""
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -436,45 +448,48 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr ""
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
-msgstr "Samlet beløb"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:89
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:19
 msgid "TEST MODE"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:103
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:110
 msgid "Orders"
-msgstr "Bestillinger"
+msgstr "Tilaukset"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:106
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:113
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:11
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:15
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
+msgstr "Vientejä ei ole vielä tehty."
+
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
@@ -489,25 +504,23 @@
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:24
 #, python-format
 msgid "Total amount: %(total)s %(currency)s"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:32
 msgid "Order"
-msgstr "Rækkefølge"
+msgstr "Tilaus"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:33
 msgid "Payment"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:34
-#, fuzzy
-#| msgid "Order date"
 msgid "Mandate date"
-msgstr "Bestillingsdato"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:35
 msgid "Associated invoices"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:70
 msgid "No orders have been part of this export."
@@ -518,15 +531,15 @@
 "The SEPA direct debit failed to be completed. Please contact the organizer "
 "of the event as soon as possible!"
 msgstr ""
 
 #: pretix_sepadebit/views.py:100
 #, python-brace-format
 msgid "Event ticket {event}-{code}"
-msgstr ""
+msgstr "Tapahtumalippu {event}-{code}"
 
 #: pretix_sepadebit/views.py:137
 msgid ""
 "The generated file did not validate for the following reasons. Please "
 "contact pretix support for more information.\n"
 "{}"
 msgstr ""
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/de/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/de/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,247 +1,260 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: 2023-05-16 20:00+0000\n"
-"Last-Translator: Moritz Lerch <dev@moritz-lerch.de>\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
+"PO-Revision-Date: 2024-05-07 09:53+0000\n"
+"Last-Translator: Raphael Michel <michel@rami.io>\n"
 "Language-Team: German <https://translate.pretix.eu/projects/pretix/"
 "pretix-plugin-sepadebit/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.17\n"
+"X-Generator: Weblate 5.4.3\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr "SEPA-Bankeinzug"
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr "Diese Erweiterung fügt Unterstützung für SEPA-Bankeinzug hinzu."
 
-#: pretix_sepadebit/exporters.py:12
+#: pretix_sepadebit/exporters.py:16
 msgid "List of previous SEPA debits"
 msgstr "Liste vorheriger SEPA-Bankeinzüge"
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
 msgctxt "export_category"
 msgid "Order data"
 msgstr "Bestelldaten"
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 "Tabelle (Excel oder CSV) mit allen SEPA-Lastschriften, die in der "
 "Vergangenheit generiert und exportiert wurden. Um einen neuen SEPA-Export zu "
 "erstellen, gehe in den Abschnitt \"SEPA-Lastschrift\" im Hauptmenü."
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr "Exportdatum"
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr "Kurzname der Veranstaltung"
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr "Veranstaltungstitel"
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
 msgstr "Bestellnummer"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
 msgstr "Bestelldatum"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
 msgstr "Rechnungen"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr "SEPA-Exportdatum"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr "Zahlbetrag"
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 "SEPA-Lastschrift ist für diese IBAN nicht möglich, bitte nimm Kontakt mit "
 "dem Veranstalter auf oder wähle eine andere Zahlungsart."
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 "Die BIC {bic} passt nicht zur IBAN, bitte überprüfen Sie Ihre Kontodaten. "
 "Laut unserer Liste wäre die korrekte BIC {correctbic}."
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr "SEPA-Lastschrift"
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 "Zahlungen im Testmodus werden nur eingezogen wenn Sie eine Datei an die Bank "
 "übermitteln, die im Testmodus erstellt wurde."
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr "Verfügbare Platzhalter: {list}"
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 "Ich habe verstanden, dass ich regelmäßig SEPA-XML-Dateien herunterladen und "
 "zu meiner Bank übertragen muss, damit meine Bank die Zahlungen der Kunden "
 "einzieht."
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr "Name des Gläubigers"
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr "Gläubiger-IBAN"
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr "Gläubiger-BIC"
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr "Gläubiger-ID"
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr "Dies muss eine gültige SEPA-Gläubiger-ID sein."
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr "Mandatsreferenz-Prefix"
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 "Dieses Feld darf nur Buchstaben, Zahlen und die folgenden Zeichen enthalten: "
 "' , . : + - / ( ) ?"
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 "Wir werden diese Zeichen der von pretix aus dem Veranstaltungs-Kurznamen und "
 "der Bestellnummer generierten Mandatsreferenz voranstellen."
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr "Vorabinformationszeit"
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 "Anzahl an Tagen zwischen der Bestellung und dem Fälligkeitsdatum der "
 "Lastschrift. Abhängig von Ihrer Gesetzeslage und den Regeln Ihrer Bank "
 "müssen Sie die Lastschriften 5-6 Tage vor Fälligkeit bei der Bank einreichen "
 "und sind möglicherweise verpflichtet, den Benutzer 14 Tage vor Fälligkeit zu "
 "informieren. Wir empfehlen, mindestens 7 Tage einzustellen."
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr "IBAN-Blockliste"
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 "Eine IBAN oder ein IBAN-Präfix pro Zeile. Das System wird diese IBANs nicht "
 "erlauben. Nützlich z.B. für bereits öfter ausgefallene Zahlungen. Es können "
 "auch ganze Ländercodes wie z.B. \"GB\" blockiert werden, wenn keine IBANs "
 "aus diesem Land akzeptiert werden sollen."
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 "Komplette Länder zu blockieren wird als SEPA-Diskriminierung angesehen, die "
 "in den meisten Ländern nicht zulässig ist und Bußgelder von "
 "Regulierungsbehörden nach sich ziehen kann."
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr "Frühstes Einzugsdatum"
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 "Frühester Termin, zu dem der Einzug fällig sein kann. Dieser Termin wird als "
 "Fälligkeitsdatum verwendet werden, wenn das Bestelldatum plus die "
 "Vorabinformationszeit in einem früheren Datum resultieren würde. Kunden mit "
 "Bestellungen, die zu diesem Datum fällig werden, erhalten eine E-Mail mit "
 "einer Erinnerung an die fällig werdende Zahlung basierend auf der "
 "konfigurierten Vorabinformationszeit."
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr "Vorabinformation E-Mail-Betreff"
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 "Der Betreff der Erinnerungs-E-Mail. Die E-Mail wird nur verschickt wenn das "
 "Früheste Einzugsdatum verwendet wird."
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr "Vorabinformation E-Mail-Text"
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 "Der Text der Erinnerungs-E-Mail. Die E-Mail wird nur verschickt wenn das "
 "Früheste Einzugsdatum verwendet wird."
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
@@ -250,106 +263,105 @@
 "über ein Webformular entgegengenommen. Abhängig von Ihrer Gesetzteslage, "
 "kann es nötig sein diese auf Papier einzufordern um das Risiko der "
 "Rücklastschrift zu verringern. SEPA-Lastschriften werden in der Shopsoftware "
 "sofort nach Bestellung als bezahlt markiert. Im Falle einer Rücklastschrift "
 "müssen Sie die Bestellung wieder als unbezahlt markieren und Kontakt zum "
 "Nutzer aufnehmen."
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 "Der Platzhalter <code>{payment_info}</code> ist nicht in Ihrer E-Mail-"
 "Vorlage enthalten, die für erhaltene Zahlungen verschickt wird. Dies ist "
 "aber rechtlich notwendig, da hier die Mandatsreferenz und das "
 "Fälligkeitsdatum mitgeteilt werden."
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 "Die Felder für die E-Mail-Inhalte der Vorabinformation sind verpflichtend "
 "auszufüllen, wenn das früheste Einzugsdatum verwendet wird."
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr "Kontoinhaber*in"
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr "IBAN"
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr "BIC"
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 "Ich ermächtige hiermit den Veranstalter zum Bankeinzug mittels SEPA-"
 "Lastschrift (siehe unten)"
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr "wird eingezogen"
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 "Wir werden den vollen Bestellbetrag am oder kurz nach dem %(date)s von Ihrem "
-"Bankkonto einziehen."
+"Bankkonto %(account)s einziehen."
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 "Diese Zahlung wird auf Ihrem Kontoauszug als %(creditor_name)s mit "
 "Mandatsreferenz %(reference)s und Gläubiger-ID %(id)s erscheinen."
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr "Die Vorabinformationszeit der SEPA-Zahlung ist nicht eingestellt."
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 "Eine Erinnerung an den fällig werdenden Zahlungseinzug wurde an den Kunden "
 "verschickt."
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr "SEPA-Lastschrift-Zahlungsverlauf"
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr "Dies entfernt exportierte SEPA-XML-Dateien mit Bankdaten vom Server."
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr "Anstehender Einzug von {debit_amount_with_currency}"
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -532,18 +544,14 @@
 "Erstelle mehrere Dateien, wenn die Lastschriften unterschiedliche "
 "Fälligkeitstermine haben (für manche Banken erforderlich)"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr "Exportierte XML-Dateien"
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr "Exportdatum"
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr "Anzahl Bestellungen"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
 msgstr "Gesamtbetrag"
@@ -565,14 +573,23 @@
 msgid "Download XML"
 msgstr "XML herunterladen"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr "Es wurden noch keine Dateien exportiert."
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+"Wir werden den vollen Bestellbetrag am oder kurz nach dem %(date)s von Ihrem "
+"Bankkonto einziehen."
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr "SEPA-Export"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/de_Informal/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,247 +1,260 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: 2023-05-16 20:00+0000\n"
-"Last-Translator: Moritz Lerch <dev@moritz-lerch.de>\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
+"PO-Revision-Date: 2024-05-07 09:53+0000\n"
+"Last-Translator: Raphael Michel <michel@rami.io>\n"
 "Language-Team: German (informal) <https://translate.pretix.eu/projects/"
 "pretix/pretix-plugin-sepadebit/de_Informal/>\n"
 "Language: de_Informal\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.17\n"
+"X-Generator: Weblate 5.4.3\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr "SEPA-Bankeinzug"
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr "Diese Erweiterung fügt Unterstützung für SEPA-Bankeinzug hinzu."
 
-#: pretix_sepadebit/exporters.py:12
+#: pretix_sepadebit/exporters.py:16
 msgid "List of previous SEPA debits"
 msgstr "Liste vorheriger SEPA-Bankeinzüge"
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
 msgctxt "export_category"
 msgid "Order data"
 msgstr "Bestelldaten"
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 "Tabelle (Excel oder CSV) mit allen SEPA-Lastschriften, die in der "
 "Vergangenheit generiert und exportiert wurden. Um einen neuen SEPA-Export zu "
 "erstellen, gehen Sie in den Abschnitt \"SEPA-Lastschrift\" im Hauptmenü."
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr "Exportdatum"
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr "Kurzname der Veranstaltung"
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr "Veranstaltungstitel"
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
 msgstr "Bestellnummer"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
 msgstr "Bestelldatum"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
 msgstr "Rechnungen"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr "SEPA-Exportdatum"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr "Zahlbetrag"
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 "SEPA-Lastschrift ist für diese IBAN nicht möglich, bitte nimm Kontakt mit "
 "dem Veranstalter auf oder wähle eine andere Zahlungsart."
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 "Die BIC {bic} passt nicht zur IBAN, bitte überprüfe deine Kontodaten. Laut "
 "unserer Liste wäre die korrekte BIC {correctbic}."
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr "SEPA-Lastschrift"
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 "Zahlungen im Testmodus werden nur eingezogen wenn du eine Datei an die Bank "
 "übermittelst, die im Testmodus erstellt wurde."
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr "Verfügbare Platzhalter: {list}"
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 "Ich habe verstanden, dass ich regelmäßig SEPA-XML-Dateien herunterladen und "
 "zu meiner Bank übertragen muss, damit meine Bank die Zahlungen der Kunden "
 "einzieht."
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr "Name des Gläubigers"
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr "Gläubiger-IBAN"
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr "Gläubiger-BIC"
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr "Gläubiger-ID"
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr "Dies muss eine gültige SEPA-Gläubiger-ID sein."
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr "Mandatsreferenz-Prefix"
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 "Dieses Feld darf nur Buchstaben, Zahlen und die folgenden Zeichen enthalten: "
 "' , . : + - / ( ) ?"
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 "Wir werden diese Zeichen der von pretix aus dem Veranstaltungs-Kurznamen und "
 "der Bestellnummer generierten Mandatsreferenz voranstellen."
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr "Vorabinformationszeit"
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 "Anzahl an Tagen zwischen der Bestellung und dem Fälligkeitsdatum der "
 "Lastschrift. Abhängig von deiner Gesetzeslage und den Regeln deiner Bank "
 "musst du die Lastschriften 5-6 Tage vor Fälligkeit bei der Bank einreichen "
 "und bist möglicherweise verpflichtet, den Benutzer 14 Tage vor Fälligkeit zu "
 "informieren. Wir empfehlen, mindestens 7 Tage einzustellen."
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr "IBAN-Blockliste"
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 "Eine IBAN oder ein IBAN-Präfix pro Zeile. Das System wird diese IBANs nicht "
 "erlauben. Nützlich z.B. für bereits öfter ausgefallene Zahlungen. Es können "
 "auch ganze Ländercodes wie z.B. \"GB\" blockiert werden, wenn keine IBANs "
 "aus diesem Land akzeptiert werden sollen."
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 "Komplette Länder zu blockieren wird als SEPA-Diskriminierung angesehen, die "
 "in den meisten Ländern nicht zulässig ist und Bußgelder von "
 "Regulierungsbehörden nach sich ziehen kann."
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr "Frühstes Einzugsdatum"
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 "Frühester Termin, zu dem der Einzug fällig sein kann. Dieser Termin wird als "
 "Fälligkeitsdatum verwendet werden, wenn das Bestelldatum plus die "
 "Vorabinformationszeit in einem früheren Datum resultieren würde. Kunden mit "
 "Bestellungen, die zu diesem Datum fällig werden, erhalten eine E-Mail mit "
 "einer Erinnerung an die fällig werdende Zahlung basierend auf der "
 "konfigurierten Vorabinformationszeit."
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr "Vorabinformation E-Mail-Betreff"
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 "Der Betreff der Erinnerungs-E-Mail. Die E-Mail wird nur verschickt wenn das "
 "Früheste Einzugsdatum verwendet wird."
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr "Vorabinformation E-Mail-Text"
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 "Der Text der Erinnerungs-E-Mail. Die E-Mail wird nur verschickt wenn das "
 "Früheste Einzugsdatum verwendet wird."
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
@@ -250,106 +263,105 @@
 "über ein Webformular entgegengenommen. Abhängig von deiner Gesetzeslage, "
 "kann es nötig sein diese auf Papier einzufordern um das Risiko der "
 "Rücklastschrift zu verringern. SEPA-Lastschriften werden in der Shopsoftware "
 "sofort nach Bestellung als bezahlt markiert. Im Falle einer Rücklastschrift "
 "musst du die Bestellung wieder als unbezahlt markieren und Kontakt zum "
 "Nutzer aufnehmen."
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 "Der Platzhalter <code>{payment_info}</code> ist nicht in deiner E-Mail-"
 "Vorlage enthalten, die für erhaltene Zahlungen verschickt wird. Dies ist "
 "aber rechtlich notwendig, da hier die Mandatsreferenz und das "
 "Fälligkeitsdatum mitgeteilt werden."
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 "Die Felder für die E-Mail-Inhalte der Vorabinformation sind verpflichtend "
 "auszufüllen, wenn das früheste Einzugsdatum verwendet wird."
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr "Kontoinhaber*in"
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr "IBAN"
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr "BIC"
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 "Ich ermächtige hiermit den Veranstalter zum Bankeinzug mittels SEPA-"
 "Lastschrift (siehe unten)"
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr "wird eingezogen"
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 "Wir werden den vollen Bestellbetrag am oder kurz nach dem %(date)s von "
-"deinem Bankkonto einziehen."
+"deinem Bankkonto %(account)s einziehen."
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 "Diese Zahlung wird auf deinem Kontoauszug als %(creditor_name)s mit "
 "Mandatsreferenz %(reference)s und Gläubiger-ID %(id)s erscheinen."
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr "Die Vorabinformationszeit der SEPA-Zahlung ist nicht eingestellt."
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 "Eine Erinnerung an den fällig werdenden Zahlungseinzug wurde an den Kunden "
 "verschickt."
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr "SEPA-Lastschrift-Zahlungsverlauf"
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr "Dies entfernt exportierte SEPA-XML-Dateien mit Bankdaten vom Server."
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr "Anstehender Einzug von {debit_amount_with_currency}"
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -532,18 +544,14 @@
 "Erstelle mehrere Dateien, wenn die Lastschriften unterschiedliche "
 "Fälligkeitstermine haben (für manche Banken erforderlich)"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr "Exportierte XML-Dateien"
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr "Exportdatum"
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr "Anzahl Bestellungen"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
 msgstr "Gesamtbetrag"
@@ -565,14 +573,23 @@
 msgid "Download XML"
 msgstr "XML herunterladen"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr "Es wurden noch keine Dateien exportiert."
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+"Wir werden den vollen Bestellbetrag am oder kurz nach dem %(date)s von "
+"deinem Bankkonto einziehen."
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr "SEPA-Export"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/django.pot` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/lv/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,299 +1,316 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
-#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
+"PO-Revision-Date: 2022-04-06 03:00+0000\n"
+"Last-Translator: Liga V <lerning_by_dreaming@gmx.de>\n"
+"Language-Team: Latvian <https://translate.pretix.eu/projects/pretix/pretix-"
+"plugin-sepadebit/lv/>\n"
+"Language: lv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=3; plural=(n % 10 == 0 || n % 100 >= 11 && n % 100 <= "
+"19) ? 0 : ((n % 10 == 1 && n % 100 != 11) ? 1 : 2);\n"
+"X-Generator: Weblate 4.11.2\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
+#, fuzzy
+#| msgid "Order date"
 msgctxt "export_category"
 msgid "Order data"
-msgstr ""
+msgstr "Pasūtījuma datums"
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
-msgid "Order code"
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr "Exporta datums"
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
-msgid "Order date"
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
+msgid "Order code"
+msgstr "Pasūtījuma kods"
+
+#: pretix_sepadebit/exporters.py:40
+msgid "Order date"
+msgstr "Pasūtījuma datums"
+
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
-msgstr ""
+msgstr "Maksājuma summa"
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
-msgstr ""
+msgstr "Konta īpašnieks"
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
-msgstr ""
+msgstr "IBAN"
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
-msgstr ""
+msgstr "BIC"
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -432,21 +449,17 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr ""
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
-msgstr ""
+msgstr "Pasūtījumu skaits"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:89
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:19
@@ -465,14 +478,21 @@
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr ""
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/el/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/el/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: el\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -20,279 +20,291 @@
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
 msgctxt "export_category"
 msgid "Order data"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr ""
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -431,18 +443,14 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr ""
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
 msgstr ""
@@ -464,14 +472,21 @@
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr ""
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/es/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/es/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
 "PO-Revision-Date: 2019-05-01 23:00+0000\n"
 "Last-Translator: Alvaro Enrique Ruano <alvaro.ruano90@outlook.com>\n"
 "Language-Team: Spanish <https://translate.pretix.eu/projects/pretix/pretix-"
 "plugin-sepadebit/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -23,281 +23,293 @@
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
 #, fuzzy
 #| msgid "Order date"
 msgctxt "export_category"
 msgid "Order data"
 msgstr "Fecha de la orden"
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
 msgstr "Código de la orden"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
 msgstr "Fecha de la orden"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
 msgstr "Facturas"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr "Monto de pago"
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr "Titular de la cuenta"
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr "IBAN"
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr "BIC"
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -436,18 +448,14 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr ""
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
 msgstr "Monto total"
@@ -469,14 +477,21 @@
 msgid "Download XML"
 msgstr "Descargar XML"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr ""
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/fi/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/sv/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,301 +3,313 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: 2021-01-07 03:00+0000\n"
-"Last-Translator: Jaakko Rinta-Filppula <jaakko@r-f.fi>\n"
-"Language-Team: Finnish <https://translate.pretix.eu/projects/pretix/pretix-"
-"plugin-sepadebit/fi/>\n"
-"Language: fi\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
+"PO-Revision-Date: 2020-10-07 05:00+0000\n"
+"Last-Translator: Tobias Sundgren <syrgas@gmail.com>\n"
+"Language-Team: Swedish <https://translate.pretix.eu/projects/pretix/pretix-"
+"plugin-sepadebit/sv/>\n"
+"Language: sv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 3.10.3\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
 #, fuzzy
 #| msgid "Order date"
 msgctxt "export_category"
 msgid "Order data"
-msgstr "Tilauksen päivämäärä"
+msgstr "Beställningsdatum"
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
-msgstr "Tilauskoodi"
+msgstr "Beställningsnummer"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
-msgstr "Tilauksen päivämäärä"
+msgstr "Beställningsdatum"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
-msgstr "Laskut"
+msgstr "Fakturor"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr ""
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -436,46 +448,49 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr "Vie päivämäärä"
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:89
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:19
 msgid "TEST MODE"
-msgstr ""
+msgstr "TESTLÄGE"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:103
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:110
 msgid "Orders"
-msgstr "Tilaukset"
+msgstr "Beställningar"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:106
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:113
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:11
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:15
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
-msgstr "Vientejä ei ole vielä tehty."
+msgstr ""
+
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
@@ -489,19 +504,19 @@
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:24
 #, python-format
 msgid "Total amount: %(total)s %(currency)s"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:32
 msgid "Order"
-msgstr "Tilaus"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:33
 msgid "Payment"
-msgstr ""
+msgstr "Betalning"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:34
 msgid "Mandate date"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:35
 msgid "Associated invoices"
@@ -516,15 +531,15 @@
 "The SEPA direct debit failed to be completed. Please contact the organizer "
 "of the event as soon as possible!"
 msgstr ""
 
 #: pretix_sepadebit/views.py:100
 #, python-brace-format
 msgid "Event ticket {event}-{code}"
-msgstr "Tapahtumalippu {event}-{code}"
+msgstr "Evenemangsbiljett {event}-{code}"
 
 #: pretix_sepadebit/views.py:137
 msgid ""
 "The generated file did not validate for the following reasons. Please "
 "contact pretix support for more information.\n"
 "{}"
 msgstr ""
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/fr/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/fr/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
 "PO-Revision-Date: 2023-06-17 18:00+0000\n"
 "Last-Translator: Ronan LE MEILLAT <ronan.le_meillat@highcanfly.club>\n"
-"Language-Team: French <https://translate.pretix.eu/projects/pretix/"
-"pretix-plugin-sepadebit/fr/>\n"
+"Language-Team: French <https://translate.pretix.eu/projects/pretix/pretix-"
+"plugin-sepadebit/fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
 "X-Generator: Weblate 4.17\n"
 
@@ -23,233 +23,250 @@
 msgid "SEPA Direct debit"
 msgstr "Prélèvement SEPA"
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr "Ce plugin ajoute la prise en charge du prélèvement SEPA à pretix"
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+#, fuzzy
+#| msgid "List of previous SEPA debits (CSV)"
+msgid "List of previous SEPA debits"
 msgstr "Liste des prélèvements SEPA précédents (CSV)"
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
 msgctxt "export_category"
 msgid "Order data"
 msgstr "Données de commande"
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 "Téléchargez une feuille de calcul de tous les prélèvements SEPA précédemment "
 "générés et exportés par le système. Pour créer une nouvelle exportation, "
 "utilisez la section « Prélèvements SEPA » dans le menu principal."
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr "Date d’exportation"
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+#, fuzzy
+#| msgid "Account name"
+msgid "Event name"
+msgstr "Nom du compte"
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
 msgstr "Code de commande"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
 msgstr "Date de commande"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
 msgstr "Factures"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr "Date d’exportation SEPA"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr "Montant du paiement"
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 "Le prélèvement automatique n’est pas autorisé pour cet IBAN, veuillez "
 "contacter l’organisateur de l’événement ou choisir un autre mode de paiement."
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 "Le numéro BIC {bic} ne correspond pas à l’IBAN. Veuillez vérifiez "
 "attentivement vos coordonnées bancaires. Selon nos données, le BIC correct "
 "serait {correctbic}."
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr "Prélèvement SEPA"
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 "Les paiements en mode Test ne seront débités que si vous soumettez un "
 "fichier créé en mode Test à votre banque."
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr "Espaces réservés disponibles : {list}"
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 "J’ai compris que je devais régulièrement créer des fichiers d’exportation "
 "SEPA XML et les transférer à ma banque afin que ma banque collecte les "
 "paiements des clients."
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr "Nom du créancier"
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr "IBAN du créancier"
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr "BIC du créancier"
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr "ID du créancier"
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr "Il doit s’agir d’un identifiant de créancier SEPA valide."
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr "Préfixe de référence du mandat"
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 "Celui-ci ne peut contenir que des lettres, des chiffres et les caractères "
 "spéciaux suivants: ' , . : + - / ( ) ?"
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 "Nous utiliserons cette chaîne et ajouterons le slug d’événement et le code "
 "de commande pour créer une référence de mandat SEPA unique."
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr "Délai de pré-notification"
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 "Nombre de jours entre la passation de la commande et la date d’échéance du "
 "prélèvement. Selon votre législation et les règles de votre banque, vous "
 "devrez peut-être remettre un débit au moins 5 jours avant la date d’échéance "
 "à votre banque et vous devrez peut-être même informer le client au moins 14 "
 "jours à l’avance. Nous vous recommandons de configurer au moins 7 jours."
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr "Liste de blocage IBAN"
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 "Mettez un préfixe IBAN ou IBAN par ligne. Le système n’autorisera aucun de "
 "ces IBAN.  Utile par exemple si vous avez déjà eu beaucoup de paiements "
 "échoués d’une personne spécifique. Vous pouvez également répertorier les "
 "codes de pays tels que « GB » si vous ne souhaitez jamais accepter les IBAN "
 "d’un pays spécifique."
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 "Ajouter des pays entiers à votre liste de blocage est considéré comme une "
 "discrimination SEPA, illégale dans la plupart des pays et peut entraîner de "
 "lourdes amendes de la part des chiens de garde gouvernementaux."
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr "Date d’échéance du débit le plus tôt"
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 "Date la plus proche à laquelle le prélèvement automatique peut être dû. "
 "Cette date est utilisée comme date d’échéance du prélèvement automatique si "
-"la date de commande plus l’heure de pré-notification entraînent une date d’"
-"échéance antérieure à cette date. Les clients dont les commandes ont été "
+"la date de commande plus l’heure de pré-notification entraînent une date "
+"d’échéance antérieure à cette date. Les clients dont les commandes ont été "
 "effectuées à la date d’échéance la plus proche recevront un e-mail leur "
 "rappelant les frais à venir en fonction des jours de pré-notification "
 "configurés."
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr "Objet de l’e-mail de pré-notification"
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 "Objet de l’e-mail de notification. Cet e-mail n’est envoyé que si l’option "
 "de date d’échéance du débit le plus tôt est utilisée."
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr "Corps de l’e-mail de pré-notification"
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 "Corps de l’e-mail de notification. Cet e-mail n’est envoyé que si l’option "
 "de date d’échéance du débit le plus tôt est utilisée."
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
@@ -258,109 +275,112 @@
 "collectés via un formulaire en ligne. Selon votre législation, il peut être "
 "nécessaire de les collecter sur papier (actuellement non pris en charge) "
 "pour exclure le risque de rétrofacturation. Les paiements par débit SEPA "
 "seront immédiatement marqués comme payés dans la boutique, veuillez donc le "
 "marquer comme impayé et contacter l’utilisateur si des rétrofacturations se "
 "produisent ou si les frais échouent en raison de fonds insuffisants."
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 "L’espace réservé <code>{payment_info}</code> n’est pas présent dans votre "
 "modèle d’e-mail configuré pour les notifications de paiement de commande. "
 "Ceci est légalement requis car il comprend la référence du mandat et la date "
 "d’échéance."
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 "Les champs d’e-mail de rappel de date d’échéance sont requis si la "
 "fonctionnalité de date d’échéance la plus ancienne est utilisée."
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr "Titulaire du compte"
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr "IBAN"
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr "BIC"
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 "J’accorde par la présente le mandat de prélèvement SEPA pour cet ordre (voir "
 "ci-dessous)"
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr "sera débité"
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
-#, python-format
+#: pretix_sepadebit/payment.py:421
+#, fuzzy, python-format
+#| msgid ""
+#| "We will debit the total amount of this order from your bank account by "
+#| "direct debit on or shortly after %(date)s."
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 "Nous débiterons le montant total de cette commande de votre compte bancaire "
 "par prélèvement automatique le ou peu de temps après %(date)s."
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
-"Ce paiement apparaîtra sur votre relevé bancaire en tant que %(creditor_name)"
-"s avec la référence de mandat %(reference)s et l’ID créancier %(id)s."
+"Ce paiement apparaîtra sur votre relevé bancaire en tant que "
+"%(creditor_name)s avec la référence de mandat %(reference)s et l’ID "
+"créancier %(id)s."
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 "Le réglage de l’heure de pré-notification du paiement SEPA n’est pas défini."
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 "Un rappel pour la prochaine date d’échéance du prélèvement automatique a été "
 "envoyé au client."
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr "Historique des débits SEPA"
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 "Cela supprimera les fichiers XML SEPA précédemment exportés contenant des "
 "informations bancaires."
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr "Prélèvement suivant de {debit_amount_with_currency}"
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -395,16 +415,16 @@
 "We will debit the total amount displayed above from your bank account "
 "<strong>%(iban)s</strong>. You hereby agree that the amount will be "
 "withdrawn from your bank account <strong>on or shortly after %(date)s</"
 "strong>."
 msgstr ""
 "Nous débiterons le montant total affiché ci-dessus de votre compte bancaire "
 "<strong>%(iban)s</strong>. Vous acceptez par la présente que le montant soit "
-"retiré de votre compte bancaire <strong>le ou peu de temps après "
-"%(date)s</strong>."
+"retiré de votre compte bancaire <strong>le ou peu de temps après %(date)s</"
+"strong>."
 
 #: pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_confirm.html:13
 #: pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_form.html:7
 #, python-format
 msgid ""
 "By submitting this mandate form, you authorise (A) the Creditor "
 "<strong>%(creditor)s</strong> to send instructions to your bank to debit "
@@ -547,18 +567,14 @@
 "Créer plusieurs fichiers si les débits ont des dates d’encaissement "
 "différentes (requis pour certaines banques)"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr "Fichiers XML exportés"
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr "Date d’exportation"
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr "Nombre de commandes"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
 msgstr "Montant total"
@@ -580,14 +596,23 @@
 msgid "Download XML"
 msgstr "Téléchargement XML"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr "Aucune exportation n’a encore été créée."
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+"Nous débiterons le montant total de cette commande de votre compte bancaire "
+"par prélèvement automatique le ou peu de temps après %(date)s."
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr "Export SEPA"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
@@ -623,16 +648,16 @@
 msgstr "Aucune commande n’a fait partie de cette exportation."
 
 #: pretix_sepadebit/templates/pretix_sepadebit/pending.html:2
 msgid ""
 "The SEPA direct debit failed to be completed. Please contact the organizer "
 "of the event as soon as possible!"
 msgstr ""
-"Le prélèvement SEPA n’a pas pu être effectué. Veuillez contacter l’"
-"organisateur de l’événement dès que possible !"
+"Le prélèvement SEPA n’a pas pu être effectué. Veuillez contacter "
+"l’organisateur de l’événement dès que possible !"
 
 #: pretix_sepadebit/views.py:100
 #, python-brace-format
 msgid "Event ticket {event}-{code}"
 msgstr "Billet d’événement {event}-{code}"
 
 #: pretix_sepadebit/views.py:137
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/hr/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/hr/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: hr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -20,279 +20,291 @@
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
 msgctxt "export_category"
 msgid "Order data"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr ""
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -431,18 +443,14 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr ""
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
 msgstr ""
@@ -464,14 +472,21 @@
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr ""
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/it/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/ca/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,301 +3,311 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: 2023-05-18 00:00+0000\n"
-"Last-Translator: M C <micasadmail@gmail.com>\n"
-"Language-Team: Italian <https://translate.pretix.eu/projects/pretix/"
-"pretix-plugin-sepadebit/it/>\n"
-"Language: it\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
+"PO-Revision-Date: 2020-12-15 21:00+0000\n"
+"Last-Translator: albert <albert.serra.monner@gmail.com>\n"
+"Language-Team: Catalan <https://translate.pretix.eu/projects/pretix/pretix-"
+"plugin-sepadebit/ca/>\n"
+"Language: ca\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.17\n"
+"X-Generator: Weblate 3.10.3\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
-#, fuzzy
-#| msgid "Order date"
+#: pretix_sepadebit/exporters.py:17
 msgctxt "export_category"
 msgid "Order data"
-msgstr "Data dell'ordine"
+msgstr ""
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr "Data d'exportació"
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
-msgstr "Codice ordine"
+msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
-msgstr "Data dell'ordine"
+msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
-msgstr "Fatture"
+msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr ""
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr "IBAN"
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
-msgstr ""
+msgstr "BIC"
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -388,44 +398,48 @@
 
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:38
 msgid "Due date"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:10
 msgid "In test mode, your exports will only contain test mode orders."
-msgstr ""
+msgstr "En mode de prova, les exportacions només contindran comandes de prova."
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:14
 msgid ""
 "If you want, you can now also create SEPA debit files for multiple events "
 "combined."
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:17
 msgid "Go to organizer-level exports"
-msgstr ""
+msgstr "Anar a les exportacions de nivell organitzador"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:24
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:33
 msgid ""
 "Refunds for SEPA debit transactions are grouped with bank transfer refunds."
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:27
+#, fuzzy
+#| msgid "Go to organizer-level exports"
 msgid "Go to refund exports"
-msgstr ""
+msgstr "Anar a les exportacions de nivell organitzador"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:36
+#, fuzzy
+#| msgid "Go to organizer-level exports"
 msgid "Go to organizer-level refund exports"
-msgstr ""
+msgstr "Anar a les exportacions de nivell organitzador"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:44
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:65
 msgid "Create new export file"
-msgstr ""
+msgstr "Crear un nou fitxer d'exportació"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:48
 #, python-format
 msgid ""
 "<strong>%(num_new)s</strong> SEPA debit orders have been placed and are not "
 "yet exported as Sepa XML."
 msgstr ""
@@ -436,45 +450,48 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr ""
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
-msgstr ""
+msgstr "Número de comandes"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:89
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:19
 msgid "TEST MODE"
-msgstr "MODALITA' TEST"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:103
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:110
 msgid "Orders"
-msgstr "Ordini"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:106
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:113
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:11
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:15
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
+msgstr "Encara no s'han creat exportacions."
+
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
@@ -489,19 +506,19 @@
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:24
 #, python-format
 msgid "Total amount: %(total)s %(currency)s"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:32
 msgid "Order"
-msgstr "Ordine"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:33
 msgid "Payment"
-msgstr "Pagamento"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:34
 msgid "Mandate date"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:35
 msgid "Associated invoices"
@@ -516,15 +533,15 @@
 "The SEPA direct debit failed to be completed. Please contact the organizer "
 "of the event as soon as possible!"
 msgstr ""
 
 #: pretix_sepadebit/views.py:100
 #, python-brace-format
 msgid "Event ticket {event}-{code}"
-msgstr "Biglietto dell'evento {event}-{code}"
+msgstr "Tiquet per l'acte {event}-{code}"
 
 #: pretix_sepadebit/views.py:137
 msgid ""
 "The generated file did not validate for the following reasons. Please "
 "contact pretix support for more information.\n"
 "{}"
 msgstr ""
@@ -537,8 +554,8 @@
 
 #: pretix_sepadebit/views.py:150
 msgid "A new export file has been created."
 msgstr ""
 
 #: pretix_sepadebit/views.py:152
 msgid "No valid orders have been found."
-msgstr ""
+msgstr "No s'han trobat comandes vàlides."
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/ja/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/ja/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -20,279 +20,291 @@
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
 msgctxt "export_category"
 msgid "Order data"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr ""
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -431,18 +443,14 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr ""
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
 msgstr ""
@@ -464,14 +472,21 @@
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr ""
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/lv/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/pl/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,302 +3,313 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: 2022-04-06 03:00+0000\n"
-"Last-Translator: Liga V <lerning_by_dreaming@gmx.de>\n"
-"Language-Team: Latvian <https://translate.pretix.eu/projects/pretix/pretix-"
-"plugin-sepadebit/lv/>\n"
-"Language: lv\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
+"PO-Revision-Date: 2023-11-23 05:00+0000\n"
+"Last-Translator: c0de-bender <code-bender@mailbox.org>\n"
+"Language-Team: Polish <https://translate.pretix.eu/projects/pretix/pretix-"
+"plugin-sepadebit/pl/>\n"
+"Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n % 10 == 0 || n % 100 >= 11 && n % 100 <= "
-"19) ? 0 : ((n % 10 == 1 && n % 100 != 11) ? 1 : 2);\n"
-"X-Generator: Weblate 4.11.2\n"
+"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
+"|| n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 5.1.1\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
-#, fuzzy
-#| msgid "Order date"
+#: pretix_sepadebit/exporters.py:17
 msgctxt "export_category"
 msgid "Order data"
-msgstr "Pasūtījuma datums"
+msgstr "Dane zamówienia"
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+#, fuzzy
+msgid "Export date"
+msgstr "Data wygaśnięcia"
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
-msgstr "Pasūtījuma kods"
+msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
-msgstr "Pasūtījuma datums"
+msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
-msgstr "Maksājuma summa"
+msgstr ""
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
-msgstr ""
+msgstr "Dostępne symbole zastępstwa: {list}"
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
-msgstr "Konta īpašnieks"
+msgstr ""
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
-msgstr "IBAN"
+msgstr "Numer IBAN"
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
-msgstr "BIC"
+msgstr "Numer BIC (SWIFT)"
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -326,24 +337,32 @@
 #, python-format
 msgid ""
 "By submitting this mandate form, you authorise (A) the Creditor "
 "<strong>%(creditor)s</strong> to send instructions to your bank to debit "
 "your account and (B) your bank to debit your account in accordance with the "
 "instructions from the Creditor."
 msgstr ""
+"Wypełniając ten formularz zgadzasz się na a) przesłanie przez "
+"<strong>%(creditor)s</strong> żądania do Twojego banku z prośbą o obciążenie "
+"rachunku oraz b) zrealizowanie tej prośby przez swój bank."
 
 #: pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_confirm.html:20
 #: pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_form.html:20
+#, fuzzy
 msgid ""
 "As part of your rights, you are entitled to a refund from your bank under "
 "the terms and conditions of your agreement with your bank. A refund must be "
 "claimed within 8 weeks starting from the date on which your account was "
 "debited. Your rights are explained in a statement that you can obtain from "
 "your bank."
 msgstr ""
+"Zgodnie z prawem masz prawdopodobnie osiem tygodni na zgłoszenie "
+"ewentualnych roszczeń do obciążeń swojego rachunku bankowego. Zanim "
+"podejmiesz jakiekolwiek akcje - zapoznaj się z regulaminem świadczenia usług "
+"swojego Banku."
 
 #: pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_confirm.html:27
 #: pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_form.html:27
 #, python-format
 msgid ""
 "The creditors ID is <strong>%(id)s</strong>. Your mandate reference will be "
 "sent to you via email after your order has been submitted."
@@ -437,25 +456,21 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr "Exporta datums"
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
-msgstr "Pasūtījumu skaits"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
-msgstr ""
+msgstr "Pełna kwota"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:89
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:19
 msgid "TEST MODE"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:103
@@ -467,15 +482,23 @@
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:113
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:11
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:15
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
+#, fuzzy
 msgid "No exports have been created yet."
+msgstr "Ten produkt może być anulowany"
+
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
@@ -490,15 +513,15 @@
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:24
 #, python-format
 msgid "Total amount: %(total)s %(currency)s"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:32
 msgid "Order"
-msgstr ""
+msgstr "Zamówienie"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:33
 msgid "Payment"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:34
 msgid "Mandate date"
@@ -537,9 +560,10 @@
 msgstr ""
 
 #: pretix_sepadebit/views.py:150
 msgid "A new export file has been created."
 msgstr ""
 
 #: pretix_sepadebit/views.py:152
+#, fuzzy
 msgid "No valid orders have been found."
-msgstr ""
+msgstr "Ten produkt może być anulowany"
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/nl/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/nl/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Dutch (pretix)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
 "PO-Revision-Date: 2023-11-14 23:00+0000\n"
 "Last-Translator: Thomas Vranken <thvranken@gmail.com>\n"
-"Language-Team: Dutch <https://translate.pretix.eu/projects/pretix/"
-"pretix-plugin-sepadebit/nl/>\n"
+"Language-Team: Dutch <https://translate.pretix.eu/projects/pretix/pretix-"
+"plugin-sepadebit/nl/>\n"
 "Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 5.1.1\n"
 
@@ -20,168 +20,183 @@
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 "Deze plugin voegt ondersteuning voor automatische SEPA-incasso's toe aan "
 "pretix"
 
-#: pretix_sepadebit/exporters.py:12
+#: pretix_sepadebit/exporters.py:16
 #, fuzzy
 #| msgid "List of SEPA debits (CSV)"
-msgid "List of previous SEPA debits (CSV)"
+msgid "List of previous SEPA debits"
 msgstr "Lijst van SEPA-incasso's (CSV)"
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
 #, fuzzy
 #| msgid "Order date"
 msgctxt "export_category"
 msgid "Order data"
 msgstr "Besteldatum"
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr "Exportdatum"
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+#, fuzzy
+#| msgid "Account name"
+msgid "Event name"
+msgstr "Naam rekeninghouder"
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
 msgstr "Bestelcode"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
 msgstr "Besteldatum"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
 msgstr "Facturen"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr "SEPA-exportdatum"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr "Te betalen bedrag"
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 "SEPA-incasso's zijn niet toegestaan voor dit IBAN. Neem contact op met de "
 "organisator van het evenement of kies een andere betalingsmethode."
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 "Het BIC-nummer {bic} komt niet met het IBAN overeen. Controleer uw "
 "bankgegevens. Volgens onze informatie zou het correcte BIC-nummer "
 "{correctbic} moeten zijn."
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr "SEPA-afschrijving"
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 "Betalingen in de testmodus zullen alleen worden geïncasseerd als u een "
 "bestand dat u in de testmodus heeft gemaakt indient bij uw bank."
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr "Beschikbare plaatsaanduidingen: {list}"
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 "Ik heb begrepen dat ik regelmatig SEPA XML-exportbestanden moet aanmaken en "
 "ze moet overdragen aan mijn bank om mijn bank de betalingen van de klanten "
 "te laten innen."
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr "Naam begunstigde"
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr "IBAN begunstigde"
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr "BIC begunstigde"
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr "Incassant-ID begunstigde"
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr "Dit moet een geldige SEPA-incassant ID zijn."
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr "Machtigingskenmerkvoorvoegsel"
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 "Dit mag alleen letters, cijfers, en de volgende speciale tekens bevatten: "
 "' , . : + - / ( ) ?"
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 "We zullen deze tekst gebruiken en hier de evenementsslug en bestelcode aan "
 "toevoegen om een uniek SEPA-machtigingskenmerk op te bouwen."
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr "Vooraanmeldingstijd"
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 "Aantal dagen tussen het plaatsen van de bestelling en de uitvoeringsdatum "
 "van de afschrijving. Afhankelijk van uw wetgeving en regels van uw bank kunt "
 "u verplicht zijn om een afschrijving ten minste 5 dagen voor de "
 "uitvoeringsdatum bij uw bank te melden, en u kunt zelfs verplicht zijn om de "
 "klant ten minste 14 dagen van tevoren te informeren. We raden aan om ten "
 "minste 7 dagen in te stellen."
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr "IBAN-blokkeerlijst"
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 #, fuzzy
 #| msgid ""
 #| "Put one IBAN or IBAN prefix per line. The system will not allow any of "
 #| "these IBANs. Useful e.g. if you had lots of failed payments already from "
 #| "a specific person. You can also list country codessuch as \"GB\" if you "
 #| "never want to accept IBANs from a specific country."
 msgid ""
@@ -192,65 +207,65 @@
 msgstr ""
 "Voer hier één IBAN of IBAN-voorvoegsel per regel in. Het systeem zal IBANs "
 "op deze lijst of IBANs beginnend met een voorvoegsel op deze lijst weigeren. "
 "Deze optie kan handig zijn als u al een groot aantal mislukte betalingen van "
 "een bepaalde persoon hebt gehad. U kunt hier ook landcodes zoals \"GB\" "
 "invoeren als u nooit IBANs van een bepaald land wilt accepteren."
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr "Eerste incassodatum"
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 "De eerste datum waarop automatische incasso's mogen worden uitgevoerd. Deze "
 "datum zal worden gebruikt als de datum om het incasso uit te voeren als de "
 "bestellingsdatum plus de meldingstijd in een eerdere datum zouden "
 "resulteren. Klanten die op deze datum een incasso zullen krijgen ontvangen "
 "vooraf een herinneringsmail over de afschrijving volgens de ingestelde "
 "notificatietijd."
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr "Onderwerp vooraankondigingsmail"
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 "Het onderwerp van de e-mail. Deze e-mail zal alleen worden verstuurd als de "
 "eerste incassodatum is ingesteld."
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr "Inhoud vooraankondigingsmail"
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 "De inhoud van de vooraankondigingsmail. Deze e-mail zal alleen worden "
 "verstuurd als de eerste incassodatum is ingesteld."
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
@@ -259,108 +274,110 @@
 "verzameld via een online formulier. Afhankelijk van uw wetgeving kan het "
 "nodig zijn om deze op papier te verzamelen (momenteel niet ondersteund) om "
 "de kans op storneringen te verkleinen. SEPA-incasso's zullen direct als "
 "betaald worden gemarkeerd in de winkel, markeer de bestelling als onbetaald "
 "en neem contact met de gebruiker op als een stornering plaatsvindt of de "
 "afschrijving mislukt door onvoldoende saldo."
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 "De plaatsaanduiding <code>{payment_info}</code> is niet aanwezig in uw "
 "ingestelde e-mailsjabloon voor betalingsmeldingen voor bestellingen. Dit is "
 "wettelijk verplicht, omdat hierin de mandaatreferentie en uitvoeringsdatum "
 "worden vermeld."
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 "Het is verplicht om een vooraankondigingsmail in te stellen als de eerste "
 "incassodatum is ingesteld."
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr "Rekeninghouder"
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr "IBAN"
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr "BIC"
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 "Hierbij geef ik toestemming voor de SEPA-incassomachtiging voor deze "
 "bestelling (zie onder)"
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
-#, python-format
+#: pretix_sepadebit/payment.py:421
+#, fuzzy, python-format
+#| msgid ""
+#| "We will debit the total amount of this order from your bank account by "
+#| "direct debit on or shortly after %(date)s."
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 "We zullen het totaalbedrag van deze bestelling via automatische incasso op "
 "of kort na %(date)s van uw bankrekening afschrijven."
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 "Deze betaling zal in uw bankafschriften verschijnen als %(creditor_name)s, "
 "met machtigingskenmerk %(reference)s en incassant-ID %(id)s."
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr "De vooraankondigingstijd voor SEPA-betalingen is niet ingesteld."
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 "Een herinnering van een aankomende automatische incasso is naar de klant "
 "verstuurd."
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr "SEPA-afschrijvingsgeschiedenis"
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 "Dit zal eerder geëxporteerde SEPA-XML-bestanden met bankinformatie "
 "verwijderen."
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr "Automatische afschrijving van {debit_amount_with_currency}"
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -544,18 +561,14 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr "Geëxporteerde XML-bestanden"
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr "Exportdatum"
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr "Aantal bestellingen"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
 msgstr "Totaal bedrag"
@@ -577,14 +590,23 @@
 msgid "Download XML"
 msgstr "Download XML"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr "Er zijn nog geen exports aangemaakt."
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+"We zullen het totaalbedrag van deze bestelling via automatische incasso op "
+"of kort na %(date)s van uw bankrekening afschrijven."
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr "SEPA-export"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/nl_BE/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/pt/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,296 +3,308 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: nl_BE\n"
+"Language: pt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
 msgctxt "export_category"
 msgid "Order data"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr ""
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -431,18 +443,14 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr ""
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
 msgstr ""
@@ -464,14 +472,21 @@
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr ""
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/nl_Informal/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/nl_Informal/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
 "PO-Revision-Date: 2021-08-05 04:00+0000\n"
 "Last-Translator: Maarten van den Berg <maartenberg1@gmail.com>\n"
 "Language-Team: Dutch (informal) <https://translate.pretix.eu/projects/pretix/"
 "pretix-plugin-sepadebit/nl_Informal/>\n"
 "Language: nl_Informal\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -25,168 +25,183 @@
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 "Deze plug-in voegt ondersteuning voor automatische SEPA-incasso's toe aan "
 "pretix"
 
-#: pretix_sepadebit/exporters.py:12
+#: pretix_sepadebit/exporters.py:16
 #, fuzzy
 #| msgid "List of SEPA debits (CSV)"
-msgid "List of previous SEPA debits (CSV)"
+msgid "List of previous SEPA debits"
 msgstr "Lijst van SEPA-incasso's (CSV)"
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
 #, fuzzy
 #| msgid "Order date"
 msgctxt "export_category"
 msgid "Order data"
 msgstr "Besteldatum"
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr "Exportdatum"
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+#, fuzzy
+#| msgid "Account name"
+msgid "Event name"
+msgstr "Naam rekeninghouder"
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
 msgstr "Bestelcode"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
 msgstr "Besteldatum"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
 msgstr "Facturen"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr "SEPA-exportdatum"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr "Te betalen bedrag"
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 "SEPA-incasso's zijn niet toegestaan voor dit IBAN. Neem contact op met de "
 "organisator van het evenement of kies een andere betalingsmethode."
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 "Het BIC-nummer {bic} komt niet met het IBAN overeen. Controleer je "
 "bankgegevens. Volgens onze informatie zou het juiste BIC-nummer {correctbic} "
 "moeten zijn."
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr "SEPA-afschrijving"
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 "Betalingen in de testmodus worden alleen afgeschreven als je een bestand dat "
 "je in de testmodus hebt gemaakt indient bij je bank."
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr "Beschikbare plaatsaanduidingen: {list}"
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 "Ik heb begrepen dat ik regelmatig SEPA XML-exportbestanden moet aanmaken en "
 "ze moet overdragen aan mijn bank om mijn bank de betalingen van de klanten "
 "te laten innen."
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr "Naam begunstigde"
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr "IBAN begunstigde"
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr "BIC begunstigde"
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr "Incassant-ID begunstigde"
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr "Dit moet een geldig SEPA-incassant-ID zijn."
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr "Machtigingskenmerkvoorvoegsel"
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 "Dit mag alleen letters, cijfers, en de volgende speciale tekens bevatten: "
 "' , . : + - / ( ) ?"
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 "We zullen deze tekst gebruiken en hier de evenementsslug en bestelcode aan "
 "toevoegen om een uniek SEPA-machtigingskenmerk op te bouwen."
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr "Vooraanmeldingstijd"
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 "Aantal dagen tussen het plaatsen van de bestelling en de uitvoeringsdatum "
 "van de afschrijving. Afhankelijk van je wetgeving en regels van je bank kan "
 "je verplicht zijn om een afschrijving ten minste 5 dagen voor de "
 "uitvoeringsdatum bij je bank te melden, en kan je zelfs verplicht zijn om de "
 "klant ten minste 14 dagen van tevoren te informeren. We raden aan om ten "
 "minste 7 dagen in te stellen."
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr "IBAN-blokkeerlijst"
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 #, fuzzy
 #| msgid ""
 #| "Put one IBAN or IBAN prefix per line. The system will not allow any of "
 #| "these IBANs. Useful e.g. if you had lots of failed payments already from "
 #| "a specific person. You can also list country codessuch as \"GB\" if you "
 #| "never want to accept IBANs from a specific country."
 msgid ""
@@ -197,65 +212,65 @@
 msgstr ""
 "Voer hier één IBAN of IBAN-voorvoegsel per regel in. Het systeem zal IBANs "
 "op deze lijst of IBANs beginnend met een voorvoegsel op deze lijst weigeren. "
 "Deze optie kan handig zijn als je al een groot aantal mislukte betalingen "
 "van een bepaalde persoon hebt gehad. Je kan hier ook landcodes zoals \"GB\" "
 "invoeren als jje nooit IBANs van een bepaald land wilt accepteren."
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr "Eerste incassodatum"
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 "De eerste datum waarop automatische incasso's mogen worden uitgevoerd. Deze "
 "datum zal worden gebruikt als de datum om het incasso uit te voeren als de "
 "bestellingsdatum plus de meldingstijd in een eerdere datum zouden "
 "resulteren. Klanten die op deze datum een incasso zullen krijgen ontvangen "
 "vooraf een herinneringsmail over de afschrijving volgens de ingestelde "
 "notificatietijd."
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr "Onderwerp vooraankondigingsmail"
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 "Het onderwerp van de e-mail. Deze e-mail zal alleen worden verstuurd als de "
 "eerste incassodatum is ingesteld."
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr "Inhoud vooraankondigingsmail"
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 "De inhoud van de vooraankondigingsmail. Deze e-mail zal alleen worden "
 "verstuurd als de eerste incassodatum is ingesteld."
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
@@ -264,108 +279,110 @@
 "verzameld via een online formulier. Afhankelijk van je wetgeving kan het "
 "nodig zijn om deze op papier te verzamelen (momenteel niet ondersteund) om "
 "de kans op storneringen te verkleinen. SEPA-incasso's zullen direct als "
 "betaald worden gemarkeerd in de winkel, markeer de bestelling als onbetaald "
 "en neem contact met de gebruiker op als een stornering plaatsvindt of de "
 "afschrijving mislukt door onvoldoende saldo."
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 "De plaatsaanduiding <code>{payment_info}</code> is niet aanwezig in je "
 "ingestelde e-mailsjabloon voor betalingsmeldingen voor bestellingen. Dit is "
 "wettelijk verplicht, omdat hierin de mandaatreferentie en uitvoeringsdatum "
 "worden vermeld."
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 "Het is verplicht om een vooraankondigingsmail in te stellen als de eerste "
 "incassodatum is ingesteld."
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr "Rekeninghouder"
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr "IBAN"
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr "BIC"
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 "Hierbij geef ik toestemming voor de SEPA-incassomachtiging voor deze "
 "bestelling (zie onder)"
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
-#, python-format
+#: pretix_sepadebit/payment.py:421
+#, fuzzy, python-format
+#| msgid ""
+#| "We will debit the total amount of this order from your bank account by "
+#| "direct debit on or shortly after %(date)s."
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 "We zullen het totaalbedrag van deze bestelling op of kort na %(date)s van je "
 "bankrekening afschrijven via automatische incasso."
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 "Deze betaling zal in je bankafschriften verschijnen als %(creditor_name)s, "
 "met machtigingskenmerk %(reference)s en incassant-ID %(id)s."
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr "De vooraankondigingstijd voor SEPA-betalingen is niet ingesteld."
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 "Een herinnering van een aankomende automatische incasso is naar de klant "
 "verstuurd."
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr "SEPA-afschrijvingsgeschiedenis"
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 "Dit zal eerder geëxporteerde SEPA-XML-bestanden met bankinformatie "
 "verwijderen."
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr "Automatische afschrijving van {debit_amount_with_currency}"
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -549,18 +566,14 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr "Geëxporteerde XML-bestanden"
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr "Exportdatum"
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr "Aantal bestellingen"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
 msgstr "Totaalbedrag"
@@ -582,14 +595,23 @@
 msgid "Download XML"
 msgstr "Download XML"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr "Er zijn nog geen exports aangemaakt."
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+"We zullen het totaalbedrag van deze bestelling op of kort na %(date)s van je "
+"bankrekening afschrijven via automatische incasso."
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr "SEPA-export"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/pl/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/da/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -3,300 +3,313 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: 2023-11-23 05:00+0000\n"
-"Last-Translator: c0de-bender <code-bender@mailbox.org>\n"
-"Language-Team: Polish <https://translate.pretix.eu/projects/pretix/"
-"pretix-plugin-sepadebit/pl/>\n"
-"Language: pl\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
+"PO-Revision-Date: 2018-03-20 21:00+0000\n"
+"Last-Translator: Mikkel Ricky <rimi@aarhus.dk>\n"
+"Language-Team: Danish <https://translate.pretix.eu/projects/pretix/pretix-"
+"plugin-sepadebit/da/>\n"
+"Language: da\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
-"|| n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 5.1.1\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 2.19.1\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
+#, fuzzy
+#| msgid "Order date"
 msgctxt "export_category"
 msgid "Order data"
-msgstr "Dane zamówienia"
+msgstr "Bestillingsdato"
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
-msgid "Order code"
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
-msgid "Order date"
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
-msgid "Invoices"
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
+msgid "Order code"
+msgstr "Bestillingskode"
+
+#: pretix_sepadebit/exporters.py:40
+msgid "Order date"
+msgstr "Bestillingsdato"
+
+#: pretix_sepadebit/exporters.py:41
+msgid "Invoices"
+msgstr "Fakturaer"
+
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr ""
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
-msgstr "Dostępne symbole zastępstwa: {list}"
+msgstr ""
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
-msgstr ""
+msgstr "Kontoejer"
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
-msgstr "Numer IBAN"
+msgstr ""
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
-msgstr "Numer BIC (SWIFT)"
+msgstr ""
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -324,32 +337,24 @@
 #, python-format
 msgid ""
 "By submitting this mandate form, you authorise (A) the Creditor "
 "<strong>%(creditor)s</strong> to send instructions to your bank to debit "
 "your account and (B) your bank to debit your account in accordance with the "
 "instructions from the Creditor."
 msgstr ""
-"Wypełniając ten formularz zgadzasz się na a) przesłanie przez "
-"<strong>%(creditor)s</strong> żądania do Twojego banku z prośbą o obciążenie "
-"rachunku oraz b) zrealizowanie tej prośby przez swój bank."
 
 #: pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_confirm.html:20
 #: pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_form.html:20
-#, fuzzy
 msgid ""
 "As part of your rights, you are entitled to a refund from your bank under "
 "the terms and conditions of your agreement with your bank. A refund must be "
 "claimed within 8 weeks starting from the date on which your account was "
 "debited. Your rights are explained in a statement that you can obtain from "
 "your bank."
 msgstr ""
-"Zgodnie z prawem masz prawdopodobnie osiem tygodni na zgłoszenie "
-"ewentualnych roszczeń do obciążeń swojego rachunku bankowego. Zanim "
-"podejmiesz jakiekolwiek akcje - zapoznaj się z regulaminem świadczenia usług "
-"swojego Banku."
 
 #: pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_confirm.html:27
 #: pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_form.html:27
 #, python-format
 msgid ""
 "The creditors ID is <strong>%(id)s</strong>. Your mandate reference will be "
 "sent to you via email after your order has been submitted."
@@ -443,48 +448,49 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-#, fuzzy
-msgid "Export date"
-msgstr "Data wygaśnięcia"
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
-msgstr "Pełna kwota"
+msgstr "Samlet beløb"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:89
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:19
 msgid "TEST MODE"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:103
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:110
 msgid "Orders"
-msgstr ""
+msgstr "Bestillinger"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:106
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:113
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:11
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:15
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
-#, fuzzy
 msgid "No exports have been created yet."
-msgstr "Ten produkt może być anulowany"
+msgstr ""
+
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
@@ -498,23 +504,25 @@
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:24
 #, python-format
 msgid "Total amount: %(total)s %(currency)s"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:32
 msgid "Order"
-msgstr "Zamówienie"
+msgstr "Rækkefølge"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:33
 msgid "Payment"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:34
+#, fuzzy
+#| msgid "Order date"
 msgid "Mandate date"
-msgstr ""
+msgstr "Bestillingsdato"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:35
 msgid "Associated invoices"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:70
 msgid "No orders have been part of this export."
@@ -545,10 +553,9 @@
 msgstr ""
 
 #: pretix_sepadebit/views.py:150
 msgid "A new export file has been created."
 msgstr ""
 
 #: pretix_sepadebit/views.py:152
-#, fuzzy
 msgid "No valid orders have been found."
-msgstr "Ten produkt może być anulowany"
+msgstr ""
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/pl_Informal/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/ru/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,296 +3,308 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: pl_Informal\n"
+"Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
 msgctxt "export_category"
 msgid "Order data"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr ""
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -431,18 +443,14 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr ""
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
 msgstr ""
@@ -464,14 +472,21 @@
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr ""
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/pt/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/django.pot`

 * *Files 2% similar despite different names*

```diff
@@ -1,298 +1,311 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
+#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
+"POT-Creation-Date: 2024-05-07 11:50+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Automatically generated\n"
-"Language-Team: none\n"
-"Language: pt\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
 msgctxt "export_category"
 msgid "Order data"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr ""
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -431,18 +444,14 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr ""
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
 msgstr ""
@@ -464,14 +473,21 @@
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr ""
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/pt_BR/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -3,301 +3,313 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: 2018-03-15 08:54+0000\n"
-"Last-Translator: Matheus Nunes <matheus@integrate.com.br>\n"
-"Language-Team: Portuguese (Brazil) <https://translate.pretix.eu/projects/"
-"pretix/pretix-plugin-sepadebit/pt_BR/>\n"
-"Language: pt_BR\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
+"PO-Revision-Date: 2019-10-23 21:00+0000\n"
+"Last-Translator: yichengsd <sunzl@jxepub.com>\n"
+"Language-Team: Chinese (Simplified) <https://translate.pretix.eu/projects/"
+"pretix/pretix-plugin-sepadebit/zh_Hans/>\n"
+"Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 2.19.1\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Generator: Weblate 3.5.1\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
 #, fuzzy
 #| msgid "Order date"
 msgctxt "export_category"
 msgid "Order data"
-msgstr "Data do pedido"
+msgstr "订单日期"
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
-msgstr "Código do pedido"
+msgstr "订单代码"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
-msgstr "Data do pedido"
+msgstr "订单日期"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
-msgstr ""
+msgstr "发票"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
-msgstr ""
+msgstr "支付金额"
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
-msgstr ""
+msgstr "账户持有人"
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
-msgstr ""
+msgstr "国际银行账号"
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
-msgstr ""
+msgstr "BIC"
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -436,47 +448,50 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr ""
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
-msgstr ""
+msgstr "总价"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:89
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:19
 msgid "TEST MODE"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:103
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:110
 msgid "Orders"
-msgstr ""
+msgstr "订单"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:106
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:113
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:11
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:15
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr ""
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
@@ -489,25 +504,23 @@
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:24
 #, python-format
 msgid "Total amount: %(total)s %(currency)s"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:32
 msgid "Order"
-msgstr ""
+msgstr "订单"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:33
 msgid "Payment"
-msgstr ""
+msgstr "支付"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:34
-#, fuzzy
-#| msgid "Order date"
 msgid "Mandate date"
-msgstr "Data do pedido"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:35
 msgid "Associated invoices"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:70
 msgid "No orders have been part of this export."
@@ -518,15 +531,15 @@
 "The SEPA direct debit failed to be completed. Please contact the organizer "
 "of the event as soon as possible!"
 msgstr ""
 
 #: pretix_sepadebit/views.py:100
 #, python-brace-format
 msgid "Event ticket {event}-{code}"
-msgstr ""
+msgstr "活动门票{event}-{code}"
 
 #: pretix_sepadebit/views.py:137
 msgid ""
 "The generated file did not validate for the following reasons. Please "
 "contact pretix support for more information.\n"
 "{}"
 msgstr ""
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/ru/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/it/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,296 +3,313 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Automatically generated\n"
-"Language-Team: none\n"
-"Language: ru\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
+"PO-Revision-Date: 2023-05-18 00:00+0000\n"
+"Last-Translator: M C <micasadmail@gmail.com>\n"
+"Language-Team: Italian <https://translate.pretix.eu/projects/pretix/pretix-"
+"plugin-sepadebit/it/>\n"
+"Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.17\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
+#, fuzzy
+#| msgid "Order date"
 msgctxt "export_category"
 msgid "Order data"
-msgstr ""
+msgstr "Data dell'ordine"
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
-msgid "Order code"
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
-msgid "Order date"
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
-msgid "Invoices"
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
+msgid "Order code"
+msgstr "Codice ordine"
+
+#: pretix_sepadebit/exporters.py:40
+msgid "Order date"
+msgstr "Data dell'ordine"
+
+#: pretix_sepadebit/exporters.py:41
+msgid "Invoices"
+msgstr "Fatture"
+
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr ""
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
-msgstr ""
+msgstr "IBAN"
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -431,47 +448,50 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr ""
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:89
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:19
 msgid "TEST MODE"
-msgstr ""
+msgstr "MODALITA' TEST"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:103
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:110
 msgid "Orders"
-msgstr ""
+msgstr "Ordini"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:106
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:113
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:11
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:15
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr ""
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
@@ -484,19 +504,19 @@
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:24
 #, python-format
 msgid "Total amount: %(total)s %(currency)s"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:32
 msgid "Order"
-msgstr ""
+msgstr "Ordine"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:33
 msgid "Payment"
-msgstr ""
+msgstr "Pagamento"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:34
 msgid "Mandate date"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:35
 msgid "Associated invoices"
@@ -511,15 +531,15 @@
 "The SEPA direct debit failed to be completed. Please contact the organizer "
 "of the event as soon as possible!"
 msgstr ""
 
 #: pretix_sepadebit/views.py:100
 #, python-brace-format
 msgid "Event ticket {event}-{code}"
-msgstr ""
+msgstr "Biglietto dell'evento {event}-{code}"
 
 #: pretix_sepadebit/views.py:137
 msgid ""
 "The generated file did not validate for the following reasons. Please "
 "contact pretix support for more information.\n"
 "{}"
 msgstr ""
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/si/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/nl_BE/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,303 +1,311 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
+#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: 2021-03-03 02:51+0000\n"
-"Last-Translator: helabasa <R45XvezA@pm.me>\n"
-"Language-Team: Sinhala <https://translate.pretix.eu/projects/pretix/pretix-"
-"plugin-sepadebit/si/>\n"
-"Language: si\n"
+"POT-Creation-Date: 2024-05-07 11:50+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.4.2\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
-#, fuzzy
-#| msgid "Order code"
+#: pretix_sepadebit/exporters.py:17
 msgctxt "export_category"
 msgid "Order data"
-msgstr "ඇණවුම් කේතය"
+msgstr ""
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
-msgstr "ඇණවුම් කේතය"
+msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr ""
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -436,18 +444,14 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr ""
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
 msgstr ""
@@ -469,14 +473,21 @@
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr ""
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/sl/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -3,300 +3,313 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: 2021-03-01 23:24+0000\n"
-"Last-Translator: lapor-kris <kristijan.tkalec@posteo.si>\n"
-"Language-Team: Slovenian <https://translate.pretix.eu/projects/pretix/pretix-"
-"plugin-sepadebit/sl/>\n"
-"Language: sl\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
+"PO-Revision-Date: 2018-03-15 08:54+0000\n"
+"Last-Translator: Matheus Nunes <matheus@integrate.com.br>\n"
+"Language-Team: Portuguese (Brazil) <https://translate.pretix.eu/projects/"
+"pretix/pretix-plugin-sepadebit/pt_BR/>\n"
+"Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
-"n%100==4 ? 2 : 3;\n"
-"X-Generator: Weblate 4.4.2\n"
+"Plural-Forms: nplurals=2; plural=n > 1;\n"
+"X-Generator: Weblate 2.19.1\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
+#, fuzzy
+#| msgid "Order date"
 msgctxt "export_category"
 msgid "Order data"
-msgstr ""
+msgstr "Data do pedido"
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
-msgid "Order code"
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
-msgid "Order date"
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:40
+msgid "Order code"
+msgstr "Código do pedido"
+
+#: pretix_sepadebit/exporters.py:40
+msgid "Order date"
+msgstr "Data do pedido"
+
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr ""
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -435,18 +448,14 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr ""
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
 msgstr ""
@@ -468,14 +477,21 @@
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr ""
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
@@ -492,19 +508,21 @@
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:32
 msgid "Order"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:33
 msgid "Payment"
-msgstr "Plačilo"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:34
+#, fuzzy
+#| msgid "Order date"
 msgid "Mandate date"
-msgstr ""
+msgstr "Data do pedido"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:35
 msgid "Associated invoices"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:70
 msgid "No orders have been part of this export."
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/sv/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/pl_Informal/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -3,301 +3,308 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: 2020-10-07 05:00+0000\n"
-"Last-Translator: Tobias Sundgren <syrgas@gmail.com>\n"
-"Language-Team: Swedish <https://translate.pretix.eu/projects/pretix/pretix-"
-"plugin-sepadebit/sv/>\n"
-"Language: sv\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: Automatically generated\n"
+"Language-Team: none\n"
+"Language: pl_Informal\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 3.10.3\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
-#, fuzzy
-#| msgid "Order date"
+#: pretix_sepadebit/exporters.py:17
 msgctxt "export_category"
 msgid "Order data"
-msgstr "Beställningsdatum"
+msgstr ""
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
-msgstr "Beställningsnummer"
+msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
-msgstr "Beställningsdatum"
+msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
-msgstr "Fakturor"
+msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
 msgstr ""
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -436,47 +443,50 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr ""
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:89
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:19
 msgid "TEST MODE"
-msgstr "TESTLÄGE"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:103
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:110
 msgid "Orders"
-msgstr "Beställningar"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:106
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:113
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:11
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:15
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr ""
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
@@ -493,15 +503,15 @@
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:32
 msgid "Order"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:33
 msgid "Payment"
-msgstr "Betalning"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:34
 msgid "Mandate date"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:35
 msgid "Associated invoices"
@@ -516,15 +526,15 @@
 "The SEPA direct debit failed to be completed. Please contact the organizer "
 "of the event as soon as possible!"
 msgstr ""
 
 #: pretix_sepadebit/views.py:100
 #, python-brace-format
 msgid "Event ticket {event}-{code}"
-msgstr "Evenemangsbiljett {event}-{code}"
+msgstr ""
 
 #: pretix_sepadebit/views.py:137
 msgid ""
 "The generated file did not validate for the following reasons. Please "
 "contact pretix support for more information.\n"
 "{}"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/uk/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/sl/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -3,300 +3,312 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: 2022-05-07 22:00+0000\n"
-"Last-Translator: Iryna N <in380@nyu.edu>\n"
-"Language-Team: Ukrainian <https://translate.pretix.eu/projects/pretix/pretix-"
-"plugin-sepadebit/uk/>\n"
-"Language: uk\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
+"PO-Revision-Date: 2021-03-01 23:24+0000\n"
+"Last-Translator: lapor-kris <kristijan.tkalec@posteo.si>\n"
+"Language-Team: Slovenian <https://translate.pretix.eu/projects/pretix/pretix-"
+"plugin-sepadebit/sl/>\n"
+"Language: sl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.12\n"
+"Plural-Forms: nplurals=4; plural=n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
+"n%100==4 ? 2 : 3;\n"
+"X-Generator: Weblate 4.4.2\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
 msgctxt "export_category"
 msgid "Order data"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
-msgstr "Сума оплати"
+msgstr ""
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
-msgstr "Доступні заповнювачі: {list}"
+msgstr ""
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -435,25 +447,21 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr ""
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
-msgstr "Загальна сума"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:89
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:19
 msgid "TEST MODE"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:103
@@ -468,14 +476,21 @@
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr ""
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
@@ -492,15 +507,15 @@
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:32
 msgid "Order"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:33
 msgid "Payment"
-msgstr "Оплата"
+msgstr "Plačilo"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:34
 msgid "Mandate date"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:35
 msgid "Associated invoices"
@@ -515,15 +530,15 @@
 "The SEPA direct debit failed to be completed. Please contact the organizer "
 "of the event as soon as possible!"
 msgstr ""
 
 #: pretix_sepadebit/views.py:100
 #, python-brace-format
 msgid "Event ticket {event}-{code}"
-msgstr "Квиток на подію {event}-{code}"
+msgstr ""
 
 #: pretix_sepadebit/views.py:137
 msgid ""
 "The generated file did not validate for the following reasons. Please "
 "contact pretix support for more information.\n"
 "{}"
 msgstr ""
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/locale/zh_Hans/LC_MESSAGES/django.po` & `pretix_sepadebit-2.5.0/pretix_sepadebit/locale/si/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -3,301 +3,313 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: 2019-10-23 21:00+0000\n"
-"Last-Translator: yichengsd <sunzl@jxepub.com>\n"
-"Language-Team: Chinese (Simplified) <https://translate.pretix.eu/projects/"
-"pretix/pretix-plugin-sepadebit/zh_Hans/>\n"
-"Language: zh_Hans\n"
+"POT-Creation-Date: 2024-05-07 11:42+0200\n"
+"PO-Revision-Date: 2021-03-03 02:51+0000\n"
+"Last-Translator: helabasa <R45XvezA@pm.me>\n"
+"Language-Team: Sinhala <https://translate.pretix.eu/projects/pretix/pretix-"
+"plugin-sepadebit/si/>\n"
+"Language: si\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 3.5.1\n"
+"Plural-Forms: nplurals=2; plural=n > 1;\n"
+"X-Generator: Weblate 4.4.2\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:12
-msgid "List of previous SEPA debits (CSV)"
+#: pretix_sepadebit/exporters.py:16
+msgid "List of previous SEPA debits"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:13
+#: pretix_sepadebit/exporters.py:17
 #, fuzzy
-#| msgid "Order date"
+#| msgid "Order code"
 msgctxt "export_category"
 msgid "Order data"
-msgstr "订单日期"
+msgstr "ඇණවුම් කේතය"
 
-#: pretix_sepadebit/exporters.py:14
+#: pretix_sepadebit/exporters.py:18
 msgid ""
 "Download a spreadsheet of all SEPA debits that have previously been "
 "generated and exported by the system. To create a new export, use the \"SEPA "
 "debit\" section in the main menu."
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:28
+#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
+msgid "Export date"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event slug"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:39
+msgid "Event name"
+msgstr ""
+
+#: pretix_sepadebit/exporters.py:40
 msgid "Order code"
-msgstr "订单代码"
+msgstr "ඇණවුම් කේතය"
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:40
 msgid "Order date"
-msgstr "订单日期"
+msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:41
 msgid "Invoices"
-msgstr "发票"
+msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:42
 msgid "SEPA export date"
 msgstr ""
 
-#: pretix_sepadebit/exporters.py:24
+#: pretix_sepadebit/exporters.py:43
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
-msgstr "支付金额"
+msgstr ""
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:57
+#: pretix_sepadebit/payment.py:61
 #, python-brace-format
 msgid ""
 "The BIC number {bic} does not match the IBAN. Please double, check your "
 "banking details. According to our data, the correct BIC would be "
 "{correctbic}."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:68 pretix_sepadebit/signals.py:46
+#: pretix_sepadebit/payment.py:72 pretix_sepadebit/signals.py:46
 #: pretix_sepadebit/signals.py:66
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:5
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:7
 msgid "SEPA debit"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:74
+#: pretix_sepadebit/payment.py:78
 msgid ""
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:83
+#: pretix_sepadebit/payment.py:87
 #, python-brace-format
 msgid "Available placeholders: {list}"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:96
+#: pretix_sepadebit/payment.py:100
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:102
+#: pretix_sepadebit/payment.py:106
 msgid "Creditor name"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:107
+#: pretix_sepadebit/payment.py:111
 msgid "Creditor IBAN"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:111
+#: pretix_sepadebit/payment.py:115
 msgid "Creditor BIC"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:115
+#: pretix_sepadebit/payment.py:119
 msgid "Creditor ID"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:120
+#: pretix_sepadebit/payment.py:124
 msgid "This must be a valid SEPA creditor ID."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:127
+#: pretix_sepadebit/payment.py:131
 msgid "Mandate reference prefix"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:131
+#: pretix_sepadebit/payment.py:135
 msgid ""
 "This may only contain letters, numbers, and the following special "
 "characters: ' , . : + - / ( ) ?"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:136
+#: pretix_sepadebit/payment.py:140
 msgid ""
 "We will use this string and append the event slug and the order code to "
 "build a unique SEPA mandate reference."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:142
+#: pretix_sepadebit/payment.py:146
 msgid "Pre-notification time"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:143
+#: pretix_sepadebit/payment.py:147
 msgid ""
 "Number of days between the placement of the order and the due date of the "
 "direct debit. Depending on your legislation and your bank rules, you might "
 "be required to hand in a debit at least 5 days before the due date at your "
 "bank and you might even be required to inform the customer at least 14 days "
 "beforehand. We recommend configuring at least 7 days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:151
+#: pretix_sepadebit/payment.py:155
 msgid "IBAN blocklist"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:155
+#: pretix_sepadebit/payment.py:159
 msgid ""
 "Put one IBAN or IBAN prefix per line. The system will not allow any of these "
 "IBANs.  Useful e.g. if you had lots of failed payments already from a "
 "specific person. You can also list country codes such as \"GB\" if you never "
 "want to accept IBANs from a specific country."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:158
+#: pretix_sepadebit/payment.py:162
 msgid ""
 "Adding whole countries to your blocklist is considered SEPA discrimination, "
 "illegal in most countries and can be cause for hefty fines from government "
 "watchdogs."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:164
+#: pretix_sepadebit/payment.py:168
 msgid "Earliest debit due date"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:165
+#: pretix_sepadebit/payment.py:169
 msgid ""
 "Earliest date the direct debit can be due. This date is used as the direct "
 "debit due date if the order date plus pre-notification time would result in "
 "a due date earlier than this. Customers with orders using the earliest due "
 "date will receive an email reminding them about the upcoming charge based on "
 "the configured pre-notification days."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:175
+#: pretix_sepadebit/payment.py:179
 msgid "Pre-notification mail subject"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:176
+#: pretix_sepadebit/payment.py:180
 msgid ""
 "The subject of the notification email. This email is only sent if the "
 "earliest debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:188
+#: pretix_sepadebit/payment.py:192
 msgid "Pre-notification mail body"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:189
+#: pretix_sepadebit/payment.py:193
 msgid ""
 "The body of the notification email. This email is only sent if the earliest "
 "debit due date option is used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:213
+#: pretix_sepadebit/payment.py:217
 msgid ""
 "If you activate this payment method, SEPA direct debit mandates will be "
 "collected via an online form. Depending on your legislation, it might be "
 "necessary to collect them on paper (currently not supported) to exclude the "
 "risk of charge backs. SEPA debit payments will be immediately marked as paid "
 "in the shop, so please mark it as unpaid and contact the user if any charge "
 "backs occur or the charge fails due to insufficient funds."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:221
+#: pretix_sepadebit/payment.py:225
 #, python-brace-format
 msgid ""
 "The placeholder <code>{payment_info}</code> is not present in your "
 "configured email template for order payment notifications. This is legally "
 "required as it includes the mandate reference and the due date."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:239
+#: pretix_sepadebit/payment.py:243
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:244
+#: pretix_sepadebit/payment.py:248
 msgid "Account holder"
-msgstr "账户持有人"
+msgstr ""
 
-#: pretix_sepadebit/payment.py:245
+#: pretix_sepadebit/payment.py:249
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
-msgstr "国际银行账号"
+msgstr ""
 
-#: pretix_sepadebit/payment.py:246
+#: pretix_sepadebit/payment.py:250
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
-msgstr "BIC"
+msgstr ""
 
-#: pretix_sepadebit/payment.py:248
+#: pretix_sepadebit/payment.py:252
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:410
+#: pretix_sepadebit/payment.py:414
 msgid "will be debited"
 msgstr ""
 
-#: pretix_sepadebit/payment.py:416
-#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#: pretix_sepadebit/payment.py:421
 #, python-format
 msgid ""
-"We will debit the total amount of this order from your bank account by "
-"direct debit on or shortly after %(date)s."
+"We will debit the total amount of this order from your bank account "
+"%(account)s by direct debit on or shortly after %(date)s."
 msgstr ""
 
-#: pretix_sepadebit/payment.py:421
+#: pretix_sepadebit/payment.py:427
 #: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:6
 #, python-format
 msgid ""
 "This payment will appear on your bank statement as %(creditor_name)s with "
 "mandate reference %(reference)s and creditor ID %(id)s."
 msgstr ""
 
 #: pretix_sepadebit/signals.py:36
 msgid "Pre-notification time setting of SEPA Payment isn't set."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:195
+#: pretix_sepadebit/signals.py:201
 msgid ""
 "A reminder for the upcoming direct debit due date has been sent to the "
 "customer."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:199
+#: pretix_sepadebit/signals.py:205
 msgid "SEPA debit history"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:201
+#: pretix_sepadebit/signals.py:207
 msgid ""
 "This will remove previously exported SEPA XML files containing banking "
 "information."
 msgstr ""
 
-#: pretix_sepadebit/signals.py:226
+#: pretix_sepadebit/signals.py:232
 #, python-brace-format
 msgid "Upcomming debit of {debit_amount_with_currency}"
 msgstr ""
 
-#: pretix_sepadebit/signals.py:236
+#: pretix_sepadebit/signals.py:242
 #, python-brace-format
 msgid ""
 "Hello,\n"
 "\n"
 "you ordered a ticket for {event}.\n"
 "\n"
 "We will debit your bank account {iban} on or shortly after {due_date}. The "
@@ -436,47 +448,50 @@
 "(required for some banks)"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:72
 msgid "Exported XML files"
 msgstr ""
 
-#: pretix_sepadebit/templates/pretix_sepadebit/export.html:77
-msgid "Export date"
-msgstr ""
-
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:78
 msgid "Number of orders"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:79
 msgid "Total amount"
-msgstr "总价"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:89
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:19
 msgid "TEST MODE"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:103
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:110
 msgid "Orders"
-msgstr "订单"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:106
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:113
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:11
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:15
 msgid "Download XML"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/export.html:121
 msgid "No exports have been created yet."
 msgstr ""
 
+#: pretix_sepadebit/templates/pretix_sepadebit/mail.txt:2
+#, python-format
+msgid ""
+"We will debit the total amount of this order from your bank account by "
+"direct debit on or shortly after %(date)s."
+msgstr ""
+
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:5
 msgid "SEPA export"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:8
 #, python-format
 msgid "SEPA export: %(date)s"
@@ -489,19 +504,19 @@
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:24
 #, python-format
 msgid "Total amount: %(total)s %(currency)s"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:32
 msgid "Order"
-msgstr "订单"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:33
 msgid "Payment"
-msgstr "支付"
+msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:34
 msgid "Mandate date"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:35
 msgid "Associated invoices"
@@ -516,15 +531,15 @@
 "The SEPA direct debit failed to be completed. Please contact the organizer "
 "of the event as soon as possible!"
 msgstr ""
 
 #: pretix_sepadebit/views.py:100
 #, python-brace-format
 msgid "Event ticket {event}-{code}"
-msgstr "活动门票{event}-{code}"
+msgstr ""
 
 #: pretix_sepadebit/views.py:137
 msgid ""
 "The generated file did not validate for the following reasons. Please "
 "contact pretix support for more information.\n"
 "{}"
 msgstr ""
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/migrations/0001_initial.py` & `pretix_sepadebit-2.5.0/pretix_sepadebit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/migrations/0002_auto_20170530_1527.py` & `pretix_sepadebit-2.5.0/pretix_sepadebit/migrations/0002_auto_20170530_1527.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/migrations/0003_sepaexportorder_payment.py` & `pretix_sepadebit-2.5.0/pretix_sepadebit/migrations/0003_sepaexportorder_payment.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/migrations/0005_auto_20190429_0811.py` & `pretix_sepadebit-2.5.0/pretix_sepadebit/migrations/0005_auto_20190429_0811.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/migrations/0007_sepaduedate.py` & `pretix_sepadebit-2.5.0/pretix_sepadebit/migrations/0007_sepaduedate.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/migrations/0008_alter_sepaduedate_payment.py` & `pretix_sepadebit-2.5.0/pretix_sepadebit/migrations/0008_alter_sepaduedate_payment.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/models.py` & `pretix_sepadebit-2.5.0/pretix_sepadebit/models.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/payment.py` & `pretix_sepadebit-2.5.0/pretix_sepadebit/payment.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,17 +413,19 @@
         if order.status == Order.STATUS_PAID:
             return _('will be debited')
 
     def render_invoice_text(self, order, payment: OrderPayment) -> str:
         ref = '%s-%s' % (self.event.slug.upper(), order.code)
         if self.settings.reference_prefix:
             ref = self.settings.reference_prefix + "-" + ref
-        t = _("We will debit the total amount of this order from your bank account by "
+        iban_redacted = 'XXXX ' + payment.info_data.get('iban', '')[-4:]
+        t = _("We will debit the total amount of this order from your bank account %(account)s by "
               "direct debit on or shortly after %(date)s.") % {
-            'date': date_format(self._due_date(order), 'SHORT_DATE_FORMAT')
+            'date': date_format(self._due_date(order), 'SHORT_DATE_FORMAT'),
+            'account': iban_redacted,
         }
         t += " "
         t += _("This payment will appear on your bank statement as %(creditor_name)s with "
                "mandate reference %(reference)s and creditor ID %(id)s.") % {
             'reference': ref,
             'id': self.settings.creditor_id,
             'creditor_name': self.settings.creditor_name,
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/signals.py` & `pretix_sepadebit-2.5.0/pretix_sepadebit/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_confirm.html` & `pretix_sepadebit-2.5.0/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_confirm.html`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_form.html` & `pretix_sepadebit-2.5.0/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_form.html`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/templates/pretix_sepadebit/control.html` & `pretix_sepadebit-2.5.0/pretix_sepadebit/templates/pretix_sepadebit/control.html`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/templates/pretix_sepadebit/export.html` & `pretix_sepadebit-2.5.0/pretix_sepadebit/templates/pretix_sepadebit/export.html`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/templates/pretix_sepadebit/orders.html` & `pretix_sepadebit-2.5.0/pretix_sepadebit/templates/pretix_sepadebit/orders.html`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/tests/test_payment.py` & `pretix_sepadebit-2.5.0/pretix_sepadebit/tests/test_payment.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/urls.py` & `pretix_sepadebit-2.5.0/pretix_sepadebit/urls.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit/views.py` & `pretix_sepadebit-2.5.0/pretix_sepadebit/views.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit.egg-info/PKG-INFO` & `pretix_sepadebit-2.5.0/pretix_sepadebit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-sepadebit
-Version: 2.4.2
+Version: 2.5.0
 Summary: This plugin adds SEPA direct debit support to pretix
 Author-email: pretix team <support@pretix.eu>
 Maintainer-email: pretix team <support@pretix.eu>
 License: Copyright 2017 Raphael Michel
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
```

### Comparing `pretix-sepadebit-2.4.2/pretix_sepadebit.egg-info/SOURCES.txt` & `pretix_sepadebit-2.5.0/pretix_sepadebit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 pretix_sepadebit/locale/nl_Informal/LC_MESSAGES/django.po
 pretix_sepadebit/locale/pl/LC_MESSAGES/django.po
 pretix_sepadebit/locale/pl_Informal/LC_MESSAGES/django.po
 pretix_sepadebit/locale/pt/LC_MESSAGES/django.po
 pretix_sepadebit/locale/pt_BR/LC_MESSAGES/django.po
 pretix_sepadebit/locale/ru/LC_MESSAGES/django.po
 pretix_sepadebit/locale/si/LC_MESSAGES/django.po
+pretix_sepadebit/locale/sk/LC_MESSAGES/django.po
 pretix_sepadebit/locale/sl/LC_MESSAGES/django.po
 pretix_sepadebit/locale/sv/LC_MESSAGES/django.po
 pretix_sepadebit/locale/uk/LC_MESSAGES/django.po
 pretix_sepadebit/locale/zh_Hans/LC_MESSAGES/django.po
 pretix_sepadebit/migrations/0001_initial.py
 pretix_sepadebit/migrations/0002_auto_20170530_1527.py
 pretix_sepadebit/migrations/0003_sepaexportorder_payment.py
```

### Comparing `pretix-sepadebit-2.4.2/pyproject.toml` & `pretix_sepadebit-2.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.2/setup.cfg` & `pretix_sepadebit-2.5.0/setup.cfg`

 * *Files identical despite different names*


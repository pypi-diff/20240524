# Comparing `tmp/pretix-pages-1.6.0.tar.gz` & `tmp/pretix_pages-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-pages-1.6.0.tar", last modified: Tue Sep 26 09:41:52 2023, max compression
+gzip compressed data, was "pretix_pages-1.6.1.tar", last modified: Fri May 24 08:22:40 2024, max compression
```

## Comparing `pretix-pages-1.6.0.tar` & `pretix_pages-1.6.1.tar`

### file list

```diff
@@ -1,139 +1,142 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:52.027129 pretix-pages-1.6.0/
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2486 2023-09-26 09:41:52.027129 pretix-pages-1.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1378 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.819124 pretix-pages-1.6.0/pretix_pages/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.831124 pretix-pages-1.6.0/pretix_pages/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.723121 pretix-pages-1.6.0/pretix_pages/locale/ar/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.831124 pretix-pages-1.6.0/pretix_pages/locale/ar/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4519 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.723121 pretix-pages-1.6.0/pretix_pages/locale/ca/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.831124 pretix-pages-1.6.0/pretix_pages/locale/ca/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4539 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.723121 pretix-pages-1.6.0/pretix_pages/locale/cs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.831124 pretix-pages-1.6.0/pretix_pages/locale/cs/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4379 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.727121 pretix-pages-1.6.0/pretix_pages/locale/da/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.835124 pretix-pages-1.6.0/pretix_pages/locale/da/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5450 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.727121 pretix-pages-1.6.0/pretix_pages/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.835124 pretix-pages-1.6.0/pretix_pages/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5461 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.839124 pretix-pages-1.6.0/pretix_pages/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-26 09:40:50.000000 pretix-pages-1.6.0/pretix_pages/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.839124 pretix-pages-1.6.0/pretix_pages/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5440 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     4157 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/django.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.727121 pretix-pages-1.6.0/pretix_pages/locale/el/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.839124 pretix-pages-1.6.0/pretix_pages/locale/el/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4132 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.727121 pretix-pages-1.6.0/pretix_pages/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.839124 pretix-pages-1.6.0/pretix_pages/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5629 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.727121 pretix-pages-1.6.0/pretix_pages/locale/fi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.839124 pretix-pages-1.6.0/pretix_pages/locale/fi/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4132 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.727121 pretix-pages-1.6.0/pretix_pages/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.839124 pretix-pages-1.6.0/pretix_pages/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4449 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.727121 pretix-pages-1.6.0/pretix_pages/locale/gl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.839124 pretix-pages-1.6.0/pretix_pages/locale/gl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4132 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/gl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.727121 pretix-pages-1.6.0/pretix_pages/locale/hr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.843124 pretix-pages-1.6.0/pretix_pages/locale/hr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4132 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.727121 pretix-pages-1.6.0/pretix_pages/locale/it/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.843124 pretix-pages-1.6.0/pretix_pages/locale/it/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4403 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.731121 pretix-pages-1.6.0/pretix_pages/locale/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.843124 pretix-pages-1.6.0/pretix_pages/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4132 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.731121 pretix-pages-1.6.0/pretix_pages/locale/lv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.843124 pretix-pages-1.6.0/pretix_pages/locale/lv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4557 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.731121 pretix-pages-1.6.0/pretix_pages/locale/nl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.843124 pretix-pages-1.6.0/pretix_pages/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5629 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.731121 pretix-pages-1.6.0/pretix_pages/locale/nl_BE/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.847124 pretix-pages-1.6.0/pretix_pages/locale/nl_BE/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4135 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/nl_BE/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.731121 pretix-pages-1.6.0/pretix_pages/locale/nl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.847124 pretix-pages-1.6.0/pretix_pages/locale/nl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5663 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/nl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.731121 pretix-pages-1.6.0/pretix_pages/locale/pl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.863125 pretix-pages-1.6.0/pretix_pages/locale/pl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4477 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.731121 pretix-pages-1.6.0/pretix_pages/locale/pl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.891125 pretix-pages-1.6.0/pretix_pages/locale/pl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4141 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/pl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.731121 pretix-pages-1.6.0/pretix_pages/locale/pt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.891125 pretix-pages-1.6.0/pretix_pages/locale/pt/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5550 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.731121 pretix-pages-1.6.0/pretix_pages/locale/pt_BR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.891125 pretix-pages-1.6.0/pretix_pages/locale/pt_BR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4691 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.735122 pretix-pages-1.6.0/pretix_pages/locale/pt_PT/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.895125 pretix-pages-1.6.0/pretix_pages/locale/pt_PT/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4437 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/pt_PT/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.735122 pretix-pages-1.6.0/pretix_pages/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.895125 pretix-pages-1.6.0/pretix_pages/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4132 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.735122 pretix-pages-1.6.0/pretix_pages/locale/si/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.895125 pretix-pages-1.6.0/pretix_pages/locale/si/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4339 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/si/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.735122 pretix-pages-1.6.0/pretix_pages/locale/sl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.895125 pretix-pages-1.6.0/pretix_pages/locale/sl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4132 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.735122 pretix-pages-1.6.0/pretix_pages/locale/sv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.895125 pretix-pages-1.6.0/pretix_pages/locale/sv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4297 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.739122 pretix-pages-1.6.0/pretix_pages/locale/tr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.899126 pretix-pages-1.6.0/pretix_pages/locale/tr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5533 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.755122 pretix-pages-1.6.0/pretix_pages/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.899126 pretix-pages-1.6.0/pretix_pages/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4407 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.963127 pretix-pages-1.6.0/pretix_pages/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1054 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1742 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/migrations/0002_auto_20170220_1423.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/migrations/0003_auto_20170504_0706.py
--rw-rw-rw-   0 root         (0) root         (0)      584 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/migrations/0004_auto_20170517_1550.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-26 09:40:50.000000 pretix-pages-1.6.0/pretix_pages/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1561 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/models.py
--rw-rw-rw-   0 root         (0) root         (0)     4833 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.763122 pretix-pages-1.6.0/pretix_pages/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.963127 pretix-pages-1.6.0/pretix_pages/static/pretix_pages/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-26 09:40:50.000000 pretix-pages-1.6.0/pretix_pages/static/pretix_pages/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     2175 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/static/pretix_pages/editor.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.999128 pretix-pages-1.6.0/pretix_pages/static/pretix_pages/quill/
--rw-rw-rw-   0 root         (0) root         (0)    22595 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/static/pretix_pages/quill/quill.bubble.css
--rw-rw-rw-   0 root         (0) root         (0)     8421 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/static/pretix_pages/quill/quill.core.css
--rw-rw-rw-   0 root         (0) root         (0)   284512 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/static/pretix_pages/quill/quill.core.js
--rw-rw-rw-   0 root         (0) root         (0)   414471 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/static/pretix_pages/quill/quill.js
--rw-rw-rw-   0 root         (0) root         (0)    23088 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/static/pretix_pages/quill/quill.snow.css
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/static/pretix_pages/quill-edit.css
--rw-rw-rw-   0 root         (0) root         (0)     6518 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/static/pretix_pages/quill-show.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.763122 pretix-pages-1.6.0/pretix_pages/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:52.019129 pretix-pages-1.6.0/pretix_pages/templates/pretix_pages/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-26 09:40:50.000000 pretix-pages-1.6.0/pretix_pages/templates/pretix_pages/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/templates/pretix_pages/control_head.html
--rw-rw-rw-   0 root         (0) root         (0)      854 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/templates/pretix_pages/delete.html
--rw-rw-rw-   0 root         (0) root         (0)     4487 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/templates/pretix_pages/form.html
--rw-rw-rw-   0 root         (0) root         (0)      367 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/templates/pretix_pages/front_page.html
--rw-rw-rw-   0 root         (0) root         (0)     3105 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/templates/pretix_pages/index.html
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/templates/pretix_pages/presale_head.html
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/templates/pretix_pages/show.html
--rw-rw-rw-   0 root         (0) root         (0)      927 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    10614 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pretix_pages/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 09:41:51.831124 pretix-pages-1.6.0/pretix_pages.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2486 2023-09-26 09:41:51.000000 pretix-pages-1.6.0/pretix_pages.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2868 2023-09-26 09:41:51.000000 pretix-pages-1.6.0/pretix_pages.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-26 09:41:51.000000 pretix-pages-1.6.0/pretix_pages.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      129 2023-09-26 09:41:51.000000 pretix-pages-1.6.0/pretix_pages.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-09-26 09:41:51.000000 pretix-pages-1.6.0/pretix_pages.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      970 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-09-26 09:41:52.031129 pretix-pages-1.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-09-26 09:40:49.000000 pretix-pages-1.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.164875 pretix_pages-1.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2486 2024-05-24 08:22:40.164875 pretix_pages-1.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1378 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.132874 pretix_pages-1.6.1/pretix_pages/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.132874 pretix_pages-1.6.1/pretix_pages/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.120874 pretix_pages-1.6.1/pretix_pages/locale/ar/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.132874 pretix_pages-1.6.1/pretix_pages/locale/ar/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4519 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.120874 pretix_pages-1.6.1/pretix_pages/locale/ca/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.136874 pretix_pages-1.6.1/pretix_pages/locale/ca/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4539 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.120874 pretix_pages-1.6.1/pretix_pages/locale/cs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.136874 pretix_pages-1.6.1/pretix_pages/locale/cs/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4379 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.120874 pretix_pages-1.6.1/pretix_pages/locale/da/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.136874 pretix_pages-1.6.1/pretix_pages/locale/da/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5450 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.124874 pretix_pages-1.6.1/pretix_pages/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.136874 pretix_pages-1.6.1/pretix_pages/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5461 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.136874 pretix_pages-1.6.1/pretix_pages/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.136874 pretix_pages-1.6.1/pretix_pages/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5440 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     4157 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/django.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.124874 pretix_pages-1.6.1/pretix_pages/locale/el/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.136874 pretix_pages-1.6.1/pretix_pages/locale/el/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.124874 pretix_pages-1.6.1/pretix_pages/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.136874 pretix_pages-1.6.1/pretix_pages/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5629 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.124874 pretix_pages-1.6.1/pretix_pages/locale/fi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.140874 pretix_pages-1.6.1/pretix_pages/locale/fi/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.124874 pretix_pages-1.6.1/pretix_pages/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.140874 pretix_pages-1.6.1/pretix_pages/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4483 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.124874 pretix_pages-1.6.1/pretix_pages/locale/gl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.140874 pretix_pages-1.6.1/pretix_pages/locale/gl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/gl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.124874 pretix_pages-1.6.1/pretix_pages/locale/hr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.140874 pretix_pages-1.6.1/pretix_pages/locale/hr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.124874 pretix_pages-1.6.1/pretix_pages/locale/it/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.140874 pretix_pages-1.6.1/pretix_pages/locale/it/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4403 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.124874 pretix_pages-1.6.1/pretix_pages/locale/ja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.140874 pretix_pages-1.6.1/pretix_pages/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.124874 pretix_pages-1.6.1/pretix_pages/locale/lv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.140874 pretix_pages-1.6.1/pretix_pages/locale/lv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4557 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.124874 pretix_pages-1.6.1/pretix_pages/locale/nl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.140874 pretix_pages-1.6.1/pretix_pages/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5629 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.124874 pretix_pages-1.6.1/pretix_pages/locale/nl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.144874 pretix_pages-1.6.1/pretix_pages/locale/nl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5663 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/nl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.124874 pretix_pages-1.6.1/pretix_pages/locale/pl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.144874 pretix_pages-1.6.1/pretix_pages/locale/pl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4477 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.124874 pretix_pages-1.6.1/pretix_pages/locale/pl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.144874 pretix_pages-1.6.1/pretix_pages/locale/pl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4141 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/pl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.124874 pretix_pages-1.6.1/pretix_pages/locale/pt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.144874 pretix_pages-1.6.1/pretix_pages/locale/pt/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5550 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.124874 pretix_pages-1.6.1/pretix_pages/locale/pt_BR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.144874 pretix_pages-1.6.1/pretix_pages/locale/pt_BR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4691 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.124874 pretix_pages-1.6.1/pretix_pages/locale/pt_PT/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.144874 pretix_pages-1.6.1/pretix_pages/locale/pt_PT/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4437 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/pt_PT/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.124874 pretix_pages-1.6.1/pretix_pages/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.144874 pretix_pages-1.6.1/pretix_pages/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.128874 pretix_pages-1.6.1/pretix_pages/locale/si/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.148874 pretix_pages-1.6.1/pretix_pages/locale/si/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4339 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/si/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.128874 pretix_pages-1.6.1/pretix_pages/locale/sk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.148874 pretix_pages-1.6.1/pretix_pages/locale/sk/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.128874 pretix_pages-1.6.1/pretix_pages/locale/sl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.148874 pretix_pages-1.6.1/pretix_pages/locale/sl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.128874 pretix_pages-1.6.1/pretix_pages/locale/sv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.148874 pretix_pages-1.6.1/pretix_pages/locale/sv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4297 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.128874 pretix_pages-1.6.1/pretix_pages/locale/tr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.148874 pretix_pages-1.6.1/pretix_pages/locale/tr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5533 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.128874 pretix_pages-1.6.1/pretix_pages/locale/uk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.148874 pretix_pages-1.6.1/pretix_pages/locale/uk/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     6550 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.128874 pretix_pages-1.6.1/pretix_pages/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.148874 pretix_pages-1.6.1/pretix_pages/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4407 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.152875 pretix_pages-1.6.1/pretix_pages/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1054 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/migrations/0002_auto_20170220_1423.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/migrations/0003_auto_20170504_0706.py
+-rw-rw-rw-   0 root         (0) root         (0)      584 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/migrations/0004_auto_20170517_1550.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4833 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.128874 pretix_pages-1.6.1/pretix_pages/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.152875 pretix_pages-1.6.1/pretix_pages/static/pretix_pages/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/static/pretix_pages/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     2175 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/static/pretix_pages/editor.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.160875 pretix_pages-1.6.1/pretix_pages/static/pretix_pages/quill/
+-rw-rw-rw-   0 root         (0) root         (0)    22595 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/static/pretix_pages/quill/quill.bubble.css
+-rw-rw-rw-   0 root         (0) root         (0)     8421 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/static/pretix_pages/quill/quill.core.css
+-rw-rw-rw-   0 root         (0) root         (0)   284512 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/static/pretix_pages/quill/quill.core.js
+-rw-rw-rw-   0 root         (0) root         (0)   414471 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/static/pretix_pages/quill/quill.js
+-rw-rw-rw-   0 root         (0) root         (0)    23088 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/static/pretix_pages/quill/quill.snow.css
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/static/pretix_pages/quill-edit.css
+-rw-rw-rw-   0 root         (0) root         (0)     6518 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/static/pretix_pages/quill-show.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.128874 pretix_pages-1.6.1/pretix_pages/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.164875 pretix_pages-1.6.1/pretix_pages/templates/pretix_pages/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/templates/pretix_pages/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/templates/pretix_pages/control_head.html
+-rw-rw-rw-   0 root         (0) root         (0)      854 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/templates/pretix_pages/delete.html
+-rw-rw-rw-   0 root         (0) root         (0)     4976 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/templates/pretix_pages/form.html
+-rw-rw-rw-   0 root         (0) root         (0)      367 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/templates/pretix_pages/front_page.html
+-rw-rw-rw-   0 root         (0) root         (0)     3105 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/templates/pretix_pages/index.html
+-rw-rw-rw-   0 root         (0) root         (0)      170 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/templates/pretix_pages/presale_head.html
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/templates/pretix_pages/show.html
+-rw-rw-rw-   0 root         (0) root         (0)      927 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    10614 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pretix_pages/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:22:40.164875 pretix_pages-1.6.1/pretix_pages.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2486 2024-05-24 08:22:40.000000 pretix_pages-1.6.1/pretix_pages.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2910 2024-05-24 08:22:40.000000 pretix_pages-1.6.1/pretix_pages.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 08:22:40.000000 pretix_pages-1.6.1/pretix_pages.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      129 2024-05-24 08:22:40.000000 pretix_pages-1.6.1/pretix_pages.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-24 08:22:40.000000 pretix_pages-1.6.1/pretix_pages.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      970 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      797 2024-05-24 08:22:40.164875 pretix_pages-1.6.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2024-05-24 08:22:18.000000 pretix_pages-1.6.1/setup.py
```

### Comparing `pretix-pages-1.6.0/LICENSE` & `pretix_pages-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/PKG-INFO` & `pretix_pages-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-pages
-Version: 1.6.0
+Version: 1.6.1
 Summary: pretix plugin that allows you to add static pages to your event site, for example for a FAQ, terms of service, etc.
 Author-email: pretix team <support@pretix.eu>
 Maintainer-email: pretix team <support@pretix.eu>
 License: Copyright 2017 Raphael Michel
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
```

### Comparing `pretix-pages-1.6.0/README.rst` & `pretix_pages-1.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/apps.py` & `pretix_pages-1.6.1/pretix_pages/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/ar/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/ca/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/cs/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/da/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/de/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/de_Informal/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/django.pot` & `pretix_pages-1.6.1/pretix_pages/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/el/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/es/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/fi/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/fr/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/fr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2018-12-06 10:11+0100\n"
-"PO-Revision-Date: 2023-01-17 01:00+0000\n"
-"Last-Translator: Maurice Kaag <maurice@kaag.me>\n"
+"PO-Revision-Date: 2023-09-11 18:00+0000\n"
+"Last-Translator: Ronan LE MEILLAT <ronan.le_meillat@highcanfly.club>\n"
 "Language-Team: French <https://translate.pretix.eu/projects/pretix/"
 "pretix-plugin-pages/fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.15\n"
+"X-Generator: Weblate 4.18.2\n"
 
 #: pretix_pages/__init__.py:10 pretix_pages/signals.py:23
 #: pretix_pages/templates/pretix_pages/index.html:6
 #: pretix_pages/templates/pretix_pages/index.html:8
 msgid "Pages"
 msgstr ""
 
@@ -115,15 +115,15 @@
 
 #: pretix_pages/templates/pretix_pages/form.html:25
 msgid "Please enable JavaScript"
 msgstr ""
 
 #: pretix_pages/templates/pretix_pages/form.html:53
 msgid "Save"
-msgstr ""
+msgstr "Sauvegarder"
 
 #: pretix_pages/templates/pretix_pages/form.html:62
 msgid "Page history"
 msgstr ""
 
 #: pretix_pages/templates/pretix_pages/front_page.html:4
 msgid "More information"
```

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/gl/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/gl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/hr/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/it/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/ja/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/lv/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/nl/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/nl_BE/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/ru/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2018-12-06 10:11+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: nl_BE\n"
+"Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_pages/__init__.py:10 pretix_pages/signals.py:23
 #: pretix_pages/templates/pretix_pages/index.html:6
 #: pretix_pages/templates/pretix_pages/index.html:8
```

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/nl_Informal/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/nl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/pl/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/pl_Informal/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/pl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/pt/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/pt_BR/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/pt_PT/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/ru/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/sk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2018-12-06 10:11+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: ru\n"
+"Language: sk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_pages/__init__.py:10 pretix_pages/signals.py:23
 #: pretix_pages/templates/pretix_pages/index.html:6
 #: pretix_pages/templates/pretix_pages/index.html:8
```

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/si/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/si/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/sl/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/sv/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/tr/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/locale/zh_Hans/LC_MESSAGES/django.po` & `pretix_pages-1.6.1/pretix_pages/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/migrations/0001_initial.py` & `pretix_pages-1.6.1/pretix_pages/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/migrations/0002_auto_20170220_1423.py` & `pretix_pages-1.6.1/pretix_pages/migrations/0002_auto_20170220_1423.py`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/migrations/0003_auto_20170504_0706.py` & `pretix_pages-1.6.1/pretix_pages/migrations/0003_auto_20170504_0706.py`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/migrations/0004_auto_20170517_1550.py` & `pretix_pages-1.6.1/pretix_pages/migrations/0004_auto_20170517_1550.py`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/models.py` & `pretix_pages-1.6.1/pretix_pages/models.py`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/signals.py` & `pretix_pages-1.6.1/pretix_pages/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/static/pretix_pages/editor.js` & `pretix_pages-1.6.1/pretix_pages/static/pretix_pages/editor.js`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/static/pretix_pages/quill/quill.bubble.css` & `pretix_pages-1.6.1/pretix_pages/static/pretix_pages/quill/quill.bubble.css`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/static/pretix_pages/quill/quill.core.css` & `pretix_pages-1.6.1/pretix_pages/static/pretix_pages/quill/quill.core.css`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/static/pretix_pages/quill/quill.core.js` & `pretix_pages-1.6.1/pretix_pages/static/pretix_pages/quill/quill.core.js`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/static/pretix_pages/quill/quill.js` & `pretix_pages-1.6.1/pretix_pages/static/pretix_pages/quill/quill.js`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/static/pretix_pages/quill/quill.snow.css` & `pretix_pages-1.6.1/pretix_pages/static/pretix_pages/quill/quill.snow.css`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/static/pretix_pages/quill-show.css` & `pretix_pages-1.6.1/pretix_pages/static/pretix_pages/quill-show.css`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/templates/pretix_pages/delete.html` & `pretix_pages-1.6.1/pretix_pages/templates/pretix_pages/delete.html`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/templates/pretix_pages/form.html` & `pretix_pages-1.6.1/pretix_pages/templates/pretix_pages/form.html`

 * *Files 9% similar despite different names*

```diff
@@ -12,20 +12,26 @@
             <div class="col-xs-12 {% if page %}col-lg-10{% endif %}">
                 <fieldset>
                     <legend>{% trans "General information" %}</legend>
                     {% bootstrap_field form.title layout="horizontal" %}
                     {% bootstrap_field form.slug layout="horizontal" %}
                     {% if page.id %}
                         <div class="form-group">
-                            <label class="col-md-3 control-label">{% trans "Page link" %}</label>
+                            <label class="col-md-3 control-label" for="id_url">{% trans "Page link" %}</label>
                             <div class="col-md-9">
                                 <div class="input-group">
                                     <input class="form-control" readonly="readonly" type="text"
-                                           value="{{ url }}">
+                                           value="{{ url }}" id="id_url">
                                     <div class="input-group-btn">
+                                        <button type="button" class="btn btn-default btn-clipboard" data-clipboard-target="#id_url">
+                                            <i class="fa fa-clipboard" aria-hidden="true"></i>
+                                            <span class="sr-only">
+                                                {% trans "Copy" %}
+                                            </span>
+                                        </button>
                                         <button type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown" title="{% trans "Create QR code" %}" aria-haspopup="true" aria-expanded="false">
                                             <i class="fa fa-qrcode" aria-hidden="true"></i>
                                         </button>
                                         {% include "pretixcontrol/event/fragment_qr_dropdown.html" with url=url %}
                                     </div>
                                 </div>
                             </div>
```

#### html2text {}

```diff
@@ -4,14 +4,15 @@
 ************ {{%% ttrraannss ""PPaaggee"" %%}} ************
 {% csrf_token %} {% bootstrap_form_errors form type='non_fields' %}
 {% trans "General information" %} {% bootstrap_field form.title
 layout="horizontal" %} {% bootstrap_field form.slug layout="horizontal" %} {%
 if page.id %}
 {% trans "Page link" %}
 [{{ url }}           ]
+{% trans "Copy" %}
 }" aria-haspopup="true" aria-expanded="false"> {% include "pretixcontrol/event/
 fragment_qr_dropdown.html" with url=url %}
 {% endif %} {% bootstrap_field form.link_on_frontpage layout="horizontal" %} {%
 bootstrap_field form.link_in_footer layout="horizontal" %} {% bootstrap_field
 form.require_confirmation layout="horizontal" %} {% trans "Page content" %}
 {% trans "Please enable JavaScript" %}
     * {% for lng, text in locales %}
```

### Comparing `pretix-pages-1.6.0/pretix_pages/templates/pretix_pages/index.html` & `pretix_pages-1.6.1/pretix_pages/templates/pretix_pages/index.html`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/urls.py` & `pretix_pages-1.6.1/pretix_pages/urls.py`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages/views.py` & `pretix_pages-1.6.1/pretix_pages/views.py`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/pretix_pages.egg-info/PKG-INFO` & `pretix_pages-1.6.1/pretix_pages.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-pages
-Version: 1.6.0
+Version: 1.6.1
 Summary: pretix plugin that allows you to add static pages to your event site, for example for a FAQ, terms of service, etc.
 Author-email: pretix team <support@pretix.eu>
 Maintainer-email: pretix team <support@pretix.eu>
 License: Copyright 2017 Raphael Michel
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
```

### Comparing `pretix-pages-1.6.0/pretix_pages.egg-info/SOURCES.txt` & `pretix_pages-1.6.1/pretix_pages.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,26 +29,27 @@
 pretix_pages/locale/fr/LC_MESSAGES/django.po
 pretix_pages/locale/gl/LC_MESSAGES/django.po
 pretix_pages/locale/hr/LC_MESSAGES/django.po
 pretix_pages/locale/it/LC_MESSAGES/django.po
 pretix_pages/locale/ja/LC_MESSAGES/django.po
 pretix_pages/locale/lv/LC_MESSAGES/django.po
 pretix_pages/locale/nl/LC_MESSAGES/django.po
-pretix_pages/locale/nl_BE/LC_MESSAGES/django.po
 pretix_pages/locale/nl_Informal/LC_MESSAGES/django.po
 pretix_pages/locale/pl/LC_MESSAGES/django.po
 pretix_pages/locale/pl_Informal/LC_MESSAGES/django.po
 pretix_pages/locale/pt/LC_MESSAGES/django.po
 pretix_pages/locale/pt_BR/LC_MESSAGES/django.po
 pretix_pages/locale/pt_PT/LC_MESSAGES/django.po
 pretix_pages/locale/ru/LC_MESSAGES/django.po
 pretix_pages/locale/si/LC_MESSAGES/django.po
+pretix_pages/locale/sk/LC_MESSAGES/django.po
 pretix_pages/locale/sl/LC_MESSAGES/django.po
 pretix_pages/locale/sv/LC_MESSAGES/django.po
 pretix_pages/locale/tr/LC_MESSAGES/django.po
+pretix_pages/locale/uk/LC_MESSAGES/django.po
 pretix_pages/locale/zh_Hans/LC_MESSAGES/django.po
 pretix_pages/migrations/0001_initial.py
 pretix_pages/migrations/0002_auto_20170220_1423.py
 pretix_pages/migrations/0003_auto_20170504_0706.py
 pretix_pages/migrations/0004_auto_20170517_1550.py
 pretix_pages/migrations/__init__.py
 pretix_pages/static/pretix_pages/.gitkeep
```

### Comparing `pretix-pages-1.6.0/pyproject.toml` & `pretix_pages-1.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.6.0/setup.cfg` & `pretix_pages-1.6.1/setup.cfg`

 * *Files identical despite different names*


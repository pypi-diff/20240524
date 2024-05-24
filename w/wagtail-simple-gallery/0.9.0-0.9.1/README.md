# Comparing `tmp/wagtail-simple-gallery-0.9.0.tar.gz` & `tmp/wagtail-simple-gallery-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wagtail-simple-gallery-0.9.0.tar", last modified: Wed Dec  7 14:49:50 2022, max compression
+gzip compressed data, was "dist\wagtail-simple-gallery-0.9.1.tar", last modified: Sun Dec 18 13:18:02 2022, max compression
```

## Comparing `wagtail-simple-gallery-0.9.0.tar` & `wagtail-simple-gallery-0.9.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2022-12-07 14:49:50.000000 wagtail-simple-gallery-0.9.0/
--rw-rw-rw-   0        0        0     1102 2016-10-06 13:10:20.000000 wagtail-simple-gallery-0.9.0/LICENSE.txt
--rw-rw-rw-   0        0        0      363 2017-03-09 13:12:01.000000 wagtail-simple-gallery-0.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4353 2022-12-07 14:49:50.000000 wagtail-simple-gallery-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     3656 2022-12-07 14:41:45.000000 wagtail-simple-gallery-0.9.0/README.md
--rw-rw-rw-   0        0        0       86 2022-12-07 14:49:50.000000 wagtail-simple-gallery-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1252 2022-12-07 13:54:50.000000 wagtail-simple-gallery-0.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-07 14:49:50.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/
--rw-rw-rw-   0        0        0      102 2022-12-07 14:42:35.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/__init__.py
--rw-rw-rw-   0        0        0      298 2018-04-25 10:34:15.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/apps.py
-drwxrwxrwx   0        0        0        0 2022-12-07 14:49:50.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/locale/
-drwxrwxrwx   0        0        0        0 2022-12-07 14:49:50.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/locale/fr/
-drwxrwxrwx   0        0        0        0 2022-12-07 14:49:50.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1478 2017-03-09 13:12:01.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     1945 2017-03-09 13:12:01.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/locale/fr/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2022-12-07 14:49:50.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/migrations/
--rw-rw-rw-   0        0        0     1583 2018-04-25 10:34:15.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     2014 2018-04-25 10:34:15.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/migrations/0002_auto_20170309_1046.py
--rw-rw-rw-   0        0        0      561 2017-11-19 13:07:24.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/migrations/0003_simplegalleryindex_order_images_by.py
--rw-rw-rw-   0        0        0      417 2022-12-07 14:04:44.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/migrations/0004_alter_simplegalleryindex_options.py
--rw-rw-rw-   0        0        0        0 2016-10-05 14:32:54.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/migrations/__init__.py
--rw-rw-rw-   0        0        0     5237 2022-07-26 09:27:10.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/models.py
-drwxrwxrwx   0        0        0        0 2022-12-07 14:49:50.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/static/
-drwxrwxrwx   0        0        0        0 2022-12-07 14:49:50.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/static/css/
--rw-rw-rw-   0        0        0     3571 2016-07-23 12:05:50.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/static/css/baguetteBox.min.css
--rw-rw-rw-   0        0        0      657 2016-10-13 10:16:23.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/static/css/simple-gallery-admin.css
--rw-rw-rw-   0        0        0     1030 2019-05-25 05:55:00.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/static/css/simple-gallery.css
-drwxrwxrwx   0        0        0        0 2022-12-07 14:49:50.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/static/js/
--rw-rw-rw-   0        0        0     8721 2016-07-23 12:05:50.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/static/js/baguetteBox.min.js
-drwxrwxrwx   0        0        0        0 2022-12-07 14:49:50.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/templates/
--rw-rw-rw-   0        0        0      743 2016-10-12 08:45:23.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/templates/simple_gallery_base.html
-drwxrwxrwx   0        0        0        0 2022-12-07 14:49:50.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/templates/wagtail_simple_gallery/
--rw-rw-rw-   0        0        0      823 2019-05-25 05:55:00.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/templates/wagtail_simple_gallery/simple_gallery.html
--rw-rw-rw-   0        0        0     2515 2019-05-25 05:55:00.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/templates/wagtail_simple_gallery/simple_gallery_index.html
-drwxrwxrwx   0        0        0        0 2022-12-07 14:49:50.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/templatetags/
--rw-rw-rw-   0        0        0        0 2016-10-06 07:54:34.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/templatetags/__init__.py
--rw-rw-rw-   0        0        0     1035 2018-04-25 10:41:11.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/templatetags/wagtailsimplegallery_tags.py
--rw-rw-rw-   0        0        0       60 2016-10-05 14:32:54.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/tests.py
--rw-rw-rw-   0        0        0      298 2020-03-30 16:18:17.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/wagtail_hooks.py
-drwxrwxrwx   0        0        0        0 2022-12-07 14:49:50.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery.egg-info/
--rw-rw-rw-   0        0        0     4353 2022-12-07 14:49:50.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1418 2022-12-07 14:49:50.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-07 14:49:50.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2022-12-07 14:49:50.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2022-12-07 14:49:50.000000 wagtail-simple-gallery-0.9.0/wagtail_simple_gallery.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-12-18 13:18:02.000000 wagtail-simple-gallery-0.9.1/
+-rw-rw-rw-   0        0        0     1102 2016-10-06 13:10:20.000000 wagtail-simple-gallery-0.9.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      363 2017-03-09 13:12:01.000000 wagtail-simple-gallery-0.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4353 2022-12-18 13:18:02.000000 wagtail-simple-gallery-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3656 2022-12-07 14:41:45.000000 wagtail-simple-gallery-0.9.1/README.md
+-rw-rw-rw-   0        0        0       86 2022-12-18 13:18:02.000000 wagtail-simple-gallery-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1252 2022-12-07 13:54:50.000000 wagtail-simple-gallery-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-18 13:18:02.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/
+-rw-rw-rw-   0        0        0      102 2022-12-18 13:17:10.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/__init__.py
+-rw-rw-rw-   0        0        0      298 2018-04-25 10:34:15.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/apps.py
+drwxrwxrwx   0        0        0        0 2022-12-18 13:18:02.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/locale/
+drwxrwxrwx   0        0        0        0 2022-12-18 13:18:02.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/locale/fr/
+drwxrwxrwx   0        0        0        0 2022-12-18 13:18:02.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1478 2017-03-09 13:12:01.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     1945 2017-03-09 13:12:01.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/locale/fr/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2022-12-18 13:18:02.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/migrations/
+-rw-rw-rw-   0        0        0     1583 2018-04-25 10:34:15.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     2014 2018-04-25 10:34:15.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/migrations/0002_auto_20170309_1046.py
+-rw-rw-rw-   0        0        0      561 2017-11-19 13:07:24.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/migrations/0003_simplegalleryindex_order_images_by.py
+-rw-rw-rw-   0        0        0      417 2022-12-07 14:04:44.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/migrations/0004_alter_simplegalleryindex_options.py
+-rw-rw-rw-   0        0        0        0 2016-10-05 14:32:54.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/migrations/__init__.py
+-rw-rw-rw-   0        0        0     5236 2022-12-18 13:16:17.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/models.py
+drwxrwxrwx   0        0        0        0 2022-12-18 13:18:02.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/static/
+drwxrwxrwx   0        0        0        0 2022-12-18 13:18:02.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/static/css/
+-rw-rw-rw-   0        0        0     3571 2016-07-23 12:05:50.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/static/css/baguetteBox.min.css
+-rw-rw-rw-   0        0        0      657 2016-10-13 10:16:23.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/static/css/simple-gallery-admin.css
+-rw-rw-rw-   0        0        0     1030 2019-05-25 05:55:00.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/static/css/simple-gallery.css
+drwxrwxrwx   0        0        0        0 2022-12-18 13:18:02.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/static/js/
+-rw-rw-rw-   0        0        0     8721 2016-07-23 12:05:50.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/static/js/baguetteBox.min.js
+drwxrwxrwx   0        0        0        0 2022-12-18 13:18:02.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/templates/
+-rw-rw-rw-   0        0        0      743 2016-10-12 08:45:23.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/templates/simple_gallery_base.html
+drwxrwxrwx   0        0        0        0 2022-12-18 13:18:02.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/templates/wagtail_simple_gallery/
+-rw-rw-rw-   0        0        0      823 2019-05-25 05:55:00.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/templates/wagtail_simple_gallery/simple_gallery.html
+-rw-rw-rw-   0        0        0     2515 2019-05-25 05:55:00.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/templates/wagtail_simple_gallery/simple_gallery_index.html
+drwxrwxrwx   0        0        0        0 2022-12-18 13:18:02.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/templatetags/
+-rw-rw-rw-   0        0        0        0 2016-10-06 07:54:34.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     1035 2018-04-25 10:41:11.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/templatetags/wagtailsimplegallery_tags.py
+-rw-rw-rw-   0        0        0       60 2016-10-05 14:32:54.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/tests.py
+-rw-rw-rw-   0        0        0      298 2020-03-30 16:18:17.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/wagtail_hooks.py
+drwxrwxrwx   0        0        0        0 2022-12-18 13:18:02.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery.egg-info/
+-rw-rw-rw-   0        0        0     4353 2022-12-18 13:18:02.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1418 2022-12-18 13:18:02.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-18 13:18:02.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2022-12-18 13:18:02.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2022-12-18 13:18:02.000000 wagtail-simple-gallery-0.9.1/wagtail_simple_gallery.egg-info/top_level.txt
```

### Comparing `wagtail-simple-gallery-0.9.0/LICENSE.txt` & `wagtail-simple-gallery-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtail-simple-gallery-0.9.0/PKG-INFO` & `wagtail-simple-gallery-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-simple-gallery
-Version: 0.9.0
+Version: 0.9.1
 Summary: A simple gallery app for Wagtail.
 Home-page: https://github.com/temeez/wagtail-simple-gallery
 Author: Teemu Nieminen
 Author-email: temeez.dev@gmail.com
 License: MIT License
 Keywords: wagtail cms model page templatetags
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-simple-gallery-0.9.0/README.md` & `wagtail-simple-gallery-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-simple-gallery-0.9.0/setup.py` & `wagtail-simple-gallery-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/locale/fr/LC_MESSAGES/django.mo` & `wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/locale/fr/LC_MESSAGES/django.po` & `wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/migrations/0001_initial.py` & `wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/migrations/0002_auto_20170309_1046.py` & `wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/migrations/0002_auto_20170309_1046.py`

 * *Files identical despite different names*

### Comparing `wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/migrations/0003_simplegalleryindex_order_images_by.py` & `wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/migrations/0003_simplegalleryindex_order_images_by.py`

 * *Files identical despite different names*

### Comparing `wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/models.py` & `wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.conf import settings
 from django.core.paginator import Paginator, EmptyPage, PageNotAnInteger
 from django.db import models
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from wagtail.admin.edit_handlers import FieldPanel
 from wagtail.core.fields import RichTextField
 from wagtail.core.models import Page
 from wagtail.images import get_image_model
 
 from django.shortcuts import render, redirect
```

### Comparing `wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/static/css/baguetteBox.min.css` & `wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/static/css/baguetteBox.min.css`

 * *Files identical despite different names*

### Comparing `wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/static/css/simple-gallery-admin.css` & `wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/static/css/simple-gallery-admin.css`

 * *Files identical despite different names*

### Comparing `wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/static/css/simple-gallery.css` & `wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/static/css/simple-gallery.css`

 * *Files identical despite different names*

### Comparing `wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/static/js/baguetteBox.min.js` & `wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/static/js/baguetteBox.min.js`

 * *Files identical despite different names*

### Comparing `wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/templates/simple_gallery_base.html` & `wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/templates/simple_gallery_base.html`

 * *Files identical despite different names*

### Comparing `wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/templates/wagtail_simple_gallery/simple_gallery.html` & `wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/templates/wagtail_simple_gallery/simple_gallery.html`

 * *Files identical despite different names*

### Comparing `wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/templates/wagtail_simple_gallery/simple_gallery_index.html` & `wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/templates/wagtail_simple_gallery/simple_gallery_index.html`

 * *Files identical despite different names*

### Comparing `wagtail-simple-gallery-0.9.0/wagtail_simple_gallery/templatetags/wagtailsimplegallery_tags.py` & `wagtail-simple-gallery-0.9.1/wagtail_simple_gallery/templatetags/wagtailsimplegallery_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-simple-gallery-0.9.0/wagtail_simple_gallery.egg-info/PKG-INFO` & `wagtail-simple-gallery-0.9.1/wagtail_simple_gallery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-simple-gallery
-Version: 0.9.0
+Version: 0.9.1
 Summary: A simple gallery app for Wagtail.
 Home-page: https://github.com/temeez/wagtail-simple-gallery
 Author: Teemu Nieminen
 Author-email: temeez.dev@gmail.com
 License: MIT License
 Keywords: wagtail cms model page templatetags
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-simple-gallery-0.9.0/wagtail_simple_gallery.egg-info/SOURCES.txt` & `wagtail-simple-gallery-0.9.1/wagtail_simple_gallery.egg-info/SOURCES.txt`

 * *Files identical despite different names*


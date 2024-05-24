# Comparing `tmp/wagtailvideos-6.0.0.tar.gz` & `tmp/wagtailvideos-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailvideos-6.0.0.tar", last modified: Fri May 10 05:29:03 2024, max compression
+gzip compressed data, was "wagtailvideos-6.1.0.tar", last modified: Fri May 24 06:25:18 2024, max compression
```

## Comparing `wagtailvideos-6.0.0.tar` & `wagtailvideos-6.1.0.tar`

### file list

```diff
@@ -1,109 +1,119 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.571055 wagtailvideos-6.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1481 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      161 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6054 2024-05-10 05:29:03.571055 wagtailvideos-6.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5023 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      295 2024-05-10 05:29:03.571055 wagtailvideos-6.0.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1373 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.556055 wagtailvideos-6.0.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.557055 wagtailvideos-6.0.0/tests/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.558055 wagtailvideos-6.0.0/tests/app/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    32030 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/app/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/app/migrations/0002_alter_testpage_video_streamfield.py
--rw-rw-rw-   0 root         (0) root         (0)    27639 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/app/migrations/0003_alter_customvideotrack_file_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/app/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1668 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/app/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2210 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/app/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1341 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/app/test_block.py
--rw-rw-rw-   0 root         (0) root         (0)      560 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/app/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     6455 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/storage.py
--rw-rw-rw-   0 root         (0) root         (0)    25986 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/test_admin_views.py
--rw-rw-rw-   0 root         (0) root         (0)     1352 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/test_custom_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1628 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/test_template_tag.py
--rw-rw-rw-   0 root         (0) root         (0)      358 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.560055 wagtailvideos-6.0.0/wagtailvideos/
--rw-rw-rw-   0 root         (0) root         (0)      838 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      911 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/blocks.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/edit_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)     2136 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/ffmpeg.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/fields.py
--rw-rw-rw-   0 root         (0) root         (0)     3206 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/forms.py
--rw-rw-rw-   0 root         (0) root         (0)      637 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/jinja2tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.551055 wagtailvideos-6.0.0/wagtailvideos/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.552055 wagtailvideos-6.0.0/wagtailvideos/locale/ru_RU/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.562055 wagtailvideos-6.0.0/wagtailvideos/locale/ru_RU/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     9219 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    13787 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.565055 wagtailvideos-6.0.0/wagtailvideos/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1966 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      757 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0002_auto_20160321_1610.py
--rw-rw-rw-   0 root         (0) root         (0)     1273 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0003_auto_20160705_1646.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0004_auto_20160706_1153.py
--rw-rw-rw-   0 root         (0) root         (0)      499 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0005_videotranscode_error_message.py
--rw-rw-rw-   0 root         (0) root         (0)      585 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0006_auto_20160707_1413.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0007_video_duration.py
--rw-rw-rw-   0 root         (0) root         (0)      465 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0008_auto_20160728_1523.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0009_videotranscode_quality.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0010_video_ordering.py
--rw-rw-rw-   0 root         (0) root         (0)    28229 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0011_video_tracks.py
--rw-rw-rw-   0 root         (0) root         (0)    26753 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0012_remove_unique_constraint.py
--rw-rw-rw-   0 root         (0) root         (0)     3473 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0013_add_choose_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)    44986 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0014_alter_videotrack_file_alter_videotrack_kind_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13904 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/models.py
--rw-rw-rw-   0 root         (0) root         (0)      322 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     2642 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.552055 wagtailvideos-6.0.0/wagtailvideos/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.552055 wagtailvideos-6.0.0/wagtailvideos/static/wagtailvideos/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.565055 wagtailvideos-6.0.0/wagtailvideos/static/wagtailvideos/css/
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/static/wagtailvideos/css/edit-video.css
--rw-rw-rw-   0 root         (0) root         (0)      364 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/static/wagtailvideos/css/summary-override.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.566055 wagtailvideos-6.0.0/wagtailvideos/static/wagtailvideos/js/
--rw-rw-rw-   0 root         (0) root         (0)     5536 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/static/wagtailvideos/js/add-multiple.js
--rw-rw-rw-   0 root         (0) root         (0)      316 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/static/wagtailvideos/js/video-chooser-telepath.js
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/static/wagtailvideos/js/video-chooser.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.552055 wagtailvideos-6.0.0/wagtailvideos/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.553055 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.566055 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/chooser/
--rw-rw-rw-   0 root         (0) root         (0)      929 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/chooser/chooser.html
--rw-rw-rw-   0 root         (0) root         (0)     1988 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/chooser/results.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.567055 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/homepage/
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/homepage/videos_summary.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.567055 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/multiple/
--rw-rw-rw-   0 root         (0) root         (0)     4414 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/multiple/add.html
--rw-rw-rw-   0 root         (0) root         (0)     1045 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/multiple/edit_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.553055 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/permissions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.567055 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/permissions/includes/
--rw-rw-rw-   0 root         (0) root         (0)      253 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/permissions/includes/video_permissions_formset.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.569055 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/
--rw-rw-rw-   0 root         (0) root         (0)      246 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/_file_field.html
--rw-rw-rw-   0 root         (0) root         (0)      232 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/_file_field_as_li.html
--rw-rw-rw-   0 root         (0) root         (0)     1225 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/add.html
--rw-rw-rw-   0 root         (0) root         (0)      820 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/confirm_delete.html
--rw-rw-rw-   0 root         (0) root         (0)     6815 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/edit.html
--rw-rw-rw-   0 root         (0) root         (0)     1393 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/index.html
--rw-rw-rw-   0 root         (0) root         (0)     2019 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/results.html
--rw-rw-rw-   0 root         (0) root         (0)     1903 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/usage.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.569055 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/widgets/
--rw-rw-rw-   0 root         (0) root         (0)      442 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/widgets/video_chooser.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.569055 wagtailvideos-6.0.0/wagtailvideos/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templatetags/wagtailvideos_tags.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.570055 wagtailvideos-6.0.0/wagtailvideos/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5285 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/views/chooser.py
--rw-rw-rw-   0 root         (0) root         (0)     4730 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/views/multiple.py
--rw-rw-rw-   0 root         (0) root         (0)     7685 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/views/videos.py
--rw-rw-rw-   0 root         (0) root         (0)     4295 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/wagtail_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     2085 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/widgets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.570055 wagtailvideos-6.0.0/wagtailvideos.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6054 2024-05-10 05:29:03.000000 wagtailvideos-6.0.0/wagtailvideos.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3389 2024-05-10 05:29:03.000000 wagtailvideos-6.0.0/wagtailvideos.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 05:29:03.000000 wagtailvideos-6.0.0/wagtailvideos.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 05:29:03.000000 wagtailvideos-6.0.0/wagtailvideos.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       94 2024-05-10 05:29:03.000000 wagtailvideos-6.0.0/wagtailvideos.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-10 05:29:03.000000 wagtailvideos-6.0.0/wagtailvideos.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.258856 wagtailvideos-6.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1481 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      161 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6037 2024-05-24 06:25:18.258856 wagtailvideos-6.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5051 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      295 2024-05-24 06:25:18.259856 wagtailvideos-6.1.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1332 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.240854 wagtailvideos-6.1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.241854 wagtailvideos-6.1.0/tests/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.242854 wagtailvideos-6.1.0/tests/app/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    32355 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/app/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/app/migrations/0002_alter_testpage_video_streamfield.py
+-rw-rw-rw-   0 root         (0) root         (0)    27639 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/app/migrations/0003_alter_customvideotrack_file_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/app/migrations/0004_customvideomodel_height_customvideomodel_width.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/app/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1668 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/app/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2210 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/app/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/app/test_block.py
+-rw-rw-rw-   0 root         (0) root         (0)      560 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/app/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     6455 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)    26157 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/test_admin_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/test_custom_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1628 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/test_template_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)      358 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.245854 wagtailvideos-6.1.0/wagtailvideos/
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/blocks.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/edit_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1351 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     2067 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     3193 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/jinja2tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.235853 wagtailvideos-6.1.0/wagtailvideos/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.235853 wagtailvideos-6.1.0/wagtailvideos/locale/ru_RU/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.247855 wagtailvideos-6.1.0/wagtailvideos/locale/ru_RU/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     9219 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    13787 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.250855 wagtailvideos-6.1.0/wagtailvideos/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      757 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0002_auto_20160321_1610.py
+-rw-rw-rw-   0 root         (0) root         (0)     1445 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0003_auto_20160705_1646.py
+-rw-rw-rw-   0 root         (0) root         (0)      599 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0004_auto_20160706_1153.py
+-rw-rw-rw-   0 root         (0) root         (0)      499 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0005_videotranscode_error_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      585 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0006_auto_20160707_1413.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0007_video_duration.py
+-rw-rw-rw-   0 root         (0) root         (0)      465 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0008_auto_20160728_1523.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0009_videotranscode_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0010_video_ordering.py
+-rw-rw-rw-   0 root         (0) root         (0)    28229 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0011_video_tracks.py
+-rw-rw-rw-   0 root         (0) root         (0)    26753 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0012_remove_unique_constraint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3473 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0013_add_choose_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)    44986 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0014_alter_videotrack_file_alter_videotrack_kind_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      648 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0015_video_height_video_width.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10304 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      322 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2266 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.236853 wagtailvideos-6.1.0/wagtailvideos/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.236853 wagtailvideos-6.1.0/wagtailvideos/static/wagtailvideos/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.251855 wagtailvideos-6.1.0/wagtailvideos/static/wagtailvideos/css/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/static/wagtailvideos/css/edit-video.css
+-rw-rw-rw-   0 root         (0) root         (0)      364 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/static/wagtailvideos/css/summary-override.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.252855 wagtailvideos-6.1.0/wagtailvideos/static/wagtailvideos/js/
+-rw-rw-rw-   0 root         (0) root         (0)     5536 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/static/wagtailvideos/js/add-multiple.js
+-rw-rw-rw-   0 root         (0) root         (0)      316 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/static/wagtailvideos/js/video-chooser-telepath.js
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/static/wagtailvideos/js/video-chooser.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.236853 wagtailvideos-6.1.0/wagtailvideos/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.237853 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.252855 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/chooser/
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/chooser/chooser.html
+-rw-rw-rw-   0 root         (0) root         (0)     1988 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/chooser/results.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.252855 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/homepage/
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/homepage/videos_summary.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.253856 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/multiple/
+-rw-rw-rw-   0 root         (0) root         (0)     4414 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/multiple/add.html
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/multiple/edit_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.237853 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/permissions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.253856 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/permissions/includes/
+-rw-rw-rw-   0 root         (0) root         (0)      253 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/permissions/includes/video_permissions_formset.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.255856 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/
+-rw-rw-rw-   0 root         (0) root         (0)      246 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/_file_field.html
+-rw-rw-rw-   0 root         (0) root         (0)      232 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/_file_field_as_li.html
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/add.html
+-rw-rw-rw-   0 root         (0) root         (0)      820 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/confirm_delete.html
+-rw-rw-rw-   0 root         (0) root         (0)     7272 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/edit.html
+-rw-rw-rw-   0 root         (0) root         (0)     1393 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/index.html
+-rw-rw-rw-   0 root         (0) root         (0)     2019 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/results.html
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/usage.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.255856 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)      442 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/widgets/video_chooser.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.255856 wagtailvideos-6.1.0/wagtailvideos/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templatetags/wagtailvideos_tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.256856 wagtailvideos-6.1.0/wagtailvideos/transcoders/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/transcoders/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.256856 wagtailvideos-6.1.0/wagtailvideos/transcoders/base/
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/transcoders/base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.256856 wagtailvideos-6.1.0/wagtailvideos/transcoders/ffmpeg/
+-rw-rw-rw-   0 root         (0) root         (0)     1901 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/transcoders/ffmpeg/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      517 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/transcoders/ffmpeg/checks.py
+-rw-rw-rw-   0 root         (0) root         (0)     6982 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/transcoders/ffmpeg/ffmpeg.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.257856 wagtailvideos-6.1.0/wagtailvideos/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5285 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/views/chooser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4730 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/views/multiple.py
+-rw-rw-rw-   0 root         (0) root         (0)     7760 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/views/videos.py
+-rw-rw-rw-   0 root         (0) root         (0)     4295 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/wagtail_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2085 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/widgets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.258856 wagtailvideos-6.1.0/wagtailvideos.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6037 2024-05-24 06:25:18.000000 wagtailvideos-6.1.0/wagtailvideos.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3734 2024-05-24 06:25:18.000000 wagtailvideos-6.1.0/wagtailvideos.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 06:25:18.000000 wagtailvideos-6.1.0/wagtailvideos.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 06:25:18.000000 wagtailvideos-6.1.0/wagtailvideos.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-24 06:25:18.000000 wagtailvideos-6.1.0/wagtailvideos.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-24 06:25:18.000000 wagtailvideos-6.1.0/wagtailvideos.egg-info/top_level.txt
```

### Comparing `wagtailvideos-6.0.0/LICENSE` & `wagtailvideos-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/PKG-INFO` & `wagtailvideos-6.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailvideos
-Version: 6.0.0
+Version: 6.1.0
 Summary: A wagtail module for uploading and displaying videos in various codecs.
 Home-page: https://github.com/neon-jungle/wagtailvideos
 Author: Neon Jungle
 Author-email: developers@neonjungle.studio
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: BSD License
 License-File: LICENSE
 Requires-Dist: wagtail>=5.2
 Requires-Dist: Django>=3.2
-Requires-Dist: django-enumchoicefield>=1.1.0
 Requires-Dist: bcp47==0.0.4
 Requires-Dist: wagtail-modeladmin>=2.0.0
 
 wagtailvideos
 =============
 
 .. image:: https://gitlab.com/neonjungle/wagtailvideos/badges/master/pipeline.svg
@@ -35,16 +34,16 @@
 Based on wagtailimages. The aim was to have feature parity with images
 but for html5 videos. Includes the ability to transcode videos to a
 html5 compliant codec using ffmpeg.
 
 Requirements
 ------------
 
--  Wagtail >= 4.0 (for older wagtail version see the tags)
--  `ffmpeg <https://ffmpeg.org/>`__
+-  Wagtail >= 5.2 (for older wagtail version see the tags)
+-  `ffmpeg <https://ffmpeg.org/>`__ (optional, for transcoding)
 
 Installing
 ----------
 
 Install using pypi
 
 .. code:: bash
```

### Comparing `wagtailvideos-6.0.0/README.rst` & `wagtailvideos-6.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 Based on wagtailimages. The aim was to have feature parity with images
 but for html5 videos. Includes the ability to transcode videos to a
 html5 compliant codec using ffmpeg.
 
 Requirements
 ------------
 
--  Wagtail >= 4.0 (for older wagtail version see the tags)
--  `ffmpeg <https://ffmpeg.org/>`__
+-  Wagtail >= 5.2 (for older wagtail version see the tags)
+-  `ffmpeg <https://ffmpeg.org/>`__ (optional, for transcoding)
 
 Installing
 ----------
 
 Install using pypi
 
 .. code:: bash
```

### Comparing `wagtailvideos-6.0.0/setup.py` & `wagtailvideos-6.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,23 @@
 with open("README.rst", "r") as f:
     readme = f.read()
 
 from setuptools import find_packages, setup  # noqa: E4
 
 setup(
     name="wagtailvideos",
-    version="6.0.0",
+    version="6.1.0",
     description="A wagtail module for uploading and displaying videos in various codecs.",
     long_description=readme,
     author="Neon Jungle",
     author_email="developers@neonjungle.studio",
     url="https://github.com/neon-jungle/wagtailvideos",
     install_requires=[
         "wagtail>=5.2",
         "Django>=3.2",
-        "django-enumchoicefield>=1.1.0",
         "bcp47==0.0.4",
         "wagtail-modeladmin>=2.0.0"
     ],
     zip_safe=False,
     license="BSD License",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `wagtailvideos-6.0.0/tests/app/migrations/0001_initial.py` & `wagtailvideos-6.1.0/tests/app/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Generated by Django 2.2.17 on 2021-02-09 04:45
 
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
-import enumchoicefield.fields
 import modelcluster.fields
 import taggit.managers
 import wagtail.fields
 import wagtail.models
 import wagtail.search.index
 import wagtailvideos.blocks
 import wagtailvideos.models
@@ -85,16 +84,31 @@
             name='video',
             field=models.OneToOneField(on_delete=django.db.models.deletion.CASCADE, related_name='track_listing', to='app.CustomVideoModel'),
         ),
         migrations.CreateModel(
             name='CustomVideoTranscode',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('media_format', enumchoicefield.fields.EnumChoiceField(enum_class=wagtailvideos.models.MediaFormats, max_length=4)),
-                ('quality', enumchoicefield.fields.EnumChoiceField(default=wagtailvideos.models.VideoQuality(1), enum_class=wagtailvideos.models.VideoQuality, max_length=7)),
+                ('media_format', models.CharField(
+                    choices=[
+                        ("webm", "VP8 and Vorbis in WebM"),
+                        ("mp4", "H.264 and AAC in Mp4"),
+                        ("ogg", "Theora and Vorbis in Ogg"),
+                    ],
+                    max_length=4,
+                )),
+                ('quality', models.CharField(
+                    choices=[
+                        ("default", "Default"),
+                        ("lowest", "Low"),
+                        ("highest", "High"),
+                    ],
+                    default="default",
+                    max_length=7,
+                )),
                 ('processing', models.BooleanField(default=False)),
                 ('file', models.FileField(blank=True, null=True, upload_to=wagtailvideos.models.get_upload_to, verbose_name='file')),
                 ('error_message', models.TextField(blank=True)),
                 ('video', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='transcodes', to='app.CustomVideoModel')),
             ],
             options={
                 'unique_together': {('video', 'media_format')},
```

### Comparing `wagtailvideos-6.0.0/tests/app/migrations/0003_alter_customvideotrack_file_and_more.py` & `wagtailvideos-6.1.0/tests/app/migrations/0003_alter_customvideotrack_file_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/tests/app/models.py` & `wagtailvideos-6.1.0/tests/app/models.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/tests/app/settings.py` & `wagtailvideos-6.1.0/tests/app/settings.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/tests/app/test_block.py` & `wagtailvideos-6.1.0/tests/app/test_block.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/tests/app/urls.py` & `wagtailvideos-6.1.0/tests/app/urls.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/tests/storage.py` & `wagtailvideos-6.1.0/tests/storage.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/tests/test_admin_views.py` & `wagtailvideos-6.1.0/tests/test_admin_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,20 +103,22 @@
         self.assertEqual(videos.count(), 1)
 
         # Test that extra fields were populated from post_save signal
         video = videos.first()
         self.assertTrue(video.thumbnail)
         self.assertTrue(video.duration)
         self.assertTrue(video.file_size)
+        self.assertTrue(video.width)
+        self.assertTrue(video.height)
 
         # Test that it was placed in the root collection
         root_collection = Collection.get_first_root_node()
         self.assertEqual(video.collection, root_collection)
 
-    @patch("wagtailvideos.ffmpeg.installed")
+    @patch("wagtailvideos.transcoders.ffmpeg.ffmpeg.installed")
     def test_add_no_ffmpeg(self, ffmpeg_installed):
         ffmpeg_installed.return_value = False
 
         video_file = create_test_video_file()
         title = "no_ffmpeg"
 
         response = self.post(
@@ -132,14 +134,16 @@
         # Check video exists but has no thumb or duration
         videos = Video.objects.filter(title=title)
         self.assertEqual(videos.count(), 1)
         video = videos.first()
 
         self.assertFalse(video.thumbnail)
         self.assertFalse(video.duration)
+        self.assertFalse(video.width)
+        self.assertFalse(video.height)
 
     def test_add_no_file_selected(self):
         response = self.post(
             {
                 "title": "nothing here",
             }
         )
```

### Comparing `wagtailvideos-6.0.0/tests/test_custom_model.py` & `wagtailvideos-6.1.0/tests/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/tests/test_template_tag.py` & `wagtailvideos-6.1.0/tests/test_template_tag.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/blocks.py` & `wagtailvideos-6.1.0/wagtailvideos/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/fields.py` & `wagtailvideos-6.1.0/wagtailvideos/fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from django.forms.fields import FileField
 from django.template.defaultfilters import filesizeformat
 from django.utils.translation import gettext_lazy as _
 
 
 class WagtailVideoField(FileField):
     def __init__(self, *args, **kwargs):
-        super(WagtailVideoField, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
         # Get max upload size from settings
         self.max_upload_size = getattr(settings, 'WAGTAILVIDEOS_MAX_UPLOAD_SIZE', 1024 * 1024 * 1024)
         max_upload_size_text = filesizeformat(self.max_upload_size)
 
         # Help text
         if self.max_upload_size is not None:
@@ -46,14 +46,14 @@
         # Check the filesize
         if f.size > self.max_upload_size:
             raise ValidationError(self.error_messages['file_too_large'] % (
                 filesizeformat(f.size),
             ), code='file_too_large')
 
     def to_python(self, data):
-        f = super(WagtailVideoField, self).to_python(data)
+        f = super().to_python(data)
 
         if f is not None:
             self.check_video_file_size(f)
             self.check_video_file_format(f)
 
         return f
```

### Comparing `wagtailvideos-6.0.0/wagtailvideos/forms.py` & `wagtailvideos-6.1.0/wagtailvideos/forms.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from django import forms
 from django.forms.models import modelform_factory
 from django.utils.translation import gettext as _
-from enumchoicefield.forms import EnumField
 from wagtail.admin import widgets
 from wagtail.admin.forms.collections import (
     BaseCollectionMemberForm, collection_member_permission_formset_factory)
 
+from wagtailvideos.enums import MediaFormats, VideoQuality
 from wagtailvideos.fields import WagtailVideoField
-from wagtailvideos.models import MediaFormats, Video, VideoQuality
+from wagtailvideos.models import Video
 from wagtailvideos.permissions import \
     permission_policy as video_permission_policy
 
 
 class BaseVideoForm(BaseCollectionMemberForm):
     permission_policy = video_permission_policy
 
     def __init__(self, *args, **kwargs):
-        super(BaseVideoForm, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         # A file is only required if there is not already a file, such as when
         # editing an existing video.  The file field is not used on the
         # multiple-upload forms, so may not be present
         if 'file' in self.fields:
             self.fields['file'].required = 'file' not in self.initial or not self.initial['file']
 
 
@@ -55,19 +55,19 @@
             'tags': widgets.AdminTagWidget,
             'file': forms.FileInput(),
             'thumbnail': forms.FileInput(),
         })
 
 
 class VideoTranscodeAdminForm(forms.Form):
-    media_format = EnumField(MediaFormats)
-    quality = EnumField(VideoQuality)
+    media_format = forms.ChoiceField(choices=MediaFormats.choices)
+    quality = forms.ChoiceField(choices=VideoQuality.choices)
 
     def __init__(self, video, data=None, **kwargs):
-        super(VideoTranscodeAdminForm, self).__init__(data=data, **kwargs)
+        super().__init__(data=data, **kwargs)
         self.video = video
 
     def save(self):
         media_format = self.cleaned_data['media_format']
         quality = self.cleaned_data['quality']
         self.video.do_transcode(media_format, quality)
```

### Comparing `wagtailvideos-6.0.0/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.mo` & `wagtailvideos-6.1.0/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.po` & `wagtailvideos-6.1.0/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/migrations/0001_initial.py` & `wagtailvideos-6.1.0/wagtailvideos/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/migrations/0002_auto_20160321_1610.py` & `wagtailvideos-6.1.0/wagtailvideos/migrations/0002_auto_20160321_1610.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/migrations/0003_auto_20160705_1646.py` & `wagtailvideos-6.1.0/wagtailvideos/migrations/0003_auto_20160705_1646.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*- coding: utf-8 -*-
 # Generated by Django 1.9.7 on 2016-07-05 06:46
 from __future__ import absolute_import, print_function, unicode_literals
 
 import django.db.models.deletion
-import enumchoicefield.fields
 from django.db import migrations, models
 
 import wagtailvideos.models
 
 
 class Migration(migrations.Migration):
 
@@ -16,15 +15,22 @@
     ]
 
     operations = [
         migrations.CreateModel(
             name='VideoTranscode',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('media_format', enumchoicefield.fields.EnumChoiceField(enum_class=wagtailvideos.models.MediaFormats, max_length=4)),
+                ('media_format', models.CharField(
+                    choices=[
+                        ("webm", "VP8 and Vorbis in WebM"),
+                        ("mp4", "H.264 and AAC in Mp4"),
+                        ("ogg", "Theora and Vorbis in Ogg"),
+                    ],
+                    max_length=4,
+                )),
                 ('processing', models.BooleanField(default=False)),
                 ('file', models.FileField(null=True, upload_to=wagtailvideos.models.get_upload_to, verbose_name='file')),
                 ('video', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='transcodes', to='wagtailvideos.Video')),
             ],
         ),
         migrations.AlterUniqueTogether(
             name='videotranscode',
```

### Comparing `wagtailvideos-6.0.0/wagtailvideos/migrations/0004_auto_20160706_1153.py` & `wagtailvideos-6.1.0/wagtailvideos/migrations/0004_auto_20160706_1153.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/migrations/0006_auto_20160707_1413.py` & `wagtailvideos-6.1.0/wagtailvideos/migrations/0006_auto_20160707_1413.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/migrations/0011_video_tracks.py` & `wagtailvideos-6.1.0/wagtailvideos/migrations/0011_video_tracks.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/migrations/0012_remove_unique_constraint.py` & `wagtailvideos-6.1.0/wagtailvideos/migrations/0012_remove_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/migrations/0013_add_choose_permissions.py` & `wagtailvideos-6.1.0/wagtailvideos/migrations/0013_add_choose_permissions.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/migrations/0014_alter_videotrack_file_alter_videotrack_kind_and_more.py` & `wagtailvideos-6.1.0/wagtailvideos/migrations/0014_alter_videotrack_file_alter_videotrack_kind_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/models.py` & `wagtailvideos-6.1.0/wagtailvideos/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,42 @@
 import logging
 import mimetypes
 import os
 import os.path
-import shutil
-import subprocess
-import tempfile
-import threading
 
 import bcp47
 from django.conf import settings
 from django.core.exceptions import SuspiciousFileOperation
-from django.core.files.base import ContentFile
 from django.db import models
 from django.forms.utils import flatatt
 from django.urls import reverse
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
-from enumchoicefield import ChoiceEnum, EnumChoiceField
 from modelcluster.fields import ParentalKey
 from modelcluster.models import ClusterableModel
 from taggit.managers import TaggableManager
 from wagtail.admin.models import get_object_usage
 from wagtail.models import CollectionMember, Orderable
 from wagtail.search import index
 from wagtail.search.queryset import SearchableQuerySetMixin
 
+from . import get_transcoder_backend
+from .enums import MediaFormats, VideoQuality, VideoTrackKind
+
 logger = logging.getLogger(__name__)
 
 
-class VideoQuality(ChoiceEnum):
-    default = 'Default'
-    lowest = 'Low'
-    highest = 'High'
-
-
-class MediaFormats(ChoiceEnum):
-    webm = 'VP8 and Vorbis in WebM'
-    mp4 = 'H.264 and AAC in Mp4'
-    ogg = 'Theora and Vorbis in Ogg'
-
-    def get_quality_param(self, quality):
-        if self is MediaFormats.webm:
-            return {
-                VideoQuality.lowest: '50',
-                VideoQuality.default: '22',
-                VideoQuality.highest: '4'
-            }[quality]
-        elif self is MediaFormats.mp4:
-            return {
-                VideoQuality.lowest: '28',
-                VideoQuality.default: '24',
-                VideoQuality.highest: '18'
-            }[quality]
-        elif self is MediaFormats.ogg:
-            return {
-                VideoQuality.lowest: '5',
-                VideoQuality.default: '7',
-                VideoQuality.highest: '9'
-            }[quality]
+def _choices(text_choices, max_length=None):
+    """Return a kwargs dict for adding choices and max_length to a CharField"""
+    if max_length is None:
+        max_length = max([len(choice) for choice in text_choices.values])
+    return {
+        "choices": text_choices.choices,
+        "max_length": max_length,
+    }
 
 
 class VideoQuerySet(SearchableQuerySetMixin, models.QuerySet):
     pass
 
 
 def get_upload_to(instance, filename):
@@ -80,27 +55,29 @@
         settings.AUTH_USER_MODEL, verbose_name=_('uploaded by user'),
         null=True, blank=True, editable=False, on_delete=models.SET_NULL
     )
 
     tags = TaggableManager(help_text=None, blank=True, verbose_name=_('tags'))
 
     file_size = models.PositiveIntegerField(null=True, editable=False)
+    width = models.IntegerField(verbose_name=_("width"), editable=False, null=True)
+    height = models.IntegerField(verbose_name=_("height"), editable=False, null=True)
 
     objects = VideoQuerySet.as_manager()
 
     search_fields = list(CollectionMember.search_fields) + [
         index.AutocompleteField('title', boost=10),
         index.RelatedFields('tags', [
             index.AutocompleteField('name', boost=10),
         ]),
         index.FilterField('uploaded_by_user'),
     ]
 
     def __init__(self, *args, **kwargs):
-        super(AbstractVideo, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self._initial_file = self.file
 
     def get_file_size(self):
         if self.file_size is None:
             try:
                 self.file_size = self.file.size
             except OSError:
@@ -141,17 +118,14 @@
             minutes, seconds = divmod(remainder, 60)
             return "%d:%02d:%02d" % (hours, minutes, seconds)
         return ''
 
     def __str__(self):
         return self.title
 
-    def save(self, **kwargs):
-        super(AbstractVideo, self).save(**kwargs)
-
     @property
     def url(self):
         return self.file.url
 
     def filename(self, include_ext=True):
         if include_ext:
             return os.path.basename(self.file.name)
@@ -216,15 +190,17 @@
         if created or transcode.processing is False:
             transcode.processing = True
             transcode.error_messages = ''
             transcode.quality = quality
             # Lock the transcode model
             transcode.save(update_fields=['processing', 'error_message',
                                           'quality'])
-            TranscodingThread(transcode).start()
+            # Generate the transcode using the selected transcoding backend
+            backend = get_transcoder_backend()
+            backend.do_transcode(transcode)
         else:
             pass  # TODO Queue?
 
     class Meta:
         abstract = True
 
 
@@ -240,97 +216,17 @@
     class Meta:
         ordering = ['-created_at']
         permissions = [
             ("choose_video", "Can choose video"),
         ]
 
 
-class TranscodingThread(threading.Thread):
-    def __init__(self, transcode, **kwargs):
-        super(TranscodingThread, self).__init__(**kwargs)
-        self.transcode = transcode
-
-    def get_file_url(self, file):
-        input_file = None
-
-        # Check if it is a local file
-        try:
-            input_file = file.path
-        except NotImplementedError:
-            input_file = None
-
-        if input_file:
-            return input_file
-
-        # Check if it is a file stored with django-storages
-        try:
-            input_file = file.url
-        except NotImplementedError:
-            input_file = None
-
-        return input_file
-
-    def run(self):
-        video = self.transcode.video
-        media_format = self.transcode.media_format
-        input_file = self.get_file_url(video.file)
-
-        if not input_file:
-            raise ValueError(
-                "Invalid input_file value {0} for file {1}".format(input_file, video.file)
-            )
-
-        output_dir = tempfile.mkdtemp()
-        transcode_name = "{0}.{1}".format(
-            video.filename(include_ext=False),
-            media_format.name)
-
-        output_file = os.path.join(output_dir, transcode_name)
-        FNULL = open(os.devnull, 'r')
-        quality_param = media_format.get_quality_param(self.transcode.quality)
-        args = ['ffmpeg', '-hide_banner', '-i', input_file]
-        try:
-            if media_format is MediaFormats.ogg:
-                subprocess.check_output(args + [
-                    '-codec:v', 'libtheora',
-                    '-qscale:v', quality_param,
-                    '-codec:a', 'libvorbis',
-                    '-qscale:a', '5',
-                    output_file,
-                ], stdin=FNULL, stderr=subprocess.STDOUT)
-            elif media_format is MediaFormats.mp4:
-                subprocess.check_output(args + [
-                    '-codec:v', 'libx264',
-                    '-preset', 'slow',  # TODO Checkout other presets
-                    '-crf', quality_param,
-                    '-codec:a', 'aac',
-                    output_file,
-                ], stdin=FNULL, stderr=subprocess.STDOUT)
-            elif media_format is MediaFormats.webm:
-                subprocess.check_output(args + [
-                    '-codec:v', 'libvpx',
-                    '-crf', quality_param,
-                    '-codec:a', 'libvorbis',
-                    output_file,
-                ], stdin=FNULL, stderr=subprocess.STDOUT)
-            self.transcode.file = ContentFile(
-                open(output_file, 'rb').read(), transcode_name)
-            self.transcode.error_message = ''
-        except subprocess.CalledProcessError as error:
-            self.transcode.error_message = error.output
-
-        finally:
-            self.transcode.processing = False
-            self.transcode.save()
-            shutil.rmtree(output_dir, ignore_errors=True)
-
-
 class AbstractVideoTranscode(models.Model):
-    media_format = EnumChoiceField(MediaFormats)
-    quality = EnumChoiceField(VideoQuality, default=VideoQuality.default)
+    media_format = models.CharField(**_choices(MediaFormats))
+    quality = models.CharField(**_choices(VideoQuality), default=VideoQuality.DEFAULT)
     processing = models.BooleanField(default=False)
     file = models.FileField(null=True, blank=True, verbose_name=_('file'),
                             upload_to=get_upload_to)
     error_message = models.TextField(blank=True)
 
     @property
     def url(self):
@@ -367,28 +263,19 @@
 class TrackListing(AbstractTrackListing):
     video = models.OneToOneField(
         Video, on_delete=models.CASCADE,
         related_name='track_listing')
 
 
 class AbstractVideoTrack(Orderable):
-    # TODO move to TextChoices once django < 3 is dropped
-    track_kinds = [
-        ('subtitles', _('Subtitles')),
-        ('captions', _('Captions')),
-        ('descriptions', _('Descriptions')),
-        ('chapters', _('Chapters')),
-        ('metadata', _('Metadata')),
-    ]
-
     file = models.FileField(
         verbose_name=_('File'),
         upload_to=get_upload_to
     )
-    kind = models.CharField(max_length=50, choices=track_kinds, default=track_kinds[0][0], verbose_name=_('Kind'))
+    kind = models.CharField(**_choices(VideoTrackKind, max_length=50), default=VideoTrackKind.SUBTITLES, verbose_name=_('Kind'))
     label = models.CharField(
         max_length=255, blank=True,
         help_text=_('A user-readable title of the text track.'),
         verbose_name=_('Label'))
     language = models.CharField(
         max_length=50,
         choices=[(v, k) for k, v in bcp47.languages.items()],
```

### Comparing `wagtailvideos-6.0.0/wagtailvideos/signals.py` & `wagtailvideos-6.1.0/wagtailvideos/signals.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from contextlib import contextmanager
 
 from django.core.files.temp import NamedTemporaryFile
 from django.db import transaction
 from django.db.models.signals import post_delete, post_save
 
-from wagtailvideos import ffmpeg, get_video_model
+from wagtailvideos import get_transcoder_backend, get_video_model
 
 
 @contextmanager
 def get_local_file(file):
     """
     Get a local version of the file, downloading it from the remote storage if
     required. The returned value should be used as a context manager to
@@ -35,33 +35,23 @@
     # Pass false so FileField doesn't save the model.
     transaction.on_commit(lambda: instance.file.delete(False))
     if hasattr(instance, 'thumbnail'):
         # Delete the thumbnail for videos too
         transaction.on_commit(lambda: instance.thumbnail.delete(False))
 
 
-# Fields that need the actual video file to create using ffmpeg
+# Fields that need the actual video file to create using the transcoding backend.
 def video_post_save(instance, **kwargs):
-    if not ffmpeg.installed():
+    backend = get_transcoder_backend()
+    if not backend.installed():
         return
-
     if hasattr(instance, '_from_signal'):
         # Sender was us, don't run post save
         return
-
-    has_changed = instance._initial_file is not instance.file
-    filled_out = instance.thumbnail is not None and instance.duration is not None
-    if has_changed or not filled_out:
-        with get_local_file(instance.file) as file_path:
-            if has_changed or instance.thumbnail is None:
-                instance.thumbnail = ffmpeg.get_thumbnail(file_path)
-
-            if has_changed or instance.duration is None:
-                instance.duration = ffmpeg.get_duration(file_path)
-
+    backend.update_video_metadata(instance)
     instance.file_size = instance.file.size
     instance._from_signal = True
     instance.save()
     del instance._from_signal
 
 
 def register_signal_handlers():
```

### Comparing `wagtailvideos-6.0.0/wagtailvideos/static/wagtailvideos/js/add-multiple.js` & `wagtailvideos-6.1.0/wagtailvideos/static/wagtailvideos/js/add-multiple.js`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/chooser/chooser.html` & `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/chooser/chooser.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/chooser/results.html` & `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/chooser/results.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/homepage/videos_summary.html` & `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/homepage/videos_summary.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/multiple/add.html` & `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/multiple/add.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/multiple/edit_form.html` & `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/multiple/edit_form.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/add.html` & `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/add.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/confirm_delete.html` & `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/edit.html` & `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/edit.html`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,14 @@
                     <dd>
                         <a href="{{ video.usage_url }}">{% blocktrans count usage_count=video.get_usage.count %}Used {{ usage_count }} time{% plural %}Used {{ usage_count }} times{% endblocktrans %}</a>
                     </dd>
                 </dl>
             </div>
         </div>
         <div class="row" style="margin-top: 2em;">
-        {% if can_transcode %}
             <h2 class="u-text-transform-uppercase">{% trans "Transcodes" %}</h2>
             <p>{% trans "If you wish to generate HTML5 compliant transcodes use the form below. This may take a while depending on the length of the video." %}</p>
             {% if transcodes %}
             <h3 class="u-text-transform-uppercase">{% trans "Available Transcodes" %}</h3>
             <ul>
                 {% for transcode in transcodes %}
                 <li>
@@ -102,27 +101,34 @@
                         </div>
                     {% endif %}
                 </li>
                 {% endfor %}
             </ul>
             {% endif %}
             <h3 class="u-text-transform-uppercase">{% trans "Create transcode" %}</h3>
+        {% if transcoder_installed and transcoder_enabled %}
             <form action="{% url 'wagtailvideos:create_transcode' video.id %}" method="POST">
                 <ul class="fields">
                     {% csrf_token %}
                     <li>{% include "wagtailadmin/shared/field.html" with field=transcode_form.media_format li_classes="label-above label-uppercase" %}</li>
                     <li>{% include "wagtailadmin/shared/field.html" with field=transcode_form.quality li_classes="label-above label-uppercase" %}</li>
                     <li>
                         <input class="button" type="submit" value="{% trans 'Start' %}" />
                     </li>
                 </ul>
             </form>
+        {% elif transcoder_installed and not transcoder_enabled %}
+            <br/><br/>
+            <span class="transcode-error">{% trans "Transcoding is disabled." %}</span>
+        {% elif not transcoder_installed and transcoder_enabled %}
+            <br/><br/>
+            <span class="transcode-error">{% trans "The selected transcoding backend is not installed on your server." %}</span>
         {% else %}
             <br/><br/>
-            <span class="transcode-error">{% trans "Ffmpeg is not found on your server or you have disabled transcodes. Please install Ffmepg and make sure that transcoding is enabled if you wish to transcode videos into an HTML5 video compliant format." %}</span>
+            <span class="transcode-error">{% trans "The selected transcoding backend is not installed on your server and you have disabled transcodes. Please install the backend requirements and enable transcoding if you wish to transcode videos into an HTML5 video compliant format." %}</span>
         {% endif %}
         {% if tracks_action_url %}
             <h2 class="u-text-transform-uppercase">{% trans "Tracks" %}</h2>
             <p>{% trans 'You can add/edit subtitles or accessibility captions for this video. For information about the filetype that should be used see the mozilla docs on <a href="https://developer.mozilla.org/en-US/docs/Web/API/WebVTT_API">WebVTT</a>' %}</p>
                 {% if video.track_listing %}
                 <ul>
                 {% for track in video.track_listing.tracks.all %}
```

### Comparing `wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/index.html` & `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/index.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/results.html` & `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/results.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/usage.html` & `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/usage.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/templatetags/wagtailvideos_tags.py` & `wagtailvideos-6.1.0/wagtailvideos/templatetags/wagtailvideos_tags.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/urls.py` & `wagtailvideos-6.1.0/wagtailvideos/urls.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/views/chooser.py` & `wagtailvideos-6.1.0/wagtailvideos/views/chooser.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/views/multiple.py` & `wagtailvideos-6.1.0/wagtailvideos/views/multiple.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/views/videos.py` & `wagtailvideos-6.1.0/wagtailvideos/views/videos.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from wagtail.admin.auth import PermissionPolicyChecker
 from wagtail.admin.forms.search import SearchForm
 from wagtail.admin.models import popular_tags_for_model
 from wagtail.models import Collection
 from wagtail.search.backends import get_search_backends
 from wagtail_modeladmin.helpers import AdminURLHelper
 
-from wagtailvideos import ffmpeg, get_video_model, is_modeladmin_installed
+from wagtailvideos import (
+    get_transcoder_backend, get_video_model, is_modeladmin_installed)
 from wagtailvideos.forms import VideoTranscodeAdminForm, get_video_form
 from wagtailvideos.permissions import permission_policy
 
 permission_checker = PermissionPolicyChecker(permission_policy)
 
 
 @permission_checker.require_any('add', 'change', 'delete', 'choose')
@@ -129,15 +130,16 @@
     else:
         action_url = ''
 
     return render(request, "wagtailvideos/videos/edit.html", {
         'video': video,
         'form': form,
         'filesize': video.get_file_size(),
-        'can_transcode': ffmpeg.installed() and not getattr(settings, 'WAGTAIL_VIDEOS_DISABLE_TRANSCODE', False),
+        'transcoder_installed': get_transcoder_backend().installed(),
+        'transcoder_enabled': not getattr(settings, 'WAGTAIL_VIDEOS_DISABLE_TRANSCODE', False),
         'transcodes': video.transcodes.all(),
         'transcode_form': VideoTranscodeAdminForm(video=video),
         'tracks_action_url': action_url,
         'user_can_delete': permission_policy.user_has_permission_for_instance(request.user, 'delete', video)
     })
```

### Comparing `wagtailvideos-6.0.0/wagtailvideos/wagtail_hooks.py` & `wagtailvideos-6.1.0/wagtailvideos/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos/widgets.py` & `wagtailvideos-6.1.0/wagtailvideos/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.0.0/wagtailvideos.egg-info/PKG-INFO` & `wagtailvideos-6.1.0/wagtailvideos.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailvideos
-Version: 6.0.0
+Version: 6.1.0
 Summary: A wagtail module for uploading and displaying videos in various codecs.
 Home-page: https://github.com/neon-jungle/wagtailvideos
 Author: Neon Jungle
 Author-email: developers@neonjungle.studio
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: BSD License
 License-File: LICENSE
 Requires-Dist: wagtail>=5.2
 Requires-Dist: Django>=3.2
-Requires-Dist: django-enumchoicefield>=1.1.0
 Requires-Dist: bcp47==0.0.4
 Requires-Dist: wagtail-modeladmin>=2.0.0
 
 wagtailvideos
 =============
 
 .. image:: https://gitlab.com/neonjungle/wagtailvideos/badges/master/pipeline.svg
@@ -35,16 +34,16 @@
 Based on wagtailimages. The aim was to have feature parity with images
 but for html5 videos. Includes the ability to transcode videos to a
 html5 compliant codec using ffmpeg.
 
 Requirements
 ------------
 
--  Wagtail >= 4.0 (for older wagtail version see the tags)
--  `ffmpeg <https://ffmpeg.org/>`__
+-  Wagtail >= 5.2 (for older wagtail version see the tags)
+-  `ffmpeg <https://ffmpeg.org/>`__ (optional, for transcoding)
 
 Installing
 ----------
 
 Install using pypi
 
 .. code:: bash
```

### Comparing `wagtailvideos-6.0.0/wagtailvideos.egg-info/SOURCES.txt` & `wagtailvideos-6.1.0/wagtailvideos.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 tests/app/models.py
 tests/app/settings.py
 tests/app/test_block.py
 tests/app/urls.py
 tests/app/migrations/0001_initial.py
 tests/app/migrations/0002_alter_testpage_video_streamfield.py
 tests/app/migrations/0003_alter_customvideotrack_file_and_more.py
+tests/app/migrations/0004_customvideomodel_height_customvideomodel_width.py
 tests/app/migrations/__init__.py
 wagtailvideos/__init__.py
 wagtailvideos/apps.py
 wagtailvideos/blocks.py
 wagtailvideos/edit_handlers.py
-wagtailvideos/ffmpeg.py
+wagtailvideos/enums.py
 wagtailvideos/fields.py
 wagtailvideos/forms.py
 wagtailvideos/jinja2tags.py
 wagtailvideos/models.py
 wagtailvideos/permissions.py
 wagtailvideos/signals.py
 wagtailvideos/urls.py
@@ -50,14 +51,15 @@
 wagtailvideos/migrations/0008_auto_20160728_1523.py
 wagtailvideos/migrations/0009_videotranscode_quality.py
 wagtailvideos/migrations/0010_video_ordering.py
 wagtailvideos/migrations/0011_video_tracks.py
 wagtailvideos/migrations/0012_remove_unique_constraint.py
 wagtailvideos/migrations/0013_add_choose_permissions.py
 wagtailvideos/migrations/0014_alter_videotrack_file_alter_videotrack_kind_and_more.py
+wagtailvideos/migrations/0015_video_height_video_width.py
 wagtailvideos/migrations/__init__.py
 wagtailvideos/static/wagtailvideos/css/edit-video.css
 wagtailvideos/static/wagtailvideos/css/summary-override.css
 wagtailvideos/static/wagtailvideos/js/add-multiple.js
 wagtailvideos/static/wagtailvideos/js/video-chooser-telepath.js
 wagtailvideos/static/wagtailvideos/js/video-chooser.js
 wagtailvideos/templates/wagtailvideos/chooser/chooser.html
@@ -73,11 +75,16 @@
 wagtailvideos/templates/wagtailvideos/videos/edit.html
 wagtailvideos/templates/wagtailvideos/videos/index.html
 wagtailvideos/templates/wagtailvideos/videos/results.html
 wagtailvideos/templates/wagtailvideos/videos/usage.html
 wagtailvideos/templates/wagtailvideos/widgets/video_chooser.html
 wagtailvideos/templatetags/__init__.py
 wagtailvideos/templatetags/wagtailvideos_tags.py
+wagtailvideos/transcoders/__init__.py
+wagtailvideos/transcoders/base/__init__.py
+wagtailvideos/transcoders/ffmpeg/__init__.py
+wagtailvideos/transcoders/ffmpeg/checks.py
+wagtailvideos/transcoders/ffmpeg/ffmpeg.py
 wagtailvideos/views/__init__.py
 wagtailvideos/views/chooser.py
 wagtailvideos/views/multiple.py
 wagtailvideos/views/videos.py
```


# Comparing `tmp/django_medicio_dental-3.1.3.tar.gz` & `tmp/django_medicio_dental-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_medicio_dental-3.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_medicio_dental-3.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_medicio_dental-3.1.3.tar` & `django_medicio_dental-3.1.4.tar`

### file list

```diff
@@ -1,169 +1,169 @@
--rw-r--r--   0        0        0       66 2024-05-10 00:04:11.365474 django_medicio_dental-3.1.3/.gitattributes
--rw-r--r--   0        0        0       20 2024-05-10 08:36:39.396618 django_medicio_dental-3.1.3/.gitignore
--rw-r--r--   0        0        0       52 2024-05-10 04:53:43.020484 django_medicio_dental-3.1.3/.idea/.gitignore
--rw-r--r--   0        0        0      411 2024-05-10 03:12:13.743449 django_medicio_dental-3.1.3/.idea/django-medicio-dental.iml
--rw-r--r--   0        0        0      174 2024-05-10 03:12:13.754363 django_medicio_dental-3.1.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      433 2024-05-10 03:12:13.750597 django_medicio_dental-3.1.3/.idea/misc.xml
--rw-r--r--   0        0        0      294 2024-05-10 03:12:13.747760 django_medicio_dental-3.1.3/.idea/modules.xml
--rw-r--r--   0        0        0      167 2024-05-10 03:12:13.779428 django_medicio_dental-3.1.3/.idea/vcs.xml
--rw-r--r--   0        0        0     1079 2024-03-19 03:45:10.033383 django_medicio_dental-3.1.3/LICENSE
--rw-r--r--   0        0        0     4904 2024-05-18 19:45:24.875146 django_medicio_dental-3.1.3/README.md
--rw-r--r--   0        0        0        0 2024-05-10 02:24:17.561066 django_medicio_dental-3.1.3/django_medicio_dental/__init__.py
--rw-r--r--   0        0        0      351 2024-05-16 05:19:53.069921 django_medicio_dental-3.1.3/django_medicio_dental/admin.py
--rw-r--r--   0        0        0      172 2024-05-10 03:09:57.361322 django_medicio_dental-3.1.3/django_medicio_dental/apps.py
--rw-r--r--   0        0        0      921 2024-05-14 03:31:23.512523 django_medicio_dental-3.1.3/django_medicio_dental/forms.py
--rw-r--r--   0        0        0     1867 2024-05-16 04:53:15.905318 django_medicio_dental-3.1.3/django_medicio_dental/migrations/0001_initial.py
--rw-r--r--   0        0        0      434 2024-05-16 05:44:15.309477 django_medicio_dental-3.1.3/django_medicio_dental/migrations/0002_alter_post_content.py
--rw-r--r--   0        0        0      602 2024-05-16 05:48:19.985375 django_medicio_dental-3.1.3/django_medicio_dental/migrations/0003_alter_post_content_alter_post_title.py
--rw-r--r--   0        0        0      627 2024-05-16 05:49:02.132131 django_medicio_dental-3.1.3/django_medicio_dental/migrations/0004_alter_post_content_alter_post_title.py
--rw-r--r--   0        0        0      476 2024-05-16 05:50:27.312461 django_medicio_dental-3.1.3/django_medicio_dental/migrations/0005_alter_post_content.py
--rw-r--r--   0        0        0      450 2024-05-16 05:51:10.141288 django_medicio_dental-3.1.3/django_medicio_dental/migrations/0006_alter_post_content.py
--rw-r--r--   0        0        0        0 2024-05-07 01:25:47.437616 django_medicio_dental-3.1.3/django_medicio_dental/migrations/__init__.py
--rw-r--r--   0        0        0     1606 2024-05-22 07:09:45.996521 django_medicio_dental-3.1.3/django_medicio_dental/models.py
--rw-r--r--   0        0        0      655 2024-05-22 07:09:45.987770 django_medicio_dental-3.1.3/django_medicio_dental/sitemaps.py
--rwxr-xr-x   0        0        0    31935 2024-05-21 00:47:46.131096 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/css/style.css
--rwxr-xr-x   0        0        0     6591 2024-03-17 05:37:08.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/js/main.js
--rwxr-xr-x   0        0        0     3011 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/scss/_footer.scss
--rwxr-xr-x   0        0        0     2001 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/scss/_general.scss
--rwxr-xr-x   0        0        0     1504 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/scss/_header.scss
--rwxr-xr-x   0        0        0     3329 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/scss/_hero.scss
--rwxr-xr-x   0        0        0     3670 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/scss/_nav.scss
--rwxr-xr-x   0        0        0    20148 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/scss/_sections.scss
--rwxr-xr-x   0        0        0      453 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/scss/_variables.scss
--rwxr-xr-x   0        0        0      136 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/scss/style.scss
--rw-r--r--   0        0        0    70607 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/animate.css/animate.compat.css
--rw-r--r--   0        0        0    95374 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/animate.css/animate.css
--rwxr-xr-x   0        0        0    71750 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/animate.css/animate.min.css
--rw-r--r--   0        0        0    19941 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/aos/aos.cjs.js
--rw-r--r--   0        0        0    28765 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/aos/aos.css
--rw-r--r--   0        0        0    19768 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/aos/aos.esm.js
--rw-r--r--   0        0        0    13800 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/aos/aos.js
--rw-r--r--   0        0        0    56459 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/aos/aos.js.map
--rw-r--r--   0        0        0    98255 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/bootstrap-icons.css
--rw-r--r--   0        0        0    52358 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/bootstrap-icons.json
--rw-r--r--   0        0        0    85875 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/bootstrap-icons.min.css
--rw-r--r--   0        0        0    57755 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/bootstrap-icons.scss
--rw-r--r--   0        0        0   176032 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
--rw-r--r--   0        0        0   130396 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
--rw-r--r--   0        0        0    70329 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0        0        0   203221 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0        0        0    51795 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0        0        0   115986 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0        0        0    70403 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.rtl.css
--rw-r--r--   0        0        0   203225 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0        0        0    51870 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0        0        0   116063 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0        0        0    12065 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0        0        0   129371 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0        0        0    10126 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0        0        0    51369 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0        0        0    12058 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.rtl.css
--rw-r--r--   0        0        0   129386 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0        0        0    10198 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0        0        0    63943 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0        0        0   107823 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.css
--rw-r--r--   0        0        0   267535 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.css.map
--rw-r--r--   0        0        0    85352 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.min.css
--rw-r--r--   0        0        0   180381 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.min.css.map
--rw-r--r--   0        0        0   107691 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.rtl.css
--rw-r--r--   0        0        0   267476 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0        0        0    85281 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0        0        0   180217 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0        0        0   281046 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.css
--rw-r--r--   0        0        0   679755 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.css.map
--rw-r--r--   0        0        0   232803 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.min.css
--rw-r--r--   0        0        0   589892 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.min.css.map
--rw-r--r--   0        0        0   280259 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.rtl.css
--rw-r--r--   0        0        0   679615 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.rtl.css.map
--rw-r--r--   0        0        0   232911 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.rtl.min.css
--rw-r--r--   0        0        0   589087 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.rtl.min.css.map
--rw-r--r--   0        0        0   207819 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0        0        0   444579 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0        0        0    80721 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   332090 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0   135829 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.esm.js
--rw-r--r--   0        0        0   305438 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.esm.js.map
--rw-r--r--   0        0        0    73935 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.esm.min.js
--rw-r--r--   0        0        0   222455 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.esm.min.js.map
--rw-r--r--   0        0        0   145401 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.js
--rw-r--r--   0        0        0   306606 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.js.map
--rw-r--r--   0        0        0    60635 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.min.js
--rw-r--r--   0        0        0   220561 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.min.js.map
--rw-r--r--   0        0        0     7522 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/boxicons/css/animations.css
--rw-r--r--   0        0        0    94202 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/boxicons/css/boxicons.css
--rw-r--r--   0        0        0    68028 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/boxicons/css/boxicons.min.css
--rw-r--r--   0        0        0      683 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/boxicons/css/transformations.css
--rw-r--r--   0        0        0   405670 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/boxicons/fonts/boxicons.eot
--rw-r--r--   0        0        0  1242122 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/boxicons/fonts/boxicons.svg
--rw-r--r--   0        0        0   320944 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/boxicons/fonts/boxicons.ttf
--rw-r--r--   0        0        0   321020 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/boxicons/fonts/boxicons.woff
--rw-r--r--   0        0        0   115680 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/boxicons/fonts/boxicons.woff2
--rw-r--r--   0        0        0   141265 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/all.css
--rw-r--r--   0        0        0   103009 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/all.min.css
--rw-r--r--   0        0        0    24920 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/brands.css
--rw-r--r--   0        0        0    19582 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/brands.min.css
--rw-r--r--   0        0        0   113480 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/fontawesome.css
--rw-r--r--   0        0        0    80888 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/fontawesome.min.css
--rw-r--r--   0        0        0      633 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/regular.css
--rw-r--r--   0        0        0      580 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/regular.min.css
--rw-r--r--   0        0        0      625 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/solid.css
--rw-r--r--   0        0        0      572 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/solid.min.css
--rw-r--r--   0        0        0    21696 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/svg-with-js.css
--rw-r--r--   0        0        0    17011 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/svg-with-js.min.css
--rw-r--r--   0        0        0     1831 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v4-font-face.css
--rw-r--r--   0        0        0     1736 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v4-font-face.min.css
--rw-r--r--   0        0        0    41574 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v4-shims.css
--rw-r--r--   0        0        0    27593 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v4-shims.min.css
--rw-r--r--   0        0        0      871 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v5-font-face.css
--rw-r--r--   0        0        0      794 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v5-font-face.min.css
--rw-r--r--   0        0        0   209128 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   117852 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    67860 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    25392 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   420332 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   156400 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0    10832 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0        0        0     4792 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0        0        0    17372 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/glightbox/css/glightbox.css
--rw-r--r--   0        0        0    13749 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/glightbox/css/glightbox.min.css
--rw-r--r--   0        0        0   109600 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/glightbox/js/glightbox.js
--rw-r--r--   0        0        0    56300 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/glightbox/js/glightbox.min.js
--rwxr-xr-x   0        0        0   238381 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/php-email-form/php-email-form.php
--rwxr-xr-x   0        0        0     2734 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/php-email-form/validate.js
--rw-r--r--   0        0        0     5417 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/purecounter/purecounter_vanilla.js
--rw-r--r--   0        0        0    24750 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/purecounter/purecounter_vanilla.js.map
--rw-r--r--   0        0        0    18432 2024-04-20 04:09:20.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/swiper/swiper-bundle.min.css
--rw-r--r--   0        0        0   149982 2024-04-20 04:09:20.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/swiper/swiper-bundle.min.js
--rw-r--r--   0        0        0   203001 2024-04-20 04:09:20.000000 django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/swiper/swiper-bundle.min.js.map
--rw-r--r--   0        0        0      930 2024-05-22 07:22:08.525475 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_about.html
--rw-r--r--   0        0        0     1222 2024-05-22 07:22:08.544094 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_appointment.html
--rw-r--r--   0        0        0     2428 2024-05-23 06:22:42.970890 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_contact.html
--rw-r--r--   0        0        0      720 2024-05-14 03:38:12.580371 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_counts.html
--rw-r--r--   0        0        0      818 2024-05-14 02:32:22.775343 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_cta.html
--rw-r--r--   0        0        0     1424 2024-05-22 07:22:08.549047 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_departments.html
--rw-r--r--   0        0        0     1469 2024-05-22 07:22:08.538864 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_doctors.html
--rw-r--r--   0        0        0      772 2024-05-08 05:23:38.100357 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_faq.html
--rw-r--r--   0        0        0      704 2024-05-09 04:50:22.638693 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_featured-services.html
--rw-r--r--   0        0        0      684 2024-05-22 07:22:08.536885 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_features.html
--rw-r--r--   0        0        0      728 2024-05-22 07:22:08.541512 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_gallery.html
--rw-r--r--   0        0        0     1272 2024-05-22 07:22:08.534815 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_hero.html
--rw-r--r--   0        0        0     1173 2024-05-09 00:34:34.141381 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_pricing.html
--rw-r--r--   0        0        0      656 2024-05-17 04:33:21.960157 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_services.html
--rw-r--r--   0        0        0     1046 2024-05-22 07:22:08.546232 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_testimonials.html
--rwxr-xr-x   0        0        0      490 2024-05-23 00:55:55.332489 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/blog-details.html
--rw-r--r--   0        0        0      376 2024-05-23 00:36:35.191410 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/breadcrumb.html
--rw-r--r--   0        0        0     3139 2024-05-23 08:08:10.471537 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/footer.html
--rwxr-xr-x   0        0        0     1579 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/forms/appointment.php
--rwxr-xr-x   0        0        0     1341 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/forms/contact.php
--rw-r--r--   0        0        0     2037 2024-05-22 07:22:08.529063 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/header.html
--rwxr-xr-x   0        0        0     4614 2024-05-22 07:14:37.245804 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/index.html
--rwxr-xr-x   0        0        0    16287 2024-05-23 00:41:03.798823 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/privacy.html
--rw-r--r--   0        0        0     1933 2024-05-22 07:22:08.532372 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/seo.html
--rwxr-xr-x   0        0        0    16327 2024-05-23 00:41:03.804529 django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/terms.html
--rw-r--r--   0        0        0        0 2023-03-21 07:32:09.033136 django_medicio_dental-3.1.3/django_medicio_dental/templatetags/__init__.py
--rw-r--r--   0        0        0     5988 2024-05-22 07:14:37.250671 django_medicio_dental-3.1.3/django_medicio_dental/templatetags/mediciodental_tags.py
--rw-r--r--   0        0        0       60 2024-05-07 01:25:47.437462 django_medicio_dental-3.1.3/django_medicio_dental/tests.py
--rw-r--r--   0        0        0      827 2024-05-22 07:09:45.998807 django_medicio_dental-3.1.3/django_medicio_dental/urls.py
--rw-r--r--   0        0        0     4288 2024-05-22 23:59:16.822501 django_medicio_dental-3.1.3/django_medicio_dental/views.py
--rw-r--r--   0        0        0      973 2024-05-23 08:08:51.627961 django_medicio_dental-3.1.3/pyproject.toml
--rw-r--r--   0        0        0     5644 1970-01-01 00:00:00.000000 django_medicio_dental-3.1.3/PKG-INFO
+-rw-r--r--   0        0        0       66 2024-05-10 00:04:11.365474 django_medicio_dental-3.1.4/.gitattributes
+-rw-r--r--   0        0        0       20 2024-05-10 08:36:39.396618 django_medicio_dental-3.1.4/.gitignore
+-rw-r--r--   0        0        0       52 2024-05-10 04:53:43.020484 django_medicio_dental-3.1.4/.idea/.gitignore
+-rw-r--r--   0        0        0      411 2024-05-10 03:12:13.743449 django_medicio_dental-3.1.4/.idea/django-medicio-dental.iml
+-rw-r--r--   0        0        0      174 2024-05-10 03:12:13.754363 django_medicio_dental-3.1.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      433 2024-05-10 03:12:13.750597 django_medicio_dental-3.1.4/.idea/misc.xml
+-rw-r--r--   0        0        0      294 2024-05-10 03:12:13.747760 django_medicio_dental-3.1.4/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2024-05-10 03:12:13.779428 django_medicio_dental-3.1.4/.idea/vcs.xml
+-rw-r--r--   0        0        0     1079 2024-03-19 03:45:10.033383 django_medicio_dental-3.1.4/LICENSE
+-rw-r--r--   0        0        0     4904 2024-05-18 19:45:24.875146 django_medicio_dental-3.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 02:24:17.561066 django_medicio_dental-3.1.4/django_medicio_dental/__init__.py
+-rw-r--r--   0        0        0      351 2024-05-16 05:19:53.069921 django_medicio_dental-3.1.4/django_medicio_dental/admin.py
+-rw-r--r--   0        0        0      172 2024-05-10 03:09:57.361322 django_medicio_dental-3.1.4/django_medicio_dental/apps.py
+-rw-r--r--   0        0        0      921 2024-05-14 03:31:23.512523 django_medicio_dental-3.1.4/django_medicio_dental/forms.py
+-rw-r--r--   0        0        0     1867 2024-05-16 04:53:15.905318 django_medicio_dental-3.1.4/django_medicio_dental/migrations/0001_initial.py
+-rw-r--r--   0        0        0      434 2024-05-16 05:44:15.309477 django_medicio_dental-3.1.4/django_medicio_dental/migrations/0002_alter_post_content.py
+-rw-r--r--   0        0        0      602 2024-05-16 05:48:19.985375 django_medicio_dental-3.1.4/django_medicio_dental/migrations/0003_alter_post_content_alter_post_title.py
+-rw-r--r--   0        0        0      627 2024-05-16 05:49:02.132131 django_medicio_dental-3.1.4/django_medicio_dental/migrations/0004_alter_post_content_alter_post_title.py
+-rw-r--r--   0        0        0      476 2024-05-16 05:50:27.312461 django_medicio_dental-3.1.4/django_medicio_dental/migrations/0005_alter_post_content.py
+-rw-r--r--   0        0        0      450 2024-05-16 05:51:10.141288 django_medicio_dental-3.1.4/django_medicio_dental/migrations/0006_alter_post_content.py
+-rw-r--r--   0        0        0        0 2024-05-07 01:25:47.437616 django_medicio_dental-3.1.4/django_medicio_dental/migrations/__init__.py
+-rw-r--r--   0        0        0     1606 2024-05-22 07:09:45.996521 django_medicio_dental-3.1.4/django_medicio_dental/models.py
+-rw-r--r--   0        0        0      655 2024-05-22 07:09:45.987770 django_medicio_dental-3.1.4/django_medicio_dental/sitemaps.py
+-rwxr-xr-x   0        0        0    31935 2024-05-21 00:47:46.131096 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/css/style.css
+-rwxr-xr-x   0        0        0     6591 2024-03-17 05:37:08.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/js/main.js
+-rwxr-xr-x   0        0        0     3011 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/scss/_footer.scss
+-rwxr-xr-x   0        0        0     2001 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/scss/_general.scss
+-rwxr-xr-x   0        0        0     1504 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/scss/_header.scss
+-rwxr-xr-x   0        0        0     3329 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/scss/_hero.scss
+-rwxr-xr-x   0        0        0     3670 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/scss/_nav.scss
+-rwxr-xr-x   0        0        0    20148 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/scss/_sections.scss
+-rwxr-xr-x   0        0        0      453 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/scss/_variables.scss
+-rwxr-xr-x   0        0        0      136 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/scss/style.scss
+-rw-r--r--   0        0        0    70607 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/animate.css/animate.compat.css
+-rw-r--r--   0        0        0    95374 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/animate.css/animate.css
+-rwxr-xr-x   0        0        0    71750 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/animate.css/animate.min.css
+-rw-r--r--   0        0        0    19941 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/aos/aos.cjs.js
+-rw-r--r--   0        0        0    28765 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/aos/aos.css
+-rw-r--r--   0        0        0    19768 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/aos/aos.esm.js
+-rw-r--r--   0        0        0    13800 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/aos/aos.js
+-rw-r--r--   0        0        0    56459 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/aos/aos.js.map
+-rw-r--r--   0        0        0    98255 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/bootstrap-icons.css
+-rw-r--r--   0        0        0    52358 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/bootstrap-icons.json
+-rw-r--r--   0        0        0    85875 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/bootstrap-icons.min.css
+-rw-r--r--   0        0        0    57755 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/bootstrap-icons.scss
+-rw-r--r--   0        0        0   176032 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
+-rw-r--r--   0        0        0   130396 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
+-rw-r--r--   0        0        0    70329 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0        0        0   203221 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.css.map
+-rw-r--r--   0        0        0    51795 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0        0        0   115986 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.min.css.map
+-rw-r--r--   0        0        0    70403 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.rtl.css
+-rw-r--r--   0        0        0   203225 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0        0        0    51870 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0        0        0   116063 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0        0        0    12065 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0        0        0   129371 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.css.map
+-rw-r--r--   0        0        0    10126 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0        0        0    51369 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0        0        0    12058 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0        0        0   129386 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0        0        0    10198 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0        0        0    63943 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0        0        0   107823 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.css
+-rw-r--r--   0        0        0   267535 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.css.map
+-rw-r--r--   0        0        0    85352 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.min.css
+-rw-r--r--   0        0        0   180381 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0        0        0   107691 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0        0        0   267476 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0        0        0    85281 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0        0        0   180217 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0        0        0   281046 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.css
+-rw-r--r--   0        0        0   679755 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0        0        0   232803 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0        0        0   589892 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0   280259 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.rtl.css
+-rw-r--r--   0        0        0   679615 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.rtl.css.map
+-rw-r--r--   0        0        0   232911 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.rtl.min.css
+-rw-r--r--   0        0        0   589087 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0        0        0   207819 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0   444579 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0    80721 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   332090 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0   135829 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.esm.js
+-rw-r--r--   0        0        0   305438 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.esm.js.map
+-rw-r--r--   0        0        0    73935 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.esm.min.js
+-rw-r--r--   0        0        0   222455 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.esm.min.js.map
+-rw-r--r--   0        0        0   145401 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.js
+-rw-r--r--   0        0        0   306606 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0        0        0    60635 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0        0        0   220561 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0     7522 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/boxicons/css/animations.css
+-rw-r--r--   0        0        0    94202 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/boxicons/css/boxicons.css
+-rw-r--r--   0        0        0    68028 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/boxicons/css/boxicons.min.css
+-rw-r--r--   0        0        0      683 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/boxicons/css/transformations.css
+-rw-r--r--   0        0        0   405670 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/boxicons/fonts/boxicons.eot
+-rw-r--r--   0        0        0  1242122 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/boxicons/fonts/boxicons.svg
+-rw-r--r--   0        0        0   320944 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/boxicons/fonts/boxicons.ttf
+-rw-r--r--   0        0        0   321020 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/boxicons/fonts/boxicons.woff
+-rw-r--r--   0        0        0   115680 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/boxicons/fonts/boxicons.woff2
+-rw-r--r--   0        0        0   141265 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/all.css
+-rw-r--r--   0        0        0   103009 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/all.min.css
+-rw-r--r--   0        0        0    24920 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/brands.css
+-rw-r--r--   0        0        0    19582 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/brands.min.css
+-rw-r--r--   0        0        0   113480 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/fontawesome.css
+-rw-r--r--   0        0        0    80888 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/fontawesome.min.css
+-rw-r--r--   0        0        0      633 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/regular.css
+-rw-r--r--   0        0        0      580 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/regular.min.css
+-rw-r--r--   0        0        0      625 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/solid.css
+-rw-r--r--   0        0        0      572 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/solid.min.css
+-rw-r--r--   0        0        0    21696 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/svg-with-js.css
+-rw-r--r--   0        0        0    17011 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/svg-with-js.min.css
+-rw-r--r--   0        0        0     1831 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v4-font-face.css
+-rw-r--r--   0        0        0     1736 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v4-font-face.min.css
+-rw-r--r--   0        0        0    41574 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v4-shims.css
+-rw-r--r--   0        0        0    27593 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v4-shims.min.css
+-rw-r--r--   0        0        0      871 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v5-font-face.css
+-rw-r--r--   0        0        0      794 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v5-font-face.min.css
+-rw-r--r--   0        0        0   209128 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   117852 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    67860 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    25392 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   420332 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   156400 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0    10832 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0        0        0     4792 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0        0        0    17372 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/glightbox/css/glightbox.css
+-rw-r--r--   0        0        0    13749 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/glightbox/css/glightbox.min.css
+-rw-r--r--   0        0        0   109600 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/glightbox/js/glightbox.js
+-rw-r--r--   0        0        0    56300 2024-04-07 13:11:34.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/glightbox/js/glightbox.min.js
+-rwxr-xr-x   0        0        0   238381 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/php-email-form/php-email-form.php
+-rwxr-xr-x   0        0        0     2734 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/php-email-form/validate.js
+-rw-r--r--   0        0        0     5417 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/purecounter/purecounter_vanilla.js
+-rw-r--r--   0        0        0    24750 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/purecounter/purecounter_vanilla.js.map
+-rw-r--r--   0        0        0    18432 2024-04-20 04:09:20.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/swiper/swiper-bundle.min.css
+-rw-r--r--   0        0        0   149982 2024-04-20 04:09:20.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/swiper/swiper-bundle.min.js
+-rw-r--r--   0        0        0   203001 2024-04-20 04:09:20.000000 django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/swiper/swiper-bundle.min.js.map
+-rw-r--r--   0        0        0      930 2024-05-22 07:22:08.525475 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_about.html
+-rw-r--r--   0        0        0     1222 2024-05-22 07:22:08.544094 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_appointment.html
+-rw-r--r--   0        0        0     2428 2024-05-23 06:22:42.970890 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_contact.html
+-rw-r--r--   0        0        0      720 2024-05-14 03:38:12.580371 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_counts.html
+-rw-r--r--   0        0        0      818 2024-05-14 02:32:22.775343 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_cta.html
+-rw-r--r--   0        0        0     1424 2024-05-22 07:22:08.549047 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_departments.html
+-rw-r--r--   0        0        0     1469 2024-05-22 07:22:08.538864 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_doctors.html
+-rw-r--r--   0        0        0      772 2024-05-08 05:23:38.100357 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_faq.html
+-rw-r--r--   0        0        0      704 2024-05-09 04:50:22.638693 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_featured-services.html
+-rw-r--r--   0        0        0      684 2024-05-22 07:22:08.536885 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_features.html
+-rw-r--r--   0        0        0      728 2024-05-22 07:22:08.541512 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_gallery.html
+-rw-r--r--   0        0        0     1272 2024-05-22 07:22:08.534815 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_hero.html
+-rw-r--r--   0        0        0     1173 2024-05-09 00:34:34.141381 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_pricing.html
+-rw-r--r--   0        0        0      656 2024-05-17 04:33:21.960157 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_services.html
+-rw-r--r--   0        0        0     1046 2024-05-22 07:22:08.546232 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_testimonials.html
+-rwxr-xr-x   0        0        0      490 2024-05-23 00:55:55.332489 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/blog-details.html
+-rw-r--r--   0        0        0      376 2024-05-23 00:36:35.191410 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/breadcrumb.html
+-rw-r--r--   0        0        0     3139 2024-05-24 00:04:16.470708 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/footer.html
+-rwxr-xr-x   0        0        0     1579 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/forms/appointment.php
+-rwxr-xr-x   0        0        0     1341 2024-03-12 00:49:58.000000 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/forms/contact.php
+-rw-r--r--   0        0        0     2037 2024-05-22 07:22:08.529063 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/header.html
+-rwxr-xr-x   0        0        0     4614 2024-05-22 07:14:37.245804 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/index.html
+-rwxr-xr-x   0        0        0    16287 2024-05-23 00:41:03.798823 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/privacy.html
+-rw-r--r--   0        0        0     1933 2024-05-22 07:22:08.532372 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/seo.html
+-rwxr-xr-x   0        0        0    16327 2024-05-23 00:41:03.804529 django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/terms.html
+-rw-r--r--   0        0        0        0 2023-03-21 07:32:09.033136 django_medicio_dental-3.1.4/django_medicio_dental/templatetags/__init__.py
+-rw-r--r--   0        0        0     5988 2024-05-22 07:14:37.250671 django_medicio_dental-3.1.4/django_medicio_dental/templatetags/mediciodental_tags.py
+-rw-r--r--   0        0        0       60 2024-05-07 01:25:47.437462 django_medicio_dental-3.1.4/django_medicio_dental/tests.py
+-rw-r--r--   0        0        0      827 2024-05-22 07:09:45.998807 django_medicio_dental-3.1.4/django_medicio_dental/urls.py
+-rw-r--r--   0        0        0     4288 2024-05-22 23:59:16.822501 django_medicio_dental-3.1.4/django_medicio_dental/views.py
+-rw-r--r--   0        0        0      973 2024-05-24 00:05:34.243524 django_medicio_dental-3.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5644 1970-01-01 00:00:00.000000 django_medicio_dental-3.1.4/PKG-INFO
```

### Comparing `django_medicio_dental-3.1.3/LICENSE` & `django_medicio_dental-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/README.md` & `django_medicio_dental-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/forms.py` & `django_medicio_dental-3.1.4/django_medicio_dental/forms.py`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/migrations/0001_initial.py` & `django_medicio_dental-3.1.4/django_medicio_dental/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/migrations/0003_alter_post_content_alter_post_title.py` & `django_medicio_dental-3.1.4/django_medicio_dental/migrations/0003_alter_post_content_alter_post_title.py`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/migrations/0004_alter_post_content_alter_post_title.py` & `django_medicio_dental-3.1.4/django_medicio_dental/migrations/0004_alter_post_content_alter_post_title.py`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/models.py` & `django_medicio_dental-3.1.4/django_medicio_dental/models.py`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/sitemaps.py` & `django_medicio_dental-3.1.4/django_medicio_dental/sitemaps.py`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/css/style.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/css/style.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/js/main.js` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/js/main.js`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/scss/_footer.scss` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/scss/_footer.scss`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/scss/_general.scss` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/scss/_general.scss`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/scss/_header.scss` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/scss/_hero.scss` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/scss/_hero.scss`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/scss/_nav.scss` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/scss/_sections.scss` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/scss/_sections.scss`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/animate.css/animate.compat.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/animate.css/animate.compat.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/animate.css/animate.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/animate.css/animate.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/animate.css/animate.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/animate.css/animate.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/aos/aos.cjs.js` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/aos/aos.cjs.js`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/aos/aos.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/aos/aos.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/aos/aos.esm.js` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/aos/aos.esm.js`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/aos/aos.js` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/aos/aos.js`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/aos/aos.js.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/aos/aos.js.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/bootstrap-icons.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/bootstrap-icons.json` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/bootstrap-icons.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/bootstrap-icons.scss` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.css.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.min.css.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.rtl.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.rtl.css.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.css.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.min.css.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.rtl.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.css.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.min.css.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.rtl.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.css.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.min.css.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.rtl.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.rtl.css.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.rtl.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.rtl.min.css.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.bundle.js` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.bundle.js.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.bundle.min.js` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.bundle.min.js.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.esm.js` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.esm.js.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.esm.min.js` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.esm.min.js.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.js` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.js.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.min.js` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.min.js.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/boxicons/css/animations.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/boxicons/css/animations.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/boxicons/css/boxicons.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/boxicons/css/boxicons.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/boxicons/css/boxicons.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/boxicons/css/boxicons.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/boxicons/css/transformations.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/boxicons/css/transformations.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/boxicons/fonts/boxicons.eot` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/boxicons/fonts/boxicons.eot`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/boxicons/fonts/boxicons.svg` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/boxicons/fonts/boxicons.svg`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/boxicons/fonts/boxicons.ttf` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/boxicons/fonts/boxicons.ttf`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/boxicons/fonts/boxicons.woff` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/boxicons/fonts/boxicons.woff`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/boxicons/fonts/boxicons.woff2` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/boxicons/fonts/boxicons.woff2`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/all.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/all.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/all.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/all.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/brands.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/brands.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/brands.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/brands.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/fontawesome.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/fontawesome.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/regular.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/regular.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/regular.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/regular.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/solid.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/solid.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/solid.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/svg-with-js.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/svg-with-js.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/svg-with-js.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/svg-with-js.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v4-font-face.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v4-font-face.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v4-font-face.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v4-font-face.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v4-shims.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v4-shims.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v4-shims.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v4-shims.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v5-font-face.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v5-font-face.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v5-font-face.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/css/v5-font-face.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-brands-400.ttf` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-brands-400.woff2` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-regular-400.ttf` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-regular-400.woff2` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-solid-900.ttf` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-solid-900.woff2` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-v4compatibility.ttf` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-v4compatibility.woff2` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/fontawesome-free/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/glightbox/css/glightbox.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/glightbox/css/glightbox.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/glightbox/css/glightbox.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/glightbox/css/glightbox.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/glightbox/js/glightbox.js` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/glightbox/js/glightbox.js`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/glightbox/js/glightbox.min.js` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/glightbox/js/glightbox.min.js`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/php-email-form/php-email-form.php` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/php-email-form/php-email-form.php`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/php-email-form/validate.js` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/php-email-form/validate.js`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/purecounter/purecounter_vanilla.js` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/purecounter/purecounter_vanilla.js`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/purecounter/purecounter_vanilla.js.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/purecounter/purecounter_vanilla.js.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/swiper/swiper-bundle.min.css` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/swiper/swiper-bundle.min.css`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/swiper/swiper-bundle.min.js` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/swiper/swiper-bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/static/mediciodental/vendor/swiper/swiper-bundle.min.js.map` & `django_medicio_dental-3.1.4/django_medicio_dental/static/mediciodental/vendor/swiper/swiper-bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_about.html` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_about.html`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_appointment.html` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_appointment.html`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_contact.html` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_contact.html`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_counts.html` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_counts.html`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_cta.html` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_cta.html`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_departments.html` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_departments.html`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_doctors.html` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_doctors.html`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_faq.html` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_faq.html`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_featured-services.html` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_featured-services.html`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_features.html` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_features.html`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_gallery.html` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_gallery.html`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_hero.html` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_hero.html`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_pricing.html` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_pricing.html`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_services.html` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_services.html`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/_testimonials.html` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/_testimonials.html`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/footer.html` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/footer.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% load django_utilsds_tags %}
 
 <footer id="footer">
   <div class="footer-top">
     <div class="container">
       <div class="row">
 
-        <div class="col-md-6">
+        <div class="col-md-5">
           <div class="footer-info">
             <h3>{{ basic_info.company_name }}</h3>
             <p>
               {% autoescape off %}
               {{ basic_info.addr|add_br:"2" }}
               {% endautoescape %}
               <br><br>
@@ -43,15 +43,15 @@
             <li><i class="bx bx-chevron-right"></i> <a href="{% url template_name|add:':privacy' %}">개인정보처리방침</a></li>
             {% for title, link in footer_link.items %}
             <li><i class="bx bx-chevron-right"></i> <a href="{{ link }}" target="_blank">{{ title }}</a></li>
             {% endfor %}
           </ul>
         </div>
 
-        <div class="col-md-3 col-sm-6 footer-links">
+        <div class="col-md-4 col-sm-7 footer-links">
           <h4>Remarkable Posts</h4>
           <ul>
             {% for r in remarkables %}
             <li><i class="bx bx-chevron-right"></i> <a href="{% url template_name|add:':post_detail' r.slug %}">{{ r.title  | truncatechars:15}}</a></li>
             {% endfor %}
           </ul>
         </div>
```

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/forms/appointment.php` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/forms/appointment.php`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/forms/contact.php` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/forms/contact.php`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/header.html` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/header.html`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/index.html` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/index.html`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/privacy.html` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/privacy.html`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/seo.html` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/seo.html`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templates/mediciodental/terms.html` & `django_medicio_dental-3.1.4/django_medicio_dental/templates/mediciodental/terms.html`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/templatetags/mediciodental_tags.py` & `django_medicio_dental-3.1.4/django_medicio_dental/templatetags/mediciodental_tags.py`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/urls.py` & `django_medicio_dental-3.1.4/django_medicio_dental/urls.py`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/django_medicio_dental/views.py` & `django_medicio_dental-3.1.4/django_medicio_dental/views.py`

 * *Files identical despite different names*

### Comparing `django_medicio_dental-3.1.3/pyproject.toml` & `django_medicio_dental-3.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django_medicio_dental"
-version = "3.1.3"
+version = "3.1.4"
 description = "my demiansoft templates"
 authors = [{name = "Hyungjin Kim", email = "hj3415@gmail.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dependencies = [
     "Django >= 4.2.11",
```

### Comparing `django_medicio_dental-3.1.3/PKG-INFO` & `django_medicio_dental-3.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_medicio_dental
-Version: 3.1.3
+Version: 3.1.4
 Summary: my demiansoft templates
 Author-email: Hyungjin Kim <hj3415@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Django >= 4.2.11
 Requires-Dist: libsass>=0.23.0
 Requires-Dist: django-analyticsds >= 0.3.1
```


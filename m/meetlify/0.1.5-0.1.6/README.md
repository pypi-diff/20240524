# Comparing `tmp/meetlify-0.1.5.tar.gz` & `tmp/meetlify-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meetlify-0.1.5.tar", last modified: Mon May 20 21:32:15 2024, max compression
+gzip compressed data, was "meetlify-0.1.6.tar", last modified: Fri May 24 01:59:05 2024, max compression
```

## Comparing `meetlify-0.1.5.tar` & `meetlify-0.1.6.tar`

### file list

```diff
@@ -1,117 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.911187 meetlify-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-20 21:32:07.000000 meetlify-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 21:32:07.000000 meetlify-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-20 21:32:15.911187 meetlify-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-20 21:32:07.000000 meetlify-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-20 21:32:07.000000 meetlify-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-20 21:32:15.911187 meetlify-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-20 21:32:07.000000 meetlify-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.875187 meetlify-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.879187 meetlify-0.1.5/src/meetlify/
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/meetup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.883187 meetlify-0.1.5/src/meetlify/share/
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/configs.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.875187 meetlify-0.1.5/src/meetlify/share/content/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.883187 meetlify-0.1.5/src/meetlify/share/content/images/
--rw-r--r--   0 runner    (1001) docker     (127)   128599 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/content/images/fatureimage.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.883187 meetlify-0.1.5/src/meetlify/share/content/meetups/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/content/meetups/0001.md
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/content/meetups/0002.md
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/content/meetups/0003.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.883187 meetlify-0.1.5/src/meetlify/share/content/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/content/pages/contact.md
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/content/pages/home.md
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/content/pages/privacy.md
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/content/pages/terms.md
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/sitemap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.875187 meetlify-0.1.5/src/meetlify/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.879187 meetlify-0.1.5/src/meetlify/themes/lindau/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.879187 meetlify-0.1.5/src/meetlify/themes/lindau/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.887187 meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   362926 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/about.png
--rw-r--r--   0 runner    (1001) docker     (127)    50969 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/author.png
--rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/banner.png
--rw-r--r--   0 runner    (1001) docker     (127)    22993 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.899187 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    70329 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.css
--rw-r--r--   0 runner    (1001) docker     (127)   203221 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    51795 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   115986 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    70403 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   203225 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    51870 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   116063 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    65696 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css
--rw-r--r--   0 runner    (1001) docker     (127)   129371 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    51369 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   129386 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    63943 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   107823 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css
--rw-r--r--   0 runner    (1001) docker     (127)   267535 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    85352 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   180381 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   107691 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   267476 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    85281 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   180217 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   281046 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   679755 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   232803 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   589892 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   280259 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   679615 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   232911 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   589087 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/cookiealert.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.899187 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   113656 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)    85044 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   238502 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.907187 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)   207819 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)   444579 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    80721 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   332090 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   135829 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.esm.js
--rw-r--r--   0 runner    (1001) docker     (127)   305438 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    73935 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   222455 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   145401 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)   306606 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    60635 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   220561 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/cookiealert.js
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/scripts.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.907187 meetlify-0.1.5/src/meetlify/themes/lindau/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/templates/meetup.html
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/templates/meetups.html
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/templates/page.html
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/templates/sitemap-index.xml
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/templates/sitemap.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.907187 meetlify-0.1.5/src/meetlify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-20 21:32:15.000000 meetlify-0.1.5/src/meetlify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-20 21:32:15.000000 meetlify-0.1.5/src/meetlify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:32:15.000000 meetlify-0.1.5/src/meetlify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-20 21:32:15.000000 meetlify-0.1.5/src/meetlify.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:32:15.000000 meetlify-0.1.5/src/meetlify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-20 21:32:15.000000 meetlify-0.1.5/src/meetlify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 21:32:15.000000 meetlify-0.1.5/src/meetlify.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.907187 meetlify-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-20 21:32:07.000000 meetlify-0.1.5/tests/test_meetups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.823558 meetlify-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-24 01:58:58.000000 meetlify-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-24 01:58:58.000000 meetlify-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-24 01:59:05.823558 meetlify-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-24 01:58:58.000000 meetlify-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-24 01:58:58.000000 meetlify-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-24 01:59:05.823558 meetlify-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-24 01:58:58.000000 meetlify-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.791558 meetlify-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.795558 meetlify-0.1.6/src/meetlify/
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/meetup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/post.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.795558 meetlify-0.1.6/src/meetlify/share/
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/configs.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.791558 meetlify-0.1.6/src/meetlify/share/content/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.795558 meetlify-0.1.6/src/meetlify/share/content/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   128599 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/content/images/fatureimage.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.795558 meetlify-0.1.6/src/meetlify/share/content/meetups/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/content/meetups/0001.md
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/content/meetups/0002.md
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/content/meetups/0003.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.799558 meetlify-0.1.6/src/meetlify/share/content/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/content/pages/contact.md
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/content/pages/home.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/content/pages/privacy.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/content/pages/terms.md
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/sitemap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.791558 meetlify-0.1.6/src/meetlify/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.791558 meetlify-0.1.6/src/meetlify/themes/lindau/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.791558 meetlify-0.1.6/src/meetlify/themes/lindau/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.799558 meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   362926 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/about.png
+-rw-r--r--   0 runner    (1001) docker     (127)    50969 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/author.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22993 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.811558 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    70329 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.css
+-rw-r--r--   0 runner    (1001) docker     (127)   203221 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    51795 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   115986 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    70403 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   203225 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    51870 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   116063 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    65696 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css
+-rw-r--r--   0 runner    (1001) docker     (127)   129371 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    51369 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   129386 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    63943 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   107823 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css
+-rw-r--r--   0 runner    (1001) docker     (127)   267535 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    85352 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   180381 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   107691 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   267476 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    85281 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   180217 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   281046 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)   679755 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   232803 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   589892 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   280259 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   679615 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   232911 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   589087 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/cookiealert.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.811558 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   113656 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    85044 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   238502 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.819558 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   207819 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)   444579 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    80721 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   332090 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   135829 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.esm.js
+-rw-r--r--   0 runner    (1001) docker     (127)   305438 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    73935 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   222455 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   145401 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)   306606 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    60635 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   220561 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/cookiealert.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/scripts.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.819558 meetlify-0.1.6/src/meetlify/themes/lindau/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/templates/meetup.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/templates/meetups.html
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/templates/sitemap-index.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/templates/sitemap.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.819558 meetlify-0.1.6/src/meetlify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-24 01:59:05.000000 meetlify-0.1.6/src/meetlify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-05-24 01:59:05.000000 meetlify-0.1.6/src/meetlify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 01:59:05.000000 meetlify-0.1.6/src/meetlify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-24 01:59:05.000000 meetlify-0.1.6/src/meetlify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 01:59:05.000000 meetlify-0.1.6/src/meetlify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-24 01:59:05.000000 meetlify-0.1.6/src/meetlify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 01:59:05.000000 meetlify-0.1.6/src/meetlify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.819558 meetlify-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-24 01:58:58.000000 meetlify-0.1.6/tests/test_meetups.py
```

### Comparing `meetlify-0.1.5/LICENSE` & `meetlify-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/PKG-INFO` & `meetlify-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: meetlify
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python Package to Generate Meetup Websites
 Home-page: https://github.com/pybodensee/meetlify
-Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.5.tar.gz
+Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.6.tar.gz
 Author: Faisal Shahzad
 Author-email: pybodensee@gmail.com
 License: MIT
 Keywords: meetups,static-site-generators,seo,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications
@@ -54,25 +54,25 @@
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: pymdown-extensions; extra == "dev"
 Provides-Extra: all
+Requires-Dist: mkdocs-gen-files; extra == "all"
+Requires-Dist: python-language-server[all]; extra == "all"
+Requires-Dist: mkdocstrings[python]; extra == "all"
 Requires-Dist: pytest; extra == "all"
-Requires-Dist: wheel; extra == "all"
+Requires-Dist: pymdown-extensions; extra == "all"
 Requires-Dist: black; extra == "all"
-Requires-Dist: mkdocstrings[python]; extra == "all"
 Requires-Dist: pytest-cov; extra == "all"
-Requires-Dist: pymdown-extensions; extra == "all"
 Requires-Dist: mkdocs; extra == "all"
-Requires-Dist: python-language-server[all]; extra == "all"
-Requires-Dist: mkdocs-gen-files; extra == "all"
-Requires-Dist: setuptools; extra == "all"
 Requires-Dist: twine; extra == "all"
+Requires-Dist: setuptools; extra == "all"
+Requires-Dist: wheel; extra == "all"
 
 # meetlify
 
 Python based Static Site Genrators for Meetups/Meetup Webites.
 
 [![license](https://img.shields.io/pypi/l/meetlify.svg?style=flat-square "Project License: MIT")](https://github.com/pybodensee/meetlify/blob/master/LICENSE)
 [![status](https://img.shields.io/pypi/status/meetlify.svg?style=flat-square "Project Development Status")](https://github.com/pybodensee/meetlify/milestone/1)
```

### Comparing `meetlify-0.1.5/README.md` & `meetlify-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/setup.py` & `meetlify-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/__init__.py` & `meetlify-0.1.6/src/meetlify/__init__.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/api.py` & `meetlify-0.1.6/src/meetlify/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # INTERNAL IMPORTS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 from .configs import Configs
+from .post import Post
 from .page import Page
 from .meetup import Meetup
 from .sitemap import Sitemap
 from .constants import STATUS
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # IMPLEMENATIONS
@@ -76,14 +77,15 @@
 
         self.renderer = Environment(
             loader=FileSystemLoader(
                 Path(self.dest, "themes", self.configs.theme, "templates")
             )
         )
         self.meetups = []
+        self.posts = []
         self.pages = []
         self.sitemaps = []
 
     def setup(self) -> None:
         """Setup Current Folder for Meetlify Website."""
 
         Path(self.dest, self.configs.folders.output).mkdir(parents=True, exist_ok=True)
@@ -122,15 +124,15 @@
             Meetup.from_markdown(mt)
             for mt in Path(self.dest, self.configs.folders.content, "meetups").iterdir()
             if mt.is_file() and mt.suffix == ".md"
         ]
         self.meetups = [
             mt
             for mt in self.meetups
-            if mt.status in [STATUS.PROGRESS.value, STATUS.DONE.value]
+            if mt.status in [STATUS.PUBLISHED.value, STATUS.DONE.value]
         ]
         self.meetups = sorted(self.meetups, key=lambda x: x.id, reverse=True)
 
         self.sitemaps.append(
             Sitemap.from_dict(
                 {
                     "name": "meetups",
@@ -157,14 +159,34 @@
                     "slug": "/",
                     "modifieddate": datetime.now(),
                     "items": self.pages,
                 }
             )
         )
 
+    def parse_posts(self):
+        """Parse Posts avaialable as Markdown"""
+
+        self.posts = [
+            Post.from_markdown(mt)
+            for mt in Path(self.dest, self.configs.folders.content, "posts").iterdir()
+            if mt.is_file() and mt.suffix == ".md"
+        ]
+
+        self.sitemaps.append(
+            Sitemap.from_dict(
+                {
+                    "name": "posts",
+                    "slug": "/",
+                    "modifieddate": datetime.now(),
+                    "items": self.posts,
+                }
+            )
+        )
+
     def render_home(self):
         """Render home page"""
         with codecs.open(
             Path(
                 self.dest,
                 self.configs.folders.content,
                 self.configs.folders.pages,
@@ -184,14 +206,15 @@
             encoding="utf-8",
         ) as file:
             file.write(
                 self.renderer.get_template("index.html").render(
                     meta=self.configs,
                     home_content="".join(home_content),
                     meetups=self.meetups[0:3],
+                    posts=self.posts[0:3],
                 )
             )
             print("... wrote output/home")
 
         with open(
             Path(self.dest, self.configs.folders.output, "404.html"),
             mode="w",
@@ -285,29 +308,78 @@
                 file.write(
                     self.renderer.get_template("meetup.html").render(
                         meta=self.configs,
                         content=_meetup.content,
                         front=_meetup,
                     )
                 )
-                print(f"... wrote output/meetups/{_meetup.slug}")
+                print(f"...... wrote output/meetups/{_meetup.slug}")
 
         # save meetup index page
         with open(
             Path(self.dest, self.configs.folders.output, "meetups", "index.html"),
             mode="w",
             encoding="utf-8",
         ) as file:
             file.write(
                 self.renderer.get_template("meetups.html").render(
                     meta=self.configs, meetups=self.meetups
                 )
             )
             print("... wrote output/meetups")
 
+    def render_posts(self):
+        """Render posts and Meetup index page"""
+
+        # TODO: Check if there are less than 3 meetups and runs without error? make 3 config variable
+        for _post in self.posts:
+            Path(self.dest, self.configs.folders.output, "posts", _post.slug).mkdir(
+                parents=True, exist_ok=True
+            )
+
+            _admonition = {
+                "type": "hint",
+                "title": "Update",
+                "message": "This is work in progress. Please checkback later for an updated version of this post.",
+            }
+
+            with open(
+                Path(
+                    self.dest,
+                    self.configs.folders.output,
+                    "posts",
+                    _post.slug,
+                    "index.html",
+                ),
+                mode="w",
+                encoding="utf-8",
+            ) as file:
+                file.write(
+                    self.renderer.get_template("post.html").render(
+                        meta=self.configs,
+                        content=_post.content,
+                        front=_post,
+                        admonition=_admonition,
+                    )
+                )
+                print(f"...... wrote output/posts/{_post.slug}")
+
+        # save meetup index page
+        with open(
+            Path(self.dest, self.configs.folders.output, "posts", "index.html"),
+            mode="w",
+            encoding="utf-8",
+        ) as file:
+            file.write(
+                self.renderer.get_template("posts.html").render(
+                    meta=self.configs, posts=self.posts
+                )
+            )
+            print("... wrote output/posts")
+
     def copy_assests(self):
         """Copy Assets e.g. Static Folders, Images, Feeds, and Sitemaps"""
 
         # copy static folders
         shutil.copytree(
             Path(self.dest, "themes", self.configs.theme, "static"),
             Path(
@@ -344,12 +416,14 @@
             print("... copied output/robots.txt filed")
 
     def make(self):
         """Make Static Site and Save to Output folder"""
 
         self.parse_meetups()
         self.parse_pages()
+        self.parse_posts()
         self.render_home()
         self.render_meetups()
+        self.render_posts()
         self.render_pages()
         self.render_sitemaps()
         self.copy_assests()
```

### Comparing `meetlify-0.1.5/src/meetlify/cli.py` & `meetlify-0.1.6/src/meetlify/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,17 +82,18 @@
     Meetlify(dest_=Path(os.getcwd())).clean()
 
 
 @main.command("make", help="Make Current Project")
 @click.option("--meetups/--no-meetups", default=False)
 @click.option("--home/--no-home", default=False)
 @click.option("--pages/--no-pages", default=False)
+@click.option("--posts/--no-posts", default=False)
 @click.option("--assets/--no-assets", default=False)
 @click.option("--sitemap/--no-sitemap", default=False)
-def make(meetups, home, pages, assets, sitemap):
+def make(meetups, home, pages, posts, assets, sitemap):
     click.echo("Make Current Project")
     _mlfy = Meetlify(dest_=Path(os.getcwd()))
 
     if meetups:
         _mlfy.parse_meetups()
         _mlfy.render_meetups()
 
@@ -100,17 +101,21 @@
         _mlfy.parse_meetups()
         _mlfy.render_home()
 
     if pages:
         _mlfy.parse_pages()
         _mlfy.render_pages()
 
+    if posts:
+        _mlfy.parse_posts()
+        # _mlfy.render_()
+
     if assets:
         _mlfy.copy_assests()
 
     if sitemap:
         _mlfy.parse_meetups()
         _mlfy.parse_pages()
         _mlfy.render_sitemaps()
 
-    if not any([meetups, home, pages, assets, sitemap]):
+    if not any([meetups, home, pages, posts, assets, sitemap]):
         _mlfy.make()
```

### Comparing `meetlify-0.1.5/src/meetlify/configs.py` & `meetlify-0.1.6/src/meetlify/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 class Folders:
     """Folder data class for differnt types of folder used in Processing"""
 
     output: str
     content: str
     meetups: str
     pages: str
+    posts: str
 
 
 @dataclass
 class Configs:
     """Config Data Class to hold Project Configurations"""
 
     name: str
```

### Comparing `meetlify-0.1.5/src/meetlify/constants.py` & `meetlify-0.1.6/src/meetlify/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # DATABASE/CONSTANTS LIST
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 VERSION_MAJOR = 0
 VERSION_MINOR = 1
-VERSION_REVISION = 5
+VERSION_REVISION = 6
 
 FULL_VERSION = f"{VERSION_MAJOR}.{VERSION_MINOR}.{VERSION_REVISION}"
 
 
 class ExtendedEnum(Enum):
     """An extended enum class to convert list of items in an enumration."""
 
@@ -57,9 +57,17 @@
 
 
 class STATUS(ExtendedEnum):
     """An enum for the different Hostings."""
 
     DRAFT = "draft"
     PLANNING = "planning"
-    PROGRESS = "progress"
+    PUBLISHED = "published"
     DONE = "done"
+
+
+class ADMONITION(ExtendedEnum):
+    """An enum for the different Admonitions."""
+
+    DRAFT = "draft"
+    INCOMPLETE = "incomplete"
+    COMPLETE = "complete"
```

### Comparing `meetlify-0.1.5/src/meetlify/meetup.py` & `meetlify-0.1.6/src/meetlify/meetup.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,22 +34,28 @@
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # STANDARD LIBARY IMPORTS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 import codecs
 from dataclasses import dataclass
 from pathlib import Path
-from datetime import datetime, timezone 
+from datetime import datetime, timezone
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # 3rd PARTY LIBRARY IMPORTS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 import markdown
-from slugify import slugify
+
+
+# +++++++++++++++++++++++++++++++++++++++++++++++++++++
+# INTERNAL IMPORTS
+# +++++++++++++++++++++++++++++++++++++++++++++++++++++
+
+from .utils import get_slug
 
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # IMPLEMENATIONS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 
@@ -80,29 +86,24 @@
             Meetup: Return Constructed Meetup Object
         """
         _md = markdown.Markdown(extensions=["meta", "attr_list"])
         with codecs.open(meetup_, "r", encoding="utf-8") as f:
             data = f.read()
             content_ = _md.convert(data)
 
-            slug_ = (
-                "".join(_md.Meta["slug"])
-                if _md.Meta.get("slug")
-                else slugify("".join(_md.Meta["title"]))
-            )
-
-
             return cls(
                 content=content_,
                 id="".join(_md.Meta["id"]),
                 date="".join(_md.Meta["date"]),
                 modifieddate=datetime.fromtimestamp(
                     Path(meetup_).stat().st_mtime, tz=timezone.utc
                 ),
                 author="".join(_md.Meta["author"]),
                 title="".join(_md.Meta["title"]),
                 description="".join(_md.Meta["description"]),
-                slug=slug_,
+                slug=get_slug(
+                    _md.Meta["slug"] if "slug" in _md.Meta else [""], _md.Meta["title"]
+                ),
                 featureimage="".join(_md.Meta["featureimage"]),
                 address="".join(_md.Meta["address"]),
                 status="".join(_md.Meta["status"]),
             )
```

### Comparing `meetlify-0.1.5/src/meetlify/page.py` & `meetlify-0.1.6/src/meetlify/page.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/share/__init__.py` & `meetlify-0.1.6/src/meetlify/share/__init__.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/share/configs.json` & `meetlify-0.1.6/src/meetlify/share/configs.json`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/share/content/images/fatureimage.png` & `meetlify-0.1.6/src/meetlify/share/content/images/fatureimage.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/share/content/meetups/0001.md` & `meetlify-0.1.6/src/meetlify/share/content/meetups/0001.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/share/content/meetups/0002.md` & `meetlify-0.1.6/src/meetlify/share/content/meetups/0002.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/share/content/meetups/0003.md` & `meetlify-0.1.6/src/meetlify/share/content/meetups/0003.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/share/content/pages/contact.md` & `meetlify-0.1.6/src/meetlify/share/content/pages/contact.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/share/content/pages/home.md` & `meetlify-0.1.6/src/meetlify/share/content/pages/home.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/share/content/pages/privacy.md` & `meetlify-0.1.6/src/meetlify/share/content/pages/privacy.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/share/content/pages/terms.md` & `meetlify-0.1.6/src/meetlify/share/content/pages/terms.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/sitemap.py` & `meetlify-0.1.6/src/meetlify/sitemap.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/about.png` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/about.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/author.png` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/author.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/banner.png` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/banner.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/favicon.png` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/logo.png` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/logo.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.css` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-icons.css` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.css` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.css.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.min.css` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/styles.css` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/styles.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.esm.js` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.js` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.js.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.min.js` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/cookiealert.js` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/cookiealert.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/scripts.js` & `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/scripts.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/templates/404.html` & `meetlify-0.1.6/src/meetlify/themes/lindau/templates/404.html`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/templates/base.html` & `meetlify-0.1.6/src/meetlify/themes/lindau/templates/base.html`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/templates/index.html` & `meetlify-0.1.6/src/meetlify/themes/lindau/templates/index.html`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/templates/meetup.html` & `meetlify-0.1.6/src/meetlify/themes/lindau/templates/meetup.html`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/templates/meetups.html` & `meetlify-0.1.6/src/meetlify/themes/lindau/templates/meetups.html`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/themes/lindau/templates/page.html` & `meetlify-0.1.6/src/meetlify/themes/lindau/templates/page.html`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.5/src/meetlify/utils.py` & `meetlify-0.1.6/src/meetlify/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,14 +35,21 @@
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 from pathlib import Path
 import shutil
 
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
+# 3rd PARTY LIBRARY IMPORTS
+# +++++++++++++++++++++++++++++++++++++++++++++++++++++
+
+from slugify import slugify
+
+
+# +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # IMPLEMENATIONS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 
 def initialize(dest_: Path) -> None:
     """Intialze Meetlify Website
 
@@ -52,7 +59,15 @@
     assert isinstance(dest_, Path)
     assert dest_.exists()
 
     shutil.copyfile(
         Path(Path(__file__).resolve().parent, "share", "configs.json"),
         Path(dest_, "configs.json"),
     )
+
+
+def get_slug(slug_, title_):
+    # slug_ = "".join(_md.Meta["slug"])
+    # slug_ = slugify("".join(_md.Meta["title"])) if not slug_ else slug_
+
+    slug_ = "".join(slug_)
+    return slugify("".join(title_)) if not slug_ else slug_
```

### Comparing `meetlify-0.1.5/src/meetlify.egg-info/PKG-INFO` & `meetlify-0.1.6/src/meetlify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: meetlify
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python Package to Generate Meetup Websites
 Home-page: https://github.com/pybodensee/meetlify
-Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.5.tar.gz
+Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.6.tar.gz
 Author: Faisal Shahzad
 Author-email: pybodensee@gmail.com
 License: MIT
 Keywords: meetups,static-site-generators,seo,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications
@@ -54,25 +54,25 @@
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: pymdown-extensions; extra == "dev"
 Provides-Extra: all
+Requires-Dist: mkdocs-gen-files; extra == "all"
+Requires-Dist: python-language-server[all]; extra == "all"
+Requires-Dist: mkdocstrings[python]; extra == "all"
 Requires-Dist: pytest; extra == "all"
-Requires-Dist: wheel; extra == "all"
+Requires-Dist: pymdown-extensions; extra == "all"
 Requires-Dist: black; extra == "all"
-Requires-Dist: mkdocstrings[python]; extra == "all"
 Requires-Dist: pytest-cov; extra == "all"
-Requires-Dist: pymdown-extensions; extra == "all"
 Requires-Dist: mkdocs; extra == "all"
-Requires-Dist: python-language-server[all]; extra == "all"
-Requires-Dist: mkdocs-gen-files; extra == "all"
-Requires-Dist: setuptools; extra == "all"
 Requires-Dist: twine; extra == "all"
+Requires-Dist: setuptools; extra == "all"
+Requires-Dist: wheel; extra == "all"
 
 # meetlify
 
 Python based Static Site Genrators for Meetups/Meetup Webites.
 
 [![license](https://img.shields.io/pypi/l/meetlify.svg?style=flat-square "Project License: MIT")](https://github.com/pybodensee/meetlify/blob/master/LICENSE)
 [![status](https://img.shields.io/pypi/status/meetlify.svg?style=flat-square "Project Development Status")](https://github.com/pybodensee/meetlify/milestone/1)
```

### Comparing `meetlify-0.1.5/src/meetlify.egg-info/SOURCES.txt` & `meetlify-0.1.6/src/meetlify.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/meetlify/__init__.py
 src/meetlify/api.py
 src/meetlify/cli.py
 src/meetlify/configs.py
 src/meetlify/constants.py
 src/meetlify/meetup.py
 src/meetlify/page.py
+src/meetlify/post.py
 src/meetlify/sitemap.py
 src/meetlify/utils.py
 src/meetlify.egg-info/PKG-INFO
 src/meetlify.egg-info/SOURCES.txt
 src/meetlify.egg-info/dependency_links.txt
 src/meetlify.egg-info/entry_points.txt
 src/meetlify.egg-info/not-zip-safe
```

### Comparing `meetlify-0.1.5/tests/test_meetups.py` & `meetlify-0.1.6/tests/test_meetups.py`

 * *Files identical despite different names*


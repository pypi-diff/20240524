# Comparing `tmp/seamm-dashboard-2024.3.27.tar.gz` & `tmp/seamm_dashboard-2024.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seamm-dashboard-2024.3.27.tar", last modified: Wed Mar 27 20:06:27 2024, max compression
+gzip compressed data, was "seamm_dashboard-2024.5.24.tar", last modified: Fri May 24 17:14:13 2024, max compression
```

## Comparing `seamm-dashboard-2024.3.27.tar` & `seamm_dashboard-2024.5.24.tar`

### file list

```diff
@@ -1,294 +1,294 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.385839 seamm-dashboard-2024.3.27/
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-03-27 20:06:27.385839 seamm-dashboard-2024.3.27/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     4850 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/requirements_dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.385839 seamm-dashboard-2024.3.27/seamm_dashboard/
--rwxr-xr-x   0 runner    (1001) docker     (127)     8236 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-27 20:06:27.385839 seamm-dashboard-2024.3.27/seamm_dashboard/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2120 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/flask_authorize_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/jwt_patch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      498 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/results_dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.333839 seamm-dashboard-2024.3.27/seamm_dashboard/routes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.345839 seamm-dashboard-2024.3.27/seamm_dashboard/routes/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/admin/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)    17344 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/admin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.345839 seamm-dashboard-2024.3.27/seamm_dashboard/routes/api/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/api/flowcharts.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/api/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/api/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/api/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/api/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/api/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/api/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.345839 seamm-dashboard-2024.3.27/seamm_dashboard/routes/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/auth/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/auth/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.349839 seamm-dashboard-2024.3.27/seamm_dashboard/routes/flowcharts/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/flowcharts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/flowcharts/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.349839 seamm-dashboard-2024.3.27/seamm_dashboard/routes/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/jobs/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)    18322 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/jobs/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.349839 seamm-dashboard-2024.3.27/seamm_dashboard/routes/main/
--rwxr-xr-x   0 runner    (1001) docker     (127)      255 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/main/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/main/forms.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1209 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/main/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.349839 seamm-dashboard-2024.3.27/seamm_dashboard/routes/projects/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/projects/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8429 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/routes/projects/views.py
--rw-r--r--   0 runner    (1001) docker     (127)    21003 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/setup_argparsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/setup_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.349839 seamm-dashboard-2024.3.27/seamm_dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.353839 seamm-dashboard-2024.3.27/seamm_dashboard/static/css/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6653 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/css/bootstrap-select.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    29130 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/css/custom_flowchart.css
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/css/jobs_list.css
--rw-r--r--   0 runner    (1001) docker     (127)     6502 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/css/prism.css
--rw-r--r--   0 runner    (1001) docker     (127)   281191 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/css/style.css
--rw-r--r--   0 runner    (1001) docker     (127)   647497 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/css/style.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   232121 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/css/style.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   876516 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/css/style.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.353839 seamm-dashboard-2024.3.27/seamm_dashboard/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)    12238 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/images/Banner_AllCaps.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    26358 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/images/MolSSI-Logo-xl.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/images/briefcase.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/images/molssi-favicon-inverted.svg
--rw-r--r--   0 runner    (1001) docker     (127)    16562 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/images/molssi-favicon.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/images/object-group.svg
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/images/project-diagram.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.353839 seamm-dashboard-2024.3.27/seamm_dashboard/static/img/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.357839 seamm-dashboard-2024.3.27/seamm_dashboard/static/img/avatars/
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/img/avatars/1.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/img/avatars/2.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/img/avatars/3.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/img/avatars/4.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    19058 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/img/avatars/5.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/img/avatars/6.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/img/avatars/7.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    20466 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/img/avatars/8.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.357839 seamm-dashboard-2024.3.27/seamm_dashboard/static/img/brand/
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/img/brand/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/img/brand/sygnet.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/img/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.361839 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/buildings.js
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/collapsible.js
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/colors.js
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/flowchart_list.js
--rw-r--r--   0 runner    (1001) docker     (127)    19705 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/job_report.js
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/jobs_list.js
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/login.js
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/logout.js
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/main.js
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/manage_groups.js
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/manage_user.js
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/manage_users.js
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/popovers.js
--rw-r--r--   0 runner    (1001) docker     (127)    32221 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/prism.js
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/project_list.js
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/render_flowchart.js
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/setup.js
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/table_api.js
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/timer.js
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/tooltips.js
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/util.js
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/js/widgets.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.337839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.333839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/@coreui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.333839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/@coreui/coreui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.333839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/@coreui/coreui/dist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.361839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/@coreui/coreui/dist/js/
--rw-r--r--   0 runner    (1001) docker     (127)    31892 2024-03-27 20:05:15.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/@coreui/coreui/dist/js/coreui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.333839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/@fortawesome/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.333839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/@fortawesome/fontawesome-free/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.361839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/@fortawesome/fontawesome-free/js/
--rw-r--r--   0 runner    (1001) docker     (127)  1196706 2024-03-27 20:05:16.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/@fortawesome/fontawesome-free/js/all.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.337839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.337839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/bootstrap/dist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.361839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/bootstrap/dist/js/
--rw-r--r--   0 runner    (1001) docker     (127)    62563 2024-03-27 20:05:15.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/bootstrap/dist/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.337839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/cytoscape/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.361839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/cytoscape/dist/
--rw-r--r--   0 runner    (1001) docker     (127)   365827 2024-03-27 20:05:16.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/cytoscape/dist/cytoscape.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.337839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.365839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net/js/
--rw-r--r--   0 runner    (1001) docker     (127)    87278 2024-03-27 20:05:15.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net/js/jquery.dataTables.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.337839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-bs4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.361839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-bs4/css/
--rw-r--r--   0 runner    (1001) docker     (127)    11663 2024-03-27 20:05:15.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-bs4/css/dataTables.bootstrap4.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.361839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-bs4/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-03-27 20:05:15.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-bs4/js/dataTables.bootstrap4.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.337839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-buttons/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.361839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-buttons/js/
--rw-r--r--   0 runner    (1001) docker     (127)    19994 2024-03-27 20:05:15.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-buttons/js/dataTables.buttons.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.337839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-buttons-bs4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.361839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-buttons-bs4/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-03-27 20:05:15.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-buttons-bs4/css/buttons.bootstrap4.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.337839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-dt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.365839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-dt/js/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-27 20:05:15.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-dt/js/dataTables.dataTables.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.337839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-select/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.365839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-select/js/
--rw-r--r--   0 runner    (1001) docker     (127)    14277 2024-03-27 20:05:15.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-select/js/dataTables.select.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.337839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-select-dt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.365839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-select-dt/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-03-27 20:05:15.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-select-dt/css/select.dataTables.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.337839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.365839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/jquery/dist/
--rw-r--r--   0 runner    (1001) docker     (127)    87533 2024-03-27 20:05:15.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/jquery/dist/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.337839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/jquery-csv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.365839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/jquery-csv/src/
--rw-r--r--   0 runner    (1001) docker     (127)     9302 2024-03-27 20:05:15.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/jquery-csv/src/jquery.csv.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.337839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/jstree/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.365839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/jstree/dist/
--rw-r--r--   0 runner    (1001) docker     (127)   141969 2024-03-27 20:05:15.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/jstree/dist/jstree.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.337839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/jstree/dist/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.365839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/jstree/dist/themes/default/
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-03-27 20:05:15.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/jstree/dist/themes/default/32px.png
--rw-r--r--   0 runner    (1001) docker     (127)    31730 2024-03-27 20:05:15.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/jstree/dist/themes/default/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-03-27 20:05:15.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/jstree/dist/themes/default/throbber.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.337839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/ngl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.365839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/ngl/dist/
--rw-r--r--   0 runner    (1001) docker     (127)  1120787 2024-03-27 20:05:16.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/ngl/dist/ngl.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.365839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/pace-progress/
--rw-r--r--   0 runner    (1001) docker     (127)    12507 2024-03-27 20:05:15.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/pace-progress/pace.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.337839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/perfect-scrollbar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.365839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/perfect-scrollbar/dist/
--rw-r--r--   0 runner    (1001) docker     (127)    19549 2024-03-27 20:05:15.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/perfect-scrollbar/dist/perfect-scrollbar.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.365839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/plotly.js-dist-min/
--rw-r--r--   0 runner    (1001) docker     (127)  3478174 2024-03-27 20:05:15.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/plotly.js-dist-min/plotly.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.337839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/popper.js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.337839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/popper.js/dist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.373839 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/popper.js/dist/umd/
--rw-r--r--   0 runner    (1001) docker     (127)    21233 2024-03-27 20:05:15.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/popper.js/dist/umd/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/only_needed_files.py
--rw-r--r--   0 runner    (1001) docker     (127)   103040 2024-03-27 20:05:39.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.373839 seamm-dashboard-2024.3.27/seamm_dashboard/static/tmp/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/static/tmp/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    22082 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/swagger.yml
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/template_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.373839 seamm-dashboard-2024.3.27/seamm_dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/401.html
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/500.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.373839 seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/change_email.html
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/change_password.html
--rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/create_group.html
--rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/create_user.html
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/delete_group.html
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/delete_user.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.377839 seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/email/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/email/change_email.html
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/email/change_email.txt
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/email/confirm.html
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/email/confirm.txt
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/email/reset_password.html
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/email/reset_password.txt
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/login.html
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/manage_groups.html
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/manage_users.html
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/register.html
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/reset_password.html
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/unconfirmed.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.377839 seamm-dashboard-2024.3.27/seamm_dashboard/templates/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/auth/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/auth/confirm_login.html
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/auth/login.html
--rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/auth/manage_account.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.377839 seamm-dashboard-2024.3.27/seamm_dashboard/templates/flowcharts/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/flowcharts/flowchart_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/flowcharts/render_flowchart.html
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    31853 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/index_full.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.377839 seamm-dashboard-2024.3.27/seamm_dashboard/templates/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/jobs/edit_job.html
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/jobs/import_job.html
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/jobs/job_parameters.html
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/jobs/job_report.html
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/jobs/jobs_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/jobs/submit_job.html
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/login_coreui.html
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/login_script.html
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/logout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.377839 seamm-dashboard-2024.3.27/seamm_dashboard/templates/projects/
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/projects/project_access.html
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/projects/project_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/register.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.377839 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.381839 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/breadcrumb.html
--rw-r--r--   0 runner    (1001) docker     (127)    41683 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/card.html
--rw-r--r--   0 runner    (1001) docker     (127)    17627 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/cards.html
--rw-r--r--   0 runner    (1001) docker     (127)    16183 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/carousel.html
--rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/collapse.html
--rw-r--r--   0 runner    (1001) docker     (127)    47501 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/forms.html
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/jumbotron.html
--rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/list-group.html
--rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/navbar.html
--rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/navs.html
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/pagination.html
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/popovers.html
--rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/progress.html
--rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/scrollspy.html
--rw-r--r--   0 runner    (1001) docker     (127)    40822 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/switches.html
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/tables.html
--rw-r--r--   0 runner    (1001) docker     (127)     9781 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/tabs.html
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/tooltips.html
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/blank.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.381839 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)    41831 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/buttons/brand-buttons.html
--rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/buttons/button-group.html
--rw-r--r--   0 runner    (1001) docker     (127)    27328 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/buttons/buttons.html
--rw-r--r--   0 runner    (1001) docker     (127)    21346 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/buttons/dropdowns.html
--rw-r--r--   0 runner    (1001) docker     (127)    38782 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/buttons/social-buttons.html
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/charts.html
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/colors.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.385839 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/icons/
--rw-r--r--   0 runner    (1001) docker     (127)    44734 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/icons/flags.html
--rw-r--r--   0 runner    (1001) docker     (127)   141248 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/icons/font-awesome.html
--rw-r--r--   0 runner    (1001) docker     (127)    26687 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/icons/simple-line-icons.html
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/login.html
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/main.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.385839 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/notifications/alerts.html
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/notifications/badge.html
--rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/notifications/modals.html
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/typography.html
--rw-r--r--   0 runner    (1001) docker     (127)    32244 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/widgets.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.385839 seamm-dashboard-2024.3.27/seamm_dashboard/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/tests/test_api_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/tests/test_api_authenticated.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/tests/test_api_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15489 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/seamm_dashboard/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:06:27.385839 seamm-dashboard-2024.3.27/seamm_dashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-03-27 20:06:27.000000 seamm-dashboard-2024.3.27/seamm_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-03-27 20:06:27.000000 seamm-dashboard-2024.3.27/seamm_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 20:06:27.000000 seamm-dashboard-2024.3.27/seamm_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-27 20:06:27.000000 seamm-dashboard-2024.3.27/seamm_dashboard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 20:05:40.000000 seamm-dashboard-2024.3.27/seamm_dashboard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-27 20:06:27.000000 seamm-dashboard-2024.3.27/seamm_dashboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-27 20:06:27.000000 seamm-dashboard-2024.3.27/seamm_dashboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-27 20:06:27.385839 seamm-dashboard-2024.3.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-03-27 20:04:13.000000 seamm-dashboard-2024.3.27/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.349808 seamm_dashboard-2024.5.24/
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-05-24 17:14:13.349808 seamm_dashboard-2024.5.24/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4850 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/requirements_dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.349808 seamm_dashboard-2024.5.24/seamm_dashboard/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8236 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-24 17:14:13.349808 seamm_dashboard-2024.5.24/seamm_dashboard/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2120 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/flask_authorize_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/jwt_patch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      498 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/results_dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.297807 seamm_dashboard-2024.5.24/seamm_dashboard/routes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.309807 seamm_dashboard-2024.5.24/seamm_dashboard/routes/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/admin/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17344 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/admin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.309807 seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/flowcharts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.309807 seamm_dashboard-2024.5.24/seamm_dashboard/routes/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/auth/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/auth/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.309807 seamm_dashboard-2024.5.24/seamm_dashboard/routes/flowcharts/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/flowcharts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/flowcharts/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.309807 seamm_dashboard-2024.5.24/seamm_dashboard/routes/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/jobs/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18322 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/jobs/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.313807 seamm_dashboard-2024.5.24/seamm_dashboard/routes/main/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      255 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/main/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/main/forms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1209 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/main/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.313807 seamm_dashboard-2024.5.24/seamm_dashboard/routes/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/projects/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/projects/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21003 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/setup_argparsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/setup_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.313807 seamm_dashboard-2024.5.24/seamm_dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.317807 seamm_dashboard-2024.5.24/seamm_dashboard/static/css/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6653 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/css/bootstrap-select.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    29130 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/css/custom_flowchart.css
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/css/jobs_list.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6502 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/css/prism.css
+-rw-r--r--   0 runner    (1001) docker     (127)   281191 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)   647497 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/css/style.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   232121 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/css/style.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   876516 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/css/style.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.317807 seamm_dashboard-2024.5.24/seamm_dashboard/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    12238 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/images/Banner_AllCaps.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    26358 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/images/MolSSI-Logo-xl.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/images/briefcase.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/images/molssi-favicon-inverted.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    16562 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/images/molssi-favicon.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/images/object-group.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/images/project-diagram.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.317807 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.321807 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/2.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/3.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/4.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    19058 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/5.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/6.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/7.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    20466 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/8.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.321807 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/brand/
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/brand/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/brand/sygnet.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.321807 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/buildings.js
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/collapsible.js
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/colors.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/flowchart_list.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19705 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/job_report.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/jobs_list.js
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/login.js
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/logout.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/manage_groups.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/manage_user.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/manage_users.js
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/popovers.js
+-rw-r--r--   0 runner    (1001) docker     (127)    32221 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/prism.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/project_list.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/render_flowchart.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/setup.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/table_api.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/timer.js
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/tooltips.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/util.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/widgets.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.297807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@coreui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.297807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@coreui/coreui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.297807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@coreui/coreui/dist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.321807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@coreui/coreui/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    31892 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@coreui/coreui/dist/js/coreui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@fortawesome/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@fortawesome/fontawesome-free/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.321807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@fortawesome/fontawesome-free/js/
+-rw-r--r--   0 runner    (1001) docker     (127)  1196706 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@fortawesome/fontawesome-free/js/all.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/bootstrap/dist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/bootstrap/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    62563 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/bootstrap/dist/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/cytoscape/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/cytoscape/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)   372530 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/cytoscape/dist/cytoscape.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    87278 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net/js/jquery.dataTables.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-bs4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-bs4/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    11663 2024-05-24 17:13:01.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-bs4/css/dataTables.bootstrap4.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-bs4/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-bs4/js/dataTables.bootstrap4.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-buttons/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-buttons/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    19994 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-buttons/js/dataTables.buttons.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-buttons-bs4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-buttons-bs4/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-24 17:13:01.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-buttons-bs4/css/buttons.bootstrap4.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-dt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-dt/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-dt/js/dataTables.dataTables.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-select/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-select/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    14277 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-select/js/dataTables.select.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-select-dt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-select-dt/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-24 17:13:01.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-select-dt/css/select.dataTables.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jquery/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)    87533 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jquery/dist/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jquery-csv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jquery-csv/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     9302 2024-05-24 17:13:01.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jquery-csv/src/jquery.csv.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.329807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)   141969 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/jstree.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.329807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/themes/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/themes/default/32px.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31730 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/themes/default/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/themes/default/throbber.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/ngl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.329807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/ngl/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)  1120787 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/ngl/dist/ngl.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.329807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/pace-progress/
+-rw-r--r--   0 runner    (1001) docker     (127)    12507 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/pace-progress/pace.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/perfect-scrollbar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.329807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/perfect-scrollbar/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)    19549 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/perfect-scrollbar/dist/perfect-scrollbar.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.329807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/plotly.js-dist-min/
+-rw-r--r--   0 runner    (1001) docker     (127)  3478174 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/plotly.js-dist-min/plotly.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/popper.js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/popper.js/dist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.333807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/popper.js/dist/umd/
+-rw-r--r--   0 runner    (1001) docker     (127)    21233 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/popper.js/dist/umd/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/only_needed_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101936 2024-05-24 17:13:25.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.333807 seamm_dashboard-2024.5.24/seamm_dashboard/static/tmp/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/tmp/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    22082 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/swagger.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/template_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.337807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/401.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/500.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.337807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/change_email.html
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/change_password.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/create_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/create_user.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/delete_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/delete_user.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.337807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/email/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/email/change_email.html
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/email/change_email.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/email/confirm.html
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/email/confirm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/email/reset_password.html
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/email/reset_password.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/manage_groups.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/manage_users.html
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/register.html
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/reset_password.html
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/unconfirmed.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.341807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/auth/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/auth/confirm_login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/auth/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/auth/manage_account.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.341807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/flowcharts/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/flowcharts/flowchart_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/flowcharts/render_flowchart.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    31853 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/index_full.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.341807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/jobs/edit_job.html
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/jobs/import_job.html
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/jobs/job_parameters.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/jobs/job_report.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/jobs/jobs_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/jobs/submit_job.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/login_coreui.html
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/login_script.html
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/logout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.341807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/projects/project_access.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/projects/project_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/register.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.341807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.345807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/breadcrumb.html
+-rw-r--r--   0 runner    (1001) docker     (127)    41683 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/card.html
+-rw-r--r--   0 runner    (1001) docker     (127)    17627 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/cards.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16183 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/carousel.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/collapse.html
+-rw-r--r--   0 runner    (1001) docker     (127)    47501 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/forms.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/jumbotron.html
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/list-group.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/navs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/popovers.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/progress.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/scrollspy.html
+-rw-r--r--   0 runner    (1001) docker     (127)    40822 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/switches.html
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/tables.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9781 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/tabs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/tooltips.html
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/blank.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.345807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)    41831 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/brand-buttons.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/button-group.html
+-rw-r--r--   0 runner    (1001) docker     (127)    27328 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/buttons.html
+-rw-r--r--   0 runner    (1001) docker     (127)    21346 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/dropdowns.html
+-rw-r--r--   0 runner    (1001) docker     (127)    38782 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/social-buttons.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/charts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/colors.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.345807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)    44734 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/icons/flags.html
+-rw-r--r--   0 runner    (1001) docker     (127)   141248 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/icons/font-awesome.html
+-rw-r--r--   0 runner    (1001) docker     (127)    26687 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/icons/simple-line-icons.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/main.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.345807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/notifications/alerts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/notifications/badge.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/notifications/modals.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/typography.html
+-rw-r--r--   0 runner    (1001) docker     (127)    32244 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/widgets.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.349808 seamm_dashboard-2024.5.24/seamm_dashboard/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/tests/test_api_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/tests/test_api_authenticated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/tests/test_api_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15489 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.349808 seamm_dashboard-2024.5.24/seamm_dashboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-05-24 17:14:13.000000 seamm_dashboard-2024.5.24/seamm_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-05-24 17:14:13.000000 seamm_dashboard-2024.5.24/seamm_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 17:14:13.000000 seamm_dashboard-2024.5.24/seamm_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-24 17:14:13.000000 seamm_dashboard-2024.5.24/seamm_dashboard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 17:13:26.000000 seamm_dashboard-2024.5.24/seamm_dashboard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-24 17:14:13.000000 seamm_dashboard-2024.5.24/seamm_dashboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-24 17:14:13.000000 seamm_dashboard-2024.5.24/seamm_dashboard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-24 17:14:13.349808 seamm_dashboard-2024.5.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/versioneer.py
```

### Comparing `seamm-dashboard-2024.3.27/LICENSE` & `seamm_dashboard-2024.5.24/LICENSE`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/PKG-INFO` & `seamm_dashboard-2024.5.24/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamm-dashboard
-Version: 2024.3.27
+Version: 2024.5.24
 Summary: The Web Dashboard for SEAMM (Simulation Environment for Atomistic and Molecular Simulations).
 Home-page: https://github.com/molssi-seamm/seamm_dashboard.git
 Author: Jessica Nash
 Author-email: janash@vt.edu
 License: BSD-3C
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `seamm-dashboard-2024.3.27/README.md` & `seamm_dashboard-2024.5.24/README.md`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/__init__.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/config.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/config.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/flask_authorize_patch.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/flask_authorize_patch.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/jwt_patch.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/jwt_patch.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/routes/admin/forms.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/routes/admin/forms.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/routes/admin/views.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/routes/admin/views.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/routes/api/auth.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/auth.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/routes/api/flowcharts.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/flowcharts.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/routes/api/groups.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/groups.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/routes/api/jobs.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/jobs.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/routes/api/projects.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/projects.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/routes/api/status.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/status.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/routes/api/users.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/users.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/routes/auth/forms.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/routes/auth/forms.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/routes/auth/views.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/routes/auth/views.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/routes/flowcharts/views.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/routes/flowcharts/views.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/routes/jobs/forms.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/routes/jobs/forms.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/routes/jobs/views.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/routes/jobs/views.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/routes/main/views.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/routes/main/views.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/routes/projects/forms.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/routes/projects/forms.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/routes/projects/views.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/routes/projects/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,19 +184,24 @@
     # Build the url ourselves.
     base_url = url_for("main.index")
     project_url = base_url + f"#projects/{project_id}/jobs"
 
     if request.method == "POST":
         if form.validate_on_submit():
 
-            if form.allow_public:
+            if form.allow_public.data:
                 permissions = deepcopy(project.permissions)
                 permissions["other"] = ["read"]
                 project.permissions = permissions
                 db.session.commit()
+            else:
+                permissions = deepcopy(project.permissions)
+                permissions["other"] = []
+                project.permissions = permissions
+                db.session.commit()
 
             user_keys = [
                 x for x in form.data.keys() if "user" in x if form.data[x] is True
             ]
 
             permissions_dict = {}
```

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/setup_argparsing.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/setup_argparsing.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/setup_logging.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/setup_logging.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/css/bootstrap-select.min.css` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/css/bootstrap-select.min.css`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/css/custom.css` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/css/custom_flowchart.css` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/css/custom_flowchart.css`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/css/prism.css` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/css/prism.css`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/css/style.css` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/css/style.css`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/css/style.css.map` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/css/style.css.map`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/css/style.min.css` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/css/style.min.css`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/css/style.min.css.map` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/css/style.min.css.map`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/images/Banner_AllCaps.jpg` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/images/Banner_AllCaps.jpg`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/images/MolSSI-Logo-xl.jpg` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/images/MolSSI-Logo-xl.jpg`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/images/molssi-favicon-inverted.svg` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/images/molssi-favicon-inverted.svg`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/images/molssi-favicon.jpg` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/images/molssi-favicon.jpg`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/images/object-group.svg` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/images/object-group.svg`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/img/avatars/1.jpg` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/1.jpg`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/img/avatars/2.jpg` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/2.jpg`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/img/avatars/3.jpg` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/3.jpg`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/img/avatars/4.jpg` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/4.jpg`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/img/avatars/5.jpg` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/5.jpg`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/img/avatars/6.jpg` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/6.jpg`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/img/avatars/7.jpg` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/7.jpg`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/img/avatars/8.jpg` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/8.jpg`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/img/brand/logo.svg` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/brand/logo.svg`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/img/brand/sygnet.svg` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/brand/sygnet.svg`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/img/favicon.ico` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/img/favicon.png` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/favicon.png`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/js/buildings.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/buildings.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/js/colors.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/colors.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/js/flowchart_list.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/flowchart_list.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/js/job_report.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/job_report.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/js/jobs_list.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/jobs_list.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/js/main.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/main.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/js/manage_groups.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/manage_groups.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/js/manage_user.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/manage_user.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/js/manage_users.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/manage_users.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/js/prism.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/prism.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/js/project_list.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/project_list.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/js/render_flowchart.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/render_flowchart.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/js/setup.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/setup.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/js/table_api.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/table_api.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/js/timer.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/timer.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/js/util.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/util.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/js/widgets.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/widgets.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/@coreui/coreui/dist/js/coreui.min.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@coreui/coreui/dist/js/coreui.min.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/@fortawesome/fontawesome-free/js/all.min.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@fortawesome/fontawesome-free/js/all.min.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/bootstrap/dist/js/bootstrap.min.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/bootstrap/dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/cytoscape/dist/cytoscape.min.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/cytoscape/dist/cytoscape.min.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright (c) 2016-2023, The Cytoscape Consortium.
+ * Copyright (c) 2016-2024, The Cytoscape Consortium.
  *
  * Permission is hereby granted, free of charge, to any person obtaining a copy of
  * this software and associated documentation files (the “Software”), to deal in
  * the Software without restriction, including without limitation the rights to
  * use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
  * of the Software, and to permit persons to whom the Software is furnished to do
  * so, subject to the following conditions:
@@ -76,83 +76,84 @@
                 try {
                     o || null == n.return || n.return()
                 } finally {
                     if (s) throw i
                 }
             }
             return a
-        }(e, t) || function(e, t) {
-            if (!e) return;
-            if ("string" == typeof e) return o(e, t);
-            var n = Object.prototype.toString.call(e).slice(8, -1);
-            "Object" === n && e.constructor && (n = e.constructor.name);
-            if ("Map" === n || "Set" === n) return Array.from(e);
-            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return o(e, t)
-        }(e, t) || function() {
+        }(e, t) || o(e, t) || function() {
             throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
     function o(e, t) {
+        if (e) {
+            if ("string" == typeof e) return s(e, t);
+            var n = Object.prototype.toString.call(e).slice(8, -1);
+            return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? s(e, t) : void 0
+        }
+    }
+
+    function s(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
         return r
     }
-    var s = "undefined" == typeof window ? null : window,
-        l = s ? s.navigator : null;
-    s && s.document;
-    var u = e(""),
-        c = e({}),
-        d = e((function() {})),
-        h = "undefined" == typeof HTMLElement ? "undefined" : e(HTMLElement),
-        p = function(e) {
-            return e && e.instanceString && g(e.instanceString) ? e.instanceString() : null
-        },
-        f = function(t) {
-            return null != t && e(t) == u
+    var l = "undefined" == typeof window ? null : window,
+        u = l ? l.navigator : null;
+    l && l.document;
+    var c = e(""),
+        d = e({}),
+        h = e((function() {})),
+        p = "undefined" == typeof HTMLElement ? "undefined" : e(HTMLElement),
+        f = function(e) {
+            return e && e.instanceString && v(e.instanceString) ? e.instanceString() : null
         },
         g = function(t) {
-            return null != t && e(t) === d
+            return null != t && e(t) == c
         },
-        v = function(e) {
-            return !x(e) && (Array.isArray ? Array.isArray(e) : null != e && e instanceof Array)
+        v = function(t) {
+            return null != t && e(t) === h
         },
-        y = function(t) {
-            return null != t && e(t) === c && !v(t) && t.constructor === Object
+        y = function(e) {
+            return !w(e) && (Array.isArray ? Array.isArray(e) : null != e && e instanceof Array)
         },
         m = function(t) {
-            return null != t && e(t) === e(1) && !isNaN(t)
+            return null != t && e(t) === d && !y(t) && t.constructor === Object
         },
-        b = function(e) {
-            return "undefined" === h ? void 0 : null != e && e instanceof HTMLElement
+        b = function(t) {
+            return null != t && e(t) === e(1) && !isNaN(t)
         },
         x = function(e) {
-            return w(e) || E(e)
+            return "undefined" === p ? void 0 : null != e && e instanceof HTMLElement
         },
         w = function(e) {
-            return "collection" === p(e) && e._private.single
+            return E(e) || k(e)
         },
         E = function(e) {
-            return "collection" === p(e) && !e._private.single
+            return "collection" === f(e) && e._private.single
         },
         k = function(e) {
-            return "core" === p(e)
+            return "collection" === f(e) && !e._private.single
         },
         C = function(e) {
-            return "stylesheet" === p(e)
+            return "core" === f(e)
         },
         S = function(e) {
+            return "stylesheet" === f(e)
+        },
+        P = function(e) {
             return null == e || !("" !== e && !e.match(/^\s+$/))
         },
-        P = function(t) {
+        D = function(t) {
             return function(t) {
-                return null != t && e(t) === c
-            }(t) && g(t.then)
+                return null != t && e(t) === d
+            }(t) && v(t.then)
         },
-        D = function(e, t) {
+        T = function(e, t) {
             t || (t = function() {
                 if (1 === arguments.length) return arguments[0];
                 if (0 === arguments.length) return "undefined";
                 for (var e = [], t = 0; t < arguments.length; t++) e.push(arguments[t]);
                 return e.join("$")
             });
             var n = function n() {
@@ -160,50 +161,50 @@
                     a = arguments,
                     o = t.apply(i, a),
                     s = n.cache;
                 return (r = s[o]) || (r = s[o] = e.apply(i, a)), r
             };
             return n.cache = {}, n
         },
-        T = D((function(e) {
+        _ = T((function(e) {
             return e.replace(/([A-Z])/g, (function(e) {
                 return "-" + e.toLowerCase()
             }))
         })),
-        _ = D((function(e) {
+        M = T((function(e) {
             return e.replace(/(-\w)/g, (function(e) {
                 return e[1].toUpperCase()
             }))
         })),
-        M = D((function(e, t) {
+        B = T((function(e, t) {
             return e + t[0].toUpperCase() + t.substring(1)
         }), (function(e, t) {
             return e + "$" + t
         })),
-        B = function(e) {
-            return S(e) ? e : e.charAt(0).toUpperCase() + e.substring(1)
+        N = function(e) {
+            return P(e) ? e : e.charAt(0).toUpperCase() + e.substring(1)
         },
-        N = "(?:[-+]?(?:(?:\\d+|\\d*\\.\\d+)(?:[Ee][+-]?\\d+)?))",
-        z = function(e, t) {
+        z = "(?:[-+]?(?:(?:\\d+|\\d*\\.\\d+)(?:[Ee][+-]?\\d+)?))",
+        I = function(e, t) {
             return e < t ? -1 : e > t ? 1 : 0
         },
-        I = null != Object.assign ? Object.assign.bind(Object) : function(e) {
+        A = null != Object.assign ? Object.assign.bind(Object) : function(e) {
             for (var t = arguments, n = 1; n < t.length; n++) {
                 var r = t[n];
                 if (null != r)
                     for (var i = Object.keys(r), a = 0; a < i.length; a++) {
                         var o = i[a];
                         e[o] = r[o]
                     }
             }
             return e
         },
         L = function(e) {
-            return (v(e) ? e : null) || function(e) {
-                return A[e.toLowerCase()]
+            return (y(e) ? e : null) || function(e) {
+                return O[e.toLowerCase()]
             }(e) || function(e) {
                 if ((4 === e.length || 7 === e.length) && "#" === e[0]) {
                     var t, n, r;
                     return 4 === e.length ? (t = parseInt(e[1] + e[1], 16), n = parseInt(e[2] + e[2], 16), r = parseInt(e[3] + e[3], 16)) : (t = parseInt(e[1] + e[2], 16), n = parseInt(e[3] + e[4], 16), r = parseInt(e[5] + e[6], 16)), [t, n, r]
                 }
             }(e) || function(e) {
                 var t, n = new RegExp("^rgb[a]?\\(((?:[-+]?(?:(?:\\d+|\\d*\\.\\d+)(?:[Ee][+-]?\\d+)?))[%]?)\\s*,\\s*((?:[-+]?(?:(?:\\d+|\\d*\\.\\d+)(?:[Ee][+-]?\\d+)?))[%]?)\\s*,\\s*((?:[-+]?(?:(?:\\d+|\\d*\\.\\d+)(?:[Ee][+-]?\\d+)?))[%]?)(?:\\s*,\\s*((?:[-+]?(?:(?:\\d+|\\d*\\.\\d+)(?:[Ee][+-]?\\d+)?))))?\\)$").exec(e);
@@ -242,15 +243,15 @@
                         o = Math.round(255 * u(h, d, n + 1 / 3)), s = Math.round(255 * u(h, d, n)), l = Math.round(255 * u(h, d, n - 1 / 3))
                     }
                     t = [o, s, l, a]
                 }
                 return t
             }(e)
         },
-        A = {
+        O = {
             transparent: [0, 0, 0, 0],
             aliceblue: [240, 248, 255],
             antiquewhite: [250, 235, 215],
             aqua: [0, 255, 255],
             aquamarine: [127, 255, 212],
             azure: [240, 255, 255],
             beige: [245, 245, 220],
@@ -392,97 +393,97 @@
             violet: [238, 130, 238],
             wheat: [245, 222, 179],
             white: [255, 255, 255],
             whitesmoke: [245, 245, 245],
             yellow: [255, 255, 0],
             yellowgreen: [154, 205, 50]
         },
-        O = function(e) {
+        R = function(e) {
             for (var t = e.map, n = e.keys, r = n.length, i = 0; i < r; i++) {
                 var a = n[i];
-                if (y(a)) throw Error("Tried to set map with object key");
+                if (m(a)) throw Error("Tried to set map with object key");
                 i < n.length - 1 ? (null == t[a] && (t[a] = {}), t = t[a]) : t[a] = e.value
             }
         },
-        R = function(e) {
+        V = function(e) {
             for (var t = e.map, n = e.keys, r = n.length, i = 0; i < r; i++) {
                 var a = n[i];
-                if (y(a)) throw Error("Tried to get map with object key");
+                if (m(a)) throw Error("Tried to get map with object key");
                 if (null == (t = t[a])) return t
             }
             return t
         };
-    var V = function(e) {
+    var F = function(e) {
             var t = typeof e;
             return null != e && ("object" == t || "function" == t)
         },
-        F = "undefined" != typeof globalThis ? globalThis : "undefined" != typeof window ? window : "undefined" != typeof global ? global : "undefined" != typeof self ? self : {};
-    var j = "object" == typeof F && F && F.Object === Object && F,
-        q = "object" == typeof self && self && self.Object === Object && self,
-        Y = j || q || Function("return this")(),
-        X = function() {
-            return Y.Date.now()
-        },
-        W = /\s/;
-    var H = function(e) {
-            for (var t = e.length; t-- && W.test(e.charAt(t)););
+        j = "undefined" != typeof globalThis ? globalThis : "undefined" != typeof window ? window : "undefined" != typeof global ? global : "undefined" != typeof self ? self : {};
+    var q = "object" == typeof j && j && j.Object === Object && j,
+        Y = "object" == typeof self && self && self.Object === Object && self,
+        X = q || Y || Function("return this")(),
+        W = function() {
+            return X.Date.now()
+        },
+        H = /\s/;
+    var K = function(e) {
+            for (var t = e.length; t-- && H.test(e.charAt(t)););
             return t
         },
-        K = /^\s+/;
-    var G = function(e) {
-            return e ? e.slice(0, H(e) + 1).replace(K, "") : e
-        },
-        U = Y.Symbol,
-        Z = Object.prototype,
-        $ = Z.hasOwnProperty,
-        Q = Z.toString,
-        J = U ? U.toStringTag : void 0;
-    var ee = function(e) {
-            var t = $.call(e, J),
-                n = e[J];
+        G = /^\s+/;
+    var U = function(e) {
+            return e ? e.slice(0, K(e) + 1).replace(G, "") : e
+        },
+        Z = X.Symbol,
+        $ = Object.prototype,
+        Q = $.hasOwnProperty,
+        J = $.toString,
+        ee = Z ? Z.toStringTag : void 0;
+    var te = function(e) {
+            var t = Q.call(e, ee),
+                n = e[ee];
             try {
-                e[J] = void 0;
+                e[ee] = void 0;
                 var r = !0
             } catch (e) {}
-            var i = Q.call(e);
-            return r && (t ? e[J] = n : delete e[J]), i
+            var i = J.call(e);
+            return r && (t ? e[ee] = n : delete e[ee]), i
         },
-        te = Object.prototype.toString;
-    var ne = function(e) {
-            return te.call(e)
-        },
-        re = U ? U.toStringTag : void 0;
-    var ie = function(e) {
-        return null == e ? void 0 === e ? "[object Undefined]" : "[object Null]" : re && re in Object(e) ? ee(e) : ne(e)
-    };
+        ne = Object.prototype.toString;
+    var re = function(e) {
+            return ne.call(e)
+        },
+        ie = Z ? Z.toStringTag : void 0;
     var ae = function(e) {
-        return null != e && "object" == typeof e
+        return null == e ? void 0 === e ? "[object Undefined]" : "[object Null]" : ie && ie in Object(e) ? te(e) : re(e)
     };
     var oe = function(e) {
-            return "symbol" == typeof e || ae(e) && "[object Symbol]" == ie(e)
+        return null != e && "object" == typeof e
+    };
+    var se = function(e) {
+            return "symbol" == typeof e || oe(e) && "[object Symbol]" == ae(e)
         },
-        se = /^[-+]0x[0-9a-f]+$/i,
-        le = /^0b[01]+$/i,
-        ue = /^0o[0-7]+$/i,
-        ce = parseInt;
-    var de = function(e) {
+        le = /^[-+]0x[0-9a-f]+$/i,
+        ue = /^0b[01]+$/i,
+        ce = /^0o[0-7]+$/i,
+        de = parseInt;
+    var he = function(e) {
             if ("number" == typeof e) return e;
-            if (oe(e)) return NaN;
-            if (V(e)) {
+            if (se(e)) return NaN;
+            if (F(e)) {
                 var t = "function" == typeof e.valueOf ? e.valueOf() : e;
-                e = V(t) ? t + "" : t
+                e = F(t) ? t + "" : t
             }
             if ("string" != typeof e) return 0 === e ? e : +e;
-            e = G(e);
-            var n = le.test(e);
-            return n || ue.test(e) ? ce(e.slice(2), n ? 2 : 8) : se.test(e) ? NaN : +e
-        },
-        he = Math.max,
-        pe = Math.min;
-    var fe = function(e, t, n) {
+            e = U(e);
+            var n = ue.test(e);
+            return n || ce.test(e) ? de(e.slice(2), n ? 2 : 8) : le.test(e) ? NaN : +e
+        },
+        pe = Math.max,
+        fe = Math.min;
+    var ge = function(e, t, n) {
             var r, i, a, o, s, l, u = 0,
                 c = !1,
                 d = !1,
                 h = !0;
             if ("function" != typeof e) throw new TypeError("Expected a function");
 
             function p(t) {
@@ -497,175 +498,175 @@
 
             function g(e) {
                 var n = e - l;
                 return void 0 === l || n >= t || n < 0 || d && e - u >= a
             }
 
             function v() {
-                var e = X();
+                var e = W();
                 if (g(e)) return y(e);
                 s = setTimeout(v, function(e) {
                     var n = t - (e - l);
-                    return d ? pe(n, a - (e - u)) : n
+                    return d ? fe(n, a - (e - u)) : n
                 }(e))
             }
 
             function y(e) {
                 return s = void 0, h && r ? p(e) : (r = i = void 0, o)
             }
 
             function m() {
-                var e = X(),
+                var e = W(),
                     n = g(e);
                 if (r = arguments, i = this, l = e, n) {
                     if (void 0 === s) return f(l);
                     if (d) return clearTimeout(s), s = setTimeout(v, t), p(l)
                 }
                 return void 0 === s && (s = setTimeout(v, t)), o
             }
-            return t = de(t) || 0, V(n) && (c = !!n.leading, a = (d = "maxWait" in n) ? he(de(n.maxWait) || 0, t) : a, h = "trailing" in n ? !!n.trailing : h), m.cancel = function() {
+            return t = he(t) || 0, F(n) && (c = !!n.leading, a = (d = "maxWait" in n) ? pe(he(n.maxWait) || 0, t) : a, h = "trailing" in n ? !!n.trailing : h), m.cancel = function() {
                 void 0 !== s && clearTimeout(s), u = 0, r = l = i = s = void 0
             }, m.flush = function() {
-                return void 0 === s ? o : y(X())
+                return void 0 === s ? o : y(W())
             }, m
         },
-        ge = s ? s.performance : null,
-        ve = ge && ge.now ? function() {
-            return ge.now()
+        ve = l ? l.performance : null,
+        ye = ve && ve.now ? function() {
+            return ve.now()
         } : function() {
             return Date.now()
         },
-        ye = function() {
-            if (s) {
-                if (s.requestAnimationFrame) return function(e) {
-                    s.requestAnimationFrame(e)
+        me = function() {
+            if (l) {
+                if (l.requestAnimationFrame) return function(e) {
+                    l.requestAnimationFrame(e)
                 };
-                if (s.mozRequestAnimationFrame) return function(e) {
-                    s.mozRequestAnimationFrame(e)
+                if (l.mozRequestAnimationFrame) return function(e) {
+                    l.mozRequestAnimationFrame(e)
                 };
-                if (s.webkitRequestAnimationFrame) return function(e) {
-                    s.webkitRequestAnimationFrame(e)
+                if (l.webkitRequestAnimationFrame) return function(e) {
+                    l.webkitRequestAnimationFrame(e)
                 };
-                if (s.msRequestAnimationFrame) return function(e) {
-                    s.msRequestAnimationFrame(e)
+                if (l.msRequestAnimationFrame) return function(e) {
+                    l.msRequestAnimationFrame(e)
                 }
             }
             return function(e) {
                 e && setTimeout((function() {
-                    e(ve())
+                    e(ye())
                 }), 1e3 / 60)
             }
         }(),
-        me = function(e) {
-            return ye(e)
+        be = function(e) {
+            return me(e)
         },
-        be = ve,
-        xe = 65599,
-        we = function(e) {
-            for (var t, n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 9261, r = n; !(t = e.next()).done;) r = r * xe + t.value | 0;
+        xe = ye,
+        we = 65599,
+        Ee = function(e) {
+            for (var t, n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 9261, r = n; !(t = e.next()).done;) r = r * we + t.value | 0;
             return r
         },
-        Ee = function(e) {
+        ke = function(e) {
             var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 9261;
-            return t * xe + e | 0
+            return t * we + e | 0
         },
-        ke = function(e) {
+        Ce = function(e) {
             var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 5381;
             return (t << 5) + t + e | 0
         },
-        Ce = function(e) {
+        Se = function(e) {
             return 2097152 * e[0] + e[1]
         },
-        Se = function(e, t) {
-            return [Ee(e[0], t[0]), ke(e[1], t[1])]
-        },
         Pe = function(e, t) {
+            return [ke(e[0], t[0]), Ce(e[1], t[1])]
+        },
+        De = function(e, t) {
             var n = {
                     value: 0,
                     done: !1
                 },
                 r = 0,
                 i = e.length;
-            return we({
+            return Ee({
                 next: function() {
                     return r < i ? n.value = e.charCodeAt(r++) : n.done = !0, n
                 }
             }, t)
         },
-        De = function() {
-            return Te(arguments)
+        Te = function() {
+            return _e(arguments)
         },
-        Te = function(e) {
+        _e = function(e) {
             for (var t, n = 0; n < e.length; n++) {
                 var r = e[n];
-                t = 0 === n ? Pe(r) : Pe(r, t)
+                t = 0 === n ? De(r) : De(r, t)
             }
             return t
         },
-        _e = !0,
-        Me = null != console.warn,
-        Be = null != console.trace,
-        Ne = Number.MAX_SAFE_INTEGER || 9007199254740991,
-        ze = function() {
+        Me = !0,
+        Be = null != console.warn,
+        Ne = null != console.trace,
+        ze = Number.MAX_SAFE_INTEGER || 9007199254740991,
+        Ie = function() {
             return !0
         },
-        Ie = function() {
+        Ae = function() {
             return !1
         },
         Le = function() {
             return 0
         },
-        Ae = function() {},
-        Oe = function(e) {
-            throw new Error(e)
-        },
+        Oe = function() {},
         Re = function(e) {
-            if (void 0 === e) return _e;
-            _e = !!e
+            throw new Error(e)
         },
         Ve = function(e) {
-            Re() && (Me ? console.warn(e) : (console.log(e), Be && console.trace()))
+            if (void 0 === e) return Me;
+            Me = !!e
         },
         Fe = function(e) {
-            return null == e ? e : v(e) ? e.slice() : y(e) ? function(e) {
-                return I({}, e)
+            Ve() && (Be ? console.warn(e) : (console.log(e), Ne && console.trace()))
+        },
+        je = function(e) {
+            return null == e ? e : y(e) ? e.slice() : m(e) ? function(e) {
+                return A({}, e)
             }(e) : e
         },
-        je = function(e, t) {
+        qe = function(e, t) {
             for (t = e = ""; e++ < 36; t += 51 * e & 52 ? (15 ^ e ? 8 ^ Math.random() * (20 ^ e ? 16 : 4) : 4).toString(16) : "-");
             return t
         },
-        qe = {},
-        Ye = function() {
-            return qe
+        Ye = {},
+        Xe = function() {
+            return Ye
         },
-        Xe = function(e) {
+        We = function(e) {
             var t = Object.keys(e);
             return function(n) {
                 for (var r = {}, i = 0; i < t.length; i++) {
                     var a = t[i],
                         o = null == n ? void 0 : n[a];
                     r[a] = void 0 === o ? e[a] : o
                 }
                 return r
             }
         },
-        We = function(e, t, n) {
+        He = function(e, t, n) {
             for (var r = e.length - 1; r >= 0 && (e[r] !== t || (e.splice(r, 1), !n)); r--);
         },
-        He = function(e) {
+        Ke = function(e) {
             e.splice(0, e.length)
         },
-        Ke = function(e, t, n) {
-            return n && (t = M(n, t)), e[t]
+        Ge = function(e, t, n) {
+            return n && (t = B(n, t)), e[t]
         },
-        Ge = function(e, t, n, r) {
-            n && (t = M(n, t)), e[t] = r
+        Ue = function(e, t, n, r) {
+            n && (t = B(n, t)), e[t] = r
         },
-        Ue = "undefined" != typeof Map ? Map : function() {
+        Ze = "undefined" != typeof Map ? Map : function() {
             function e() {
                 t(this, e), this._obj = {}
             }
             return r(e, [{
                 key: "set",
                 value: function(e, t) {
                     return this._obj[e] = t, this
@@ -688,15 +689,15 @@
             }, {
                 key: "get",
                 value: function(e) {
                     return this._obj[e]
                 }
             }]), e
         }(),
-        Ze = function() {
+        $e = function() {
             function e(n) {
                 if (t(this, e), this._obj = Object.create(null), this.size = 0, null != n) {
                     var r;
                     r = null != n.instanceString && n.instanceString() === this.instanceString() ? n.toArray() : n;
                     for (var i = 0; i < r.length; i++) this.add(r[i])
                 }
             }
@@ -738,18 +739,18 @@
             }, {
                 key: "forEach",
                 value: function(e, t) {
                     return this.toArray().forEach(e, t)
                 }
             }]), e
         }(),
-        $e = "undefined" !== ("undefined" == typeof Set ? "undefined" : e(Set)) ? Set : Ze,
-        Qe = function(e, t) {
+        Qe = "undefined" !== ("undefined" == typeof Set ? "undefined" : e(Set)) ? Set : $e,
+        Je = function(e, t) {
             var n = !(arguments.length > 2 && void 0 !== arguments[2]) || arguments[2];
-            if (void 0 !== e && void 0 !== t && k(e)) {
+            if (void 0 !== e && void 0 !== t && C(e)) {
                 var r = t.group;
                 if (null == r && (r = t.data && null != t.data.source && null != t.data.target ? "edges" : "nodes"), "nodes" === r || "edges" === r) {
                     this.length = 1, this[0] = this;
                     var i = this._private = {
                         cy: e,
                         single: !0,
                         data: t.data || {},
@@ -771,15 +772,15 @@
                         selected: !!t.selected,
                         selectable: void 0 === t.selectable || !!t.selectable,
                         locked: !!t.locked,
                         grabbed: !1,
                         grabbable: void 0 === t.grabbable || !!t.grabbable,
                         pannable: void 0 === t.pannable ? "edges" === r : !!t.pannable,
                         active: !1,
-                        classes: new $e,
+                        classes: new Qe,
                         animation: {
                             current: [],
                             queue: []
                         },
                         rscratch: {},
                         scratch: t.scratch || {},
                         edges: [],
@@ -813,58 +814,58 @@
                             s = e.zoom();
                         i.position = {
                             x: (a.x - o.x) / s,
                             y: (a.y - o.y) / s
                         }
                     }
                     var l = [];
-                    v(t.classes) ? l = t.classes : f(t.classes) && (l = t.classes.split(/\s+/));
+                    y(t.classes) ? l = t.classes : g(t.classes) && (l = t.classes.split(/\s+/));
                     for (var u = 0, c = l.length; u < c; u++) {
                         var d = l[u];
                         d && "" !== d && i.classes.add(d)
                     }
                     this.createEmitter();
                     var h = t.style || t.css;
-                    h && (Ve("Setting a `style` bypass at element creation should be done only when absolutely necessary.  Try to use the stylesheet instead."), this.style(h)), (void 0 === n || n) && this.restore()
-                } else Oe("An element must be of type `nodes` or `edges`; you specified `" + r + "`")
-            } else Oe("An element must have a core reference and parameters set")
+                    h && (Fe("Setting a `style` bypass at element creation should be done only when absolutely necessary.  Try to use the stylesheet instead."), this.style(h)), (void 0 === n || n) && this.restore()
+                } else Re("An element must be of type `nodes` or `edges`; you specified `" + r + "`")
+            } else Re("An element must have a core reference and parameters set")
         },
-        Je = function(e) {
+        et = function(e) {
             return e = {
                     bfs: e.bfs || !e.dfs,
                     dfs: e.dfs || !e.bfs
                 },
                 function(t, n, r) {
                     var i;
-                    y(t) && !x(t) && (t = (i = t).roots || i.root, n = i.visit, r = i.directed), r = 2 !== arguments.length || g(n) ? r : n, n = g(n) ? n : function() {};
-                    for (var a, o = this._private.cy, s = t = f(t) ? this.filter(t) : t, l = [], u = [], c = {}, d = {}, h = {}, p = 0, v = this.byGroup(), m = v.nodes, b = v.edges, w = 0; w < s.length; w++) {
-                        var E = s[w],
+                    m(t) && !w(t) && (t = (i = t).roots || i.root, n = i.visit, r = i.directed), r = 2 !== arguments.length || v(n) ? r : n, n = v(n) ? n : function() {};
+                    for (var a, o = this._private.cy, s = t = g(t) ? this.filter(t) : t, l = [], u = [], c = {}, d = {}, h = {}, p = 0, f = this.byGroup(), y = f.nodes, b = f.edges, x = 0; x < s.length; x++) {
+                        var E = s[x],
                             k = E.id();
                         E.isNode() && (l.unshift(E), e.bfs && (h[k] = !0, u.push(E)), d[k] = 0)
                     }
                     for (var C = function() {
                             var t = e.bfs ? l.shift() : l.pop(),
                                 i = t.id();
                             if (e.dfs) {
                                 if (h[i]) return "continue";
                                 h[i] = !0, u.push(t)
                             }
                             var o, s = d[i],
                                 f = c[i],
                                 g = null != f ? f.source() : null,
                                 v = null != f ? f.target() : null,
-                                y = null == f ? void 0 : t.same(g) ? v[0] : g[0];
-                            if (!0 === (o = n(t, f, y, p++, s))) return a = t, "break";
+                                m = null == f ? void 0 : t.same(g) ? v[0] : g[0];
+                            if (!0 === (o = n(t, f, m, p++, s))) return a = t, "break";
                             if (!1 === o) return "break";
                             for (var x = t.connectedEdges().filter((function(e) {
                                     return (!r || e.source().same(t)) && b.has(e)
                                 })), w = 0; w < x.length; w++) {
                                 var E = x[w],
                                     k = E.connectedNodes().filter((function(e) {
-                                        return !e.same(t) && m.has(e)
+                                        return !e.same(t) && y.has(e)
                                     })),
                                     C = k.id();
                                 0 === k.length || h[C] || (k = k[0], l.push(k), e.bfs && (h[C] = !0, u.push(k)), c[C] = E, d[C] = d[i] + 1)
                             }
                         }; 0 !== l.length;) {
                         var S = C();
                         if ("continue" !== S && "break" === S) break
@@ -876,24 +877,24 @@
                     }
                     return {
                         path: o.collection(P),
                         found: o.collection(a)
                     }
                 }
         },
-        et = {
-            breadthFirstSearch: Je({
+        tt = {
+            breadthFirstSearch: et({
                 bfs: !0
             }),
-            depthFirstSearch: Je({
+            depthFirstSearch: et({
                 dfs: !0
             })
         };
-    et.bfs = et.breadthFirstSearch, et.dfs = et.depthFirstSearch;
-    var tt = function(e, t) {
+    tt.bfs = tt.breadthFirstSearch, tt.dfs = tt.depthFirstSearch;
+    var nt = function(e, t) {
             return e(t = {
                 exports: {}
             }, t.exports), t.exports
         }((function(e, t) {
             (function() {
                 var t, n, r, i, a, o, s, l, u, c, d, h, p, f, g;
                 r = Math.floor, c = Math.min, n = function(e, t) {
@@ -976,61 +977,61 @@
                     }, e.prototype.clone = function() {
                         var t;
                         return (t = new e).nodes = this.nodes.slice(0), t
                     }, e.prototype.toArray = function() {
                         return this.nodes.slice(0)
                     }, e.prototype.insert = e.prototype.push, e.prototype.top = e.prototype.peek, e.prototype.front = e.prototype.peek, e.prototype.has = e.prototype.contains, e.prototype.copy = e.prototype.clone, e
                 }(), e.exports = t
-            }).call(F)
+            }).call(j)
         })),
-        nt = Xe({
+        rt = We({
             root: null,
             weight: function(e) {
                 return 1
             },
             directed: !1
         }),
-        rt = {
+        it = {
             dijkstra: function(e) {
-                if (!y(e)) {
+                if (!m(e)) {
                     var t = arguments;
                     e = {
                         root: t[0],
                         weight: t[1],
                         directed: t[2]
                     }
                 }
-                var n = nt(e),
+                var n = rt(e),
                     r = n.root,
                     i = n.weight,
                     a = n.directed,
                     o = this,
                     s = i,
-                    l = f(r) ? this.filter(r)[0] : r[0],
+                    l = g(r) ? this.filter(r)[0] : r[0],
                     u = {},
                     c = {},
                     d = {},
                     h = this.byGroup(),
                     p = h.nodes,
-                    g = h.edges;
-                g.unmergeBy((function(e) {
+                    f = h.edges;
+                f.unmergeBy((function(e) {
                     return e.isLoop()
                 }));
                 for (var v = function(e) {
                         return u[e.id()]
-                    }, m = function(e, t) {
+                    }, y = function(e, t) {
                         u[e.id()] = t, b.updateItem(e)
-                    }, b = new tt((function(e, t) {
+                    }, b = new nt((function(e, t) {
                         return v(e) - v(t)
                     })), x = 0; x < p.length; x++) {
                     var w = p[x];
                     u[w.id()] = w.same(l) ? 0 : 1 / 0, b.push(w)
                 }
                 for (var E = function(e, t) {
-                        for (var n, r = (a ? e.edgesTo(t) : e.edgesWith(t)).intersect(g), i = 1 / 0, o = 0; o < r.length; o++) {
+                        for (var n, r = (a ? e.edgesTo(t) : e.edgesWith(t)).intersect(f), i = 1 / 0, o = 0; o < r.length; o++) {
                             var l = r[o],
                                 u = s(l);
                             (u < i || !n) && (i = u, n = l)
                         }
                         return {
                             edge: n,
                             dist: i
@@ -1041,41 +1042,41 @@
                         S = k.id();
                     if (d[S] = C, C !== 1 / 0)
                         for (var P = k.neighborhood().intersect(p), D = 0; D < P.length; D++) {
                             var T = P[D],
                                 _ = T.id(),
                                 M = E(k, T),
                                 B = C + M.dist;
-                            B < v(T) && (m(T, B), c[_] = {
+                            B < v(T) && (y(T, B), c[_] = {
                                 node: k,
                                 edge: M.edge
                             })
                         }
                 }
                 return {
                     distanceTo: function(e) {
-                        var t = f(e) ? p.filter(e)[0] : e[0];
+                        var t = g(e) ? p.filter(e)[0] : e[0];
                         return d[t.id()]
                     },
                     pathTo: function(e) {
-                        var t = f(e) ? p.filter(e)[0] : e[0],
+                        var t = g(e) ? p.filter(e)[0] : e[0],
                             n = [],
                             r = t,
                             i = r.id();
                         if (t.length > 0)
                             for (n.unshift(t); c[i];) {
                                 var a = c[i];
                                 n.unshift(a.edge), n.unshift(a.node), i = (r = a.node).id()
                             }
                         return o.spawn(n)
                     }
                 }
             }
         },
-        it = {
+        at = {
             kruskal: function(e) {
                 e = e || function(e) {
                     return 1
                 };
                 for (var t = this.byGroup(), n = t.nodes, r = t.edges, i = n.length, a = new Array(i), o = n, s = function(e) {
                         for (var t = 0; t < a.length; t++) {
                             if (a[t].has(e)) return t
@@ -1092,44 +1093,44 @@
                         v = a[f],
                         y = a[g];
                     f !== g && (o.merge(d), v.merge(y), a.splice(g, 1))
                 }
                 return o
             }
         },
-        at = Xe({
+        ot = We({
             root: null,
             goal: null,
             weight: function(e) {
                 return 1
             },
             heuristic: function(e) {
                 return 0
             },
             directed: !1
         }),
-        ot = {
+        st = {
             aStar: function(e) {
                 var t = this.cy(),
-                    n = at(e),
+                    n = ot(e),
                     r = n.root,
                     i = n.goal,
                     a = n.heuristic,
                     o = n.directed,
                     s = n.weight;
                 r = t.collection(r)[0], i = t.collection(i)[0];
                 var l, u, c = r.id(),
                     d = i.id(),
                     h = {},
                     p = {},
                     f = {},
-                    g = new tt((function(e, t) {
+                    g = new nt((function(e, t) {
                         return p[e.id()] - p[t.id()]
                     })),
-                    v = new $e,
+                    v = new Qe,
                     y = {},
                     m = {},
                     b = function(e, t) {
                         g.push(e), v.add(t)
                     };
                 b(r, c), h[c] = 0, p[c] = a(r);
                 for (var x, w = 0; g.size() > 0;) {
@@ -1161,30 +1162,30 @@
                     found: !1,
                     distance: void 0,
                     path: void 0,
                     steps: w
                 }
             }
         },
-        st = Xe({
+        lt = We({
             weight: function(e) {
                 return 1
             },
             directed: !1
         }),
-        lt = {
+        ut = {
             floydWarshall: function(e) {
-                for (var t = this.cy(), n = st(e), r = n.weight, i = n.directed, a = r, o = this.byGroup(), s = o.nodes, l = o.edges, u = s.length, c = u * u, d = function(e) {
+                for (var t = this.cy(), n = lt(e), r = n.weight, i = n.directed, a = r, o = this.byGroup(), s = o.nodes, l = o.edges, u = s.length, c = u * u, d = function(e) {
                         return s.indexOf(e)
                     }, h = function(e) {
                         return s[e]
-                    }, p = new Array(c), g = 0; g < c; g++) {
-                    var v = g % u,
-                        y = (g - v) / u;
-                    p[g] = y === v ? 0 : 1 / 0
+                    }, p = new Array(c), f = 0; f < c; f++) {
+                    var v = f % u,
+                        y = (f - v) / u;
+                    p[f] = y === v ? 0 : 1 / 0
                 }
                 for (var m = new Array(c), b = new Array(c), x = 0; x < l.length; x++) {
                     var w = l[x],
                         E = w.source()[0],
                         k = w.target()[0];
                     if (E !== k) {
                         var C = d(E),
@@ -1200,71 +1201,71 @@
                 for (var _ = 0; _ < u; _++)
                     for (var M = 0; M < u; M++)
                         for (var B = M * u + _, N = 0; N < u; N++) {
                             var z = M * u + N,
                                 I = _ * u + N;
                             p[B] + p[I] < p[z] && (p[z] = p[B] + p[I], m[z] = m[B])
                         }
-                var L = function(e) {
+                var A = function(e) {
                     return d(function(e) {
-                        return (f(e) ? t.filter(e) : e)[0]
+                        return (g(e) ? t.filter(e) : e)[0]
                     }(e))
                 };
                 return {
                     distance: function(e, t) {
-                        var n = L(e),
-                            r = L(t);
+                        var n = A(e),
+                            r = A(t);
                         return p[n * u + r]
                     },
                     path: function(e, n) {
-                        var r = L(e),
-                            i = L(n),
+                        var r = A(e),
+                            i = A(n),
                             a = h(r);
                         if (r === i) return a.collection();
                         if (null == m[r * u + i]) return t.collection();
                         var o, s = t.collection(),
                             l = r;
                         for (s.merge(a); r !== i;) l = r, r = m[r * u + i], o = b[l * u + r], s.merge(o), s.merge(h(r));
                         return s
                     }
                 }
             }
         },
-        ut = Xe({
+        ct = We({
             weight: function(e) {
                 return 1
             },
             directed: !1,
             root: null
         }),
-        ct = {
+        dt = {
             bellmanFord: function(e) {
                 var t = this,
-                    n = ut(e),
+                    n = ct(e),
                     r = n.weight,
                     i = n.directed,
                     a = n.root,
                     o = r,
                     s = this,
                     l = this.cy(),
                     u = this.byGroup(),
                     c = u.edges,
                     d = u.nodes,
                     h = d.length,
-                    p = new Ue,
-                    g = !1,
+                    p = new Ze,
+                    f = !1,
                     v = [];
                 a = l.collection(a)[0], c.unmergeBy((function(e) {
                     return e.isLoop()
                 }));
                 for (var y = c.length, m = function(e) {
                         var t = p.get(e.id());
                         return t || (t = {}, p.set(e.id(), t)), t
                     }, b = function(e) {
-                        return (f(e) ? l.$(e) : e)[0]
+                        return (g(e) ? l.$(e) : e)[0]
                     }, x = 0; x < h; x++) {
                     var w = d[x],
                         E = m(w);
                     w.same(a) ? E.dist = 0 : E.dist = 1 / 0, E.pred = null, E.edge = null
                 }
                 for (var k = !1, C = function(e, t, n, r, i, a) {
                         var o = r.dist + a;
@@ -1280,24 +1281,24 @@
                             N = m(_);
                         C(T, 0, D, B, N, M), i || C(_, 0, D, N, B, M)
                     }
                     if (!k) break
                 }
                 if (k)
                     for (var z = [], I = 0; I < y; I++) {
-                        var L = c[I],
-                            A = L.source(),
-                            O = L.target(),
-                            R = o(L),
-                            V = m(A).dist,
+                        var A = c[I],
+                            L = A.source(),
+                            O = A.target(),
+                            R = o(A),
+                            V = m(L).dist,
                             F = m(O).dist;
                         if (V + R < F || !i && F + R < V) {
-                            if (g || (Ve("Graph contains a negative weight cycle for Bellman-Ford"), g = !0), !1 === e.findNegativeWeightCycles) break;
+                            if (f || (Fe("Graph contains a negative weight cycle for Bellman-Ford"), f = !0), !1 === e.findNegativeWeightCycles) break;
                             var j = [];
-                            V + R < F && j.push(A), !i && F + R < V && j.push(O);
+                            V + R < F && j.push(L), !i && F + R < V && j.push(O);
                             for (var q = j.length, Y = 0; Y < q; Y++) {
                                 var X = j[Y],
                                     W = [X];
                                 W.push(m(X).edge);
                                 for (var H = m(X).pred; - 1 === W.indexOf(H);) W.push(H), W.push(m(H).edge), H = m(H).pred;
                                 for (var K = (W = W.slice(W.indexOf(H)))[0].id(), G = 0, U = 2; U < W.length; U += 2) W[U].id() < K && (K = W[U].id(), G = U);
                                 (W = W.slice(G).concat(W.slice(0, G))).push(W[0]);
@@ -1318,69 +1319,69 @@
                                 u = l.edge,
                                 c = l.pred;
                             if (i.unshift(o[0]), o.same(n) && i.length > 0) break;
                             null != u && i.unshift(u), o = c
                         }
                         return s.spawn(i)
                     },
-                    hasNegativeWeightCycle: g,
+                    hasNegativeWeightCycle: f,
                     negativeWeightCycles: v
                 }
             }
         },
-        dt = Math.sqrt(2),
-        ht = function(e, t, n) {
-            0 === n.length && Oe("Karger-Stein must be run on a connected (sub)graph");
+        ht = Math.sqrt(2),
+        pt = function(e, t, n) {
+            0 === n.length && Re("Karger-Stein must be run on a connected (sub)graph");
             for (var r = n[e], i = r[1], a = r[2], o = t[i], s = t[a], l = n, u = l.length - 1; u >= 0; u--) {
                 var c = l[u],
                     d = c[1],
                     h = c[2];
                 (t[d] === o && t[h] === s || t[d] === s && t[h] === o) && l.splice(u, 1)
             }
             for (var p = 0; p < l.length; p++) {
                 var f = l[p];
                 f[1] === s ? (l[p] = f.slice(), l[p][1] = o) : f[2] === s && (l[p] = f.slice(), l[p][2] = o)
             }
             for (var g = 0; g < t.length; g++) t[g] === s && (t[g] = o);
             return l
         },
-        pt = function(e, t, n, r) {
+        ft = function(e, t, n, r) {
             for (; n > r;) {
                 var i = Math.floor(Math.random() * t.length);
-                t = ht(i, e, t), n--
+                t = pt(i, e, t), n--
             }
             return t
         },
-        ft = {
+        gt = {
             kargerStein: function() {
                 var e = this,
                     t = this.byGroup(),
                     n = t.nodes,
                     r = t.edges;
                 r.unmergeBy((function(e) {
                     return e.isLoop()
                 }));
                 var i = n.length,
                     a = r.length,
                     o = Math.ceil(Math.pow(Math.log(i) / Math.LN2, 2)),
-                    s = Math.floor(i / dt);
+                    s = Math.floor(i / ht);
                 if (!(i < 2)) {
                     for (var l = [], u = 0; u < a; u++) {
                         var c = r[u];
                         l.push([u, n.indexOf(c.source()), n.indexOf(c.target())])
                     }
                     for (var d = 1 / 0, h = [], p = new Array(i), f = new Array(i), g = new Array(i), v = function(e, t) {
                             for (var n = 0; n < i; n++) t[n] = e[n]
                         }, y = 0; y <= o; y++) {
                         for (var m = 0; m < i; m++) f[m] = m;
-                        var b = pt(f, l.slice(), i, s),
+                        var b = ft(f, l.slice(), i, s),
                             x = b.slice();
                         v(f, g);
-                        var w = pt(f, b, s, 2),
-                            E = pt(g, x, s, 2);
+                        var w = ft(f, b, s, 2),
+                            E = ft(g, x, s, 2);
                         w.length <= E.length && w.length < d ? (d = w.length, h = w, v(f, p)) : E.length <= w.length && E.length < d && (d = E.length, h = E, v(g, p))
                     }
                     for (var k = this.spawn(h.map((function(e) {
                             return r[e[0]]
                         }))), C = this.spawn(), S = this.spawn(), P = p[0], D = 0; D < p.length; D++) {
                         var T = p[D],
                             _ = n[D];
@@ -1398,70 +1399,70 @@
                     return {
                         cut: k,
                         components: B,
                         partition1: C,
                         partition2: S
                     }
                 }
-                Oe("At least 2 nodes are required for Karger-Stein algorithm")
+                Re("At least 2 nodes are required for Karger-Stein algorithm")
             }
         },
-        gt = function(e, t, n) {
+        vt = function(e, t, n) {
             return {
                 x: e.x * t + n.x,
                 y: e.y * t + n.y
             }
         },
-        vt = function(e, t, n) {
+        yt = function(e, t, n) {
             return {
                 x: (e.x - n.x) / t,
                 y: (e.y - n.y) / t
             }
         },
-        yt = function(e) {
+        mt = function(e) {
             return {
                 x: e[0],
                 y: e[1]
             }
         },
-        mt = function(e, t) {
+        bt = function(e, t) {
             return Math.atan2(t, e) - Math.PI / 2
         },
-        bt = Math.log2 || function(e) {
+        xt = Math.log2 || function(e) {
             return Math.log(e) / Math.log(2)
         },
-        xt = function(e) {
+        wt = function(e) {
             return e > 0 ? 1 : e < 0 ? -1 : 0
         },
-        wt = function(e, t) {
-            return Math.sqrt(Et(e, t))
-        },
         Et = function(e, t) {
+            return Math.sqrt(kt(e, t))
+        },
+        kt = function(e, t) {
             var n = t.x - e.x,
                 r = t.y - e.y;
             return n * n + r * r
         },
-        kt = function(e) {
+        Ct = function(e) {
             for (var t = e.length, n = 0, r = 0; r < t; r++) n += e[r];
             for (var i = 0; i < t; i++) e[i] = e[i] / n;
             return e
         },
-        Ct = function(e, t, n, r) {
+        St = function(e, t, n, r) {
             return (1 - r) * (1 - r) * e + 2 * (1 - r) * r * t + r * r * n
         },
-        St = function(e, t, n, r) {
+        Pt = function(e, t, n, r) {
             return {
-                x: Ct(e.x, t.x, n.x, r),
-                y: Ct(e.y, t.y, n.y, r)
+                x: St(e.x, t.x, n.x, r),
+                y: St(e.y, t.y, n.y, r)
             }
         },
-        Pt = function(e, t, n) {
+        Dt = function(e, t, n) {
             return Math.max(e, Math.min(n, t))
         },
-        Dt = function(e) {
+        Tt = function(e) {
             if (null == e) return {
                 x1: 1 / 0,
                 y1: 1 / 0,
                 x2: -1 / 0,
                 y2: -1 / 0,
                 w: 0,
                 h: 0
@@ -1481,148 +1482,171 @@
                     x2: e.x1 + e.w,
                     y2: e.y1 + e.h,
                     w: e.w,
                     h: e.h
                 }
             }
         },
-        Tt = function(e, t) {
+        _t = function(e, t) {
             e.x1 = Math.min(e.x1, t.x1), e.x2 = Math.max(e.x2, t.x2), e.w = e.x2 - e.x1, e.y1 = Math.min(e.y1, t.y1), e.y2 = Math.max(e.y2, t.y2), e.h = e.y2 - e.y1
         },
-        _t = function(e, t, n) {
+        Mt = function(e, t, n) {
             e.x1 = Math.min(e.x1, t), e.x2 = Math.max(e.x2, t), e.w = e.x2 - e.x1, e.y1 = Math.min(e.y1, n), e.y2 = Math.max(e.y2, n), e.h = e.y2 - e.y1
         },
-        Mt = function(e) {
+        Bt = function(e) {
             var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0;
             return e.x1 -= t, e.x2 += t, e.y1 -= t, e.y2 += t, e.w = e.x2 - e.x1, e.h = e.y2 - e.y1, e
         },
-        Bt = function(e) {
+        Nt = function(e) {
             var t, n, r, i, o = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : [0];
             if (1 === o.length) t = n = r = i = o[0];
             else if (2 === o.length) t = r = o[0], i = n = o[1];
             else if (4 === o.length) {
                 var s = a(o, 4);
                 t = s[0], n = s[1], r = s[2], i = s[3]
             }
             return e.x1 -= i, e.x2 += n, e.y1 -= t, e.y2 += r, e.w = e.x2 - e.x1, e.h = e.y2 - e.y1, e
         },
-        Nt = function(e, t) {
+        zt = function(e, t) {
             e.x1 = t.x1, e.y1 = t.y1, e.x2 = t.x2, e.y2 = t.y2, e.w = e.x2 - e.x1, e.h = e.y2 - e.y1
         },
-        zt = function(e, t) {
+        It = function(e, t) {
             return !(e.x1 > t.x2) && (!(t.x1 > e.x2) && (!(e.x2 < t.x1) && (!(t.x2 < e.x1) && (!(e.y2 < t.y1) && (!(t.y2 < e.y1) && (!(e.y1 > t.y2) && !(t.y1 > e.y2)))))))
         },
-        It = function(e, t, n) {
+        At = function(e, t, n) {
             return e.x1 <= t && t <= e.x2 && e.y1 <= n && n <= e.y2
         },
         Lt = function(e, t) {
-            return It(e, t.x1, t.y1) && It(e, t.x2, t.y2)
-        },
-        At = function(e, t, n, r, i, a, o) {
-            var s, l = en(i, a),
-                u = i / 2,
-                c = a / 2,
-                d = r - c - o;
-            if ((s = Gt(e, t, n, r, n - u + l - o, d, n + u - l + o, d, !1)).length > 0) return s;
-            var h = n + u + o;
-            if ((s = Gt(e, t, n, r, h, r - c + l - o, h, r + c - l + o, !1)).length > 0) return s;
-            var p = r + c + o;
-            if ((s = Gt(e, t, n, r, n - u + l - o, p, n + u - l + o, p, !1)).length > 0) return s;
-            var f, g = n - u - o;
-            if ((s = Gt(e, t, n, r, g, r - c + l - o, g, r + c - l + o, !1)).length > 0) return s;
-            var v = n - u + l,
-                y = r - c + l;
-            if ((f = Ht(e, t, n, r, v, y, l + o)).length > 0 && f[0] <= v && f[1] <= y) return [f[0], f[1]];
-            var m = n + u - l,
-                b = r - c + l;
-            if ((f = Ht(e, t, n, r, m, b, l + o)).length > 0 && f[0] >= m && f[1] <= b) return [f[0], f[1]];
-            var x = n + u - l,
-                w = r + c - l;
-            if ((f = Ht(e, t, n, r, x, w, l + o)).length > 0 && f[0] >= x && f[1] >= w) return [f[0], f[1]];
-            var E = n - u + l,
-                k = r + c - l;
-            return (f = Ht(e, t, n, r, E, k, l + o)).length > 0 && f[0] <= E && f[1] >= k ? [f[0], f[1]] : []
+            return At(e, t.x1, t.y1) && At(e, t.x2, t.y2)
         },
         Ot = function(e, t, n, r, i, a, o) {
+            var s, l, u = arguments.length > 7 && void 0 !== arguments[7] ? arguments[7] : "auto",
+                c = "auto" === u ? tn(i, a) : u,
+                d = i / 2,
+                h = a / 2,
+                p = (c = Math.min(c, d, h)) !== d,
+                f = c !== h;
+            if (p) {
+                var g = n - d + c - o,
+                    v = r - h - o,
+                    y = n + d - c + o,
+                    m = v;
+                if ((s = Ut(e, t, n, r, g, v, y, m, !1)).length > 0) return s
+            }
+            if (f) {
+                var b = n + d + o,
+                    x = r - h + c - o,
+                    w = b,
+                    E = r + h - c + o;
+                if ((s = Ut(e, t, n, r, b, x, w, E, !1)).length > 0) return s
+            }
+            if (p) {
+                var k = n - d + c - o,
+                    C = r + h + o,
+                    S = n + d - c + o,
+                    P = C;
+                if ((s = Ut(e, t, n, r, k, C, S, P, !1)).length > 0) return s
+            }
+            if (f) {
+                var D = n - d - o,
+                    T = r - h + c - o,
+                    _ = D,
+                    M = r + h - c + o;
+                if ((s = Ut(e, t, n, r, D, T, _, M, !1)).length > 0) return s
+            }
+            var B = n - d + c,
+                N = r - h + c;
+            if ((l = Kt(e, t, n, r, B, N, c + o)).length > 0 && l[0] <= B && l[1] <= N) return [l[0], l[1]];
+            var z = n + d - c,
+                I = r - h + c;
+            if ((l = Kt(e, t, n, r, z, I, c + o)).length > 0 && l[0] >= z && l[1] <= I) return [l[0], l[1]];
+            var A = n + d - c,
+                L = r + h - c;
+            if ((l = Kt(e, t, n, r, A, L, c + o)).length > 0 && l[0] >= A && l[1] >= L) return [l[0], l[1]];
+            var O = n - d + c,
+                R = r + h - c;
+            return (l = Kt(e, t, n, r, O, R, c + o)).length > 0 && l[0] <= O && l[1] >= R ? [l[0], l[1]] : []
+        },
+        Rt = function(e, t, n, r, i, a, o) {
             var s = o,
                 l = Math.min(n, i),
                 u = Math.max(n, i),
                 c = Math.min(r, a),
                 d = Math.max(r, a);
             return l - s <= e && e <= u + s && c - s <= t && t <= d + s
         },
-        Rt = function(e, t, n, r, i, a, o, s, l) {
+        Vt = function(e, t, n, r, i, a, o, s, l) {
             var u = Math.min(n, o, i) - l,
                 c = Math.max(n, o, i) + l,
                 d = Math.min(r, s, a) - l,
                 h = Math.max(r, s, a) + l;
             return !(e < u || e > c || t < d || t > h)
         },
-        Vt = function(e, t, n, r, i, a, o, s) {
+        Ft = function(e, t, n, r, i, a, o, s) {
             var l = [];
             ! function(e, t, n, r, i) {
                 var a, o, s, l, u, c, d, h;
                 0 === e && (e = 1e-5), s = -27 * (r /= e) + (t /= e) * (9 * (n /= e) - t * t * 2), a = (o = (3 * n - t * t) / 9) * o * o + (s /= 54) * s, i[1] = 0, d = t / 3, a > 0 ? (u = (u = s + Math.sqrt(a)) < 0 ? -Math.pow(-u, 1 / 3) : Math.pow(u, 1 / 3), c = (c = s - Math.sqrt(a)) < 0 ? -Math.pow(-c, 1 / 3) : Math.pow(c, 1 / 3), i[0] = -d + u + c, d += (u + c) / 2, i[4] = i[2] = -d, d = Math.sqrt(3) * (-c + u) / 2, i[3] = d, i[5] = -d) : (i[5] = i[3] = 0, 0 === a ? (h = s < 0 ? -Math.pow(-s, 1 / 3) : Math.pow(s, 1 / 3), i[0] = 2 * h - d, i[4] = i[2] = -(h + d)) : (l = (o = -o) * o * o, l = Math.acos(s / Math.sqrt(l)), h = 2 * Math.sqrt(o), i[0] = -d + h * Math.cos(l / 3), i[2] = -d + h * Math.cos((l + 2 * Math.PI) / 3), i[4] = -d + h * Math.cos((l + 4 * Math.PI) / 3)))
             }(1 * n * n - 4 * n * i + 2 * n * o + 4 * i * i - 4 * i * o + o * o + r * r - 4 * r * a + 2 * r * s + 4 * a * a - 4 * a * s + s * s, 9 * n * i - 3 * n * n - 3 * n * o - 6 * i * i + 3 * i * o + 9 * r * a - 3 * r * r - 3 * r * s - 6 * a * a + 3 * a * s, 3 * n * n - 6 * n * i + n * o - n * e + 2 * i * i + 2 * i * e - o * e + 3 * r * r - 6 * r * a + r * s - r * t + 2 * a * a + 2 * a * t - s * t, 1 * n * i - n * n + n * e - i * e + r * a - r * r + r * t - a * t, l);
             for (var u = [], c = 0; c < 6; c += 2) Math.abs(l[c + 1]) < 1e-7 && l[c] >= 0 && l[c] <= 1 && u.push(l[c]);
             u.push(1), u.push(0);
             for (var d, h, p, f = -1, g = 0; g < u.length; g++) d = Math.pow(1 - u[g], 2) * n + 2 * (1 - u[g]) * u[g] * i + u[g] * u[g] * o, h = Math.pow(1 - u[g], 2) * r + 2 * (1 - u[g]) * u[g] * a + u[g] * u[g] * s, p = Math.pow(d - e, 2) + Math.pow(h - t, 2), f >= 0 ? p < f && (f = p) : f = p;
             return f
         },
-        Ft = function(e, t, n, r, i, a) {
+        jt = function(e, t, n, r, i, a) {
             var o = [e - n, t - r],
                 s = [i - n, a - r],
                 l = s[0] * s[0] + s[1] * s[1],
                 u = o[0] * o[0] + o[1] * o[1],
                 c = o[0] * s[0] + o[1] * s[1],
                 d = c * c / l;
             return c < 0 ? u : d > l ? (e - i) * (e - i) + (t - a) * (t - a) : u - d
         },
-        jt = function(e, t, n) {
+        qt = function(e, t, n) {
             for (var r, i, a, o, s = 0, l = 0; l < n.length / 2; l++)
                 if (r = n[2 * l], i = n[2 * l + 1], l + 1 < n.length / 2 ? (a = n[2 * (l + 1)], o = n[2 * (l + 1) + 1]) : (a = n[2 * (l + 1 - n.length / 2)], o = n[2 * (l + 1 - n.length / 2) + 1]), r == e && a == e);
                 else {
                     if (!(r >= e && e >= a || r <= e && e <= a)) continue;
                     (e - r) / (a - r) * (o - i) + i > t && s++
                 } return s % 2 != 0
         },
-        qt = function(e, t, n, r, i, a, o, s, l) {
+        Yt = function(e, t, n, r, i, a, o, s, l) {
             var u, c = new Array(n.length);
             null != s[0] ? (u = Math.atan(s[1] / s[0]), s[0] < 0 ? u += Math.PI / 2 : u = -u - Math.PI / 2) : u = s;
             for (var d, h = Math.cos(-u), p = Math.sin(-u), f = 0; f < c.length / 2; f++) c[2 * f] = a / 2 * (n[2 * f] * h - n[2 * f + 1] * p), c[2 * f + 1] = o / 2 * (n[2 * f + 1] * h + n[2 * f] * p), c[2 * f] += r, c[2 * f + 1] += i;
             if (l > 0) {
-                var g = Xt(c, -l);
-                d = Yt(g)
+                var g = Wt(c, -l);
+                d = Xt(g)
             } else d = c;
-            return jt(e, t, d)
+            return qt(e, t, d)
         },
-        Yt = function(e) {
+        Xt = function(e) {
             for (var t, n, r, i, a, o, s, l, u = new Array(e.length / 2), c = 0; c < e.length / 4; c++) {
                 t = e[4 * c], n = e[4 * c + 1], r = e[4 * c + 2], i = e[4 * c + 3], c < e.length / 4 - 1 ? (a = e[4 * (c + 1)], o = e[4 * (c + 1) + 1], s = e[4 * (c + 1) + 2], l = e[4 * (c + 1) + 3]) : (a = e[0], o = e[1], s = e[2], l = e[3]);
-                var d = Gt(t, n, r, i, a, o, s, l, !0);
+                var d = Ut(t, n, r, i, a, o, s, l, !0);
                 u[2 * c] = d[0], u[2 * c + 1] = d[1]
             }
             return u
         },
-        Xt = function(e, t) {
+        Wt = function(e, t) {
             for (var n, r, i, a, o = new Array(2 * e.length), s = 0; s < e.length / 2; s++) {
                 n = e[2 * s], r = e[2 * s + 1], s < e.length / 2 - 1 ? (i = e[2 * (s + 1)], a = e[2 * (s + 1) + 1]) : (i = e[0], a = e[1]);
                 var l = a - r,
                     u = -(i - n),
                     c = Math.sqrt(l * l + u * u),
                     d = l / c,
                     h = u / c;
                 o[4 * s] = n + d * t, o[4 * s + 1] = r + h * t, o[4 * s + 2] = i + d * t, o[4 * s + 3] = a + h * t
             }
             return o
         },
-        Wt = function(e, t, n, r, i, a, o) {
+        Ht = function(e, t, n, r, i, a, o) {
             return e -= i, t -= a, (e /= n / 2 + o) * e + (t /= r / 2 + o) * t <= 1
         },
-        Ht = function(e, t, n, r, i, a, o) {
+        Kt = function(e, t, n, r, i, a, o) {
             var s = [n - e, r - t],
                 l = [e - i, t - a],
                 u = s[0] * s[0] + s[1] * s[1],
                 c = 2 * (l[0] * s[0] + l[1] * s[1]),
                 d = c * c - 4 * u * (l[0] * l[0] + l[1] * l[1] - o * o);
             if (d < 0) return [];
             var h = (-c + Math.sqrt(d)) / (2 * u),
@@ -1631,96 +1655,96 @@
                 g = Math.max(h, p),
                 v = [];
             if (f >= 0 && f <= 1 && v.push(f), g >= 0 && g <= 1 && v.push(g), 0 === v.length) return [];
             var y = v[0] * s[0] + e,
                 m = v[0] * s[1] + t;
             return v.length > 1 ? v[0] == v[1] ? [y, m] : [y, m, v[1] * s[0] + e, v[1] * s[1] + t] : [y, m]
         },
-        Kt = function(e, t, n) {
+        Gt = function(e, t, n) {
             return t <= e && e <= n || n <= e && e <= t ? e : e <= t && t <= n || n <= t && t <= e ? t : n
         },
-        Gt = function(e, t, n, r, i, a, o, s, l) {
+        Ut = function(e, t, n, r, i, a, o, s, l) {
             var u = e - i,
                 c = n - e,
                 d = o - i,
                 h = t - a,
                 p = r - t,
                 f = s - a,
                 g = d * h - f * u,
                 v = c * h - p * u,
                 y = f * c - d * p;
             if (0 !== y) {
                 var m = g / y,
                     b = v / y;
                 return -.001 <= m && m <= 1.001 && -.001 <= b && b <= 1.001 || l ? [e + m * c, t + m * p] : []
             }
-            return 0 === g || 0 === v ? Kt(e, n, o) === o ? [o, s] : Kt(e, n, i) === i ? [i, a] : Kt(i, o, n) === n ? [n, r] : [] : []
+            return 0 === g || 0 === v ? Gt(e, n, o) === o ? [o, s] : Gt(e, n, i) === i ? [i, a] : Gt(i, o, n) === n ? [n, r] : [] : []
         },
-        Ut = function(e, t, n, r, i, a, o, s) {
+        Zt = function(e, t, n, r, i, a, o, s) {
             var l, u, c, d, h, p, f = [],
                 g = new Array(n.length),
                 v = !0;
             if (null == a && (v = !1), v) {
                 for (var y = 0; y < g.length / 2; y++) g[2 * y] = n[2 * y] * a + r, g[2 * y + 1] = n[2 * y + 1] * o + i;
                 if (s > 0) {
-                    var m = Xt(g, -s);
-                    u = Yt(m)
+                    var m = Wt(g, -s);
+                    u = Xt(m)
                 } else u = g
             } else u = n;
-            for (var b = 0; b < u.length / 2; b++) c = u[2 * b], d = u[2 * b + 1], b < u.length / 2 - 1 ? (h = u[2 * (b + 1)], p = u[2 * (b + 1) + 1]) : (h = u[0], p = u[1]), 0 !== (l = Gt(e, t, r, i, c, d, h, p)).length && f.push(l[0], l[1]);
+            for (var b = 0; b < u.length / 2; b++) c = u[2 * b], d = u[2 * b + 1], b < u.length / 2 - 1 ? (h = u[2 * (b + 1)], p = u[2 * (b + 1) + 1]) : (h = u[0], p = u[1]), 0 !== (l = Ut(e, t, r, i, c, d, h, p)).length && f.push(l[0], l[1]);
             return f
         },
-        Zt = function(e, t, n) {
+        $t = function(e, t, n) {
             var r = [e[0] - t[0], e[1] - t[1]],
                 i = Math.sqrt(r[0] * r[0] + r[1] * r[1]),
                 a = (i - n) / i;
             return a < 0 && (a = 1e-5), [t[0] + a * r[0], t[1] + a * r[1]]
         },
-        $t = function(e, t) {
-            var n = Jt(e, t);
-            return n = Qt(n)
+        Qt = function(e, t) {
+            var n = en(e, t);
+            return n = Jt(n)
         },
-        Qt = function(e) {
+        Jt = function(e) {
             for (var t, n, r = e.length / 2, i = 1 / 0, a = 1 / 0, o = -1 / 0, s = -1 / 0, l = 0; l < r; l++) t = e[2 * l], n = e[2 * l + 1], i = Math.min(i, t), o = Math.max(o, t), a = Math.min(a, n), s = Math.max(s, n);
             for (var u = 2 / (o - i), c = 2 / (s - a), d = 0; d < r; d++) t = e[2 * d] = e[2 * d] * u, n = e[2 * d + 1] = e[2 * d + 1] * c, i = Math.min(i, t), o = Math.max(o, t), a = Math.min(a, n), s = Math.max(s, n);
             if (a < -1)
                 for (var h = 0; h < r; h++) n = e[2 * h + 1] = e[2 * h + 1] + (-1 - a);
             return e
         },
-        Jt = function(e, t) {
+        en = function(e, t) {
             var n = 1 / e * 2 * Math.PI,
                 r = e % 2 == 0 ? Math.PI / 2 + n / 2 : Math.PI / 2;
             r += t;
             for (var i, a = new Array(2 * e), o = 0; o < e; o++) i = o * n + r, a[2 * o] = Math.cos(i), a[2 * o + 1] = Math.sin(-i);
             return a
         },
-        en = function(e, t) {
+        tn = function(e, t) {
             return Math.min(e / 4, t / 4, 8)
         },
-        tn = function(e, t) {
+        nn = function(e, t) {
             return Math.min(e / 10, t / 10, 8)
         },
-        nn = function(e, t) {
+        rn = function(e, t) {
             return {
                 heightOffset: Math.min(15, .05 * t),
                 widthOffset: Math.min(100, .25 * e),
                 ctrlPtOffsetPct: .05
             }
         },
-        rn = Xe({
+        an = We({
             dampingFactor: .8,
             precision: 1e-6,
             iterations: 200,
             weight: function(e) {
                 return 1
             }
         }),
-        an = {
+        on = {
             pageRank: function(e) {
-                for (var t = rn(e), n = t.dampingFactor, r = t.precision, i = t.iterations, a = t.weight, o = this._private.cy, s = this.byGroup(), l = s.nodes, u = s.edges, c = l.length, d = c * c, h = u.length, p = new Array(d), f = new Array(c), g = (1 - n) / c, v = 0; v < c; v++) {
+                for (var t = an(e), n = t.dampingFactor, r = t.precision, i = t.iterations, a = t.weight, o = this._private.cy, s = this.byGroup(), l = s.nodes, u = s.edges, c = l.length, d = c * c, h = u.length, p = new Array(d), f = new Array(c), g = (1 - n) / c, v = 0; v < c; v++) {
                     for (var y = 0; y < c; y++) {
                         p[v * c + y] = 0
                     }
                     f[v] = 0
                 }
                 for (var m = 0; m < h; m++) {
                     var b = u[m],
@@ -1740,79 +1764,79 @@
                         } else
                             for (var T = 0; T < c; T++) {
                                 var _ = T * c + P;
                                 p[_] = p[_] / f[P] + g
                             }
                 for (var M, B = new Array(c), N = new Array(c), z = 0; z < c; z++) B[z] = 1;
                 for (var I = 0; I < i; I++) {
-                    for (var L = 0; L < c; L++) N[L] = 0;
-                    for (var A = 0; A < c; A++)
+                    for (var A = 0; A < c; A++) N[A] = 0;
+                    for (var L = 0; L < c; L++)
                         for (var O = 0; O < c; O++) {
-                            var R = A * c + O;
-                            N[A] += p[R] * B[O]
+                            var R = L * c + O;
+                            N[L] += p[R] * B[O]
                         }
-                    kt(N), M = B, B = N, N = M;
+                    Ct(N), M = B, B = N, N = M;
                     for (var V = 0, F = 0; F < c; F++) {
                         var j = M[F] - B[F];
                         V += j * j
                     }
                     if (V < r) break
                 }
                 return {
                     rank: function(e) {
                         return e = o.collection(e)[0], B[l.indexOf(e)]
                     }
                 }
             }
         },
-        on = Xe({
+        sn = We({
             root: null,
             weight: function(e) {
                 return 1
             },
             directed: !1,
             alpha: 0
         }),
-        sn = {
+        ln = {
             degreeCentralityNormalized: function(e) {
-                e = on(e);
+                e = sn(e);
                 var t = this.cy(),
                     n = this.nodes(),
                     r = n.length;
                 if (e.directed) {
                     for (var i = {}, a = {}, o = 0, s = 0, l = 0; l < r; l++) {
                         var u = n[l],
                             c = u.id();
                         e.root = u;
                         var d = this.degreeCentrality(e);
                         o < d.indegree && (o = d.indegree), s < d.outdegree && (s = d.outdegree), i[c] = d.indegree, a[c] = d.outdegree
                     }
                     return {
                         indegree: function(e) {
-                            return 0 == o ? 0 : (f(e) && (e = t.filter(e)), i[e.id()] / o)
+                            return 0 == o ? 0 : (g(e) && (e = t.filter(e)), i[e.id()] / o)
                         },
                         outdegree: function(e) {
-                            return 0 === s ? 0 : (f(e) && (e = t.filter(e)), a[e.id()] / s)
+                            return 0 === s ? 0 : (g(e) && (e = t.filter(e)), a[e.id()] / s)
                         }
                     }
                 }
-                for (var h = {}, p = 0, g = 0; g < r; g++) {
-                    var v = n[g];
+                for (var h = {}, p = 0, f = 0; f < r; f++) {
+                    var v = n[f];
                     e.root = v;
                     var y = this.degreeCentrality(e);
                     p < y.degree && (p = y.degree), h[v.id()] = y.degree
                 }
                 return {
                     degree: function(e) {
-                        return 0 === p ? 0 : (f(e) && (e = t.filter(e)), h[e.id()] / p)
+                        return 0 === p ? 0 : (g(e) && (e = t.filter(e)), h[e.id()] / p)
                     }
                 }
             },
             degreeCentrality: function(e) {
-                e = on(e);
+                e = sn(e);
                 var t = this.cy(),
                     n = this,
                     r = e,
                     i = r.root,
                     a = r.weight,
                     o = r.directed,
                     s = r.alpha;
@@ -1830,43 +1854,43 @@
                 }
                 for (var y = i.connectedEdges().intersection(n), m = y.length, b = 0, x = 0; x < y.length; x++) b += a(y[x]);
                 return {
                     degree: Math.pow(m, 1 - s) * Math.pow(b, s)
                 }
             }
         };
-    sn.dc = sn.degreeCentrality, sn.dcn = sn.degreeCentralityNormalised = sn.degreeCentralityNormalized;
-    var ln = Xe({
+    ln.dc = ln.degreeCentrality, ln.dcn = ln.degreeCentralityNormalised = ln.degreeCentralityNormalized;
+    var un = We({
             harmonic: !0,
             weight: function() {
                 return 1
             },
             directed: !1,
             root: null
         }),
-        un = {
+        cn = {
             closenessCentralityNormalized: function(e) {
-                for (var t = ln(e), n = t.harmonic, r = t.weight, i = t.directed, a = this.cy(), o = {}, s = 0, l = this.nodes(), u = this.floydWarshall({
+                for (var t = un(e), n = t.harmonic, r = t.weight, i = t.directed, a = this.cy(), o = {}, s = 0, l = this.nodes(), u = this.floydWarshall({
                         weight: r,
                         directed: i
                     }), c = 0; c < l.length; c++) {
                     for (var d = 0, h = l[c], p = 0; p < l.length; p++)
                         if (c !== p) {
-                            var g = u.distance(h, l[p]);
-                            d += n ? 1 / g : g
+                            var f = u.distance(h, l[p]);
+                            d += n ? 1 / f : f
                         } n || (d = 1 / d), s < d && (s = d), o[h.id()] = d
                 }
                 return {
                     closeness: function(e) {
-                        return 0 == s ? 0 : (e = f(e) ? a.filter(e)[0].id() : e.id(), o[e] / s)
+                        return 0 == s ? 0 : (e = g(e) ? a.filter(e)[0].id() : e.id(), o[e] / s)
                     }
                 }
             },
             closenessCentrality: function(e) {
-                var t = ln(e),
+                var t = un(e),
                     n = t.root,
                     r = t.weight,
                     i = t.directed,
                     a = t.harmonic;
                 n = this.filter(n)[0];
                 for (var o = this.dijkstra({
                         root: n,
@@ -1878,32 +1902,32 @@
                         var d = o.distanceTo(c);
                         s += a ? 1 / d : d
                     }
                 }
                 return a ? s : 1 / s
             }
         };
-    un.cc = un.closenessCentrality, un.ccn = un.closenessCentralityNormalised = un.closenessCentralityNormalized;
-    var cn = Xe({
+    cn.cc = cn.closenessCentrality, cn.ccn = cn.closenessCentralityNormalised = cn.closenessCentralityNormalized;
+    var dn = We({
             weight: null,
             directed: !1
         }),
-        dn = {
+        hn = {
             betweennessCentrality: function(e) {
-                for (var t = cn(e), n = t.directed, r = t.weight, i = null != r, a = this.cy(), o = this.nodes(), s = {}, l = {}, u = 0, c = function(e, t) {
+                for (var t = dn(e), n = t.directed, r = t.weight, i = null != r, a = this.cy(), o = this.nodes(), s = {}, l = {}, u = 0, c = function(e, t) {
                         l[e] = t, t > u && (u = t)
                     }, d = function(e) {
                         return l[e]
                     }, h = 0; h < o.length; h++) {
                     var p = o[h],
                         f = p.id();
                     s[f] = n ? p.outgoers().nodes() : p.openNeighborhood().nodes(), c(f, 0)
                 }
                 for (var g = function(e) {
-                        for (var t = o[e].id(), n = [], l = {}, u = {}, h = {}, p = new tt((function(e, t) {
+                        for (var t = o[e].id(), n = [], l = {}, u = {}, h = {}, p = new nt((function(e, t) {
                                 return h[e] - h[t]
                             })), f = 0; f < o.length; f++) {
                             var g = o[f].id();
                             l[g] = [], u[g] = 0, h[g] = 1 / 0
                         }
                         for (u[t] = 1, h[t] = 0, p.push(t); !p.empty();) {
                             var v = p.pop();
@@ -1940,327 +1964,330 @@
                         var t = a.collection(e).id();
                         return d(t) / u
                     }
                 };
                 return y.betweennessNormalised = y.betweennessNormalized, y
             }
         };
-    dn.bc = dn.betweennessCentrality;
-    var hn = Xe({
+    hn.bc = hn.betweennessCentrality;
+    var pn = We({
             expandFactor: 2,
             inflateFactor: 2,
             multFactor: 1,
             maxIterations: 20,
             attributes: [function(e) {
                 return 1
             }]
         }),
-        pn = function(e, t) {
+        fn = function(e, t) {
             for (var n = 0, r = 0; r < t.length; r++) n += t[r](e);
             return n
         },
-        fn = function(e, t) {
+        gn = function(e, t) {
             for (var n, r = 0; r < t; r++) {
                 n = 0;
                 for (var i = 0; i < t; i++) n += e[i * t + r];
                 for (var a = 0; a < t; a++) e[a * t + r] = e[a * t + r] / n
             }
         },
-        gn = function(e, t, n) {
+        vn = function(e, t, n) {
             for (var r = new Array(n * n), i = 0; i < n; i++) {
                 for (var a = 0; a < n; a++) r[i * n + a] = 0;
                 for (var o = 0; o < n; o++)
                     for (var s = 0; s < n; s++) r[i * n + s] += e[i * n + o] * t[o * n + s]
             }
             return r
         },
-        vn = function(e, t, n) {
-            for (var r = e.slice(0), i = 1; i < n; i++) e = gn(e, r, t);
+        yn = function(e, t, n) {
+            for (var r = e.slice(0), i = 1; i < n; i++) e = vn(e, r, t);
             return e
         },
-        yn = function(e, t, n) {
+        mn = function(e, t, n) {
             for (var r = new Array(t * t), i = 0; i < t * t; i++) r[i] = Math.pow(e[i], n);
-            return fn(r, t), r
+            return gn(r, t), r
         },
-        mn = function(e, t, n, r) {
+        bn = function(e, t, n, r) {
             for (var i = 0; i < n; i++) {
                 if (Math.round(e[i] * Math.pow(10, r)) / Math.pow(10, r) !== Math.round(t[i] * Math.pow(10, r)) / Math.pow(10, r)) return !1
             }
             return !0
         },
-        bn = function(e, t) {
+        xn = function(e, t) {
             for (var n = 0; n < e.length; n++)
                 if (!t[n] || e[n].id() !== t[n].id()) return !1;
             return !0
         },
-        xn = function(e) {
+        wn = function(e) {
             for (var t = this.nodes(), n = this.edges(), r = this.cy(), i = function(e) {
-                    return hn(e)
+                    return pn(e)
                 }(e), a = {}, o = 0; o < t.length; o++) a[t[o].id()] = o;
             for (var s, l = t.length, u = l * l, c = new Array(u), d = 0; d < u; d++) c[d] = 0;
             for (var h = 0; h < n.length; h++) {
                 var p = n[h],
                     f = a[p.source().id()],
                     g = a[p.target().id()],
-                    v = pn(p, i.attributes);
+                    v = fn(p, i.attributes);
                 c[f * l + g] += v, c[g * l + f] += v
             }! function(e, t, n) {
                 for (var r = 0; r < t; r++) e[r * t + r] = n
-            }(c, l, i.multFactor), fn(c, l);
-            for (var y = !0, m = 0; y && m < i.maxIterations;) y = !1, s = vn(c, l, i.expandFactor), c = yn(s, l, i.inflateFactor), mn(c, s, u, 4) || (y = !0), m++;
+            }(c, l, i.multFactor), gn(c, l);
+            for (var y = !0, m = 0; y && m < i.maxIterations;) y = !1, s = yn(c, l, i.expandFactor), c = mn(s, l, i.inflateFactor), bn(c, s, u, 4) || (y = !0), m++;
             var b = function(e, t, n, r) {
                 for (var i = [], a = 0; a < t; a++) {
                     for (var o = [], s = 0; s < t; s++) Math.round(1e3 * e[a * t + s]) / 1e3 > 0 && o.push(n[s]);
                     0 !== o.length && i.push(r.collection(o))
                 }
                 return i
             }(c, l, t, r);
             return b = function(e) {
                 for (var t = 0; t < e.length; t++)
-                    for (var n = 0; n < e.length; n++) t != n && bn(e[t], e[n]) && e.splice(n, 1);
+                    for (var n = 0; n < e.length; n++) t != n && xn(e[t], e[n]) && e.splice(n, 1);
                 return e
             }(b)
         },
-        wn = {
-            markovClustering: xn,
-            mcl: xn
+        En = {
+            markovClustering: wn,
+            mcl: wn
         },
-        En = function(e) {
+        kn = function(e) {
             return e
         },
-        kn = function(e, t) {
+        Cn = function(e, t) {
             return Math.abs(t - e)
         },
-        Cn = function(e, t, n) {
-            return e + kn(t, n)
-        },
         Sn = function(e, t, n) {
+            return e + Cn(t, n)
+        },
+        Pn = function(e, t, n) {
             return e + Math.pow(n - t, 2)
         },
-        Pn = function(e) {
+        Dn = function(e) {
             return Math.sqrt(e)
         },
-        Dn = function(e, t, n) {
-            return Math.max(e, kn(t, n))
+        Tn = function(e, t, n) {
+            return Math.max(e, Cn(t, n))
         },
-        Tn = function(e, t, n, r, i) {
-            for (var a = arguments.length > 5 && void 0 !== arguments[5] ? arguments[5] : En, o = r, s = 0; s < e; s++) o = i(o, t(s), n(s));
+        _n = function(e, t, n, r, i) {
+            for (var a = arguments.length > 5 && void 0 !== arguments[5] ? arguments[5] : kn, o = r, s = 0; s < e; s++) o = i(o, t(s), n(s));
             return a(o)
         },
-        _n = {
+        Mn = {
             euclidean: function(e, t, n) {
-                return e >= 2 ? Tn(e, t, n, 0, Sn, Pn) : Tn(e, t, n, 0, Cn)
+                return e >= 2 ? _n(e, t, n, 0, Pn, Dn) : _n(e, t, n, 0, Sn)
             },
             squaredEuclidean: function(e, t, n) {
-                return Tn(e, t, n, 0, Sn)
+                return _n(e, t, n, 0, Pn)
             },
             manhattan: function(e, t, n) {
-                return Tn(e, t, n, 0, Cn)
+                return _n(e, t, n, 0, Sn)
             },
             max: function(e, t, n) {
-                return Tn(e, t, n, -1 / 0, Dn)
+                return _n(e, t, n, -1 / 0, Tn)
             }
         };
 
-    function Mn(e, t, n, r, i, a) {
+    function Bn(e, t, n, r, i, a) {
         var o;
-        return o = g(e) ? e : _n[e] || _n.euclidean, 0 === t && g(e) ? o(i, a) : o(t, n, r, i, a)
+        return o = v(e) ? e : Mn[e] || Mn.euclidean, 0 === t && v(e) ? o(i, a) : o(t, n, r, i, a)
     }
-    _n["squared-euclidean"] = _n.squaredEuclidean, _n.squaredeuclidean = _n.squaredEuclidean;
-    var Bn = Xe({
+    Mn["squared-euclidean"] = Mn.squaredEuclidean, Mn.squaredeuclidean = Mn.squaredEuclidean;
+    var Nn = We({
             k: 2,
             m: 2,
             sensitivityThreshold: 1e-4,
             distance: "euclidean",
             maxIterations: 10,
             attributes: [],
             testMode: !1,
             testCentroids: null
         }),
-        Nn = function(e) {
-            return Bn(e)
+        zn = function(e) {
+            return Nn(e)
         },
-        zn = function(e, t, n, r, i) {
+        In = function(e, t, n, r, i) {
             var a = "kMedoids" !== i ? function(e) {
                     return n[e]
                 } : function(e) {
                     return r[e](n)
                 },
                 o = n,
                 s = t;
-            return Mn(e, r.length, a, (function(e) {
+            return Bn(e, r.length, a, (function(e) {
                 return r[e](t)
             }), o, s)
         },
-        In = function(e, t, n) {
+        An = function(e, t, n) {
             for (var r = n.length, i = new Array(r), a = new Array(r), o = new Array(t), s = null, l = 0; l < r; l++) i[l] = e.min(n[l]).value, a[l] = e.max(n[l]).value;
             for (var u = 0; u < t; u++) {
                 s = [];
                 for (var c = 0; c < r; c++) s[c] = Math.random() * (a[c] - i[c]) + i[c];
                 o[u] = s
             }
             return o
         },
         Ln = function(e, t, n, r, i) {
             for (var a = 1 / 0, o = 0, s = 0; s < t.length; s++) {
-                var l = zn(n, e, t[s], r, i);
+                var l = In(n, e, t[s], r, i);
                 l < a && (a = l, o = s)
             }
             return o
         },
-        An = function(e, t, n) {
+        On = function(e, t, n) {
             for (var r = [], i = null, a = 0; a < t.length; a++) n[(i = t[a]).id()] === e && r.push(i);
             return r
         },
-        On = function(e, t, n) {
+        Rn = function(e, t, n) {
+            return Math.abs(t - e) <= n
+        },
+        Vn = function(e, t, n) {
             for (var r = 0; r < e.length; r++)
                 for (var i = 0; i < e[r].length; i++) {
                     if (Math.abs(e[r][i] - t[r][i]) > n) return !1
                 }
             return !0
         },
-        Rn = function(e, t, n) {
+        Fn = function(e, t, n) {
             for (var r = 0; r < n; r++)
                 if (e === t[r]) return !0;
             return !1
         },
-        Vn = function(e, t) {
+        jn = function(e, t) {
             var n = new Array(t);
             if (e.length < 50)
                 for (var r = 0; r < t; r++) {
-                    for (var i = e[Math.floor(Math.random() * e.length)]; Rn(i, n, r);) i = e[Math.floor(Math.random() * e.length)];
+                    for (var i = e[Math.floor(Math.random() * e.length)]; Fn(i, n, r);) i = e[Math.floor(Math.random() * e.length)];
                     n[r] = i
                 } else
                     for (var a = 0; a < t; a++) n[a] = e[Math.floor(Math.random() * e.length)];
             return n
         },
-        Fn = function(e, t, n) {
-            for (var r = 0, i = 0; i < t.length; i++) r += zn("manhattan", t[i], e, n, "kMedoids");
+        qn = function(e, t, n) {
+            for (var r = 0, i = 0; i < t.length; i++) r += In("manhattan", t[i], e, n, "kMedoids");
             return r
         },
-        jn = function(e, t, n, r, i) {
+        Yn = function(e, t, n, r, i) {
             for (var a, o, s = 0; s < t.length; s++)
                 for (var l = 0; l < e.length; l++) r[s][l] = Math.pow(n[s][l], i.m);
             for (var u = 0; u < e.length; u++)
                 for (var c = 0; c < i.attributes.length; c++) {
                     a = 0, o = 0;
                     for (var d = 0; d < t.length; d++) a += r[d][u] * i.attributes[c](t[d]), o += r[d][u];
                     e[u][c] = a / o
                 }
         },
-        qn = function(e, t, n, r, i) {
+        Xn = function(e, t, n, r, i) {
             for (var a = 0; a < e.length; a++) t[a] = e[a].slice();
             for (var o, s, l, u = 2 / (i.m - 1), c = 0; c < n.length; c++)
                 for (var d = 0; d < r.length; d++) {
                     o = 0;
-                    for (var h = 0; h < n.length; h++) s = zn(i.distance, r[d], n[c], i.attributes, "cmeans"), l = zn(i.distance, r[d], n[h], i.attributes, "cmeans"), o += Math.pow(s / l, u);
+                    for (var h = 0; h < n.length; h++) s = In(i.distance, r[d], n[c], i.attributes, "cmeans"), l = In(i.distance, r[d], n[h], i.attributes, "cmeans"), o += Math.pow(s / l, u);
                     e[d][c] = 1 / o
                 }
         },
-        Yn = function(e) {
+        Wn = function(e) {
             var t, n, r, i, a = this.cy(),
                 o = this.nodes(),
-                s = Nn(e);
+                s = zn(e);
             r = new Array(o.length);
             for (var l = 0; l < o.length; l++) r[l] = new Array(s.k);
             n = new Array(o.length);
             for (var u = 0; u < o.length; u++) n[u] = new Array(s.k);
             for (var c = 0; c < o.length; c++) {
                 for (var d = 0, h = 0; h < s.k; h++) n[c][h] = Math.random(), d += n[c][h];
                 for (var p = 0; p < s.k; p++) n[c][p] = n[c][p] / d
             }
             t = new Array(s.k);
             for (var f = 0; f < s.k; f++) t[f] = new Array(s.attributes.length);
             i = new Array(o.length);
             for (var g = 0; g < o.length; g++) i[g] = new Array(s.k);
-            for (var v = !0, y = 0; v && y < s.maxIterations;) v = !1, jn(t, o, n, i, s), qn(n, r, t, o, s), On(n, r, s.sensitivityThreshold) || (v = !0), y++;
+            for (var v = !0, y = 0; v && y < s.maxIterations;) v = !1, Yn(t, o, n, i, s), Xn(n, r, t, o, s), Vn(n, r, s.sensitivityThreshold) || (v = !0), y++;
             return {
                 clusters: function(e, t, n, r) {
                     for (var i, a, o = new Array(n.k), s = 0; s < o.length; s++) o[s] = [];
                     for (var l = 0; l < t.length; l++) {
                         i = -1 / 0, a = -1;
                         for (var u = 0; u < t[0].length; u++) t[l][u] > i && (i = t[l][u], a = u);
                         o[a].push(e[l])
                     }
                     for (var c = 0; c < o.length; c++) o[c] = r.collection(o[c]);
                     return o
                 }(o, n, s, a),
                 degreeOfMembership: n
             }
         },
-        Xn = {
+        Hn = {
             kMeans: function(t) {
                 var n, r = this.cy(),
                     i = this.nodes(),
                     a = null,
-                    o = Nn(t),
+                    o = zn(t),
                     s = new Array(o.k),
                     l = {};
-                o.testMode ? "number" == typeof o.testCentroids ? (o.testCentroids, n = In(i, o.k, o.attributes)) : n = "object" === e(o.testCentroids) ? o.testCentroids : In(i, o.k, o.attributes) : n = In(i, o.k, o.attributes);
-                for (var u, c, d, h = !0, p = 0; h && p < o.maxIterations;) {
-                    for (var f = 0; f < i.length; f++) l[(a = i[f]).id()] = Ln(a, n, o.distance, o.attributes, "kMeans");
-                    h = !1;
-                    for (var g = 0; g < o.k; g++) {
-                        var v = An(g, i, l);
-                        if (0 !== v.length) {
-                            for (var y = o.attributes.length, m = n[g], b = new Array(y), x = new Array(y), w = 0; w < y; w++) {
-                                x[w] = 0;
-                                for (var E = 0; E < v.length; E++) a = v[E], x[w] += o.attributes[w](a);
-                                b[w] = x[w] / v.length, u = b[w], c = m[w], d = o.sensitivityThreshold, Math.abs(c - u) <= d || (h = !0)
+                o.testMode ? "number" == typeof o.testCentroids ? (o.testCentroids, n = An(i, o.k, o.attributes)) : n = "object" === e(o.testCentroids) ? o.testCentroids : An(i, o.k, o.attributes) : n = An(i, o.k, o.attributes);
+                for (var u = !0, c = 0; u && c < o.maxIterations;) {
+                    for (var d = 0; d < i.length; d++) l[(a = i[d]).id()] = Ln(a, n, o.distance, o.attributes, "kMeans");
+                    u = !1;
+                    for (var h = 0; h < o.k; h++) {
+                        var p = On(h, i, l);
+                        if (0 !== p.length) {
+                            for (var f = o.attributes.length, g = n[h], v = new Array(f), y = new Array(f), m = 0; m < f; m++) {
+                                y[m] = 0;
+                                for (var b = 0; b < p.length; b++) a = p[b], y[m] += o.attributes[m](a);
+                                v[m] = y[m] / p.length, Rn(v[m], g[m], o.sensitivityThreshold) || (u = !0)
                             }
-                            n[g] = b, s[g] = r.collection(v)
+                            n[h] = v, s[h] = r.collection(p)
                         }
                     }
-                    p++
+                    c++
                 }
                 return s
             },
             kMedoids: function(t) {
                 var n, r, i = this.cy(),
                     a = this.nodes(),
                     o = null,
-                    s = Nn(t),
+                    s = zn(t),
                     l = new Array(s.k),
                     u = {},
                     c = new Array(s.k);
-                s.testMode ? "number" == typeof s.testCentroids || (n = "object" === e(s.testCentroids) ? s.testCentroids : Vn(a, s.k)) : n = Vn(a, s.k);
+                s.testMode ? "number" == typeof s.testCentroids || (n = "object" === e(s.testCentroids) ? s.testCentroids : jn(a, s.k)) : n = jn(a, s.k);
                 for (var d = !0, h = 0; d && h < s.maxIterations;) {
                     for (var p = 0; p < a.length; p++) u[(o = a[p]).id()] = Ln(o, n, s.distance, s.attributes, "kMedoids");
                     d = !1;
                     for (var f = 0; f < n.length; f++) {
-                        var g = An(f, a, u);
+                        var g = On(f, a, u);
                         if (0 !== g.length) {
-                            c[f] = Fn(n[f], g, s.attributes);
-                            for (var v = 0; v < g.length; v++)(r = Fn(g[v], g, s.attributes)) < c[f] && (c[f] = r, n[f] = g[v], d = !0);
+                            c[f] = qn(n[f], g, s.attributes);
+                            for (var v = 0; v < g.length; v++)(r = qn(g[v], g, s.attributes)) < c[f] && (c[f] = r, n[f] = g[v], d = !0);
                             l[f] = i.collection(g)
                         }
                     }
                     h++
                 }
                 return l
             },
-            fuzzyCMeans: Yn,
-            fcm: Yn
+            fuzzyCMeans: Wn,
+            fcm: Wn
         },
-        Wn = Xe({
+        Kn = We({
             distance: "euclidean",
             linkage: "min",
             mode: "threshold",
             threshold: 1 / 0,
             addDendrogram: !1,
             dendrogramDepth: 0,
             attributes: []
         }),
-        Hn = {
+        Gn = {
             single: "min",
             complete: "max"
         },
-        Kn = function(e, t, n, r, i) {
+        Un = function(e, t, n, r, i) {
             for (var a, o = 0, s = 1 / 0, l = i.attributes, u = function(e, t) {
-                    return Mn(i.distance, l.length, (function(t) {
+                    return Bn(i.distance, l.length, (function(t) {
                         return l[t](e)
                     }), (function(e) {
                         return l[e](t)
                     }), e, t)
                 }, c = 0; c < e.length; c++) {
                 var d = e[c].key,
                     h = n[d][r[d]];
@@ -2290,24 +2317,24 @@
                     }
                     r[b] = x
                 }
                 e[m].index = m
             }
             return f.key = g.key = f.index = g.index = null, !0
         },
-        Gn = function e(t, n, r) {
+        Zn = function e(t, n, r) {
             t && (t.value ? n.push(t.value) : (t.left && e(t.left, n), t.right && e(t.right, n)))
         },
-        Un = function(e) {
+        $n = function(e) {
             for (var t = this.cy(), n = this.nodes(), r = function(e) {
-                    var t = Wn(e),
-                        n = Hn[t.linkage];
+                    var t = Kn(e),
+                        n = Gn[t.linkage];
                     return null != n && (t.linkage = n), t
                 }(e), i = r.attributes, a = function(e, t) {
-                    return Mn(r.distance, i.length, (function(t) {
+                    return Bn(r.distance, i.length, (function(t) {
                         return i[t](e)
                     }), (function(e) {
                         return i[e](t)
                     }), e, t)
                 }, o = [], s = [], l = [], u = [], c = 0; c < n.length; c++) {
                 var d = {
                     value: "dendrogram" === r.mode ? n[c] : [n[c]],
@@ -2317,21 +2344,21 @@
                 o[c] = d, u[c] = d, s[c] = [], l[c] = 0
             }
             for (var h = 0; h < o.length; h++)
                 for (var p = 0; p <= h; p++) {
                     var f = void 0;
                     f = "dendrogram" === r.mode ? h === p ? 1 / 0 : a(o[h].value, o[p].value) : h === p ? 1 / 0 : a(o[h].value[0], o[p].value[0]), s[h][p] = f, s[p][h] = f, f < s[h][l[h]] && (l[h] = p)
                 }
-            for (var g, v = Kn(o, u, s, l, r); v;) v = Kn(o, u, s, l, r);
+            for (var g, v = Un(o, u, s, l, r); v;) v = Un(o, u, s, l, r);
             return "dendrogram" === r.mode ? (g = function e(t, n, r) {
                 if (!t) return [];
                 var i = [],
                     a = [],
                     o = [];
-                return 0 === n ? (t.left && Gn(t.left, i), t.right && Gn(t.right, a), o = i.concat(a), [r.collection(o)]) : 1 === n ? t.value ? [r.collection(t.value)] : (t.left && Gn(t.left, i), t.right && Gn(t.right, a), [r.collection(i), r.collection(a)]) : t.value ? [r.collection(t.value)] : (t.left && (i = e(t.left, n - 1, r)), t.right && (a = e(t.right, n - 1, r)), i.concat(a))
+                return 0 === n ? (t.left && Zn(t.left, i), t.right && Zn(t.right, a), o = i.concat(a), [r.collection(o)]) : 1 === n ? t.value ? [r.collection(t.value)] : (t.left && Zn(t.left, i), t.right && Zn(t.right, a), [r.collection(i), r.collection(a)]) : t.value ? [r.collection(t.value)] : (t.left && (i = e(t.left, n - 1, r)), t.right && (a = e(t.right, n - 1, r)), i.concat(a))
             }(o[0], r.dendrogramDepth, t), r.addDendrogram && function e(t, n) {
                 if (!t) return "";
                 if (t.left && t.right) {
                     var r = e(t.left, n),
                         i = e(t.right, n),
                         a = n.add({
                             group: "nodes",
@@ -2354,37 +2381,37 @@
                     }), a.id()
                 }
                 return t.value ? t.value.id() : void 0
             }(o[0], t)) : (g = new Array(o.length), o.forEach((function(e, n) {
                 e.key = e.index = null, g[n] = t.collection(e.value)
             }))), g
         },
-        Zn = {
-            hierarchicalClustering: Un,
-            hca: Un
+        Qn = {
+            hierarchicalClustering: $n,
+            hca: $n
         },
-        $n = Xe({
+        Jn = We({
             distance: "euclidean",
             preference: "median",
             damping: .8,
             maxIterations: 1e3,
             minIterations: 100,
             attributes: []
         }),
-        Qn = function(e, t, n, r) {
+        er = function(e, t, n, r) {
             var i = function(e, t) {
                 return r[t](e)
             };
-            return -Mn(e, r.length, (function(e) {
+            return -Bn(e, r.length, (function(e) {
                 return i(t, e)
             }), (function(e) {
                 return i(n, e)
             }), t, n)
         },
-        Jn = function(e, t) {
+        tr = function(e, t) {
             return "median" === t ? function(e) {
                 var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0,
                     n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : e.length,
                     r = !(arguments.length > 3 && void 0 !== arguments[3]) || arguments[3],
                     i = !(arguments.length > 4 && void 0 !== arguments[4]) || arguments[4],
                     a = !(arguments.length > 5 && void 0 !== arguments[5]) || arguments[5];
                 r ? e = e.slice(t, n) : (n < e.length && e.splice(n, e.length - n), t > 0 && e.splice(0, t));
@@ -2414,60 +2441,60 @@
                 for (var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0, n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : e.length, r = -1 / 0, i = t; i < n; i++) {
                     var a = e[i];
                     isFinite(a) && (r = Math.max(a, r))
                 }
                 return r
             }(e) : t
         },
-        er = function(e, t, n) {
+        nr = function(e, t, n) {
             for (var r = [], i = 0; i < e; i++) {
                 for (var a = -1, o = -1 / 0, s = 0; s < n.length; s++) {
                     var l = n[s];
                     t[i * e + l] > o && (a = l, o = t[i * e + l])
                 }
                 a > 0 && r.push(a)
             }
             for (var u = 0; u < n.length; u++) r[n[u]] = n[u];
             return r
         },
-        tr = function(e) {
+        rr = function(e) {
             for (var t, n, r, i, a, o, s = this.cy(), l = this.nodes(), u = function(e) {
                     var t = e.damping,
                         n = e.preference;
-                    .5 <= t && t < 1 || Oe("Damping must range on [0.5, 1).  Got: ".concat(t));
+                    .5 <= t && t < 1 || Re("Damping must range on [0.5, 1).  Got: ".concat(t));
                     var r = ["median", "mean", "min", "max"];
                     return r.some((function(e) {
                         return e === n
-                    })) || m(n) || Oe("Preference must be one of [".concat(r.map((function(e) {
+                    })) || b(n) || Re("Preference must be one of [".concat(r.map((function(e) {
                         return "'".concat(e, "'")
-                    })).join(", "), "] or a number.  Got: ").concat(n)), $n(e)
+                    })).join(", "), "] or a number.  Got: ").concat(n)), Jn(e)
                 }(e), c = {}, d = 0; d < l.length; d++) c[l[d].id()] = d;
             n = (t = l.length) * t, r = new Array(n);
             for (var h = 0; h < n; h++) r[h] = -1 / 0;
             for (var p = 0; p < t; p++)
-                for (var f = 0; f < t; f++) p !== f && (r[p * t + f] = Qn(u.distance, l[p], l[f], u.attributes));
-            i = Jn(r, u.preference);
+                for (var f = 0; f < t; f++) p !== f && (r[p * t + f] = er(u.distance, l[p], l[f], u.attributes));
+            i = tr(r, u.preference);
             for (var g = 0; g < t; g++) r[g * t + g] = i;
             a = new Array(n);
             for (var v = 0; v < n; v++) a[v] = 0;
             o = new Array(n);
             for (var y = 0; y < n; y++) o[y] = 0;
-            for (var b = new Array(t), x = new Array(t), w = new Array(t), E = 0; E < t; E++) b[E] = 0, x[E] = 0, w[E] = 0;
+            for (var m = new Array(t), x = new Array(t), w = new Array(t), E = 0; E < t; E++) m[E] = 0, x[E] = 0, w[E] = 0;
             for (var k, C = new Array(t * u.minIterations), S = 0; S < C.length; S++) C[S] = 0;
             for (k = 0; k < u.maxIterations; k++) {
                 for (var P = 0; P < t; P++) {
-                    for (var D = -1 / 0, T = -1 / 0, _ = -1, M = 0, B = 0; B < t; B++) b[B] = a[P * t + B], (M = o[P * t + B] + r[P * t + B]) >= D ? (T = D, D = M, _ = B) : M > T && (T = M);
-                    for (var N = 0; N < t; N++) a[P * t + N] = (1 - u.damping) * (r[P * t + N] - D) + u.damping * b[N];
-                    a[P * t + _] = (1 - u.damping) * (r[P * t + _] - T) + u.damping * b[_]
+                    for (var D = -1 / 0, T = -1 / 0, _ = -1, M = 0, B = 0; B < t; B++) m[B] = a[P * t + B], (M = o[P * t + B] + r[P * t + B]) >= D ? (T = D, D = M, _ = B) : M > T && (T = M);
+                    for (var N = 0; N < t; N++) a[P * t + N] = (1 - u.damping) * (r[P * t + N] - D) + u.damping * m[N];
+                    a[P * t + _] = (1 - u.damping) * (r[P * t + _] - T) + u.damping * m[_]
                 }
                 for (var z = 0; z < t; z++) {
-                    for (var I = 0, L = 0; L < t; L++) b[L] = o[L * t + z], x[L] = Math.max(0, a[L * t + z]), I += x[L];
+                    for (var I = 0, A = 0; A < t; A++) m[A] = o[A * t + z], x[A] = Math.max(0, a[A * t + z]), I += x[A];
                     I -= x[z], x[z] = a[z * t + z], I += x[z];
-                    for (var A = 0; A < t; A++) o[A * t + z] = (1 - u.damping) * Math.min(0, I - x[A]) + u.damping * b[A];
-                    o[z * t + z] = (1 - u.damping) * (I - x[z]) + u.damping * b[z]
+                    for (var L = 0; L < t; L++) o[L * t + z] = (1 - u.damping) * Math.min(0, I - x[L]) + u.damping * m[L];
+                    o[z * t + z] = (1 - u.damping) * (I - x[z]) + u.damping * m[z]
                 }
                 for (var O = 0, R = 0; R < t; R++) {
                     var V = o[R * t + R] + a[R * t + R] > 0 ? 1 : 0;
                     C[k % u.minIterations * t + R] = V, O += V
                 }
                 if (O > 0 && (k >= u.minIterations - 1 || k == u.maxIterations - 1)) {
                     for (var F = 0, j = 0; j < t; j++) {
@@ -2478,40 +2505,40 @@
                     if (F === t) break
                 }
             }
             for (var Y = function(e, t, n) {
                     for (var r = [], i = 0; i < e; i++) t[i * e + i] + n[i * e + i] > 0 && r.push(i);
                     return r
                 }(t, a, o), X = function(e, t, n) {
-                    for (var r = er(e, t, n), i = 0; i < n.length; i++) {
+                    for (var r = nr(e, t, n), i = 0; i < n.length; i++) {
                         for (var a = [], o = 0; o < r.length; o++) r[o] === n[i] && a.push(o);
                         for (var s = -1, l = -1 / 0, u = 0; u < a.length; u++) {
                             for (var c = 0, d = 0; d < a.length; d++) c += t[a[d] * e + a[u]];
                             c > l && (s = u, l = c)
                         }
                         n[i] = a[s]
                     }
-                    return r = er(e, t, n)
+                    return r = nr(e, t, n)
                 }(t, r, Y), W = {}, H = 0; H < Y.length; H++) W[Y[H]] = [];
             for (var K = 0; K < l.length; K++) {
                 var G = X[c[l[K].id()]];
                 null != G && W[G].push(l[K])
             }
             for (var U = new Array(Y.length), Z = 0; Z < Y.length; Z++) U[Z] = s.collection(W[Y[Z]]);
             return U
         },
-        nr = {
-            affinityPropagation: tr,
-            ap: tr
+        ir = {
+            affinityPropagation: rr,
+            ap: rr
         },
-        rr = Xe({
+        ar = We({
             root: void 0,
             directed: !1
         }),
-        ir = function() {
+        or = function() {
             var e = this,
                 t = {},
                 n = 0,
                 r = 0,
                 i = [],
                 a = [],
                 o = {},
@@ -2554,15 +2581,15 @@
                 return e.getElementById(t)
             }));
             return {
                 cut: e.spawn(l),
                 components: i
             }
         },
-        ar = function() {
+        sr = function() {
             var e = this,
                 t = {},
                 n = 0,
                 r = [],
                 i = [],
                 a = e.spawn(e);
             return e.forEach((function(o) {
@@ -2588,30 +2615,30 @@
                     }(s)
                 }
             })), {
                 cut: a,
                 components: r
             }
         },
-        or = {};
-    [et, rt, it, ot, lt, ct, ft, an, sn, un, dn, wn, Xn, Zn, nr, {
+        lr = {};
+    [tt, it, at, st, ut, dt, gt, on, ln, cn, hn, En, Hn, Qn, ir, {
         hierholzer: function(e) {
-            if (!y(e)) {
+            if (!m(e)) {
                 var t = arguments;
                 e = {
                     root: t[0],
                     directed: t[1]
                 }
             }
-            var n, r, i, a = rr(e),
+            var n, r, i, a = ar(e),
                 o = a.root,
                 s = a.directed,
                 l = this,
                 u = !1;
-            o && (i = f(o) ? this.filter(o)[0].id() : o[0].id());
+            o && (i = g(o) ? this.filter(o)[0].id() : o[0].id());
             var c = {},
                 d = {};
             s ? l.forEach((function(e) {
                 var t = e.id();
                 if (e.isNode()) {
                     var i = e.indegree(!0),
                         a = e.outdegree(!0),
@@ -2645,88 +2672,88 @@
                     for (var t, n, r, i = e, a = [e]; c[i].length;) t = c[i].shift(), n = d[t][0], i != (r = d[t][1]) ? (c[r] = c[r].filter((function(e) {
                         return e != t
                     })), i = r) : s || i == n || (c[n] = c[n].filter((function(e) {
                         return e != t
                     })), i = n), a.unshift(t), a.unshift(i);
                     return a
                 },
-                g = [],
+                f = [],
                 v = [];
-            for (v = p(i); 1 != v.length;) 0 == c[v[0]].length ? (g.unshift(l.getElementById(v.shift())), g.unshift(l.getElementById(v.shift()))) : v = p(v.shift()).concat(v);
-            for (var m in g.unshift(l.getElementById(v.shift())), c)
-                if (c[m].length) return h;
-            return h.found = !0, h.trail = this.spawn(g, !0), h
+            for (v = p(i); 1 != v.length;) 0 == c[v[0]].length ? (f.unshift(l.getElementById(v.shift())), f.unshift(l.getElementById(v.shift()))) : v = p(v.shift()).concat(v);
+            for (var y in f.unshift(l.getElementById(v.shift())), c)
+                if (c[y].length) return h;
+            return h.found = !0, h.trail = this.spawn(f, !0), h
         }
     }, {
-        hopcroftTarjanBiconnected: ir,
-        htbc: ir,
-        htb: ir,
-        hopcroftTarjanBiconnectedComponents: ir
+        hopcroftTarjanBiconnected: or,
+        htbc: or,
+        htb: or,
+        hopcroftTarjanBiconnectedComponents: or
     }, {
-        tarjanStronglyConnected: ar,
-        tsc: ar,
-        tscc: ar,
-        tarjanStronglyConnectedComponents: ar
+        tarjanStronglyConnected: sr,
+        tsc: sr,
+        tscc: sr,
+        tarjanStronglyConnectedComponents: sr
     }].forEach((function(e) {
-        I(or, e)
+        A(lr, e)
     }));
     /*!
       Embeddable Minimum Strictly-Compliant Promises/A+ 1.1.1 Thenable
       Copyright (c) 2013-2014 Ralf S. Engelschall (http://engelschall.com)
       Licensed under The MIT License (http://opensource.org/licenses/MIT)
       */
-    var sr = function e(t) {
+    var ur = function e(t) {
         if (!(this instanceof e)) return new e(t);
         this.id = "Thenable/1.0.7", this.state = 0, this.fulfillValue = void 0, this.rejectReason = void 0, this.onFulfilled = [], this.onRejected = [], this.proxy = {
             then: this.then.bind(this)
         }, "function" == typeof t && t.call(this, this.fulfill.bind(this), this.reject.bind(this))
     };
-    sr.prototype = {
+    ur.prototype = {
         fulfill: function(e) {
-            return lr(this, 1, "fulfillValue", e)
+            return cr(this, 1, "fulfillValue", e)
         },
         reject: function(e) {
-            return lr(this, 2, "rejectReason", e)
+            return cr(this, 2, "rejectReason", e)
         },
         then: function(e, t) {
-            var n = new sr;
-            return this.onFulfilled.push(dr(e, n, "fulfill")), this.onRejected.push(dr(t, n, "reject")), ur(this), n.proxy
+            var n = new ur;
+            return this.onFulfilled.push(pr(e, n, "fulfill")), this.onRejected.push(pr(t, n, "reject")), dr(this), n.proxy
         }
     };
-    var lr = function(e, t, n, r) {
-            return 0 === e.state && (e.state = t, e[n] = r, ur(e)), e
+    var cr = function(e, t, n, r) {
+            return 0 === e.state && (e.state = t, e[n] = r, dr(e)), e
         },
-        ur = function(e) {
-            1 === e.state ? cr(e, "onFulfilled", e.fulfillValue) : 2 === e.state && cr(e, "onRejected", e.rejectReason)
+        dr = function(e) {
+            1 === e.state ? hr(e, "onFulfilled", e.fulfillValue) : 2 === e.state && hr(e, "onRejected", e.rejectReason)
         },
-        cr = function(e, t, n) {
+        hr = function(e, t, n) {
             if (0 !== e[t].length) {
                 var r = e[t];
                 e[t] = [];
                 var i = function() {
                     for (var e = 0; e < r.length; e++) r[e](n)
                 };
                 "function" == typeof setImmediate ? setImmediate(i) : setTimeout(i, 0)
             }
         },
-        dr = function(e, t, n) {
+        pr = function(e, t, n) {
             return function(r) {
                 if ("function" != typeof e) t[n].call(t, r);
                 else {
                     var i;
                     try {
                         i = e(r)
                     } catch (e) {
                         return void t.reject(e)
                     }
-                    hr(t, i)
+                    fr(t, i)
                 }
             }
         },
-        hr = function t(n, r) {
+        fr = function t(n, r) {
             if (n !== r && n.proxy !== r) {
                 var i;
                 if ("object" === e(r) && null !== r || "function" == typeof r) try {
                     i = r.then
                 } catch (e) {
                     return void n.reject(e)
                 }
@@ -2741,44 +2768,44 @@
                         }))
                     } catch (e) {
                         a || n.reject(e)
                     }
                 }
             } else n.reject(new TypeError("cannot resolve promise with itself"))
         };
-    sr.all = function(e) {
-        return new sr((function(t, n) {
+    ur.all = function(e) {
+        return new ur((function(t, n) {
             for (var r = new Array(e.length), i = 0, a = function(n, a) {
                     r[n] = a, ++i === e.length && t(r)
                 }, o = 0; o < e.length; o++) ! function(t) {
                 var r = e[t];
                 null != r && null != r.then ? r.then((function(e) {
                     a(t, e)
                 }), (function(e) {
                     n(e)
                 })) : a(t, r)
             }(o)
         }))
-    }, sr.resolve = function(e) {
-        return new sr((function(t, n) {
+    }, ur.resolve = function(e) {
+        return new ur((function(t, n) {
             t(e)
         }))
-    }, sr.reject = function(e) {
-        return new sr((function(t, n) {
+    }, ur.reject = function(e) {
+        return new ur((function(t, n) {
             n(e)
         }))
     };
-    var pr = "undefined" != typeof Promise ? Promise : sr,
-        fr = function(e, t, n) {
-            var r = k(e),
+    var gr = "undefined" != typeof Promise ? Promise : ur,
+        vr = function(e, t, n) {
+            var r = C(e),
                 i = !r,
-                a = this._private = I({
+                a = this._private = A({
                     duration: 1e3
                 }, t, n);
-            if (a.target = e, a.style = a.style || a.css, a.started = !1, a.playing = !1, a.hooked = !1, a.applying = !1, a.progress = 0, a.completes = [], a.frames = [], a.complete && g(a.complete) && a.completes.push(a.complete), i) {
+            if (a.target = e, a.style = a.style || a.css, a.started = !1, a.playing = !1, a.hooked = !1, a.applying = !1, a.progress = 0, a.completes = [], a.frames = [], a.complete && v(a.complete) && a.completes.push(a.complete), i) {
                 var o = e.position();
                 a.startPosition = a.startPosition || {
                     x: o.x,
                     y: o.y
                 }, a.startStyle = a.startStyle || e.cy().style().getAnimationStartStyle(e, a.style)
             }
             if (r) {
@@ -2786,24 +2813,24 @@
                 a.startPan = {
                     x: s.x,
                     y: s.y
                 }, a.startZoom = e.zoom()
             }
             this.length = 1, this[0] = this
         },
-        gr = fr.prototype;
-    I(gr, {
+        yr = vr.prototype;
+    A(yr, {
         instanceString: function() {
             return "animation"
         },
         hook: function() {
             var e = this._private;
             if (!e.hooked) {
                 var t = e.target._private.animation;
-                (e.queue ? t.queue : t.current).push(this), x(e.target) && e.target.cy().addToAnimationPool(e.target), e.hooked = !0
+                (e.queue ? t.queue : t.current).push(this), w(e.target) && e.target.cy().addToAnimationPool(e.target), e.hooked = !0
             }
             return this
         },
         play: function() {
             var e = this._private;
             return 1 === e.progress && (e.progress = 0), e.playing = !0, e.started = !1, e.stopped = !1, this.hook(), this
         },
@@ -2867,22 +2894,22 @@
                     t = n.frames;
                     break;
                 default:
                 case "complete":
                 case "completed":
                     t = n.completes
             }
-            return new pr((function(e, n) {
+            return new gr((function(e, n) {
                 t.push((function() {
                     e()
                 }))
             }))
         }
-    }), gr.complete = gr.completed, gr.run = gr.play, gr.running = gr.playing;
-    var vr = {
+    }), yr.complete = yr.completed, yr.run = yr.play, yr.running = yr.playing;
+    var mr = {
             animated: function() {
                 return function() {
                     var e = void 0 !== this.length ? this : [this];
                     if (!(this._private.cy || this).styleEnabled()) return !1;
                     var t = e[0];
                     return t ? t._private.animation.current.length > 0 : void 0
                 }
@@ -2920,27 +2947,27 @@
                     var n = void 0 !== this.length,
                         r = n ? this : [this],
                         i = this._private.cy || this,
                         a = !n,
                         o = !a;
                     if (!i.styleEnabled()) return this;
                     var s = i.style();
-                    if (e = I({}, e, t), 0 === Object.keys(e).length) return new fr(r[0], e);
+                    if (e = A({}, e, t), 0 === Object.keys(e).length) return new vr(r[0], e);
                     switch (void 0 === e.duration && (e.duration = 400), e.duration) {
                         case "slow":
                             e.duration = 600;
                             break;
                         case "fast":
                             e.duration = 200
                     }
                     if (o && (e.style = s.getPropsList(e.style || e.css), e.css = void 0), o && null != e.renderedPosition) {
                         var l = e.renderedPosition,
                             u = i.pan(),
                             c = i.zoom();
-                        e.position = vt(l, c, u)
+                        e.position = yt(l, c, u)
                     }
                     if (a && null != e.panBy) {
                         var d = e.panBy,
                             h = i.pan();
                         e.pan = {
                             x: h.x + d.x,
                             y: h.y + d.y
@@ -2952,26 +2979,26 @@
                         null != f && (e.pan = f)
                     }
                     if (a && null != e.fit) {
                         var g = e.fit,
                             v = i.getFitViewport(g.eles || g.boundingBox, g.padding);
                         null != v && (e.pan = v.pan, e.zoom = v.zoom)
                     }
-                    if (a && y(e.zoom)) {
-                        var m = i.getZoomedViewport(e.zoom);
-                        null != m ? (m.zoomed && (e.zoom = m.zoom), m.panned && (e.pan = m.pan)) : e.zoom = null
+                    if (a && m(e.zoom)) {
+                        var y = i.getZoomedViewport(e.zoom);
+                        null != y ? (y.zoomed && (e.zoom = y.zoom), y.panned && (e.pan = y.pan)) : e.zoom = null
                     }
-                    return new fr(r[0], e)
+                    return new vr(r[0], e)
                 }
             },
             animate: function() {
                 return function(e, t) {
                     var n = void 0 !== this.length ? this : [this];
                     if (!(this._private.cy || this).styleEnabled()) return this;
-                    t && (e = I({}, e, t));
+                    t && (e = A({}, e, t));
                     for (var r = 0; r < n.length; r++) {
                         var i = n[r],
                             a = i.animated() && (void 0 === e.queue || e.queue);
                         i.animation(e, a ? {
                             queue: !0
                         } : void 0).play()
                     }
@@ -2990,295 +3017,295 @@
                         }
                         e && (a.animation.queue = []), t || (a.animation.current = [])
                     }
                     return r.notify("draw"), this
                 }
             }
         },
-        yr = Array.isArray,
-        mr = /\.|\[(?:[^[\]]*|(["'])(?:(?!\1)[^\\]|\\.)*?\1)\]/,
-        br = /^\w*$/;
-    var xr = function(e, t) {
-        if (yr(e)) return !1;
+        br = Array.isArray,
+        xr = /\.|\[(?:[^[\]]*|(["'])(?:(?!\1)[^\\]|\\.)*?\1)\]/,
+        wr = /^\w*$/;
+    var Er = function(e, t) {
+        if (br(e)) return !1;
         var n = typeof e;
-        return !("number" != n && "symbol" != n && "boolean" != n && null != e && !oe(e)) || (br.test(e) || !mr.test(e) || null != t && e in Object(t))
+        return !("number" != n && "symbol" != n && "boolean" != n && null != e && !se(e)) || (wr.test(e) || !xr.test(e) || null != t && e in Object(t))
     };
-    var wr, Er = function(e) {
-            if (!V(e)) return !1;
-            var t = ie(e);
+    var kr, Cr = function(e) {
+            if (!F(e)) return !1;
+            var t = ae(e);
             return "[object Function]" == t || "[object GeneratorFunction]" == t || "[object AsyncFunction]" == t || "[object Proxy]" == t
         },
-        kr = Y["__core-js_shared__"],
-        Cr = (wr = /[^.]+$/.exec(kr && kr.keys && kr.keys.IE_PROTO || "")) ? "Symbol(src)_1." + wr : "";
-    var Sr = function(e) {
-            return !!Cr && Cr in e
-        },
-        Pr = Function.prototype.toString;
+        Sr = X["__core-js_shared__"],
+        Pr = (kr = /[^.]+$/.exec(Sr && Sr.keys && Sr.keys.IE_PROTO || "")) ? "Symbol(src)_1." + kr : "";
     var Dr = function(e) {
+            return !!Pr && Pr in e
+        },
+        Tr = Function.prototype.toString;
+    var _r = function(e) {
             if (null != e) {
                 try {
-                    return Pr.call(e)
+                    return Tr.call(e)
                 } catch (e) {}
                 try {
                     return e + ""
                 } catch (e) {}
             }
             return ""
         },
-        Tr = /^\[object .+?Constructor\]$/,
-        _r = Function.prototype,
-        Mr = Object.prototype,
-        Br = _r.toString,
-        Nr = Mr.hasOwnProperty,
-        zr = RegExp("^" + Br.call(Nr).replace(/[\\^$.*+?()[\]{}|]/g, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$");
-    var Ir = function(e) {
-        return !(!V(e) || Sr(e)) && (Er(e) ? zr : Tr).test(Dr(e))
+        Mr = /^\[object .+?Constructor\]$/,
+        Br = Function.prototype,
+        Nr = Object.prototype,
+        zr = Br.toString,
+        Ir = Nr.hasOwnProperty,
+        Ar = RegExp("^" + zr.call(Ir).replace(/[\\^$.*+?()[\]{}|]/g, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$");
+    var Lr = function(e) {
+        return !(!F(e) || Dr(e)) && (Cr(e) ? Ar : Mr).test(_r(e))
     };
-    var Lr = function(e, t) {
+    var Or = function(e, t) {
         return null == e ? void 0 : e[t]
     };
-    var Ar = function(e, t) {
-            var n = Lr(e, t);
-            return Ir(n) ? n : void 0
-        },
-        Or = Ar(Object, "create");
-    var Rr = function() {
-        this.__data__ = Or ? Or(null) : {}, this.size = 0
+    var Rr = function(e, t) {
+            var n = Or(e, t);
+            return Lr(n) ? n : void 0
+        },
+        Vr = Rr(Object, "create");
+    var Fr = function() {
+        this.__data__ = Vr ? Vr(null) : {}, this.size = 0
     };
-    var Vr = function(e) {
+    var jr = function(e) {
             var t = this.has(e) && delete this.__data__[e];
             return this.size -= t ? 1 : 0, t
         },
-        Fr = Object.prototype.hasOwnProperty;
-    var jr = function(e) {
+        qr = Object.prototype.hasOwnProperty;
+    var Yr = function(e) {
             var t = this.__data__;
-            if (Or) {
+            if (Vr) {
                 var n = t[e];
                 return "__lodash_hash_undefined__" === n ? void 0 : n
             }
-            return Fr.call(t, e) ? t[e] : void 0
+            return qr.call(t, e) ? t[e] : void 0
         },
-        qr = Object.prototype.hasOwnProperty;
-    var Yr = function(e) {
+        Xr = Object.prototype.hasOwnProperty;
+    var Wr = function(e) {
         var t = this.__data__;
-        return Or ? void 0 !== t[e] : qr.call(t, e)
+        return Vr ? void 0 !== t[e] : Xr.call(t, e)
     };
-    var Xr = function(e, t) {
+    var Hr = function(e, t) {
         var n = this.__data__;
-        return this.size += this.has(e) ? 0 : 1, n[e] = Or && void 0 === t ? "__lodash_hash_undefined__" : t, this
+        return this.size += this.has(e) ? 0 : 1, n[e] = Vr && void 0 === t ? "__lodash_hash_undefined__" : t, this
     };
 
-    function Wr(e) {
+    function Kr(e) {
         var t = -1,
             n = null == e ? 0 : e.length;
         for (this.clear(); ++t < n;) {
             var r = e[t];
             this.set(r[0], r[1])
         }
     }
-    Wr.prototype.clear = Rr, Wr.prototype.delete = Vr, Wr.prototype.get = jr, Wr.prototype.has = Yr, Wr.prototype.set = Xr;
-    var Hr = Wr;
-    var Kr = function() {
+    Kr.prototype.clear = Fr, Kr.prototype.delete = jr, Kr.prototype.get = Yr, Kr.prototype.has = Wr, Kr.prototype.set = Hr;
+    var Gr = Kr;
+    var Ur = function() {
         this.__data__ = [], this.size = 0
     };
-    var Gr = function(e, t) {
+    var Zr = function(e, t) {
         return e === t || e != e && t != t
     };
-    var Ur = function(e, t) {
+    var $r = function(e, t) {
             for (var n = e.length; n--;)
-                if (Gr(e[n][0], t)) return n;
+                if (Zr(e[n][0], t)) return n;
             return -1
         },
-        Zr = Array.prototype.splice;
-    var $r = function(e) {
+        Qr = Array.prototype.splice;
+    var Jr = function(e) {
         var t = this.__data__,
-            n = Ur(t, e);
-        return !(n < 0) && (n == t.length - 1 ? t.pop() : Zr.call(t, n, 1), --this.size, !0)
+            n = $r(t, e);
+        return !(n < 0) && (n == t.length - 1 ? t.pop() : Qr.call(t, n, 1), --this.size, !0)
     };
-    var Qr = function(e) {
+    var ei = function(e) {
         var t = this.__data__,
-            n = Ur(t, e);
+            n = $r(t, e);
         return n < 0 ? void 0 : t[n][1]
     };
-    var Jr = function(e) {
-        return Ur(this.__data__, e) > -1
+    var ti = function(e) {
+        return $r(this.__data__, e) > -1
     };
-    var ei = function(e, t) {
+    var ni = function(e, t) {
         var n = this.__data__,
-            r = Ur(n, e);
+            r = $r(n, e);
         return r < 0 ? (++this.size, n.push([e, t])) : n[r][1] = t, this
     };
 
-    function ti(e) {
+    function ri(e) {
         var t = -1,
             n = null == e ? 0 : e.length;
         for (this.clear(); ++t < n;) {
             var r = e[t];
             this.set(r[0], r[1])
         }
     }
-    ti.prototype.clear = Kr, ti.prototype.delete = $r, ti.prototype.get = Qr, ti.prototype.has = Jr, ti.prototype.set = ei;
-    var ni = ti,
-        ri = Ar(Y, "Map");
-    var ii = function() {
+    ri.prototype.clear = Ur, ri.prototype.delete = Jr, ri.prototype.get = ei, ri.prototype.has = ti, ri.prototype.set = ni;
+    var ii = ri,
+        ai = Rr(X, "Map");
+    var oi = function() {
         this.size = 0, this.__data__ = {
-            hash: new Hr,
-            map: new(ri || ni),
-            string: new Hr
+            hash: new Gr,
+            map: new(ai || ii),
+            string: new Gr
         }
     };
-    var ai = function(e) {
+    var si = function(e) {
         var t = typeof e;
         return "string" == t || "number" == t || "symbol" == t || "boolean" == t ? "__proto__" !== e : null === e
     };
-    var oi = function(e, t) {
+    var li = function(e, t) {
         var n = e.__data__;
-        return ai(t) ? n["string" == typeof t ? "string" : "hash"] : n.map
+        return si(t) ? n["string" == typeof t ? "string" : "hash"] : n.map
     };
-    var si = function(e) {
-        var t = oi(this, e).delete(e);
+    var ui = function(e) {
+        var t = li(this, e).delete(e);
         return this.size -= t ? 1 : 0, t
     };
-    var li = function(e) {
-        return oi(this, e).get(e)
+    var ci = function(e) {
+        return li(this, e).get(e)
     };
-    var ui = function(e) {
-        return oi(this, e).has(e)
+    var di = function(e) {
+        return li(this, e).has(e)
     };
-    var ci = function(e, t) {
-        var n = oi(this, e),
+    var hi = function(e, t) {
+        var n = li(this, e),
             r = n.size;
         return n.set(e, t), this.size += n.size == r ? 0 : 1, this
     };
 
-    function di(e) {
+    function pi(e) {
         var t = -1,
             n = null == e ? 0 : e.length;
         for (this.clear(); ++t < n;) {
             var r = e[t];
             this.set(r[0], r[1])
         }
     }
-    di.prototype.clear = ii, di.prototype.delete = si, di.prototype.get = li, di.prototype.has = ui, di.prototype.set = ci;
-    var hi = di;
+    pi.prototype.clear = oi, pi.prototype.delete = ui, pi.prototype.get = ci, pi.prototype.has = di, pi.prototype.set = hi;
+    var fi = pi;
 
-    function pi(e, t) {
+    function gi(e, t) {
         if ("function" != typeof e || null != t && "function" != typeof t) throw new TypeError("Expected a function");
         var n = function() {
             var r = arguments,
                 i = t ? t.apply(this, r) : r[0],
                 a = n.cache;
             if (a.has(i)) return a.get(i);
             var o = e.apply(this, r);
             return n.cache = a.set(i, o) || a, o
         };
-        return n.cache = new(pi.Cache || hi), n
+        return n.cache = new(gi.Cache || fi), n
     }
-    pi.Cache = hi;
-    var fi = pi;
-    var gi = /[^.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|$))/g,
-        vi = /\\(\\)?/g,
-        yi = function(e) {
-            var t = fi(e, (function(e) {
+    gi.Cache = fi;
+    var vi = gi;
+    var yi = /[^.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|$))/g,
+        mi = /\\(\\)?/g,
+        bi = function(e) {
+            var t = vi(e, (function(e) {
                     return 500 === n.size && n.clear(), e
                 })),
                 n = t.cache;
             return t
         }((function(e) {
             var t = [];
-            return 46 === e.charCodeAt(0) && t.push(""), e.replace(gi, (function(e, n, r, i) {
-                t.push(r ? i.replace(vi, "$1") : n || e)
+            return 46 === e.charCodeAt(0) && t.push(""), e.replace(yi, (function(e, n, r, i) {
+                t.push(r ? i.replace(mi, "$1") : n || e)
             })), t
         }));
-    var mi = function(e, t) {
+    var xi = function(e, t) {
             for (var n = -1, r = null == e ? 0 : e.length, i = Array(r); ++n < r;) i[n] = t(e[n], n, e);
             return i
         },
-        bi = U ? U.prototype : void 0,
-        xi = bi ? bi.toString : void 0;
-    var wi = function e(t) {
+        wi = Z ? Z.prototype : void 0,
+        Ei = wi ? wi.toString : void 0;
+    var ki = function e(t) {
         if ("string" == typeof t) return t;
-        if (yr(t)) return mi(t, e) + "";
-        if (oe(t)) return xi ? xi.call(t) : "";
+        if (br(t)) return xi(t, e) + "";
+        if (se(t)) return Ei ? Ei.call(t) : "";
         var n = t + "";
         return "0" == n && 1 / t == -1 / 0 ? "-0" : n
     };
-    var Ei = function(e) {
-        return null == e ? "" : wi(e)
+    var Ci = function(e) {
+        return null == e ? "" : ki(e)
     };
-    var ki = function(e, t) {
-        return yr(e) ? e : xr(e, t) ? [e] : yi(Ei(e))
+    var Si = function(e, t) {
+        return br(e) ? e : Er(e, t) ? [e] : bi(Ci(e))
     };
-    var Ci = function(e) {
-        if ("string" == typeof e || oe(e)) return e;
+    var Pi = function(e) {
+        if ("string" == typeof e || se(e)) return e;
         var t = e + "";
         return "0" == t && 1 / e == -1 / 0 ? "-0" : t
     };
-    var Si = function(e, t) {
-        for (var n = 0, r = (t = ki(t, e)).length; null != e && n < r;) e = e[Ci(t[n++])];
+    var Di = function(e, t) {
+        for (var n = 0, r = (t = Si(t, e)).length; null != e && n < r;) e = e[Pi(t[n++])];
         return n && n == r ? e : void 0
     };
-    var Pi = function(e, t, n) {
-            var r = null == e ? void 0 : Si(e, t);
+    var Ti = function(e, t, n) {
+            var r = null == e ? void 0 : Di(e, t);
             return void 0 === r ? n : r
         },
-        Di = function() {
+        _i = function() {
             try {
-                var e = Ar(Object, "defineProperty");
+                var e = Rr(Object, "defineProperty");
                 return e({}, "", {}), e
             } catch (e) {}
         }();
-    var Ti = function(e, t, n) {
-            "__proto__" == t && Di ? Di(e, t, {
+    var Mi = function(e, t, n) {
+            "__proto__" == t && _i ? _i(e, t, {
                 configurable: !0,
                 enumerable: !0,
                 value: n,
                 writable: !0
             }) : e[t] = n
         },
-        _i = Object.prototype.hasOwnProperty;
-    var Mi = function(e, t, n) {
+        Bi = Object.prototype.hasOwnProperty;
+    var Ni = function(e, t, n) {
             var r = e[t];
-            _i.call(e, t) && Gr(r, n) && (void 0 !== n || t in e) || Ti(e, t, n)
+            Bi.call(e, t) && Zr(r, n) && (void 0 !== n || t in e) || Mi(e, t, n)
         },
-        Bi = /^(?:0|[1-9]\d*)$/;
-    var Ni = function(e, t) {
+        zi = /^(?:0|[1-9]\d*)$/;
+    var Ii = function(e, t) {
         var n = typeof e;
-        return !!(t = null == t ? 9007199254740991 : t) && ("number" == n || "symbol" != n && Bi.test(e)) && e > -1 && e % 1 == 0 && e < t
+        return !!(t = null == t ? 9007199254740991 : t) && ("number" == n || "symbol" != n && zi.test(e)) && e > -1 && e % 1 == 0 && e < t
     };
-    var zi = function(e, t, n, r) {
-        if (!V(e)) return e;
-        for (var i = -1, a = (t = ki(t, e)).length, o = a - 1, s = e; null != s && ++i < a;) {
-            var l = Ci(t[i]),
+    var Ai = function(e, t, n, r) {
+        if (!F(e)) return e;
+        for (var i = -1, a = (t = Si(t, e)).length, o = a - 1, s = e; null != s && ++i < a;) {
+            var l = Pi(t[i]),
                 u = n;
             if ("__proto__" === l || "constructor" === l || "prototype" === l) return e;
             if (i != o) {
                 var c = s[l];
-                void 0 === (u = r ? r(c, l, s) : void 0) && (u = V(c) ? c : Ni(t[i + 1]) ? [] : {})
+                void 0 === (u = r ? r(c, l, s) : void 0) && (u = F(c) ? c : Ii(t[i + 1]) ? [] : {})
             }
-            Mi(s, l, u), s = s[l]
+            Ni(s, l, u), s = s[l]
         }
         return e
     };
-    var Ii = function(e, t, n) {
-        return null == e ? e : zi(e, t, n)
+    var Li = function(e, t, n) {
+        return null == e ? e : Ai(e, t, n)
     };
-    var Li = function(e, t) {
+    var Oi = function(e, t) {
         var n = -1,
             r = e.length;
         for (t || (t = Array(r)); ++n < r;) t[n] = e[n];
         return t
     };
-    var Ai = function(e) {
-            return yr(e) ? mi(e, Ci) : oe(e) ? [e] : Li(yi(Ei(e)))
+    var Ri = function(e) {
+            return br(e) ? xi(e, Pi) : se(e) ? [e] : Oi(bi(Ci(e)))
         },
-        Oi = {};
-    [vr, {
+        Vi = {};
+    [mr, {
         data: function(e) {
-            return e = I({}, {
+            return e = A({}, {
                     field: "data",
                     bindingEvent: "data",
                     allowBinding: !1,
                     allowSetting: !1,
                     allowGetting: !1,
                     settingEvent: "data",
                     settingTriggersEvent: !1,
@@ -3293,115 +3320,115 @@
                     }
                 }, e),
                 function(t, n) {
                     var r = e,
                         a = void 0 !== this.length,
                         o = a ? this : [this],
                         s = a ? this[0] : this;
-                    if (f(t)) {
-                        var l, u = -1 !== t.indexOf(".") && Ai(t);
-                        if (r.allowGetting && void 0 === n) return s && (r.beforeGet(s), l = u && void 0 === s._private[r.field][t] ? Pi(s._private[r.field], u) : s._private[r.field][t]), l;
+                    if (g(t)) {
+                        var l, u = -1 !== t.indexOf(".") && Ri(t);
+                        if (r.allowGetting && void 0 === n) return s && (r.beforeGet(s), l = u && void 0 === s._private[r.field][t] ? Ti(s._private[r.field], u) : s._private[r.field][t]), l;
                         if (r.allowSetting && void 0 !== n && !r.immutableKeys[t]) {
                             var c = i({}, t, n);
                             r.beforeSet(this, c);
                             for (var d = 0, h = o.length; d < h; d++) {
                                 var p = o[d];
-                                r.canSet(p) && (u && void 0 === s._private[r.field][t] ? Ii(p._private[r.field], u, n) : p._private[r.field][t] = n)
+                                r.canSet(p) && (u && void 0 === s._private[r.field][t] ? Li(p._private[r.field], u, n) : p._private[r.field][t] = n)
                             }
                             r.updateStyle && this.updateStyle(), r.onSet(this), r.settingTriggersEvent && this[r.triggerFnName](r.settingEvent)
                         }
-                    } else if (r.allowSetting && y(t)) {
-                        var v, m, b = t,
+                    } else if (r.allowSetting && m(t)) {
+                        var f, y, b = t,
                             x = Object.keys(b);
                         r.beforeSet(this, b);
                         for (var w = 0; w < x.length; w++) {
-                            if (m = b[v = x[w]], !r.immutableKeys[v])
+                            if (y = b[f = x[w]], !r.immutableKeys[f])
                                 for (var E = 0; E < o.length; E++) {
                                     var k = o[E];
-                                    r.canSet(k) && (k._private[r.field][v] = m)
+                                    r.canSet(k) && (k._private[r.field][f] = y)
                                 }
                         }
                         r.updateStyle && this.updateStyle(), r.onSet(this), r.settingTriggersEvent && this[r.triggerFnName](r.settingEvent)
-                    } else if (r.allowBinding && g(t)) {
+                    } else if (r.allowBinding && v(t)) {
                         var C = t;
                         this.on(r.bindingEvent, C)
                     } else if (r.allowGetting && void 0 === t) {
                         var S;
                         return s && (r.beforeGet(s), S = s._private[r.field]), S
                     }
                     return this
                 }
         },
         removeData: function(e) {
-            return e = I({}, {
+            return e = A({}, {
                     field: "data",
                     event: "data",
                     triggerFnName: "trigger",
                     triggerEvent: !1,
                     immutableKeys: {}
                 }, e),
                 function(t) {
                     var n = e,
                         r = void 0 !== this.length ? this : [this];
-                    if (f(t)) {
+                    if (g(t)) {
                         for (var i = t.split(/\s+/), a = i.length, o = 0; o < a; o++) {
                             var s = i[o];
-                            if (!S(s))
+                            if (!P(s))
                                 if (!n.immutableKeys[s])
                                     for (var l = 0, u = r.length; l < u; l++) r[l]._private[n.field][s] = void 0
                         }
                         n.triggerEvent && this[n.triggerFnName](n.event)
                     } else if (void 0 === t) {
                         for (var c = 0, d = r.length; c < d; c++)
-                            for (var h = r[c]._private[n.field], p = Object.keys(h), g = 0; g < p.length; g++) {
-                                var v = p[g];
+                            for (var h = r[c]._private[n.field], p = Object.keys(h), f = 0; f < p.length; f++) {
+                                var v = p[f];
                                 !n.immutableKeys[v] && (h[v] = void 0)
                             }
                         n.triggerEvent && this[n.triggerFnName](n.event)
                     }
                     return this
                 }
         }
     }, {
         eventAliasesOn: function(e) {
             var t = e;
             t.addListener = t.listen = t.bind = t.on, t.unlisten = t.unbind = t.off = t.removeListener, t.trigger = t.emit, t.pon = t.promiseOn = function(e, t) {
                 var n = this,
                     r = Array.prototype.slice.call(arguments, 0);
-                return new pr((function(e, t) {
+                return new gr((function(e, t) {
                     var i = r.concat([function(t) {
                             n.off.apply(n, a), e(t)
                         }]),
                         a = i.concat([]);
                     n.on.apply(n, i)
                 }))
             }
         }
     }].forEach((function(e) {
-        I(Oi, e)
+        A(Vi, e)
     }));
-    var Ri = {
-            animate: Oi.animate(),
-            animation: Oi.animation(),
-            animated: Oi.animated(),
-            clearQueue: Oi.clearQueue(),
-            delay: Oi.delay(),
-            delayAnimation: Oi.delayAnimation(),
-            stop: Oi.stop()
+    var Fi = {
+            animate: Vi.animate(),
+            animation: Vi.animation(),
+            animated: Vi.animated(),
+            clearQueue: Vi.clearQueue(),
+            delay: Vi.delay(),
+            delayAnimation: Vi.delayAnimation(),
+            stop: Vi.stop()
         },
-        Vi = {
+        ji = {
             classes: function(e) {
                 if (void 0 === e) {
                     var t = [];
                     return this[0]._private.classes.forEach((function(e) {
                         return t.push(e)
                     })), t
                 }
-                v(e) || (e = (e || "").match(/\S+/g) || []);
-                for (var n = [], r = new $e(e), i = 0; i < this.length; i++) {
+                y(e) || (e = (e || "").match(/\S+/g) || []);
+                for (var n = [], r = new Qe(e), i = 0; i < this.length; i++) {
                     for (var a = this[i], o = a._private, s = o.classes, l = !1, u = 0; u < e.length; u++) {
                         var c = e[u];
                         if (!s.has(c)) {
                             l = !0;
                             break
                         }
                     }
@@ -3413,15 +3440,15 @@
                 return this.toggleClass(e, !0)
             },
             hasClass: function(e) {
                 var t = this[0];
                 return null != t && t._private.classes.has(e)
             },
             toggleClass: function(e, t) {
-                v(e) || (e = e.match(/\S+/g) || []);
+                y(e) || (e = e.match(/\S+/g) || []);
                 for (var n = void 0 === t, r = [], i = 0, a = this.length; i < a; i++)
                     for (var o = this[i], s = o._private.classes, l = !1, u = 0; u < e.length; u++) {
                         var c = e[u],
                             d = s.has(c),
                             h = !1;
                         t || n && !d ? (s.add(c), h = !0) : (!t || n && d) && (s.delete(c), h = !0), !l && h && (r.push(o), l = !0)
                     }
@@ -3435,58 +3462,58 @@
                 if (null == t) t = 250;
                 else if (0 === t) return n;
                 return n.addClass(e), setTimeout((function() {
                     n.removeClass(e)
                 }), t), n
             }
         };
-    Vi.className = Vi.classNames = Vi.classes;
-    var Fi = {
+    ji.className = ji.classNames = ji.classes;
+    var qi = {
         metaChar: "[\\!\\\"\\#\\$\\%\\&\\'\\(\\)\\*\\+\\,\\.\\/\\:\\;\\<\\=\\>\\?\\@\\[\\]\\^\\`\\{\\|\\}\\~]",
         comparatorOp: "=|\\!=|>|>=|<|<=|\\$=|\\^=|\\*=",
         boolOp: "\\?|\\!|\\^",
         string: "\"(?:\\\\\"|[^\"])*\"|'(?:\\\\'|[^'])*'",
-        number: N,
+        number: z,
         meta: "degree|indegree|outdegree",
         separator: "\\s*,\\s*",
         descendant: "\\s+",
         child: "\\s+>\\s+",
         subject: "\\$",
         group: "node|edge|\\*",
         directedEdge: "\\s+->\\s+",
         undirectedEdge: "\\s+<->\\s+"
     };
-    Fi.variable = "(?:[\\w-.]|(?:\\\\" + Fi.metaChar + "))+", Fi.className = "(?:[\\w-]|(?:\\\\" + Fi.metaChar + "))+", Fi.value = Fi.string + "|" + Fi.number, Fi.id = Fi.variable,
+    qi.variable = "(?:[\\w-.]|(?:\\\\" + qi.metaChar + "))+", qi.className = "(?:[\\w-]|(?:\\\\" + qi.metaChar + "))+", qi.value = qi.string + "|" + qi.number, qi.id = qi.variable,
         function() {
             var e, t, n;
-            for (e = Fi.comparatorOp.split("|"), n = 0; n < e.length; n++) t = e[n], Fi.comparatorOp += "|@" + t;
-            for (e = Fi.comparatorOp.split("|"), n = 0; n < e.length; n++)(t = e[n]).indexOf("!") >= 0 || "=" !== t && (Fi.comparatorOp += "|\\!" + t)
+            for (e = qi.comparatorOp.split("|"), n = 0; n < e.length; n++) t = e[n], qi.comparatorOp += "|@" + t;
+            for (e = qi.comparatorOp.split("|"), n = 0; n < e.length; n++)(t = e[n]).indexOf("!") >= 0 || "=" !== t && (qi.comparatorOp += "|\\!" + t)
         }();
-    var ji = 0,
-        qi = 1,
-        Yi = 2,
-        Xi = 3,
-        Wi = 4,
-        Hi = 5,
-        Ki = 6,
-        Gi = 7,
-        Ui = 8,
-        Zi = 9,
-        $i = 10,
-        Qi = 11,
-        Ji = 12,
-        ea = 13,
-        ta = 14,
-        na = 15,
-        ra = 16,
-        ia = 17,
-        aa = 18,
-        oa = 19,
-        sa = 20,
-        la = [{
+    var Yi = 0,
+        Xi = 1,
+        Wi = 2,
+        Hi = 3,
+        Ki = 4,
+        Gi = 5,
+        Ui = 6,
+        Zi = 7,
+        $i = 8,
+        Qi = 9,
+        Ji = 10,
+        ea = 11,
+        ta = 12,
+        na = 13,
+        ra = 14,
+        ia = 15,
+        aa = 16,
+        oa = 17,
+        sa = 18,
+        la = 19,
+        ua = 20,
+        ca = [{
             selector: ":selected",
             matches: function(e) {
                 return e.selected()
             }
         }, {
             selector: ":unselected",
             matches: function(e) {
@@ -3625,227 +3652,227 @@
         }, {
             selector: ":nonbackgrounding",
             matches: function(e) {
                 return !e.backgrounding()
             }
         }].sort((function(e, t) {
             return function(e, t) {
-                return -1 * z(e, t)
+                return -1 * I(e, t)
             }(e.selector, t.selector)
         })),
-        ua = function() {
-            for (var e, t = {}, n = 0; n < la.length; n++) t[(e = la[n]).selector] = e.matches;
+        da = function() {
+            for (var e, t = {}, n = 0; n < ca.length; n++) t[(e = ca[n]).selector] = e.matches;
             return t
         }(),
-        ca = "(" + la.map((function(e) {
+        ha = "(" + ca.map((function(e) {
             return e.selector
         })).join("|") + ")",
-        da = function(e) {
-            return e.replace(new RegExp("\\\\(" + Fi.metaChar + ")", "g"), (function(e, t) {
+        pa = function(e) {
+            return e.replace(new RegExp("\\\\(" + qi.metaChar + ")", "g"), (function(e, t) {
                 return t
             }))
         },
-        ha = function(e, t, n) {
+        fa = function(e, t, n) {
             e[e.length - 1] = n
         },
-        pa = [{
+        ga = [{
             name: "group",
             query: !0,
-            regex: "(" + Fi.group + ")",
+            regex: "(" + qi.group + ")",
             populate: function(e, t, n) {
                 var r = a(n, 1)[0];
                 t.checks.push({
-                    type: ji,
+                    type: Yi,
                     value: "*" === r ? r : r + "s"
                 })
             }
         }, {
             name: "state",
             query: !0,
-            regex: ca,
+            regex: ha,
             populate: function(e, t, n) {
                 var r = a(n, 1)[0];
                 t.checks.push({
-                    type: Gi,
+                    type: Zi,
                     value: r
                 })
             }
         }, {
             name: "id",
             query: !0,
-            regex: "\\#(" + Fi.id + ")",
+            regex: "\\#(" + qi.id + ")",
             populate: function(e, t, n) {
                 var r = a(n, 1)[0];
                 t.checks.push({
-                    type: Ui,
-                    value: da(r)
+                    type: $i,
+                    value: pa(r)
                 })
             }
         }, {
             name: "className",
             query: !0,
-            regex: "\\.(" + Fi.className + ")",
+            regex: "\\.(" + qi.className + ")",
             populate: function(e, t, n) {
                 var r = a(n, 1)[0];
                 t.checks.push({
-                    type: Zi,
-                    value: da(r)
+                    type: Qi,
+                    value: pa(r)
                 })
             }
         }, {
             name: "dataExists",
             query: !0,
-            regex: "\\[\\s*(" + Fi.variable + ")\\s*\\]",
+            regex: "\\[\\s*(" + qi.variable + ")\\s*\\]",
             populate: function(e, t, n) {
                 var r = a(n, 1)[0];
                 t.checks.push({
-                    type: Wi,
-                    field: da(r)
+                    type: Ki,
+                    field: pa(r)
                 })
             }
         }, {
             name: "dataCompare",
             query: !0,
-            regex: "\\[\\s*(" + Fi.variable + ")\\s*(" + Fi.comparatorOp + ")\\s*(" + Fi.value + ")\\s*\\]",
+            regex: "\\[\\s*(" + qi.variable + ")\\s*(" + qi.comparatorOp + ")\\s*(" + qi.value + ")\\s*\\]",
             populate: function(e, t, n) {
                 var r = a(n, 3),
                     i = r[0],
                     o = r[1],
                     s = r[2];
-                s = null != new RegExp("^" + Fi.string + "$").exec(s) ? s.substring(1, s.length - 1) : parseFloat(s), t.checks.push({
-                    type: Xi,
-                    field: da(i),
+                s = null != new RegExp("^" + qi.string + "$").exec(s) ? s.substring(1, s.length - 1) : parseFloat(s), t.checks.push({
+                    type: Hi,
+                    field: pa(i),
                     operator: o,
                     value: s
                 })
             }
         }, {
             name: "dataBool",
             query: !0,
-            regex: "\\[\\s*(" + Fi.boolOp + ")\\s*(" + Fi.variable + ")\\s*\\]",
+            regex: "\\[\\s*(" + qi.boolOp + ")\\s*(" + qi.variable + ")\\s*\\]",
             populate: function(e, t, n) {
                 var r = a(n, 2),
                     i = r[0],
                     o = r[1];
                 t.checks.push({
-                    type: Hi,
-                    field: da(o),
+                    type: Gi,
+                    field: pa(o),
                     operator: i
                 })
             }
         }, {
             name: "metaCompare",
             query: !0,
-            regex: "\\[\\[\\s*(" + Fi.meta + ")\\s*(" + Fi.comparatorOp + ")\\s*(" + Fi.number + ")\\s*\\]\\]",
+            regex: "\\[\\[\\s*(" + qi.meta + ")\\s*(" + qi.comparatorOp + ")\\s*(" + qi.number + ")\\s*\\]\\]",
             populate: function(e, t, n) {
                 var r = a(n, 3),
                     i = r[0],
                     o = r[1],
                     s = r[2];
                 t.checks.push({
-                    type: Ki,
-                    field: da(i),
+                    type: Ui,
+                    field: pa(i),
                     operator: o,
                     value: parseFloat(s)
                 })
             }
         }, {
             name: "nextQuery",
             separator: !0,
-            regex: Fi.separator,
+            regex: qi.separator,
             populate: function(e, t) {
                 var n = e.currentSubject,
                     r = e.edgeCount,
                     i = e.compoundCount,
                     a = e[e.length - 1];
                 return null != n && (a.subject = n, e.currentSubject = null), a.edgeCount = r, a.compoundCount = i, e.edgeCount = 0, e.compoundCount = 0, e[e.length++] = {
                     checks: []
                 }
             }
         }, {
             name: "directedEdge",
             separator: !0,
-            regex: Fi.directedEdge,
+            regex: qi.directedEdge,
             populate: function(e, t) {
                 if (null == e.currentSubject) {
                     var n = {
                             checks: []
                         },
                         r = t,
                         i = {
                             checks: []
                         };
                     return n.checks.push({
-                        type: Qi,
+                        type: ea,
                         source: r,
                         target: i
-                    }), ha(e, 0, n), e.edgeCount++, i
+                    }), fa(e, 0, n), e.edgeCount++, i
                 }
                 var a = {
                         checks: []
                     },
                     o = t,
                     s = {
                         checks: []
                     };
                 return a.checks.push({
-                    type: Ji,
+                    type: ta,
                     source: o,
                     target: s
-                }), ha(e, 0, a), e.edgeCount++, s
+                }), fa(e, 0, a), e.edgeCount++, s
             }
         }, {
             name: "undirectedEdge",
             separator: !0,
-            regex: Fi.undirectedEdge,
+            regex: qi.undirectedEdge,
             populate: function(e, t) {
                 if (null == e.currentSubject) {
                     var n = {
                             checks: []
                         },
                         r = t,
                         i = {
                             checks: []
                         };
                     return n.checks.push({
-                        type: $i,
+                        type: Ji,
                         nodes: [r, i]
-                    }), ha(e, 0, n), e.edgeCount++, i
+                    }), fa(e, 0, n), e.edgeCount++, i
                 }
                 var a = {
                         checks: []
                     },
                     o = t,
                     s = {
                         checks: []
                     };
                 return a.checks.push({
-                    type: ta,
+                    type: ra,
                     node: o,
                     neighbor: s
-                }), ha(e, 0, a), s
+                }), fa(e, 0, a), s
             }
         }, {
             name: "child",
             separator: !0,
-            regex: Fi.child,
+            regex: qi.child,
             populate: function(e, t) {
                 if (null == e.currentSubject) {
                     var n = {
                             checks: []
                         },
                         r = {
                             checks: []
                         },
                         i = e[e.length - 1];
                     return n.checks.push({
-                        type: na,
+                        type: ia,
                         parent: i,
                         child: r
-                    }), ha(e, 0, n), e.compoundCount++, r
+                    }), fa(e, 0, n), e.compoundCount++, r
                 }
                 if (e.currentSubject === t) {
                     var a = {
                             checks: []
                         },
                         o = e[e.length - 1],
                         s = {
@@ -3857,59 +3884,59 @@
                         u = {
                             checks: []
                         },
                         c = {
                             checks: []
                         };
                     return a.checks.push({
-                        type: oa,
+                        type: la,
                         left: o,
                         right: s,
                         subject: l
                     }), l.checks = t.checks, t.checks = [{
-                        type: sa
+                        type: ua
                     }], c.checks.push({
-                        type: sa
+                        type: ua
                     }), s.checks.push({
-                        type: ia,
+                        type: oa,
                         parent: c,
                         child: u
-                    }), ha(e, 0, a), e.currentSubject = l, e.compoundCount++, u
+                    }), fa(e, 0, a), e.currentSubject = l, e.compoundCount++, u
                 }
                 var d = {
                         checks: []
                     },
                     h = {
                         checks: []
                     },
                     p = [{
-                        type: ia,
+                        type: oa,
                         parent: d,
                         child: h
                     }];
                 return d.checks = t.checks, t.checks = p, e.compoundCount++, h
             }
         }, {
             name: "descendant",
             separator: !0,
-            regex: Fi.descendant,
+            regex: qi.descendant,
             populate: function(e, t) {
                 if (null == e.currentSubject) {
                     var n = {
                             checks: []
                         },
                         r = {
                             checks: []
                         },
                         i = e[e.length - 1];
                     return n.checks.push({
-                        type: ra,
+                        type: aa,
                         ancestor: i,
                         descendant: r
-                    }), ha(e, 0, n), e.compoundCount++, r
+                    }), fa(e, 0, n), e.compoundCount++, r
                 }
                 if (e.currentSubject === t) {
                     var a = {
                             checks: []
                         },
                         o = e[e.length - 1],
                         s = {
@@ -3921,59 +3948,59 @@
                         u = {
                             checks: []
                         },
                         c = {
                             checks: []
                         };
                     return a.checks.push({
-                        type: oa,
+                        type: la,
                         left: o,
                         right: s,
                         subject: l
                     }), l.checks = t.checks, t.checks = [{
-                        type: sa
+                        type: ua
                     }], c.checks.push({
-                        type: sa
+                        type: ua
                     }), s.checks.push({
-                        type: aa,
+                        type: sa,
                         ancestor: c,
                         descendant: u
-                    }), ha(e, 0, a), e.currentSubject = l, e.compoundCount++, u
+                    }), fa(e, 0, a), e.currentSubject = l, e.compoundCount++, u
                 }
                 var d = {
                         checks: []
                     },
                     h = {
                         checks: []
                     },
                     p = [{
-                        type: aa,
+                        type: sa,
                         ancestor: d,
                         descendant: h
                     }];
                 return d.checks = t.checks, t.checks = p, e.compoundCount++, h
             }
         }, {
             name: "subject",
             modifier: !0,
-            regex: Fi.subject,
+            regex: qi.subject,
             populate: function(e, t) {
-                if (null != e.currentSubject && e.currentSubject !== t) return Ve("Redefinition of subject in selector `" + e.toString() + "`"), !1;
+                if (null != e.currentSubject && e.currentSubject !== t) return Fe("Redefinition of subject in selector `" + e.toString() + "`"), !1;
                 e.currentSubject = t;
                 var n = e[e.length - 1].checks[0],
                     r = null == n ? null : n.type;
-                r === Qi ? n.type = ea : r === $i && (n.type = ta, n.node = n.nodes[1], n.neighbor = n.nodes[0], n.nodes = null)
+                r === ea ? n.type = na : r === Ji && (n.type = ra, n.node = n.nodes[1], n.neighbor = n.nodes[0], n.nodes = null)
             }
         }];
-    pa.forEach((function(e) {
+    ga.forEach((function(e) {
         return e.regexObj = new RegExp("^" + e.regex)
     }));
-    var fa = function(e) {
-            for (var t, n, r, i = 0; i < pa.length; i++) {
-                var a = pa[i],
+    var va = function(e) {
+            for (var t, n, r, i = 0; i < ga.length; i++) {
+                var a = ga[i],
                     o = a.name,
                     s = e.match(a.regexObj);
                 if (null != s) {
                     n = s, t = a, r = o;
                     var l = s[0];
                     e = e.substring(l.length);
                     break
@@ -3982,108 +4009,108 @@
             return {
                 expr: t,
                 match: n,
                 name: r,
                 remaining: e
             }
         },
-        ga = {
+        ya = {
             parse: function(e) {
                 var t = this.inputText = e,
                     n = this[0] = {
                         checks: []
                     };
                 for (this.length = 1, t = function(e) {
                         var t = e.match(/^\s+/);
                         if (t) {
                             var n = t[0];
                             e = e.substring(n.length)
                         }
                         return e
                     }(t);;) {
-                    var r = fa(t);
-                    if (null == r.expr) return Ve("The selector `" + e + "`is invalid"), !1;
+                    var r = va(t);
+                    if (null == r.expr) return Fe("The selector `" + e + "`is invalid"), !1;
                     var i = r.match.slice(1),
                         a = r.expr.populate(this, n, i);
                     if (!1 === a) return !1;
                     if (null != a && (n = a), (t = r.remaining).match(/^\s*$/)) break
                 }
                 var o = this[this.length - 1];
                 null != this.currentSubject && (o.subject = this.currentSubject), o.edgeCount = this.edgeCount, o.compoundCount = this.compoundCount;
                 for (var s = 0; s < this.length; s++) {
                     var l = this[s];
-                    if (l.compoundCount > 0 && l.edgeCount > 0) return Ve("The selector `" + e + "` is invalid because it uses both a compound selector and an edge selector"), !1;
-                    if (l.edgeCount > 1) return Ve("The selector `" + e + "` is invalid because it uses multiple edge selectors"), !1;
-                    1 === l.edgeCount && Ve("The selector `" + e + "` is deprecated.  Edge selectors do not take effect on changes to source and target nodes after an edge is added, for performance reasons.  Use a class or data selector on edges instead, updating the class or data of an edge when your app detects a change in source or target nodes.")
+                    if (l.compoundCount > 0 && l.edgeCount > 0) return Fe("The selector `" + e + "` is invalid because it uses both a compound selector and an edge selector"), !1;
+                    if (l.edgeCount > 1) return Fe("The selector `" + e + "` is invalid because it uses multiple edge selectors"), !1;
+                    1 === l.edgeCount && Fe("The selector `" + e + "` is deprecated.  Edge selectors do not take effect on changes to source and target nodes after an edge is added, for performance reasons.  Use a class or data selector on edges instead, updating the class or data of an edge when your app detects a change in source or target nodes.")
                 }
                 return !0
             },
             toString: function() {
                 if (null != this.toStringCache) return this.toStringCache;
                 for (var e = function(e) {
                         return null == e ? "" : e
                     }, t = function(t) {
-                        return f(t) ? '"' + t + '"' : e(t)
+                        return g(t) ? '"' + t + '"' : e(t)
                     }, n = function(e) {
                         return " " + e + " "
                     }, r = function(r, a) {
                         var o = r.type,
                             s = r.value;
                         switch (o) {
-                            case ji:
+                            case Yi:
                                 var l = e(s);
                                 return l.substring(0, l.length - 1);
-                            case Xi:
+                            case Hi:
                                 var u = r.field,
                                     c = r.operator;
                                 return "[" + u + n(e(c)) + t(s) + "]";
-                            case Hi:
+                            case Gi:
                                 var d = r.operator,
                                     h = r.field;
                                 return "[" + e(d) + h + "]";
-                            case Wi:
-                                return "[" + r.field + "]";
                             case Ki:
+                                return "[" + r.field + "]";
+                            case Ui:
                                 var p = r.operator;
                                 return "[[" + r.field + n(e(p)) + t(s) + "]]";
-                            case Gi:
+                            case Zi:
                                 return s;
-                            case Ui:
+                            case $i:
                                 return "#" + s;
-                            case Zi:
+                            case Qi:
                                 return "." + s;
+                            case oa:
                             case ia:
-                            case na:
                                 return i(r.parent, a) + n(">") + i(r.child, a);
+                            case sa:
                             case aa:
-                            case ra:
                                 return i(r.ancestor, a) + " " + i(r.descendant, a);
-                            case oa:
+                            case la:
                                 var f = i(r.left, a),
                                     g = i(r.subject, a),
                                     v = i(r.right, a);
                                 return f + (f.length > 0 ? " " : "") + g + v;
-                            case sa:
+                            case ua:
                                 return ""
                         }
                     }, i = function(e, t) {
                         return e.checks.reduce((function(n, i, a) {
                             return n + (t === e && 0 === a ? "$" : "") + r(i, t)
                         }), "")
                     }, a = "", o = 0; o < this.length; o++) {
                     var s = this[o];
                     a += i(s, s.subject), this.length > 1 && o < this.length - 1 && (a += ", ")
                 }
                 return this.toStringCache = a, a
             }
         },
-        va = function(e, t, n) {
-            var r, i, a, o = f(e),
-                s = m(e),
-                l = f(n),
+        ma = function(e, t, n) {
+            var r, i, a, o = g(e),
+                s = b(e),
+                l = g(n),
                 u = !1,
                 c = !1,
                 d = !1;
             switch (t.indexOf("!") >= 0 && (t = t.replace("!", ""), c = !0), t.indexOf("@") >= 0 && (t = t.replace("@", ""), u = !0), (o || l || u) && (i = o || s ? "" + e : "", a = "" + n), u && (e = i = i.toLowerCase(), n = a = a.toLowerCase()), t) {
                 case "*=":
                     r = i.indexOf(a) >= 0;
                     break;
@@ -4109,165 +4136,165 @@
                     d = !0, r = e <= n;
                     break;
                 default:
                     r = !1
             }
             return !c || null == e && d || (r = !r), r
         },
-        ya = function(e, t) {
+        ba = function(e, t) {
             return e.data(t)
         },
-        ma = [],
-        ba = function(e, t) {
+        xa = [],
+        wa = function(e, t) {
             return e.checks.every((function(e) {
-                return ma[e.type](e, t)
+                return xa[e.type](e, t)
             }))
         };
-    ma[ji] = function(e, t) {
+    xa[Yi] = function(e, t) {
         var n = e.value;
         return "*" === n || n === t.group()
-    }, ma[Gi] = function(e, t) {
+    }, xa[Zi] = function(e, t) {
         return function(e, t) {
-            return ua[e](t)
+            return da[e](t)
         }(e.value, t)
-    }, ma[Ui] = function(e, t) {
+    }, xa[$i] = function(e, t) {
         var n = e.value;
         return t.id() === n
-    }, ma[Zi] = function(e, t) {
+    }, xa[Qi] = function(e, t) {
         var n = e.value;
         return t.hasClass(n)
-    }, ma[Ki] = function(e, t) {
+    }, xa[Ui] = function(e, t) {
         var n = e.field,
             r = e.operator,
             i = e.value;
-        return va(function(e, t) {
+        return ma(function(e, t) {
             return e[t]()
         }(t, n), r, i)
-    }, ma[Xi] = function(e, t) {
+    }, xa[Hi] = function(e, t) {
         var n = e.field,
             r = e.operator,
             i = e.value;
-        return va(ya(t, n), r, i)
-    }, ma[Hi] = function(e, t) {
+        return ma(ba(t, n), r, i)
+    }, xa[Gi] = function(e, t) {
         var n = e.field,
             r = e.operator;
         return function(e, t) {
             switch (t) {
                 case "?":
                     return !!e;
                 case "!":
                     return !e;
                 case "^":
                     return void 0 === e
             }
-        }(ya(t, n), r)
-    }, ma[Wi] = function(e, t) {
+        }(ba(t, n), r)
+    }, xa[Ki] = function(e, t) {
         var n = e.field;
-        return e.operator, void 0 !== ya(t, n)
-    }, ma[$i] = function(e, t) {
+        return e.operator, void 0 !== ba(t, n)
+    }, xa[Ji] = function(e, t) {
         var n = e.nodes[0],
             r = e.nodes[1],
             i = t.source(),
             a = t.target();
-        return ba(n, i) && ba(r, a) || ba(r, i) && ba(n, a)
-    }, ma[ta] = function(e, t) {
-        return ba(e.node, t) && t.neighborhood().some((function(t) {
-            return t.isNode() && ba(e.neighbor, t)
+        return wa(n, i) && wa(r, a) || wa(r, i) && wa(n, a)
+    }, xa[ra] = function(e, t) {
+        return wa(e.node, t) && t.neighborhood().some((function(t) {
+            return t.isNode() && wa(e.neighbor, t)
         }))
-    }, ma[Qi] = function(e, t) {
-        return ba(e.source, t.source()) && ba(e.target, t.target())
-    }, ma[Ji] = function(e, t) {
-        return ba(e.source, t) && t.outgoers().some((function(t) {
-            return t.isNode() && ba(e.target, t)
+    }, xa[ea] = function(e, t) {
+        return wa(e.source, t.source()) && wa(e.target, t.target())
+    }, xa[ta] = function(e, t) {
+        return wa(e.source, t) && t.outgoers().some((function(t) {
+            return t.isNode() && wa(e.target, t)
         }))
-    }, ma[ea] = function(e, t) {
-        return ba(e.target, t) && t.incomers().some((function(t) {
-            return t.isNode() && ba(e.source, t)
+    }, xa[na] = function(e, t) {
+        return wa(e.target, t) && t.incomers().some((function(t) {
+            return t.isNode() && wa(e.source, t)
         }))
-    }, ma[na] = function(e, t) {
-        return ba(e.child, t) && ba(e.parent, t.parent())
-    }, ma[ia] = function(e, t) {
-        return ba(e.parent, t) && t.children().some((function(t) {
-            return ba(e.child, t)
+    }, xa[ia] = function(e, t) {
+        return wa(e.child, t) && wa(e.parent, t.parent())
+    }, xa[oa] = function(e, t) {
+        return wa(e.parent, t) && t.children().some((function(t) {
+            return wa(e.child, t)
         }))
-    }, ma[ra] = function(e, t) {
-        return ba(e.descendant, t) && t.ancestors().some((function(t) {
-            return ba(e.ancestor, t)
+    }, xa[aa] = function(e, t) {
+        return wa(e.descendant, t) && t.ancestors().some((function(t) {
+            return wa(e.ancestor, t)
         }))
-    }, ma[aa] = function(e, t) {
-        return ba(e.ancestor, t) && t.descendants().some((function(t) {
-            return ba(e.descendant, t)
+    }, xa[sa] = function(e, t) {
+        return wa(e.ancestor, t) && t.descendants().some((function(t) {
+            return wa(e.descendant, t)
         }))
-    }, ma[oa] = function(e, t) {
-        return ba(e.subject, t) && ba(e.left, t) && ba(e.right, t)
-    }, ma[sa] = function() {
+    }, xa[la] = function(e, t) {
+        return wa(e.subject, t) && wa(e.left, t) && wa(e.right, t)
+    }, xa[ua] = function() {
         return !0
-    }, ma[qi] = function(e, t) {
+    }, xa[Xi] = function(e, t) {
         return e.value.has(t)
-    }, ma[Yi] = function(e, t) {
+    }, xa[Wi] = function(e, t) {
         return (0, e.value)(t)
     };
-    var xa = function(e) {
-            this.inputText = e, this.currentSubject = null, this.compoundCount = 0, this.edgeCount = 0, this.length = 0, null == e || f(e) && e.match(/^\s*$/) || (x(e) ? this.addQuery({
+    var Ea = function(e) {
+            this.inputText = e, this.currentSubject = null, this.compoundCount = 0, this.edgeCount = 0, this.length = 0, null == e || g(e) && e.match(/^\s*$/) || (w(e) ? this.addQuery({
                 checks: [{
-                    type: qi,
+                    type: Xi,
                     value: e.collection()
                 }]
-            }) : g(e) ? this.addQuery({
+            }) : v(e) ? this.addQuery({
                 checks: [{
-                    type: Yi,
+                    type: Wi,
                     value: e
                 }]
-            }) : f(e) ? this.parse(e) || (this.invalid = !0) : Oe("A selector must be created from a string; found "))
+            }) : g(e) ? this.parse(e) || (this.invalid = !0) : Re("A selector must be created from a string; found "))
         },
-        wa = xa.prototype;
-    [ga, {
+        ka = Ea.prototype;
+    [ya, {
         matches: function(e) {
             for (var t = 0; t < this.length; t++) {
                 var n = this[t];
-                if (ba(n, e)) return !0
+                if (wa(n, e)) return !0
             }
             return !1
         },
         filter: function(e) {
             var t = this;
-            if (1 === t.length && 1 === t[0].checks.length && t[0].checks[0].type === Ui) return e.getElementById(t[0].checks[0].value).collection();
+            if (1 === t.length && 1 === t[0].checks.length && t[0].checks[0].type === $i) return e.getElementById(t[0].checks[0].value).collection();
             var n = function(e) {
                 for (var n = 0; n < t.length; n++) {
                     var r = t[n];
-                    if (ba(r, e)) return !0
+                    if (wa(r, e)) return !0
                 }
                 return !1
             };
             return null == t.text() && (n = function() {
                 return !0
             }), e.filter(n)
         }
     }].forEach((function(e) {
-        return I(wa, e)
-    })), wa.text = function() {
+        return A(ka, e)
+    })), ka.text = function() {
         return this.inputText
-    }, wa.size = function() {
+    }, ka.size = function() {
         return this.length
-    }, wa.eq = function(e) {
+    }, ka.eq = function(e) {
         return this[e]
-    }, wa.sameText = function(e) {
+    }, ka.sameText = function(e) {
         return !this.invalid && !e.invalid && this.text() === e.text()
-    }, wa.addQuery = function(e) {
+    }, ka.addQuery = function(e) {
         this[this.length++] = e
-    }, wa.selector = wa.toString;
-    var Ea = {
+    }, ka.selector = ka.toString;
+    var Ca = {
         allAre: function(e) {
-            var t = new xa(e);
+            var t = new Ea(e);
             return this.every((function(e) {
                 return t.matches(e)
             }))
         },
         is: function(e) {
-            var t = new xa(e);
+            var t = new Ea(e);
             return this.some((function(e) {
                 return t.matches(e)
             }))
         },
         some: function(e, t) {
             for (var n = 0; n < this.length; n++) {
                 if (t ? e.apply(t, [this[n], n, this]) : e(this[n], n, this)) return !0
@@ -4304,30 +4331,30 @@
             e = this.cy().collection(e);
             var t = this;
             return e.every((function(e) {
                 return t.hasElementWithId(e.id())
             }))
         }
     };
-    Ea.allAreNeighbours = Ea.allAreNeighbors, Ea.has = Ea.contains, Ea.equal = Ea.equals = Ea.same;
-    var ka, Ca, Sa = function(e, t) {
+    Ca.allAreNeighbours = Ca.allAreNeighbors, Ca.has = Ca.contains, Ca.equal = Ca.equals = Ca.same;
+    var Sa, Pa, Da = function(e, t) {
             return function(n, r, i, a) {
                 var o, s = n;
-                if (null == s ? o = "" : x(s) && 1 === s.length && (o = s.id()), 1 === this.length && o) {
+                if (null == s ? o = "" : w(s) && 1 === s.length && (o = s.id()), 1 === this.length && o) {
                     var l = this[0]._private,
                         u = l.traversalCache = l.traversalCache || {},
                         c = u[t] = u[t] || [],
-                        d = Pe(o),
+                        d = De(o),
                         h = c[d];
                     return h || (c[d] = e.call(this, n, r, i, a))
                 }
                 return e.call(this, n, r, i, a)
             }
         },
-        Pa = {
+        Ta = {
             parent: function(e) {
                 var t = [];
                 if (1 === this.length) {
                     var n = this[0]._private.parent;
                     if (n) return n
                 }
                 for (var r = 0; r < this.length; r++) {
@@ -4359,15 +4386,15 @@
                 })).filter(e)
             },
             nonorphans: function(e) {
                 return this.stdFilter((function(e) {
                     return e.isChild()
                 })).filter(e)
             },
-            children: Sa((function(e) {
+            children: Da((function(e) {
                 for (var t = [], n = 0; n < this.length; n++)
                     for (var r = this[n]._private.children, i = 0; i < r.length; i++) t.push(r[i]);
                 return this.spawn(t, !0).filter(e)
             }), "children"),
             siblings: function(e) {
                 return this.parent().children().not(this).filter(e)
             },
@@ -4394,55 +4421,55 @@
                         var i = n[r];
                         t.push(i), i.children().nonempty() && e(i.children())
                     }
                 }(this.children()), this.spawn(t, !0).filter(e)
             }
         };
 
-    function Da(e, t, n, r) {
-        for (var i = [], a = new $e, o = e.cy().hasCompoundNodes(), s = 0; s < e.length; s++) {
+    function _a(e, t, n, r) {
+        for (var i = [], a = new Qe, o = e.cy().hasCompoundNodes(), s = 0; s < e.length; s++) {
             var l = e[s];
             n ? i.push(l) : o && r(i, a, l)
         }
         for (; i.length > 0;) {
             var u = i.shift();
             t(u), a.add(u.id()), o && r(i, a, u)
         }
         return e
     }
 
-    function Ta(e, t, n) {
+    function Ma(e, t, n) {
         if (n.isParent())
             for (var r = n._private.children, i = 0; i < r.length; i++) {
                 var a = r[i];
                 t.has(a.id()) || e.push(a)
             }
     }
 
-    function _a(e, t, n) {
+    function Ba(e, t, n) {
         if (n.isChild()) {
             var r = n._private.parent;
             t.has(r.id()) || e.push(r)
         }
     }
 
-    function Ma(e, t, n) {
-        _a(e, t, n), Ta(e, t, n)
+    function Na(e, t, n) {
+        Ba(e, t, n), Ma(e, t, n)
     }
-    Pa.forEachDown = function(e) {
+    Ta.forEachDown = function(e) {
         var t = !(arguments.length > 1 && void 0 !== arguments[1]) || arguments[1];
-        return Da(this, e, t, Ta)
-    }, Pa.forEachUp = function(e) {
+        return _a(this, e, t, Ma)
+    }, Ta.forEachUp = function(e) {
         var t = !(arguments.length > 1 && void 0 !== arguments[1]) || arguments[1];
-        return Da(this, e, t, _a)
-    }, Pa.forEachUpAndDown = function(e) {
+        return _a(this, e, t, Ba)
+    }, Ta.forEachUpAndDown = function(e) {
         var t = !(arguments.length > 1 && void 0 !== arguments[1]) || arguments[1];
-        return Da(this, e, t, Ma)
-    }, Pa.ancestors = Pa.parents, (ka = Ca = {
-        data: Oi.data({
+        return _a(this, e, t, Na)
+    }, Ta.ancestors = Ta.parents, (Sa = Pa = {
+        data: Vi.data({
             field: "data",
             bindingEvent: "data",
             allowBinding: !0,
             allowSetting: !0,
             settingEvent: "data",
             settingTriggersEvent: !0,
             triggerFnName: "trigger",
@@ -4451,173 +4478,173 @@
                 id: !0,
                 source: !0,
                 target: !0,
                 parent: !0
             },
             updateStyle: !0
         }),
-        removeData: Oi.removeData({
+        removeData: Vi.removeData({
             field: "data",
             event: "data",
             triggerFnName: "trigger",
             triggerEvent: !0,
             immutableKeys: {
                 id: !0,
                 source: !0,
                 target: !0,
                 parent: !0
             },
             updateStyle: !0
         }),
-        scratch: Oi.data({
+        scratch: Vi.data({
             field: "scratch",
             bindingEvent: "scratch",
             allowBinding: !0,
             allowSetting: !0,
             settingEvent: "scratch",
             settingTriggersEvent: !0,
             triggerFnName: "trigger",
             allowGetting: !0,
             updateStyle: !0
         }),
-        removeScratch: Oi.removeData({
+        removeScratch: Vi.removeData({
             field: "scratch",
             event: "scratch",
             triggerFnName: "trigger",
             triggerEvent: !0,
             updateStyle: !0
         }),
-        rscratch: Oi.data({
+        rscratch: Vi.data({
             field: "rscratch",
             allowBinding: !1,
             allowSetting: !0,
             settingTriggersEvent: !1,
             allowGetting: !0
         }),
-        removeRscratch: Oi.removeData({
+        removeRscratch: Vi.removeData({
             field: "rscratch",
             triggerEvent: !1
         }),
         id: function() {
             var e = this[0];
             if (e) return e._private.data.id
         }
-    }).attr = ka.data, ka.removeAttr = ka.removeData;
-    var Ba, Na, za = Ca,
-        Ia = {};
+    }).attr = Sa.data, Sa.removeAttr = Sa.removeData;
+    var za, Ia, Aa = Pa,
+        La = {};
 
-    function La(e) {
+    function Oa(e) {
         return function(t) {
             if (void 0 === t && (t = !0), 0 !== this.length && this.isNode() && !this.removed()) {
                 for (var n = 0, r = this[0], i = r._private.edges, a = 0; a < i.length; a++) {
                     var o = i[a];
                     !t && o.isLoop() || (n += e(r, o))
                 }
                 return n
             }
         }
     }
 
-    function Aa(e, t) {
+    function Ra(e, t) {
         return function(n) {
             for (var r, i = this.nodes(), a = 0; a < i.length; a++) {
                 var o = i[a][e](n);
                 void 0 === o || void 0 !== r && !t(o, r) || (r = o)
             }
             return r
         }
     }
-    I(Ia, {
-        degree: La((function(e, t) {
+    A(La, {
+        degree: Oa((function(e, t) {
             return t.source().same(t.target()) ? 2 : 1
         })),
-        indegree: La((function(e, t) {
+        indegree: Oa((function(e, t) {
             return t.target().same(e) ? 1 : 0
         })),
-        outdegree: La((function(e, t) {
+        outdegree: Oa((function(e, t) {
             return t.source().same(e) ? 1 : 0
         }))
-    }), I(Ia, {
-        minDegree: Aa("degree", (function(e, t) {
+    }), A(La, {
+        minDegree: Ra("degree", (function(e, t) {
             return e < t
         })),
-        maxDegree: Aa("degree", (function(e, t) {
+        maxDegree: Ra("degree", (function(e, t) {
             return e > t
         })),
-        minIndegree: Aa("indegree", (function(e, t) {
+        minIndegree: Ra("indegree", (function(e, t) {
             return e < t
         })),
-        maxIndegree: Aa("indegree", (function(e, t) {
+        maxIndegree: Ra("indegree", (function(e, t) {
             return e > t
         })),
-        minOutdegree: Aa("outdegree", (function(e, t) {
+        minOutdegree: Ra("outdegree", (function(e, t) {
             return e < t
         })),
-        maxOutdegree: Aa("outdegree", (function(e, t) {
+        maxOutdegree: Ra("outdegree", (function(e, t) {
             return e > t
         }))
-    }), I(Ia, {
+    }), A(La, {
         totalDegree: function(e) {
             for (var t = 0, n = this.nodes(), r = 0; r < n.length; r++) t += n[r].degree(e);
             return t
         }
     });
-    var Oa = function(e, t, n) {
+    var Va = function(e, t, n) {
             for (var r = 0; r < e.length; r++) {
                 var i = e[r];
                 if (!i.locked()) {
                     var a = i._private.position,
                         o = {
                             x: null != t.x ? t.x - a.x : 0,
                             y: null != t.y ? t.y - a.y : 0
                         };
                     !i.isParent() || 0 === o.x && 0 === o.y || i.children().shift(o, n), i.dirtyBoundingBoxCache()
                 }
             }
         },
-        Ra = {
+        Fa = {
             field: "position",
             bindingEvent: "position",
             allowBinding: !0,
             allowSetting: !0,
             settingEvent: "position",
             settingTriggersEvent: !0,
             triggerFnName: "emitAndNotify",
             allowGetting: !0,
             validKeys: ["x", "y"],
             beforeGet: function(e) {
                 e.updateCompoundBounds()
             },
             beforeSet: function(e, t) {
-                Oa(e, t, !1)
+                Va(e, t, !1)
             },
             onSet: function(e) {
                 e.dirtyCompoundBoundsCache()
             },
             canSet: function(e) {
                 return !e.locked()
             }
         };
-    (Ba = Na = {
-        position: Oi.data(Ra),
-        silentPosition: Oi.data(I({}, Ra, {
+    (za = Ia = {
+        position: Vi.data(Fa),
+        silentPosition: Vi.data(A({}, Fa, {
             allowBinding: !1,
             allowSetting: !0,
             settingTriggersEvent: !1,
             allowGetting: !1,
             beforeSet: function(e, t) {
-                Oa(e, t, !0)
+                Va(e, t, !0)
             },
             onSet: function(e) {
                 e.dirtyCompoundBoundsCache()
             }
         })),
         positions: function(e, t) {
-            if (y(e)) t ? this.silentPosition(e) : this.position(e);
-            else if (g(e)) {
+            if (m(e)) t ? this.silentPosition(e) : this.position(e);
+            else if (v(e)) {
                 var n = e,
                     r = this.cy();
                 r.startBatch();
                 for (var i = 0; i < this.length; i++) {
                     var a, o = this[i];
                     (a = n(o, i)) && (t ? o.silentPosition(a) : o.position(a))
                 }
@@ -4626,18 +4653,18 @@
             return this
         },
         silentPositions: function(e) {
             return this.positions(e, !0)
         },
         shift: function(e, t, n) {
             var r;
-            if (y(e) ? (r = {
-                    x: m(e.x) ? e.x : 0,
-                    y: m(e.y) ? e.y : 0
-                }, n = t) : f(e) && m(t) && ((r = {
+            if (m(e) ? (r = {
+                    x: b(e.x) ? e.x : 0,
+                    y: b(e.y) ? e.y : 0
+                }, n = t) : g(e) && b(t) && ((r = {
                     x: 0,
                     y: 0
                 })[e] = t), null != r) {
                 var i = this.cy();
                 i.startBatch();
                 for (var a = 0; a < this.length; a++) {
                     var o = this[a];
@@ -4651,40 +4678,40 @@
                     }
                 }
                 i.endBatch()
             }
             return this
         },
         silentShift: function(e, t) {
-            return y(e) ? this.shift(e, !0) : f(e) && m(t) && this.shift(e, t, !0), this
+            return m(e) ? this.shift(e, !0) : g(e) && b(t) && this.shift(e, t, !0), this
         },
         renderedPosition: function(e, t) {
             var n = this[0],
                 r = this.cy(),
                 i = r.zoom(),
                 a = r.pan(),
-                o = y(e) ? e : void 0,
-                s = void 0 !== o || void 0 !== t && f(e);
+                o = m(e) ? e : void 0,
+                s = void 0 !== o || void 0 !== t && g(e);
             if (n && n.isNode()) {
                 if (!s) {
                     var l = n.position();
-                    return o = gt(l, i, a), void 0 === e ? o : o[e]
+                    return o = vt(l, i, a), void 0 === e ? o : o[e]
                 }
                 for (var u = 0; u < this.length; u++) {
                     var c = this[u];
-                    void 0 !== t ? c.position(e, (t - a[e]) / i) : void 0 !== o && c.position(vt(o, i, a))
+                    void 0 !== t ? c.position(e, (t - a[e]) / i) : void 0 !== o && c.position(yt(o, i, a))
                 }
             } else if (!s) return;
             return this
         },
         relativePosition: function(e, t) {
             var n = this[0],
                 r = this.cy(),
-                i = y(e) ? e : void 0,
-                a = void 0 !== i || void 0 !== t && f(e),
+                i = m(e) ? e : void 0,
+                a = void 0 !== i || void 0 !== t && g(e),
                 o = r.hasCompoundNodes();
             if (n && n.isNode()) {
                 if (!a) {
                     var s = n.position(),
                         l = o ? n.parent() : null,
                         u = l && l.length > 0,
                         c = u;
@@ -4696,33 +4723,33 @@
                     return i = {
                         x: s.x - d.x,
                         y: s.y - d.y
                     }, void 0 === e ? i : i[e]
                 }
                 for (var h = 0; h < this.length; h++) {
                     var p = this[h],
-                        g = o ? p.parent() : null,
-                        v = g && g.length > 0,
-                        m = v;
-                    v && (g = g[0]);
-                    var b = m ? g.position() : {
+                        f = o ? p.parent() : null,
+                        v = f && f.length > 0,
+                        y = v;
+                    v && (f = f[0]);
+                    var b = y ? f.position() : {
                         x: 0,
                         y: 0
                     };
                     void 0 !== t ? p.position(e, t + b[e]) : void 0 !== i && p.position({
                         x: i.x + b.x,
                         y: i.y + b.y
                     })
                 }
             } else if (!a) return;
             return this
         }
-    }).modelPosition = Ba.point = Ba.position, Ba.modelPositions = Ba.points = Ba.positions, Ba.renderedPoint = Ba.renderedPosition, Ba.relativePoint = Ba.relativePosition;
-    var Va, Fa, ja = Na;
-    Va = Fa = {}, Fa.renderedBoundingBox = function(e) {
+    }).modelPosition = za.point = za.position, za.modelPositions = za.points = za.positions, za.renderedPoint = za.renderedPosition, za.relativePoint = za.relativePosition;
+    var ja, qa, Ya = Ia;
+    ja = qa = {}, qa.renderedBoundingBox = function(e) {
         var t = this.boundingBox(e),
             n = this.cy(),
             r = n.zoom(),
             i = n.pan(),
             a = t.x1 * r + i.x,
             o = t.x2 * r + i.x,
             s = t.y1 * r + i.y,
@@ -4731,24 +4758,24 @@
             x1: a,
             x2: o,
             y1: s,
             y2: l,
             w: o - a,
             h: l - s
         }
-    }, Fa.dirtyCompoundBoundsCache = function() {
+    }, qa.dirtyCompoundBoundsCache = function() {
         var e = arguments.length > 0 && void 0 !== arguments[0] && arguments[0],
             t = this.cy();
         return t.styleEnabled() && t.hasCompoundNodes() ? (this.forEachUp((function(t) {
             if (t.isParent()) {
                 var n = t._private;
                 n.compoundBoundsClean = !1, n.bbCache = null, e || t.emitAndNotify("bounds")
             }
         })), this) : this
-    }, Fa.updateCompoundBounds = function() {
+    }, qa.updateCompoundBounds = function() {
         var e = arguments.length > 0 && void 0 !== arguments[0] && arguments[0],
             t = this.cy();
         if (!t.styleEnabled() || !t.hasCompoundNodes()) return this;
         if (!e && t.batching()) return this;
 
         function n(e) {
             if (e.isParent()) {
@@ -4823,52 +4850,52 @@
         for (var r = 0; r < this.length; r++) {
             var i = this[r],
                 a = i._private;
             a.compoundBoundsClean && !e || (n(i), t.batching() || (a.compoundBoundsClean = !0))
         }
         return this
     };
-    var qa = function(e) {
+    var Xa = function(e) {
             return e === 1 / 0 || e === -1 / 0 ? 0 : e
         },
-        Ya = function(e, t, n, r, i) {
+        Wa = function(e, t, n, r, i) {
             r - t != 0 && i - n != 0 && null != t && null != n && null != r && null != i && (e.x1 = t < e.x1 ? t : e.x1, e.x2 = r > e.x2 ? r : e.x2, e.y1 = n < e.y1 ? n : e.y1, e.y2 = i > e.y2 ? i : e.y2, e.w = e.x2 - e.x1, e.h = e.y2 - e.y1)
         },
-        Xa = function(e, t) {
-            return null == t ? e : Ya(e, t.x1, t.y1, t.x2, t.y2)
+        Ha = function(e, t) {
+            return null == t ? e : Wa(e, t.x1, t.y1, t.x2, t.y2)
         },
-        Wa = function(e, t, n) {
-            return Ke(e, t, n)
+        Ka = function(e, t, n) {
+            return Ge(e, t, n)
         },
-        Ha = function(e, t, n) {
+        Ga = function(e, t, n) {
             if (!t.cy().headless()) {
                 var r, i, a = t._private,
                     o = a.rstyle,
                     s = o.arrowWidth / 2;
                 if ("none" !== t.pstyle(n + "-arrow-shape").value) {
                     "source" === n ? (r = o.srcX, i = o.srcY) : "target" === n ? (r = o.tgtX, i = o.tgtY) : (r = o.midX, i = o.midY);
                     var l = a.arrowBounds = a.arrowBounds || {},
                         u = l[n] = l[n] || {};
-                    u.x1 = r - s, u.y1 = i - s, u.x2 = r + s, u.y2 = i + s, u.w = u.x2 - u.x1, u.h = u.y2 - u.y1, Mt(u, 1), Ya(e, u.x1, u.y1, u.x2, u.y2)
+                    u.x1 = r - s, u.y1 = i - s, u.x2 = r + s, u.y2 = i + s, u.w = u.x2 - u.x1, u.h = u.y2 - u.y1, Bt(u, 1), Wa(e, u.x1, u.y1, u.x2, u.y2)
                 }
             }
         },
-        Ka = function(e, t, n) {
+        Ua = function(e, t, n) {
             if (!t.cy().headless()) {
                 var r;
                 r = n ? n + "-" : "";
                 var i = t._private,
                     a = i.rstyle;
                 if (t.pstyle(r + "label").strValue) {
                     var o, s, l, u, c = t.pstyle("text-halign"),
                         d = t.pstyle("text-valign"),
-                        h = Wa(a, "labelWidth", n),
-                        p = Wa(a, "labelHeight", n),
-                        f = Wa(a, "labelX", n),
-                        g = Wa(a, "labelY", n),
+                        h = Ka(a, "labelWidth", n),
+                        p = Ka(a, "labelHeight", n),
+                        f = Ka(a, "labelX", n),
+                        g = Ka(a, "labelY", n),
                         v = t.pstyle(r + "text-margin-x").pfValue,
                         y = t.pstyle(r + "text-margin-y").pfValue,
                         m = t.isEdge(),
                         b = t.pstyle(r + "text-rotation"),
                         x = t.pstyle("text-outline-width").pfValue,
                         w = t.pstyle("text-border-width").pfValue / 2,
                         E = t.pstyle("text-background-padding").pfValue,
@@ -4903,59 +4930,59 @@
                     var D = n || "main",
                         T = i.labelBounds,
                         _ = T[D] = T[D] || {};
                     _.x1 = o, _.y1 = l, _.x2 = s, _.y2 = u, _.w = s - o, _.h = u - l;
                     var M = m && "autorotate" === b.strValue,
                         B = null != b.pfValue && 0 !== b.pfValue;
                     if (M || B) {
-                        var N = M ? Wa(i.rstyle, "labelAngle", n) : b.pfValue,
+                        var N = M ? Ka(i.rstyle, "labelAngle", n) : b.pfValue,
                             z = Math.cos(N),
                             I = Math.sin(N),
-                            L = (o + s) / 2,
-                            A = (l + u) / 2;
+                            A = (o + s) / 2,
+                            L = (l + u) / 2;
                         if (!m) {
                             switch (c.value) {
                                 case "left":
-                                    L = s;
+                                    A = s;
                                     break;
                                 case "right":
-                                    L = o
+                                    A = o
                             }
                             switch (d.value) {
                                 case "top":
-                                    A = u;
+                                    L = u;
                                     break;
                                 case "bottom":
-                                    A = l
+                                    L = l
                             }
                         }
                         var O = function(e, t) {
                                 return {
-                                    x: (e -= L) * z - (t -= A) * I + L,
-                                    y: e * I + t * z + A
+                                    x: (e -= A) * z - (t -= L) * I + A,
+                                    y: e * I + t * z + L
                                 }
                             },
                             R = O(o, l),
                             V = O(o, u),
                             F = O(s, l),
                             j = O(s, u);
                         o = Math.min(R.x, V.x, F.x, j.x), s = Math.max(R.x, V.x, F.x, j.x), l = Math.min(R.y, V.y, F.y, j.y), u = Math.max(R.y, V.y, F.y, j.y)
                     }
                     var q = D + "Rot",
                         Y = T[q] = T[q] || {};
-                    Y.x1 = o, Y.y1 = l, Y.x2 = s, Y.y2 = u, Y.w = s - o, Y.h = u - l, Ya(e, o, l, s, u), Ya(i.labelBounds.all, o, l, s, u)
+                    Y.x1 = o, Y.y1 = l, Y.x2 = s, Y.y2 = u, Y.w = s - o, Y.h = u - l, Wa(e, o, l, s, u), Wa(i.labelBounds.all, o, l, s, u)
                 }
                 return e
             }
         },
-        Ga = function(e, t) {
+        Za = function(e, t) {
             var n, r, i, a, o, s, l, u = e._private.cy,
                 c = u.styleEnabled(),
                 d = u.headless(),
-                h = Dt(),
+                h = Tt(),
                 p = e._private,
                 f = e.isNode(),
                 g = e.isEdge(),
                 v = p.rstyle,
                 y = f && c ? e.pstyle("bounds-expansion").pfValue : [0],
                 m = function(e) {
                     return "none" !== e.pstyle("display").value
@@ -4969,197 +4996,199 @@
                 var E = Math.max(x, w),
                     k = 0;
                 if (c && (k = e.pstyle("width").pfValue / 2), f && t.includeNodes) {
                     var C = e.position();
                     o = C.x, s = C.y;
                     var S = e.outerWidth() / 2,
                         P = e.outerHeight() / 2;
-                    Ya(h, n = o - S, i = s - P, r = o + S, a = s + P), c && t.includeOutlines && function(e, t) {
+                    Wa(h, n = o - S, i = s - P, r = o + S, a = s + P), c && t.includeOutlines && function(e, t) {
                         if (!t.cy().headless()) {
                             var n, r, i, a = t.pstyle("outline-opacity").value,
                                 o = t.pstyle("outline-width").value;
                             if (a > 0 && o > 0) {
                                 var s = t.pstyle("outline-offset").value,
                                     l = t.pstyle("shape").value,
                                     u = o + s,
                                     c = (e.w + 2 * u) / e.w,
                                     d = (e.h + 2 * u) / e.h,
                                     h = 0;
                                 ["diamond", "pentagon", "round-triangle"].includes(l) ? (c = (e.w + 2.4 * u) / e.w, h = -u / 3.6) : ["concave-hexagon", "rhomboid", "right-rhomboid"].includes(l) ? c = (e.w + 2.4 * u) / e.w : "star" === l ? (c = (e.w + 2.8 * u) / e.w, d = (e.h + 2.6 * u) / e.h, h = -u / 3.8) : "triangle" === l ? (c = (e.w + 2.8 * u) / e.w, d = (e.h + 2.4 * u) / e.h, h = -u / 1.4) : "vee" === l && (c = (e.w + 4.4 * u) / e.w, d = (e.h + 3.8 * u) / e.h, h = .5 * -u);
                                 var p = e.h * d - e.h,
                                     f = e.w * c - e.w;
-                                if (Bt(e, [Math.ceil(p / 2), Math.ceil(f / 2)]), 0 !== h) {
+                                if (Nt(e, [Math.ceil(p / 2), Math.ceil(f / 2)]), 0 !== h) {
                                     var g = (r = 0, i = h, {
                                         x1: (n = e).x1 + r,
                                         x2: n.x2 + r,
                                         y1: n.y1 + i,
                                         y2: n.y2 + i,
                                         w: n.w,
                                         h: n.h
                                     });
-                                    Tt(e, g)
+                                    _t(e, g)
                                 }
                             }
                         }
                     }(h, e)
                 } else if (g && t.includeEdges)
                     if (c && !d) {
                         var D = e.pstyle("curve-style").strValue;
-                        if (n = Math.min(v.srcX, v.midX, v.tgtX), r = Math.max(v.srcX, v.midX, v.tgtX), i = Math.min(v.srcY, v.midY, v.tgtY), a = Math.max(v.srcY, v.midY, v.tgtY), Ya(h, n -= k, i -= k, r += k, a += k), "haystack" === D) {
+                        if (n = Math.min(v.srcX, v.midX, v.tgtX), r = Math.max(v.srcX, v.midX, v.tgtX), i = Math.min(v.srcY, v.midY, v.tgtY), a = Math.max(v.srcY, v.midY, v.tgtY), Wa(h, n -= k, i -= k, r += k, a += k), "haystack" === D) {
                             var T = v.haystackPts;
                             if (T && 2 === T.length) {
                                 if (n = T[0].x, i = T[0].y, n > (r = T[1].x)) {
                                     var _ = n;
                                     n = r, r = _
                                 }
                                 if (i > (a = T[1].y)) {
                                     var M = i;
                                     i = a, a = M
                                 }
-                                Ya(h, n - k, i - k, r + k, a + k)
+                                Wa(h, n - k, i - k, r + k, a + k)
                             }
-                        } else if ("bezier" === D || "unbundled-bezier" === D || "segments" === D || "taxi" === D) {
+                        } else if ("bezier" === D || "unbundled-bezier" === D || D.endsWith("segments") || D.endsWith("taxi")) {
                             var B;
                             switch (D) {
                                 case "bezier":
                                 case "unbundled-bezier":
                                     B = v.bezierPts;
                                     break;
                                 case "segments":
                                 case "taxi":
+                                case "round-segments":
+                                case "round-taxi":
                                     B = v.linePts
                             }
                             if (null != B)
                                 for (var N = 0; N < B.length; N++) {
                                     var z = B[N];
-                                    n = z.x - k, r = z.x + k, i = z.y - k, a = z.y + k, Ya(h, n, i, r, a)
+                                    n = z.x - k, r = z.x + k, i = z.y - k, a = z.y + k, Wa(h, n, i, r, a)
                                 }
                         }
                     } else {
                         var I = e.source().position(),
-                            L = e.target().position();
-                        if ((n = I.x) > (r = L.x)) {
-                            var A = n;
-                            n = r, r = A
+                            A = e.target().position();
+                        if ((n = I.x) > (r = A.x)) {
+                            var L = n;
+                            n = r, r = L
                         }
-                        if ((i = I.y) > (a = L.y)) {
+                        if ((i = I.y) > (a = A.y)) {
                             var O = i;
                             i = a, a = O
                         }
-                        Ya(h, n -= k, i -= k, r += k, a += k)
-                    } if (c && t.includeEdges && g && (Ha(h, e, "mid-source"), Ha(h, e, "mid-target"), Ha(h, e, "source"), Ha(h, e, "target")), c)
+                        Wa(h, n -= k, i -= k, r += k, a += k)
+                    } if (c && t.includeEdges && g && (Ga(h, e, "mid-source"), Ga(h, e, "mid-target"), Ga(h, e, "source"), Ga(h, e, "target")), c)
                     if ("yes" === e.pstyle("ghost").value) {
                         var R = e.pstyle("ghost-offset-x").pfValue,
                             V = e.pstyle("ghost-offset-y").pfValue;
-                        Ya(h, h.x1 + R, h.y1 + V, h.x2 + R, h.y2 + V)
+                        Wa(h, h.x1 + R, h.y1 + V, h.x2 + R, h.y2 + V)
                     } var F = p.bodyBounds = p.bodyBounds || {};
-                Nt(F, h), Bt(F, y), Mt(F, 1), c && (n = h.x1, r = h.x2, i = h.y1, a = h.y2, Ya(h, n - E, i - E, r + E, a + E));
+                zt(F, h), Nt(F, y), Bt(F, 1), c && (n = h.x1, r = h.x2, i = h.y1, a = h.y2, Wa(h, n - E, i - E, r + E, a + E));
                 var j = p.overlayBounds = p.overlayBounds || {};
-                Nt(j, h), Bt(j, y), Mt(j, 1);
+                zt(j, h), Nt(j, y), Bt(j, 1);
                 var q = p.labelBounds = p.labelBounds || {};
-                null != q.all ? ((l = q.all).x1 = 1 / 0, l.y1 = 1 / 0, l.x2 = -1 / 0, l.y2 = -1 / 0, l.w = 0, l.h = 0) : q.all = Dt(), c && t.includeLabels && (t.includeMainLabels && Ka(h, e, null), g && (t.includeSourceLabels && Ka(h, e, "source"), t.includeTargetLabels && Ka(h, e, "target")))
+                null != q.all ? ((l = q.all).x1 = 1 / 0, l.y1 = 1 / 0, l.x2 = -1 / 0, l.y2 = -1 / 0, l.w = 0, l.h = 0) : q.all = Tt(), c && t.includeLabels && (t.includeMainLabels && Ua(h, e, null), g && (t.includeSourceLabels && Ua(h, e, "source"), t.includeTargetLabels && Ua(h, e, "target")))
             }
-            return h.x1 = qa(h.x1), h.y1 = qa(h.y1), h.x2 = qa(h.x2), h.y2 = qa(h.y2), h.w = qa(h.x2 - h.x1), h.h = qa(h.y2 - h.y1), h.w > 0 && h.h > 0 && b && (Bt(h, y), Mt(h, 1)), h
+            return h.x1 = Xa(h.x1), h.y1 = Xa(h.y1), h.x2 = Xa(h.x2), h.y2 = Xa(h.y2), h.w = Xa(h.x2 - h.x1), h.h = Xa(h.y2 - h.y1), h.w > 0 && h.h > 0 && b && (Nt(h, y), Bt(h, 1)), h
         },
-        Ua = function(e) {
+        $a = function(e) {
             var t = 0,
                 n = function(e) {
                     return (e ? 1 : 0) << t++
                 },
                 r = 0;
             return r += n(e.incudeNodes), r += n(e.includeEdges), r += n(e.includeLabels), r += n(e.includeMainLabels), r += n(e.includeSourceLabels), r += n(e.includeTargetLabels), r += n(e.includeOverlays), r += n(e.includeOutlines)
         },
-        Za = function(e) {
+        Qa = function(e) {
             if (e.isEdge()) {
                 var t = e.source().position(),
                     n = e.target().position(),
                     r = function(e) {
                         return Math.round(e)
                     };
                 return function(e, t) {
                     var n = {
                             value: 0,
                             done: !1
                         },
                         r = 0,
                         i = e.length;
-                    return we({
+                    return Ee({
                         next: function() {
                             return r < i ? n.value = e[r++] : n.done = !0, n
                         }
                     }, t)
                 }([r(t.x), r(t.y), r(n.x), r(n.y)])
             }
             return 0
         },
-        $a = function(e, t) {
+        Ja = function(e, t) {
             var n, r = e._private,
                 i = e.isEdge(),
-                a = (null == t ? Ja : Ua(t)) === Ja,
-                o = Za(e),
+                a = (null == t ? to : $a(t)) === to,
+                o = Qa(e),
                 s = r.bbCachePosKey === o,
                 l = t.useCache && s,
                 u = function(e) {
                     return null == e._private.bbCache || e._private.styleDirty
                 };
-            if (!l || u(e) || i && u(e.source()) || u(e.target()) ? (s || e.recalculateRenderedStyle(l), n = Ga(e, Qa), r.bbCache = n, r.bbCachePosKey = o) : n = r.bbCache, !a) {
+            if (!l || u(e) || i && u(e.source()) || u(e.target()) ? (s || e.recalculateRenderedStyle(l), n = Za(e, eo), r.bbCache = n, r.bbCachePosKey = o) : n = r.bbCache, !a) {
                 var c = e.isNode();
-                n = Dt(), (t.includeNodes && c || t.includeEdges && !c) && (t.includeOverlays ? Xa(n, r.overlayBounds) : Xa(n, r.bodyBounds)), t.includeLabels && (t.includeMainLabels && (!i || t.includeSourceLabels && t.includeTargetLabels) ? Xa(n, r.labelBounds.all) : (t.includeMainLabels && Xa(n, r.labelBounds.mainRot), t.includeSourceLabels && Xa(n, r.labelBounds.sourceRot), t.includeTargetLabels && Xa(n, r.labelBounds.targetRot))), n.w = n.x2 - n.x1, n.h = n.y2 - n.y1
+                n = Tt(), (t.includeNodes && c || t.includeEdges && !c) && (t.includeOverlays ? Ha(n, r.overlayBounds) : Ha(n, r.bodyBounds)), t.includeLabels && (t.includeMainLabels && (!i || t.includeSourceLabels && t.includeTargetLabels) ? Ha(n, r.labelBounds.all) : (t.includeMainLabels && Ha(n, r.labelBounds.mainRot), t.includeSourceLabels && Ha(n, r.labelBounds.sourceRot), t.includeTargetLabels && Ha(n, r.labelBounds.targetRot))), n.w = n.x2 - n.x1, n.h = n.y2 - n.y1
             }
             return n
         },
-        Qa = {
+        eo = {
             includeNodes: !0,
             includeEdges: !0,
             includeLabels: !0,
             includeMainLabels: !0,
             includeSourceLabels: !0,
             includeTargetLabels: !0,
             includeOverlays: !0,
             includeUnderlays: !0,
             includeOutlines: !0,
             useCache: !0
         },
-        Ja = Ua(Qa),
-        eo = Xe(Qa);
-    Fa.boundingBox = function(e) {
+        to = $a(eo),
+        no = We(eo);
+    qa.boundingBox = function(e) {
         var t;
         if (1 !== this.length || null == this[0]._private.bbCache || this[0]._private.styleDirty || void 0 !== e && void 0 !== e.useCache && !0 !== e.useCache) {
-            t = Dt();
-            var n = eo(e = e || Qa);
+            t = Tt();
+            var n = no(e = e || eo);
             if (this.cy().styleEnabled())
                 for (var r = 0; r < this.length; r++) {
                     var i = this[r],
                         a = i._private,
-                        o = Za(i),
+                        o = Qa(i),
                         s = a.bbCachePosKey === o,
                         l = n.useCache && s && !a.styleDirty;
                     i.recalculateRenderedStyle(l)
                 }
             this.updateCompoundBounds(!e.useCache);
             for (var u = 0; u < this.length; u++) {
                 var c = this[u];
-                Xa(t, $a(c, n))
+                Ha(t, Ja(c, n))
             }
-        } else e = void 0 === e ? Qa : eo(e), t = $a(this[0], e);
-        return t.x1 = qa(t.x1), t.y1 = qa(t.y1), t.x2 = qa(t.x2), t.y2 = qa(t.y2), t.w = qa(t.x2 - t.x1), t.h = qa(t.y2 - t.y1), t
-    }, Fa.dirtyBoundingBoxCache = function() {
+        } else e = void 0 === e ? eo : no(e), t = Ja(this[0], e);
+        return t.x1 = Xa(t.x1), t.y1 = Xa(t.y1), t.x2 = Xa(t.x2), t.y2 = Xa(t.y2), t.w = Xa(t.x2 - t.x1), t.h = Xa(t.y2 - t.y1), t
+    }, qa.dirtyBoundingBoxCache = function() {
         for (var e = 0; e < this.length; e++) {
             var t = this[e]._private;
             t.bbCache = null, t.bbCachePosKey = null, t.bodyBounds = null, t.overlayBounds = null, t.labelBounds.all = null, t.labelBounds.source = null, t.labelBounds.target = null, t.labelBounds.main = null, t.labelBounds.sourceRot = null, t.labelBounds.targetRot = null, t.labelBounds.mainRot = null, t.arrowBounds.source = null, t.arrowBounds.target = null, t.arrowBounds["mid-source"] = null, t.arrowBounds["mid-target"] = null
         }
         return this.emitAndNotify("bounds"), this
-    }, Fa.boundingBoxAt = function(e) {
+    }, qa.boundingBoxAt = function(e) {
         var t = this.nodes(),
             n = this.cy(),
             r = n.hasCompoundNodes(),
             i = n.collection();
         if (r && (i = t.filter((function(e) {
                 return e.isParent()
-            })), t = t.not(i)), y(e)) {
+            })), t = t.not(i)), m(e)) {
             var a = e;
             e = function() {
                 return a
             }
         }
         n.startBatch(), t.forEach((function(t, n) {
             return t._private.bbAtOldPos = e(t, n)
@@ -5175,62 +5204,62 @@
             }
         }(this.boundingBox({
             useCache: !1
         }));
         return t.silentPositions((function(e) {
             return e._private.bbAtOldPos
         })), r && (i.dirtyCompoundBoundsCache(), i.dirtyBoundingBoxCache(), i.updateCompoundBounds(!0)), n.endBatch(), o
-    }, Va.boundingbox = Va.bb = Va.boundingBox, Va.renderedBoundingbox = Va.renderedBoundingBox;
-    var to, no, ro = Fa;
-    to = no = {};
-    var io = function(e) {
-        e.uppercaseName = B(e.name), e.autoName = "auto" + e.uppercaseName, e.labelName = "label" + e.uppercaseName, e.outerName = "outer" + e.uppercaseName, e.uppercaseOuterName = B(e.outerName), to[e.name] = function() {
+    }, ja.boundingbox = ja.bb = ja.boundingBox, ja.renderedBoundingbox = ja.renderedBoundingBox;
+    var ro, io, ao = qa;
+    ro = io = {};
+    var oo = function(e) {
+        e.uppercaseName = N(e.name), e.autoName = "auto" + e.uppercaseName, e.labelName = "label" + e.uppercaseName, e.outerName = "outer" + e.uppercaseName, e.uppercaseOuterName = N(e.outerName), ro[e.name] = function() {
             var t = this[0],
                 n = t._private,
                 r = n.cy._private.styleEnabled;
             if (t) {
                 if (!r) return 1;
                 if (t.isParent()) return t.updateCompoundBounds(), n[e.autoName] || 0;
                 var i = t.pstyle(e.name);
                 switch (i.strValue) {
                     case "label":
                         return t.recalculateRenderedStyle(), n.rstyle[e.labelName] || 0;
                     default:
                         return i.pfValue
                 }
             }
-        }, to["outer" + e.uppercaseName] = function() {
+        }, ro["outer" + e.uppercaseName] = function() {
             var t = this[0],
                 n = t._private.cy._private.styleEnabled;
             if (t) return n ? t[e.name]() + t.pstyle("border-width").pfValue + 2 * t.padding() : 1
-        }, to["rendered" + e.uppercaseName] = function() {
+        }, ro["rendered" + e.uppercaseName] = function() {
             var t = this[0];
             if (t) return t[e.name]() * this.cy().zoom()
-        }, to["rendered" + e.uppercaseOuterName] = function() {
+        }, ro["rendered" + e.uppercaseOuterName] = function() {
             var t = this[0];
             if (t) return t[e.outerName]() * this.cy().zoom()
         }
     };
-    io({
+    oo({
         name: "width"
-    }), io({
+    }), oo({
         name: "height"
-    }), no.padding = function() {
+    }), io.padding = function() {
         var e = this[0],
             t = e._private;
         return e.isParent() ? (e.updateCompoundBounds(), void 0 !== t.autoPadding ? t.autoPadding : e.pstyle("padding").pfValue) : e.pstyle("padding").pfValue
-    }, no.paddedHeight = function() {
+    }, io.paddedHeight = function() {
         var e = this[0];
         return e.height() + 2 * e.padding()
-    }, no.paddedWidth = function() {
+    }, io.paddedWidth = function() {
         var e = this[0];
         return e.width() + 2 * e.padding()
     };
-    var ao = no,
-        oo = {
+    var so = io,
+        lo = {
             controlPoints: {
                 get: function(e) {
                     return e.renderer().getControlPoints(e)
                 },
                 mult: !0
             },
             segmentPoints: {
@@ -5251,90 +5280,90 @@
             },
             midpoint: {
                 get: function(e) {
                     return e.renderer().getEdgeMidpoint(e)
                 }
             }
         },
-        so = Object.keys(oo).reduce((function(e, t) {
-            var n = oo[t],
+        uo = Object.keys(lo).reduce((function(e, t) {
+            var n = lo[t],
                 r = function(e) {
                     return "rendered" + e[0].toUpperCase() + e.substr(1)
                 }(t);
             return e[t] = function() {
                 return function(e, t) {
                     if (e.isEdge()) return t(e)
                 }(this, n.get)
             }, n.mult ? e[r] = function() {
                 return function(e, t) {
                     if (e.isEdge()) {
                         var n = e.cy(),
                             r = n.pan(),
                             i = n.zoom();
                         return t(e).map((function(e) {
-                            return gt(e, i, r)
+                            return vt(e, i, r)
                         }))
                     }
                 }(this, n.get)
             } : e[r] = function() {
                 return function(e, t) {
                     if (e.isEdge()) {
                         var n = e.cy();
-                        return gt(t(e), n.zoom(), n.pan())
+                        return vt(t(e), n.zoom(), n.pan())
                     }
                 }(this, n.get)
             }, e
         }), {}),
-        lo = I({}, ja, ro, ao, so),
-        uo = function(e, t) {
+        co = A({}, Ya, ao, so, uo),
+        ho = function(e, t) {
             this.recycle(e, t)
         };
 
-    function co() {
+    function po() {
         return !1
     }
 
-    function ho() {
+    function fo() {
         return !0
     }
-    uo.prototype = {
+    ho.prototype = {
         instanceString: function() {
             return "event"
         },
         recycle: function(e, t) {
-            if (this.isImmediatePropagationStopped = this.isPropagationStopped = this.isDefaultPrevented = co, null != e && e.preventDefault ? (this.type = e.type, this.isDefaultPrevented = e.defaultPrevented ? ho : co) : null != e && e.type ? t = e : this.type = e, null != t && (this.originalEvent = t.originalEvent, this.type = null != t.type ? t.type : this.type, this.cy = t.cy, this.target = t.target, this.position = t.position, this.renderedPosition = t.renderedPosition, this.namespace = t.namespace, this.layout = t.layout), null != this.cy && null != this.position && null == this.renderedPosition) {
+            if (this.isImmediatePropagationStopped = this.isPropagationStopped = this.isDefaultPrevented = po, null != e && e.preventDefault ? (this.type = e.type, this.isDefaultPrevented = e.defaultPrevented ? fo : po) : null != e && e.type ? t = e : this.type = e, null != t && (this.originalEvent = t.originalEvent, this.type = null != t.type ? t.type : this.type, this.cy = t.cy, this.target = t.target, this.position = t.position, this.renderedPosition = t.renderedPosition, this.namespace = t.namespace, this.layout = t.layout), null != this.cy && null != this.position && null == this.renderedPosition) {
                 var n = this.position,
                     r = this.cy.zoom(),
                     i = this.cy.pan();
                 this.renderedPosition = {
                     x: n.x * r + i.x,
                     y: n.y * r + i.y
                 }
             }
             this.timeStamp = e && e.timeStamp || Date.now()
         },
         preventDefault: function() {
-            this.isDefaultPrevented = ho;
+            this.isDefaultPrevented = fo;
             var e = this.originalEvent;
             e && e.preventDefault && e.preventDefault()
         },
         stopPropagation: function() {
-            this.isPropagationStopped = ho;
+            this.isPropagationStopped = fo;
             var e = this.originalEvent;
             e && e.stopPropagation && e.stopPropagation()
         },
         stopImmediatePropagation: function() {
-            this.isImmediatePropagationStopped = ho, this.stopPropagation()
+            this.isImmediatePropagationStopped = fo, this.stopPropagation()
         },
-        isDefaultPrevented: co,
-        isPropagationStopped: co,
-        isImmediatePropagationStopped: co
+        isDefaultPrevented: po,
+        isPropagationStopped: po,
+        isImmediatePropagationStopped: po
     };
-    var po = /^([^.]+)(\.(?:[^.]+))?$/,
-        fo = {
+    var go = /^([^.]+)(\.(?:[^.]+))?$/,
+        vo = {
             qualifierCompare: function(e, t) {
                 return e === t
             },
             eventMatches: function() {
                 return !0
             },
             addEventFields: function() {},
@@ -5347,90 +5376,90 @@
                 return !1
             },
             parent: function() {
                 return null
             },
             context: null
         },
-        go = Object.keys(fo),
-        vo = {};
+        yo = Object.keys(vo),
+        mo = {};
 
-    function yo() {
-        for (var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : vo, t = arguments.length > 1 ? arguments[1] : void 0, n = 0; n < go.length; n++) {
-            var r = go[n];
-            this[r] = e[r] || fo[r]
+    function bo() {
+        for (var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : mo, t = arguments.length > 1 ? arguments[1] : void 0, n = 0; n < yo.length; n++) {
+            var r = yo[n];
+            this[r] = e[r] || vo[r]
         }
         this.context = t || this.context, this.listeners = [], this.emitting = 0
     }
-    var mo = yo.prototype,
-        bo = function(e, t, n, r, i, a, o) {
-            g(r) && (i = r, r = null), o && (a = null == a ? o : I({}, a, o));
-            for (var s = v(n) ? n : n.split(/\s+/), l = 0; l < s.length; l++) {
+    var xo = bo.prototype,
+        wo = function(e, t, n, r, i, a, o) {
+            v(r) && (i = r, r = null), o && (a = null == a ? o : A({}, a, o));
+            for (var s = y(n) ? n : n.split(/\s+/), l = 0; l < s.length; l++) {
                 var u = s[l];
-                if (!S(u)) {
-                    var c = u.match(po);
+                if (!P(u)) {
+                    var c = u.match(go);
                     if (c)
                         if (!1 === t(e, u, c[1], c[2] ? c[2] : null, r, i, a)) break
                 }
             }
         },
-        xo = function(e, t) {
-            return e.addEventFields(e.context, t), new uo(t.type, t)
+        Eo = function(e, t) {
+            return e.addEventFields(e.context, t), new ho(t.type, t)
         },
-        wo = function(e, t, n) {
-            if ("event" !== p(n))
-                if (y(n)) t(e, xo(e, n));
+        ko = function(e, t, n) {
+            if ("event" !== f(n))
+                if (m(n)) t(e, Eo(e, n));
                 else
-                    for (var r = v(n) ? n : n.split(/\s+/), i = 0; i < r.length; i++) {
+                    for (var r = y(n) ? n : n.split(/\s+/), i = 0; i < r.length; i++) {
                         var a = r[i];
-                        if (!S(a)) {
-                            var o = a.match(po);
+                        if (!P(a)) {
+                            var o = a.match(go);
                             if (o) {
                                 var s = o[1],
                                     l = o[2] ? o[2] : null;
-                                t(e, xo(e, {
+                                t(e, Eo(e, {
                                     type: s,
                                     namespace: l,
                                     target: e.context
                                 }))
                             }
                         }
                     } else t(e, n)
         };
-    mo.on = mo.addListener = function(e, t, n, r, i) {
-        return bo(this, (function(e, t, n, r, i, a, o) {
-            g(a) && e.listeners.push({
+    xo.on = xo.addListener = function(e, t, n, r, i) {
+        return wo(this, (function(e, t, n, r, i, a, o) {
+            v(a) && e.listeners.push({
                 event: t,
                 callback: a,
                 type: n,
                 namespace: r,
                 qualifier: i,
                 conf: o
             })
         }), e, t, n, r, i), this
-    }, mo.one = function(e, t, n, r) {
+    }, xo.one = function(e, t, n, r) {
         return this.on(e, t, n, r, {
             one: !0
         })
-    }, mo.removeListener = mo.off = function(e, t, n, r) {
+    }, xo.removeListener = xo.off = function(e, t, n, r) {
         var i = this;
         0 !== this.emitting && (this.listeners = this.listeners.slice());
         for (var a = this.listeners, o = function(o) {
                 var s = a[o];
-                bo(i, (function(t, n, r, i, l, u) {
+                wo(i, (function(t, n, r, i, l, u) {
                     if ((s.type === r || "*" === e) && (!i && ".*" !== s.namespace || s.namespace === i) && (!l || t.qualifierCompare(s.qualifier, l)) && (!u || s.callback === u)) return a.splice(o, 1), !1
                 }), e, t, n, r)
             }, s = a.length - 1; s >= 0; s--) o(s);
         return this
-    }, mo.removeAllListeners = function() {
+    }, xo.removeAllListeners = function() {
         return this.removeListener("*")
-    }, mo.emit = mo.trigger = function(e, t, n) {
+    }, xo.emit = xo.trigger = function(e, t, n) {
         var r = this.listeners,
             i = r.length;
-        return this.emitting++, v(t) || (t = [t]), wo(this, (function(e, a) {
+        return this.emitting++, y(t) || (t = [t]), ko(this, (function(e, a) {
             null != n && (r = [{
                 event: a.event,
                 type: a.type,
                 namespace: a.namespace,
                 callback: n
             }], i = r.length);
             for (var o = function(n) {
@@ -5449,21 +5478,21 @@
                             l = i.callback.apply(s, o);
                         e.afterEmit(e.context, i, a), !1 === l && (a.stopPropagation(), a.preventDefault())
                     }
                 }, s = 0; s < i; s++) o(s);
             e.bubble(e.context) && !a.isPropagationStopped() && e.parent(e.context).emit(a, t)
         }), e), this.emitting--, this
     };
-    var Eo = {
+    var Co = {
             qualifierCompare: function(e, t) {
                 return null == e || null == t ? null == e && null == t : e.sameText(t)
             },
             eventMatches: function(e, t, n) {
                 var r = t.qualifier;
-                return null == r || e !== n.target && w(n.target) && r.matches(n.target)
+                return null == r || e !== n.target && E(n.target) && r.matches(n.target)
             },
             addEventFields: function(e, t) {
                 t.cy = e.cy(), t.target = e
             },
             callbackContext: function(e, t, n) {
                 return null != t.qualifier ? n.target : e
             },
@@ -5473,55 +5502,55 @@
             bubble: function() {
                 return !0
             },
             parent: function(e) {
                 return e.isChild() ? e.parent() : e.cy()
             }
         },
-        ko = function(e) {
-            return f(e) ? new xa(e) : e
+        So = function(e) {
+            return g(e) ? new Ea(e) : e
         },
-        Co = {
+        Po = {
             createEmitter: function() {
                 for (var e = 0; e < this.length; e++) {
                     var t = this[e],
                         n = t._private;
-                    n.emitter || (n.emitter = new yo(Eo, t))
+                    n.emitter || (n.emitter = new bo(Co, t))
                 }
                 return this
             },
             emitter: function() {
                 return this._private.emitter
             },
             on: function(e, t, n) {
-                for (var r = ko(t), i = 0; i < this.length; i++) {
+                for (var r = So(t), i = 0; i < this.length; i++) {
                     this[i].emitter().on(e, r, n)
                 }
                 return this
             },
             removeListener: function(e, t, n) {
-                for (var r = ko(t), i = 0; i < this.length; i++) {
+                for (var r = So(t), i = 0; i < this.length; i++) {
                     this[i].emitter().removeListener(e, r, n)
                 }
                 return this
             },
             removeAllListeners: function() {
                 for (var e = 0; e < this.length; e++) {
                     this[e].emitter().removeAllListeners()
                 }
                 return this
             },
             one: function(e, t, n) {
-                for (var r = ko(t), i = 0; i < this.length; i++) {
+                for (var r = So(t), i = 0; i < this.length; i++) {
                     this[i].emitter().one(e, r, n)
                 }
                 return this
             },
             once: function(e, t, n) {
-                for (var r = ko(t), i = 0; i < this.length; i++) {
+                for (var r = So(t), i = 0; i < this.length; i++) {
                     this[i].emitter().on(e, r, n, {
                         once: !0,
                         onceCollection: this
                     })
                 }
             },
             emit: function(e, t) {
@@ -5530,16 +5559,16 @@
                 }
                 return this
             },
             emitAndNotify: function(e, t) {
                 if (0 !== this.length) return this.cy().notify(e, this), this.emit(e, t), this
             }
         };
-    Oi.eventAliasesOn(Co);
-    var So = {
+    Vi.eventAliasesOn(Po);
+    var Do = {
             nodes: function(e) {
                 return this.filter((function(e) {
                     return e.isNode()
                 })).filter(e)
             },
             edges: function(e) {
                 return this.filter((function(e) {
@@ -5554,66 +5583,66 @@
                 return {
                     nodes: e,
                     edges: t
                 }
             },
             filter: function(e, t) {
                 if (void 0 === e) return this;
-                if (f(e) || x(e)) return new xa(e).filter(this);
-                if (g(e)) {
+                if (g(e) || w(e)) return new Ea(e).filter(this);
+                if (v(e)) {
                     for (var n = this.spawn(), r = 0; r < this.length; r++) {
                         var i = this[r];
                         (t ? e.apply(t, [i, r, this]) : e(i, r, this)) && n.push(i)
                     }
                     return n
                 }
                 return this.spawn()
             },
             not: function(e) {
                 if (e) {
-                    f(e) && (e = this.filter(e));
+                    g(e) && (e = this.filter(e));
                     for (var t = this.spawn(), n = 0; n < this.length; n++) {
                         var r = this[n];
                         e.has(r) || t.push(r)
                     }
                     return t
                 }
                 return this
             },
             absoluteComplement: function() {
                 return this.cy().mutableElements().not(this)
             },
             intersect: function(e) {
-                if (f(e)) {
+                if (g(e)) {
                     var t = e;
                     return this.filter(t)
                 }
                 for (var n = this.spawn(), r = e, i = this.length < e.length, a = i ? this : r, o = i ? r : this, s = 0; s < a.length; s++) {
                     var l = a[s];
                     o.has(l) && n.push(l)
                 }
                 return n
             },
             xor: function(e) {
                 var t = this._private.cy;
-                f(e) && (e = t.$(e));
+                g(e) && (e = t.$(e));
                 var n = this.spawn(),
                     r = e,
                     i = function(e, t) {
                         for (var r = 0; r < e.length; r++) {
                             var i = e[r],
                                 a = i._private.data.id;
                             t.hasElementWithId(a) || n.push(i)
                         }
                     };
                 return i(this, r), i(r, this), n
             },
             diff: function(e) {
                 var t = this._private.cy;
-                f(e) && (e = t.$(e));
+                g(e) && (e = t.$(e));
                 var n = this.spawn(),
                     r = this.spawn(),
                     i = this.spawn(),
                     a = e,
                     o = function(e, t, n) {
                         for (var r = 0; r < e.length; r++) {
                             var a = e[r],
@@ -5626,30 +5655,30 @@
                     right: r,
                     both: i
                 }
             },
             add: function(e) {
                 var t = this._private.cy;
                 if (!e) return this;
-                if (f(e)) {
+                if (g(e)) {
                     var n = e;
                     e = t.mutableElements().filter(n)
                 }
                 for (var r = this.spawnSelf(), i = 0; i < e.length; i++) {
                     var a = e[i],
                         o = !this.has(a);
                     o && r.push(a)
                 }
                 return r
             },
             merge: function(e) {
                 var t = this._private,
                     n = t.cy;
                 if (!e) return this;
-                if (e && f(e)) {
+                if (e && g(e)) {
                     var r = e;
                     e = n.mutableElements().filter(r)
                 }
                 for (var i = t.map, a = 0; a < e.length; a++) {
                     var o = e[a],
                         s = o._private.data.id;
                     if (!i.has(s)) {
@@ -5686,15 +5715,15 @@
                 if (!r) return this;
                 var i = r.index;
                 return this.unmergeAt(i), this
             },
             unmerge: function(e) {
                 var t = this._private.cy;
                 if (!e) return this;
-                if (e && f(e)) {
+                if (e && g(e)) {
                     var n = e;
                     e = t.mutableElements().filter(n)
                 }
                 for (var r = 0; r < e.length; r++) this.unmergeOne(e[r]);
                 return this
             },
             unmergeBy: function(e) {
@@ -5734,37 +5763,37 @@
                 }
                 return {
                     value: r,
                     ele: n
                 }
             }
         },
-        Po = So;
-    Po.u = Po["|"] = Po["+"] = Po.union = Po.or = Po.add, Po["\\"] = Po["!"] = Po["-"] = Po.difference = Po.relativeComplement = Po.subtract = Po.not, Po.n = Po["&"] = Po["."] = Po.and = Po.intersection = Po.intersect, Po["^"] = Po["(+)"] = Po["(-)"] = Po.symmetricDifference = Po.symdiff = Po.xor, Po.fnFilter = Po.filterFn = Po.stdFilter = Po.filter, Po.complement = Po.abscomp = Po.absoluteComplement;
-    var Do = function(e, t) {
+        To = Do;
+    To.u = To["|"] = To["+"] = To.union = To.or = To.add, To["\\"] = To["!"] = To["-"] = To.difference = To.relativeComplement = To.subtract = To.not, To.n = To["&"] = To["."] = To.and = To.intersection = To.intersect, To["^"] = To["(+)"] = To["(-)"] = To.symmetricDifference = To.symdiff = To.xor, To.fnFilter = To.filterFn = To.stdFilter = To.filter, To.complement = To.abscomp = To.absoluteComplement;
+    var _o = function(e, t) {
             var n = e.cy().hasCompoundNodes();
 
             function r(e) {
                 var t = e.pstyle("z-compound-depth");
-                return "auto" === t.value ? n ? e.zDepth() : 0 : "bottom" === t.value ? -1 : "top" === t.value ? Ne : 0
+                return "auto" === t.value ? n ? e.zDepth() : 0 : "bottom" === t.value ? -1 : "top" === t.value ? ze : 0
             }
             var i = r(e) - r(t);
             if (0 !== i) return i;
 
             function a(e) {
                 return "auto" === e.pstyle("z-index-compare").value && e.isNode() ? 1 : 0
             }
             var o = a(e) - a(t);
             if (0 !== o) return o;
             var s = e.pstyle("z-index").value - t.pstyle("z-index").value;
             return 0 !== s ? s : e.poolIndex() - t.poolIndex()
         },
-        To = {
+        Mo = {
             forEach: function(e, t) {
-                if (g(e))
+                if (v(e))
                     for (var n = this.length, r = 0; r < n; r++) {
                         var i = this[r];
                         if (!1 === (t ? e.apply(t, [i, r, this]) : e(i, r, this))) break
                     }
                 return this
             },
             toArray: function() {
@@ -5793,39 +5822,39 @@
             empty: function() {
                 return 0 === this.length
             },
             nonempty: function() {
                 return !this.empty()
             },
             sort: function(e) {
-                if (!g(e)) return this;
+                if (!v(e)) return this;
                 var t = this.toArray().sort(e);
                 return this.spawn(t)
             },
             sortByZIndex: function() {
-                return this.sort(Do)
+                return this.sort(_o)
             },
             zDepth: function() {
                 var e = this[0];
                 if (e) {
                     var t = e._private;
                     if ("nodes" === t.group) {
                         var n = t.data.parent ? e.parents().size() : 0;
-                        return e.isParent() ? n : Ne - 1
+                        return e.isParent() ? n : ze - 1
                     }
                     var r = t.source,
                         i = t.target,
                         a = r.zDepth(),
                         o = i.zDepth();
                     return Math.max(a, o, 0)
                 }
             }
         };
-    To.each = To.forEach;
-    "undefined" != ("undefined" == typeof Symbol ? "undefined" : e(Symbol)) && "undefined" != e(Symbol.iterator) && (To[Symbol.iterator] = function() {
+    Mo.each = Mo.forEach;
+    "undefined" != ("undefined" == typeof Symbol ? "undefined" : e(Symbol)) && "undefined" != e(Symbol.iterator) && (Mo[Symbol.iterator] = function() {
         var e = this,
             t = {
                 value: void 0,
                 done: !1
             },
             n = 0,
             r = this.length;
@@ -5833,21 +5862,21 @@
             next: function() {
                 return n < r ? t.value = e[n++] : (t.value = void 0, t.done = !0), t
             }
         }, Symbol.iterator, (function() {
             return this
         }))
     });
-    var _o = Xe({
+    var Bo = We({
             nodeDimensionsIncludeLabels: !1
         }),
-        Mo = {
+        No = {
             layoutDimensions: function(e) {
                 var t;
-                if (e = _o(e), this.takesUpSpace())
+                if (e = Bo(e), this.takesUpSpace())
                     if (e.nodeDimensionsIncludeLabels) {
                         var n = this.boundingBox();
                         t = {
                             w: n.w,
                             h: n.h
                         }
                     } else t = {
@@ -5865,30 +5894,30 @@
                         return !e.isParent()
                     })),
                     i = this.cy(),
                     a = t.eles,
                     o = function(e) {
                         return e.id()
                     },
-                    s = D(n, o);
+                    s = T(n, o);
                 e.emit({
                     type: "layoutstart",
                     layout: e
                 }), e.animations = [];
                 var l = t.spacingFactor && 1 !== t.spacingFactor,
                     u = function() {
                         if (!l) return null;
-                        for (var e = Dt(), t = 0; t < r.length; t++) {
+                        for (var e = Tt(), t = 0; t < r.length; t++) {
                             var n = r[t],
                                 i = s(n, t);
-                            _t(e, i.x, i.y)
+                            Mt(e, i.x, i.y)
                         }
                         return e
                     }(),
-                    c = D((function(e, n) {
+                    c = T((function(e, n) {
                         var r = s(e, n);
                         l && (r = function(e, t, n) {
                             var r = t.x1 + t.w / 2,
                                 i = t.y1 + t.h / 2;
                             return {
                                 x: r + (n.x - r) * e,
                                 y: i + (n.y - i) * e
@@ -5929,15 +5958,15 @@
                         e.animations.push(v)
                     }
                     e.animations.forEach((function(e) {
                         return e.play()
                     })), e.one("layoutready", t.ready), e.emit({
                         type: "layoutready",
                         layout: e
-                    }), pr.all(e.animations.map((function(e) {
+                    }), gr.all(e.animations.map((function(e) {
                         return e.promise()
                     }))).then((function() {
                         e.one("layoutstop", t.stop), e.emit({
                             type: "layoutstop",
                             layout: e
                         })
                     }))
@@ -5947,45 +5976,45 @@
                 }), e.one("layoutstop", t.stop), e.emit({
                     type: "layoutstop",
                     layout: e
                 });
                 return this
             },
             layout: function(e) {
-                return this.cy().makeLayout(I({}, e, {
+                return this.cy().makeLayout(A({}, e, {
                     eles: this
                 }))
             }
         };
 
-    function Bo(e, t, n) {
+    function zo(e, t, n) {
         var r, i = n._private,
             a = i.styleCache = i.styleCache || [];
         return null != (r = a[e]) ? r : r = a[e] = t(n)
     }
 
-    function No(e, t) {
-        return e = Pe(e),
+    function Io(e, t) {
+        return e = De(e),
             function(n) {
-                return Bo(e, t, n)
+                return zo(e, t, n)
             }
     }
 
-    function zo(e, t) {
-        e = Pe(e);
+    function Ao(e, t) {
+        e = De(e);
         var n = function(e) {
             return t.call(e)
         };
         return function() {
             var t = this[0];
-            if (t) return Bo(e, n, t)
+            if (t) return zo(e, n, t)
         }
     }
-    Mo.createLayout = Mo.makeLayout = Mo.layout;
-    var Io = {
+    No.createLayout = No.makeLayout = No.layout;
+    var Lo = {
         recalculateRenderedStyle: function(e) {
             var t = this.cy(),
                 n = t.renderer(),
                 r = t.styleEnabled();
             return n && r && n.recalculateRenderedStyle(this, e), this
         },
         dirtyStyleCache: function() {
@@ -6044,18 +6073,18 @@
             var n = this[0];
             return n ? t.style().getRenderedStyle(n, e) : void 0
         },
         style: function(e, t) {
             var n = this.cy();
             if (!n.styleEnabled()) return this;
             var r = n.style();
-            if (y(e)) {
+            if (m(e)) {
                 var i = e;
                 r.applyBypass(this, i, !1), this.emitAndNotify("style")
-            } else if (f(e)) {
+            } else if (g(e)) {
                 if (void 0 === t) {
                     var a = this[0];
                     return a ? r.getStylePropertyValue(a, e) : void 0
                 }
                 r.applyBypass(this, e, t, !1), this.emitAndNotify("style")
             } else if (void 0 === e) {
                 var o = this[0];
@@ -6110,89 +6139,89 @@
             return e ? t ? 0 === e.effectiveOpacity() : 0 === e.pstyle("opacity").value : void 0
         },
         backgrounding: function() {
             return !!this.cy().styleEnabled() && !!this[0]._private.backgrounding
         }
     };
 
-    function Lo(e, t) {
+    function Oo(e, t) {
         var n = e._private.data.parent ? e.parents() : null;
         if (n)
             for (var r = 0; r < n.length; r++) {
                 if (!t(n[r])) return !1
             }
         return !0
     }
 
-    function Ao(e) {
+    function Ro(e) {
         var t = e.ok,
             n = e.edgeOkViaNode || e.ok,
             r = e.parentOk || e.ok;
         return function() {
             var e = this.cy();
             if (!e.styleEnabled()) return !0;
             var i = this[0],
                 a = e.hasCompoundNodes();
             if (i) {
                 var o = i._private;
                 if (!t(i)) return !1;
-                if (i.isNode()) return !a || Lo(i, r);
+                if (i.isNode()) return !a || Oo(i, r);
                 var s = o.source,
                     l = o.target;
-                return n(s) && (!a || Lo(s, n)) && (s === l || n(l) && (!a || Lo(l, n)))
+                return n(s) && (!a || Oo(s, n)) && (s === l || n(l) && (!a || Oo(l, n)))
             }
         }
     }
-    var Oo = No("eleTakesUpSpace", (function(e) {
+    var Vo = Io("eleTakesUpSpace", (function(e) {
         return "element" === e.pstyle("display").value && 0 !== e.width() && (!e.isNode() || 0 !== e.height())
     }));
-    Io.takesUpSpace = zo("takesUpSpace", Ao({
-        ok: Oo
+    Lo.takesUpSpace = Ao("takesUpSpace", Ro({
+        ok: Vo
     }));
-    var Ro = No("eleInteractive", (function(e) {
-            return "yes" === e.pstyle("events").value && "visible" === e.pstyle("visibility").value && Oo(e)
+    var Fo = Io("eleInteractive", (function(e) {
+            return "yes" === e.pstyle("events").value && "visible" === e.pstyle("visibility").value && Vo(e)
         })),
-        Vo = No("parentInteractive", (function(e) {
-            return "visible" === e.pstyle("visibility").value && Oo(e)
+        jo = Io("parentInteractive", (function(e) {
+            return "visible" === e.pstyle("visibility").value && Vo(e)
         }));
-    Io.interactive = zo("interactive", Ao({
-        ok: Ro,
-        parentOk: Vo,
-        edgeOkViaNode: Oo
-    })), Io.noninteractive = function() {
+    Lo.interactive = Ao("interactive", Ro({
+        ok: Fo,
+        parentOk: jo,
+        edgeOkViaNode: Vo
+    })), Lo.noninteractive = function() {
         var e = this[0];
         if (e) return !e.interactive()
     };
-    var Fo = No("eleVisible", (function(e) {
-            return "visible" === e.pstyle("visibility").value && 0 !== e.pstyle("opacity").pfValue && Oo(e)
+    var qo = Io("eleVisible", (function(e) {
+            return "visible" === e.pstyle("visibility").value && 0 !== e.pstyle("opacity").pfValue && Vo(e)
         })),
-        jo = Oo;
-    Io.visible = zo("visible", Ao({
-        ok: Fo,
-        edgeOkViaNode: jo
-    })), Io.hidden = function() {
+        Yo = Vo;
+    Lo.visible = Ao("visible", Ro({
+        ok: qo,
+        edgeOkViaNode: Yo
+    })), Lo.hidden = function() {
         var e = this[0];
         if (e) return !e.visible()
-    }, Io.isBundledBezier = zo("isBundledBezier", (function() {
+    }, Lo.isBundledBezier = Ao("isBundledBezier", (function() {
         return !!this.cy().styleEnabled() && (!this.removed() && "bezier" === this.pstyle("curve-style").value && this.takesUpSpace())
-    })), Io.bypass = Io.css = Io.style, Io.renderedCss = Io.renderedStyle, Io.removeBypass = Io.removeCss = Io.removeStyle, Io.pstyle = Io.parsedStyle;
-    var qo = {};
+    })), Lo.bypass = Lo.css = Lo.style, Lo.renderedCss = Lo.renderedStyle, Lo.removeBypass = Lo.removeCss = Lo.removeStyle, Lo.pstyle = Lo.parsedStyle;
+    var Xo = {};
 
-    function Yo(e) {
+    function Wo(e) {
         return function() {
             var t = arguments,
                 n = [];
             if (2 === t.length) {
                 var r = t[0],
                     i = t[1];
                 this.on(e.event, r, i)
-            } else if (1 === t.length && g(t[0])) {
+            } else if (1 === t.length && v(t[0])) {
                 var a = t[0];
                 this.on(e.event, a)
-            } else if (0 === t.length || 1 === t.length && v(t[0])) {
+            } else if (0 === t.length || 1 === t.length && y(t[0])) {
                 for (var o = 1 === t.length ? t[0] : null, s = 0; s < this.length; s++) {
                     var l = this[s],
                         u = !e.ableField || l._private[e.ableField],
                         c = l._private[e.field] != e.value;
                     if (e.overrideAble) {
                         var d = e.overrideAble(l);
                         if (void 0 !== d && (u = d, !d)) return this
@@ -6202,84 +6231,84 @@
                 var h = this.spawn(n);
                 h.updateStyle(), h.emit(e.event), o && h.emit(o)
             }
             return this
         }
     }
 
-    function Xo(e) {
-        qo[e.field] = function() {
+    function Ho(e) {
+        Xo[e.field] = function() {
             var t = this[0];
             if (t) {
                 if (e.overrideField) {
                     var n = e.overrideField(t);
                     if (void 0 !== n) return n
                 }
                 return t._private[e.field]
             }
-        }, qo[e.on] = Yo({
+        }, Xo[e.on] = Wo({
             event: e.on,
             field: e.field,
             ableField: e.ableField,
             overrideAble: e.overrideAble,
             value: !0
-        }), qo[e.off] = Yo({
+        }), Xo[e.off] = Wo({
             event: e.off,
             field: e.field,
             ableField: e.ableField,
             overrideAble: e.overrideAble,
             value: !1
         })
     }
-    Xo({
+    Ho({
         field: "locked",
         overrideField: function(e) {
             return !!e.cy().autolock() || void 0
         },
         on: "lock",
         off: "unlock"
-    }), Xo({
+    }), Ho({
         field: "grabbable",
         overrideField: function(e) {
             return !e.cy().autoungrabify() && !e.pannable() && void 0
         },
         on: "grabify",
         off: "ungrabify"
-    }), Xo({
+    }), Ho({
         field: "selected",
         ableField: "selectable",
         overrideAble: function(e) {
             return !e.cy().autounselectify() && void 0
         },
         on: "select",
         off: "unselect"
-    }), Xo({
+    }), Ho({
         field: "selectable",
         overrideField: function(e) {
             return !e.cy().autounselectify() && void 0
         },
         on: "selectify",
         off: "unselectify"
-    }), qo.deselect = qo.unselect, qo.grabbed = function() {
+    }), Xo.deselect = Xo.unselect, Xo.grabbed = function() {
         var e = this[0];
         if (e) return e._private.grabbed
-    }, Xo({
+    }, Ho({
         field: "active",
         on: "activate",
         off: "unactivate"
-    }), Xo({
+    }), Ho({
         field: "pannable",
         on: "panify",
         off: "unpanify"
-    }), qo.inactive = function() {
+    }), Xo.inactive = function() {
         var e = this[0];
         if (e) return !e._private.active
     };
-    var Wo = {},
-        Ho = function(e) {
+    var Ko = {},
+        Go = function(e) {
             return function(t) {
                 for (var n = [], r = 0; r < this.length; r++) {
                     var i = this[r];
                     if (i.isNode()) {
                         for (var a = !1, o = i.connectedEdges(), s = 0; s < o.length; s++) {
                             var l = o[s],
                                 u = l.source(),
@@ -6291,30 +6320,30 @@
                         }
                         a || n.push(i)
                     }
                 }
                 return this.spawn(n, !0).filter(t)
             }
         },
-        Ko = function(e) {
+        Uo = function(e) {
             return function(t) {
                 for (var n = [], r = 0; r < this.length; r++) {
                     var i = this[r];
                     if (i.isNode())
                         for (var a = i.connectedEdges(), o = 0; o < a.length; o++) {
                             var s = a[o],
                                 l = s.source(),
                                 u = s.target();
                             e.outgoing && l === i ? (n.push(s), n.push(u)) : e.incoming && u === i && (n.push(s), n.push(l))
                         }
                 }
                 return this.spawn(n, !0).filter(t)
             }
         },
-        Go = function(e) {
+        Zo = function(e) {
             return function(t) {
                 for (var n = this, r = [], i = {};;) {
                     var a = e.outgoing ? n.outgoers() : n.incomers();
                     if (0 === a.length) break;
                     for (var o = !1, s = 0; s < a.length; s++) {
                         var l = a[s],
                             u = l.id();
@@ -6323,30 +6352,30 @@
                     if (!o) break;
                     n = a
                 }
                 return this.spawn(r, !0).filter(t)
             }
         };
 
-    function Uo(e) {
+    function $o(e) {
         return function(t) {
             for (var n = [], r = 0; r < this.length; r++) {
                 var i = this[r]._private[e.attr];
                 i && n.push(i)
             }
             return this.spawn(n, !0).filter(t)
         }
     }
 
-    function Zo(e) {
+    function Qo(e) {
         return function(t) {
             var n = [],
                 r = this._private.cy,
                 i = e || {};
-            f(t) && (t = r.$(t));
+            g(t) && (t = r.$(t));
             for (var a = 0; a < t.length; a++)
                 for (var o = t[a]._private.edges, s = 0; s < o.length; s++) {
                     var l = o[s],
                         u = l._private.data,
                         c = this.hasElementWithId(u.source) && t.hasElementWithId(u.target),
                         d = t.hasElementWithId(u.source) && this.hasElementWithId(u.target);
                     if (c || d) {
@@ -6357,16 +6386,16 @@
                         n.push(l)
                     }
                 }
             return this.spawn(n, !0)
         }
     }
 
-    function $o(e) {
-        return e = I({}, {
+    function Jo(e) {
+        return e = A({}, {
                 codirected: !1
             }, e),
             function(t) {
                 for (var n = [], r = this.edges(), i = e, a = 0; a < r.length; a++)
                     for (var o = r[a]._private, s = o.source, l = s._private.data.id, u = o.data.target, c = s._private.edges, d = 0; d < c.length; d++) {
                         var h = c[d],
                             p = h._private.data,
@@ -6375,37 +6404,37 @@
                             v = f === u && g === l,
                             y = l === f && u === g;
                         (i.codirected && v || !i.codirected && (v || y)) && n.push(h)
                     }
                 return this.spawn(n, !0).filter(t)
             }
     }
-    Wo.clearTraversalCache = function() {
+    Ko.clearTraversalCache = function() {
         for (var e = 0; e < this.length; e++) this[e]._private.traversalCache = null
-    }, I(Wo, {
-        roots: Ho({
+    }, A(Ko, {
+        roots: Go({
             noIncomingEdges: !0
         }),
-        leaves: Ho({
+        leaves: Go({
             noOutgoingEdges: !0
         }),
-        outgoers: Sa(Ko({
+        outgoers: Da(Uo({
             outgoing: !0
         }), "outgoers"),
-        successors: Go({
+        successors: Zo({
             outgoing: !0
         }),
-        incomers: Sa(Ko({
+        incomers: Da(Uo({
             incoming: !0
         }), "incomers"),
-        predecessors: Go({
+        predecessors: Zo({
             incoming: !0
         })
-    }), I(Wo, {
-        neighborhood: Sa((function(e) {
+    }), A(Ko, {
+        neighborhood: Da((function(e) {
             for (var t = [], n = this.nodes(), r = 0; r < n.length; r++)
                 for (var i = n[r], a = i.connectedEdges(), o = 0; o < a.length; o++) {
                     var s = a[o],
                         l = s.source(),
                         u = s.target(),
                         c = i === l ? u : l;
                     c.length > 0 && t.push(c[0]), t.push(s[0])
@@ -6414,58 +6443,58 @@
         }), "neighborhood"),
         closedNeighborhood: function(e) {
             return this.neighborhood().add(this).filter(e)
         },
         openNeighborhood: function(e) {
             return this.neighborhood(e)
         }
-    }), Wo.neighbourhood = Wo.neighborhood, Wo.closedNeighbourhood = Wo.closedNeighborhood, Wo.openNeighbourhood = Wo.openNeighborhood, I(Wo, {
-        source: Sa((function(e) {
+    }), Ko.neighbourhood = Ko.neighborhood, Ko.closedNeighbourhood = Ko.closedNeighborhood, Ko.openNeighbourhood = Ko.openNeighborhood, A(Ko, {
+        source: Da((function(e) {
             var t, n = this[0];
             return n && (t = n._private.source || n.cy().collection()), t && e ? t.filter(e) : t
         }), "source"),
-        target: Sa((function(e) {
+        target: Da((function(e) {
             var t, n = this[0];
             return n && (t = n._private.target || n.cy().collection()), t && e ? t.filter(e) : t
         }), "target"),
-        sources: Uo({
+        sources: $o({
             attr: "source"
         }),
-        targets: Uo({
+        targets: $o({
             attr: "target"
         })
-    }), I(Wo, {
-        edgesWith: Sa(Zo(), "edgesWith"),
-        edgesTo: Sa(Zo({
+    }), A(Ko, {
+        edgesWith: Da(Qo(), "edgesWith"),
+        edgesTo: Da(Qo({
             thisIsSrc: !0
         }), "edgesTo")
-    }), I(Wo, {
-        connectedEdges: Sa((function(e) {
+    }), A(Ko, {
+        connectedEdges: Da((function(e) {
             for (var t = [], n = 0; n < this.length; n++) {
                 var r = this[n];
                 if (r.isNode())
                     for (var i = r._private.edges, a = 0; a < i.length; a++) {
                         var o = i[a];
                         t.push(o)
                     }
             }
             return this.spawn(t, !0).filter(e)
         }), "connectedEdges"),
-        connectedNodes: Sa((function(e) {
+        connectedNodes: Da((function(e) {
             for (var t = [], n = 0; n < this.length; n++) {
                 var r = this[n];
                 r.isEdge() && (t.push(r.source()[0]), t.push(r.target()[0]))
             }
             return this.spawn(t, !0).filter(e)
         }), "connectedNodes"),
-        parallelEdges: Sa($o(), "parallelEdges"),
-        codirectedEdges: Sa($o({
+        parallelEdges: Da(Jo(), "parallelEdges"),
+        codirectedEdges: Da(Jo({
             codirected: !0
         }), "codirectedEdges")
-    }), I(Wo, {
+    }), A(Ko, {
         components: function(e) {
             var t = this,
                 n = t.cy(),
                 r = n.collection(),
                 i = null == e ? t.nodes() : e.nodes(),
                 a = [];
             null != e && i.empty() && (i = e.sources());
@@ -6494,31 +6523,31 @@
             } while (i.length > 0);
             return a
         },
         component: function() {
             var e = this[0];
             return e.cy().mutableElements().components(e)[0]
         }
-    }), Wo.componentsOf = Wo.components;
-    var Qo = function(e, t) {
+    }), Ko.componentsOf = Ko.components;
+    var es = function(e, t) {
             var n = arguments.length > 2 && void 0 !== arguments[2] && arguments[2],
                 r = arguments.length > 3 && void 0 !== arguments[3] && arguments[3];
             if (void 0 !== e) {
-                var i = new Ue,
+                var i = new Ze,
                     a = !1;
                 if (t) {
-                    if (t.length > 0 && y(t[0]) && !w(t[0])) {
+                    if (t.length > 0 && m(t[0]) && !E(t[0])) {
                         a = !0;
-                        for (var o = [], s = new $e, l = 0, u = t.length; l < u; l++) {
+                        for (var o = [], s = new Qe, l = 0, u = t.length; l < u; l++) {
                             var c = t[l];
                             null == c.data && (c.data = {});
                             var d = c.data;
-                            if (null == d.id) d.id = je();
+                            if (null == d.id) d.id = qe();
                             else if (e.hasElementWithId(d.id) || s.has(d.id)) continue;
-                            var h = new Qe(e, c, !1);
+                            var h = new Je(e, c, !1);
                             o.push(h), s.add(d.id)
                         }
                         t = o
                     }
                 } else t = [];
                 this.length = 0;
                 for (var p = 0, f = t.length; p < f; p++) {
@@ -6537,65 +6566,65 @@
                     get map() {
                         return null == this.lazyMap && this.rebuildMap(), this.lazyMap
                     },
                     set map(e) {
                         this.lazyMap = e
                     },
                     rebuildMap: function() {
-                        for (var e = this.lazyMap = new Ue, t = this.eles, n = 0; n < t.length; n++) {
+                        for (var e = this.lazyMap = new Ze, t = this.eles, n = 0; n < t.length; n++) {
                             var r = t[n];
                             e.set(r.id(), {
                                 index: n,
                                 ele: r
                             })
                         }
                     }
                 }, n && (this._private.map = i), a && !r && this.restore()
-            } else Oe("A collection must have a reference to the core")
+            } else Re("A collection must have a reference to the core")
         },
-        Jo = Qe.prototype = Qo.prototype = Object.create(Array.prototype);
-    Jo.instanceString = function() {
+        ts = Je.prototype = es.prototype = Object.create(Array.prototype);
+    ts.instanceString = function() {
         return "collection"
-    }, Jo.spawn = function(e, t) {
-        return new Qo(this.cy(), e, t)
-    }, Jo.spawnSelf = function() {
+    }, ts.spawn = function(e, t) {
+        return new es(this.cy(), e, t)
+    }, ts.spawnSelf = function() {
         return this.spawn(this)
-    }, Jo.cy = function() {
+    }, ts.cy = function() {
         return this._private.cy
-    }, Jo.renderer = function() {
+    }, ts.renderer = function() {
         return this._private.cy.renderer()
-    }, Jo.element = function() {
+    }, ts.element = function() {
         return this[0]
-    }, Jo.collection = function() {
-        return E(this) ? this : new Qo(this._private.cy, [this])
-    }, Jo.unique = function() {
-        return new Qo(this._private.cy, this, !0)
-    }, Jo.hasElementWithId = function(e) {
+    }, ts.collection = function() {
+        return k(this) ? this : new es(this._private.cy, [this])
+    }, ts.unique = function() {
+        return new es(this._private.cy, this, !0)
+    }, ts.hasElementWithId = function(e) {
         return e = "" + e, this._private.map.has(e)
-    }, Jo.getElementById = function(e) {
+    }, ts.getElementById = function(e) {
         e = "" + e;
         var t = this._private.cy,
             n = this._private.map.get(e);
-        return n ? n.ele : new Qo(t)
-    }, Jo.$id = Jo.getElementById, Jo.poolIndex = function() {
+        return n ? n.ele : new es(t)
+    }, ts.$id = ts.getElementById, ts.poolIndex = function() {
         var e = this._private.cy._private.elements,
             t = this[0]._private.data.id;
         return e._private.map.get(t).index
-    }, Jo.indexOf = function(e) {
+    }, ts.indexOf = function(e) {
         var t = e[0]._private.data.id;
         return this._private.map.get(t).index
-    }, Jo.indexOfId = function(e) {
+    }, ts.indexOfId = function(e) {
         return e = "" + e, this._private.map.get(e).index
-    }, Jo.json = function(e) {
+    }, ts.json = function(e) {
         var t = this.element(),
             n = this.cy();
         if (null == t && e) return this;
         if (null != t) {
             var r = t._private;
-            if (y(e)) {
+            if (m(e)) {
                 if (n.startBatch(), e.data) {
                     t.data(e.data);
                     var i = r.data;
                     if (t.isEdge()) {
                         var a = !1,
                             o = {},
                             s = e.data.source,
@@ -6614,16 +6643,16 @@
                     var o = e[n];
                     null != o && o !== r[n] && (o ? t[i]() : t[a]())
                 };
                 return d("removed", "remove", "restore"), d("selected", "select", "unselect"), d("selectable", "selectify", "unselectify"), d("locked", "lock", "unlock"), d("grabbable", "grabify", "ungrabify"), d("pannable", "panify", "unpanify"), null != e.classes && t.classes(e.classes), n.endBatch(), this
             }
             if (void 0 === e) {
                 var h = {
-                    data: Fe(r.data),
-                    position: Fe(r.position),
+                    data: je(r.data),
+                    position: je(r.position),
                     group: r.group,
                     removed: r.removed,
                     selected: r.selected,
                     selectable: r.selectable,
                     locked: r.locked,
                     grabbable: r.grabbable,
                     pannable: r.pannable,
@@ -6632,113 +6661,113 @@
                 h.classes = "";
                 var p = 0;
                 return r.classes.forEach((function(e) {
                     return h.classes += 0 == p++ ? e : " " + e
                 })), h
             }
         }
-    }, Jo.jsons = function() {
+    }, ts.jsons = function() {
         for (var e = [], t = 0; t < this.length; t++) {
             var n = this[t].json();
             e.push(n)
         }
         return e
-    }, Jo.clone = function() {
+    }, ts.clone = function() {
         for (var e = this.cy(), t = [], n = 0; n < this.length; n++) {
             var r = this[n].json(),
-                i = new Qe(e, r, !1);
+                i = new Je(e, r, !1);
             t.push(i)
         }
-        return new Qo(e, t)
-    }, Jo.copy = Jo.clone, Jo.restore = function() {
+        return new es(e, t)
+    }, ts.copy = ts.clone, ts.restore = function() {
         for (var e, t, n = !(arguments.length > 0 && void 0 !== arguments[0]) || arguments[0], r = !(arguments.length > 1 && void 0 !== arguments[1]) || arguments[1], i = this, a = i.cy(), o = a._private, s = [], l = [], u = 0, c = i.length; u < c; u++) {
             var d = i[u];
             r && !d.removed() || (d.isNode() ? s.push(d) : l.push(d))
         }
         e = s.concat(l);
         var h = function() {
             e.splice(t, 1), t--
         };
         for (t = 0; t < e.length; t++) {
             var p = e[t],
-                g = p._private,
-                v = g.data;
-            if (p.clearTraversalCache(), r || g.removed)
-                if (void 0 === v.id) v.id = je();
-                else if (m(v.id)) v.id = "" + v.id;
+                f = p._private,
+                v = f.data;
+            if (p.clearTraversalCache(), r || f.removed)
+                if (void 0 === v.id) v.id = qe();
+                else if (b(v.id)) v.id = "" + v.id;
             else {
-                if (S(v.id) || !f(v.id)) {
-                    Oe("Can not create element with invalid string ID `" + v.id + "`"), h();
+                if (P(v.id) || !g(v.id)) {
+                    Re("Can not create element with invalid string ID `" + v.id + "`"), h();
                     continue
                 }
                 if (a.hasElementWithId(v.id)) {
-                    Oe("Can not create second element with ID `" + v.id + "`"), h();
+                    Re("Can not create second element with ID `" + v.id + "`"), h();
                     continue
                 }
             } else;
             var y = v.id;
             if (p.isNode()) {
-                var b = g.position;
-                null == b.x && (b.x = 0), null == b.y && (b.y = 0)
+                var m = f.position;
+                null == m.x && (m.x = 0), null == m.y && (m.y = 0)
             }
             if (p.isEdge()) {
                 for (var x = p, w = ["source", "target"], E = w.length, k = !1, C = 0; C < E; C++) {
-                    var P = w[C],
-                        D = v[P];
-                    m(D) && (D = v[P] = "" + v[P]), null == D || "" === D ? (Oe("Can not create edge `" + y + "` with unspecified " + P), k = !0) : a.hasElementWithId(D) || (Oe("Can not create edge `" + y + "` with nonexistant " + P + " `" + D + "`"), k = !0)
+                    var S = w[C],
+                        D = v[S];
+                    b(D) && (D = v[S] = "" + v[S]), null == D || "" === D ? (Re("Can not create edge `" + y + "` with unspecified " + S), k = !0) : a.hasElementWithId(D) || (Re("Can not create edge `" + y + "` with nonexistant " + S + " `" + D + "`"), k = !0)
                 }
                 if (k) {
                     h();
                     continue
                 }
                 var T = a.getElementById(v.source),
                     _ = a.getElementById(v.target);
                 T.same(_) ? T._private.edges.push(x) : (T._private.edges.push(x), _._private.edges.push(x)), x._private.source = T, x._private.target = _
             }
-            g.map = new Ue, g.map.set(y, {
+            f.map = new Ze, f.map.set(y, {
                 ele: p,
                 index: 0
-            }), g.removed = !1, r && a.addToPool(p)
+            }), f.removed = !1, r && a.addToPool(p)
         }
         for (var M = 0; M < s.length; M++) {
             var B = s[M],
                 N = B._private.data;
-            m(N.parent) && (N.parent = "" + N.parent);
+            b(N.parent) && (N.parent = "" + N.parent);
             var z = N.parent,
                 I = null != z;
             if (I || B._private.parent) {
-                var L = B._private.parent ? a.collection().merge(B._private.parent) : a.getElementById(z);
-                if (L.empty()) N.parent = void 0;
-                else if (L[0].removed()) Ve("Node added with missing parent, reference to parent removed"), N.parent = void 0, B._private.parent = null;
+                var A = B._private.parent ? a.collection().merge(B._private.parent) : a.getElementById(z);
+                if (A.empty()) N.parent = void 0;
+                else if (A[0].removed()) Fe("Node added with missing parent, reference to parent removed"), N.parent = void 0, B._private.parent = null;
                 else {
-                    for (var A = !1, O = L; !O.empty();) {
+                    for (var L = !1, O = A; !O.empty();) {
                         if (B.same(O)) {
-                            A = !0, N.parent = void 0;
+                            L = !0, N.parent = void 0;
                             break
                         }
                         O = O.parent()
                     }
-                    A || (L[0]._private.children.push(B), B._private.parent = L[0], o.hasCompoundNodes = !0)
+                    L || (A[0]._private.children.push(B), B._private.parent = A[0], o.hasCompoundNodes = !0)
                 }
             }
         }
         if (e.length > 0) {
-            for (var R = e.length === i.length ? i : new Qo(a, e), V = 0; V < R.length; V++) {
+            for (var R = e.length === i.length ? i : new es(a, e), V = 0; V < R.length; V++) {
                 var F = R[V];
                 F.isNode() || (F.parallelEdges().clearTraversalCache(), F.source().clearTraversalCache(), F.target().clearTraversalCache())
             }(o.hasCompoundNodes ? a.collection().merge(R).merge(R.connectedNodes()).merge(R.parent()) : R).dirtyCompoundBoundsCache().dirtyBoundingBoxCache().updateStyle(n), n ? R.emitAndNotify("add") : r && R.emit("add")
         }
         return i
-    }, Jo.removed = function() {
+    }, ts.removed = function() {
         var e = this[0];
         return e && e._private.removed
-    }, Jo.inside = function() {
+    }, ts.inside = function() {
         var e = this[0];
         return e && !e._private.removed
-    }, Jo.remove = function() {
+    }, ts.remove = function() {
         var e = !(arguments.length > 0 && void 0 !== arguments[0]) || arguments[0],
             t = !(arguments.length > 1 && void 0 !== arguments[1]) || arguments[1],
             n = this,
             r = [],
             i = {},
             a = n._private.cy;
 
@@ -6757,27 +6786,27 @@
         for (var u = 0, c = n.length; u < c; u++) {
             var d = n[u];
             l(d)
         }
 
         function h(e, t) {
             var n = e._private.edges;
-            We(n, t), e.clearTraversalCache()
+            He(n, t), e.clearTraversalCache()
         }
 
         function p(e) {
             e.clearTraversalCache()
         }
         var f = [];
 
         function g(e, t) {
             t = t[0];
             var n = (e = e[0])._private.children,
                 r = e.id();
-            We(n, t), t._private.parent = null, f.ids[r] || (f.ids[r] = !0, f.push(e))
+            He(n, t), t._private.parent = null, f.ids[r] || (f.ids[r] = !0, f.push(e))
         }
         f.ids = {}, n.dirtyCompoundBoundsCache(), t && a.removeFromPool(r);
         for (var v = 0; v < r.length; v++) {
             var y = r[v];
             if (y.isEdge()) {
                 var m = y.source()[0],
                     b = y.target()[0];
@@ -6797,22 +6826,22 @@
         for (var S = 0; S < C.length; S++) {
             var P = C[S];
             if (P.isParent()) {
                 a._private.hasCompoundNodes = !0;
                 break
             }
         }
-        var D = new Qo(this.cy(), r);
+        var D = new es(this.cy(), r);
         D.size() > 0 && (e ? D.emitAndNotify("remove") : t && D.emit("remove"));
         for (var T = 0; T < f.length; T++) {
             var _ = f[T];
             t && _.removed() || _.updateStyle()
         }
         return D
-    }, Jo.move = function(e) {
+    }, ts.move = function(e) {
         var t = this._private.cy,
             n = this,
             r = function(e) {
                 return null == e ? e : "" + e
             };
         if (void 0 !== e.source || void 0 !== e.target) {
             var i = r(e.source),
@@ -6841,15 +6870,15 @@
                         r.isNode() && (i.parent = u)
                     }
                     e.restore(!1, !1)
                 })), n.emitAndNotify("move")
             }
         }
         return this
-    }, [or, Ri, Vi, Ea, Pa, za, Ia, lo, Co, So, {
+    }, [lr, Fi, ji, Ca, Ta, Aa, La, co, Po, Do, {
         isNode: function() {
             return "nodes" === this.group()
         },
         isEdge: function() {
             return "edges" === this.group()
         },
         isLoop: function() {
@@ -6858,62 +6887,62 @@
         isSimple: function() {
             return this.isEdge() && this.source()[0] !== this.target()[0]
         },
         group: function() {
             var e = this[0];
             if (e) return e._private.group
         }
-    }, To, Mo, Io, qo, Wo].forEach((function(e) {
-        I(Jo, e)
+    }, Mo, No, Lo, Xo, Ko].forEach((function(e) {
+        A(ts, e)
     }));
-    var es = {
+    var ns = {
         add: function(e) {
             var t, n = this;
-            if (x(e)) {
+            if (w(e)) {
                 var r = e;
                 if (r._private.cy === n) t = r.restore();
                 else {
                     for (var i = [], a = 0; a < r.length; a++) {
                         var o = r[a];
                         i.push(o.json())
                     }
-                    t = new Qo(n, i)
+                    t = new es(n, i)
                 }
-            } else if (v(e)) {
-                t = new Qo(n, e)
-            } else if (y(e) && (v(e.nodes) || v(e.edges))) {
+            } else if (y(e)) {
+                t = new es(n, e)
+            } else if (m(e) && (y(e.nodes) || y(e.edges))) {
                 for (var s = e, l = [], u = ["nodes", "edges"], c = 0, d = u.length; c < d; c++) {
                     var h = u[c],
                         p = s[h];
-                    if (v(p))
+                    if (y(p))
                         for (var f = 0, g = p.length; f < g; f++) {
-                            var m = I({
+                            var v = A({
                                 group: h
                             }, p[f]);
-                            l.push(m)
+                            l.push(v)
                         }
                 }
-                t = new Qo(n, l)
+                t = new es(n, l)
             } else {
-                t = new Qe(n, e).collection()
+                t = new Je(n, e).collection()
             }
             return t
         },
         remove: function(e) {
-            if (x(e));
-            else if (f(e)) {
+            if (w(e));
+            else if (g(e)) {
                 var t = e;
                 e = this.$(t)
             }
             return e.remove()
         }
     };
     /*! Bezier curve function generator. Copyright Gaetan Renaudeau. MIT License: http://en.wikipedia.org/wiki/MIT_License */
     /*! Runge-Kutta spring physics function generator. Adapted from Framer.js, copyright Koen Bok. MIT License: http://en.wikipedia.org/wiki/MIT_License */
-    var ts = function() {
+    var rs = function() {
             function e(e) {
                 return -e.tension * e.x - e.friction * e.v
             }
 
             function t(t, n, r) {
                 var i = {
                     x: t.x + r.dx * n,
@@ -6950,15 +6979,15 @@
                     c = 0;
                 for (t = parseFloat(t) || 500, r = parseFloat(r) || 20, i = i || null, l.tension = t, l.friction = r, o = (a = null !== i) ? (c = e(t, r)) / i * .016 : .016; s = n(s || l, o), u.push(1 + s.x), c += 16, Math.abs(s.x) > 1e-4 && Math.abs(s.v) > 1e-4;);
                 return a ? function(e) {
                     return u[e * (u.length - 1) | 0]
                 } : c
             }
         }(),
-        ns = function(e, t, n, r) {
+        is = function(e, t, n, r) {
             var i = function(e, t, n, r) {
                 var i = 4,
                     a = .001,
                     o = 1e-7,
                     s = 10,
                     l = 11,
                     u = 1 / (l - 1),
@@ -7039,142 +7068,142 @@
                     return S
                 }, C
             }(e, t, n, r);
             return function(e, t, n) {
                 return e + (t - e) * i(n)
             }
         },
-        rs = {
+        as = {
             linear: function(e, t, n) {
                 return e + (t - e) * n
             },
-            ease: ns(.25, .1, .25, 1),
-            "ease-in": ns(.42, 0, 1, 1),
-            "ease-out": ns(0, 0, .58, 1),
-            "ease-in-out": ns(.42, 0, .58, 1),
-            "ease-in-sine": ns(.47, 0, .745, .715),
-            "ease-out-sine": ns(.39, .575, .565, 1),
-            "ease-in-out-sine": ns(.445, .05, .55, .95),
-            "ease-in-quad": ns(.55, .085, .68, .53),
-            "ease-out-quad": ns(.25, .46, .45, .94),
-            "ease-in-out-quad": ns(.455, .03, .515, .955),
-            "ease-in-cubic": ns(.55, .055, .675, .19),
-            "ease-out-cubic": ns(.215, .61, .355, 1),
-            "ease-in-out-cubic": ns(.645, .045, .355, 1),
-            "ease-in-quart": ns(.895, .03, .685, .22),
-            "ease-out-quart": ns(.165, .84, .44, 1),
-            "ease-in-out-quart": ns(.77, 0, .175, 1),
-            "ease-in-quint": ns(.755, .05, .855, .06),
-            "ease-out-quint": ns(.23, 1, .32, 1),
-            "ease-in-out-quint": ns(.86, 0, .07, 1),
-            "ease-in-expo": ns(.95, .05, .795, .035),
-            "ease-out-expo": ns(.19, 1, .22, 1),
-            "ease-in-out-expo": ns(1, 0, 0, 1),
-            "ease-in-circ": ns(.6, .04, .98, .335),
-            "ease-out-circ": ns(.075, .82, .165, 1),
-            "ease-in-out-circ": ns(.785, .135, .15, .86),
+            ease: is(.25, .1, .25, 1),
+            "ease-in": is(.42, 0, 1, 1),
+            "ease-out": is(0, 0, .58, 1),
+            "ease-in-out": is(.42, 0, .58, 1),
+            "ease-in-sine": is(.47, 0, .745, .715),
+            "ease-out-sine": is(.39, .575, .565, 1),
+            "ease-in-out-sine": is(.445, .05, .55, .95),
+            "ease-in-quad": is(.55, .085, .68, .53),
+            "ease-out-quad": is(.25, .46, .45, .94),
+            "ease-in-out-quad": is(.455, .03, .515, .955),
+            "ease-in-cubic": is(.55, .055, .675, .19),
+            "ease-out-cubic": is(.215, .61, .355, 1),
+            "ease-in-out-cubic": is(.645, .045, .355, 1),
+            "ease-in-quart": is(.895, .03, .685, .22),
+            "ease-out-quart": is(.165, .84, .44, 1),
+            "ease-in-out-quart": is(.77, 0, .175, 1),
+            "ease-in-quint": is(.755, .05, .855, .06),
+            "ease-out-quint": is(.23, 1, .32, 1),
+            "ease-in-out-quint": is(.86, 0, .07, 1),
+            "ease-in-expo": is(.95, .05, .795, .035),
+            "ease-out-expo": is(.19, 1, .22, 1),
+            "ease-in-out-expo": is(1, 0, 0, 1),
+            "ease-in-circ": is(.6, .04, .98, .335),
+            "ease-out-circ": is(.075, .82, .165, 1),
+            "ease-in-out-circ": is(.785, .135, .15, .86),
             spring: function(e, t, n) {
-                if (0 === n) return rs.linear;
-                var r = ts(e, t, n);
+                if (0 === n) return as.linear;
+                var r = rs(e, t, n);
                 return function(e, t, n) {
                     return e + (t - e) * r(n)
                 }
             },
-            "cubic-bezier": ns
+            "cubic-bezier": is
         };
 
-    function is(e, t, n, r, i) {
+    function os(e, t, n, r, i) {
         if (1 === r) return n;
         if (t === n) return n;
         var a = i(t, n, r);
         return null == e || ((e.roundValue || e.color) && (a = Math.round(a)), void 0 !== e.min && (a = Math.max(a, e.min)), void 0 !== e.max && (a = Math.min(a, e.max))), a
     }
 
-    function as(e, t) {
+    function ss(e, t) {
         return null != e.pfValue || null != e.value ? null == e.pfValue || null != t && "%" === t.type.units ? e.value : e.pfValue : e
     }
 
-    function os(e, t, n, r, i) {
+    function ls(e, t, n, r, i) {
         var a = null != i ? i.type : null;
         n < 0 ? n = 0 : n > 1 && (n = 1);
-        var o = as(e, i),
-            s = as(t, i);
-        if (m(o) && m(s)) return is(a, o, s, n, r);
-        if (v(o) && v(s)) {
+        var o = ss(e, i),
+            s = ss(t, i);
+        if (b(o) && b(s)) return os(a, o, s, n, r);
+        if (y(o) && y(s)) {
             for (var l = [], u = 0; u < s.length; u++) {
                 var c = o[u],
                     d = s[u];
                 if (null != c && null != d) {
-                    var h = is(a, c, d, n, r);
+                    var h = os(a, c, d, n, r);
                     l.push(h)
                 } else l.push(d)
             }
             return l
         }
     }
 
-    function ss(e, t, n, r) {
+    function us(e, t, n, r) {
         var i = !r,
             a = e._private,
             o = t._private,
             s = o.easing,
             l = o.startTime,
             u = (r ? e : e.cy()).style();
         if (!o.easingImpl)
-            if (null == s) o.easingImpl = rs.linear;
+            if (null == s) o.easingImpl = as.linear;
             else {
                 var c, d, h;
-                if (f(s)) c = u.parse("transition-timing-function", s).value;
+                if (g(s)) c = u.parse("transition-timing-function", s).value;
                 else c = s;
-                f(c) ? (d = c, h = []) : (d = c[1], h = c.slice(2).map((function(e) {
+                g(c) ? (d = c, h = []) : (d = c[1], h = c.slice(2).map((function(e) {
                     return +e
-                }))), h.length > 0 ? ("spring" === d && h.push(o.duration), o.easingImpl = rs[d].apply(null, h)) : o.easingImpl = rs[d]
-            } var p, g = o.easingImpl;
+                }))), h.length > 0 ? ("spring" === d && h.push(o.duration), o.easingImpl = as[d].apply(null, h)) : o.easingImpl = as[d]
+            } var p, f = o.easingImpl;
         if (p = 0 === o.duration ? 1 : (n - l) / o.duration, o.applying && (p = o.progress), p < 0 ? p = 0 : p > 1 && (p = 1), null == o.delay) {
             var v = o.startPosition,
                 y = o.position;
             if (y && i && !e.locked()) {
                 var m = {};
-                ls(v.x, y.x) && (m.x = os(v.x, y.x, p, g)), ls(v.y, y.y) && (m.y = os(v.y, y.y, p, g)), e.position(m)
+                cs(v.x, y.x) && (m.x = ls(v.x, y.x, p, f)), cs(v.y, y.y) && (m.y = ls(v.y, y.y, p, f)), e.position(m)
             }
             var b = o.startPan,
                 x = o.pan,
                 w = a.pan,
                 E = null != x && r;
-            E && (ls(b.x, x.x) && (w.x = os(b.x, x.x, p, g)), ls(b.y, x.y) && (w.y = os(b.y, x.y, p, g)), e.emit("pan"));
+            E && (cs(b.x, x.x) && (w.x = ls(b.x, x.x, p, f)), cs(b.y, x.y) && (w.y = ls(b.y, x.y, p, f)), e.emit("pan"));
             var k = o.startZoom,
                 C = o.zoom,
                 S = null != C && r;
-            S && (ls(k, C) && (a.zoom = Pt(a.minZoom, os(k, C, p, g), a.maxZoom)), e.emit("zoom")), (E || S) && e.emit("viewport");
+            S && (cs(k, C) && (a.zoom = Dt(a.minZoom, ls(k, C, p, f), a.maxZoom)), e.emit("zoom")), (E || S) && e.emit("viewport");
             var P = o.style;
             if (P && P.length > 0 && i) {
                 for (var D = 0; D < P.length; D++) {
                     var T = P[D],
                         _ = T.name,
                         M = T,
                         B = o.startStyle[_],
-                        N = os(B, M, p, g, u.properties[B.name]);
+                        N = ls(B, M, p, f, u.properties[B.name]);
                     u.overrideBypass(e, _, N)
                 }
                 e.emit("style")
             }
         }
         return o.progress = p, p
     }
 
-    function ls(e, t) {
-        return null != e && null != t && (!(!m(e) || !m(t)) || !(!e || !t))
+    function cs(e, t) {
+        return null != e && null != t && (!(!b(e) || !b(t)) || !(!e || !t))
     }
 
-    function us(e, t, n, r) {
+    function ds(e, t, n, r) {
         var i = t._private;
         i.started = !0, i.startTime = n - i.progress * i.duration
     }
 
-    function cs(e, t) {
+    function hs(e, t) {
         var n = t._private.aniEles,
             r = [];
 
         function i(t, n) {
             var i = t._private,
                 a = i.animation.current,
                 o = i.animation.queue,
@@ -7187,134 +7216,134 @@
                     for (var t = e.length - 1; t >= 0; t--) {
                         (0, e[t])()
                     }
                     e.splice(0, e.length)
                 }, c = a.length - 1; c >= 0; c--) {
                 var d = a[c],
                     h = d._private;
-                h.stopped ? (a.splice(c, 1), h.hooked = !1, h.playing = !1, h.started = !1, u(h.frames)) : (h.playing || h.applying) && (h.playing && h.applying && (h.applying = !1), h.started || us(0, d, e), ss(t, d, e, n), h.applying && (h.applying = !1), u(h.frames), null != h.step && h.step(e), d.completed() && (a.splice(c, 1), h.hooked = !1, h.playing = !1, h.started = !1, u(h.completes)), s = !0)
+                h.stopped ? (a.splice(c, 1), h.hooked = !1, h.playing = !1, h.started = !1, u(h.frames)) : (h.playing || h.applying) && (h.playing && h.applying && (h.applying = !1), h.started || ds(0, d, e), us(t, d, e, n), h.applying && (h.applying = !1), u(h.frames), null != h.step && h.step(e), d.completed() && (a.splice(c, 1), h.hooked = !1, h.playing = !1, h.started = !1, u(h.completes)), s = !0)
             }
             return n || 0 !== a.length || 0 !== o.length || r.push(t), s
         }
         for (var a = !1, o = 0; o < n.length; o++) {
             var s = i(n[o]);
             a = a || s
         }
         var l = i(t, !0);
         (a || l) && (n.length > 0 ? t.notify("draw", n) : t.notify("draw")), n.unmerge(r), t.emit("step")
     }
-    var ds = {
-            animate: Oi.animate(),
-            animation: Oi.animation(),
-            animated: Oi.animated(),
-            clearQueue: Oi.clearQueue(),
-            delay: Oi.delay(),
-            delayAnimation: Oi.delayAnimation(),
-            stop: Oi.stop(),
+    var ps = {
+            animate: Vi.animate(),
+            animation: Vi.animation(),
+            animated: Vi.animated(),
+            clearQueue: Vi.clearQueue(),
+            delay: Vi.delay(),
+            delayAnimation: Vi.delayAnimation(),
+            stop: Vi.stop(),
             addToAnimationPool: function(e) {
                 this.styleEnabled() && this._private.aniEles.merge(e)
             },
             stopAnimationLoop: function() {
                 this._private.animationsRunning = !1
             },
             startAnimationLoop: function() {
                 var e = this;
                 if (e._private.animationsRunning = !0, e.styleEnabled()) {
                     var t = e.renderer();
                     t && t.beforeRender ? t.beforeRender((function(t, n) {
-                        cs(n, e)
+                        hs(n, e)
                     }), t.beforeRenderPriorities.animations) : function t() {
-                        e._private.animationsRunning && me((function(n) {
-                            cs(n, e), t()
+                        e._private.animationsRunning && be((function(n) {
+                            hs(n, e), t()
                         }))
                     }()
                 }
             }
         },
-        hs = {
+        fs = {
             qualifierCompare: function(e, t) {
                 return null == e || null == t ? null == e && null == t : e.sameText(t)
             },
             eventMatches: function(e, t, n) {
                 var r = t.qualifier;
-                return null == r || e !== n.target && w(n.target) && r.matches(n.target)
+                return null == r || e !== n.target && E(n.target) && r.matches(n.target)
             },
             addEventFields: function(e, t) {
                 t.cy = e, t.target = e
             },
             callbackContext: function(e, t, n) {
                 return null != t.qualifier ? n.target : e
             }
         },
-        ps = function(e) {
-            return f(e) ? new xa(e) : e
+        gs = function(e) {
+            return g(e) ? new Ea(e) : e
         },
-        fs = {
+        vs = {
             createEmitter: function() {
                 var e = this._private;
-                return e.emitter || (e.emitter = new yo(hs, this)), this
+                return e.emitter || (e.emitter = new bo(fs, this)), this
             },
             emitter: function() {
                 return this._private.emitter
             },
             on: function(e, t, n) {
-                return this.emitter().on(e, ps(t), n), this
+                return this.emitter().on(e, gs(t), n), this
             },
             removeListener: function(e, t, n) {
-                return this.emitter().removeListener(e, ps(t), n), this
+                return this.emitter().removeListener(e, gs(t), n), this
             },
             removeAllListeners: function() {
                 return this.emitter().removeAllListeners(), this
             },
             one: function(e, t, n) {
-                return this.emitter().one(e, ps(t), n), this
+                return this.emitter().one(e, gs(t), n), this
             },
             once: function(e, t, n) {
-                return this.emitter().one(e, ps(t), n), this
+                return this.emitter().one(e, gs(t), n), this
             },
             emit: function(e, t) {
                 return this.emitter().emit(e, t), this
             },
             emitAndNotify: function(e, t) {
                 return this.emit(e), this.notify(e, t), this
             }
         };
-    Oi.eventAliasesOn(fs);
-    var gs = {
+    Vi.eventAliasesOn(vs);
+    var ys = {
         png: function(e) {
             return e = e || {}, this._private.renderer.png(e)
         },
         jpg: function(e) {
             var t = this._private.renderer;
             return (e = e || {}).bg = e.bg || "#fff", t.jpg(e)
         }
     };
-    gs.jpeg = gs.jpg;
-    var vs = {
+    ys.jpeg = ys.jpg;
+    var ms = {
         layout: function(e) {
             if (null != e)
                 if (null != e.name) {
                     var t = e.name,
                         n = this.extension("layout", t);
                     if (null != n) {
                         var r;
-                        r = f(e.eles) ? this.$(e.eles) : null != e.eles ? e.eles : this.$();
-                        var i = new n(I({}, e, {
+                        r = g(e.eles) ? this.$(e.eles) : null != e.eles ? e.eles : this.$();
+                        var i = new n(A({}, e, {
                             cy: this,
                             eles: r
                         }));
                         return i
                     }
-                    Oe("No such layout `" + t + "` found.  Did you forget to import it and `cytoscape.use()` it?")
-                } else Oe("A `name` must be specified to make a layout");
-            else Oe("Layout options must be specified to make a layout")
+                    Re("No such layout `" + t + "` found.  Did you forget to import it and `cytoscape.use()` it?")
+                } else Re("A `name` must be specified to make a layout");
+            else Re("Layout options must be specified to make a layout")
         }
     };
-    vs.createLayout = vs.makeLayout = vs.layout;
-    var ys = {
+    ms.createLayout = ms.makeLayout = ms.layout;
+    var bs = {
             notify: function(e, t) {
                 var n = this._private;
                 if (this.batching()) {
                     n.batchNotifications = n.batchNotifications || {};
                     var r = n.batchNotifications[e] = n.batchNotifications[e] || this.collection();
                     null != t && r.merge(t)
                 } else if (n.notificationsEnabled) {
@@ -7359,27 +7388,27 @@
                         var i = n[r],
                             a = e[i];
                         t.getElementById(i).data(a)
                     }
                 }))
             }
         },
-        ms = Xe({
+        xs = We({
             hideEdgesOnViewport: !1,
             textureOnViewport: !1,
             motionBlur: !1,
             motionBlurOpacity: .05,
             pixelRatio: void 0,
             desktopTapThreshold: 4,
             touchTapThreshold: 8,
             wheelSensitivity: 1,
             debug: !1,
             showFps: !1
         }),
-        bs = {
+        ws = {
             renderTo: function(e, t, n, r) {
                 return this._private.renderer.renderTo(e, t, n, r), this
             },
             renderer: function() {
                 return this._private.renderer
             },
             forceRender: function() {
@@ -7387,18 +7416,18 @@
             },
             resize: function() {
                 return this.invalidateSize(), this.emitAndNotify("resize"), this
             },
             initRenderer: function(e) {
                 var t = this.extension("renderer", e.name);
                 if (null != t) {
-                    void 0 !== e.wheelSensitivity && Ve("You have set a custom wheel sensitivity.  This will make your app zoom unnaturally when using mainstream mice.  You should change this value from the default only if you can guarantee that all your users will use the same hardware and OS configuration as your current machine.");
-                    var n = ms(e);
+                    void 0 !== e.wheelSensitivity && Fe("You have set a custom wheel sensitivity.  This will make your app zoom unnaturally when using mainstream mice.  You should change this value from the default only if you can guarantee that all your users will use the same hardware and OS configuration as your current machine.");
+                    var n = xs(e);
                     n.cy = this, this._private.renderer = new t(n), this.notify("init")
-                } else Oe("Can not initialise: No such renderer `".concat(e.name, "` found. Did you forget to import it and `cytoscape.use()` it?"))
+                } else Re("Can not initialise: No such renderer `".concat(e.name, "` found. Did you forget to import it and `cytoscape.use()` it?"))
             },
             destroyRenderer: function() {
                 this.notify("destroy");
                 var e = this.container();
                 if (e)
                     for (e._cyreg = null; e.childNodes.length > 0;) e.removeChild(e.childNodes[0]);
                 this._private.renderer = null, this.mutableElements().forEach((function(e) {
@@ -7409,18 +7438,18 @@
             onRender: function(e) {
                 return this.on("render", e)
             },
             offRender: function(e) {
                 return this.off("render", e)
             }
         };
-    bs.invalidateDimensions = bs.resize;
-    var xs = {
+    ws.invalidateDimensions = ws.resize;
+    var Es = {
         collection: function(e, t) {
-            return f(e) ? this.$(e) : x(e) ? e.collection() : v(e) ? (t || (t = {}), new Qo(this, e, t.unique, t.removed)) : new Qo(this)
+            return g(e) ? this.$(e) : w(e) ? e.collection() : y(e) ? (t || (t = {}), new es(this, e, t.unique, t.removed)) : new es(this)
         },
         nodes: function(e) {
             var t = this.$((function(e) {
                 return e.isNode()
             }));
             return e ? t.filter(e) : t
         },
@@ -7434,28 +7463,28 @@
             var t = this._private.elements;
             return e ? t.filter(e) : t.spawnSelf()
         },
         mutableElements: function() {
             return this._private.elements
         }
     };
-    xs.elements = xs.filter = xs.$;
-    var ws = {};
-    ws.apply = function(e) {
+    Es.elements = Es.filter = Es.$;
+    var ks = {};
+    ks.apply = function(e) {
         for (var t = this._private.cy.collection(), n = 0; n < e.length; n++) {
             var r = e[n],
                 i = this.getContextMeta(r);
             if (!i.empty) {
                 var a = this.getContextStyle(i),
                     o = this.applyContextStyle(i, a, r);
                 r._private.appliedInitStyle ? this.updateTransitions(r, o.diffProps) : r._private.appliedInitStyle = !0, this.updateStyleHints(r) && t.push(r)
             }
         }
         return t
-    }, ws.getPropertiesDiff = function(e, t) {
+    }, ks.getPropertiesDiff = function(e, t) {
         var n = this._private.propDiffs = this._private.propDiffs || {},
             r = e + "-" + t,
             i = n[r];
         if (i) return i;
         for (var a = [], o = {}, s = 0; s < this.length; s++) {
             var l = this[s],
                 u = "t" === e[s],
@@ -7471,25 +7500,25 @@
                         if ("t" === t[m] && (y = null != b.properties[g.name])) break
                     }
                     o[v] || y || (o[v] = !0, a.push(v))
                 }
             }
         }
         return n[r] = a, a
-    }, ws.getContextMeta = function(e) {
+    }, ks.getContextMeta = function(e) {
         for (var t, n = "", r = e._private.styleCxtKey || "", i = 0; i < this.length; i++) {
             var a = this[i];
             n += a.selector && a.selector.matches(e) ? "t" : "f"
         }
         return t = this.getPropertiesDiff(r, n), e._private.styleCxtKey = n, {
             key: n,
             diffPropNames: t,
             empty: 0 === t.length
         }
-    }, ws.getContextStyle = function(e) {
+    }, ks.getContextStyle = function(e) {
         var t = e.key,
             n = this._private.contextStyles = this._private.contextStyles || {};
         if (n[t]) return n[t];
         for (var r = {
                 _private: {
                     key: t
                 }
@@ -7498,15 +7527,15 @@
             if ("t" === t[i])
                 for (var o = 0; o < a.properties.length; o++) {
                     var s = a.properties[o];
                     r[s.name] = s
                 }
         }
         return n[t] = r, r
-    }, ws.applyContextStyle = function(e, t, n) {
+    }, ks.applyContextStyle = function(e, t, n) {
         for (var r = e.diffPropNames, i = {}, a = this.types, o = 0; o < r.length; o++) {
             var s = r[o],
                 l = t[s],
                 u = n.pstyle(s);
             if (!l) {
                 if (!u) continue;
                 l = u.bypass ? {
@@ -7527,15 +7556,15 @@
                 };
                 this.applyParsedProperty(n, l), d.next = n.pstyle(s), d.next && d.next.bypass && (d.next = d.next.bypassed)
             }
         }
         return {
             diffProps: i
         }
-    }, ws.updateStyleHints = function(e) {
+    }, ks.updateStyleHints = function(e) {
         var t = e._private,
             n = this,
             r = n.propertyGroupNames,
             i = n.propertyGroupKeys,
             a = function(e, t, r) {
                 return n.getPropertiesHash(e, t, r)
             },
@@ -7545,17 +7574,17 @@
             l = e._private.style;
         r = Object.keys(l);
         for (var u = 0; u < i.length; u++) {
             var c = i[u];
             t.styleKeys[c] = [9261, 5381]
         }
         for (var d, h = function(e, n) {
-                return t.styleKeys[n][0] = Ee(e, t.styleKeys[n][0])
+                return t.styleKeys[n][0] = ke(e, t.styleKeys[n][0])
             }, p = function(e, n) {
-                return t.styleKeys[n][1] = ke(e, t.styleKeys[n][1])
+                return t.styleKeys[n][1] = Ce(e, t.styleKeys[n][1])
             }, f = function(e, t) {
                 h(e, t), p(e, t)
             }, g = function(e, t) {
                 for (var n = 0; n < e.length; n++) {
                     var r = e.charCodeAt(n);
                     h(r, t), p(r, t)
                 }
@@ -7575,44 +7604,44 @@
                 if (x.number && S && !x.multiple) f(-128 < (d = C ? E : k) && d < 128 && Math.floor(d) !== d ? 2e9 - (1024 * d | 0) : d, w), C || null == P || g(P, w);
                 else g(m.strValue, w)
             }
         }
         for (var D, T, _ = [9261, 5381], M = 0; M < i.length; M++) {
             var B = i[M],
                 N = t.styleKeys[B];
-            _[0] = Ee(N[0], _[0]), _[1] = ke(N[1], _[1])
+            _[0] = ke(N[0], _[0]), _[1] = Ce(N[1], _[1])
         }
         t.styleKey = (D = _[0], T = _[1], 2097152 * D + T);
         var z = t.styleKeys;
-        t.labelDimsKey = Ce(z.labelDimensions);
+        t.labelDimsKey = Se(z.labelDimensions);
         var I = a(e, ["label"], z.labelDimensions);
-        if (t.labelKey = Ce(I), t.labelStyleKey = Ce(Se(z.commonLabel, I)), !s) {
-            var L = a(e, ["source-label"], z.labelDimensions);
-            t.sourceLabelKey = Ce(L), t.sourceLabelStyleKey = Ce(Se(z.commonLabel, L));
-            var A = a(e, ["target-label"], z.labelDimensions);
-            t.targetLabelKey = Ce(A), t.targetLabelStyleKey = Ce(Se(z.commonLabel, A))
+        if (t.labelKey = Se(I), t.labelStyleKey = Se(Pe(z.commonLabel, I)), !s) {
+            var A = a(e, ["source-label"], z.labelDimensions);
+            t.sourceLabelKey = Se(A), t.sourceLabelStyleKey = Se(Pe(z.commonLabel, A));
+            var L = a(e, ["target-label"], z.labelDimensions);
+            t.targetLabelKey = Se(L), t.targetLabelStyleKey = Se(Pe(z.commonLabel, L))
         }
         if (s) {
             var O = t.styleKeys,
                 R = O.nodeBody,
                 V = O.nodeBorder,
                 F = O.nodeOutline,
                 j = O.backgroundImage,
                 q = O.compound,
                 Y = O.pie,
                 X = [R, V, F, j, q, Y].filter((function(e) {
                     return null != e
-                })).reduce(Se, [9261, 5381]);
-            t.nodeKey = Ce(X), t.hasPie = null != Y && 9261 !== Y[0] && 5381 !== Y[1]
+                })).reduce(Pe, [9261, 5381]);
+            t.nodeKey = Se(X), t.hasPie = null != Y && 9261 !== Y[0] && 5381 !== Y[1]
         }
         return o !== t.styleKey
-    }, ws.clearStyleHints = function(e) {
+    }, ks.clearStyleHints = function(e) {
         var t = e._private;
         t.styleCxtKey = "", t.styleKeys = {}, t.styleKey = null, t.labelKey = null, t.labelStyleKey = null, t.sourceLabelKey = null, t.sourceLabelStyleKey = null, t.targetLabelKey = null, t.targetLabelStyleKey = null, t.nodeKey = null, t.hasPie = null
-    }, ws.applyParsedProperty = function(e, t) {
+    }, ks.applyParsedProperty = function(e, t) {
         var n, r = this,
             i = t,
             a = e._private.style,
             o = r.types,
             s = r.properties[i.name].type,
             l = i.bypass,
             u = a[i.name],
@@ -7626,23 +7655,23 @@
                     n = h(i);
                 r.checkTriggers(e, i.name, t, n)
             };
         if ("curve-style" === t.name && e.isEdge() && ("bezier" !== t.value && e.isLoop() || "haystack" === t.value && (e.source().isParent() || e.target().isParent())) && (i = t = this.parse(t.name, "bezier", l)), i.delete) return a[i.name] = void 0, p(), !0;
         if (i.deleteBypassed) return u ? !!u.bypass && (u.bypassed = void 0, p(), !0) : (p(), !0);
         if (i.deleteBypass) return u ? !!u.bypass && (a[i.name] = u.bypassed, p(), !0) : (p(), !0);
         var f = function() {
-            Ve("Do not assign mappings to elements without corresponding data (i.e. ele `" + e.id() + "` has no mapping for property `" + i.name + "` with data field `" + i.field + "`); try a `[" + i.field + "]` selector to limit scope to elements with `" + i.field + "` defined")
+            Fe("Do not assign mappings to elements without corresponding data (i.e. ele `" + e.id() + "` has no mapping for property `" + i.name + "` with data field `" + i.field + "`); try a `[" + i.field + "]` selector to limit scope to elements with `" + i.field + "` defined")
         };
         switch (i.mapped) {
             case o.mapData:
-                for (var g, v = i.field.split("."), y = d.data, b = 0; b < v.length && y; b++) {
-                    y = y[v[b]]
+                for (var g, v = i.field.split("."), y = d.data, m = 0; m < v.length && y; m++) {
+                    y = y[v[m]]
                 }
                 if (null == y) return f(), !1;
-                if (!m(y)) return Ve("Do not use continuous mappers without specifying numeric data (i.e. `" + i.field + ": " + y + "` for `" + e.id() + "` is non-numeric)"), !1;
+                if (!b(y)) return Fe("Do not use continuous mappers without specifying numeric data (i.e. `" + i.field + ": " + y + "` for `" + e.id() + "` is non-numeric)"), !1;
                 var x = i.fieldMax - i.fieldMin;
                 if ((g = 0 === x ? 0 : (y - i.fieldMin) / x) < 0 ? g = 0 : g > 1 && (g = 1), s.color) {
                     var w = i.valueMin[0],
                         E = i.valueMax[0],
                         k = i.valueMin[1],
                         C = i.valueMax[1],
                         S = i.valueMin[2],
@@ -7669,138 +7698,138 @@
                     N = N[B[z]]
                 }
                 if (null != N && (n = this.parse(i.name, N, i.bypass, "mapping")), !n) return f(), !1;
                 n.mapping = i, i = n;
                 break;
             case o.fn:
                 var I = i.value,
-                    L = null != i.fnValue ? i.fnValue : I(e);
-                if (i.prevFnValue = L, null == L) return Ve("Custom function mappers may not return null (i.e. `" + i.name + "` for ele `" + e.id() + "` is null)"), !1;
-                if (!(n = this.parse(i.name, L, i.bypass, "mapping"))) return Ve("Custom function mappers may not return invalid values for the property type (i.e. `" + i.name + "` for ele `" + e.id() + "` is invalid)"), !1;
-                n.mapping = Fe(i), i = n;
+                    A = null != i.fnValue ? i.fnValue : I(e);
+                if (i.prevFnValue = A, null == A) return Fe("Custom function mappers may not return null (i.e. `" + i.name + "` for ele `" + e.id() + "` is null)"), !1;
+                if (!(n = this.parse(i.name, A, i.bypass, "mapping"))) return Fe("Custom function mappers may not return invalid values for the property type (i.e. `" + i.name + "` for ele `" + e.id() + "` is invalid)"), !1;
+                n.mapping = je(i), i = n;
                 break;
             case void 0:
                 break;
             default:
                 return !1
         }
         return l ? (i.bypassed = c ? u.bypassed : u, a[i.name] = i) : c ? u.bypassed = i : a[i.name] = i, p(), !0
-    }, ws.cleanElements = function(e, t) {
+    }, ks.cleanElements = function(e, t) {
         for (var n = 0; n < e.length; n++) {
             var r = e[n];
             if (this.clearStyleHints(r), r.dirtyCompoundBoundsCache(), r.dirtyBoundingBoxCache(), t)
                 for (var i = r._private.style, a = Object.keys(i), o = 0; o < a.length; o++) {
                     var s = a[o],
                         l = i[s];
                     null != l && (l.bypass ? l.bypassed = null : i[s] = null)
                 } else r._private.style = {}
         }
-    }, ws.update = function() {
+    }, ks.update = function() {
         this._private.cy.mutableElements().updateStyle()
-    }, ws.updateTransitions = function(e, t) {
+    }, ks.updateTransitions = function(e, t) {
         var n = this,
             r = e._private,
             i = e.pstyle("transition-property").value,
             a = e.pstyle("transition-duration").pfValue,
             o = e.pstyle("transition-delay").pfValue;
         if (i.length > 0 && a > 0) {
             for (var s = {}, l = !1, u = 0; u < i.length; u++) {
                 var c = i[u],
                     d = e.pstyle(c),
                     h = t[c];
                 if (h) {
                     var p = h.prev,
                         f = null != h.next ? h.next : d,
                         g = !1,
-                        y = void 0;
-                    p && (m(p.pfValue) && m(f.pfValue) ? (g = f.pfValue - p.pfValue, y = p.pfValue + 1e-6 * g) : m(p.value) && m(f.value) ? (g = f.value - p.value, y = p.value + 1e-6 * g) : v(p.value) && v(f.value) && (g = p.value[0] !== f.value[0] || p.value[1] !== f.value[1] || p.value[2] !== f.value[2], y = p.strValue), g && (s[c] = f.strValue, this.applyBypass(e, c, y), l = !0))
+                        v = void 0;
+                    p && (b(p.pfValue) && b(f.pfValue) ? (g = f.pfValue - p.pfValue, v = p.pfValue + 1e-6 * g) : b(p.value) && b(f.value) ? (g = f.value - p.value, v = p.value + 1e-6 * g) : y(p.value) && y(f.value) && (g = p.value[0] !== f.value[0] || p.value[1] !== f.value[1] || p.value[2] !== f.value[2], v = p.strValue), g && (s[c] = f.strValue, this.applyBypass(e, c, v), l = !0))
                 }
             }
             if (!l) return;
-            r.transitioning = !0, new pr((function(t) {
+            r.transitioning = !0, new gr((function(t) {
                 o > 0 ? e.delayAnimation(o).play().promise().then(t) : t()
             })).then((function() {
                 return e.animation({
                     style: s,
                     duration: a,
                     easing: e.pstyle("transition-timing-function").value,
                     queue: !1
                 }).play().promise()
             })).then((function() {
                 n.removeBypasses(e, i), e.emitAndNotify("style"), r.transitioning = !1
             }))
         } else r.transitioning && (this.removeBypasses(e, i), e.emitAndNotify("style"), r.transitioning = !1)
-    }, ws.checkTrigger = function(e, t, n, r, i, a) {
+    }, ks.checkTrigger = function(e, t, n, r, i, a) {
         var o = this.properties[t],
             s = i(o);
         null != s && s(n, r) && a(o)
-    }, ws.checkZOrderTrigger = function(e, t, n, r) {
+    }, ks.checkZOrderTrigger = function(e, t, n, r) {
         var i = this;
         this.checkTrigger(e, t, n, r, (function(e) {
             return e.triggersZOrder
         }), (function() {
             i._private.cy.notify("zorder", e)
         }))
-    }, ws.checkBoundsTrigger = function(e, t, n, r) {
+    }, ks.checkBoundsTrigger = function(e, t, n, r) {
         this.checkTrigger(e, t, n, r, (function(e) {
             return e.triggersBounds
         }), (function(i) {
             e.dirtyCompoundBoundsCache(), e.dirtyBoundingBoxCache(), !i.triggersBoundsOfParallelBeziers || "curve-style" !== t || "bezier" !== n && "bezier" !== r || e.parallelEdges().forEach((function(e) {
                 e.isBundledBezier() && e.dirtyBoundingBoxCache()
             })), !i.triggersBoundsOfConnectedEdges || "display" !== t || "none" !== n && "none" !== r || e.connectedEdges().forEach((function(e) {
                 e.dirtyBoundingBoxCache()
             }))
         }))
-    }, ws.checkTriggers = function(e, t, n, r) {
+    }, ks.checkTriggers = function(e, t, n, r) {
         e.dirtyStyleCache(), this.checkZOrderTrigger(e, t, n, r), this.checkBoundsTrigger(e, t, n, r)
     };
-    var Es = {
+    var Cs = {
             applyBypass: function(e, t, n, r) {
                 var i = [];
                 if ("*" === t || "**" === t) {
                     if (void 0 !== n)
                         for (var a = 0; a < this.properties.length; a++) {
                             var o = this.properties[a].name,
                                 s = this.parse(o, n, !0);
                             s && i.push(s)
                         }
-                } else if (f(t)) {
+                } else if (g(t)) {
                     var l = this.parse(t, n, !0);
                     l && i.push(l)
                 } else {
-                    if (!y(t)) return !1;
+                    if (!m(t)) return !1;
                     var u = t;
                     r = n;
                     for (var c = Object.keys(u), d = 0; d < c.length; d++) {
                         var h = c[d],
                             p = u[h];
-                        if (void 0 === p && (p = u[_(h)]), void 0 !== p) {
-                            var g = this.parse(h, p, !0);
-                            g && i.push(g)
+                        if (void 0 === p && (p = u[M(h)]), void 0 !== p) {
+                            var f = this.parse(h, p, !0);
+                            f && i.push(f)
                         }
                     }
                 }
                 if (0 === i.length) return !1;
-                for (var v = !1, m = 0; m < e.length; m++) {
-                    for (var b = e[m], x = {}, w = void 0, E = 0; E < i.length; E++) {
+                for (var v = !1, y = 0; y < e.length; y++) {
+                    for (var b = e[y], x = {}, w = void 0, E = 0; E < i.length; E++) {
                         var k = i[E];
                         if (r) {
                             var C = b.pstyle(k.name);
                             w = x[k.name] = {
                                 prev: C
                             }
                         }
-                        v = this.applyParsedProperty(b, Fe(k)) || v, r && (w.next = b.pstyle(k.name))
+                        v = this.applyParsedProperty(b, je(k)) || v, r && (w.next = b.pstyle(k.name))
                     }
                     v && this.updateStyleHints(b), r && this.updateTransitions(b, x, !0)
                 }
                 return v
             },
             overrideBypass: function(e, t, n) {
-                t = T(t);
+                t = _(t);
                 for (var r = 0; r < e.length; r++) {
                     var i = e[r],
                         a = i._private.style[t],
                         o = this.properties[t].type,
                         s = o.color,
                         l = o.mutiple,
                         u = a ? null != a.pfValue ? a.pfValue : a.value : null;
@@ -7824,36 +7853,36 @@
                             this.applyParsedProperty(i, c), d.next = i.pstyle(l.name)
                         }
                     }
                     this.updateStyleHints(i), n && this.updateTransitions(i, a, !0)
                 }
             }
         },
-        ks = {
+        Ss = {
             getEmSizeInPixels: function() {
                 var e = this.containerCss("font-size");
                 return null != e ? parseFloat(e) : 1
             },
             containerCss: function(e) {
                 var t = this._private.cy,
                     n = t.container(),
                     r = t.window();
                 if (r && n && r.getComputedStyle) return r.getComputedStyle(n).getPropertyValue(e)
             }
         },
-        Cs = {
+        Ps = {
             getRenderedStyle: function(e, t) {
                 return t ? this.getStylePropertyValue(e, t, !0) : this.getRawStyle(e, !0)
             },
             getRawStyle: function(e, t) {
                 if (e = e[0]) {
                     for (var n = {}, r = 0; r < this.properties.length; r++) {
                         var i = this.properties[r],
                             a = this.getStylePropertyValue(e, i.name, t);
-                        null != a && (n[i.name] = a, n[_(i.name)] = a)
+                        null != a && (n[i.name] = a, n[M(i.name)] = a)
                     }
                     return n
                 }
             },
             getIndexedStyle: function(e, t, n, r) {
                 var i = e.pstyle(t)[n][r];
                 return null != i ? i : e.cy().style().getDefaultProperty(t)[n][0]
@@ -7864,70 +7893,70 @@
                     r.alias && (r = r.pointsTo);
                     var i = r.type,
                         a = e.pstyle(r.name);
                     if (a) {
                         var o = a.value,
                             s = a.units,
                             l = a.strValue;
-                        if (n && i.number && null != o && m(o)) {
+                        if (n && i.number && null != o && b(o)) {
                             var u = e.cy().zoom(),
                                 c = function(e) {
                                     return e * u
                                 },
                                 d = function(e, t) {
                                     return c(e) + t
                                 },
-                                h = v(o);
+                                h = y(o);
                             return (h ? s.every((function(e) {
                                 return null != e
                             })) : null != s) ? h ? o.map((function(e, t) {
                                 return d(e, s[t])
                             })).join(" ") : d(o, s) : h ? o.map((function(e) {
-                                return f(e) ? e : "" + c(e)
+                                return g(e) ? e : "" + c(e)
                             })).join(" ") : "" + c(o)
                         }
                         if (null != l) return l
                     }
                     return null
                 }
             },
             getAnimationStartStyle: function(e, t) {
                 for (var n = {}, r = 0; r < t.length; r++) {
                     var i = t[r].name,
                         a = e.pstyle(i);
-                    void 0 !== a && (a = y(a) ? this.parse(i, a.strValue) : this.parse(i, a)), a && (n[i] = a)
+                    void 0 !== a && (a = m(a) ? this.parse(i, a.strValue) : this.parse(i, a)), a && (n[i] = a)
                 }
                 return n
             },
             getPropsList: function(e) {
                 var t = [],
                     n = e,
                     r = this.properties;
                 if (n)
                     for (var i = Object.keys(n), a = 0; a < i.length; a++) {
                         var o = i[a],
                             s = n[o],
-                            l = r[o] || r[T(o)],
+                            l = r[o] || r[_(o)],
                             u = this.parse(l.name, s);
                         u && t.push(u)
                     }
                 return t
             },
             getNonDefaultPropertiesHash: function(e, t, n) {
                 var r, i, a, o, s, l, u = n.slice();
                 for (s = 0; s < t.length; s++)
                     if (r = t[s], null != (i = e.pstyle(r, !1)))
-                        if (null != i.pfValue) u[0] = Ee(o, u[0]), u[1] = ke(o, u[1]);
+                        if (null != i.pfValue) u[0] = ke(o, u[0]), u[1] = Ce(o, u[1]);
                         else
-                            for (a = i.strValue, l = 0; l < a.length; l++) o = a.charCodeAt(l), u[0] = Ee(o, u[0]), u[1] = ke(o, u[1]);
+                            for (a = i.strValue, l = 0; l < a.length; l++) o = a.charCodeAt(l), u[0] = ke(o, u[0]), u[1] = Ce(o, u[1]);
                 return u
             }
         };
-    Cs.getPropertiesHash = Cs.getNonDefaultPropertiesHash;
-    var Ss = {
+    Ps.getPropertiesHash = Ps.getNonDefaultPropertiesHash;
+    var Ds = {
             appendFromJson: function(e) {
                 for (var t = 0; t < e.length; t++) {
                     var n = e[t],
                         r = n.selector,
                         i = n.style || n.css,
                         a = Object.keys(i);
                     this.selector(r);
@@ -7952,56 +7981,56 @@
                         selector: r ? r.toString() : "core",
                         style: a
                     })
                 }
                 return e
             }
         },
-        Ps = {
+        Ts = {
             appendFromString: function(e) {
                 var t, n, r, i = "" + e;
 
                 function a() {
                     i = i.length > t.length ? i.substr(t.length) : ""
                 }
 
                 function o() {
                     n = n.length > r.length ? n.substr(r.length) : ""
                 }
                 for (i = i.replace(/[/][*](\s|.)+?[*][/]/g, "");;) {
                     if (i.match(/^\s*$/)) break;
                     var s = i.match(/^\s*((?:.|\s)+?)\s*\{((?:.|\s)+?)\}/);
                     if (!s) {
-                        Ve("Halting stylesheet parsing: String stylesheet contains more to parse but no selector and block found in: " + i);
+                        Fe("Halting stylesheet parsing: String stylesheet contains more to parse but no selector and block found in: " + i);
                         break
                     }
                     t = s[0];
                     var l = s[1];
                     if ("core" !== l)
-                        if (new xa(l).invalid) {
-                            Ve("Skipping parsing of block: Invalid selector found in string stylesheet: " + l), a();
+                        if (new Ea(l).invalid) {
+                            Fe("Skipping parsing of block: Invalid selector found in string stylesheet: " + l), a();
                             continue
                         } var u = s[2],
                         c = !1;
                     n = u;
                     for (var d = [];;) {
                         if (n.match(/^\s*$/)) break;
                         var h = n.match(/^\s*(.+?)\s*:\s*(.+?)(?:\s*;|\s*$)/);
                         if (!h) {
-                            Ve("Skipping parsing of block: Invalid formatting of style property and value definitions found in:" + u), c = !0;
+                            Fe("Skipping parsing of block: Invalid formatting of style property and value definitions found in:" + u), c = !0;
                             break
                         }
                         r = h[0];
                         var p = h[1],
                             f = h[2];
                         if (this.properties[p]) this.parse(p, f) ? (d.push({
                             name: p,
                             val: f
-                        }), o()) : (Ve("Skipping property: Invalid property definition in: " + r), o());
-                        else Ve("Skipping property: Invalid property name in: " + r), o()
+                        }), o()) : (Fe("Skipping property: Invalid property definition in: " + r), o());
+                        else Fe("Skipping property: Invalid property name in: " + r), o()
                     }
                     if (c) {
                         a();
                         break
                     }
                     this.selector(l);
                     for (var g = 0; g < d.length; g++) {
@@ -8012,26 +8041,26 @@
                 }
                 return this
             },
             fromString: function(e) {
                 return this.resetToDefault(), this.appendFromString(e), this
             }
         },
-        Ds = {};
+        _s = {};
     ! function() {
-        var e = N,
+        var e = z,
             t = function(e) {
                 return "^" + e + "\\s*\\(\\s*([\\w\\.]+)\\s*\\)$"
             },
             n = function(t) {
                 var n = e + "|\\w+|rgb[a]?\\((?:(?:[-+]?(?:(?:\\d+|\\d*\\.\\d+)(?:[Ee][+-]?\\d+)?))[%]?)\\s*,\\s*(?:(?:[-+]?(?:(?:\\d+|\\d*\\.\\d+)(?:[Ee][+-]?\\d+)?))[%]?)\\s*,\\s*(?:(?:[-+]?(?:(?:\\d+|\\d*\\.\\d+)(?:[Ee][+-]?\\d+)?))[%]?)(?:\\s*,\\s*(?:(?:[-+]?(?:(?:\\d+|\\d*\\.\\d+)(?:[Ee][+-]?\\d+)?))))?\\)|hsl[a]?\\((?:(?:[-+]?(?:(?:\\d+|\\d*\\.\\d+)(?:[Ee][+-]?\\d+)?)))\\s*,\\s*(?:(?:[-+]?(?:(?:\\d+|\\d*\\.\\d+)(?:[Ee][+-]?\\d+)?))[%])\\s*,\\s*(?:(?:[-+]?(?:(?:\\d+|\\d*\\.\\d+)(?:[Ee][+-]?\\d+)?))[%])(?:\\s*,\\s*(?:(?:[-+]?(?:(?:\\d+|\\d*\\.\\d+)(?:[Ee][+-]?\\d+)?))))?\\)|\\#[0-9a-fA-F]{3}|\\#[0-9a-fA-F]{6}";
                 return "^" + t + "\\s*\\(([\\w\\.]+)\\s*\\,\\s*(" + e + ")\\s*\\,\\s*(" + e + ")\\s*,\\s*(" + n + ")\\s*\\,\\s*(" + n + ")\\)$"
             },
             r = ["^url\\s*\\(\\s*['\"]?(.+?)['\"]?\\s*\\)$", "^(none)$", "^(.+)$"];
-        Ds.types = {
+        _s.types = {
             time: {
                 number: !0,
                 min: 0,
                 units: "s|ms",
                 implicitUnits: "ms"
             },
             percent: {
@@ -8183,19 +8212,29 @@
             },
             lineStyle: {
                 enums: ["solid", "dotted", "dashed"]
             },
             lineCap: {
                 enums: ["butt", "round", "square"]
             },
+            linePosition: {
+                enums: ["center", "inside", "outside"]
+            },
+            lineJoin: {
+                enums: ["round", "bevel", "miter"]
+            },
             borderStyle: {
                 enums: ["solid", "dotted", "dashed", "double"]
             },
             curveStyle: {
-                enums: ["bezier", "unbundled-bezier", "haystack", "segments", "straight", "straight-triangle", "taxi"]
+                enums: ["bezier", "unbundled-bezier", "haystack", "segments", "straight", "straight-triangle", "taxi", "round-segments", "round-taxi"]
+            },
+            radiusType: {
+                enums: ["arc-radius", "influence-radius"],
+                multiple: !0
             },
             fontFamily: {
                 regex: '^([\\w- \\"]+(?:\\s*,\\s*[\\w- \\"]+)*)$'
             },
             fontStyle: {
                 enums: ["italic", "normal", "oblique"]
             },
@@ -8219,14 +8258,21 @@
             },
             nodeShape: {
                 enums: ["rectangle", "roundrectangle", "round-rectangle", "cutrectangle", "cut-rectangle", "bottomroundrectangle", "bottom-round-rectangle", "barrel", "ellipse", "triangle", "round-triangle", "square", "pentagon", "round-pentagon", "hexagon", "round-hexagon", "concavehexagon", "concave-hexagon", "heptagon", "round-heptagon", "octagon", "round-octagon", "tag", "round-tag", "star", "diamond", "round-diamond", "vee", "rhomboid", "right-rhomboid", "polygon"]
             },
             overlayShape: {
                 enums: ["roundrectangle", "round-rectangle", "ellipse"]
             },
+            cornerRadius: {
+                number: !0,
+                min: 0,
+                units: "px|em",
+                implicitUnits: "px",
+                enums: ["auto"]
+            },
             compoundIncludeLabels: {
                 enums: ["include", "exclude"]
             },
             arrowShape: {
                 enums: ["tee", "triangle", "triangle-tee", "circle-triangle", "triangle-cross", "triangle-backcurve", "vee", "square", "circle", "diamond", "chevron", "none"]
             },
             arrowFill: {
@@ -8332,15 +8378,15 @@
                 enums: ["inside-to-node", "outside-to-node", "outside-to-node-or-label", "outside-to-line", "outside-to-line-or-label"],
                 singleEnum: !0,
                 validate: function(e, t) {
                     switch (e.length) {
                         case 2:
                             return "deg" !== t[0] && "rad" !== t[0] && "deg" !== t[1] && "rad" !== t[1];
                         case 1:
-                            return f(e[0]) || "deg" === t[0] || "rad" === t[0];
+                            return g(e[0]) || "deg" === t[0] || "rad" === t[0];
                         default:
                             return !1
                     }
                 }
             },
             easing: {
                 regexes: ["^(spring)\\s*\\(\\s*(" + e + ")\\s*,\\s*(" + e + ")\\s*\\)$", "^(cubic-bezier)\\s*\\(\\s*(" + e + ")\\s*,\\s*(" + e + ")\\s*,\\s*(" + e + ")\\s*,\\s*(" + e + ")\\s*\\)$"],
@@ -8363,20 +8409,20 @@
                 zeroNonZero: function(e, t) {
                     return (null == e || null == t) && e !== t || (0 == e && 0 != t || 0 != e && 0 == t)
                 },
                 any: function(e, t) {
                     return e != t
                 },
                 emptyNonEmpty: function(e, t) {
-                    var n = S(e),
-                        r = S(t);
+                    var n = P(e),
+                        r = P(t);
                     return n && !r || !n && r
                 }
             },
-            a = Ds.types,
+            a = _s.types,
             o = [{
                 name: "label",
                 type: a.text,
                 triggersBounds: i.any,
                 triggersZOrder: i.emptyNonEmpty
             }, {
                 name: "text-rotation",
@@ -8576,30 +8622,36 @@
                 name: "overlay-opacity",
                 type: a.zeroOneNumber,
                 triggersBounds: i.zeroNonZero
             }, {
                 name: "overlay-shape",
                 type: a.overlayShape,
                 triggersBounds: i.any
+            }, {
+                name: "overlay-corner-radius",
+                type: a.cornerRadius
             }],
-            g = [{
+            f = [{
                 name: "underlay-padding",
                 type: a.size,
                 triggersBounds: i.any
             }, {
                 name: "underlay-color",
                 type: a.color
             }, {
                 name: "underlay-opacity",
                 type: a.zeroOneNumber,
                 triggersBounds: i.zeroNonZero
             }, {
                 name: "underlay-shape",
                 type: a.overlayShape,
                 triggersBounds: i.any
+            }, {
+                name: "underlay-corner-radius",
+                type: a.cornerRadius
             }],
             v = [{
                 name: "transition-property",
                 type: a.propList
             }, {
                 name: "transition-duration",
                 type: a.time
@@ -8628,14 +8680,17 @@
                 type: a.nodeShape,
                 triggersBounds: i.any
             }, {
                 name: "shape-polygon-points",
                 type: a.polygonPointList,
                 triggersBounds: i.any
             }, {
+                name: "corner-radius",
+                type: a.cornerRadius
+            }, {
                 name: "background-color",
                 type: a.color
             }, {
                 name: "background-fill",
                 type: a.fill
             }, {
                 name: "background-opacity",
@@ -8674,14 +8729,29 @@
             }, {
                 name: "border-width",
                 type: a.size,
                 triggersBounds: i.any
             }, {
                 name: "border-style",
                 type: a.borderStyle
+            }, {
+                name: "border-cap",
+                type: a.lineCap
+            }, {
+                name: "border-join",
+                type: a.lineJoin
+            }, {
+                name: "border-dash-pattern",
+                type: a.numbers
+            }, {
+                name: "border-dash-offset",
+                type: a.number
+            }, {
+                name: "border-position",
+                type: a.linePosition
             }],
             x = [{
                 name: "outline-color",
                 type: a.color
             }, {
                 name: "outline-opacity",
                 type: a.zeroOneNumber
@@ -8840,26 +8910,38 @@
                 type: a.bidirectionalSizes,
                 triggersBounds: i.any
             }, {
                 name: "segment-weights",
                 type: a.numbers,
                 triggersBounds: i.any
             }, {
+                name: "segment-radii",
+                type: a.numbers,
+                triggersBounds: i.any
+            }, {
+                name: "radius-type",
+                type: a.radiusType,
+                triggersBounds: i.any
+            }, {
                 name: "taxi-turn",
                 type: a.bidirectionalSizeMaybePercent,
                 triggersBounds: i.any
             }, {
                 name: "taxi-turn-min-distance",
                 type: a.size,
                 triggersBounds: i.any
             }, {
                 name: "taxi-direction",
                 type: a.axisDirection,
                 triggersBounds: i.any
             }, {
+                name: "taxi-radius",
+                type: a.number,
+                triggersBounds: i.any
+            }, {
                 name: "edge-distances",
                 type: a.edgeDistances,
                 triggersBounds: i.any
             }, {
                 name: "arrow-scale",
                 type: a.positiveNumber,
                 triggersBounds: i.any
@@ -8892,15 +8974,15 @@
                 name: "ghost-offset-y",
                 type: a.bidirectionalSize,
                 triggersBounds: i.any
             }, {
                 name: "ghost-opacity",
                 type: a.zeroOneNumber
             }],
-            P = [{
+            S = [{
                 name: "selection-box-color",
                 type: a.color
             }, {
                 name: "selection-box-opacity",
                 type: a.zeroOneNumber
             }, {
                 name: "selection-box-border-color",
@@ -8921,30 +9003,30 @@
                 name: "outside-texture-bg-color",
                 type: a.color
             }, {
                 name: "outside-texture-bg-opacity",
                 type: a.zeroOneNumber
             }],
             D = [];
-        Ds.pieBackgroundN = 16, D.push({
+        _s.pieBackgroundN = 16, D.push({
             name: "pie-size",
             type: a.sizeMaybePercent
         });
-        for (var T = 1; T <= Ds.pieBackgroundN; T++) D.push({
+        for (var T = 1; T <= _s.pieBackgroundN; T++) D.push({
             name: "pie-" + T + "-background-color",
             type: a.color
         }), D.push({
             name: "pie-" + T + "-background-size",
             type: a.percent
         }), D.push({
             name: "pie-" + T + "-background-opacity",
             type: a.zeroOneNumber
         });
         var _ = [],
-            M = Ds.arrowPrefixes = ["source", "mid-source", "target", "mid-target"];
+            M = _s.arrowPrefixes = ["source", "mid-source", "target", "mid-target"];
         [{
             name: "arrow-shape",
             type: a.arrowShape,
             triggersBounds: i.any
         }, {
             name: "arrow-color",
             type: a.color
@@ -8962,55 +9044,64 @@
                 _.push({
                     name: n,
                     type: r,
                     triggersBounds: i
                 })
             }))
         }), {});
-        var B = Ds.properties = [].concat(d, v, h, p, g, C, c, u, o, s, l, m, b, x, w, D, E, k, _, P),
-            z = Ds.propertyGroups = {
+        var B = _s.properties = [].concat(d, v, h, p, f, C, c, u, o, s, l, m, b, x, w, D, E, k, _, S),
+            N = _s.propertyGroups = {
                 behavior: d,
                 transition: v,
                 visibility: h,
                 overlay: p,
-                underlay: g,
+                underlay: f,
                 ghost: C,
                 commonLabel: c,
                 labelDimensions: u,
                 mainLabel: o,
                 sourceLabel: s,
                 targetLabel: l,
                 nodeBody: m,
                 nodeBorder: b,
                 nodeOutline: x,
                 backgroundImage: w,
                 pie: D,
                 compound: E,
                 edgeLine: k,
                 edgeArrow: _,
-                core: P
+                core: S
             },
-            I = Ds.propertyGroupNames = {};
-        (Ds.propertyGroupKeys = Object.keys(z)).forEach((function(e) {
-            I[e] = z[e].map((function(e) {
+            I = _s.propertyGroupNames = {};
+        (_s.propertyGroupKeys = Object.keys(N)).forEach((function(e) {
+            I[e] = N[e].map((function(e) {
                 return e.name
-            })), z[e].forEach((function(t) {
+            })), N[e].forEach((function(t) {
                 return t.groupKey = e
             }))
         }));
-        var L = Ds.aliases = [{
+        var A = _s.aliases = [{
             name: "content",
             pointsTo: "label"
         }, {
             name: "control-point-distance",
             pointsTo: "control-point-distances"
         }, {
             name: "control-point-weight",
             pointsTo: "control-point-weights"
         }, {
+            name: "segment-distance",
+            pointsTo: "segment-distances"
+        }, {
+            name: "segment-weight",
+            pointsTo: "segment-weights"
+        }, {
+            name: "segment-radius",
+            pointsTo: "segment-radii"
+        }, {
             name: "edge-text-rotation",
             pointsTo: "text-rotation"
         }, {
             name: "padding-left",
             pointsTo: "padding"
         }, {
             name: "padding-right",
@@ -9018,37 +9109,37 @@
         }, {
             name: "padding-top",
             pointsTo: "padding"
         }, {
             name: "padding-bottom",
             pointsTo: "padding"
         }];
-        Ds.propertyNames = B.map((function(e) {
+        _s.propertyNames = B.map((function(e) {
             return e.name
         }));
-        for (var A = 0; A < B.length; A++) {
-            var O = B[A];
+        for (var L = 0; L < B.length; L++) {
+            var O = B[L];
             B[O.name] = O
         }
-        for (var R = 0; R < L.length; R++) {
-            var V = L[R],
+        for (var R = 0; R < A.length; R++) {
+            var V = A[R],
                 F = B[V.pointsTo],
                 j = {
                     name: V.name,
                     alias: !0,
                     pointsTo: F
                 };
             B.push(j), B[V.name] = j
         }
-    }(), Ds.getDefaultProperty = function(e) {
+    }(), _s.getDefaultProperty = function(e) {
         return this.getDefaultProperties()[e]
-    }, Ds.getDefaultProperties = function() {
+    }, _s.getDefaultProperties = function() {
         var e = this._private;
         if (null != e.defaultProperties) return e.defaultProperties;
-        for (var t = I({
+        for (var t = A({
                 "selection-box-color": "#ddd",
                 "selection-box-opacity": .65,
                 "selection-box-border-color": "#aaa",
                 "selection-box-border-width": 1,
                 "active-bg-color": "black",
                 "active-bg-opacity": .15,
                 "active-bg-size": 30,
@@ -9103,18 +9194,20 @@
                 "target-text-offset": 0,
                 "target-text-margin-x": 0,
                 "target-text-margin-y": 0,
                 "overlay-opacity": 0,
                 "overlay-color": "#000",
                 "overlay-padding": 10,
                 "overlay-shape": "round-rectangle",
+                "overlay-corner-radius": "auto",
                 "underlay-opacity": 0,
                 "underlay-color": "#000",
                 "underlay-padding": 10,
                 "underlay-shape": "round-rectangle",
+                "underlay-corner-radius": "auto",
                 "transition-property": "none",
                 "transition-duration": 0,
                 "transition-delay": 0,
                 "transition-timing-function": "linear",
                 "background-blacken": 0,
                 "background-color": "#999",
                 "background-fill": "solid",
@@ -9135,23 +9228,29 @@
                 "background-clip": "node",
                 "background-width": "auto",
                 "background-height": "auto",
                 "border-color": "#000",
                 "border-opacity": 1,
                 "border-width": 0,
                 "border-style": "solid",
+                "border-dash-pattern": [4, 2],
+                "border-dash-offset": 0,
+                "border-cap": "butt",
+                "border-join": "miter",
+                "border-position": "center",
                 "outline-color": "#999",
                 "outline-opacity": 1,
                 "outline-width": 0,
                 "outline-offset": 0,
                 "outline-style": "solid",
                 height: 30,
                 width: 30,
                 shape: "ellipse",
                 "shape-polygon-points": "-1, -1,   1, -1,   1, 1,   -1, 1",
+                "corner-radius": "auto",
                 "bounds-expansion": 0,
                 "background-gradient-direction": "to-bottom",
                 "background-gradient-stop-colors": "#999",
                 "background-gradient-stop-positions": "0%",
                 ghost: "no",
                 "ghost-offset-y": 0,
                 "ghost-offset-x": 0,
@@ -9174,15 +9273,15 @@
             }, {
                 name: "pie-{{i}}-background-size",
                 value: "0%"
             }, {
                 name: "pie-{{i}}-background-opacity",
                 value: 1
             }].reduce((function(e, t) {
-                for (var n = 1; n <= Ds.pieBackgroundN; n++) {
+                for (var n = 1; n <= _s.pieBackgroundN; n++) {
                     var r = t.name.replace("{{i}}", n),
                         i = t.value;
                     e[r] = i
                 }
                 return e
             }), {}), {
                 "line-style": "solid",
@@ -9192,15 +9291,18 @@
                 "line-opacity": 1,
                 "line-gradient-stop-colors": "#999",
                 "line-gradient-stop-positions": "0%",
                 "control-point-step-size": 40,
                 "control-point-weights": .5,
                 "segment-weights": .5,
                 "segment-distances": 20,
+                "segment-radii": 15,
+                "radius-type": "arc-radius",
                 "taxi-turn": "50%",
+                "taxi-radius": 15,
                 "taxi-turn-min-distance": 10,
                 "taxi-direction": "auto",
                 "edge-distances": "intersection",
                 "curve-style": "haystack",
                 "haystack-radius": 0,
                 "arrow-scale": 1,
                 "loop-direction": "-45deg",
@@ -9220,30 +9322,30 @@
             }, {
                 name: "arrow-fill",
                 value: "filled"
             }, {
                 name: "arrow-width",
                 value: 1
             }].reduce((function(e, t) {
-                return Ds.arrowPrefixes.forEach((function(n) {
+                return _s.arrowPrefixes.forEach((function(n) {
                     var r = n + "-" + t.name,
                         i = t.value;
                     e[r] = i
                 })), e
             }), {})), n = {}, r = 0; r < this.properties.length; r++) {
             var i = this.properties[r];
             if (!i.pointsTo) {
                 var a = i.name,
                     o = t[a],
                     s = this.parse(a, o);
                 n[a] = s
             }
         }
         return e.defaultProperties = n, e.defaultProperties
-    }, Ds.addDefaultStylesheet = function() {
+    }, _s.addDefaultStylesheet = function() {
         this.selector(":parent").css({
             shape: "rectangle",
             padding: 10,
             "background-color": "#eee",
             "border-color": "#ccc",
             "border-width": 1
         }).selector("edge").css({
@@ -9266,45 +9368,45 @@
             "border-color": "#aec8e5"
         }).selector(":active").css({
             "overlay-color": "black",
             "overlay-padding": 10,
             "overlay-opacity": .25
         }), this.defaultLength = this.length
     };
-    var Ts = {
+    var Ms = {
         parse: function(e, t, n, r) {
-            if (g(t)) return this.parseImplWarn(e, t, n, r);
-            var i, a = De(e, "" + t, n ? "t" : "f", "mapping" === r || !0 === r || !1 === r || null == r ? "dontcare" : r),
+            if (v(t)) return this.parseImplWarn(e, t, n, r);
+            var i, a = Te(e, "" + t, n ? "t" : "f", "mapping" === r || !0 === r || !1 === r || null == r ? "dontcare" : r),
                 o = this.propCache = this.propCache || [];
-            return (i = o[a]) || (i = o[a] = this.parseImplWarn(e, t, n, r)), (n || "mapping" === r) && (i = Fe(i)) && (i.value = Fe(i.value)), i
+            return (i = o[a]) || (i = o[a] = this.parseImplWarn(e, t, n, r)), (n || "mapping" === r) && (i = je(i)) && (i.value = je(i.value)), i
         },
         parseImplWarn: function(e, t, n, r) {
             var i = this.parseImpl(e, t, n, r);
-            return i || null == t || Ve("The style property `".concat(e, ": ").concat(t, "` is invalid")), !i || "width" !== i.name && "height" !== i.name || "label" !== t || Ve("The style value of `label` is deprecated for `" + i.name + "`"), i
+            return i || null == t || Fe("The style property `".concat(e, ": ").concat(t, "` is invalid")), !i || "width" !== i.name && "height" !== i.name || "label" !== t || Fe("The style value of `label` is deprecated for `" + i.name + "`"), i
         }
     };
-    Ts.parseImpl = function(e, t, n, r) {
-        e = T(e);
+    Ms.parseImpl = function(e, t, n, r) {
+        e = _(e);
         var i = this.properties[e],
             a = t,
             o = this.types;
         if (!i) return null;
         if (void 0 === t) return null;
         i.alias && (i = i.pointsTo, e = i.name);
-        var s = f(t);
+        var s = g(t);
         s && (t = t.trim());
         var l, u, c = i.type;
         if (!c) return null;
         if (n && ("" === t || null === t)) return {
             name: e,
             value: t,
             bypass: !0,
             deleteBypass: !0
         };
-        if (g(t)) return {
+        if (v(t)) return {
             name: e,
             value: t,
             strValue: "fn",
             mapped: o.fn,
             bypass: n
         };
         if (!s || r || t.length < 7 || "a" !== t[1]);
@@ -9324,58 +9426,58 @@
             if (t.length >= 10 && "m" === t[0] && (u = new RegExp(o.mapData.regex).exec(t))) {
                 if (n) return !1;
                 if (c.multiple) return !1;
                 var h = o.mapData;
                 if (!c.color && !c.number) return !1;
                 var p = this.parse(e, u[4]);
                 if (!p || p.mapped) return !1;
-                var y = this.parse(e, u[5]);
-                if (!y || y.mapped) return !1;
-                if (p.pfValue === y.pfValue || p.strValue === y.strValue) return Ve("`" + e + ": " + t + "` is not a valid mapper because the output range is zero; converting to `" + e + ": " + p.strValue + "`"), this.parse(e, p.strValue);
+                var f = this.parse(e, u[5]);
+                if (!f || f.mapped) return !1;
+                if (p.pfValue === f.pfValue || p.strValue === f.strValue) return Fe("`" + e + ": " + t + "` is not a valid mapper because the output range is zero; converting to `" + e + ": " + p.strValue + "`"), this.parse(e, p.strValue);
                 if (c.color) {
-                    var b = p.value,
-                        x = y.value;
-                    if (!(b[0] !== x[0] || b[1] !== x[1] || b[2] !== x[2] || b[3] !== x[3] && (null != b[3] && 1 !== b[3] || null != x[3] && 1 !== x[3]))) return !1
+                    var m = p.value,
+                        x = f.value;
+                    if (!(m[0] !== x[0] || m[1] !== x[1] || m[2] !== x[2] || m[3] !== x[3] && (null != m[3] && 1 !== m[3] || null != x[3] && 1 !== x[3]))) return !1
                 }
                 return {
                     name: e,
                     value: u,
                     strValue: "" + t,
                     mapped: h,
                     field: u[1],
                     fieldMin: parseFloat(u[2]),
                     fieldMax: parseFloat(u[3]),
                     valueMin: p.value,
-                    valueMax: y.value,
+                    valueMax: f.value,
                     bypass: n
                 }
             }
         }
         if (c.multiple && "multiple" !== r) {
             var w;
-            if (w = s ? t.split(/\s+/) : v(t) ? t : [t], c.evenMultiple && w.length % 2 != 0) return null;
+            if (w = s ? t.split(/\s+/) : y(t) ? t : [t], c.evenMultiple && w.length % 2 != 0) return null;
             for (var E = [], k = [], C = [], S = "", P = !1, D = 0; D < w.length; D++) {
-                var _ = this.parse(e, w[D], n, "multiple");
-                P = P || f(_.value), E.push(_.value), C.push(null != _.pfValue ? _.pfValue : _.value), k.push(_.units), S += (D > 0 ? " " : "") + _.strValue
+                var T = this.parse(e, w[D], n, "multiple");
+                P = P || g(T.value), E.push(T.value), C.push(null != T.pfValue ? T.pfValue : T.value), k.push(T.units), S += (D > 0 ? " " : "") + T.strValue
             }
-            return c.validate && !c.validate(E, k) ? null : c.singleEnum && P ? 1 === E.length && f(E[0]) ? {
+            return c.validate && !c.validate(E, k) ? null : c.singleEnum && P ? 1 === E.length && g(E[0]) ? {
                 name: e,
                 value: E[0],
                 strValue: E[0],
                 bypass: n
             } : null : {
                 name: e,
                 value: E,
                 pfValue: C,
                 strValue: S,
                 bypass: n,
                 units: k
             }
         }
-        var M, B, z = function() {
+        var M, B, N = function() {
             for (var r = 0; r < c.enums.length; r++) {
                 if (c.enums[r] === t) return {
                     name: e,
                     value: t,
                     strValue: "" + t,
                     bypass: n
                 }
@@ -9384,20 +9486,20 @@
         };
         if (c.number) {
             var I, A = "px";
             if (c.units && (I = c.units), c.implicitUnits && (A = c.implicitUnits), !c.unitless)
                 if (s) {
                     var O = "px|em" + (c.allowPercent ? "|\\%" : "");
                     I && (O = I);
-                    var R = t.match("^(" + N + ")(" + O + ")?$");
+                    var R = t.match("^(" + z + ")(" + O + ")?$");
                     R && (t = R[1], I = R[2] || A)
                 } else I && !c.implicitUnits || (I = A);
             if (t = parseFloat(t), isNaN(t) && void 0 === c.enums) return null;
-            if (isNaN(t) && void 0 !== c.enums) return t = a, z();
-            if (c.integer && (!m(B = t) || Math.floor(B) !== B)) return null;
+            if (isNaN(t) && void 0 !== c.enums) return t = a, N();
+            if (c.integer && (!b(B = t) || Math.floor(B) !== B)) return null;
             if (void 0 !== c.min && (t < c.min || c.strictMin && t === c.min) || void 0 !== c.max && (t > c.max || c.strictMax && t === c.max)) return null;
             var V = {
                 name: e,
                 value: t,
                 strValue: "" + t + (I || ""),
                 units: I,
                 bypass: n
@@ -9407,15 +9509,15 @@
         if (c.propList) {
             var F = [],
                 j = "" + t;
             if ("none" === j);
             else {
                 for (var q = j.split(/\s*,\s*|\s+/), Y = 0; Y < q.length; Y++) {
                     var X = q[Y].trim();
-                    this.properties[X] ? F.push(X) : Ve("`" + X + "` is not a valid property name")
+                    this.properties[X] ? F.push(X) : Fe("`" + X + "` is not a valid property name")
                 }
                 if (0 === F.length) return null
             }
             return {
                 name: e,
                 value: F,
                 strValue: 0 === F.length ? "none" : F.join(" "),
@@ -9430,15 +9532,15 @@
                 pfValue: W,
                 strValue: "rgb(" + W[0] + "," + W[1] + "," + W[2] + ")",
                 bypass: n
             } : null
         }
         if (c.regex || c.regexes) {
             if (c.enums) {
-                var H = z();
+                var H = N();
                 if (H) return H
             }
             for (var K = c.regexes ? c.regexes : [c.regex], G = 0; G < K.length; G++) {
                 var U = new RegExp(K[G]).exec(t);
                 if (U) return {
                     name: e,
                     value: c.singleRegexMatchValue ? U[1] : U,
@@ -9449,86 +9551,86 @@
             return null
         }
         return c.string ? {
             name: e,
             value: "" + t,
             strValue: "" + t,
             bypass: n
-        } : c.enums ? z() : null
+        } : c.enums ? N() : null
     };
-    var _s = function e(t) {
+    var Bs = function e(t) {
             if (!(this instanceof e)) return new e(t);
-            k(t) ? (this._private = {
+            C(t) ? (this._private = {
                 cy: t,
                 coreStyle: {}
-            }, this.length = 0, this.resetToDefault()) : Oe("A style must have a core reference")
+            }, this.length = 0, this.resetToDefault()) : Re("A style must have a core reference")
         },
-        Ms = _s.prototype;
-    Ms.instanceString = function() {
+        Ns = Bs.prototype;
+    Ns.instanceString = function() {
         return "style"
-    }, Ms.clear = function() {
+    }, Ns.clear = function() {
         for (var e = this._private, t = e.cy.elements(), n = 0; n < this.length; n++) this[n] = void 0;
         return this.length = 0, e.contextStyles = {}, e.propDiffs = {}, this.cleanElements(t, !0), t.forEach((function(e) {
             var t = e[0]._private;
             t.styleDirty = !0, t.appliedInitStyle = !1
         })), this
-    }, Ms.resetToDefault = function() {
+    }, Ns.resetToDefault = function() {
         return this.clear(), this.addDefaultStylesheet(), this
-    }, Ms.core = function(e) {
+    }, Ns.core = function(e) {
         return this._private.coreStyle[e] || this.getDefaultProperty(e)
-    }, Ms.selector = function(e) {
-        var t = "core" === e ? null : new xa(e),
+    }, Ns.selector = function(e) {
+        var t = "core" === e ? null : new Ea(e),
             n = this.length++;
         return this[n] = {
             selector: t,
             properties: [],
             mappedProperties: [],
             index: n
         }, this
-    }, Ms.css = function() {
+    }, Ns.css = function() {
         var e = this,
             t = arguments;
         if (1 === t.length)
             for (var n = t[0], r = 0; r < e.properties.length; r++) {
                 var i = e.properties[r],
                     a = n[i.name];
-                void 0 === a && (a = n[_(i.name)]), void 0 !== a && this.cssRule(i.name, a)
+                void 0 === a && (a = n[M(i.name)]), void 0 !== a && this.cssRule(i.name, a)
             } else 2 === t.length && this.cssRule(t[0], t[1]);
         return this
-    }, Ms.style = Ms.css, Ms.cssRule = function(e, t) {
+    }, Ns.style = Ns.css, Ns.cssRule = function(e, t) {
         var n = this.parse(e, t);
         if (n) {
             var r = this.length - 1;
             this[r].properties.push(n), this[r].properties[n.name] = n, n.name.match(/pie-(\d+)-background-size/) && n.value && (this._private.hasPie = !0), n.mapped && this[r].mappedProperties.push(n), !this[r].selector && (this._private.coreStyle[n.name] = n)
         }
         return this
-    }, Ms.append = function(e) {
-        return C(e) ? e.appendToStyle(this) : v(e) ? this.appendFromJson(e) : f(e) && this.appendFromString(e), this
-    }, _s.fromJson = function(e, t) {
-        var n = new _s(e);
+    }, Ns.append = function(e) {
+        return S(e) ? e.appendToStyle(this) : y(e) ? this.appendFromJson(e) : g(e) && this.appendFromString(e), this
+    }, Bs.fromJson = function(e, t) {
+        var n = new Bs(e);
         return n.fromJson(t), n
-    }, _s.fromString = function(e, t) {
-        return new _s(e).fromString(t)
-    }, [ws, Es, ks, Cs, Ss, Ps, Ds, Ts].forEach((function(e) {
-        I(Ms, e)
-    })), _s.types = Ms.types, _s.properties = Ms.properties, _s.propertyGroups = Ms.propertyGroups, _s.propertyGroupNames = Ms.propertyGroupNames, _s.propertyGroupKeys = Ms.propertyGroupKeys;
-    var Bs = {
+    }, Bs.fromString = function(e, t) {
+        return new Bs(e).fromString(t)
+    }, [ks, Cs, Ss, Ps, Ds, Ts, _s, Ms].forEach((function(e) {
+        A(Ns, e)
+    })), Bs.types = Ns.types, Bs.properties = Ns.properties, Bs.propertyGroups = Ns.propertyGroups, Bs.propertyGroupNames = Ns.propertyGroupNames, Bs.propertyGroupKeys = Ns.propertyGroupKeys;
+    var zs = {
             style: function(e) {
                 e && this.setStyle(e).update();
                 return this._private.style
             },
             setStyle: function(e) {
                 var t = this._private;
-                return C(e) ? t.style = e.generateStyle(this) : v(e) ? t.style = _s.fromJson(this, e) : f(e) ? t.style = _s.fromString(this, e) : t.style = _s(this), t.style
+                return S(e) ? t.style = e.generateStyle(this) : y(e) ? t.style = Bs.fromJson(this, e) : g(e) ? t.style = Bs.fromString(this, e) : t.style = Bs(this), t.style
             },
             updateStyle: function() {
                 this.mutableElements().updateStyle()
             }
         },
-        Ns = {
+        Is = {
             autolock: function(e) {
                 return void 0 === e ? this._private.autolock : (this._private.autolock = !!e, this)
             },
             autoungrabify: function(e) {
                 return void 0 === e ? this._private.autoungrabify : (this._private.autoungrabify = !!e, this)
             },
             autounselectify: function(e) {
@@ -9556,67 +9658,67 @@
             pan: function() {
                 var e, t, n, r, i, a = arguments,
                     o = this._private.pan;
                 switch (a.length) {
                     case 0:
                         return o;
                     case 1:
-                        if (f(a[0])) return o[e = a[0]];
-                        if (y(a[0])) {
+                        if (g(a[0])) return o[e = a[0]];
+                        if (m(a[0])) {
                             if (!this._private.panningEnabled) return this;
-                            r = (n = a[0]).x, i = n.y, m(r) && (o.x = r), m(i) && (o.y = i), this.emit("pan viewport")
+                            r = (n = a[0]).x, i = n.y, b(r) && (o.x = r), b(i) && (o.y = i), this.emit("pan viewport")
                         }
                         break;
                     case 2:
                         if (!this._private.panningEnabled) return this;
-                        e = a[0], t = a[1], "x" !== e && "y" !== e || !m(t) || (o[e] = t), this.emit("pan viewport")
+                        e = a[0], t = a[1], "x" !== e && "y" !== e || !b(t) || (o[e] = t), this.emit("pan viewport")
                 }
                 return this.notify("viewport"), this
             },
             panBy: function(e, t) {
                 var n, r, i, a, o, s = arguments,
                     l = this._private.pan;
                 if (!this._private.panningEnabled) return this;
                 switch (s.length) {
                     case 1:
-                        y(e) && (a = (i = s[0]).x, o = i.y, m(a) && (l.x += a), m(o) && (l.y += o), this.emit("pan viewport"));
+                        m(e) && (a = (i = s[0]).x, o = i.y, b(a) && (l.x += a), b(o) && (l.y += o), this.emit("pan viewport"));
                         break;
                     case 2:
-                        r = t, "x" !== (n = e) && "y" !== n || !m(r) || (l[n] += r), this.emit("pan viewport")
+                        r = t, "x" !== (n = e) && "y" !== n || !b(r) || (l[n] += r), this.emit("pan viewport")
                 }
                 return this.notify("viewport"), this
             },
             fit: function(e, t) {
                 var n = this.getFitViewport(e, t);
                 if (n) {
                     var r = this._private;
                     r.zoom = n.zoom, r.pan = n.pan, this.emit("pan zoom viewport"), this.notify("viewport")
                 }
                 return this
             },
             getFitViewport: function(e, t) {
-                if (m(e) && void 0 === t && (t = e, e = void 0), this._private.panningEnabled && this._private.zoomingEnabled) {
+                if (b(e) && void 0 === t && (t = e, e = void 0), this._private.panningEnabled && this._private.zoomingEnabled) {
                     var n, r;
-                    if (f(e)) {
+                    if (g(e)) {
                         var i = e;
                         e = this.$(i)
-                    } else if (y(r = e) && m(r.x1) && m(r.x2) && m(r.y1) && m(r.y2)) {
+                    } else if (m(r = e) && b(r.x1) && b(r.x2) && b(r.y1) && b(r.y2)) {
                         var a = e;
                         (n = {
                             x1: a.x1,
                             y1: a.y1,
                             x2: a.x2,
                             y2: a.y2
                         }).w = n.x2 - n.x1, n.h = n.y2 - n.y1
-                    } else x(e) || (e = this.mutableElements());
-                    if (!x(e) || !e.empty()) {
+                    } else w(e) || (e = this.mutableElements());
+                    if (!w(e) || !e.empty()) {
                         n = n || e.boundingBox();
                         var o, s = this.width(),
                             l = this.height();
-                        if (t = m(t) ? t : 0, !isNaN(s) && !isNaN(l) && s > 0 && l > 0 && !isNaN(n.w) && !isNaN(n.h) && n.w > 0 && n.h > 0) return {
+                        if (t = b(t) ? t : 0, !isNaN(s) && !isNaN(l) && s > 0 && l > 0 && !isNaN(n.w) && !isNaN(n.h) && n.w > 0 && n.h > 0) return {
                             zoom: o = (o = (o = Math.min((s - 2 * t) / n.w, (l - 2 * t) / n.h)) > this._private.maxZoom ? this._private.maxZoom : o) < this._private.minZoom ? this._private.minZoom : o,
                             pan: {
                                 x: (s - o * (n.x1 + n.x2)) / 2,
                                 y: (l - o * (n.y1 + n.y2)) / 2
                             }
                         }
                     }
@@ -9624,15 +9726,15 @@
             },
             zoomRange: function(e, t) {
                 var n = this._private;
                 if (null == t) {
                     var r = e;
                     e = r.min, t = r.max
                 }
-                return m(e) && m(t) && e <= t ? (n.minZoom = e, n.maxZoom = t) : m(e) && void 0 === t && e <= n.maxZoom ? n.minZoom = e : m(t) && void 0 === e && t >= n.minZoom && (n.maxZoom = t), this
+                return b(e) && b(t) && e <= t ? (n.minZoom = e, n.maxZoom = t) : b(e) && void 0 === t && e <= n.maxZoom ? n.minZoom = e : b(t) && void 0 === e && t >= n.minZoom && (n.maxZoom = t), this
             },
             minZoom: function(e) {
                 return void 0 === e ? this._private.minZoom : this.zoomRange({
                     min: e
                 })
             },
             maxZoom: function(e) {
@@ -9641,15 +9743,15 @@
                 })
             },
             getZoomedViewport: function(e) {
                 var t, n, r = this._private,
                     i = r.pan,
                     a = r.zoom,
                     o = !1;
-                if (r.zoomingEnabled || (o = !0), m(e) ? n = e : y(e) && (n = e.level, null != e.position ? t = gt(e.position, a, i) : null != e.renderedPosition && (t = e.renderedPosition), null == t || r.panningEnabled || (o = !0)), n = (n = n > r.maxZoom ? r.maxZoom : n) < r.minZoom ? r.minZoom : n, o || !m(n) || n === a || null != t && (!m(t.x) || !m(t.y))) return null;
+                if (r.zoomingEnabled || (o = !0), b(e) ? n = e : m(e) && (n = e.level, null != e.position ? t = vt(e.position, a, i) : null != e.renderedPosition && (t = e.renderedPosition), null == t || r.panningEnabled || (o = !0)), n = (n = n > r.maxZoom ? r.maxZoom : n) < r.minZoom ? r.minZoom : n, o || !b(n) || n === a || null != t && (!b(t.x) || !b(t.y))) return null;
                 if (null != t) {
                     var s = i,
                         l = a,
                         u = n;
                     return {
                         zoomed: !0,
                         panned: !0,
@@ -9677,35 +9779,35 @@
                 var t = this._private,
                     n = !0,
                     r = !0,
                     i = [],
                     a = !1,
                     o = !1;
                 if (!e) return this;
-                if (m(e.zoom) || (n = !1), y(e.pan) || (r = !1), !n && !r) return this;
+                if (b(e.zoom) || (n = !1), m(e.pan) || (r = !1), !n && !r) return this;
                 if (n) {
                     var s = e.zoom;
                     s < t.minZoom || s > t.maxZoom || !t.zoomingEnabled ? a = !0 : (t.zoom = s, i.push("zoom"))
                 }
                 if (r && (!a || !e.cancelOnFailedZoom) && t.panningEnabled) {
                     var l = e.pan;
-                    m(l.x) && (t.pan.x = l.x, o = !1), m(l.y) && (t.pan.y = l.y, o = !1), o || i.push("pan")
+                    b(l.x) && (t.pan.x = l.x, o = !1), b(l.y) && (t.pan.y = l.y, o = !1), o || i.push("pan")
                 }
                 return i.length > 0 && (i.push("viewport"), this.emit(i.join(" ")), this.notify("viewport")), this
             },
             center: function(e) {
                 var t = this.getCenterPan(e);
                 return t && (this._private.pan = t, this.emit("pan viewport"), this.notify("viewport")), this
             },
             getCenterPan: function(e, t) {
                 if (this._private.panningEnabled) {
-                    if (f(e)) {
+                    if (g(e)) {
                         var n = e;
                         e = this.mutableElements().filter(n)
-                    } else x(e) || (e = this.mutableElements());
+                    } else w(e) || (e = this.mutableElements());
                     if (0 !== e.length) {
                         var r = e.boundingBox(),
                             i = this.width(),
                             a = this.height();
                         return {
                             x: (i - (t = void 0 === t ? this._private.zoom : t) * (r.x1 + r.x2)) / 2,
                             y: (a - t * (r.y1 + r.y2)) / 2
@@ -9769,144 +9871,144 @@
                     h: t
                 }
             },
             multiClickDebounceTime: function(e) {
                 return e ? (this._private.multiClickDebounceTime = e, this) : this._private.multiClickDebounceTime
             }
         };
-    Ns.centre = Ns.center, Ns.autolockNodes = Ns.autolock, Ns.autoungrabifyNodes = Ns.autoungrabify;
-    var zs = {
-        data: Oi.data({
+    Is.centre = Is.center, Is.autolockNodes = Is.autolock, Is.autoungrabifyNodes = Is.autoungrabify;
+    var As = {
+        data: Vi.data({
             field: "data",
             bindingEvent: "data",
             allowBinding: !0,
             allowSetting: !0,
             settingEvent: "data",
             settingTriggersEvent: !0,
             triggerFnName: "trigger",
             allowGetting: !0,
             updateStyle: !0
         }),
-        removeData: Oi.removeData({
+        removeData: Vi.removeData({
             field: "data",
             event: "data",
             triggerFnName: "trigger",
             triggerEvent: !0,
             updateStyle: !0
         }),
-        scratch: Oi.data({
+        scratch: Vi.data({
             field: "scratch",
             bindingEvent: "scratch",
             allowBinding: !0,
             allowSetting: !0,
             settingEvent: "scratch",
             settingTriggersEvent: !0,
             triggerFnName: "trigger",
             allowGetting: !0,
             updateStyle: !0
         }),
-        removeScratch: Oi.removeData({
+        removeScratch: Vi.removeData({
             field: "scratch",
             event: "scratch",
             triggerFnName: "trigger",
             triggerEvent: !0,
             updateStyle: !0
         })
     };
-    zs.attr = zs.data, zs.removeAttr = zs.removeData;
-    var Is = function(e) {
+    As.attr = As.data, As.removeAttr = As.removeData;
+    var Ls = function(e) {
             var t = this,
-                n = (e = I({}, e)).container;
-            n && !b(n) && b(n[0]) && (n = n[0]);
+                n = (e = A({}, e)).container;
+            n && !x(n) && x(n[0]) && (n = n[0]);
             var r = n ? n._cyreg : null;
             (r = r || {}) && r.cy && (r.cy.destroy(), r = {});
             var i = r.readies = r.readies || [];
             n && (n._cyreg = r), r.cy = t;
-            var a = void 0 !== s && void 0 !== n && !e.headless,
+            var a = void 0 !== l && void 0 !== n && !e.headless,
                 o = e;
-            o.layout = I({
+            o.layout = A({
                 name: a ? "grid" : "null"
-            }, o.layout), o.renderer = I({
+            }, o.layout), o.renderer = A({
                 name: a ? "canvas" : "null"
             }, o.renderer);
-            var l = function(e, t, n) {
+            var s = function(e, t, n) {
                     return void 0 !== t ? t : void 0 !== n ? n : e
                 },
                 u = this._private = {
                     container: n,
                     ready: !1,
                     options: o,
-                    elements: new Qo(this),
+                    elements: new es(this),
                     listeners: [],
-                    aniEles: new Qo(this),
+                    aniEles: new es(this),
                     data: o.data || {},
                     scratch: {},
                     layout: null,
                     renderer: null,
                     destroyed: !1,
                     notificationsEnabled: !0,
                     minZoom: 1e-50,
                     maxZoom: 1e50,
-                    zoomingEnabled: l(!0, o.zoomingEnabled),
-                    userZoomingEnabled: l(!0, o.userZoomingEnabled),
-                    panningEnabled: l(!0, o.panningEnabled),
-                    userPanningEnabled: l(!0, o.userPanningEnabled),
-                    boxSelectionEnabled: l(!0, o.boxSelectionEnabled),
-                    autolock: l(!1, o.autolock, o.autolockNodes),
-                    autoungrabify: l(!1, o.autoungrabify, o.autoungrabifyNodes),
-                    autounselectify: l(!1, o.autounselectify),
+                    zoomingEnabled: s(!0, o.zoomingEnabled),
+                    userZoomingEnabled: s(!0, o.userZoomingEnabled),
+                    panningEnabled: s(!0, o.panningEnabled),
+                    userPanningEnabled: s(!0, o.userPanningEnabled),
+                    boxSelectionEnabled: s(!0, o.boxSelectionEnabled),
+                    autolock: s(!1, o.autolock, o.autolockNodes),
+                    autoungrabify: s(!1, o.autoungrabify, o.autoungrabifyNodes),
+                    autounselectify: s(!1, o.autounselectify),
                     styleEnabled: void 0 === o.styleEnabled ? a : o.styleEnabled,
-                    zoom: m(o.zoom) ? o.zoom : 1,
+                    zoom: b(o.zoom) ? o.zoom : 1,
                     pan: {
-                        x: y(o.pan) && m(o.pan.x) ? o.pan.x : 0,
-                        y: y(o.pan) && m(o.pan.y) ? o.pan.y : 0
+                        x: m(o.pan) && b(o.pan.x) ? o.pan.x : 0,
+                        y: m(o.pan) && b(o.pan.y) ? o.pan.y : 0
                     },
                     animation: {
                         current: [],
                         queue: []
                     },
                     hasCompoundNodes: !1,
-                    multiClickDebounceTime: l(250, o.multiClickDebounceTime)
+                    multiClickDebounceTime: s(250, o.multiClickDebounceTime)
                 };
             this.createEmitter(), this.selectionType(o.selectionType), this.zoomRange({
                 min: o.minZoom,
                 max: o.maxZoom
             });
             u.styleEnabled && t.setStyle([]);
-            var c = I({}, o, o.renderer);
+            var c = A({}, o, o.renderer);
             t.initRenderer(c);
             ! function(e, t) {
-                if (e.some(P)) return pr.all(e).then(t);
+                if (e.some(D)) return gr.all(e).then(t);
                 t(e)
             }([o.style, o.elements], (function(e) {
                 var n = e[0],
                     a = e[1];
                 u.styleEnabled && t.style().append(n),
                     function(e, n, r) {
                         t.notifications(!1);
                         var i = t.mutableElements();
-                        i.length > 0 && i.remove(), null != e && (y(e) || v(e)) && t.add(e), t.one("layoutready", (function(e) {
+                        i.length > 0 && i.remove(), null != e && (m(e) || y(e)) && t.add(e), t.one("layoutready", (function(e) {
                             t.notifications(!0), t.emit(e), t.one("load", n), t.emitAndNotify("load")
                         })).one("layoutstop", (function() {
                             t.one("done", r), t.emit("done")
                         }));
-                        var a = I({}, t._private.options.layout);
+                        var a = A({}, t._private.options.layout);
                         a.eles = t.elements(), t.layout(a).run()
                     }(a, (function() {
-                        t.startAnimationLoop(), u.ready = !0, g(o.ready) && t.on("ready", o.ready);
+                        t.startAnimationLoop(), u.ready = !0, v(o.ready) && t.on("ready", o.ready);
                         for (var e = 0; e < i.length; e++) {
                             var n = i[e];
                             t.on("ready", n)
                         }
                         r && (r.readies = []), t.emit("ready")
                     }), o.done)
             }))
         },
-        Ls = Is.prototype;
-    I(Ls, {
+        Os = Ls.prototype;
+    A(Os, {
         instanceString: function() {
             return "core"
         },
         isReady: function() {
             return this._private.ready
         },
         destroyed: function() {
@@ -9940,70 +10042,70 @@
         removeFromPool: function(e) {
             return this._private.elements.unmerge(e), this
         },
         container: function() {
             return this._private.container || null
         },
         window: function() {
-            if (null == this._private.container) return s;
+            if (null == this._private.container) return l;
             var e = this._private.container.ownerDocument;
-            return void 0 === e || null == e ? s : e.defaultView || s
+            return void 0 === e || null == e ? l : e.defaultView || l
         },
         mount: function(e) {
             if (null != e) {
                 var t = this,
                     n = t._private,
                     r = n.options;
-                return !b(e) && b(e[0]) && (e = e[0]), t.stopAnimationLoop(), t.destroyRenderer(), n.container = e, n.styleEnabled = !0, t.invalidateSize(), t.initRenderer(I({}, r, r.renderer, {
+                return !x(e) && x(e[0]) && (e = e[0]), t.stopAnimationLoop(), t.destroyRenderer(), n.container = e, n.styleEnabled = !0, t.invalidateSize(), t.initRenderer(A({}, r, r.renderer, {
                     name: "null" === r.renderer.name ? "canvas" : r.renderer.name
                 })), t.startAnimationLoop(), t.style(r.style), t.emit("mount"), t
             }
         },
         unmount: function() {
             var e = this;
             return e.stopAnimationLoop(), e.destroyRenderer(), e.initRenderer({
                 name: "null"
             }), e.emit("unmount"), e
         },
         options: function() {
-            return Fe(this._private.options)
+            return je(this._private.options)
         },
         json: function(e) {
             var t = this,
                 n = t._private,
                 r = t.mutableElements();
-            if (y(e)) {
+            if (m(e)) {
                 if (t.startBatch(), e.elements) {
                     var i = {},
                         a = function(e, n) {
                             for (var r = [], a = [], o = 0; o < e.length; o++) {
                                 var s = e[o];
                                 if (s.data.id) {
                                     var l = "" + s.data.id,
                                         u = t.getElementById(l);
                                     i[l] = !0, 0 !== u.length ? a.push({
                                         ele: u,
                                         json: s
                                     }) : n ? (s.group = n, r.push(s)) : r.push(s)
-                                } else Ve("cy.json() cannot handle elements without an ID attribute")
+                                } else Fe("cy.json() cannot handle elements without an ID attribute")
                             }
                             t.add(r);
                             for (var c = 0; c < a.length; c++) {
                                 var d = a[c],
                                     h = d.ele,
                                     p = d.json;
                                 h.json(p)
                             }
                         };
-                    if (v(e.elements)) a(e.elements);
+                    if (y(e.elements)) a(e.elements);
                     else
                         for (var o = ["nodes", "edges"], s = 0; s < o.length; s++) {
                             var l = o[s],
                                 u = e.elements[l];
-                            v(u) && a(u, l)
+                            y(u) && a(u, l)
                         }
                     var c = t.collection();
                     r.filter((function(e) {
                         return !i[e.id()]
                     })).forEach((function(e) {
                         e.isParent() ? c.merge(e) : e.remove()
                     })), c.forEach((function(e) {
@@ -10025,22 +10127,22 @@
             }
             var f = {};
             !!e ? f.elements = this.elements().map((function(e) {
                 return e.json()
             })) : (f.elements = {}, r.forEach((function(e) {
                 var t = e.group();
                 f.elements[t] || (f.elements[t] = []), f.elements[t].push(e.json())
-            }))), this._private.styleEnabled && (f.style = t.style().json()), f.data = Fe(t.data());
+            }))), this._private.styleEnabled && (f.style = t.style().json()), f.data = je(t.data());
             var g = n.options;
-            return f.zoomingEnabled = n.zoomingEnabled, f.userZoomingEnabled = n.userZoomingEnabled, f.zoom = n.zoom, f.minZoom = n.minZoom, f.maxZoom = n.maxZoom, f.panningEnabled = n.panningEnabled, f.userPanningEnabled = n.userPanningEnabled, f.pan = Fe(n.pan), f.boxSelectionEnabled = n.boxSelectionEnabled, f.renderer = Fe(g.renderer), f.hideEdgesOnViewport = g.hideEdgesOnViewport, f.textureOnViewport = g.textureOnViewport, f.wheelSensitivity = g.wheelSensitivity, f.motionBlur = g.motionBlur, f.multiClickDebounceTime = g.multiClickDebounceTime, f
+            return f.zoomingEnabled = n.zoomingEnabled, f.userZoomingEnabled = n.userZoomingEnabled, f.zoom = n.zoom, f.minZoom = n.minZoom, f.maxZoom = n.maxZoom, f.panningEnabled = n.panningEnabled, f.userPanningEnabled = n.userPanningEnabled, f.pan = je(n.pan), f.boxSelectionEnabled = n.boxSelectionEnabled, f.renderer = je(g.renderer), f.hideEdgesOnViewport = g.hideEdgesOnViewport, f.textureOnViewport = g.textureOnViewport, f.wheelSensitivity = g.wheelSensitivity, f.motionBlur = g.motionBlur, f.multiClickDebounceTime = g.multiClickDebounceTime, f
         }
-    }), Ls.$id = Ls.getElementById, [es, ds, fs, gs, vs, ys, bs, xs, Bs, Ns, zs].forEach((function(e) {
-        I(Ls, e)
+    }), Os.$id = Os.getElementById, [ns, ps, vs, ys, ms, bs, ws, Es, zs, Is, As].forEach((function(e) {
+        A(Os, e)
     }));
-    var As = {
+    var Rs = {
             fit: !0,
             directed: !1,
             padding: 30,
             circle: !1,
             grid: !1,
             spacingFactor: 1.75,
             boundingBox: void 0,
@@ -10056,115 +10158,115 @@
             },
             ready: void 0,
             stop: void 0,
             transform: function(e, t) {
                 return t
             }
         },
-        Os = {
+        Vs = {
             maximal: !1,
             acyclic: !1
         },
-        Rs = function(e) {
+        Fs = function(e) {
             return e.scratch("breadthfirst")
         },
-        Vs = function(e, t) {
+        js = function(e, t) {
             return e.scratch("breadthfirst", t)
         };
 
-    function Fs(e) {
-        this.options = I({}, As, Os, e)
+    function qs(e) {
+        this.options = A({}, Rs, Vs, e)
     }
-    Fs.prototype.run = function() {
+    qs.prototype.run = function() {
         var e, t = this.options,
             n = t,
             r = t.cy,
             i = n.eles,
             a = i.nodes().filter((function(e) {
                 return !e.isParent()
             })),
             o = i,
             s = n.directed,
             l = n.acyclic || n.maximal || n.maximalAdjustments > 0,
-            u = Dt(n.boundingBox ? n.boundingBox : {
+            u = Tt(n.boundingBox ? n.boundingBox : {
                 x1: 0,
                 y1: 0,
                 w: r.width(),
                 h: r.height()
             });
-        if (x(n.roots)) e = n.roots;
-        else if (v(n.roots)) {
+        if (w(n.roots)) e = n.roots;
+        else if (y(n.roots)) {
             for (var c = [], d = 0; d < n.roots.length; d++) {
                 var h = n.roots[d],
                     p = r.getElementById(h);
                 c.push(p)
             }
             e = r.collection(c)
-        } else if (f(n.roots)) e = r.$(n.roots);
+        } else if (g(n.roots)) e = r.$(n.roots);
         else if (s) e = a.roots();
         else {
-            var g = i.components();
+            var f = i.components();
             e = r.collection();
-            for (var y = function(t) {
-                    var n = g[t],
+            for (var v = function(t) {
+                    var n = f[t],
                         r = n.maxDegree(!1),
                         i = n.filter((function(e) {
                             return e.degree(!1) === r
                         }));
                     e = e.add(i)
-                }, m = 0; m < g.length; m++) y(m)
+                }, m = 0; m < f.length; m++) v(m)
         }
         var b = [],
-            w = {},
+            x = {},
             E = function(e, t) {
                 null == b[t] && (b[t] = []);
                 var n = b[t].length;
-                b[t].push(e), Vs(e, {
+                b[t].push(e), js(e, {
                     index: n,
                     depth: t
                 })
             };
         o.bfs({
             roots: e,
             directed: n.directed,
             visit: function(e, t, n, r, i) {
                 var a = e[0],
                     o = a.id();
-                E(a, i), w[o] = !0
+                E(a, i), x[o] = !0
             }
         });
         for (var k = [], C = 0; C < a.length; C++) {
             var S = a[C];
-            w[S.id()] || k.push(S)
+            x[S.id()] || k.push(S)
         }
         var P = function(e) {
                 for (var t = b[e], n = 0; n < t.length; n++) {
                     var r = t[n];
-                    null != r ? Vs(r, {
+                    null != r ? js(r, {
                         depth: e,
                         index: n
                     }) : (t.splice(n, 1), n--)
                 }
             },
             D = function() {
                 for (var e = 0; e < b.length; e++) P(e)
             },
             T = function(e, t) {
-                for (var r = Rs(e), a = e.incomers().filter((function(e) {
+                for (var r = Fs(e), a = e.incomers().filter((function(e) {
                         return e.isNode() && i.has(e)
                     })), o = -1, s = e.id(), l = 0; l < a.length; l++) {
                     var u = a[l],
-                        c = Rs(u);
+                        c = Fs(u);
                     o = Math.max(o, c.depth)
                 }
                 if (r.depth <= o) {
                     if (!n.acyclic && t[s]) return null;
                     var d = o + 1;
                     return function(e, t) {
-                        var n = Rs(e),
+                        var n = Fs(e),
                             r = n.depth,
                             i = n.index;
                         b[r][i] = null, E(e, t)
                     }(e, d), t[s] = d, !0
                 }
                 return !1
             };
@@ -10174,89 +10276,89 @@
                 B = function(e) {
                     return _.push(e)
                 };
             for (a.forEach((function(e) {
                     return _.push(e)
                 })); _.length > 0;) {
                 var N = _.shift(),
-                    I = T(N, M);
-                if (I) N.outgoers().filter((function(e) {
+                    z = T(N, M);
+                if (z) N.outgoers().filter((function(e) {
                     return e.isNode() && i.has(e)
                 })).forEach(B);
-                else if (null === I) {
-                    Ve("Detected double maximal shift for node `" + N.id() + "`.  Bailing maximal adjustment due to cycle.  Use `options.maximal: true` only on DAGs.");
+                else if (null === z) {
+                    Fe("Detected double maximal shift for node `" + N.id() + "`.  Bailing maximal adjustment due to cycle.  Use `options.maximal: true` only on DAGs.");
                     break
                 }
             }
         }
         D();
-        var L = 0;
+        var A = 0;
         if (n.avoidOverlap)
-            for (var A = 0; A < a.length; A++) {
-                var O = a[A].layoutDimensions(n),
+            for (var L = 0; L < a.length; L++) {
+                var O = a[L].layoutDimensions(n),
                     R = O.w,
                     V = O.h;
-                L = Math.max(L, R, V)
+                A = Math.max(A, R, V)
             }
         var F = {},
             j = function(e) {
                 if (F[e.id()]) return F[e.id()];
-                for (var t = Rs(e).depth, n = e.neighborhood(), r = 0, i = 0, o = 0; o < n.length; o++) {
+                for (var t = Fs(e).depth, n = e.neighborhood(), r = 0, i = 0, o = 0; o < n.length; o++) {
                     var s = n[o];
                     if (!s.isEdge() && !s.isParent() && a.has(s)) {
-                        var l = Rs(s);
+                        var l = Fs(s);
                         if (null != l) {
                             var u = l.index,
                                 c = l.depth;
                             if (null != u && null != c) {
                                 var d = b[c].length;
                                 c < t && (r += u / d, i++)
                             }
                         }
                     }
                 }
                 return r /= i = Math.max(1, i), 0 === i && (r = 0), F[e.id()] = r, r
             },
             q = function(e, t) {
                 var n = j(e) - j(t);
-                return 0 === n ? z(e.id(), t.id()) : n
+                return 0 === n ? I(e.id(), t.id()) : n
             };
         void 0 !== n.depthSort && (q = n.depthSort);
         for (var Y = 0; Y < b.length; Y++) b[Y].sort(q), P(Y);
         for (var X = [], W = 0; W < k.length; W++) X.push(k[W]);
         b.unshift(X), D();
         for (var H = 0, K = 0; K < b.length; K++) H = Math.max(b[K].length, H);
         var G = u.x1 + u.w / 2,
             U = u.x1 + u.h / 2,
             Z = b.reduce((function(e, t) {
                 return Math.max(e, t.length)
             }), 0);
         return i.nodes().layoutPositions(this, n, (function(e) {
-            var t = Rs(e),
+            var t = Fs(e),
                 r = t.depth,
                 i = t.index,
                 a = b[r].length,
-                o = Math.max(u.w / ((n.grid ? Z : a) + 1), L),
-                s = Math.max(u.h / (b.length + 1), L),
+                o = Math.max(u.w / ((n.grid ? Z : a) + 1), A),
+                s = Math.max(u.h / (b.length + 1), A),
                 l = Math.min(u.w / 2 / b.length, u.h / 2 / b.length);
-            if (l = Math.max(l, L), n.circle) {
+            if (l = Math.max(l, A), n.circle) {
                 var c = l * r + l - (b.length > 0 && b[0].length <= 3 ? l / 2 : 0),
                     d = 2 * Math.PI / b[r].length * i;
                 return 0 === r && 1 === b[0].length && (c = 1), {
                     x: G + c * Math.cos(d),
                     y: U + c * Math.sin(d)
                 }
             }
             return {
                 x: G + (i + 1 - (a + 1) / 2) * o,
                 y: (r + 1) * s
             }
         })), this
     };
-    var js = {
+    var Ys = {
         fit: !0,
         padding: 30,
         boundingBox: void 0,
         avoidOverlap: !0,
         nodeDimensionsIncludeLabels: !1,
         spacingFactor: void 0,
         radius: void 0,
@@ -10273,54 +10375,54 @@
         ready: void 0,
         stop: void 0,
         transform: function(e, t) {
             return t
         }
     };
 
-    function qs(e) {
-        this.options = I({}, js, e)
+    function Xs(e) {
+        this.options = A({}, Ys, e)
     }
-    qs.prototype.run = function() {
+    Xs.prototype.run = function() {
         var e = this.options,
             t = e,
             n = e.cy,
             r = t.eles,
             i = void 0 !== t.counterclockwise ? !t.counterclockwise : t.clockwise,
             a = r.nodes().not(":parent");
         t.sort && (a = a.sort(t.sort));
-        for (var o, s = Dt(t.boundingBox ? t.boundingBox : {
+        for (var o, s = Tt(t.boundingBox ? t.boundingBox : {
                 x1: 0,
                 y1: 0,
                 w: n.width(),
                 h: n.height()
             }), l = s.x1 + s.w / 2, u = s.y1 + s.h / 2, c = (void 0 === t.sweep ? 2 * Math.PI - 2 * Math.PI / a.length : t.sweep) / Math.max(1, a.length - 1), d = 0, h = 0; h < a.length; h++) {
             var p = a[h].layoutDimensions(t),
                 f = p.w,
                 g = p.h;
             d = Math.max(d, f, g)
         }
-        if (o = m(t.radius) ? t.radius : a.length <= 1 ? 0 : Math.min(s.h, s.w) / 2 - d, a.length > 1 && t.avoidOverlap) {
+        if (o = b(t.radius) ? t.radius : a.length <= 1 ? 0 : Math.min(s.h, s.w) / 2 - d, a.length > 1 && t.avoidOverlap) {
             d *= 1.75;
             var v = Math.cos(c) - Math.cos(0),
                 y = Math.sin(c) - Math.sin(0),
-                b = Math.sqrt(d * d / (v * v + y * y));
-            o = Math.max(b, o)
+                m = Math.sqrt(d * d / (v * v + y * y));
+            o = Math.max(m, o)
         }
         return r.nodes().layoutPositions(this, t, (function(e, n) {
             var r = t.startAngle + n * c * (i ? 1 : -1),
                 a = o * Math.cos(r),
                 s = o * Math.sin(r);
             return {
                 x: l + a,
                 y: u + s
             }
         })), this
     };
-    var Ys, Xs = {
+    var Ws, Hs = {
         fit: !0,
         padding: 30,
         startAngle: 1.5 * Math.PI,
         sweep: void 0,
         clockwise: !0,
         equidistant: !1,
         minNodeSpacing: 10,
@@ -10345,19 +10447,19 @@
         ready: void 0,
         stop: void 0,
         transform: function(e, t) {
             return t
         }
     };
 
-    function Ws(e) {
-        this.options = I({}, Xs, e)
+    function Ks(e) {
+        this.options = A({}, Hs, e)
     }
-    Ws.prototype.run = function() {
-        for (var e = this.options, t = e, n = void 0 !== t.counterclockwise ? !t.counterclockwise : t.clockwise, r = e.cy, i = t.eles, a = i.nodes().not(":parent"), o = Dt(t.boundingBox ? t.boundingBox : {
+    Ks.prototype.run = function() {
+        for (var e = this.options, t = e, n = void 0 !== t.counterclockwise ? !t.counterclockwise : t.clockwise, r = e.cy, i = t.eles, a = i.nodes().not(":parent"), o = Tt(t.boundingBox ? t.boundingBox : {
                 x1: 0,
                 y1: 0,
                 w: r.width(),
                 h: r.height()
             }), s = o.x1 + o.w / 2, l = o.y1 + o.h / 2, u = [], c = 0, d = 0; d < a.length; d++) {
             var h, p = a[d];
             h = t.concentric(p), u.push({
@@ -10396,21 +10498,21 @@
                     B = Math.sqrt(w * w / (_ * _ + M * M));
                 C = Math.max(B, C)
             }
             P.r = C, C += w
         }
         if (t.equidistant) {
             for (var N = 0, z = 0, I = 0; I < y.length; I++) {
-                var L = y[I].r - z;
-                N = Math.max(N, L)
+                var A = y[I].r - z;
+                N = Math.max(N, A)
             }
             z = 0;
-            for (var A = 0; A < y.length; A++) {
-                var O = y[A];
-                0 === A && (z = O.r), O.r = z, z += N
+            for (var L = 0; L < y.length; L++) {
+                var O = y[L];
+                0 === L && (z = O.r), O.r = z, z += N
             }
         }
         for (var R = {}, V = 0; V < y.length; V++)
             for (var F = y[V], j = F.dTheta, q = F.r, Y = 0; Y < F.length; Y++) {
                 var X = F[Y],
                     W = t.startAngle + (n ? 1 : -1) * j * Y,
                     H = {
@@ -10420,15 +10522,15 @@
                 R[X.node.id()] = H
             }
         return i.nodes().layoutPositions(this, t, (function(e) {
             var t = e.id();
             return R[t]
         })), this
     };
-    var Hs = {
+    var Gs = {
         ready: function() {},
         stop: function() {},
         animate: !0,
         animationEasing: void 0,
         animationDuration: void 0,
         animateFilter: function(e, t) {
             return !0
@@ -10455,77 +10557,77 @@
         gravity: 1,
         numIter: 1e3,
         initialTemp: 1e3,
         coolingFactor: .99,
         minTemp: 1
     };
 
-    function Ks(e) {
-        this.options = I({}, Hs, e), this.options.layout = this;
+    function Us(e) {
+        this.options = A({}, Gs, e), this.options.layout = this;
         var t = this.options.eles.nodes(),
             n = this.options.eles.edges().filter((function(e) {
                 var n = e.source().data("id"),
                     r = e.target().data("id"),
                     i = t.some((function(e) {
                         return e.data("id") === n
                     })),
                     a = t.some((function(e) {
                         return e.data("id") === r
                     }));
                 return !i || !a
             }));
         this.options.eles = this.options.eles.not(n)
     }
-    Ks.prototype.run = function() {
+    Us.prototype.run = function() {
         var e = this.options,
             t = e.cy,
             n = this;
         n.stopped = !1, !0 !== e.animate && !1 !== e.animate || n.emit({
             type: "layoutstart",
             layout: n
-        }), Ys = !0 === e.debug;
-        var r = Gs(t, n, e);
-        Ys && (void 0)(r), e.randomize && $s(r);
-        var i = be(),
+        }), Ws = !0 === e.debug;
+        var r = Zs(t, n, e);
+        Ws && (void 0)(r), e.randomize && Js(r);
+        var i = xe(),
             a = function() {
-                Js(r, t, e), !0 === e.fit && t.fit(e.padding)
+                tl(r, t, e), !0 === e.fit && t.fit(e.padding)
             },
             o = function(t) {
-                return !(n.stopped || t >= e.numIter) && (el(r, e), r.temperature = r.temperature * e.coolingFactor, !(r.temperature < e.minTemp))
+                return !(n.stopped || t >= e.numIter) && (nl(r, e), r.temperature = r.temperature * e.coolingFactor, !(r.temperature < e.minTemp))
             },
             s = function() {
                 if (!0 === e.animate || !1 === e.animate) a(), n.one("layoutstop", e.stop), n.emit({
                     type: "layoutstop",
                     layout: n
                 });
                 else {
                     var t = e.eles.nodes(),
-                        i = Qs(r, e, t);
+                        i = el(r, e, t);
                     t.layoutPositions(n, e, i)
                 }
             },
             l = 0,
             u = !0;
         if (!0 === e.animate) {
             ! function t() {
                 for (var n = 0; u && n < e.refresh;) u = o(l), l++, n++;
-                u ? (be() - i >= e.animationThreshold && a(), me(t)) : (hl(r, e), s())
+                u ? (xe() - i >= e.animationThreshold && a(), be(t)) : (fl(r, e), s())
             }()
         } else {
             for (; u;) u = o(l), l++;
-            hl(r, e), s()
+            fl(r, e), s()
         }
         return this
-    }, Ks.prototype.stop = function() {
+    }, Us.prototype.stop = function() {
         return this.stopped = !0, this.thread && this.thread.stop(), this.emit("layoutstop"), this
-    }, Ks.prototype.destroy = function() {
+    }, Us.prototype.destroy = function() {
         return this.thread && this.thread.stop(), this
     };
-    var Gs = function(e, t, n) {
-            for (var r = n.eles.edges(), i = n.eles.nodes(), a = Dt(n.boundingBox ? n.boundingBox : {
+    var Zs = function(e, t, n) {
+            for (var r = n.eles.edges(), i = n.eles.nodes(), a = Tt(n.boundingBox ? n.boundingBox : {
                     x1: 0,
                     y1: 0,
                     w: e.width(),
                     h: e.height()
                 }), o = {
                     isCompound: e.hasCompoundNodes(),
                     layoutNodes: [],
@@ -10541,62 +10643,62 @@
                     boundingBox: a
                 }, s = n.eles.components(), l = {}, u = 0; u < s.length; u++)
                 for (var c = s[u], d = 0; d < c.length; d++) {
                     l[c[d].id()] = u
                 }
             for (u = 0; u < o.nodeSize; u++) {
                 var h = (m = i[u]).layoutDimensions(n);
-                (I = {}).isLocked = m.locked(), I.id = m.data("id"), I.parentId = m.data("parent"), I.cmptId = l[m.id()], I.children = [], I.positionX = m.position("x"), I.positionY = m.position("y"), I.offsetX = 0, I.offsetY = 0, I.height = h.w, I.width = h.h, I.maxX = I.positionX + I.width / 2, I.minX = I.positionX - I.width / 2, I.maxY = I.positionY + I.height / 2, I.minY = I.positionY - I.height / 2, I.padLeft = parseFloat(m.style("padding")), I.padRight = parseFloat(m.style("padding")), I.padTop = parseFloat(m.style("padding")), I.padBottom = parseFloat(m.style("padding")), I.nodeRepulsion = g(n.nodeRepulsion) ? n.nodeRepulsion(m) : n.nodeRepulsion, o.layoutNodes.push(I), o.idToIndex[I.id] = u
+                (I = {}).isLocked = m.locked(), I.id = m.data("id"), I.parentId = m.data("parent"), I.cmptId = l[m.id()], I.children = [], I.positionX = m.position("x"), I.positionY = m.position("y"), I.offsetX = 0, I.offsetY = 0, I.height = h.w, I.width = h.h, I.maxX = I.positionX + I.width / 2, I.minX = I.positionX - I.width / 2, I.maxY = I.positionY + I.height / 2, I.minY = I.positionY - I.height / 2, I.padLeft = parseFloat(m.style("padding")), I.padRight = parseFloat(m.style("padding")), I.padTop = parseFloat(m.style("padding")), I.padBottom = parseFloat(m.style("padding")), I.nodeRepulsion = v(n.nodeRepulsion) ? n.nodeRepulsion(m) : n.nodeRepulsion, o.layoutNodes.push(I), o.idToIndex[I.id] = u
             }
             var p = [],
                 f = 0,
-                v = -1,
+                g = -1,
                 y = [];
             for (u = 0; u < o.nodeSize; u++) {
                 var m, b = (m = o.layoutNodes[u]).parentId;
-                null != b ? o.layoutNodes[o.idToIndex[b]].children.push(m.id) : (p[++v] = m.id, y.push(m.id))
+                null != b ? o.layoutNodes[o.idToIndex[b]].children.push(m.id) : (p[++g] = m.id, y.push(m.id))
             }
-            for (o.graphSet.push(y); f <= v;) {
+            for (o.graphSet.push(y); f <= g;) {
                 var x = p[f++],
                     w = o.idToIndex[x],
                     E = o.layoutNodes[w].children;
                 if (E.length > 0) {
                     o.graphSet.push(E);
-                    for (u = 0; u < E.length; u++) p[++v] = E[u]
+                    for (u = 0; u < E.length; u++) p[++g] = E[u]
                 }
             }
             for (u = 0; u < o.graphSet.length; u++) {
                 var k = o.graphSet[u];
                 for (d = 0; d < k.length; d++) {
                     var C = o.idToIndex[k[d]];
                     o.indexToGraph[C] = u
                 }
             }
             for (u = 0; u < o.edgeSize; u++) {
                 var S = r[u],
                     P = {};
                 P.id = S.data("id"), P.sourceId = S.data("source"), P.targetId = S.data("target");
-                var D = g(n.idealEdgeLength) ? n.idealEdgeLength(S) : n.idealEdgeLength,
-                    T = g(n.edgeElasticity) ? n.edgeElasticity(S) : n.edgeElasticity,
+                var D = v(n.idealEdgeLength) ? n.idealEdgeLength(S) : n.idealEdgeLength,
+                    T = v(n.edgeElasticity) ? n.edgeElasticity(S) : n.edgeElasticity,
                     _ = o.idToIndex[P.sourceId],
                     M = o.idToIndex[P.targetId];
                 if (o.indexToGraph[_] != o.indexToGraph[M]) {
-                    for (var B = Us(P.sourceId, P.targetId, o), N = o.graphSet[B], z = 0, I = o.layoutNodes[_]; - 1 === N.indexOf(I.id);) I = o.layoutNodes[o.idToIndex[I.parentId]], z++;
+                    for (var B = $s(P.sourceId, P.targetId, o), N = o.graphSet[B], z = 0, I = o.layoutNodes[_]; - 1 === N.indexOf(I.id);) I = o.layoutNodes[o.idToIndex[I.parentId]], z++;
                     for (I = o.layoutNodes[M]; - 1 === N.indexOf(I.id);) I = o.layoutNodes[o.idToIndex[I.parentId]], z++;
                     D *= z * n.nestingFactor
                 }
                 P.idealLength = D, P.elasticity = T, o.layoutEdges.push(P)
             }
             return o
         },
-        Us = function(e, t, n) {
-            var r = Zs(e, t, 0, n);
+        $s = function(e, t, n) {
+            var r = Qs(e, t, 0, n);
             return 2 > r.count ? 0 : r.graph
         },
-        Zs = function e(t, n, r, i) {
+        Qs = function e(t, n, r, i) {
             var a = i.graphSet[r];
             if (-1 < a.indexOf(t) && -1 < a.indexOf(n)) return {
                 count: 2,
                 graph: r
             };
             for (var o = 0, s = 0; s < a.length; s++) {
                 var l = a[s],
@@ -10611,21 +10713,21 @@
                 }
             }
             return {
                 count: o,
                 graph: r
             }
         },
-        $s = function(e, t) {
+        Js = function(e, t) {
             for (var n = e.clientWidth, r = e.clientHeight, i = 0; i < e.nodeSize; i++) {
                 var a = e.layoutNodes[i];
                 0 !== a.children.length || a.isLocked || (a.positionX = Math.random() * n, a.positionY = Math.random() * r)
             }
         },
-        Qs = function(e, t, n) {
+        el = function(e, t, n) {
             var r = e.boundingBox,
                 i = {
                     x1: 1 / 0,
                     x2: -1 / 0,
                     y1: 1 / 0,
                     y2: -1 / 0
                 };
@@ -10645,98 +10747,98 @@
                     }
                     return {
                         x: o.positionX,
                         y: o.positionY
                     }
                 }
         },
-        Js = function(e, t, n) {
+        tl = function(e, t, n) {
             var r = n.layout,
                 i = n.eles.nodes(),
-                a = Qs(e, n, i);
+                a = el(e, n, i);
             i.positions(a), !0 !== e.ready && (e.ready = !0, r.one("layoutready", n.ready), r.emit({
                 type: "layoutready",
                 layout: this
             }))
         },
-        el = function(e, t, n) {
-            tl(e, t), ol(e), sl(e, t), ll(e), ul(e)
+        nl = function(e, t, n) {
+            rl(e, t), ll(e), ul(e, t), cl(e), dl(e)
         },
-        tl = function(e, t) {
+        rl = function(e, t) {
             for (var n = 0; n < e.graphSet.length; n++)
                 for (var r = e.graphSet[n], i = r.length, a = 0; a < i; a++)
                     for (var o = e.layoutNodes[e.idToIndex[r[a]]], s = a + 1; s < i; s++) {
                         var l = e.layoutNodes[e.idToIndex[r[s]]];
-                        rl(o, l, e, t)
+                        al(o, l, e, t)
                     }
         },
-        nl = function(e) {
+        il = function(e) {
             return -e + 2 * e * Math.random()
         },
-        rl = function(e, t, n, r) {
+        al = function(e, t, n, r) {
             if (e.cmptId === t.cmptId || n.isCompound) {
                 var i = t.positionX - e.positionX,
                     a = t.positionY - e.positionY;
-                0 === i && 0 === a && (i = nl(1), a = nl(1));
-                var o = il(e, t, i, a);
+                0 === i && 0 === a && (i = il(1), a = il(1));
+                var o = ol(e, t, i, a);
                 if (o > 0) var s = (u = r.nodeOverlap * o) * i / (g = Math.sqrt(i * i + a * a)),
                     l = u * a / g;
                 else {
-                    var u, c = al(e, i, a),
-                        d = al(t, -1 * i, -1 * a),
+                    var u, c = sl(e, i, a),
+                        d = sl(t, -1 * i, -1 * a),
                         h = d.x - c.x,
                         p = d.y - c.y,
                         f = h * h + p * p,
                         g = Math.sqrt(f);
                     s = (u = (e.nodeRepulsion + t.nodeRepulsion) / f) * h / g, l = u * p / g
                 }
                 e.isLocked || (e.offsetX -= s, e.offsetY -= l), t.isLocked || (t.offsetX += s, t.offsetY += l)
             }
         },
-        il = function(e, t, n, r) {
+        ol = function(e, t, n, r) {
             if (n > 0) var i = e.maxX - t.minX;
             else i = t.maxX - e.minX;
             if (r > 0) var a = e.maxY - t.minY;
             else a = t.maxY - e.minY;
             return i >= 0 && a >= 0 ? Math.sqrt(i * i + a * a) : 0
         },
-        al = function(e, t, n) {
+        sl = function(e, t, n) {
             var r = e.positionX,
                 i = e.positionY,
                 a = e.height || 1,
                 o = e.width || 1,
                 s = n / t,
                 l = a / o,
                 u = {};
             return 0 === t && 0 < n || 0 === t && 0 > n ? (u.x = r, u.y = i + a / 2, u) : 0 < t && -1 * l <= s && s <= l ? (u.x = r + o / 2, u.y = i + o * n / 2 / t, u) : 0 > t && -1 * l <= s && s <= l ? (u.x = r - o / 2, u.y = i - o * n / 2 / t, u) : 0 < n && (s <= -1 * l || s >= l) ? (u.x = r + a * t / 2 / n, u.y = i + a / 2, u) : 0 > n && (s <= -1 * l || s >= l) ? (u.x = r - a * t / 2 / n, u.y = i - a / 2, u) : u
         },
-        ol = function(e, t) {
+        ll = function(e, t) {
             for (var n = 0; n < e.edgeSize; n++) {
                 var r = e.layoutEdges[n],
                     i = e.idToIndex[r.sourceId],
                     a = e.layoutNodes[i],
                     o = e.idToIndex[r.targetId],
                     s = e.layoutNodes[o],
                     l = s.positionX - a.positionX,
                     u = s.positionY - a.positionY;
                 if (0 !== l || 0 !== u) {
-                    var c = al(a, l, u),
-                        d = al(s, -1 * l, -1 * u),
+                    var c = sl(a, l, u),
+                        d = sl(s, -1 * l, -1 * u),
                         h = d.x - c.x,
                         p = d.y - c.y,
                         f = Math.sqrt(h * h + p * p),
                         g = Math.pow(r.idealLength - f, 2) / r.elasticity;
                     if (0 !== f) var v = g * h / f,
                         y = g * p / f;
                     else v = 0, y = 0;
                     a.isLocked || (a.offsetX += v, a.offsetY += y), s.isLocked || (s.offsetX -= v, s.offsetY -= y)
                 }
             }
         },
-        sl = function(e, t) {
+        ul = function(e, t) {
             if (0 !== t.gravity)
                 for (var n = 0; n < e.graphSet.length; n++) {
                     var r = e.graphSet[n],
                         i = r.length;
                     if (0 === n) var a = e.clientHeight / 2,
                         o = e.clientWidth / 2;
                     else {
@@ -10755,15 +10857,15 @@
                                     g = t.gravity * h / p;
                                 c.offsetX += f, c.offsetY += g
                             }
                         }
                     }
                 }
         },
-        ll = function(e, t) {
+        cl = function(e, t) {
             var n = [],
                 r = 0,
                 i = -1;
             for (n.push.apply(n, e.graphSet[0]), i += e.graphSet[0].length; r <= i;) {
                 var a = n[r++],
                     o = e.idToIndex[a],
                     s = e.layoutNodes[o],
@@ -10773,50 +10875,50 @@
                         var h = e.layoutNodes[e.idToIndex[l[d]]];
                         h.offsetX += u, h.offsetY += c, n[++i] = l[d]
                     }
                     s.offsetX = 0, s.offsetY = 0
                 }
             }
         },
-        ul = function(e, t) {
+        dl = function(e, t) {
             for (var n = 0; n < e.nodeSize; n++) {
                 0 < (i = e.layoutNodes[n]).children.length && (i.maxX = void 0, i.minX = void 0, i.maxY = void 0, i.minY = void 0)
             }
             for (n = 0; n < e.nodeSize; n++) {
                 if (!(0 < (i = e.layoutNodes[n]).children.length || i.isLocked)) {
-                    var r = cl(i.offsetX, i.offsetY, e.temperature);
-                    i.positionX += r.x, i.positionY += r.y, i.offsetX = 0, i.offsetY = 0, i.minX = i.positionX - i.width, i.maxX = i.positionX + i.width, i.minY = i.positionY - i.height, i.maxY = i.positionY + i.height, dl(i, e)
+                    var r = hl(i.offsetX, i.offsetY, e.temperature);
+                    i.positionX += r.x, i.positionY += r.y, i.offsetX = 0, i.offsetY = 0, i.minX = i.positionX - i.width, i.maxX = i.positionX + i.width, i.minY = i.positionY - i.height, i.maxY = i.positionY + i.height, pl(i, e)
                 }
             }
             for (n = 0; n < e.nodeSize; n++) {
                 var i;
                 0 < (i = e.layoutNodes[n]).children.length && !i.isLocked && (i.positionX = (i.maxX + i.minX) / 2, i.positionY = (i.maxY + i.minY) / 2, i.width = i.maxX - i.minX, i.height = i.maxY - i.minY)
             }
         },
-        cl = function(e, t, n) {
+        hl = function(e, t, n) {
             var r = Math.sqrt(e * e + t * t);
             if (r > n) var i = {
                 x: n * e / r,
                 y: n * t / r
             };
             else i = {
                 x: e,
                 y: t
             };
             return i
         },
-        dl = function e(t, n) {
+        pl = function e(t, n) {
             var r = t.parentId;
             if (null != r) {
                 var i = n.layoutNodes[n.idToIndex[r]],
                     a = !1;
                 return (null == i.maxX || t.maxX + i.padRight > i.maxX) && (i.maxX = t.maxX + i.padRight, a = !0), (null == i.minX || t.minX - i.padLeft < i.minX) && (i.minX = t.minX - i.padLeft, a = !0), (null == i.maxY || t.maxY + i.padBottom > i.maxY) && (i.maxY = t.maxY + i.padBottom, a = !0), (null == i.minY || t.minY - i.padTop < i.minY) && (i.minY = t.minY - i.padTop, a = !0), a ? e(i, n) : void 0
             }
         },
-        hl = function(e, t) {
+        fl = function(e, t) {
             for (var n = e.layoutNodes, r = [], i = 0; i < n.length; i++) {
                 var a = n[i],
                     o = a.cmptId;
                 (r[o] = r[o] || []).push(a)
             }
             var s = 0;
             for (i = 0; i < r.length; i++) {
@@ -10843,15 +10945,15 @@
                     for (l = 0; l < g.length; l++) {
                         (u = g[l]).isLocked || (u.positionX += c - g.x1, u.positionY += d - g.y1)
                     }
                     c += g.w + t.componentSpacing, h += g.w + t.componentSpacing, p = Math.max(p, g.h), h > f && (d += p + t.componentSpacing, c = 0, h = 0, p = 0)
                 }
             }
         },
-        pl = {
+        gl = {
             fit: !0,
             padding: 30,
             boundingBox: void 0,
             avoidOverlap: !0,
             avoidOverlapPadding: 10,
             nodeDimensionsIncludeLabels: !1,
             spacingFactor: void 0,
@@ -10869,25 +10971,25 @@
             ready: void 0,
             stop: void 0,
             transform: function(e, t) {
                 return t
             }
         };
 
-    function fl(e) {
-        this.options = I({}, pl, e)
+    function vl(e) {
+        this.options = A({}, gl, e)
     }
-    fl.prototype.run = function() {
+    vl.prototype.run = function() {
         var e = this.options,
             t = e,
             n = e.cy,
             r = t.eles,
             i = r.nodes().not(":parent");
         t.sort && (i = i.sort(t.sort));
-        var a = Dt(t.boundingBox ? t.boundingBox : {
+        var a = Tt(t.boundingBox ? t.boundingBox : {
             x1: 0,
             y1: 0,
             w: n.width(),
             h: n.height()
         });
         if (0 === a.h || 0 === a.w) r.nodes().layoutPositions(this, t, (function(e) {
             return {
@@ -10939,26 +11041,26 @@
             for (var D = {}, T = function(e, t) {
                     return !!D["c-" + e + "-" + t]
                 }, _ = function(e, t) {
                     D["c-" + e + "-" + t] = !0
                 }, M = 0, B = 0, N = function() {
                     ++B >= u && (B = 0, M++)
                 }, z = {}, I = 0; I < i.length; I++) {
-                var L = i[I],
-                    A = t.position(L);
-                if (A && (void 0 !== A.row || void 0 !== A.col)) {
+                var A = i[I],
+                    L = t.position(A);
+                if (L && (void 0 !== L.row || void 0 !== L.col)) {
                     var O = {
-                        row: A.row,
-                        col: A.col
+                        row: L.row,
+                        col: L.col
                     };
                     if (void 0 === O.col)
                         for (O.col = 0; T(O.row, O.col);) O.col++;
                     else if (void 0 === O.row)
                         for (O.row = 0; T(O.row, O.col);) O.row++;
-                    z[L.id()] = O, _(O.row, O.col)
+                    z[A.id()] = O, _(O.row, O.col)
                 }
             }
             i.layoutPositions(this, t, (function(e, t) {
                 var n, r;
                 if (e.locked() || e.isParent()) return !1;
                 var i = z[e.id()];
                 if (i) n = i.col * m + m / 2 + a.x1, r = i.row * b + b / 2 + a.y1;
@@ -10970,35 +11072,35 @@
                     x: n,
                     y: r
                 }
             }))
         }
         return this
     };
-    var gl = {
+    var yl = {
         ready: function() {},
         stop: function() {}
     };
 
-    function vl(e) {
-        this.options = I({}, gl, e)
+    function ml(e) {
+        this.options = A({}, yl, e)
     }
-    vl.prototype.run = function() {
+    ml.prototype.run = function() {
         var e = this.options,
             t = e.eles;
         return e.cy, this.emit("layoutstart"), t.nodes().positions((function() {
             return {
                 x: 0,
                 y: 0
             }
         })), this.one("layoutready", e.ready), this.emit("layoutready"), this.one("layoutstop", e.stop), this.emit("layoutstop"), this
-    }, vl.prototype.stop = function() {
+    }, ml.prototype.stop = function() {
         return this
     };
-    var yl = {
+    var bl = {
         positions: void 0,
         zoom: void 0,
         pan: void 0,
         fit: !0,
         padding: 30,
         spacingFactor: void 0,
         animate: !1,
@@ -11010,21 +11112,21 @@
         ready: void 0,
         stop: void 0,
         transform: function(e, t) {
             return t
         }
     };
 
-    function ml(e) {
-        this.options = I({}, yl, e)
+    function xl(e) {
+        this.options = A({}, bl, e)
     }
-    ml.prototype.run = function() {
+    xl.prototype.run = function() {
         var e = this.options,
             t = e.eles.nodes(),
-            n = g(e.positions);
+            n = v(e.positions);
         return t.layoutPositions(this, e, (function(t, r) {
             var i = function(t) {
                 if (null == e.positions) return function(e) {
                     return {
                         x: e.x,
                         y: e.y
                     }
@@ -11032,15 +11134,15 @@
                 if (n) return e.positions(t);
                 var r = e.positions[t._private.data.id];
                 return null == r ? null : r
             }(t);
             return !t.locked() && null != i && i
         })), this
     };
-    var bl = {
+    var wl = {
         fit: !0,
         padding: 30,
         boundingBox: void 0,
         animate: !1,
         animationDuration: 500,
         animationEasing: void 0,
         animateFilter: function(e, t) {
@@ -11049,80 +11151,80 @@
         ready: void 0,
         stop: void 0,
         transform: function(e, t) {
             return t
         }
     };
 
-    function xl(e) {
-        this.options = I({}, bl, e)
+    function El(e) {
+        this.options = A({}, wl, e)
     }
-    xl.prototype.run = function() {
+    El.prototype.run = function() {
         var e = this.options,
             t = e.cy,
             n = e.eles,
-            r = Dt(e.boundingBox ? e.boundingBox : {
+            r = Tt(e.boundingBox ? e.boundingBox : {
                 x1: 0,
                 y1: 0,
                 w: t.width(),
                 h: t.height()
             });
         return n.nodes().layoutPositions(this, e, (function(e, t) {
             return {
                 x: r.x1 + Math.round(Math.random() * r.w),
                 y: r.y1 + Math.round(Math.random() * r.h)
             }
         })), this
     };
-    var wl = [{
+    var kl = [{
         name: "breadthfirst",
-        impl: Fs
+        impl: qs
     }, {
         name: "circle",
-        impl: qs
+        impl: Xs
     }, {
         name: "concentric",
-        impl: Ws
+        impl: Ks
     }, {
         name: "cose",
-        impl: Ks
+        impl: Us
     }, {
         name: "grid",
-        impl: fl
+        impl: vl
     }, {
         name: "null",
-        impl: vl
+        impl: ml
     }, {
         name: "preset",
-        impl: ml
+        impl: xl
     }, {
         name: "random",
-        impl: xl
+        impl: El
     }];
 
-    function El(e) {
+    function Cl(e) {
         this.options = e, this.notifications = 0
     }
-    var kl = function() {},
-        Cl = function() {
+    var Sl = function() {},
+        Pl = function() {
             throw new Error("A headless instance can not render images")
         };
-    El.prototype = {
-        recalculateRenderedStyle: kl,
+    Cl.prototype = {
+        recalculateRenderedStyle: Sl,
         notify: function() {
             this.notifications++
         },
-        init: kl,
+        init: Sl,
         isHeadless: function() {
             return !0
         },
-        png: Cl,
-        jpg: Cl
+        png: Pl,
+        jpg: Pl
     };
-    var Sl = {
+    var Dl = {
             arrowShapeWidth: .3,
             registerArrowShapes: function() {
                 var e = this.arrowShapes = {},
                     t = this,
                     n = function(e, t, n, r, i, a, o) {
                         var s = i.x - n / 2 - o,
                             l = i.x + n / 2 + o,
@@ -11153,36 +11255,36 @@
                         }
                         return t
                     },
                     o = function(e) {
                         return e.pstyle("width").pfValue * e.pstyle("arrow-scale").pfValue * 2
                     },
                     s = function(r, s) {
-                        f(s) && (s = e[s]), e[r] = I({
+                        g(s) && (s = e[s]), e[r] = A({
                             name: r,
                             points: [-.15, -.3, .15, -.3, .15, .3, -.15, .3],
                             collide: function(e, t, n, r, o, s) {
                                 var l = a(i(this.points, n + 2 * s, r, o));
-                                return jt(e, t, l)
+                                return qt(e, t, l)
                             },
                             roughCollide: n,
                             draw: function(e, n, r, a) {
                                 var o = i(this.points, n, r, a);
                                 t.arrowShapeImpl("polygon")(e, o)
                             },
                             spacing: function(e) {
                                 return 0
                             },
                             gap: o
                         }, s)
                     };
                 s("none", {
-                    collide: Ie,
-                    roughCollide: Ie,
-                    draw: Ae,
+                    collide: Ae,
+                    roughCollide: Ae,
+                    draw: Oe,
                     spacing: Le,
                     gap: Le
                 }), s("triangle", {
                     points: [-.15, -.3, 0, 0, .15, -.3]
                 }), s("arrow", "triangle"), s("triangle-backcurve", {
                     points: e.triangle.points,
                     controlPoint: [0, -.15],
@@ -11198,29 +11300,29 @@
                     }
                 }), s("triangle-tee", {
                     points: [0, 0, .15, -.3, -.15, -.3, 0, 0],
                     pointsTee: [-.15, -.4, -.15, -.5, .15, -.5, .15, -.4],
                     collide: function(e, t, n, r, o, s, l) {
                         var u = a(i(this.points, n + 2 * l, r, o)),
                             c = a(i(this.pointsTee, n + 2 * l, r, o));
-                        return jt(e, t, u) || jt(e, t, c)
+                        return qt(e, t, u) || qt(e, t, c)
                     },
                     draw: function(e, n, r, a, o) {
                         var s = i(this.points, n, r, a),
                             l = i(this.pointsTee, n, r, a);
                         t.arrowShapeImpl(this.name)(e, s, l)
                     }
                 }), s("circle-triangle", {
                     radius: .15,
                     pointsTr: [0, -.15, .15, -.45, -.15, -.45, 0, -.15],
                     collide: function(e, t, n, r, o, s, l) {
                         var u = o,
                             c = Math.pow(u.x - e, 2) + Math.pow(u.y - t, 2) <= Math.pow((n + 2 * l) * this.radius, 2),
                             d = a(i(this.points, n + 2 * l, r, o));
-                        return jt(e, t, d) || c
+                        return qt(e, t, d) || c
                     },
                     draw: function(e, n, r, a, o) {
                         var s = i(this.pointsTr, n, r, a);
                         t.arrowShapeImpl(this.name)(e, s, a.x, a.y, this.radius * n)
                     },
                     spacing: function(e) {
                         return t.getArrowWidth(e.pstyle("width").pfValue, e.pstyle("arrow-scale").value) * this.radius
@@ -11232,15 +11334,15 @@
                         var n = this.baseCrossLinePts.slice(),
                             r = t / e;
                         return n[3] = n[3] - r, n[5] = n[5] - r, n
                     },
                     collide: function(e, t, n, r, o, s, l) {
                         var u = a(i(this.points, n + 2 * l, r, o)),
                             c = a(i(this.crossLinePts(n, s), n + 2 * l, r, o));
-                        return jt(e, t, u) || jt(e, t, c)
+                        return qt(e, t, u) || qt(e, t, c)
                     },
                     draw: function(e, n, r, a, o) {
                         var s = i(this.points, n, r, a),
                             l = i(this.crossLinePts(n, o), n, r, a);
                         t.arrowShapeImpl(this.name)(e, s, l)
                     }
                 }), s("vee", {
@@ -11279,15 +11381,15 @@
                     points: [0, 0, -.15, -.15, -.1, -.2, 0, -.1, .1, -.2, .15, -.15],
                     gap: function(e) {
                         return .95 * e.pstyle("width").pfValue * e.pstyle("arrow-scale").value
                     }
                 })
             }
         },
-        Pl = {
+        Tl = {
             projectIntoViewport: function(e, t) {
                 var n = this.cy,
                     r = this.findContainerClientCoords(),
                     i = r[0],
                     a = r[1],
                     o = r[4],
                     s = n.pan(),
@@ -11356,34 +11458,36 @@
                 }
 
                 function y(n) {
                     var r = n.outerWidth() + 2 * p,
                         i = n.outerHeight() + 2 * p,
                         a = r / 2,
                         l = i / 2,
-                        u = n.position();
-                    if (u.x - a <= e && e <= u.x + a && u.y - l <= t && t <= u.y + l && s.nodeShapes[o.getNodeShape(n)].checkPoint(e, t, 0, r, i, u.x, u.y)) return v(n, 0), !0
+                        u = n.position(),
+                        c = "auto" === n.pstyle("corner-radius").value ? "auto" : n.pstyle("corner-radius").pfValue,
+                        d = n._private.rscratch;
+                    if (u.x - a <= e && e <= u.x + a && u.y - l <= t && t <= u.y + l && s.nodeShapes[o.getNodeShape(n)].checkPoint(e, t, 0, r, i, u.x, u.y, c, d)) return v(n, 0), !0
                 }
 
                 function m(n) {
                     var r, i = n._private,
                         a = i.rscratch,
                         l = n.pstyle("width").pfValue,
                         c = n.pstyle("arrow-scale").value,
                         p = l / 2 + h,
                         f = p * p,
                         g = 2 * p,
                         m = i.source,
                         b = i.target;
                     if ("segments" === a.edgeType || "straight" === a.edgeType || "haystack" === a.edgeType) {
                         for (var x = a.allpts, w = 0; w + 3 < x.length; w += 2)
-                            if (Ot(e, t, x[w], x[w + 1], x[w + 2], x[w + 3], g) && f > (r = Ft(e, t, x[w], x[w + 1], x[w + 2], x[w + 3]))) return v(n, r), !0
+                            if (Rt(e, t, x[w], x[w + 1], x[w + 2], x[w + 3], g) && f > (r = jt(e, t, x[w], x[w + 1], x[w + 2], x[w + 3]))) return v(n, r), !0
                     } else if ("bezier" === a.edgeType || "multibezier" === a.edgeType || "self" === a.edgeType || "compound" === a.edgeType)
                         for (x = a.allpts, w = 0; w + 5 < a.allpts.length; w += 4)
-                            if (Rt(e, t, x[w], x[w + 1], x[w + 2], x[w + 3], x[w + 4], x[w + 5], g) && f > (r = Vt(e, t, x[w], x[w + 1], x[w + 2], x[w + 3], x[w + 4], x[w + 5]))) return v(n, r), !0;
+                            if (Vt(e, t, x[w], x[w + 1], x[w + 2], x[w + 3], x[w + 4], x[w + 5], g) && f > (r = Ft(e, t, x[w], x[w + 1], x[w + 2], x[w + 3], x[w + 4], x[w + 5]))) return v(n, r), !0;
                     m = m || i.source, b = b || i.target;
                     var E = o.getArrowWidth(l, c),
                         k = [{
                             name: "source",
                             x: a.arrowStartX,
                             y: a.arrowStartY,
                             angle: a.srcArrowAngle
@@ -11415,15 +11519,15 @@
                                 y: C.y
                             }, P, h)) return v(n), !0
                     }
                     d && u.length > 0 && (y(m), y(b))
                 }
 
                 function b(e, t, n) {
-                    return Ke(e, t, n)
+                    return Ge(e, t, n)
                 }
 
                 function x(n, r) {
                     var i, a = n._private,
                         o = f;
                     i = r ? r + "-" : "", n.boundingBox();
                     var s = a.labelBounds[r || "main"],
@@ -11448,127 +11552,173 @@
                                     }
                                 },
                                 C = k(g, m),
                                 S = k(g, x),
                                 P = k(y, m),
                                 D = k(y, x),
                                 T = [C.x + h, C.y + p, P.x + h, P.y + p, D.x + h, D.y + p, S.x + h, S.y + p];
-                            if (jt(e, t, T)) return v(n), !0
-                        } else if (It(s, e, t)) return v(n), !0
+                            if (qt(e, t, T)) return v(n), !0
+                        } else if (At(s, e, t)) return v(n), !0
                     }
                 }
                 n && (l = l.interactive);
                 for (var w = l.length - 1; w >= 0; w--) {
                     var E = l[w];
                     E.isNode() ? y(E) || x(E) : m(E) || x(E) || x(E, "source") || x(E, "target")
                 }
                 return u
             },
             getAllInBox: function(e, t, n, r) {
-                for (var i, a, o = this.getCachedZSortedEles().interactive, s = [], l = Math.min(e, n), u = Math.max(e, n), c = Math.min(t, r), d = Math.max(t, r), h = Dt({
+                for (var i, a, o = this.getCachedZSortedEles().interactive, s = [], l = Math.min(e, n), u = Math.max(e, n), c = Math.min(t, r), d = Math.max(t, r), h = Tt({
                         x1: e = l,
                         y1: t = c,
                         x2: n = u,
                         y2: r = d
                     }), p = 0; p < o.length; p++) {
                     var f = o[p];
                     if (f.isNode()) {
                         var g = f,
                             v = g.boundingBox({
                                 includeNodes: !0,
                                 includeEdges: !1,
                                 includeLabels: !1
                             });
-                        zt(h, v) && !Lt(v, h) && s.push(g)
+                        It(h, v) && !Lt(v, h) && s.push(g)
                     } else {
                         var y = f,
                             m = y._private,
                             b = m.rscratch;
-                        if (null != b.startX && null != b.startY && !It(h, b.startX, b.startY)) continue;
-                        if (null != b.endX && null != b.endY && !It(h, b.endX, b.endY)) continue;
+                        if (null != b.startX && null != b.startY && !At(h, b.startX, b.startY)) continue;
+                        if (null != b.endX && null != b.endY && !At(h, b.endX, b.endY)) continue;
                         if ("bezier" === b.edgeType || "multibezier" === b.edgeType || "self" === b.edgeType || "compound" === b.edgeType || "segments" === b.edgeType || "haystack" === b.edgeType) {
                             for (var x = m.rstyle.bezierPts || m.rstyle.linePts || m.rstyle.haystackPts, w = !0, E = 0; E < x.length; E++)
-                                if (i = h, a = x[E], !It(i, a.x, a.y)) {
+                                if (i = h, a = x[E], !At(i, a.x, a.y)) {
                                     w = !1;
                                     break
                                 } w && s.push(y)
                         } else "haystack" !== b.edgeType && "straight" !== b.edgeType || s.push(y)
                     }
                 }
                 return s
             }
         },
-        Dl = {
+        _l = {
             calculateArrowAngles: function(e) {
                 var t, n, r, i, a, o, s = e._private.rscratch,
                     l = "haystack" === s.edgeType,
                     u = "bezier" === s.edgeType,
                     c = "multibezier" === s.edgeType,
                     d = "segments" === s.edgeType,
                     h = "compound" === s.edgeType,
                     p = "self" === s.edgeType;
                 if (l ? (r = s.haystackPts[0], i = s.haystackPts[1], a = s.haystackPts[2], o = s.haystackPts[3]) : (r = s.arrowStartX, i = s.arrowStartY, a = s.arrowEndX, o = s.arrowEndY), g = s.midX, v = s.midY, d) t = r - s.segpts[0], n = i - s.segpts[1];
                 else if (c || h || p || u) {
                     var f = s.allpts;
-                    t = r - Ct(f[0], f[2], f[4], .1), n = i - Ct(f[1], f[3], f[5], .1)
+                    t = r - St(f[0], f[2], f[4], .1), n = i - St(f[1], f[3], f[5], .1)
                 } else t = r - g, n = i - v;
-                s.srcArrowAngle = mt(t, n);
+                s.srcArrowAngle = bt(t, n);
                 var g = s.midX,
                     v = s.midY;
                 if (l && (g = (r + a) / 2, v = (i + o) / 2), t = a - r, n = o - i, d)
                     if ((f = s.allpts).length / 2 % 2 == 0) {
-                        var y = (m = f.length / 2) - 2;
-                        t = f[m] - f[y], n = f[m + 1] - f[y + 1]
-                    } else {
-                        y = (m = f.length / 2 - 1) - 2;
-                        var m, b = m + 2;
-                        t = f[m] - f[y], n = f[m + 1] - f[y + 1]
-                    }
-                else if (c || h || p) {
-                    var x, w, E, k, f = s.allpts;
+                        var y = (S = f.length / 2) - 2;
+                        t = f[S] - f[y], n = f[S + 1] - f[y + 1]
+                    } else if (s.isRound) t = s.midVector[1], n = -s.midVector[0];
+                else {
+                    y = (S = f.length / 2 - 1) - 2;
+                    t = f[S] - f[y], n = f[S + 1] - f[y + 1]
+                } else if (c || h || p) {
+                    var m, b, x, w, f = s.allpts;
                     if (s.ctrlpts.length / 2 % 2 == 0) {
-                        var C = (S = (P = f.length / 2 - 1) + 2) + 2;
-                        x = Ct(f[P], f[S], f[C], 0), w = Ct(f[P + 1], f[S + 1], f[C + 1], 0), E = Ct(f[P], f[S], f[C], 1e-4), k = Ct(f[P + 1], f[S + 1], f[C + 1], 1e-4)
+                        var E = (k = (C = f.length / 2 - 1) + 2) + 2;
+                        m = St(f[C], f[k], f[E], 0), b = St(f[C + 1], f[k + 1], f[E + 1], 0), x = St(f[C], f[k], f[E], 1e-4), w = St(f[C + 1], f[k + 1], f[E + 1], 1e-4)
                     } else {
-                        var S, P;
-                        C = (S = f.length / 2 - 1) + 2;
-                        x = Ct(f[P = S - 2], f[S], f[C], .4999), w = Ct(f[P + 1], f[S + 1], f[C + 1], .4999), E = Ct(f[P], f[S], f[C], .5), k = Ct(f[P + 1], f[S + 1], f[C + 1], .5)
-                    }
-                    t = E - x, n = k - w
-                }(s.midtgtArrowAngle = mt(t, n), s.midDispX = t, s.midDispY = n, t *= -1, n *= -1, d) && ((f = s.allpts).length / 2 % 2 == 0 || (t = -(f[b = (m = f.length / 2 - 1) + 2] - f[m]), n = -(f[b + 1] - f[m + 1])));
-                if (s.midsrcArrowAngle = mt(t, n), d) t = a - s.segpts[s.segpts.length - 2], n = o - s.segpts[s.segpts.length - 1];
+                        var k, C;
+                        E = (k = f.length / 2 - 1) + 2;
+                        m = St(f[C = k - 2], f[k], f[E], .4999), b = St(f[C + 1], f[k + 1], f[E + 1], .4999), x = St(f[C], f[k], f[E], .5), w = St(f[C + 1], f[k + 1], f[E + 1], .5)
+                    }
+                    t = x - m, n = w - b
+                }
+                if (s.midtgtArrowAngle = bt(t, n), s.midDispX = t, s.midDispY = n, t *= -1, n *= -1, d)
+                    if ((f = s.allpts).length / 2 % 2 == 0);
+                    else if (!s.isRound) {
+                    var S, P = (S = f.length / 2 - 1) + 2;
+                    t = -(f[P] - f[S]), n = -(f[P + 1] - f[S + 1])
+                }
+                if (s.midsrcArrowAngle = bt(t, n), d) t = a - s.segpts[s.segpts.length - 2], n = o - s.segpts[s.segpts.length - 1];
                 else if (c || h || p || u) {
                     var D = (f = s.allpts).length;
-                    t = a - Ct(f[D - 6], f[D - 4], f[D - 2], .9), n = o - Ct(f[D - 5], f[D - 3], f[D - 1], .9)
+                    t = a - St(f[D - 6], f[D - 4], f[D - 2], .9), n = o - St(f[D - 5], f[D - 3], f[D - 1], .9)
                 } else t = a - g, n = o - v;
-                s.tgtArrowAngle = mt(t, n)
+                s.tgtArrowAngle = bt(t, n)
             }
         };
-    Dl.getArrowWidth = Dl.getArrowHeight = function(e, t) {
+    _l.getArrowWidth = _l.getArrowHeight = function(e, t) {
         var n = this.arrowWidthCache = this.arrowWidthCache || {},
             r = n[e + ", " + t];
         return r || (r = Math.max(Math.pow(13.37 * e, .9), 29) * t, n[e + ", " + t] = r, r)
     };
-    var Tl = {};
+    var Ml, Bl, Nl, zl, Il, Al, Ll, Ol, Rl, Vl, Fl, jl, ql, Yl, Xl, Wl, Hl, Kl = {},
+        Gl = {},
+        Ul = function(e, t, n) {
+            n.x = t.x - e.x, n.y = t.y - e.y, n.len = Math.sqrt(n.x * n.x + n.y * n.y), n.nx = n.x / n.len, n.ny = n.y / n.len, n.ang = Math.atan2(n.ny, n.nx)
+        },
+        Zl = function(e, t, n, r, i) {
+            var a, o;
+            if (e !== Hl ? Ul(t, e, Kl) : ((o = Kl).x = -1 * (a = Gl).x, o.y = -1 * a.y, o.nx = -1 * a.nx, o.ny = -1 * a.ny, o.ang = a.ang > 0 ? -(Math.PI - a.ang) : Math.PI + a.ang), Ul(t, n, Gl), Nl = Kl.nx * Gl.ny - Kl.ny * Gl.nx, zl = Kl.nx * Gl.nx - Kl.ny * -Gl.ny, Ll = Math.asin(Math.max(-1, Math.min(1, Nl))), Math.abs(Ll) < 1e-6) return Ml = t.x, Bl = t.y, void(Rl = Fl = 0);
+            Il = 1, Al = !1, zl < 0 ? Ll < 0 ? Ll = Math.PI + Ll : (Ll = Math.PI - Ll, Il = -1, Al = !0) : Ll > 0 && (Il = -1, Al = !0), Fl = void 0 !== t.radius ? t.radius : r, Ol = Ll / 2, jl = Math.min(Kl.len / 2, Gl.len / 2), i ? (Vl = Math.abs(Math.cos(Ol) * Fl / Math.sin(Ol))) > jl ? (Vl = jl, Rl = Math.abs(Vl * Math.sin(Ol) / Math.cos(Ol))) : Rl = Fl : (Vl = Math.min(jl, Fl), Rl = Math.abs(Vl * Math.sin(Ol) / Math.cos(Ol))), Xl = t.x + Gl.nx * Vl, Wl = t.y + Gl.ny * Vl, Ml = Xl - Gl.ny * Rl * Il, Bl = Wl + Gl.nx * Rl * Il, ql = t.x + Kl.nx * Vl, Yl = t.y + Kl.ny * Vl, Hl = t
+        };
+
+    function $l(e, t) {
+        0 === t.radius ? e.lineTo(t.cx, t.cy) : e.arc(t.cx, t.cy, t.radius, t.startAngle, t.endAngle, t.counterClockwise)
+    }
+
+    function Ql(e, t, n, r) {
+        var i = !(arguments.length > 4 && void 0 !== arguments[4]) || arguments[4];
+        return 0 === r || 0 === t.radius ? {
+            cx: t.x,
+            cy: t.y,
+            radius: 0,
+            startX: t.x,
+            startY: t.y,
+            stopX: t.x,
+            stopY: t.y,
+            startAngle: void 0,
+            endAngle: void 0,
+            counterClockwise: void 0
+        } : (Zl(e, t, n, r, i), {
+            cx: Ml,
+            cy: Bl,
+            radius: Rl,
+            startX: ql,
+            startY: Yl,
+            stopX: Xl,
+            stopY: Wl,
+            startAngle: Kl.ang + Math.PI / 2 * Il,
+            endAngle: Gl.ang - Math.PI / 2 * Il,
+            counterClockwise: Al
+        })
+    }
+    var Jl = {};
 
-    function _l(e) {
+    function eu(e) {
         var t = [];
         if (null != e) {
             for (var n = 0; n < e.length; n += 2) {
                 var r = e[n],
                     i = e[n + 1];
                 t.push({
                     x: r,
                     y: i
                 })
             }
             return t
         }
     }
-    Tl.findMidptPtsEtc = function(e, t) {
+    Jl.findMidptPtsEtc = function(e, t) {
         var n, r = t.posPts,
             i = t.intersectionPts,
             o = t.vectorNormInverse,
             s = e.pstyle("source-endpoint"),
             l = e.pstyle("target-endpoint"),
             u = null != s.units && null != l.units;
         switch (e.pstyle("edge-distances").value) {
@@ -11597,21 +11747,21 @@
                             a = n - e,
                             o = Math.sqrt(a * a + i * i);
                         return {
                             x: -i / o,
                             y: a / o
                         }
                     }(d, h, f, g), n = v
-                } else Ve("Edge ".concat(e.id(), " has edge-distances:endpoints specified without manual endpoints specified via source-endpoint and target-endpoint.  Falling back on edge-distances:intersection (default).")), n = i
+                } else Fe("Edge ".concat(e.id(), " has edge-distances:endpoints specified without manual endpoints specified via source-endpoint and target-endpoint.  Falling back on edge-distances:intersection (default).")), n = i
         }
         return {
             midptPts: n,
             vectorNormInverse: o
         }
-    }, Tl.findHaystackPoints = function(e) {
+    }, Jl.findHaystackPoints = function(e) {
         for (var t = 0; t < e.length; t++) {
             var n = e[t],
                 r = n._private,
                 i = r.rscratch;
             if (!i.haystack) {
                 var a = 2 * Math.random() * Math.PI;
                 i.source = {
@@ -11629,35 +11779,39 @@
                 c = o.width(),
                 d = s.width(),
                 h = o.height(),
                 p = s.height(),
                 f = n.pstyle("haystack-radius").value / 2;
             i.haystackPts = i.allpts = [i.source.x * c * f + l.x, i.source.y * h * f + l.y, i.target.x * d * f + u.x, i.target.y * p * f + u.y], i.midX = (i.allpts[0] + i.allpts[2]) / 2, i.midY = (i.allpts[1] + i.allpts[3]) / 2, i.edgeType = "haystack", i.haystack = !0, this.storeEdgeProjections(n), this.calculateArrowAngles(n), this.recalculateEdgeLabelProjections(n), this.calculateLabelAngles(n)
         }
-    }, Tl.findSegmentsPoints = function(e, t) {
+    }, Jl.findSegmentsPoints = function(e, t) {
         var n = e._private.rscratch,
             r = e.pstyle("segment-weights"),
             i = e.pstyle("segment-distances"),
-            a = Math.min(r.pfValue.length, i.pfValue.length);
-        n.edgeType = "segments", n.segpts = [];
-        for (var o = 0; o < a; o++) {
-            var s = r.pfValue[o],
-                l = i.pfValue[o],
-                u = 1 - s,
-                c = s,
-                d = this.findMidptPtsEtc(e, t),
-                h = d.midptPts,
-                p = d.vectorNormInverse,
-                f = {
-                    x: h.x1 * u + h.x2 * c,
-                    y: h.y1 * u + h.y2 * c
+            a = e.pstyle("segment-radii"),
+            o = e.pstyle("radius-type"),
+            s = Math.min(r.pfValue.length, i.pfValue.length),
+            l = a.pfValue[a.pfValue.length - 1],
+            u = o.pfValue[o.pfValue.length - 1];
+        n.edgeType = "segments", n.segpts = [], n.radii = [], n.isArcRadius = [];
+        for (var c = 0; c < s; c++) {
+            var d = r.pfValue[c],
+                h = i.pfValue[c],
+                p = 1 - d,
+                f = d,
+                g = this.findMidptPtsEtc(e, t),
+                v = g.midptPts,
+                y = g.vectorNormInverse,
+                m = {
+                    x: v.x1 * p + v.x2 * f,
+                    y: v.y1 * p + v.y2 * f
                 };
-            n.segpts.push(f.x + p.x * l, f.y + p.y * l)
+            n.segpts.push(m.x + y.x * h, m.y + y.y * h), n.radii.push(void 0 !== a.pfValue[c] ? a.pfValue[c] : l), n.isArcRadius.push("arc-radius" === (void 0 !== o.pfValue[c] ? o.pfValue[c] : u))
         }
-    }, Tl.findLoopPoints = function(e, t, n, r) {
+    }, Jl.findLoopPoints = function(e, t, n, r) {
         var i = e._private.rscratch,
             a = t.dirCounts,
             o = t.srcPos,
             s = e.pstyle("control-point-distances"),
             l = s ? s.pfValue[0] : void 0,
             u = e.pstyle("loop-direction").pfValue,
             c = e.pstyle("loop-sweep").pfValue,
@@ -11667,15 +11821,15 @@
             p = d;
         r && (h = 0, p = l);
         var f = u - Math.PI / 2,
             g = f - c / 2,
             v = f + c / 2,
             y = String(u + "_" + c);
         h = void 0 === a[y] ? a[y] = 0 : ++a[y], i.ctrlpts = [o.x + 1.4 * Math.cos(g) * p * (h / 3 + 1), o.y + 1.4 * Math.sin(g) * p * (h / 3 + 1), o.x + 1.4 * Math.cos(v) * p * (h / 3 + 1), o.y + 1.4 * Math.sin(v) * p * (h / 3 + 1)]
-    }, Tl.findCompoundLoopPoints = function(e, t, n, r) {
+    }, Jl.findCompoundLoopPoints = function(e, t, n, r) {
         var i = e._private.rscratch;
         i.edgeType = "compound";
         var a = t.srcPos,
             o = t.tgtPos,
             s = t.srcW,
             l = t.srcH,
             u = t.tgtW,
@@ -11697,44 +11851,44 @@
             m = {
                 x: Math.min(v.x, y.x),
                 y: Math.min(v.y, y.y)
             },
             b = Math.max(.5, Math.log(.01 * s)),
             x = Math.max(.5, Math.log(.01 * u));
         i.ctrlpts = [m.x, m.y - (1 + Math.pow(50, 1.12) / 100) * g * (f / 3 + 1) * b, m.x - (1 + Math.pow(50, 1.12) / 100) * g * (f / 3 + 1) * x, m.y]
-    }, Tl.findStraightEdgePoints = function(e) {
+    }, Jl.findStraightEdgePoints = function(e) {
         e._private.rscratch.edgeType = "straight"
-    }, Tl.findBezierPoints = function(e, t, n, r, i) {
+    }, Jl.findBezierPoints = function(e, t, n, r, i) {
         var a = e._private.rscratch,
             o = e.pstyle("control-point-step-size").pfValue,
             s = e.pstyle("control-point-distances"),
             l = e.pstyle("control-point-weights"),
             u = s && l ? Math.min(s.value.length, l.value.length) : 1,
             c = s ? s.pfValue[0] : void 0,
             d = l.value[0],
             h = r;
         a.edgeType = h ? "multibezier" : "bezier", a.ctrlpts = [];
         for (var p = 0; p < u; p++) {
             var f = (.5 - t.eles.length / 2 + n) * o * (i ? -1 : 1),
                 g = void 0,
-                v = xt(f);
+                v = wt(f);
             h && (c = s ? s.pfValue[p] : o, d = l.value[p]);
             var y = void 0 !== (g = r ? c : void 0 !== c ? v * c : void 0) ? g : f,
                 m = 1 - d,
                 b = d,
                 x = this.findMidptPtsEtc(e, t),
                 w = x.midptPts,
                 E = x.vectorNormInverse,
                 k = {
                     x: w.x1 * m + w.x2 * b,
                     y: w.y1 * m + w.y2 * b
                 };
             a.ctrlpts.push(k.x + E.x * y, k.y + E.y * y)
         }
-    }, Tl.findTaxiPoints = function(e, t) {
+    }, Jl.findTaxiPoints = function(e, t) {
         var n = e._private.rscratch;
         n.edgeType = "segments";
         var r = t.posPts,
             i = t.srcW,
             a = t.srcH,
             o = t.tgtW,
             s = t.tgtH,
@@ -11756,31 +11910,31 @@
             w = x(m, v),
             E = x(b, y),
             k = !1;
         "auto" === c ? u = Math.abs(w) > Math.abs(E) ? "horizontal" : "vertical" : "upward" === c || "downward" === c ? (u = "vertical", k = !0) : "leftward" !== c && "rightward" !== c || (u = "horizontal", k = !0);
         var C, S = "vertical" === u,
             P = S ? E : w,
             D = S ? b : m,
-            T = xt(D),
+            T = wt(D),
             _ = !1;
         (k && (h || f) || !("downward" === c && D < 0 || "upward" === c && D > 0 || "leftward" === c && D > 0 || "rightward" === c && D < 0) || (P = (T *= -1) * Math.abs(P), _ = !0), h) ? C = (p < 0 ? 1 + p : p) * P: C = (p < 0 ? P : 0) + p * T;
         var M = function(e) {
                 return Math.abs(e) < g || Math.abs(e) >= Math.abs(P)
             },
             B = M(C),
             N = M(Math.abs(P) - Math.abs(C));
         if ((B || N) && !_)
             if (S) {
                 var z = Math.abs(D) <= a / 2,
                     I = Math.abs(m) <= o / 2;
                 if (z) {
-                    var L = (r.x1 + r.x2) / 2,
-                        A = r.y1,
+                    var A = (r.x1 + r.x2) / 2,
+                        L = r.y1,
                         O = r.y2;
-                    n.segpts = [L, A, L, O]
+                    n.segpts = [A, L, A, O]
                 } else if (I) {
                     var R = (r.y1 + r.y2) / 2,
                         V = r.x1,
                         F = r.x2;
                     n.segpts = [V, R, F, R]
                 } else n.segpts = [r.x1, r.y2]
             } else {
@@ -11805,127 +11959,166 @@
             n.segpts = [Z, U, $, U]
         } else {
             var Q = r.x1 + C + (l ? i / 2 * T : 0),
                 J = r.y1,
                 ee = r.y2;
             n.segpts = [Q, J, Q, ee]
         }
-    }, Tl.tryToCorrectInvalidPoints = function(e, t) {
+        if (n.isRound) {
+            var te = e.pstyle("taxi-radius").value,
+                ne = "arc-radius" === e.pstyle("radius-type").value[0];
+            n.radii = new Array(n.segpts.length / 2).fill(te), n.isArcRadius = new Array(n.segpts.length / 2).fill(ne)
+        }
+    }, Jl.tryToCorrectInvalidPoints = function(e, t) {
         var n = e._private.rscratch;
         if ("bezier" === n.edgeType) {
             var r = t.srcPos,
                 i = t.tgtPos,
                 a = t.srcW,
                 o = t.srcH,
                 s = t.tgtW,
                 l = t.tgtH,
                 u = t.srcShape,
                 c = t.tgtShape,
-                d = !m(n.startX) || !m(n.startY),
-                h = !m(n.arrowStartX) || !m(n.arrowStartY),
-                p = !m(n.endX) || !m(n.endY),
-                f = !m(n.arrowEndX) || !m(n.arrowEndY),
-                g = 3 * (this.getArrowWidth(e.pstyle("width").pfValue, e.pstyle("arrow-scale").value) * this.arrowShapeWidth),
-                v = wt({
+                d = t.srcCornerRadius,
+                h = t.tgtCornerRadius,
+                p = t.srcRs,
+                f = t.tgtRs,
+                g = !b(n.startX) || !b(n.startY),
+                v = !b(n.arrowStartX) || !b(n.arrowStartY),
+                y = !b(n.endX) || !b(n.endY),
+                m = !b(n.arrowEndX) || !b(n.arrowEndY),
+                x = 3 * (this.getArrowWidth(e.pstyle("width").pfValue, e.pstyle("arrow-scale").value) * this.arrowShapeWidth),
+                w = Et({
                     x: n.ctrlpts[0],
                     y: n.ctrlpts[1]
                 }, {
                     x: n.startX,
                     y: n.startY
                 }),
-                y = v < g,
-                b = wt({
+                E = w < x,
+                k = Et({
                     x: n.ctrlpts[0],
                     y: n.ctrlpts[1]
                 }, {
                     x: n.endX,
                     y: n.endY
                 }),
-                x = b < g,
-                w = !1;
-            if (d || h || y) {
-                w = !0;
-                var E = {
+                C = k < x,
+                S = !1;
+            if (g || v || E) {
+                S = !0;
+                var P = {
                         x: n.ctrlpts[0] - r.x,
                         y: n.ctrlpts[1] - r.y
                     },
-                    k = Math.sqrt(E.x * E.x + E.y * E.y),
-                    C = {
-                        x: E.x / k,
-                        y: E.y / k
-                    },
-                    S = Math.max(a, o),
-                    P = {
-                        x: n.ctrlpts[0] + 2 * C.x * S,
-                        y: n.ctrlpts[1] + 2 * C.y * S
-                    },
-                    D = u.intersectLine(r.x, r.y, a, o, P.x, P.y, 0);
-                y ? (n.ctrlpts[0] = n.ctrlpts[0] + C.x * (g - v), n.ctrlpts[1] = n.ctrlpts[1] + C.y * (g - v)) : (n.ctrlpts[0] = D[0] + C.x * g, n.ctrlpts[1] = D[1] + C.y * g)
-            }
-            if (p || f || x) {
-                w = !0;
-                var T = {
+                    D = Math.sqrt(P.x * P.x + P.y * P.y),
+                    T = {
+                        x: P.x / D,
+                        y: P.y / D
+                    },
+                    _ = Math.max(a, o),
+                    M = {
+                        x: n.ctrlpts[0] + 2 * T.x * _,
+                        y: n.ctrlpts[1] + 2 * T.y * _
+                    },
+                    B = u.intersectLine(r.x, r.y, a, o, M.x, M.y, 0, d, p);
+                E ? (n.ctrlpts[0] = n.ctrlpts[0] + T.x * (x - w), n.ctrlpts[1] = n.ctrlpts[1] + T.y * (x - w)) : (n.ctrlpts[0] = B[0] + T.x * x, n.ctrlpts[1] = B[1] + T.y * x)
+            }
+            if (y || m || C) {
+                S = !0;
+                var N = {
                         x: n.ctrlpts[0] - i.x,
                         y: n.ctrlpts[1] - i.y
                     },
-                    _ = Math.sqrt(T.x * T.x + T.y * T.y),
-                    M = {
-                        x: T.x / _,
-                        y: T.y / _
+                    z = Math.sqrt(N.x * N.x + N.y * N.y),
+                    I = {
+                        x: N.x / z,
+                        y: N.y / z
                     },
-                    B = Math.max(a, o),
-                    N = {
-                        x: n.ctrlpts[0] + 2 * M.x * B,
-                        y: n.ctrlpts[1] + 2 * M.y * B
+                    A = Math.max(a, o),
+                    L = {
+                        x: n.ctrlpts[0] + 2 * I.x * A,
+                        y: n.ctrlpts[1] + 2 * I.y * A
                     },
-                    z = c.intersectLine(i.x, i.y, s, l, N.x, N.y, 0);
-                x ? (n.ctrlpts[0] = n.ctrlpts[0] + M.x * (g - b), n.ctrlpts[1] = n.ctrlpts[1] + M.y * (g - b)) : (n.ctrlpts[0] = z[0] + M.x * g, n.ctrlpts[1] = z[1] + M.y * g)
+                    O = c.intersectLine(i.x, i.y, s, l, L.x, L.y, 0, h, f);
+                C ? (n.ctrlpts[0] = n.ctrlpts[0] + I.x * (x - k), n.ctrlpts[1] = n.ctrlpts[1] + I.y * (x - k)) : (n.ctrlpts[0] = O[0] + I.x * x, n.ctrlpts[1] = O[1] + I.y * x)
             }
-            w && this.findEndpoints(e)
+            S && this.findEndpoints(e)
         }
-    }, Tl.storeAllpts = function(e) {
+    }, Jl.storeAllpts = function(e) {
         var t = e._private.rscratch;
         if ("multibezier" === t.edgeType || "bezier" === t.edgeType || "self" === t.edgeType || "compound" === t.edgeType) {
             t.allpts = [], t.allpts.push(t.startX, t.startY);
             for (var n = 0; n + 1 < t.ctrlpts.length; n += 2) t.allpts.push(t.ctrlpts[n], t.ctrlpts[n + 1]), n + 3 < t.ctrlpts.length && t.allpts.push((t.ctrlpts[n] + t.ctrlpts[n + 2]) / 2, (t.ctrlpts[n + 1] + t.ctrlpts[n + 3]) / 2);
             var r;
-            t.allpts.push(t.endX, t.endY), t.ctrlpts.length / 2 % 2 == 0 ? (r = t.allpts.length / 2 - 1, t.midX = t.allpts[r], t.midY = t.allpts[r + 1]) : (r = t.allpts.length / 2 - 3, .5, t.midX = Ct(t.allpts[r], t.allpts[r + 2], t.allpts[r + 4], .5), t.midY = Ct(t.allpts[r + 1], t.allpts[r + 3], t.allpts[r + 5], .5))
+            t.allpts.push(t.endX, t.endY), t.ctrlpts.length / 2 % 2 == 0 ? (r = t.allpts.length / 2 - 1, t.midX = t.allpts[r], t.midY = t.allpts[r + 1]) : (r = t.allpts.length / 2 - 3, .5, t.midX = St(t.allpts[r], t.allpts[r + 2], t.allpts[r + 4], .5), t.midY = St(t.allpts[r + 1], t.allpts[r + 3], t.allpts[r + 5], .5))
         } else if ("straight" === t.edgeType) t.allpts = [t.startX, t.startY, t.endX, t.endY], t.midX = (t.startX + t.endX + t.arrowStartX + t.arrowEndX) / 4, t.midY = (t.startY + t.endY + t.arrowStartY + t.arrowEndY) / 4;
-        else if ("segments" === t.edgeType)
-            if (t.allpts = [], t.allpts.push(t.startX, t.startY), t.allpts.push.apply(t.allpts, t.segpts), t.allpts.push(t.endX, t.endY), t.segpts.length % 4 == 0) {
-                var i = t.segpts.length / 2,
-                    a = i - 2;
-                t.midX = (t.segpts[a] + t.segpts[i]) / 2, t.midY = (t.segpts[a + 1] + t.segpts[i + 1]) / 2
+        else if ("segments" === t.edgeType) {
+            if (t.allpts = [], t.allpts.push(t.startX, t.startY), t.allpts.push.apply(t.allpts, t.segpts), t.allpts.push(t.endX, t.endY), t.isRound) {
+                t.roundCorners = [];
+                for (var i = 2; i + 3 < t.allpts.length; i += 2) {
+                    var a = t.radii[i / 2 - 1],
+                        o = t.isArcRadius[i / 2 - 1];
+                    t.roundCorners.push(Ql({
+                        x: t.allpts[i - 2],
+                        y: t.allpts[i - 1]
+                    }, {
+                        x: t.allpts[i],
+                        y: t.allpts[i + 1],
+                        radius: a
+                    }, {
+                        x: t.allpts[i + 2],
+                        y: t.allpts[i + 3]
+                    }, a, o))
+                }
+            }
+            if (t.segpts.length % 4 == 0) {
+                var s = t.segpts.length / 2,
+                    l = s - 2;
+                t.midX = (t.segpts[l] + t.segpts[s]) / 2, t.midY = (t.segpts[l + 1] + t.segpts[s + 1]) / 2
             } else {
-                var o = t.segpts.length / 2 - 1;
-                t.midX = t.segpts[o], t.midY = t.segpts[o + 1]
+                var u = t.segpts.length / 2 - 1;
+                if (t.isRound) {
+                    var c = {
+                            x: t.segpts[u],
+                            y: t.segpts[u + 1]
+                        },
+                        d = t.roundCorners[u / 2],
+                        h = [c.x - d.cx, c.y - d.cy],
+                        p = d.radius / Math.sqrt(Math.pow(h[0], 2) + Math.pow(h[1], 2));
+                    h = h.map((function(e) {
+                        return e * p
+                    })), t.midX = d.cx + h[0], t.midY = d.cy + h[1], t.midVector = h
+                } else t.midX = t.segpts[u], t.midY = t.segpts[u + 1]
             }
-    }, Tl.checkForInvalidEdgeWarning = function(e) {
+        }
+    }, Jl.checkForInvalidEdgeWarning = function(e) {
         var t = e[0]._private.rscratch;
-        t.nodesOverlap || m(t.startX) && m(t.startY) && m(t.endX) && m(t.endY) ? t.loggedErr = !1 : t.loggedErr || (t.loggedErr = !0, Ve("Edge `" + e.id() + "` has invalid endpoints and so it is impossible to draw.  Adjust your edge style (e.g. control points) accordingly or use an alternative edge type.  This is expected behaviour when the source node and the target node overlap."))
-    }, Tl.findEdgeControlPoints = function(e) {
+        t.nodesOverlap || b(t.startX) && b(t.startY) && b(t.endX) && b(t.endY) ? t.loggedErr = !1 : t.loggedErr || (t.loggedErr = !0, Fe("Edge `" + e.id() + "` has invalid endpoints and so it is impossible to draw.  Adjust your edge style (e.g. control points) accordingly or use an alternative edge type.  This is expected behaviour when the source node and the target node overlap."))
+    }, Jl.findEdgeControlPoints = function(e) {
         var t = this;
         if (e && 0 !== e.length) {
             for (var n = this, r = n.cy.hasCompoundNodes(), i = {
-                    map: new Ue,
+                    map: new Ze,
                     get: function(e) {
                         var t = this.map.get(e[0]);
                         return null != t ? t.get(e[1]) : null
                     },
                     set: function(e, t) {
                         var n = this.map.get(e[0]);
-                        null == n && (n = new Ue, this.map.set(e[0], n)), n.set(e[1], t)
+                        null == n && (n = new Ze, this.map.set(e[0], n)), n.set(e[1], t)
                     }
                 }, a = [], o = [], s = 0; s < e.length; s++) {
                 var l = e[s],
                     u = l._private,
                     c = l.pstyle("curve-style").value;
                 if (!l.removed() && l.takesUpSpace())
                     if ("haystack" !== c) {
-                        var d = "unbundled-bezier" === c || "segments" === c || "straight" === c || "straight-triangle" === c || "taxi" === c,
+                        var d = "unbundled-bezier" === c || c.endsWith("segments") || "straight" === c || "straight-triangle" === c || c.endsWith("taxi"),
                             h = "unbundled-bezier" === c || "bezier" === c,
                             p = u.source,
                             f = u.target,
                             g = [p.poolIndex(), f.poolIndex()].sort(),
                             v = i.get(g);
                         null == v && (v = {
                             eles: []
@@ -11936,15 +12129,15 @@
                     var o = a[e],
                         s = i.get(o),
                         l = void 0;
                     if (!s.hasUnbundled) {
                         var u = s.eles[0].parallelEdges().filter((function(e) {
                             return e.isBundledBezier()
                         }));
-                        He(s.eles), u.forEach((function(e) {
+                        Ke(s.eles), u.forEach((function(e) {
                             return s.eles.push(e)
                         })), s.eles.sort((function(e, t) {
                             return e.poolIndex() - t.poolIndex()
                         }))
                     }
                     var c = s.eles[0],
                         d = c.source(),
@@ -11953,235 +12146,244 @@
                         var p = d;
                         d = h, h = p
                     }
                     var f = s.srcPos = d.position(),
                         g = s.tgtPos = h.position(),
                         v = s.srcW = d.outerWidth(),
                         y = s.srcH = d.outerHeight(),
-                        b = s.tgtW = h.outerWidth(),
+                        m = s.tgtW = h.outerWidth(),
                         x = s.tgtH = h.outerHeight(),
                         w = s.srcShape = n.nodeShapes[t.getNodeShape(d)],
-                        E = s.tgtShape = n.nodeShapes[t.getNodeShape(h)];
+                        E = s.tgtShape = n.nodeShapes[t.getNodeShape(h)],
+                        k = s.srcCornerRadius = "auto" === d.pstyle("corner-radius").value ? "auto" : d.pstyle("corner-radius").pfValue,
+                        C = s.tgtCornerRadius = "auto" === h.pstyle("corner-radius").value ? "auto" : h.pstyle("corner-radius").pfValue,
+                        S = s.tgtRs = h._private.rscratch,
+                        P = s.srcRs = d._private.rscratch;
                     s.dirCounts = {
                         north: 0,
                         west: 0,
                         south: 0,
                         east: 0,
                         northwest: 0,
                         southwest: 0,
                         northeast: 0,
                         southeast: 0
                     };
-                    for (var k = 0; k < s.eles.length; k++) {
-                        var C = s.eles[k],
-                            S = C[0]._private.rscratch,
-                            P = C.pstyle("curve-style").value,
-                            D = "unbundled-bezier" === P || "segments" === P || "taxi" === P,
-                            T = !d.same(C.source());
+                    for (var D = 0; D < s.eles.length; D++) {
+                        var T = s.eles[D],
+                            _ = T[0]._private.rscratch,
+                            M = T.pstyle("curve-style").value,
+                            B = "unbundled-bezier" === M || M.endsWith("segments") || M.endsWith("taxi"),
+                            N = !d.same(T.source());
                         if (!s.calculatedIntersection && d !== h && (s.hasBezier || s.hasUnbundled)) {
                             s.calculatedIntersection = !0;
-                            var _ = w.intersectLine(f.x, f.y, v, y, g.x, g.y, 0),
-                                M = s.srcIntn = _,
-                                B = E.intersectLine(g.x, g.y, b, x, f.x, f.y, 0),
-                                N = s.tgtIntn = B,
-                                z = s.intersectionPts = {
-                                    x1: _[0],
-                                    x2: B[0],
-                                    y1: _[1],
-                                    y2: B[1]
+                            var z = w.intersectLine(f.x, f.y, v, y, g.x, g.y, 0, k, P),
+                                I = s.srcIntn = z,
+                                A = E.intersectLine(g.x, g.y, m, x, f.x, f.y, 0, C, S),
+                                L = s.tgtIntn = A,
+                                O = s.intersectionPts = {
+                                    x1: z[0],
+                                    x2: A[0],
+                                    y1: z[1],
+                                    y2: A[1]
                                 },
-                                I = s.posPts = {
+                                R = s.posPts = {
                                     x1: f.x,
                                     x2: g.x,
                                     y1: f.y,
                                     y2: g.y
                                 },
-                                L = B[1] - _[1],
-                                A = B[0] - _[0],
-                                O = Math.sqrt(A * A + L * L),
-                                R = s.vector = {
-                                    x: A,
-                                    y: L
+                                V = A[1] - z[1],
+                                F = A[0] - z[0],
+                                j = Math.sqrt(F * F + V * V),
+                                q = s.vector = {
+                                    x: F,
+                                    y: V
                                 },
-                                V = s.vectorNorm = {
-                                    x: R.x / O,
-                                    y: R.y / O
+                                Y = s.vectorNorm = {
+                                    x: q.x / j,
+                                    y: q.y / j
                                 },
-                                F = {
-                                    x: -V.y,
-                                    y: V.x
+                                X = {
+                                    x: -Y.y,
+                                    y: Y.x
                                 };
-                            s.nodesOverlap = !m(O) || E.checkPoint(_[0], _[1], 0, b, x, g.x, g.y) || w.checkPoint(B[0], B[1], 0, v, y, f.x, f.y), s.vectorNormInverse = F, l = {
+                            s.nodesOverlap = !b(j) || E.checkPoint(z[0], z[1], 0, m, x, g.x, g.y, C, S) || w.checkPoint(A[0], A[1], 0, v, y, f.x, f.y, k, P), s.vectorNormInverse = X, l = {
                                 nodesOverlap: s.nodesOverlap,
                                 dirCounts: s.dirCounts,
                                 calculatedIntersection: !0,
                                 hasBezier: s.hasBezier,
                                 hasUnbundled: s.hasUnbundled,
                                 eles: s.eles,
                                 srcPos: g,
                                 tgtPos: f,
-                                srcW: b,
+                                srcW: m,
                                 srcH: x,
                                 tgtW: v,
                                 tgtH: y,
-                                srcIntn: N,
-                                tgtIntn: M,
+                                srcIntn: L,
+                                tgtIntn: I,
                                 srcShape: E,
                                 tgtShape: w,
                                 posPts: {
-                                    x1: I.x2,
-                                    y1: I.y2,
-                                    x2: I.x1,
-                                    y2: I.y1
+                                    x1: R.x2,
+                                    y1: R.y2,
+                                    x2: R.x1,
+                                    y2: R.y1
                                 },
                                 intersectionPts: {
-                                    x1: z.x2,
-                                    y1: z.y2,
-                                    x2: z.x1,
-                                    y2: z.y1
+                                    x1: O.x2,
+                                    y1: O.y2,
+                                    x2: O.x1,
+                                    y2: O.y1
                                 },
                                 vector: {
-                                    x: -R.x,
-                                    y: -R.y
+                                    x: -q.x,
+                                    y: -q.y
                                 },
                                 vectorNorm: {
-                                    x: -V.x,
-                                    y: -V.y
+                                    x: -Y.x,
+                                    y: -Y.y
                                 },
                                 vectorNormInverse: {
-                                    x: -F.x,
-                                    y: -F.y
+                                    x: -X.x,
+                                    y: -X.y
                                 }
                             }
                         }
-                        var j = T ? l : s;
-                        S.nodesOverlap = j.nodesOverlap, S.srcIntn = j.srcIntn, S.tgtIntn = j.tgtIntn, r && (d.isParent() || d.isChild() || h.isParent() || h.isChild()) && (d.parents().anySame(h) || h.parents().anySame(d) || d.same(h) && d.isParent()) ? t.findCompoundLoopPoints(C, j, k, D) : d === h ? t.findLoopPoints(C, j, k, D) : "segments" === P ? t.findSegmentsPoints(C, j) : "taxi" === P ? t.findTaxiPoints(C, j) : "straight" === P || !D && s.eles.length % 2 == 1 && k === Math.floor(s.eles.length / 2) ? t.findStraightEdgePoints(C) : t.findBezierPoints(C, j, k, D, T), t.findEndpoints(C), t.tryToCorrectInvalidPoints(C, j), t.checkForInvalidEdgeWarning(C), t.storeAllpts(C), t.storeEdgeProjections(C), t.calculateArrowAngles(C), t.recalculateEdgeLabelProjections(C), t.calculateLabelAngles(C)
+                        var W = N ? l : s;
+                        _.nodesOverlap = W.nodesOverlap, _.srcIntn = W.srcIntn, _.tgtIntn = W.tgtIntn, _.isRound = M.startsWith("round"), r && (d.isParent() || d.isChild() || h.isParent() || h.isChild()) && (d.parents().anySame(h) || h.parents().anySame(d) || d.same(h) && d.isParent()) ? t.findCompoundLoopPoints(T, W, D, B) : d === h ? t.findLoopPoints(T, W, D, B) : M.endsWith("segments") ? t.findSegmentsPoints(T, W) : M.endsWith("taxi") ? t.findTaxiPoints(T, W) : "straight" === M || !B && s.eles.length % 2 == 1 && D === Math.floor(s.eles.length / 2) ? t.findStraightEdgePoints(T) : t.findBezierPoints(T, W, D, B, N), t.findEndpoints(T), t.tryToCorrectInvalidPoints(T, W), t.checkForInvalidEdgeWarning(T), t.storeAllpts(T), t.storeEdgeProjections(T), t.calculateArrowAngles(T), t.recalculateEdgeLabelProjections(T), t.calculateLabelAngles(T)
                     }
-                }, b = 0; b < a.length; b++) y(b);
+                }, m = 0; m < a.length; m++) y(m);
             this.findHaystackPoints(o)
         }
-    }, Tl.getSegmentPoints = function(e) {
+    }, Jl.getSegmentPoints = function(e) {
         var t = e[0]._private.rscratch;
-        if ("segments" === t.edgeType) return this.recalculateRenderedStyle(e), _l(t.segpts)
-    }, Tl.getControlPoints = function(e) {
+        if ("segments" === t.edgeType) return this.recalculateRenderedStyle(e), eu(t.segpts)
+    }, Jl.getControlPoints = function(e) {
         var t = e[0]._private.rscratch,
             n = t.edgeType;
-        if ("bezier" === n || "multibezier" === n || "self" === n || "compound" === n) return this.recalculateRenderedStyle(e), _l(t.ctrlpts)
-    }, Tl.getEdgeMidpoint = function(e) {
+        if ("bezier" === n || "multibezier" === n || "self" === n || "compound" === n) return this.recalculateRenderedStyle(e), eu(t.ctrlpts)
+    }, Jl.getEdgeMidpoint = function(e) {
         var t = e[0]._private.rscratch;
         return this.recalculateRenderedStyle(e), {
             x: t.midX,
             y: t.midY
         }
     };
-    var Ml = {
+    var tu = {
             manualEndptToPx: function(e, t) {
                 var n = e.position(),
                     r = e.outerWidth(),
-                    i = e.outerHeight();
+                    i = e.outerHeight(),
+                    a = e._private.rscratch;
                 if (2 === t.value.length) {
-                    var a = [t.pfValue[0], t.pfValue[1]];
-                    return "%" === t.units[0] && (a[0] = a[0] * r), "%" === t.units[1] && (a[1] = a[1] * i), a[0] += n.x, a[1] += n.y, a
+                    var o = [t.pfValue[0], t.pfValue[1]];
+                    return "%" === t.units[0] && (o[0] = o[0] * r), "%" === t.units[1] && (o[1] = o[1] * i), o[0] += n.x, o[1] += n.y, o
                 }
-                var o = t.pfValue[0];
-                o = -Math.PI / 2 + o;
-                var s = 2 * Math.max(r, i),
-                    l = [n.x + Math.cos(o) * s, n.y + Math.sin(o) * s];
-                return this.nodeShapes[this.getNodeShape(e)].intersectLine(n.x, n.y, r, i, l[0], l[1], 0)
+                var s = t.pfValue[0];
+                s = -Math.PI / 2 + s;
+                var l = 2 * Math.max(r, i),
+                    u = [n.x + Math.cos(s) * l, n.y + Math.sin(s) * l];
+                return this.nodeShapes[this.getNodeShape(e)].intersectLine(n.x, n.y, r, i, u[0], u[1], 0, "auto" === e.pstyle("corner-radius").value ? "auto" : e.pstyle("corner-radius").pfValue, a)
             },
             findEndpoints: function(e) {
                 var t, n, r, i, a, o = this,
                     s = e.source()[0],
                     l = e.target()[0],
                     u = s.position(),
                     c = l.position(),
                     d = e.pstyle("target-arrow-shape").value,
                     h = e.pstyle("source-arrow-shape").value,
                     p = e.pstyle("target-distance-from-node").pfValue,
                     f = e.pstyle("source-distance-from-node").pfValue,
-                    g = e.pstyle("curve-style").value,
-                    v = e._private.rscratch,
-                    y = v.edgeType,
-                    b = "self" === y || "compound" === y,
-                    x = "bezier" === y || "multibezier" === y || b,
-                    w = "bezier" !== y,
-                    E = "straight" === y || "segments" === y,
-                    k = "segments" === y,
-                    C = x || w || E,
-                    S = b || "taxi" === g,
-                    P = e.pstyle("source-endpoint"),
-                    D = S ? "outside-to-node" : P.value,
-                    T = e.pstyle("target-endpoint"),
-                    _ = S ? "outside-to-node" : T.value;
-                if (v.srcManEndpt = P, v.tgtManEndpt = T, x) {
-                    var M = [v.ctrlpts[0], v.ctrlpts[1]];
-                    n = w ? [v.ctrlpts[v.ctrlpts.length - 2], v.ctrlpts[v.ctrlpts.length - 1]] : M, r = M
-                } else if (E) {
-                    var B = k ? v.segpts.slice(0, 2) : [c.x, c.y];
-                    n = k ? v.segpts.slice(v.segpts.length - 2) : [u.x, u.y], r = B
-                }
-                if ("inside-to-node" === _) t = [c.x, c.y];
-                else if (T.units) t = this.manualEndptToPx(l, T);
-                else if ("outside-to-line" === _) t = v.tgtIntn;
-                else if ("outside-to-node" === _ || "outside-to-node-or-label" === _ ? i = n : "outside-to-line" !== _ && "outside-to-line-or-label" !== _ || (i = [u.x, u.y]), t = o.nodeShapes[this.getNodeShape(l)].intersectLine(c.x, c.y, l.outerWidth(), l.outerHeight(), i[0], i[1], 0), "outside-to-node-or-label" === _ || "outside-to-line-or-label" === _) {
-                    var N = l._private.rscratch,
-                        z = N.labelWidth,
-                        I = N.labelHeight,
-                        L = N.labelX,
-                        A = N.labelY,
-                        O = z / 2,
-                        R = I / 2,
-                        V = l.pstyle("text-valign").value;
-                    "top" === V ? A -= R : "bottom" === V && (A += R);
-                    var F = l.pstyle("text-halign").value;
-                    "left" === F ? L -= O : "right" === F && (L += O);
-                    var j = Ut(i[0], i[1], [L - O, A - R, L + O, A - R, L + O, A + R, L - O, A + R], c.x, c.y);
-                    if (j.length > 0) {
-                        var q = u,
-                            Y = Et(q, yt(t)),
-                            X = Et(q, yt(j)),
-                            W = Y;
-                        if (X < Y && (t = j, W = X), j.length > 2) Et(q, {
-                            x: j[2],
-                            y: j[3]
-                        }) < W && (t = [j[2], j[3]])
-                    }
-                }
-                var H = Zt(t, n, o.arrowShapes[d].spacing(e) + p),
-                    K = Zt(t, n, o.arrowShapes[d].gap(e) + p);
-                if (v.endX = K[0], v.endY = K[1], v.arrowEndX = H[0], v.arrowEndY = H[1], "inside-to-node" === D) t = [u.x, u.y];
-                else if (P.units) t = this.manualEndptToPx(s, P);
-                else if ("outside-to-line" === D) t = v.srcIntn;
-                else if ("outside-to-node" === D || "outside-to-node-or-label" === D ? a = r : "outside-to-line" !== D && "outside-to-line-or-label" !== D || (a = [c.x, c.y]), t = o.nodeShapes[this.getNodeShape(s)].intersectLine(u.x, u.y, s.outerWidth(), s.outerHeight(), a[0], a[1], 0), "outside-to-node-or-label" === D || "outside-to-line-or-label" === D) {
-                    var G = s._private.rscratch,
-                        U = G.labelWidth,
-                        Z = G.labelHeight,
-                        $ = G.labelX,
-                        Q = G.labelY,
-                        J = U / 2,
-                        ee = Z / 2,
-                        te = s.pstyle("text-valign").value;
-                    "top" === te ? Q -= ee : "bottom" === te && (Q += ee);
-                    var ne = s.pstyle("text-halign").value;
-                    "left" === ne ? $ -= J : "right" === ne && ($ += J);
-                    var re = Ut(a[0], a[1], [$ - J, Q - ee, $ + J, Q - ee, $ + J, Q + ee, $ - J, Q + ee], u.x, u.y);
-                    if (re.length > 0) {
-                        var ie = c,
-                            ae = Et(ie, yt(t)),
-                            oe = Et(ie, yt(re)),
-                            se = ae;
-                        if (oe < ae && (t = [re[0], re[1]], se = oe), re.length > 2) Et(ie, {
-                            x: re[2],
-                            y: re[3]
-                        }) < se && (t = [re[2], re[3]])
-                    }
-                }
-                var le = Zt(t, r, o.arrowShapes[h].spacing(e) + f),
-                    ue = Zt(t, r, o.arrowShapes[h].gap(e) + f);
-                v.startX = ue[0], v.startY = ue[1], v.arrowStartX = le[0], v.arrowStartY = le[1], C && (m(v.startX) && m(v.startY) && m(v.endX) && m(v.endY) ? v.badLine = !1 : v.badLine = !0)
+                    g = s._private.rscratch,
+                    v = l._private.rscratch,
+                    y = e.pstyle("curve-style").value,
+                    m = e._private.rscratch,
+                    x = m.edgeType,
+                    w = "self" === x || "compound" === x,
+                    E = "bezier" === x || "multibezier" === x || w,
+                    k = "bezier" !== x,
+                    C = "straight" === x || "segments" === x,
+                    S = "segments" === x,
+                    P = E || k || C,
+                    D = w || "taxi" === y,
+                    T = e.pstyle("source-endpoint"),
+                    _ = D ? "outside-to-node" : T.value,
+                    M = "auto" === s.pstyle("corner-radius").value ? "auto" : s.pstyle("corner-radius").pfValue,
+                    B = e.pstyle("target-endpoint"),
+                    N = D ? "outside-to-node" : B.value,
+                    z = "auto" === l.pstyle("corner-radius").value ? "auto" : l.pstyle("corner-radius").pfValue;
+                if (m.srcManEndpt = T, m.tgtManEndpt = B, E) {
+                    var I = [m.ctrlpts[0], m.ctrlpts[1]];
+                    n = k ? [m.ctrlpts[m.ctrlpts.length - 2], m.ctrlpts[m.ctrlpts.length - 1]] : I, r = I
+                } else if (C) {
+                    var A = S ? m.segpts.slice(0, 2) : [c.x, c.y];
+                    n = S ? m.segpts.slice(m.segpts.length - 2) : [u.x, u.y], r = A
+                }
+                if ("inside-to-node" === N) t = [c.x, c.y];
+                else if (B.units) t = this.manualEndptToPx(l, B);
+                else if ("outside-to-line" === N) t = m.tgtIntn;
+                else if ("outside-to-node" === N || "outside-to-node-or-label" === N ? i = n : "outside-to-line" !== N && "outside-to-line-or-label" !== N || (i = [u.x, u.y]), t = o.nodeShapes[this.getNodeShape(l)].intersectLine(c.x, c.y, l.outerWidth(), l.outerHeight(), i[0], i[1], 0, z, v), "outside-to-node-or-label" === N || "outside-to-line-or-label" === N) {
+                    var L = l._private.rscratch,
+                        O = L.labelWidth,
+                        R = L.labelHeight,
+                        V = L.labelX,
+                        F = L.labelY,
+                        j = O / 2,
+                        q = R / 2,
+                        Y = l.pstyle("text-valign").value;
+                    "top" === Y ? F -= q : "bottom" === Y && (F += q);
+                    var X = l.pstyle("text-halign").value;
+                    "left" === X ? V -= j : "right" === X && (V += j);
+                    var W = Zt(i[0], i[1], [V - j, F - q, V + j, F - q, V + j, F + q, V - j, F + q], c.x, c.y);
+                    if (W.length > 0) {
+                        var H = u,
+                            K = kt(H, mt(t)),
+                            G = kt(H, mt(W)),
+                            U = K;
+                        if (G < K && (t = W, U = G), W.length > 2) kt(H, {
+                            x: W[2],
+                            y: W[3]
+                        }) < U && (t = [W[2], W[3]])
+                    }
+                }
+                var Z = $t(t, n, o.arrowShapes[d].spacing(e) + p),
+                    $ = $t(t, n, o.arrowShapes[d].gap(e) + p);
+                if (m.endX = $[0], m.endY = $[1], m.arrowEndX = Z[0], m.arrowEndY = Z[1], "inside-to-node" === _) t = [u.x, u.y];
+                else if (T.units) t = this.manualEndptToPx(s, T);
+                else if ("outside-to-line" === _) t = m.srcIntn;
+                else if ("outside-to-node" === _ || "outside-to-node-or-label" === _ ? a = r : "outside-to-line" !== _ && "outside-to-line-or-label" !== _ || (a = [c.x, c.y]), t = o.nodeShapes[this.getNodeShape(s)].intersectLine(u.x, u.y, s.outerWidth(), s.outerHeight(), a[0], a[1], 0, M, g), "outside-to-node-or-label" === _ || "outside-to-line-or-label" === _) {
+                    var Q = s._private.rscratch,
+                        J = Q.labelWidth,
+                        ee = Q.labelHeight,
+                        te = Q.labelX,
+                        ne = Q.labelY,
+                        re = J / 2,
+                        ie = ee / 2,
+                        ae = s.pstyle("text-valign").value;
+                    "top" === ae ? ne -= ie : "bottom" === ae && (ne += ie);
+                    var oe = s.pstyle("text-halign").value;
+                    "left" === oe ? te -= re : "right" === oe && (te += re);
+                    var se = Zt(a[0], a[1], [te - re, ne - ie, te + re, ne - ie, te + re, ne + ie, te - re, ne + ie], u.x, u.y);
+                    if (se.length > 0) {
+                        var le = c,
+                            ue = kt(le, mt(t)),
+                            ce = kt(le, mt(se)),
+                            de = ue;
+                        if (ce < ue && (t = [se[0], se[1]], de = ce), se.length > 2) kt(le, {
+                            x: se[2],
+                            y: se[3]
+                        }) < de && (t = [se[2], se[3]])
+                    }
+                }
+                var he = $t(t, r, o.arrowShapes[h].spacing(e) + f),
+                    pe = $t(t, r, o.arrowShapes[h].gap(e) + f);
+                m.startX = pe[0], m.startY = pe[1], m.arrowStartX = he[0], m.arrowStartY = he[1], P && (b(m.startX) && b(m.startY) && b(m.endX) && b(m.endY) ? m.badLine = !1 : m.badLine = !0)
             },
             getSourceEndpoint: function(e) {
                 var t = e[0]._private.rscratch;
                 switch (this.recalculateRenderedStyle(e), t.edgeType) {
                     case "haystack":
                         return {
                             x: t.haystackPts[0], y: t.haystackPts[1]
@@ -12202,34 +12404,34 @@
                     default:
                         return {
                             x: t.arrowEndX, y: t.arrowEndY
                         }
                 }
             }
         },
-        Bl = {};
+        nu = {};
 
-    function Nl(e, t, n) {
+    function ru(e, t, n) {
         for (var r = function(e, t, n, r) {
-                return Ct(e, t, n, r)
+                return St(e, t, n, r)
             }, i = t._private.rstyle.bezierPts, a = 0; a < e.bezierProjPcts.length; a++) {
             var o = e.bezierProjPcts[a];
             i.push({
                 x: r(n[0], n[2], n[4], o),
                 y: r(n[1], n[3], n[5], o)
             })
         }
     }
-    Bl.storeEdgeProjections = function(e) {
+    nu.storeEdgeProjections = function(e) {
         var t = e._private,
             n = t.rscratch,
             r = n.edgeType;
         if (t.rstyle.bezierPts = null, t.rstyle.linePts = null, t.rstyle.haystackPts = null, "multibezier" === r || "bezier" === r || "self" === r || "compound" === r) {
             t.rstyle.bezierPts = [];
-            for (var i = 0; i + 5 < n.allpts.length; i += 4) Nl(this, e, n.allpts.slice(i, i + 6))
+            for (var i = 0; i + 5 < n.allpts.length; i += 4) ru(this, e, n.allpts.slice(i, i + 6))
         } else if ("segments" === r) {
             var a = t.rstyle.linePts = [];
             for (i = 0; i + 1 < n.allpts.length; i += 2) a.push({
                 x: n.allpts[i],
                 y: n.allpts[i + 1]
             })
         } else if ("haystack" === r) {
@@ -12239,21 +12441,21 @@
                 y: o[1]
             }, {
                 x: o[2],
                 y: o[3]
             }]
         }
         t.rstyle.arrowWidth = this.getArrowWidth(e.pstyle("width").pfValue, e.pstyle("arrow-scale").value) * this.arrowShapeWidth
-    }, Bl.recalculateEdgeProjections = function(e) {
+    }, nu.recalculateEdgeProjections = function(e) {
         this.findEdgeControlPoints(e)
     };
-    var zl = {
+    var iu = {
             recalculateNodeLabelProjection: function(e) {
                 var t = e.pstyle("label").strValue;
-                if (!S(t)) {
+                if (!P(t)) {
                     var n, r, i = e._private,
                         a = e.width(),
                         o = e.height(),
                         s = e.padding(),
                         l = e.position(),
                         u = e.pstyle("text-halign").strValue,
                         c = e.pstyle("text-valign").strValue,
@@ -12279,42 +12481,42 @@
                         default:
                             r = l.y
                     }
                     d.labelX = n, d.labelY = r, h.labelX = n, h.labelY = r, this.calculateLabelAngles(e), this.applyLabelDimensions(e)
                 }
             }
         },
-        Il = function(e, t) {
+        au = function(e, t) {
             var n = Math.atan(t / e);
             return 0 === e && n < 0 && (n *= -1), n
         },
-        Ll = function(e, t) {
+        ou = function(e, t) {
             var n = t.x - e.x,
                 r = t.y - e.y;
-            return Il(n, r)
+            return au(n, r)
         };
-    zl.recalculateEdgeLabelProjections = function(e) {
+    iu.recalculateEdgeLabelProjections = function(e) {
         var t, n = e._private,
             r = n.rscratch,
             i = this,
             a = {
                 mid: e.pstyle("label").strValue,
                 source: e.pstyle("source-label").strValue,
                 target: e.pstyle("target-label").strValue
             };
         if (a.mid || a.source || a.target) {
             t = {
                 x: r.midX,
                 y: r.midY
             };
             var o = function(e, t, r) {
-                Ge(n.rscratch, e, t, r), Ge(n.rstyle, e, t, r)
+                Ue(n.rscratch, e, t, r), Ue(n.rstyle, e, t, r)
             };
             o("labelX", null, t.x), o("labelY", null, t.y);
-            var s = Il(r.midDispX, r.midDispY);
+            var s = au(r.midDispX, r.midDispY);
             o("labelAutoAngle", null, s);
             var l = function(s) {
                 var l, u = "source" === s;
                 if (a[s]) {
                     var c = e.pstyle(s + "-text-offset").pfValue;
                     switch (r.edgeType) {
                         case "self":
@@ -12345,15 +12547,15 @@
                                             segments: []
                                         })
                                     }
                                     var u = n.rstyle.bezierPts,
                                         c = i.bezierProjPcts.length;
 
                                     function d(e, t, n, r, i) {
-                                        var a = wt(t, n),
+                                        var a = Et(t, n),
                                             o = e.segments[e.segments.length - 1],
                                             s = {
                                                 p0: t,
                                                 p1: n,
                                                 t0: r,
                                                 t1: i,
                                                 startDist: o ? o.startDist + o.length : 0,
@@ -12384,20 +12586,20 @@
                                 if (d) break
                             }
                             var x = d.cp,
                                 w = d.segment,
                                 E = (c - p) / w.length,
                                 k = w.t1 - w.t0,
                                 C = u ? w.t0 + k * E : w.t1 - k * E;
-                            C = Pt(0, C, 1), t = St(x.p0, x.p1, x.p2, C), l = function(e, t, n, r) {
-                                var i = Pt(0, r - .001, 1),
-                                    a = Pt(0, r + .001, 1),
-                                    o = St(e, t, n, i),
-                                    s = St(e, t, n, a);
-                                return Ll(o, s)
+                            C = Dt(0, C, 1), t = Pt(x.p0, x.p1, x.p2, C), l = function(e, t, n, r) {
+                                var i = Dt(0, r - .001, 1),
+                                    a = Dt(0, r + .001, 1),
+                                    o = Pt(e, t, n, i),
+                                    s = Pt(e, t, n, a);
+                                return ou(o, s)
                             }(x.p0, x.p1, x.p2, C);
                             break;
                         case "straight":
                         case "segments":
                         case "haystack":
                             for (var S, P, D, T, _ = 0, M = r.allpts.length, B = 0; B + 3 < M && (u ? (D = {
                                     x: r.allpts[B],
@@ -12407,55 +12609,55 @@
                                     y: r.allpts[B + 3]
                                 }) : (D = {
                                     x: r.allpts[M - 2 - B],
                                     y: r.allpts[M - 1 - B]
                                 }, T = {
                                     x: r.allpts[M - 4 - B],
                                     y: r.allpts[M - 3 - B]
-                                }), P = _, !((_ += S = wt(D, T)) >= c)); B += 2);
+                                }), P = _, !((_ += S = Et(D, T)) >= c)); B += 2);
                             var N = (c - P) / S;
-                            N = Pt(0, N, 1), t = function(e, t, n, r) {
+                            N = Dt(0, N, 1), t = function(e, t, n, r) {
                                 var i = t.x - e.x,
                                     a = t.y - e.y,
-                                    o = wt(e, t),
+                                    o = Et(e, t),
                                     s = i / o,
                                     l = a / o;
                                 return n = null == n ? 0 : n, r = null != r ? r : n * o, {
                                     x: e.x + s * r,
                                     y: e.y + l * r
                                 }
-                            }(D, T, N), l = Ll(D, T)
+                            }(D, T, N), l = ou(D, T)
                     }
                     o("labelX", s, t.x), o("labelY", s, t.y), o("labelAutoAngle", s, l)
                 }
             };
             l("source"), l("target"), this.applyLabelDimensions(e)
         }
-    }, zl.applyLabelDimensions = function(e) {
+    }, iu.applyLabelDimensions = function(e) {
         this.applyPrefixedLabelDimensions(e), e.isEdge() && (this.applyPrefixedLabelDimensions(e, "source"), this.applyPrefixedLabelDimensions(e, "target"))
-    }, zl.applyPrefixedLabelDimensions = function(e, t) {
+    }, iu.applyPrefixedLabelDimensions = function(e, t) {
         var n = e._private,
             r = this.getLabelText(e, t),
             i = this.calculateLabelDimensions(e, r),
             a = e.pstyle("line-height").pfValue,
             o = e.pstyle("text-wrap").strValue,
-            s = Ke(n.rscratch, "labelWrapCachedLines", t) || [],
+            s = Ge(n.rscratch, "labelWrapCachedLines", t) || [],
             l = "wrap" !== o ? 1 : Math.max(s.length, 1),
             u = i.height / l,
             c = u * a,
             d = i.width,
             h = i.height + (l - 1) * (a - 1) * u;
-        Ge(n.rstyle, "labelWidth", t, d), Ge(n.rscratch, "labelWidth", t, d), Ge(n.rstyle, "labelHeight", t, h), Ge(n.rscratch, "labelHeight", t, h), Ge(n.rscratch, "labelLineHeight", t, c)
-    }, zl.getLabelText = function(e, t) {
+        Ue(n.rstyle, "labelWidth", t, d), Ue(n.rscratch, "labelWidth", t, d), Ue(n.rstyle, "labelHeight", t, h), Ue(n.rscratch, "labelHeight", t, h), Ue(n.rscratch, "labelLineHeight", t, c)
+    }, iu.getLabelText = function(e, t) {
         var n = e._private,
             r = t ? t + "-" : "",
             i = e.pstyle(r + "label").strValue,
             a = e.pstyle("text-transform").value,
             o = function(e, r) {
-                return r ? (Ge(n.rscratch, e, t, r), r) : Ke(n.rscratch, e, t)
+                return r ? (Ue(n.rscratch, e, t, r), r) : Ge(n.rscratch, e, t)
             };
         if (!i) return "";
         "none" == a || ("uppercase" == a ? i = i.toUpperCase() : "lowercase" == a && (i = i.toLowerCase()));
         var s = e.pstyle("text-wrap").value;
         if ("wrap" === s) {
             var l = o("labelKey");
             if (null != l && o("labelWrapKey") === l) return o("labelWrapCachedText");
@@ -12484,29 +12686,29 @@
             for (var D = 0; D < i.length; D++) {
                 if (this.calculateLabelDimensions(e, S + i[D] + "…").width > C) break;
                 S += i[D], D === i.length - 1 && (P = !0)
             }
             return P || (S += "…"), S
         }
         return i
-    }, zl.getLabelJustification = function(e) {
+    }, iu.getLabelJustification = function(e) {
         var t = e.pstyle("text-justification").strValue,
             n = e.pstyle("text-halign").strValue;
         if ("auto" !== t) return t;
         if (!e.isNode()) return "center";
         switch (n) {
             case "left":
                 return "right";
             case "right":
                 return "left";
             default:
                 return "center"
         }
-    }, zl.calculateLabelDimensions = function(e, t) {
-        var n = Pe(t, e._private.labelDimsKey),
+    }, iu.calculateLabelDimensions = function(e, t) {
+        var n = De(t, e._private.labelDimsKey),
             r = this.labelDimCache || (this.labelDimCache = []),
             i = r[n];
         if (null != i) return i;
         var a = e.pstyle("font-style").strValue,
             o = e.pstyle("font-size").pfValue,
             s = e.pstyle("font-family").strValue,
             l = e.pstyle("font-weight").strValue,
@@ -12525,40 +12727,40 @@
                 b = o;
             h = Math.max(m, h), p += b
         }
         return h += 0, p += 0, r[n] = {
             width: h,
             height: p
         }
-    }, zl.calculateLabelAngle = function(e, t) {
+    }, iu.calculateLabelAngle = function(e, t) {
         var n = e._private.rscratch,
             r = e.isEdge(),
             i = t ? t + "-" : "",
             a = e.pstyle(i + "text-rotation"),
             o = a.strValue;
         return "none" === o ? 0 : r && "autorotate" === o ? n.labelAutoAngle : "autorotate" === o ? 0 : a.pfValue
-    }, zl.calculateLabelAngles = function(e) {
+    }, iu.calculateLabelAngles = function(e) {
         var t = this,
             n = e.isEdge(),
             r = e._private.rscratch;
         r.labelAngle = t.calculateLabelAngle(e), n && (r.sourceLabelAngle = t.calculateLabelAngle(e, "source"), r.targetLabelAngle = t.calculateLabelAngle(e, "target"))
     };
-    var Al = {},
-        Ol = !1;
-    Al.getNodeShape = function(e) {
+    var su = {},
+        lu = !1;
+    su.getNodeShape = function(e) {
         var t = e.pstyle("shape").value;
-        if ("cutrectangle" === t && (e.width() < 28 || e.height() < 28)) return Ol || (Ve("The `cutrectangle` node shape can not be used at small sizes so `rectangle` is used instead"), Ol = !0), "rectangle";
+        if ("cutrectangle" === t && (e.width() < 28 || e.height() < 28)) return lu || (Fe("The `cutrectangle` node shape can not be used at small sizes so `rectangle` is used instead"), lu = !0), "rectangle";
         if (e.isParent()) return "rectangle" === t || "roundrectangle" === t || "round-rectangle" === t || "cutrectangle" === t || "cut-rectangle" === t || "barrel" === t ? t : "rectangle";
         if ("polygon" === t) {
             var n = e.pstyle("shape-polygon-points").value;
             return this.nodeShapes.makePolygon(n).name
         }
         return t
     };
-    var Rl = {
+    var uu = {
             registerCalculationListeners: function() {
                 var e = this.cy,
                     t = e.collection(),
                     n = this,
                     r = function(e) {
                         var n = !(arguments.length > 1 && void 0 !== arguments[1]) || arguments[1];
                         if (t.merge(e), n)
@@ -12625,15 +12827,15 @@
                             g = f.rstyle,
                             v = f.rscratch;
                         g.srcX = v.arrowStartX, g.srcY = v.arrowStartY, g.tgtX = v.arrowEndX, g.tgtY = v.arrowEndY, g.midX = v.midX, g.midY = v.midY, g.labelAngle = v.labelAngle, g.sourceLabelAngle = v.sourceLabelAngle, g.targetLabelAngle = v.targetLabelAngle
                     }
                 }
             }
         },
-        Vl = {
+        cu = {
             updateCachedGrabbedEles: function() {
                 var e = this.cachedZSortedEles;
                 if (e) {
                     e.drag = [], e.nondrag = [];
                     for (var t = [], n = 0; n < e.length; n++) {
                         var r = (i = e[n])._private.rscratch;
                         i.grabbed() && !i.isParent() ? t.push(i) : r.inDragLayer ? e.drag.push(i) : e.nondrag.push(i)
@@ -12646,45 +12848,45 @@
             },
             invalidateCachedZSortedEles: function() {
                 this.cachedZSortedEles = null
             },
             getCachedZSortedEles: function(e) {
                 if (e || !this.cachedZSortedEles) {
                     var t = this.cy.mutableElements().toArray();
-                    t.sort(Do), t.interactive = t.filter((function(e) {
+                    t.sort(_o), t.interactive = t.filter((function(e) {
                         return e.interactive()
                     })), this.cachedZSortedEles = t, this.updateCachedGrabbedEles()
                 } else t = this.cachedZSortedEles;
                 return t
             }
         },
-        Fl = {};
-    [Pl, Dl, Tl, Ml, Bl, zl, Al, Rl, Vl].forEach((function(e) {
-        I(Fl, e)
+        du = {};
+    [Tl, _l, Jl, tu, nu, iu, su, uu, cu].forEach((function(e) {
+        A(du, e)
     }));
-    var jl = {
+    var hu = {
             getCachedImage: function(e, t, n) {
                 var r = this.imageCache = this.imageCache || {},
                     i = r[e];
                 if (i) return i.image.complete || i.image.addEventListener("load", n), i.image;
                 var a = (i = r[e] = r[e] || {}).image = new Image;
                 a.addEventListener("load", n), a.addEventListener("error", (function() {
                     a.error = !0
                 }));
                 return "data:" === e.substring(0, "data:".length).toLowerCase() || (t = "null" === t ? null : t, a.crossOrigin = t), a.src = e, a
             }
         },
-        ql = {
+        pu = {
             registerBinding: function(e, t, n, r) {
                 var i = Array.prototype.slice.apply(arguments, [1]),
                     a = this.binder(e);
                 return a.on.apply(a, i)
             }
         };
-    ql.binder = function(e) {
+    pu.binder = function(e) {
         var t, n = this,
             r = n.cy.window(),
             i = e === r || e === r.document || e === r.document.body || (t = e, "undefined" != typeof HTMLElement && t instanceof HTMLElement);
         if (null == n.supportsPassiveEvents) {
             var a = !1;
             try {
                 var o = Object.defineProperty({}, "passive", {
@@ -12709,19 +12911,19 @@
         };
         return {
             on: s,
             addEventListener: s,
             addListener: s,
             bind: s
         }
-    }, ql.nodeIsDraggable = function(e) {
+    }, pu.nodeIsDraggable = function(e) {
         return e && e.isNode() && !e.locked() && e.grabbable()
-    }, ql.nodeIsGrabbable = function(e) {
+    }, pu.nodeIsGrabbable = function(e) {
         return this.nodeIsDraggable(e) && e.interactive()
-    }, ql.load = function() {
+    }, pu.load = function() {
         var e = this,
             t = e.cy.window(),
             n = function(e) {
                 return e.selected()
             },
             r = function(t, n, r, i) {
                 null == t && (t = e.cy);
@@ -12820,15 +13022,15 @@
                     }
             }
         })), e.container.parentNode && e.removeObserver.observe(e.container.parentNode, {
             childList: !0
         })) : e.registerBinding(e.container, "DOMNodeRemoved", (function(t) {
             e.destroy()
         }));
-        var v = fe((function() {
+        var v = ge((function() {
             e.cy.resize()
         }), 100);
         f && (e.styleObserver = new MutationObserver(v), e.styleObserver.observe(e.container, {
             attributes: !0
         })), e.registerBinding(t, "resize", v), g && (e.resizeObserver = new ResizeObserver(v), e.resizeObserver.observe(e.container));
         var y = function() {
             e.invalidateContainerClientCoordsCache()
@@ -12836,15 +13038,15 @@
         ! function(e, t) {
             for (; null != e;) t(e), e = e.parentNode
         }(e.container, (function(t) {
             e.registerBinding(t, "transitionend", y), e.registerBinding(t, "animationend", y), e.registerBinding(t, "scroll", y)
         })), e.registerBinding(e.container, "contextmenu", (function(e) {
             e.preventDefault()
         }));
-        var b, x, w, E = function(t) {
+        var m, x, w, E = function(t) {
             for (var n = e.findContainerClientCoords(), r = n[0], i = n[1], a = n[2], o = n[3], s = t.touches ? t.touches : [t], l = !1, u = 0; u < s.length; u++) {
                 var c = s[u];
                 if (r <= c.clientX && c.clientX <= r + a && i <= c.clientY && c.clientY <= i + o) {
                     l = !0;
                     break
                 }
             }
@@ -12945,15 +13147,15 @@
                     c = e.projectIntoViewport(l[0], l[1]),
                     h = e.hoverData.mdownPos,
                     p = e.hoverData.mdownGPos,
                     f = e.selection,
                     g = null;
                 e.hoverData.draggingEles || e.hoverData.dragging || e.hoverData.selecting || (g = e.findNearestElement(c[0], c[1], !0, !1));
                 var v, y = e.hoverData.last,
-                    b = e.hoverData.down,
+                    m = e.hoverData.down,
                     x = [c[0] - f[2], c[1] - f[3]],
                     w = e.dragData.possibleDragElements;
                 if (p) {
                     var k = l[0] - p[0],
                         C = k * k,
                         S = l[1] - p[1],
                         P = C + S * S;
@@ -12981,15 +13183,15 @@
                             originalEvent: t,
                             type: "cxtdrag",
                             position: {
                                 x: c[0],
                                 y: c[1]
                             }
                         };
-                        b ? b.emit(_) : o.emit(_), e.hoverData.cxtDragged = !0, e.hoverData.cxtOver && g === e.hoverData.cxtOver || (e.hoverData.cxtOver && e.hoverData.cxtOver.emit({
+                        m ? m.emit(_) : o.emit(_), e.hoverData.cxtDragged = !0, e.hoverData.cxtOver && g === e.hoverData.cxtOver || (e.hoverData.cxtOver && e.hoverData.cxtOver.emit({
                             originalEvent: t,
                             type: "cxtdragout",
                             position: {
                                 x: c[0],
                                 y: c[1]
                             }
                         }), e.hoverData.cxtOver = g, g && g.emit({
@@ -13013,51 +13215,51 @@
                         } else M = {
                             x: x[0] * s,
                             y: x[1] * s
                         };
                         o.panBy(M), o.emit("dragpan"), e.hoverData.dragged = !0
                     }
                     c = e.projectIntoViewport(t.clientX, t.clientY)
-                } else if (1 != f[4] || null != b && !b.pannable()) {
-                    if (b && b.pannable() && b.active() && b.unactivate(), b && b.grabbed() || g == y || (y && r(y, ["mouseout", "tapdragout"], t, {
+                } else if (1 != f[4] || null != m && !m.pannable()) {
+                    if (m && m.pannable() && m.active() && m.unactivate(), m && m.grabbed() || g == y || (y && r(y, ["mouseout", "tapdragout"], t, {
                             x: c[0],
                             y: c[1]
                         }), g && r(g, ["mouseover", "tapdragover"], t, {
                             x: c[0],
                             y: c[1]
-                        }), e.hoverData.last = g), b)
+                        }), e.hoverData.last = g), m)
                         if (v) {
-                            if (o.boxSelectionEnabled() && D) b && b.grabbed() && (d(w), b.emit("freeon"), w.emit("free"), e.dragData.didDrag && (b.emit("dragfreeon"), w.emit("dragfree"))), T();
-                            else if (b && b.grabbed() && e.nodeIsDraggable(b)) {
+                            if (o.boxSelectionEnabled() && D) m && m.grabbed() && (d(w), m.emit("freeon"), w.emit("free"), e.dragData.didDrag && (m.emit("dragfreeon"), w.emit("dragfree"))), T();
+                            else if (m && m.grabbed() && e.nodeIsDraggable(m)) {
                                 var N = !e.dragData.didDrag;
                                 N && e.redrawHint("eles", !0), e.dragData.didDrag = !0, e.hoverData.draggingEles || u(w, {
                                     inDragLayer: !0
                                 });
                                 var z = {
                                     x: 0,
                                     y: 0
                                 };
-                                if (m(x[0]) && m(x[1]) && (z.x += x[0], z.y += x[1], N)) {
+                                if (b(x[0]) && b(x[1]) && (z.x += x[0], z.y += x[1], N)) {
                                     var I = e.hoverData.dragDelta;
-                                    I && m(I[0]) && m(I[1]) && (z.x += I[0], z.y += I[1])
+                                    I && b(I[0]) && b(I[1]) && (z.x += I[0], z.y += I[1])
                                 }
                                 e.hoverData.draggingEles = !0, w.silentShift(z).emit("position drag"), e.redrawHint("drag", !0), e.redraw()
                             }
                         } else ! function() {
                             var t = e.hoverData.dragDelta = e.hoverData.dragDelta || [];
                             0 === t.length ? (t.push(x[0]), t.push(x[1])) : (t[0] += x[0], t[1] += x[1])
                         }();
                     n = !0
                 } else if (v) {
                     if (e.hoverData.dragging || !o.boxSelectionEnabled() || !D && o.panningEnabled() && o.userPanningEnabled()) {
                         if (!e.hoverData.selecting && o.panningEnabled() && o.userPanningEnabled()) {
-                            a(b, e.hoverData.downs) && (e.hoverData.dragging = !0, e.hoverData.justStartedPan = !0, f[4] = 0, e.data.bgActivePosistion = yt(h), e.redrawHint("select", !0), e.redraw())
+                            a(m, e.hoverData.downs) && (e.hoverData.dragging = !0, e.hoverData.justStartedPan = !0, f[4] = 0, e.data.bgActivePosistion = mt(h), e.redrawHint("select", !0), e.redraw())
                         }
                     } else T();
-                    b && b.pannable() && b.active() && b.unactivate()
+                    m && m.pannable() && m.active() && m.unactivate()
                 }
                 return f[2] = c[0], f[3] = c[1], n ? (t.stopPropagation && t.stopPropagation(), t.preventDefault && t.preventDefault(), !1) : void 0
             }
         }), !1), e.registerBinding(t, "mouseup", (function(t) {
             if (e.hoverData.capture) {
                 e.hoverData.capture = !1;
                 var a = e.cy,
@@ -13091,18 +13293,18 @@
                 } else if (1 === e.hoverData.which) {
                     if (r(l, ["mouseup", "tapend", "vmouseup"], t, {
                             x: o[0],
                             y: o[1]
                         }), e.dragData.didDrag || e.hoverData.dragged || e.hoverData.selecting || e.hoverData.isOverThresholdDrag || (r(c, ["click", "tap", "vclick"], t, {
                             x: o[0],
                             y: o[1]
-                        }), x = !1, t.timeStamp - w <= a.multiClickDebounceTime() ? (b && clearTimeout(b), x = !0, w = null, r(c, ["dblclick", "dbltap", "vdblclick"], t, {
+                        }), x = !1, t.timeStamp - w <= a.multiClickDebounceTime() ? (m && clearTimeout(m), x = !0, w = null, r(c, ["dblclick", "dbltap", "vdblclick"], t, {
                             x: o[0],
                             y: o[1]
-                        })) : (b = setTimeout((function() {
+                        })) : (m = setTimeout((function() {
                             x || r(c, ["oneclick", "onetap", "voneclick"], t, {
                                 x: o[0],
                                 y: o[1]
                             })
                         }), a.multiClickDebounceTime()), w = t.timeStamp)), null != c || e.dragData.didDrag || e.hoverData.selecting || e.hoverData.dragged || i(t) || (a.$(n).unselect(["tapunselect"]), u.length > 0 && e.redrawHint("eles", !0), e.dragData.possibleDragElements = u = a.collection()), l != c || e.dragData.didDrag || e.hoverData.selecting || null != l && l._private.selectable && (e.hoverData.dragging || ("additive" === a.selectionType() || h ? l.selected() ? l.unselect(["tapunselect"]) : l.select(["tapselect"]) : h || (a.$(n).unmerge(l).unselect(["tapunselect"]), l.select(["tapselect"]))), e.redrawHint("eles", !0)), e.hoverData.selecting) {
                         var g = a.collection(e.getAllInBox(s[0], s[1], s[2], s[3]));
                         e.redrawHint("select", !0), g.length > 0 && e.redrawHint("eles", !0), a.emit({
@@ -13123,15 +13325,15 @@
                         var y = c && c.grabbed();
                         d(u), y && (c.emit("freeon"), u.emit("free"), e.dragData.didDrag && (c.emit("dragfreeon"), u.emit("dragfree")))
                     }
                 }
                 s[4] = 0, e.hoverData.down = null, e.hoverData.cxtStarted = !1, e.hoverData.draggingEles = !1, e.hoverData.selecting = !1, e.hoverData.isOverThresholdDrag = !1, e.dragData.didDrag = !1, e.hoverData.dragged = !1, e.hoverData.dragDelta = [], e.hoverData.mdownPos = null, e.hoverData.mdownGPos = null
             }
         }), !1);
-        var k, C, S, P, D, T, _, M, B, N, z, I, L, A = function(t) {
+        var k, C, S, P, D, T, _, M, B, N, z, I, A, L = function(t) {
             if (!e.scrollingPage) {
                 var n = e.cy,
                     r = n.zoom(),
                     i = n.pan(),
                     a = e.projectIntoViewport(t.clientX, t.clientY),
                     o = [a[0] * r + i.x, a[1] * r + i.y];
                 if (e.hoverData.draggingEles || e.hoverData.dragging || e.hoverData.cxtStarted || 0 !== e.selection[4]) t.preventDefault();
@@ -13147,22 +13349,22 @@
                             x: o[0],
                             y: o[1]
                         }
                     }), n.emit("gesturechange" === t.type ? "pinchzoom" : "scrollzoom")
                 }
             }
         };
-        e.registerBinding(e.container, "wheel", A, !0), e.registerBinding(t, "scroll", (function(t) {
+        e.registerBinding(e.container, "wheel", L, !0), e.registerBinding(t, "scroll", (function(t) {
             e.scrollingPage = !0, clearTimeout(e.scrollingPageTimeout), e.scrollingPageTimeout = setTimeout((function() {
                 e.scrollingPage = !1
             }), 250)
         }), !0), e.registerBinding(e.container, "gesturestart", (function(t) {
             e.gestureStartZoom = e.cy.zoom(), e.hasTouchStarted || t.preventDefault()
         }), !0), e.registerBinding(e.container, "gesturechange", (function(t) {
-            e.hasTouchStarted || A(t)
+            e.hasTouchStarted || L(t)
         }), !0), e.registerBinding(e.container, "mouseout", (function(t) {
             var n = e.projectIntoViewport(t.clientX, t.clientY);
             e.cy.emit({
                 originalEvent: t,
                 type: "mouseout",
                 position: {
                     x: n[0],
@@ -13203,15 +13405,15 @@
                     if (t.touches[2]) {
                         o = e.projectIntoViewport(t.touches[2].clientX, t.touches[2].clientY);
                         i[4] = o[0], i[5] = o[1]
                     }
                     if (t.touches[1]) {
                         e.touchData.singleTouchMoved = !0, d(e.dragData.touchDragEles);
                         var l = e.findContainerClientCoords();
-                        B = l[0], N = l[1], z = l[2], I = l[3], k = t.touches[0].clientX - B, C = t.touches[0].clientY - N, S = t.touches[1].clientX - B, P = t.touches[1].clientY - N, L = 0 <= k && k <= z && 0 <= S && S <= z && 0 <= C && C <= I && 0 <= P && P <= I;
+                        B = l[0], N = l[1], z = l[2], I = l[3], k = t.touches[0].clientX - B, C = t.touches[0].clientY - N, S = t.touches[1].clientX - B, P = t.touches[1].clientY - N, A = 0 <= k && k <= z && 0 <= S && S <= z && 0 <= C && C <= I && 0 <= P && P <= I;
                         var h = n.pan(),
                             f = n.zoom();
                         D = X(k, C, S, P), T = W(k, C, S, P), M = [((_ = [(k + S) / 2, (C + P) / 2])[0] - h.x) / f, (_[1] - h.y) / f];
                         if (T < 4e4 && !t.touches[2]) {
                             var g = e.findNearestElement(i[0], i[1], !0, !0),
                                 v = e.findNearestElement(i[2], i[3], !0, !0);
                             return g && g.isNode() ? (g.activate().emit({
@@ -13277,15 +13479,15 @@
                             !1 !== e.touchData.singleTouchMoved || e.pinching || e.touchData.selecting || r(e.touchData.start, ["taphold"], t, {
                                 x: i[0],
                                 y: i[1]
                             })
                         }), e.tapholdDuration)
                     }
                     if (t.touches.length >= 1) {
-                        for (var A = e.touchData.startPosition = [null, null, null, null, null, null], O = 0; O < i.length; O++) A[O] = a[O] = i[O];
+                        for (var L = e.touchData.startPosition = [null, null, null, null, null, null], O = 0; O < i.length; O++) L[O] = a[O] = i[O];
                         var R = t.touches[0];
                         e.touchData.startGPosition = [R.clientX, R.clientY]
                     }
                 }
             }, !1), e.registerBinding(window, "touchmove", R = function(t) {
                 var n = e.touchData.capture;
                 if (n || E(t)) {
@@ -13306,26 +13508,26 @@
                         h = e.projectIntoViewport(t.touches[2].clientX, t.touches[2].clientY);
                         s[4] = h[0], s[5] = h[1]
                     }
                     var p, f = e.touchData.startGPosition;
                     if (n && t.touches[0] && f) {
                         for (var g = [], v = 0; v < s.length; v++) g[v] = s[v] - l[v];
                         var y = t.touches[0].clientX - f[0],
-                            b = y * y,
+                            m = y * y,
                             x = t.touches[0].clientY - f[1];
-                        p = b + x * x >= e.touchTapThreshold2
+                        p = m + x * x >= e.touchTapThreshold2
                     }
                     if (n && e.touchData.cxt) {
                         t.preventDefault();
                         var w = t.touches[0].clientX - B,
                             _ = t.touches[0].clientY - N,
                             z = t.touches[1].clientX - B,
                             I = t.touches[1].clientY - N,
-                            A = W(w, _, z, I);
-                        if (A / T >= 2.25 || A >= 22500) {
+                            L = W(w, _, z, I);
+                        if (L / T >= 2.25 || L >= 22500) {
                             e.touchData.cxt = !1, e.data.bgActivePosistion = void 0, e.redrawHint("select", !0);
                             var O = {
                                 originalEvent: t,
                                 type: "cxttapend",
                                 position: {
                                     x: s[0],
                                     y: s[1]
@@ -13375,15 +13577,15 @@
                                 var F = ee[V]._private;
                                 F.grabbed = !1, F.rscratch.inDragLayer = !1
                             }
                         }
                         var j = e.touchData.start,
                             q = (w = t.touches[0].clientX - B, _ = t.touches[0].clientY - N, z = t.touches[1].clientX - B, I = t.touches[1].clientY - N, X(w, _, z, I)),
                             Y = q / D;
-                        if (L) {
+                        if (A) {
                             var H = (w - k + (z - S)) / 2,
                                 K = (_ - C + (I - P)) / 2,
                                 G = o.zoom(),
                                 U = G * Y,
                                 Z = o.pan(),
                                 $ = M[0] * G + Z.x,
                                 Q = M[1] * G + Z.y,
@@ -13423,16 +13625,16 @@
                                 re && u(ee, {
                                     inDragLayer: !0
                                 }), e.dragData.didDrag = !0;
                                 var ie = {
                                     x: 0,
                                     y: 0
                                 };
-                                if (m(g[0]) && m(g[1]))
-                                    if (ie.x += g[0], ie.y += g[1], re) e.redrawHint("eles", !0), (ae = e.touchData.dragDelta) && m(ae[0]) && m(ae[1]) && (ie.x += ae[0], ie.y += ae[1]);
+                                if (b(g[0]) && b(g[1]))
+                                    if (ie.x += g[0], ie.y += g[1], re) e.redrawHint("eles", !0), (ae = e.touchData.dragDelta) && b(ae[0]) && b(ae[1]) && (ie.x += ae[0], ie.y += ae[1]);
                                 e.hoverData.draggingEles = !0, ee.silentShift(ie).emit("position drag"), e.redrawHint("drag", !0), e.touchData.startPosition[0] == l[0] && e.touchData.startPosition[1] == l[1] && e.redrawHint("eles", !0), e.redraw()
                             } else {
                                 var ae;
                                 0 === (ae = e.touchData.dragDelta = e.touchData.dragDelta || []).length ? (ae.push(g[0]), ae.push(g[1])) : (ae[0] += g[0], ae[1] += g[1])
                             } if (r(te || R, ["touchmove", "tapdrag", "vmousemove"], t, {
                                 x: s[0],
                                 y: s[1]
@@ -13449,15 +13651,15 @@
                                 position: {
                                     x: s[0],
                                     y: s[1]
                                 }
                             })), e.touchData.last = R, n)
                             for (V = 0; V < s.length; V++) s[V] && e.touchData.startPosition[V] && p && (e.touchData.singleTouchMoved = !0);
                         if (n && (null == te || te.pannable()) && o.panningEnabled() && o.userPanningEnabled()) {
-                            a(te, e.touchData.starts) && (t.preventDefault(), e.data.bgActivePosistion || (e.data.bgActivePosistion = yt(e.touchData.startPosition)), e.swipePanning ? (o.panBy({
+                            a(te, e.touchData.starts) && (t.preventDefault(), e.data.bgActivePosistion || (e.data.bgActivePosistion = mt(e.touchData.startPosition)), e.swipePanning ? (o.panBy({
                                 x: g[0] * c,
                                 y: g[1] * c
                             }), o.emit("dragpan")) : p && (e.swipePanning = !0, o.panBy({
                                 x: y * c,
                                 y: x * c
                             }), o.emit("dragpan"), te && (te.unactivate(), e.redrawHint("select", !0), e.touchData.start = null)));
                             h = e.projectIntoViewport(t.touches[0].clientX, t.touches[0].clientY);
@@ -13617,251 +13819,233 @@
                         return t.event.pointerId === e.pointerId
                     }))[0];
                     t.event = e, t.touch = K(e)
                 }(e), Z(e), R(e))
             }))
         }
     };
-    var Yl = {
+    var fu = {
         generatePolygon: function(e, t) {
             return this.nodeShapes[e] = {
                 renderer: this,
                 name: e,
                 points: t,
-                draw: function(e, t, n, r, i) {
+                draw: function(e, t, n, r, i, a) {
                     this.renderer.nodeShapeImpl("polygon", e, t, n, r, i, this.points)
                 },
-                intersectLine: function(e, t, n, r, i, a, o) {
-                    return Ut(i, a, this.points, e, t, n / 2, r / 2, o)
+                intersectLine: function(e, t, n, r, i, a, o, s) {
+                    return Zt(i, a, this.points, e, t, n / 2, r / 2, o)
                 },
-                checkPoint: function(e, t, n, r, i, a, o) {
-                    return qt(e, t, this.points, a, o, r, i, [0, -1], n)
+                checkPoint: function(e, t, n, r, i, a, o, s) {
+                    return Yt(e, t, this.points, a, o, r, i, [0, -1], n)
                 }
             }
         }
     };
-    Yl.generateEllipse = function() {
+    fu.generateEllipse = function() {
         return this.nodeShapes.ellipse = {
             renderer: this,
             name: "ellipse",
-            draw: function(e, t, n, r, i) {
+            draw: function(e, t, n, r, i, a) {
                 this.renderer.nodeShapeImpl(this.name, e, t, n, r, i)
             },
-            intersectLine: function(e, t, n, r, i, a, o) {
+            intersectLine: function(e, t, n, r, i, a, o, s) {
                 return function(e, t, n, r, i, a) {
                     var o = n - e,
                         s = r - t;
                     o /= i, s /= a;
                     var l = Math.sqrt(o * o + s * s),
                         u = l - 1;
                     if (u < 0) return [];
                     var c = u / l;
                     return [(n - e) * c + e, (r - t) * c + t]
                 }(i, a, e, t, n / 2 + o, r / 2 + o)
             },
-            checkPoint: function(e, t, n, r, i, a, o) {
-                return Wt(e, t, r, i, a, o, n)
+            checkPoint: function(e, t, n, r, i, a, o, s) {
+                return Ht(e, t, r, i, a, o, n)
             }
         }
-    }, Yl.generateRoundPolygon = function(e, t) {
-        for (var n = new Array(2 * t.length), r = 0; r < t.length / 2; r++) {
-            var i = 2 * r,
-                a = void 0;
-            a = r < t.length / 2 - 1 ? 2 * (r + 1) : 0, n[4 * r] = t[i], n[4 * r + 1] = t[i + 1];
-            var o = t[a] - t[i],
-                s = t[a + 1] - t[i + 1],
-                l = Math.sqrt(o * o + s * s);
-            n[4 * r + 2] = o / l, n[4 * r + 3] = s / l
-        }
+    }, fu.generateRoundPolygon = function(e, t) {
         return this.nodeShapes[e] = {
             renderer: this,
             name: e,
-            points: n,
-            draw: function(e, t, n, r, i) {
-                this.renderer.nodeShapeImpl("round-polygon", e, t, n, r, i, this.points)
+            points: t,
+            getOrCreateCorners: function(e, n, r, i, a, o, s) {
+                if (void 0 !== o[s] && o[s + "-cx"] === e && o[s + "-cy"] === n) return o[s];
+                o[s] = new Array(t.length / 2), o[s + "-cx"] = e, o[s + "-cy"] = n;
+                var l = r / 2,
+                    u = i / 2;
+                a = "auto" === a ? nn(r, i) : a;
+                for (var c = new Array(t.length / 2), d = 0; d < t.length / 2; d++) c[d] = {
+                    x: e + l * t[2 * d],
+                    y: n + u * t[2 * d + 1]
+                };
+                var h, p, f, g, v = c.length;
+                for (p = c[v - 1], h = 0; h < v; h++) f = c[h % v], g = c[(h + 1) % v], o[s][h] = Ql(p, f, g, a), p = f, f = g;
+                return o[s]
+            },
+            draw: function(e, t, n, r, i, a, o) {
+                this.renderer.nodeShapeImpl("round-polygon", e, t, n, r, i, this.points, this.getOrCreateCorners(t, n, r, i, a, o, "drawCorners"))
+            },
+            intersectLine: function(e, t, n, r, i, a, o, s, l) {
+                return function(e, t, n, r, i, a, o, s, l) {
+                    var u, c = [],
+                        d = new Array(2 * n.length);
+                    l.forEach((function(n, a) {
+                        0 === a ? (d[d.length - 2] = n.startX, d[d.length - 1] = n.startY) : (d[4 * a - 2] = n.startX, d[4 * a - 1] = n.startY), d[4 * a] = n.stopX, d[4 * a + 1] = n.stopY, 0 !== (u = Kt(e, t, r, i, n.cx, n.cy, n.radius)).length && c.push(u[0], u[1])
+                    }));
+                    for (var h = 0; h < d.length / 4; h++) 0 !== (u = Ut(e, t, r, i, d[4 * h], d[4 * h + 1], d[4 * h + 2], d[4 * h + 3], !1)).length && c.push(u[0], u[1]);
+                    if (c.length > 2) {
+                        for (var p = [c[0], c[1]], f = Math.pow(p[0] - e, 2) + Math.pow(p[1] - t, 2), g = 1; g < c.length / 2; g++) {
+                            var v = Math.pow(c[2 * g] - e, 2) + Math.pow(c[2 * g + 1] - t, 2);
+                            v <= f && (p[0] = c[2 * g], p[1] = c[2 * g + 1], f = v)
+                        }
+                        return p
+                    }
+                    return c
+                }(i, a, this.points, e, t, 0, 0, 0, this.getOrCreateCorners(e, t, n, r, s, l, "corners"))
             },
-            intersectLine: function(e, t, n, r, i, a, o) {
+            checkPoint: function(e, t, n, r, i, a, o, s, l) {
                 return function(e, t, n, r, i, a, o, s) {
-                    for (var l, u = [], c = new Array(n.length), d = a / 2, h = o / 2, p = tn(a, o), f = 0; f < n.length / 4; f++) {
-                        var g, v = void 0;
-                        v = 0 === f ? n.length - 2 : 4 * f - 2, g = 4 * f + 2;
-                        var y = r + d * n[4 * f],
-                            m = i + h * n[4 * f + 1],
-                            b = -n[v] * n[g] - n[v + 1] * n[g + 1],
-                            x = p / Math.tan(Math.acos(b) / 2),
-                            w = y - x * n[v],
-                            E = m - x * n[v + 1],
-                            k = y + x * n[g],
-                            C = m + x * n[g + 1];
-                        0 === f ? (c[n.length - 2] = w, c[n.length - 1] = E) : (c[4 * f - 2] = w, c[4 * f - 1] = E), c[4 * f] = k, c[4 * f + 1] = C;
-                        var S = n[v + 1],
-                            P = -n[v];
-                        S * n[g] + P * n[g + 1] < 0 && (S *= -1, P *= -1), 0 !== (l = Ht(e, t, r, i, w + S * p, E + P * p, p)).length && u.push(l[0], l[1])
-                    }
-                    for (var D = 0; D < c.length / 4; D++) 0 !== (l = Gt(e, t, r, i, c[4 * D], c[4 * D + 1], c[4 * D + 2], c[4 * D + 3], !1)).length && u.push(l[0], l[1]);
-                    if (u.length > 2) {
-                        for (var T = [u[0], u[1]], _ = Math.pow(T[0] - e, 2) + Math.pow(T[1] - t, 2), M = 1; M < u.length / 2; M++) {
-                            var B = Math.pow(u[2 * M] - e, 2) + Math.pow(u[2 * M + 1] - t, 2);
-                            B <= _ && (T[0] = u[2 * M], T[1] = u[2 * M + 1], _ = B)
-                        }
-                        return T
-                    }
-                    return u
-                }(i, a, this.points, e, t, n, r)
-            },
-            checkPoint: function(e, t, n, r, i, a, o) {
-                return function(e, t, n, r, i, a, o) {
-                    for (var s = new Array(n.length), l = a / 2, u = o / 2, c = tn(a, o), d = c * c, h = 0; h < n.length / 4; h++) {
-                        var p, f = void 0;
-                        f = 0 === h ? n.length - 2 : 4 * h - 2, p = 4 * h + 2;
-                        var g = r + l * n[4 * h],
-                            v = i + u * n[4 * h + 1],
-                            y = -n[f] * n[p] - n[f + 1] * n[p + 1],
-                            m = c / Math.tan(Math.acos(y) / 2),
-                            b = g - m * n[f],
-                            x = v - m * n[f + 1],
-                            w = g + m * n[p],
-                            E = v + m * n[p + 1];
-                        s[4 * h] = b, s[4 * h + 1] = x, s[4 * h + 2] = w, s[4 * h + 3] = E;
-                        var k = n[f + 1],
-                            C = -n[f];
-                        k * n[p] + C * n[p + 1] < 0 && (k *= -1, C *= -1);
-                        var S = b + k * c,
-                            P = x + C * c;
-                        if (Math.pow(S - e, 2) + Math.pow(P - t, 2) <= d) return !0
+                    for (var l = new Array(2 * n.length), u = 0; u < s.length; u++) {
+                        var c = s[u];
+                        if (l[4 * u + 0] = c.startX, l[4 * u + 1] = c.startY, l[4 * u + 2] = c.stopX, l[4 * u + 3] = c.stopY, Math.pow(c.cx - e, 2) + Math.pow(c.cy - t, 2) <= Math.pow(c.radius, 2)) return !0
                     }
-                    return jt(e, t, s)
-                }(e, t, this.points, a, o, r, i)
+                    return qt(e, t, l)
+                }(e, t, this.points, 0, 0, 0, 0, this.getOrCreateCorners(a, o, r, i, s, l, "corners"))
             }
         }
-    }, Yl.generateRoundRectangle = function() {
+    }, fu.generateRoundRectangle = function() {
         return this.nodeShapes["round-rectangle"] = this.nodeShapes.roundrectangle = {
             renderer: this,
             name: "round-rectangle",
-            points: $t(4, 0),
-            draw: function(e, t, n, r, i) {
-                this.renderer.nodeShapeImpl(this.name, e, t, n, r, i)
-            },
-            intersectLine: function(e, t, n, r, i, a, o) {
-                return At(i, a, e, t, n, r, o)
-            },
-            checkPoint: function(e, t, n, r, i, a, o) {
-                var s = en(r, i),
-                    l = 2 * s;
-                return !!qt(e, t, this.points, a, o, r, i - l, [0, -1], n) || (!!qt(e, t, this.points, a, o, r - l, i, [0, -1], n) || (!!Wt(e, t, l, l, a - r / 2 + s, o - i / 2 + s, n) || (!!Wt(e, t, l, l, a + r / 2 - s, o - i / 2 + s, n) || (!!Wt(e, t, l, l, a + r / 2 - s, o + i / 2 - s, n) || !!Wt(e, t, l, l, a - r / 2 + s, o + i / 2 - s, n)))))
+            points: Qt(4, 0),
+            draw: function(e, t, n, r, i, a) {
+                this.renderer.nodeShapeImpl(this.name, e, t, n, r, i, this.points, a)
+            },
+            intersectLine: function(e, t, n, r, i, a, o, s) {
+                return Ot(i, a, e, t, n, r, o, s)
+            },
+            checkPoint: function(e, t, n, r, i, a, o, s) {
+                var l = r / 2,
+                    u = i / 2;
+                s = "auto" === s ? tn(r, i) : s;
+                var c = 2 * (s = Math.min(l, u, s));
+                return !!Yt(e, t, this.points, a, o, r, i - c, [0, -1], n) || (!!Yt(e, t, this.points, a, o, r - c, i, [0, -1], n) || (!!Ht(e, t, c, c, a - l + s, o - u + s, n) || (!!Ht(e, t, c, c, a + l - s, o - u + s, n) || (!!Ht(e, t, c, c, a + l - s, o + u - s, n) || !!Ht(e, t, c, c, a - l + s, o + u - s, n)))))
             }
         }
-    }, Yl.generateCutRectangle = function() {
+    }, fu.generateCutRectangle = function() {
         return this.nodeShapes["cut-rectangle"] = this.nodeShapes.cutrectangle = {
             renderer: this,
             name: "cut-rectangle",
             cornerLength: 8,
-            points: $t(4, 0),
-            draw: function(e, t, n, r, i) {
-                this.renderer.nodeShapeImpl(this.name, e, t, n, r, i)
-            },
-            generateCutTrianglePts: function(e, t, n, r) {
-                var i = this.cornerLength,
-                    a = t / 2,
-                    o = e / 2,
-                    s = n - o,
-                    l = n + o,
-                    u = r - a,
-                    c = r + a;
+            points: Qt(4, 0),
+            draw: function(e, t, n, r, i, a) {
+                this.renderer.nodeShapeImpl(this.name, e, t, n, r, i, null, a)
+            },
+            generateCutTrianglePts: function(e, t, n, r, i) {
+                var a = "auto" === i ? this.cornerLength : i,
+                    o = t / 2,
+                    s = e / 2,
+                    l = n - s,
+                    u = n + s,
+                    c = r - o,
+                    d = r + o;
                 return {
-                    topLeft: [s, u + i, s + i, u, s + i, u + i],
-                    topRight: [l - i, u, l, u + i, l - i, u + i],
-                    bottomRight: [l, c - i, l - i, c, l - i, c - i],
-                    bottomLeft: [s + i, c, s, c - i, s + i, c - i]
-                }
-            },
-            intersectLine: function(e, t, n, r, i, a, o) {
-                var s = this.generateCutTrianglePts(n + 2 * o, r + 2 * o, e, t),
-                    l = [].concat.apply([], [s.topLeft.splice(0, 4), s.topRight.splice(0, 4), s.bottomRight.splice(0, 4), s.bottomLeft.splice(0, 4)]);
-                return Ut(i, a, l, e, t)
-            },
-            checkPoint: function(e, t, n, r, i, a, o) {
-                if (qt(e, t, this.points, a, o, r, i - 2 * this.cornerLength, [0, -1], n)) return !0;
-                if (qt(e, t, this.points, a, o, r - 2 * this.cornerLength, i, [0, -1], n)) return !0;
-                var s = this.generateCutTrianglePts(r, i, a, o);
-                return jt(e, t, s.topLeft) || jt(e, t, s.topRight) || jt(e, t, s.bottomRight) || jt(e, t, s.bottomLeft)
+                    topLeft: [l, c + a, l + a, c, l + a, c + a],
+                    topRight: [u - a, c, u, c + a, u - a, c + a],
+                    bottomRight: [u, d - a, u - a, d, u - a, d - a],
+                    bottomLeft: [l + a, d, l, d - a, l + a, d - a]
+                }
+            },
+            intersectLine: function(e, t, n, r, i, a, o, s) {
+                var l = this.generateCutTrianglePts(n + 2 * o, r + 2 * o, e, t, s),
+                    u = [].concat.apply([], [l.topLeft.splice(0, 4), l.topRight.splice(0, 4), l.bottomRight.splice(0, 4), l.bottomLeft.splice(0, 4)]);
+                return Zt(i, a, u, e, t)
+            },
+            checkPoint: function(e, t, n, r, i, a, o, s) {
+                var l = "auto" === s ? this.cornerLength : s;
+                if (Yt(e, t, this.points, a, o, r, i - 2 * l, [0, -1], n)) return !0;
+                if (Yt(e, t, this.points, a, o, r - 2 * l, i, [0, -1], n)) return !0;
+                var u = this.generateCutTrianglePts(r, i, a, o);
+                return qt(e, t, u.topLeft) || qt(e, t, u.topRight) || qt(e, t, u.bottomRight) || qt(e, t, u.bottomLeft)
             }
         }
-    }, Yl.generateBarrel = function() {
+    }, fu.generateBarrel = function() {
         return this.nodeShapes.barrel = {
             renderer: this,
             name: "barrel",
-            points: $t(4, 0),
-            draw: function(e, t, n, r, i) {
+            points: Qt(4, 0),
+            draw: function(e, t, n, r, i, a) {
                 this.renderer.nodeShapeImpl(this.name, e, t, n, r, i)
             },
-            intersectLine: function(e, t, n, r, i, a, o) {
-                var s = this.generateBarrelBezierPts(n + 2 * o, r + 2 * o, e, t),
-                    l = function(e) {
-                        var t = St({
+            intersectLine: function(e, t, n, r, i, a, o, s) {
+                var l = this.generateBarrelBezierPts(n + 2 * o, r + 2 * o, e, t),
+                    u = function(e) {
+                        var t = Pt({
                                 x: e[0],
                                 y: e[1]
                             }, {
                                 x: e[2],
                                 y: e[3]
                             }, {
                                 x: e[4],
                                 y: e[5]
                             }, .15),
-                            n = St({
+                            n = Pt({
                                 x: e[0],
                                 y: e[1]
                             }, {
                                 x: e[2],
                                 y: e[3]
                             }, {
                                 x: e[4],
                                 y: e[5]
                             }, .5),
-                            r = St({
+                            r = Pt({
                                 x: e[0],
                                 y: e[1]
                             }, {
                                 x: e[2],
                                 y: e[3]
                             }, {
                                 x: e[4],
                                 y: e[5]
                             }, .85);
                         return [e[0], e[1], t.x, t.y, n.x, n.y, r.x, r.y, e[4], e[5]]
                     },
-                    u = [].concat(l(s.topLeft), l(s.topRight), l(s.bottomRight), l(s.bottomLeft));
-                return Ut(i, a, u, e, t)
+                    c = [].concat(u(l.topLeft), u(l.topRight), u(l.bottomRight), u(l.bottomLeft));
+                return Zt(i, a, c, e, t)
             },
             generateBarrelBezierPts: function(e, t, n, r) {
                 var i = t / 2,
                     a = e / 2,
                     o = n - a,
                     s = n + a,
                     l = r - i,
                     u = r + i,
-                    c = nn(e, t),
+                    c = rn(e, t),
                     d = c.heightOffset,
                     h = c.widthOffset,
                     p = c.ctrlPtOffsetPct * e,
                     f = {
                         topLeft: [o, l + d, o + p, l, o + h, l],
                         topRight: [s - h, l, s - p, l, s, l + d],
                         bottomRight: [s, u - d, s - p, u, s - h, u],
                         bottomLeft: [o + h, u, o + p, u, o, u - d]
                     };
                 return f.topLeft.isTop = !0, f.topRight.isTop = !0, f.bottomLeft.isBottom = !0, f.bottomRight.isBottom = !0, f
             },
-            checkPoint: function(e, t, n, r, i, a, o) {
-                var s = nn(r, i),
-                    l = s.heightOffset,
-                    u = s.widthOffset;
-                if (qt(e, t, this.points, a, o, r, i - 2 * l, [0, -1], n)) return !0;
-                if (qt(e, t, this.points, a, o, r - 2 * u, i, [0, -1], n)) return !0;
-                for (var c = this.generateBarrelBezierPts(r, i, a, o), d = function(e, t, n) {
+            checkPoint: function(e, t, n, r, i, a, o, s) {
+                var l = rn(r, i),
+                    u = l.heightOffset,
+                    c = l.widthOffset;
+                if (Yt(e, t, this.points, a, o, r, i - 2 * u, [0, -1], n)) return !0;
+                if (Yt(e, t, this.points, a, o, r - 2 * c, i, [0, -1], n)) return !0;
+                for (var d = this.generateBarrelBezierPts(r, i, a, o), h = function(e, t, n) {
                         var r, i, a = n[4],
                             o = n[2],
                             s = n[0],
                             l = n[5],
                             u = n[1],
                             c = Math.min(a, s),
                             d = Math.max(a, s),
@@ -13877,138 +14061,137 @@
                                     return [(-t + a) / o, (-t - a) / o]
                                 }(f[0], f[1], f[2], e).filter((function(e) {
                                     return 0 <= e && e <= 1
                                 }));
                             if (g.length > 0) return g[0]
                         }
                         return null
-                    }, h = Object.keys(c), p = 0; p < h.length; p++) {
-                    var f = c[h[p]],
-                        g = d(e, t, f);
-                    if (null != g) {
-                        var v = f[5],
-                            y = f[3],
-                            m = f[1],
-                            b = Ct(v, y, m, g);
-                        if (f.isTop && b <= t) return !0;
-                        if (f.isBottom && t <= b) return !0
+                    }, p = Object.keys(d), f = 0; f < p.length; f++) {
+                    var g = d[p[f]],
+                        v = h(e, t, g);
+                    if (null != v) {
+                        var y = g[5],
+                            m = g[3],
+                            b = g[1],
+                            x = St(y, m, b, v);
+                        if (g.isTop && x <= t) return !0;
+                        if (g.isBottom && t <= x) return !0
                     }
                 }
                 return !1
             }
         }
-    }, Yl.generateBottomRoundrectangle = function() {
+    }, fu.generateBottomRoundrectangle = function() {
         return this.nodeShapes["bottom-round-rectangle"] = this.nodeShapes.bottomroundrectangle = {
             renderer: this,
             name: "bottom-round-rectangle",
-            points: $t(4, 0),
-            draw: function(e, t, n, r, i) {
-                this.renderer.nodeShapeImpl(this.name, e, t, n, r, i)
-            },
-            intersectLine: function(e, t, n, r, i, a, o) {
-                var s = t - (r / 2 + o),
-                    l = Gt(i, a, e, t, e - (n / 2 + o), s, e + (n / 2 + o), s, !1);
-                return l.length > 0 ? l : At(i, a, e, t, n, r, o)
-            },
-            checkPoint: function(e, t, n, r, i, a, o) {
-                var s = en(r, i),
-                    l = 2 * s;
-                if (qt(e, t, this.points, a, o, r, i - l, [0, -1], n)) return !0;
-                if (qt(e, t, this.points, a, o, r - l, i, [0, -1], n)) return !0;
+            points: Qt(4, 0),
+            draw: function(e, t, n, r, i, a) {
+                this.renderer.nodeShapeImpl(this.name, e, t, n, r, i, this.points, a)
+            },
+            intersectLine: function(e, t, n, r, i, a, o, s) {
+                var l = t - (r / 2 + o),
+                    u = Ut(i, a, e, t, e - (n / 2 + o), l, e + (n / 2 + o), l, !1);
+                return u.length > 0 ? u : Ot(i, a, e, t, n, r, o, s)
+            },
+            checkPoint: function(e, t, n, r, i, a, o, s) {
+                var l = 2 * (s = "auto" === s ? tn(r, i) : s);
+                if (Yt(e, t, this.points, a, o, r, i - l, [0, -1], n)) return !0;
+                if (Yt(e, t, this.points, a, o, r - l, i, [0, -1], n)) return !0;
                 var u = r / 2 + 2 * n,
                     c = i / 2 + 2 * n;
-                return !!jt(e, t, [a - u, o - c, a - u, o, a + u, o, a + u, o - c]) || (!!Wt(e, t, l, l, a + r / 2 - s, o + i / 2 - s, n) || !!Wt(e, t, l, l, a - r / 2 + s, o + i / 2 - s, n))
+                return !!qt(e, t, [a - u, o - c, a - u, o, a + u, o, a + u, o - c]) || (!!Ht(e, t, l, l, a + r / 2 - s, o + i / 2 - s, n) || !!Ht(e, t, l, l, a - r / 2 + s, o + i / 2 - s, n))
             }
         }
-    }, Yl.registerNodeShapes = function() {
+    }, fu.registerNodeShapes = function() {
         var e = this.nodeShapes = {},
             t = this;
-        this.generateEllipse(), this.generatePolygon("triangle", $t(3, 0)), this.generateRoundPolygon("round-triangle", $t(3, 0)), this.generatePolygon("rectangle", $t(4, 0)), e.square = e.rectangle, this.generateRoundRectangle(), this.generateCutRectangle(), this.generateBarrel(), this.generateBottomRoundrectangle();
+        this.generateEllipse(), this.generatePolygon("triangle", Qt(3, 0)), this.generateRoundPolygon("round-triangle", Qt(3, 0)), this.generatePolygon("rectangle", Qt(4, 0)), e.square = e.rectangle, this.generateRoundRectangle(), this.generateCutRectangle(), this.generateBarrel(), this.generateBottomRoundrectangle();
         var n = [0, 1, 1, 0, 0, -1, -1, 0];
-        this.generatePolygon("diamond", n), this.generateRoundPolygon("round-diamond", n), this.generatePolygon("pentagon", $t(5, 0)), this.generateRoundPolygon("round-pentagon", $t(5, 0)), this.generatePolygon("hexagon", $t(6, 0)), this.generateRoundPolygon("round-hexagon", $t(6, 0)), this.generatePolygon("heptagon", $t(7, 0)), this.generateRoundPolygon("round-heptagon", $t(7, 0)), this.generatePolygon("octagon", $t(8, 0)), this.generateRoundPolygon("round-octagon", $t(8, 0));
+        this.generatePolygon("diamond", n), this.generateRoundPolygon("round-diamond", n), this.generatePolygon("pentagon", Qt(5, 0)), this.generateRoundPolygon("round-pentagon", Qt(5, 0)), this.generatePolygon("hexagon", Qt(6, 0)), this.generateRoundPolygon("round-hexagon", Qt(6, 0)), this.generatePolygon("heptagon", Qt(7, 0)), this.generateRoundPolygon("round-heptagon", Qt(7, 0)), this.generatePolygon("octagon", Qt(8, 0)), this.generateRoundPolygon("round-octagon", Qt(8, 0));
         var r = new Array(20),
-            i = Jt(5, 0),
-            a = Jt(5, Math.PI / 5),
+            i = en(5, 0),
+            a = en(5, Math.PI / 5),
             o = .5 * (3 - Math.sqrt(5));
         o *= 1.57;
         for (var s = 0; s < a.length / 2; s++) a[2 * s] *= o, a[2 * s + 1] *= o;
         for (s = 0; s < 5; s++) r[4 * s] = i[2 * s], r[4 * s + 1] = i[2 * s + 1], r[4 * s + 2] = a[2 * s], r[4 * s + 3] = a[2 * s + 1];
-        r = Qt(r), this.generatePolygon("star", r), this.generatePolygon("vee", [-1, -1, 0, -.333, 1, -1, 0, 1]), this.generatePolygon("rhomboid", [-1, -1, .333, -1, 1, 1, -.333, 1]), this.generatePolygon("right-rhomboid", [-.333, -1, 1, -1, .333, 1, -1, 1]), this.nodeShapes.concavehexagon = this.generatePolygon("concave-hexagon", [-1, -.95, -.75, 0, -1, .95, 1, .95, .75, 0, 1, -.95]);
+        r = Jt(r), this.generatePolygon("star", r), this.generatePolygon("vee", [-1, -1, 0, -.333, 1, -1, 0, 1]), this.generatePolygon("rhomboid", [-1, -1, .333, -1, 1, 1, -.333, 1]), this.generatePolygon("right-rhomboid", [-.333, -1, 1, -1, .333, 1, -1, 1]), this.nodeShapes.concavehexagon = this.generatePolygon("concave-hexagon", [-1, -.95, -.75, 0, -1, .95, 1, .95, .75, 0, 1, -.95]);
         var l = [-1, -1, .25, -1, 1, 0, .25, 1, -1, 1];
         this.generatePolygon("tag", l), this.generateRoundPolygon("round-tag", l), e.makePolygon = function(e) {
             var n, r = "polygon-" + e.join("$");
             return (n = this[r]) ? n : t.generatePolygon(r, e)
         }
     };
-    var Xl = {
+    var gu = {
             timeToRender: function() {
                 return this.redrawTotalTime / this.redrawCount
             },
             redraw: function(e) {
-                e = e || Ye();
+                e = e || Xe();
                 var t = this;
                 void 0 === t.averageRedrawTime && (t.averageRedrawTime = 0), void 0 === t.lastRedrawTime && (t.lastRedrawTime = 0), void 0 === t.lastDrawTime && (t.lastDrawTime = 0), t.requestedFrame = !0, t.renderOptions = e
             },
             beforeRender: function(e, t) {
                 if (!this.destroyed) {
-                    null == t && Oe("Priority is not optional for beforeRender");
+                    null == t && Re("Priority is not optional for beforeRender");
                     var n = this.beforeRenderCallbacks;
                     n.push({
                         fn: e,
                         priority: t
                     }), n.sort((function(e, t) {
                         return t.priority - e.priority
                     }))
                 }
             }
         },
-        Wl = function(e, t, n) {
+        vu = function(e, t, n) {
             for (var r = e.beforeRenderCallbacks, i = 0; i < r.length; i++) r[i].fn(t, n)
         };
-    Xl.startRenderLoop = function() {
+    gu.startRenderLoop = function() {
         var e = this,
             t = e.cy;
         if (!e.renderLoopStarted) {
             e.renderLoopStarted = !0;
-            me((function n(r) {
+            be((function n(r) {
                 if (!e.destroyed) {
                     if (t.batching());
                     else if (e.requestedFrame && !e.skipFrame) {
-                        Wl(e, !0, r);
-                        var i = be();
+                        vu(e, !0, r);
+                        var i = xe();
                         e.render(e.renderOptions);
-                        var a = e.lastDrawTime = be();
+                        var a = e.lastDrawTime = xe();
                         void 0 === e.averageRedrawTime && (e.averageRedrawTime = a - i), void 0 === e.redrawCount && (e.redrawCount = 0), e.redrawCount++, void 0 === e.redrawTotalTime && (e.redrawTotalTime = 0);
                         var o = a - i;
                         e.redrawTotalTime += o, e.lastRedrawTime = o, e.averageRedrawTime = e.averageRedrawTime / 2 + o / 2, e.requestedFrame = !1
-                    } else Wl(e, !1, r);
-                    e.skipFrame = !1, me(n)
+                    } else vu(e, !1, r);
+                    e.skipFrame = !1, be(n)
                 }
             }))
         }
     };
-    var Hl = function(e) {
+    var yu = function(e) {
             this.init(e)
         },
-        Kl = Hl.prototype;
-    Kl.clientFunctions = ["redrawHint", "render", "renderTo", "matchCanvasSize", "nodeShapeImpl", "arrowShapeImpl"], Kl.init = function(e) {
+        mu = yu.prototype;
+    mu.clientFunctions = ["redrawHint", "render", "renderTo", "matchCanvasSize", "nodeShapeImpl", "arrowShapeImpl"], mu.init = function(e) {
         var t = this;
         t.options = e, t.cy = e.cy;
         var n = t.container = e.cy.container(),
             r = t.cy.window();
         if (r) {
             var i = r.document,
                 a = i.head,
                 o = "__________cytoscape_container",
                 s = null != i.getElementById("__________cytoscape_stylesheet");
             if (n.className.indexOf(o) < 0 && (n.className = (n.className || "") + " " + o), !s) {
                 var l = i.createElement("style");
                 l.id = "__________cytoscape_stylesheet", l.textContent = "." + o + " { position: relative; }", a.insertBefore(l, a.children[0])
             }
-            "static" === r.getComputedStyle(n).getPropertyValue("position") && Ve("A Cytoscape container has style position:static and so can not use UI extensions properly")
+            "static" === r.getComputedStyle(n).getPropertyValue("position") && Fe("A Cytoscape container has style position:static and so can not use UI extensions properly")
         }
         t.selection = [void 0, void 0, void 0, void 0, 0], t.bezierProjPcts = [.05, .225, .4, .5, .6, .775, .95], t.hoverData = {
             down: null,
             last: null,
             downTime: null,
             triggerMode: null,
             dragging: !1,
@@ -14020,60 +14203,60 @@
             start: null,
             capture: !1,
             startPosition: [null, null, null, null, null, null],
             singleTouchStartTime: null,
             singleTouchMoved: !0,
             now: [null, null, null, null, null, null],
             earlier: [null, null, null, null, null, null]
-        }, t.redraws = 0, t.showFps = e.showFps, t.debug = e.debug, t.hideEdgesOnViewport = e.hideEdgesOnViewport, t.textureOnViewport = e.textureOnViewport, t.wheelSensitivity = e.wheelSensitivity, t.motionBlurEnabled = e.motionBlur, t.forcedPixelRatio = m(e.pixelRatio) ? e.pixelRatio : null, t.motionBlur = e.motionBlur, t.motionBlurOpacity = e.motionBlurOpacity, t.motionBlurTransparency = 1 - t.motionBlurOpacity, t.motionBlurPxRatio = 1, t.mbPxRBlurry = 1, t.minMbLowQualFrames = 4, t.fullQualityMb = !1, t.clearedForMotionBlur = [], t.desktopTapThreshold = e.desktopTapThreshold, t.desktopTapThreshold2 = e.desktopTapThreshold * e.desktopTapThreshold, t.touchTapThreshold = e.touchTapThreshold, t.touchTapThreshold2 = e.touchTapThreshold * e.touchTapThreshold, t.tapholdDuration = 500, t.bindings = [], t.beforeRenderCallbacks = [], t.beforeRenderPriorities = {
+        }, t.redraws = 0, t.showFps = e.showFps, t.debug = e.debug, t.hideEdgesOnViewport = e.hideEdgesOnViewport, t.textureOnViewport = e.textureOnViewport, t.wheelSensitivity = e.wheelSensitivity, t.motionBlurEnabled = e.motionBlur, t.forcedPixelRatio = b(e.pixelRatio) ? e.pixelRatio : null, t.motionBlur = e.motionBlur, t.motionBlurOpacity = e.motionBlurOpacity, t.motionBlurTransparency = 1 - t.motionBlurOpacity, t.motionBlurPxRatio = 1, t.mbPxRBlurry = 1, t.minMbLowQualFrames = 4, t.fullQualityMb = !1, t.clearedForMotionBlur = [], t.desktopTapThreshold = e.desktopTapThreshold, t.desktopTapThreshold2 = e.desktopTapThreshold * e.desktopTapThreshold, t.touchTapThreshold = e.touchTapThreshold, t.touchTapThreshold2 = e.touchTapThreshold * e.touchTapThreshold, t.tapholdDuration = 500, t.bindings = [], t.beforeRenderCallbacks = [], t.beforeRenderPriorities = {
             animations: 400,
             eleCalcs: 300,
             eleTxrDeq: 200,
             lyrTxrDeq: 150,
             lyrTxrSkip: 100
         }, t.registerNodeShapes(), t.registerArrowShapes(), t.registerCalculationListeners()
-    }, Kl.notify = function(e, t) {
+    }, mu.notify = function(e, t) {
         var n = this,
             r = n.cy;
         this.destroyed || ("init" !== e ? "destroy" !== e ? (("add" === e || "remove" === e || "move" === e && r.hasCompoundNodes() || "load" === e || "zorder" === e || "mount" === e) && n.invalidateCachedZSortedEles(), "viewport" === e && n.redrawHint("select", !0), "load" !== e && "resize" !== e && "mount" !== e || (n.invalidateContainerClientCoordsCache(), n.matchCanvasSize(n.container)), n.redrawHint("eles", !0), n.redrawHint("drag", !0), this.startRenderLoop(), this.redraw()) : n.destroy() : n.load())
-    }, Kl.destroy = function() {
+    }, mu.destroy = function() {
         var e = this;
         e.destroyed = !0, e.cy.stopAnimationLoop();
         for (var t = 0; t < e.bindings.length; t++) {
             var n = e.bindings[t],
                 r = n.target;
             (r.off || r.removeEventListener).apply(r, n.args)
         }
         if (e.bindings = [], e.beforeRenderCallbacks = [], e.onUpdateEleCalcsFns = [], e.removeObserver && e.removeObserver.disconnect(), e.styleObserver && e.styleObserver.disconnect(), e.resizeObserver && e.resizeObserver.disconnect(), e.labelCalcDiv) try {
             document.body.removeChild(e.labelCalcDiv)
         } catch (e) {}
-    }, Kl.isHeadless = function() {
+    }, mu.isHeadless = function() {
         return !1
-    }, [Sl, Fl, jl, ql, Yl, Xl].forEach((function(e) {
-        I(Kl, e)
+    }, [Dl, du, hu, pu, fu, gu].forEach((function(e) {
+        A(mu, e)
     }));
-    var Gl = function(e) {
+    var bu = function(e) {
             return function() {
                 var t = this,
                     n = this.renderer;
                 if (!t.dequeueingSetup) {
                     t.dequeueingSetup = !0;
-                    var r = fe((function() {
+                    var r = ge((function() {
                             n.redrawHint("eles", !0), n.redrawHint("drag", !0), n.redraw()
                         }), e.deqRedrawThreshold),
-                        i = e.priority || Ae;
+                        i = e.priority || Oe;
                     n.beforeRender((function(i, a) {
-                        var o = be(),
+                        var o = xe(),
                             s = n.averageRedrawTime,
                             l = n.lastRedrawTime,
                             u = [],
                             c = n.cy.extent(),
                             d = n.getPixelRatio();
                         for (i || n.flushRenderedStyleQueue();;) {
-                            var h = be(),
+                            var h = xe(),
                                 p = h - o,
                                 f = h - a;
                             if (l < 1e3 / 60) {
                                 var g = 1e3 / 60 - (i ? s : 0);
                                 if (f >= e.deqFastCost * g) break
                             } else if (i) {
                                 if (p >= e.deqCost * l || p >= e.deqAvgCost * s) break
@@ -14083,26 +14266,26 @@
                             for (var y = 0; y < v.length; y++) u.push(v[y])
                         }
                         u.length > 0 && (e.onDeqd(t, u), !i && e.shouldRedraw(t, u, d, c) && r())
                     }), i(t))
                 }
             }
         },
-        Ul = function() {
+        xu = function() {
             function e(n) {
-                var r = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : Ie;
-                t(this, e), this.idsByKey = new Ue, this.keyForId = new Ue, this.cachesByLvl = new Ue, this.lvls = [], this.getKey = n, this.doesEleInvalidateKey = r
+                var r = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : Ae;
+                t(this, e), this.idsByKey = new Ze, this.keyForId = new Ze, this.cachesByLvl = new Ze, this.lvls = [], this.getKey = n, this.doesEleInvalidateKey = r
             }
             return r(e, [{
                 key: "getIdsFor",
                 value: function(e) {
-                    null == e && Oe("Can not get id list for null key");
+                    null == e && Re("Can not get id list for null key");
                     var t = this.idsByKey,
                         n = this.idsByKey.get(e);
-                    return n || (n = new $e, t.set(e, n)), n
+                    return n || (n = new Qe, t.set(e, n)), n
                 }
             }, {
                 key: "addIdForKey",
                 value: function(e, t) {
                     null != e && this.getIdsFor(e).add(t)
                 }
             }, {
@@ -14143,15 +14326,15 @@
                 }
             }, {
                 key: "getCachesAt",
                 value: function(e) {
                     var t = this.cachesByLvl,
                         n = this.lvls,
                         r = t.get(e);
-                    return r || (r = new Ue, t.set(e, r), n.push(e)), r
+                    return r || (r = new Ze, t.set(e, r), n.push(e)), r
                 }
             }, {
                 key: "getCache",
                 value: function(e, t) {
                     return this.getCachesAt(t).get(e)
                 }
             }, {
@@ -14215,55 +14398,55 @@
                         n = this.keyForId.get(t);
                     this.deleteKeyMappingFor(e);
                     var r = this.doesEleInvalidateKey(e);
                     return r && this.invalidateKey(n), r || 0 === this.getNumberOfIdsForKey(n)
                 }
             }]), e
         }(),
-        Zl = {
+        wu = {
             dequeue: "dequeue",
             downscale: "downscale",
             highQuality: "highQuality"
         },
-        $l = Xe({
+        Eu = We({
             getKey: null,
-            doesEleInvalidateKey: Ie,
+            doesEleInvalidateKey: Ae,
             drawElement: null,
             getBoundingBox: null,
             getRotationPoint: null,
             getRotationOffset: null,
-            isVisible: ze,
+            isVisible: Ie,
             allowEdgeTxrCaching: !0,
             allowParentTxrCaching: !0
         }),
-        Ql = function(e, t) {
+        ku = function(e, t) {
             this.renderer = e, this.onDequeues = [];
-            var n = $l(t);
-            I(this, n), this.lookup = new Ul(n.getKey, n.doesEleInvalidateKey), this.setupDequeueing()
+            var n = Eu(t);
+            A(this, n), this.lookup = new xu(n.getKey, n.doesEleInvalidateKey), this.setupDequeueing()
         },
-        Jl = Ql.prototype;
-    Jl.reasons = Zl, Jl.getTextureQueue = function(e) {
+        Cu = ku.prototype;
+    Cu.reasons = wu, Cu.getTextureQueue = function(e) {
         return this.eleImgCaches = this.eleImgCaches || {}, this.eleImgCaches[e] = this.eleImgCaches[e] || []
-    }, Jl.getRetiredTextureQueue = function(e) {
+    }, Cu.getRetiredTextureQueue = function(e) {
         var t = this.eleImgCaches.retired = this.eleImgCaches.retired || {};
         return t[e] = t[e] || []
-    }, Jl.getElementQueue = function() {
-        return this.eleCacheQueue = this.eleCacheQueue || new tt((function(e, t) {
+    }, Cu.getElementQueue = function() {
+        return this.eleCacheQueue = this.eleCacheQueue || new nt((function(e, t) {
             return t.reqs - e.reqs
         }))
-    }, Jl.getElementKeyToQueue = function() {
+    }, Cu.getElementKeyToQueue = function() {
         return this.eleKeyToCacheQueue = this.eleKeyToCacheQueue || {}
-    }, Jl.getElement = function(e, t, n, r, i) {
+    }, Cu.getElement = function(e, t, n, r, i) {
         var a = this,
             o = this.renderer,
             s = o.cy.zoom(),
             l = this.lookup;
         if (!t || 0 === t.w || 0 === t.h || isNaN(t.w) || isNaN(t.h) || !e.visible() || e.removed()) return null;
         if (!a.allowEdgeTxrCaching && e.isEdge() || !a.allowParentTxrCaching && e.isParent()) return null;
-        if (null == r && (r = Math.ceil(bt(s * n))), r < -4) r = -4;
+        if (null == r && (r = Math.ceil(xt(s * n))), r < -4) r = -4;
         else if (s >= 7.99 || r > 3) return null;
         var u = Math.pow(2, r),
             c = t.h * u,
             d = t.w * u,
             h = o.eleTextBiggerThanMin(e, u);
         if (!this.isVisible(e, h)) return null;
         var p, f = l.get(e, r);
@@ -14273,29 +14456,29 @@
             v = g[g.length - 2],
             y = function() {
                 return a.recycleTexture(p, d) || a.addTexture(p, d)
             };
         v || (v = g[g.length - 1]), v || (v = y()), v.width - v.usedWidth < d && (v = y());
         for (var m, b = function(e) {
                 return e && e.scaledLabelShown === h
-            }, x = i && i === Zl.dequeue, w = i && i === Zl.highQuality, E = i && i === Zl.downscale, k = r + 1; k <= 3; k++) {
+            }, x = i && i === wu.dequeue, w = i && i === wu.highQuality, E = i && i === wu.downscale, k = r + 1; k <= 3; k++) {
             var C = l.get(e, k);
             if (C) {
                 m = C;
                 break
             }
         }
         var S = m && m.level === r + 1 ? m : null,
             P = function() {
                 v.context.drawImage(S.texture.canvas, S.x, 0, S.width, S.height, v.usedWidth, 0, d, c)
             };
         if (v.context.setTransform(1, 0, 0, 1, 0, 0), v.context.clearRect(v.usedWidth, 0, d, p), b(S)) P();
         else if (b(m)) {
             if (!w) return a.queueElement(e, m.level - 1), m;
-            for (var D = m.level; D > r; D--) S = a.getElement(e, t, n, D, Zl.downscale);
+            for (var D = m.level; D > r; D--) S = a.getElement(e, t, n, D, wu.downscale);
             P()
         } else {
             var T;
             if (!x && !w && !E)
                 for (var _ = r - 1; _ >= -4; _--) {
                     var M = l.get(e, _);
                     if (M) {
@@ -14311,17 +14494,17 @@
             texture: v,
             level: r,
             scale: u,
             width: d,
             height: c,
             scaledLabelShown: h
         }, v.usedWidth += Math.ceil(d + 8), v.eleCaches.push(f), l.set(e, r, f), a.checkTextureFullness(v), f
-    }, Jl.invalidateElements = function(e) {
+    }, Cu.invalidateElements = function(e) {
         for (var t = 0; t < e.length; t++) this.invalidateElement(e[t])
-    }, Jl.invalidateElement = function(e) {
+    }, Cu.invalidateElement = function(e) {
         var t = this.lookup,
             n = [];
         if (t.isInvalid(e)) {
             for (var r = -4; r <= 3; r++) {
                 var i = t.getForCachedKey(e, r);
                 i && n.push(i)
             }
@@ -14329,76 +14512,76 @@
                 for (var a = 0; a < n.length; a++) {
                     var o = n[a],
                         s = o.texture;
                     s.invalidatedWidth += o.width, o.invalidated = !0, this.checkTextureUtility(s)
                 }
             this.removeFromQueue(e)
         }
-    }, Jl.checkTextureUtility = function(e) {
+    }, Cu.checkTextureUtility = function(e) {
         e.invalidatedWidth >= .2 * e.width && this.retireTexture(e)
-    }, Jl.checkTextureFullness = function(e) {
+    }, Cu.checkTextureFullness = function(e) {
         var t = this.getTextureQueue(e.height);
-        e.usedWidth / e.width > .8 && e.fullnessChecks >= 10 ? We(t, e) : e.fullnessChecks++
-    }, Jl.retireTexture = function(e) {
+        e.usedWidth / e.width > .8 && e.fullnessChecks >= 10 ? He(t, e) : e.fullnessChecks++
+    }, Cu.retireTexture = function(e) {
         var t = e.height,
             n = this.getTextureQueue(t),
             r = this.lookup;
-        We(n, e), e.retired = !0;
+        He(n, e), e.retired = !0;
         for (var i = e.eleCaches, a = 0; a < i.length; a++) {
             var o = i[a];
             r.deleteCache(o.key, o.level)
         }
-        He(i), this.getRetiredTextureQueue(t).push(e)
-    }, Jl.addTexture = function(e, t) {
+        Ke(i), this.getRetiredTextureQueue(t).push(e)
+    }, Cu.addTexture = function(e, t) {
         var n = {};
         return this.getTextureQueue(e).push(n), n.eleCaches = [], n.height = e, n.width = Math.max(1024, t), n.usedWidth = 0, n.invalidatedWidth = 0, n.fullnessChecks = 0, n.canvas = this.renderer.makeOffscreenCanvas(n.width, n.height), n.context = n.canvas.getContext("2d"), n
-    }, Jl.recycleTexture = function(e, t) {
+    }, Cu.recycleTexture = function(e, t) {
         for (var n = this.getTextureQueue(e), r = this.getRetiredTextureQueue(e), i = 0; i < r.length; i++) {
             var a = r[i];
-            if (a.width >= t) return a.retired = !1, a.usedWidth = 0, a.invalidatedWidth = 0, a.fullnessChecks = 0, He(a.eleCaches), a.context.setTransform(1, 0, 0, 1, 0, 0), a.context.clearRect(0, 0, a.width, a.height), We(r, a), n.push(a), a
+            if (a.width >= t) return a.retired = !1, a.usedWidth = 0, a.invalidatedWidth = 0, a.fullnessChecks = 0, Ke(a.eleCaches), a.context.setTransform(1, 0, 0, 1, 0, 0), a.context.clearRect(0, 0, a.width, a.height), He(r, a), n.push(a), a
         }
-    }, Jl.queueElement = function(e, t) {
+    }, Cu.queueElement = function(e, t) {
         var n = this.getElementQueue(),
             r = this.getElementKeyToQueue(),
             i = this.getKey(e),
             a = r[i];
         if (a) a.level = Math.max(a.level, t), a.eles.merge(e), a.reqs++, n.updateItem(a);
         else {
             var o = {
                 eles: e.spawn().merge(e),
                 level: t,
                 reqs: 1,
                 key: i
             };
             n.push(o), r[i] = o
         }
-    }, Jl.dequeue = function(e) {
+    }, Cu.dequeue = function(e) {
         for (var t = this.getElementQueue(), n = this.getElementKeyToQueue(), r = [], i = this.lookup, a = 0; a < 1 && t.size() > 0; a++) {
             var o = t.pop(),
                 s = o.key,
                 l = o.eles[0],
                 u = i.hasCache(l, o.level);
             if (n[s] = null, !u) {
                 r.push(o);
                 var c = this.getBoundingBox(l);
-                this.getElement(l, c, e, o.level, Zl.dequeue)
+                this.getElement(l, c, e, o.level, wu.dequeue)
             }
         }
         return r
-    }, Jl.removeFromQueue = function(e) {
+    }, Cu.removeFromQueue = function(e) {
         var t = this.getElementQueue(),
             n = this.getElementKeyToQueue(),
             r = this.getKey(e),
             i = n[r];
-        null != i && (1 === i.eles.length ? (i.reqs = Ne, t.updateItem(i), t.pop(), n[r] = null) : i.eles.unmerge(e))
-    }, Jl.onDequeue = function(e) {
+        null != i && (1 === i.eles.length ? (i.reqs = ze, t.updateItem(i), t.pop(), n[r] = null) : i.eles.unmerge(e))
+    }, Cu.onDequeue = function(e) {
         this.onDequeues.push(e)
-    }, Jl.offDequeue = function(e) {
-        We(this.onDequeues, e)
-    }, Jl.setupDequeueing = Gl({
+    }, Cu.offDequeue = function(e) {
+        He(this.onDequeues, e)
+    }, Cu.setupDequeueing = bu({
         deqRedrawThreshold: 100,
         deqCost: .15,
         deqAvgCost: .1,
         deqNoDrawCost: .9,
         deqFastCost: .9,
         deq: function(e, t, n) {
             return e.dequeue(t, n)
@@ -14408,65 +14591,65 @@
                 (0, e.onDequeues[n])(t)
             }
         },
         shouldRedraw: function(e, t, n, r) {
             for (var i = 0; i < t.length; i++)
                 for (var a = t[i].eles, o = 0; o < a.length; o++) {
                     var s = a[o].boundingBox();
-                    if (zt(s, r)) return !0
+                    if (It(s, r)) return !0
                 }
             return !1
         },
         priority: function(e) {
             return e.renderer.beforeRenderPriorities.eleTxrDeq
         }
     });
-    var eu = function(e) {
+    var Su = function(e) {
             var t = this,
                 n = t.renderer = e,
                 r = n.cy;
-            t.layersByLevel = {}, t.firstGet = !0, t.lastInvalidationTime = be() - 500, t.skipping = !1, t.eleTxrDeqs = r.collection(), t.scheduleElementRefinement = fe((function() {
+            t.layersByLevel = {}, t.firstGet = !0, t.lastInvalidationTime = xe() - 500, t.skipping = !1, t.eleTxrDeqs = r.collection(), t.scheduleElementRefinement = ge((function() {
                 t.refineElementTextures(t.eleTxrDeqs), t.eleTxrDeqs.unmerge(t.eleTxrDeqs)
             }), 50), n.beforeRender((function(e, n) {
                 n - t.lastInvalidationTime <= 250 ? t.skipping = !0 : t.skipping = !1
             }), n.beforeRenderPriorities.lyrTxrSkip);
-            t.layersQueue = new tt((function(e, t) {
+            t.layersQueue = new nt((function(e, t) {
                 return t.reqs - e.reqs
             })), t.setupDequeueing()
         },
-        tu = eu.prototype,
-        nu = 0,
-        ru = Math.pow(2, 53) - 1;
-    tu.makeLayer = function(e, t) {
+        Pu = Su.prototype,
+        Du = 0,
+        Tu = Math.pow(2, 53) - 1;
+    Pu.makeLayer = function(e, t) {
         var n = Math.pow(2, t),
             r = Math.ceil(e.w * n),
             i = Math.ceil(e.h * n),
             a = this.renderer.makeOffscreenCanvas(r, i),
             o = {
-                id: nu = ++nu % ru,
+                id: Du = ++Du % Tu,
                 bb: e,
                 level: t,
                 width: r,
                 height: i,
                 canvas: a,
                 context: a.getContext("2d"),
                 eles: [],
                 elesQueue: [],
                 reqs: 0
             },
             s = o.context,
             l = -o.bb.x1,
             u = -o.bb.y1;
         return s.scale(n, n), s.translate(l, u), o
-    }, tu.getLayers = function(e, t, n) {
+    }, Pu.getLayers = function(e, t, n) {
         var r = this,
             i = r.renderer.cy.zoom(),
             a = r.firstGet;
         if (r.firstGet = !1, null == n)
-            if ((n = Math.ceil(bt(i * t))) < -4) n = -4;
+            if ((n = Math.ceil(xt(i * t))) < -4) n = -4;
             else if (i >= 3.99 || n > 2) return null;
         r.validateLayersElesOrdering(n, e);
         var o, s, l = r.layersByLevel,
             u = Math.pow(2, n),
             c = l[n] = l[n] || [];
         if (r.levelIsComplete(n, e)) return c;
         ! function() {
@@ -14476,23 +14659,23 @@
                 i = function(e) {
                     if (!s)
                         for (var r = n + e; - 4 <= r && r <= 2 && !t(r); r += e);
                 };
             i(1), i(-1);
             for (var a = c.length - 1; a >= 0; a--) {
                 var o = c[a];
-                o.invalid && We(c, o)
+                o.invalid && He(c, o)
             }
         }();
         var d = function(t) {
             var i = (t = t || {}).after;
             if (function() {
                     if (!o) {
-                        o = Dt();
-                        for (var t = 0; t < e.length; t++) Tt(o, e[t].boundingBox())
+                        o = Tt();
+                        for (var t = 0; t < e.length; t++) _t(o, e[t].boundingBox())
                     }
                 }(), o.w * u * (o.h * u) > 16e6) return null;
             var a = r.makeLayer(o, n);
             if (null != i) {
                 var s = c.indexOf(i) + 1;
                 c.splice(s, 0, a)
             } else(void 0 === t.insert || t.insert) && c.unshift(a);
@@ -14510,32 +14693,32 @@
                         insert: !0,
                         after: h
                     }))) return null;
                 s || f ? r.queueLayer(h, v) : r.drawEleInLayer(h, v, n, t), h.eles.push(v), m[n] = h
             }
         }
         return s || (f ? null : c)
-    }, tu.getEleLevelForLayerLevel = function(e, t) {
+    }, Pu.getEleLevelForLayerLevel = function(e, t) {
         return e
-    }, tu.drawEleInLayer = function(e, t, n, r) {
+    }, Pu.drawEleInLayer = function(e, t, n, r) {
         var i = this.renderer,
             a = e.context,
             o = t.boundingBox();
         0 !== o.w && 0 !== o.h && t.visible() && (n = this.getEleLevelForLayerLevel(n, r), i.setImgSmoothing(a, !1), i.drawCachedElement(a, t, null, null, n, !0), i.setImgSmoothing(a, !0))
-    }, tu.levelIsComplete = function(e, t) {
+    }, Pu.levelIsComplete = function(e, t) {
         var n = this.layersByLevel[e];
         if (!n || 0 === n.length) return !1;
         for (var r = 0, i = 0; i < n.length; i++) {
             var a = n[i];
             if (a.reqs > 0) return !1;
             if (a.invalid) return !1;
             r += a.eles.length
         }
         return r === t.length
-    }, tu.validateLayersElesOrdering = function(e, t) {
+    }, Pu.validateLayersElesOrdering = function(e, t) {
         var n = this.layersByLevel[e];
         if (n)
             for (var r = 0; r < n.length; r++) {
                 for (var i = n[r], a = -1, o = 0; o < t.length; o++)
                     if (i.eles[0] === t[o]) {
                         a = o;
                         break
@@ -14545,126 +14728,126 @@
                     for (o = 0; o < i.eles.length; o++)
                         if (i.eles[o] !== t[s + o]) {
                             this.invalidateLayer(i);
                             break
                         }
                 }
             }
-    }, tu.updateElementsInLayers = function(e, t) {
-        for (var n = w(e[0]), r = 0; r < e.length; r++)
+    }, Pu.updateElementsInLayers = function(e, t) {
+        for (var n = E(e[0]), r = 0; r < e.length; r++)
             for (var i = n ? null : e[r], a = n ? e[r] : e[r].ele, o = a._private.rscratch, s = o.imgLayerCaches = o.imgLayerCaches || {}, l = -4; l <= 2; l++) {
                 var u = s[l];
                 u && (i && this.getEleLevelForLayerLevel(u.level) !== i.level || t(u, a, i))
             }
-    }, tu.haveLayers = function() {
+    }, Pu.haveLayers = function() {
         for (var e = !1, t = -4; t <= 2; t++) {
             var n = this.layersByLevel[t];
             if (n && n.length > 0) {
                 e = !0;
                 break
             }
         }
         return e
-    }, tu.invalidateElements = function(e) {
+    }, Pu.invalidateElements = function(e) {
         var t = this;
-        0 !== e.length && (t.lastInvalidationTime = be(), 0 !== e.length && t.haveLayers() && t.updateElementsInLayers(e, (function(e, n, r) {
+        0 !== e.length && (t.lastInvalidationTime = xe(), 0 !== e.length && t.haveLayers() && t.updateElementsInLayers(e, (function(e, n, r) {
             t.invalidateLayer(e)
         })))
-    }, tu.invalidateLayer = function(e) {
-        if (this.lastInvalidationTime = be(), !e.invalid) {
+    }, Pu.invalidateLayer = function(e) {
+        if (this.lastInvalidationTime = xe(), !e.invalid) {
             var t = e.level,
                 n = e.eles,
                 r = this.layersByLevel[t];
-            We(r, e), e.elesQueue = [], e.invalid = !0, e.replacement && (e.replacement.invalid = !0);
+            He(r, e), e.elesQueue = [], e.invalid = !0, e.replacement && (e.replacement.invalid = !0);
             for (var i = 0; i < n.length; i++) {
                 var a = n[i]._private.rscratch.imgLayerCaches;
                 a && (a[t] = null)
             }
         }
-    }, tu.refineElementTextures = function(e) {
+    }, Pu.refineElementTextures = function(e) {
         var t = this;
         t.updateElementsInLayers(e, (function(e, n, r) {
             var i = e.replacement;
             if (i || ((i = e.replacement = t.makeLayer(e.bb, e.level)).replaces = e, i.eles = e.eles), !i.reqs)
                 for (var a = 0; a < i.eles.length; a++) t.queueLayer(i, i.eles[a])
         }))
-    }, tu.enqueueElementRefinement = function(e) {
+    }, Pu.enqueueElementRefinement = function(e) {
         this.eleTxrDeqs.merge(e), this.scheduleElementRefinement()
-    }, tu.queueLayer = function(e, t) {
+    }, Pu.queueLayer = function(e, t) {
         var n = this.layersQueue,
             r = e.elesQueue,
             i = r.hasId = r.hasId || {};
         if (!e.replacement) {
             if (t) {
                 if (i[t.id()]) return;
                 r.push(t), i[t.id()] = !0
             }
             e.reqs ? (e.reqs++, n.updateItem(e)) : (e.reqs = 1, n.push(e))
         }
-    }, tu.dequeue = function(e) {
+    }, Pu.dequeue = function(e) {
         for (var t = this.layersQueue, n = [], r = 0; r < 1 && 0 !== t.size();) {
             var i = t.peek();
             if (i.replacement) t.pop();
             else if (i.replaces && i !== i.replaces.replacement) t.pop();
             else if (i.invalid) t.pop();
             else {
                 var a = i.elesQueue.shift();
                 a && (this.drawEleInLayer(i, a, i.level, e), r++), 0 === n.length && n.push(!0), 0 === i.elesQueue.length && (t.pop(), i.reqs = 0, i.replaces && this.applyLayerReplacement(i), this.requestRedraw())
             }
         }
         return n
-    }, tu.applyLayerReplacement = function(e) {
+    }, Pu.applyLayerReplacement = function(e) {
         var t = this.layersByLevel[e.level],
             n = e.replaces,
             r = t.indexOf(n);
         if (!(r < 0 || n.invalid)) {
             t[r] = e;
             for (var i = 0; i < e.eles.length; i++) {
                 var a = e.eles[i]._private,
                     o = a.imgLayerCaches = a.imgLayerCaches || {};
                 o && (o[e.level] = e)
             }
             this.requestRedraw()
         }
-    }, tu.requestRedraw = fe((function() {
+    }, Pu.requestRedraw = ge((function() {
         var e = this.renderer;
         e.redrawHint("eles", !0), e.redrawHint("drag", !0), e.redraw()
-    }), 100), tu.setupDequeueing = Gl({
+    }), 100), Pu.setupDequeueing = bu({
         deqRedrawThreshold: 50,
         deqCost: .15,
         deqAvgCost: .1,
         deqNoDrawCost: .9,
         deqFastCost: .9,
         deq: function(e, t) {
             return e.dequeue(t)
         },
-        onDeqd: Ae,
-        shouldRedraw: ze,
+        onDeqd: Oe,
+        shouldRedraw: Ie,
         priority: function(e) {
             return e.renderer.beforeRenderPriorities.lyrTxrDeq
         }
     });
-    var iu, au = {};
+    var _u, Mu = {};
 
-    function ou(e, t) {
+    function Bu(e, t) {
         for (var n = 0; n < t.length; n++) {
             var r = t[n];
             e.lineTo(r.x, r.y)
         }
     }
 
-    function su(e, t, n) {
+    function Nu(e, t, n) {
         for (var r, i = 0; i < t.length; i++) {
             var a = t[i];
             0 === i && (r = a), e.lineTo(a.x, a.y)
         }
         e.quadraticCurveTo(n.x, n.y, r.x, r.y)
     }
 
-    function lu(e, t, n) {
+    function zu(e, t, n) {
         e.beginPath && e.beginPath();
         for (var r = t, i = 0; i < r.length; i++) {
             var a = r[i];
             e.lineTo(a.x, a.y)
         }
         var o = n,
             s = n[0];
@@ -14672,40 +14855,40 @@
         for (i = 1; i < o.length; i++) {
             a = o[i];
             e.lineTo(a.x, a.y)
         }
         e.closePath && e.closePath()
     }
 
-    function uu(e, t, n, r, i) {
+    function Iu(e, t, n, r, i) {
         e.beginPath && e.beginPath(), e.arc(n, r, i, 0, 2 * Math.PI, !1);
         var a = t,
             o = a[0];
         e.moveTo(o.x, o.y);
         for (var s = 0; s < a.length; s++) {
             var l = a[s];
             e.lineTo(l.x, l.y)
         }
         e.closePath && e.closePath()
     }
 
-    function cu(e, t, n, r) {
+    function Au(e, t, n, r) {
         e.arc(t, n, r, 0, 2 * Math.PI, !1)
     }
-    au.arrowShapeImpl = function(e) {
-        return (iu || (iu = {
-            polygon: ou,
-            "triangle-backcurve": su,
-            "triangle-tee": lu,
-            "circle-triangle": uu,
-            "triangle-cross": lu,
-            circle: cu
+    Mu.arrowShapeImpl = function(e) {
+        return (_u || (_u = {
+            polygon: Bu,
+            "triangle-backcurve": Nu,
+            "triangle-tee": zu,
+            "circle-triangle": Iu,
+            "triangle-cross": zu,
+            circle: Au
         }))[e]
     };
-    var du = {
+    var Lu = {
             drawElement: function(e, t, n, r, i, a) {
                 t.isNode() ? this.drawNode(e, t, n, r, i, a) : this.drawEdge(e, t, n, r, i, a)
             },
             drawElementOverlay: function(e, t) {
                 t.isNode() ? this.drawNodeOverlay(e, t) : this.drawEdgeOverlay(e, t)
             },
             drawElementUnderlay: function(e, t) {
@@ -14731,71 +14914,71 @@
                             h = C.x, p = C.y
                         } else h = b, p = x;
                         1 !== d && (y = e.globalAlpha, e.globalAlpha = y * d), e.drawImage(c.texture.canvas, c.x, 0, c.width, c.height, h, p, w, E), 1 !== d && (e.globalAlpha = y), 0 !== m && (e.rotate(-m), e.translate(-f, -g), v || l.setImgSmoothing(e, !1))
                     } else n.drawElement(e, t)
                 }
             }
         },
-        hu = function() {
+        Ou = function() {
             return 0
         },
-        pu = function(e, t) {
+        Ru = function(e, t) {
             return e.getTextAngle(t, null)
         },
-        fu = function(e, t) {
+        Vu = function(e, t) {
             return e.getTextAngle(t, "source")
         },
-        gu = function(e, t) {
+        Fu = function(e, t) {
             return e.getTextAngle(t, "target")
         },
-        vu = function(e, t) {
+        ju = function(e, t) {
             return t.effectiveOpacity()
         },
-        yu = function(e, t) {
+        qu = function(e, t) {
             return t.pstyle("text-opacity").pfValue * t.effectiveOpacity()
         };
-    du.drawCachedElement = function(e, t, n, r, i, a) {
+    Lu.drawCachedElement = function(e, t, n, r, i, a) {
         var o = this,
             s = o.data,
             l = s.eleTxrCache,
             u = s.lblTxrCache,
             c = s.slbTxrCache,
             d = s.tlbTxrCache,
             h = t.boundingBox(),
             p = !0 === a ? l.reasons.highQuality : null;
-        if (0 !== h.w && 0 !== h.h && t.visible() && (!r || zt(h, r))) {
+        if (0 !== h.w && 0 !== h.h && t.visible() && (!r || It(h, r))) {
             var f = t.isEdge(),
                 g = t.element()._private.rscratch.badLine;
-            o.drawElementUnderlay(e, t), o.drawCachedElementPortion(e, t, l, n, i, p, hu, vu), f && g || o.drawCachedElementPortion(e, t, u, n, i, p, pu, yu), f && !g && (o.drawCachedElementPortion(e, t, c, n, i, p, fu, yu), o.drawCachedElementPortion(e, t, d, n, i, p, gu, yu)), o.drawElementOverlay(e, t)
+            o.drawElementUnderlay(e, t), o.drawCachedElementPortion(e, t, l, n, i, p, Ou, ju), f && g || o.drawCachedElementPortion(e, t, u, n, i, p, Ru, qu), f && !g && (o.drawCachedElementPortion(e, t, c, n, i, p, Vu, qu), o.drawCachedElementPortion(e, t, d, n, i, p, Fu, qu)), o.drawElementOverlay(e, t)
         }
-    }, du.drawElements = function(e, t) {
+    }, Lu.drawElements = function(e, t) {
         for (var n = 0; n < t.length; n++) {
             var r = t[n];
             this.drawElement(e, r)
         }
-    }, du.drawCachedElements = function(e, t, n, r) {
+    }, Lu.drawCachedElements = function(e, t, n, r) {
         for (var i = 0; i < t.length; i++) {
             var a = t[i];
             this.drawCachedElement(e, a, n, r)
         }
-    }, du.drawCachedNodes = function(e, t, n, r) {
+    }, Lu.drawCachedNodes = function(e, t, n, r) {
         for (var i = 0; i < t.length; i++) {
             var a = t[i];
             a.isNode() && this.drawCachedElement(e, a, n, r)
         }
-    }, du.drawLayeredElements = function(e, t, n, r) {
+    }, Lu.drawLayeredElements = function(e, t, n, r) {
         var i = this.data.lyrTxrCache.getLayers(t, n);
         if (i)
             for (var a = 0; a < i.length; a++) {
                 var o = i[a],
                     s = o.bb;
                 0 !== s.w && 0 !== s.h && e.drawImage(o.canvas, s.x1, s.y1, s.w, s.h)
             } else this.drawCachedElements(e, t, n, r)
     };
-    var mu = {
+    var Yu = {
             drawEdge: function(e, t, n) {
                 var r = !(arguments.length > 3 && void 0 !== arguments[3]) || arguments[3],
                     i = !(arguments.length > 4 && void 0 !== arguments[4]) || arguments[4],
                     a = !(arguments.length > 5 && void 0 !== arguments[5]) || arguments[5],
                     o = this,
                     s = t._private.rscratch;
                 if ((!a || t.visible()) && !s.badLine && null != s.allpts && !isNaN(s.allpts[0])) {
@@ -14835,15 +15018,15 @@
                             P = g * S;
                         e.translate(k, C), y(P), x(P), e.translate(-k, -C)
                     }
                     b(), y(), x(), m(), w(), n && e.translate(l.x1, l.y1)
                 }
             }
         },
-        bu = function(e) {
+        Xu = function(e) {
             if (!["overlay", "underlay"].includes(e)) throw new Error("Invalid state");
             return function(t, n) {
                 if (n.visible()) {
                     var r = n.pstyle("".concat(e, "-opacity")).value;
                     if (0 !== r) {
                         var i = this,
                             a = i.usePaths(),
@@ -14851,62 +15034,123 @@
                             s = 2 * n.pstyle("".concat(e, "-padding")).pfValue,
                             l = n.pstyle("".concat(e, "-color")).value;
                         t.lineWidth = s, "self" !== o.edgeType || a ? t.lineCap = "round" : t.lineCap = "butt", i.colorStrokeStyle(t, l[0], l[1], l[2], r), i.drawEdgePath(n, t, o.allpts, "solid")
                     }
                 }
             }
         };
-    mu.drawEdgeOverlay = bu("overlay"), mu.drawEdgeUnderlay = bu("underlay"), mu.drawEdgePath = function(e, t, n, r) {
+    Yu.drawEdgeOverlay = Xu("overlay"), Yu.drawEdgeUnderlay = Xu("underlay"), Yu.drawEdgePath = function(e, t, n, r) {
         var i, a = e._private.rscratch,
-            o = t,
-            s = !1,
-            l = this.usePaths(),
-            u = e.pstyle("line-dash-pattern").pfValue,
-            c = e.pstyle("line-dash-offset").pfValue;
-        if (l) {
-            var d = n.join("$");
-            a.pathCacheKey && a.pathCacheKey === d ? (i = t = a.pathCache, s = !0) : (i = t = new Path2D, a.pathCacheKey = d, a.pathCache = i)
+            s = t,
+            l = !1,
+            u = this.usePaths(),
+            c = e.pstyle("line-dash-pattern").pfValue,
+            d = e.pstyle("line-dash-offset").pfValue;
+        if (u) {
+            var h = n.join("$");
+            a.pathCacheKey && a.pathCacheKey === h ? (i = t = a.pathCache, l = !0) : (i = t = new Path2D, a.pathCacheKey = h, a.pathCache = i)
         }
-        if (o.setLineDash) switch (r) {
+        if (s.setLineDash) switch (r) {
             case "dotted":
-                o.setLineDash([1, 1]);
+                s.setLineDash([1, 1]);
                 break;
             case "dashed":
-                o.setLineDash(u), o.lineDashOffset = c;
+                s.setLineDash(c), s.lineDashOffset = d;
                 break;
             case "solid":
-                o.setLineDash([])
+                s.setLineDash([])
         }
-        if (!s && !a.badLine) switch (t.beginPath && t.beginPath(), t.moveTo(n[0], n[1]), a.edgeType) {
+        if (!l && !a.badLine) switch (t.beginPath && t.beginPath(), t.moveTo(n[0], n[1]), a.edgeType) {
             case "bezier":
             case "self":
             case "compound":
             case "multibezier":
-                for (var h = 2; h + 3 < n.length; h += 4) t.quadraticCurveTo(n[h], n[h + 1], n[h + 2], n[h + 3]);
+                for (var p = 2; p + 3 < n.length; p += 4) t.quadraticCurveTo(n[p], n[p + 1], n[p + 2], n[p + 3]);
                 break;
             case "straight":
-            case "segments":
             case "haystack":
-                for (var p = 2; p + 1 < n.length; p += 2) t.lineTo(n[p], n[p + 1])
+                for (var f = 2; f + 1 < n.length; f += 2) t.lineTo(n[f], n[f + 1]);
+                break;
+            case "segments":
+                if (a.isRound) {
+                    var g, v = function(e, t) {
+                        var n = "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
+                        if (!n) {
+                            if (Array.isArray(e) || (n = o(e)) || t && e && "number" == typeof e.length) {
+                                n && (e = n);
+                                var r = 0,
+                                    i = function() {};
+                                return {
+                                    s: i,
+                                    n: function() {
+                                        return r >= e.length ? {
+                                            done: !0
+                                        } : {
+                                            done: !1,
+                                            value: e[r++]
+                                        }
+                                    },
+                                    e: function(e) {
+                                        throw e
+                                    },
+                                    f: i
+                                }
+                            }
+                            throw new TypeError("Invalid attempt to iterate non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
+                        }
+                        var a, s = !0,
+                            l = !1;
+                        return {
+                            s: function() {
+                                n = n.call(e)
+                            },
+                            n: function() {
+                                var e = n.next();
+                                return s = e.done, e
+                            },
+                            e: function(e) {
+                                l = !0, a = e
+                            },
+                            f: function() {
+                                try {
+                                    s || null == n.return || n.return()
+                                } finally {
+                                    if (l) throw a
+                                }
+                            }
+                        }
+                    }(a.roundCorners);
+                    try {
+                        for (v.s(); !(g = v.n()).done;) {
+                            $l(t, g.value)
+                        }
+                    } catch (e) {
+                        v.e(e)
+                    } finally {
+                        v.f()
+                    }
+                    t.lineTo(n[n.length - 2], n[n.length - 1])
+                } else
+                    for (var y = 2; y + 1 < n.length; y += 2) t.lineTo(n[y], n[y + 1])
         }
-        t = o, l ? t.stroke(i) : t.stroke(), t.setLineDash && t.setLineDash([])
-    }, mu.drawEdgeTrianglePath = function(e, t, n) {
+        t = s, u ? t.stroke(i) : t.stroke(), t.setLineDash && t.setLineDash([])
+    }, Yu.drawEdgeTrianglePath = function(e, t, n) {
         t.fillStyle = t.strokeStyle;
         for (var r = e.pstyle("width").pfValue, i = 0; i + 1 < n.length; i += 2) {
             var a = [n[i + 2] - n[i], n[i + 3] - n[i + 1]],
                 o = Math.sqrt(a[0] * a[0] + a[1] * a[1]),
                 s = [a[1] / o, -a[0] / o],
                 l = [s[0] * r / 2, s[1] * r / 2];
             t.beginPath(), t.moveTo(n[i] - l[0], n[i + 1] - l[1]), t.lineTo(n[i] + l[0], n[i + 1] + l[1]), t.lineTo(n[i + 2], n[i + 3]), t.closePath(), t.fill()
         }
-    }, mu.drawArrowheads = function(e, t, n) {
+    }, Yu.drawArrowheads = function(e, t, n) {
         var r = t._private.rscratch,
             i = "haystack" === r.edgeType;
         i || this.drawArrowhead(e, t, "source", r.arrowStartX, r.arrowStartY, r.srcArrowAngle, n), this.drawArrowhead(e, t, "mid-target", r.midX, r.midY, r.midtgtArrowAngle, n), this.drawArrowhead(e, t, "mid-source", r.midX, r.midY, r.midsrcArrowAngle, n), i || this.drawArrowhead(e, t, "target", r.arrowEndX, r.arrowEndY, r.tgtArrowAngle, n)
-    }, mu.drawArrowhead = function(e, t, n, r, i, a, o) {
+    }, Yu.drawArrowhead = function(e, t, n, r, i, a, o) {
         if (!(isNaN(r) || null == r || isNaN(i) || null == i || isNaN(a) || null == a)) {
             var s = t.pstyle(n + "-arrow-shape").value;
             if ("none" !== s) {
                 var l = "hollow" === t.pstyle(n + "-arrow-fill").value ? "both" : "filled",
                     u = t.pstyle(n + "-arrow-fill").value,
                     c = t.pstyle("width").pfValue,
                     d = t.pstyle(n + "-arrow-width"),
@@ -14916,43 +15160,43 @@
                 void 0 === o && (o = p);
                 var f = e.globalCompositeOperation;
                 1 === o && "hollow" !== u || (e.globalCompositeOperation = "destination-out", this.colorFillStyle(e, 255, 255, 255, 1), this.colorStrokeStyle(e, 255, 255, 255, 1), this.drawArrowShape(t, e, l, c, s, h, r, i, a), e.globalCompositeOperation = f);
                 var g = t.pstyle(n + "-arrow-color").value;
                 this.colorFillStyle(e, g[0], g[1], g[2], o), this.colorStrokeStyle(e, g[0], g[1], g[2], o), this.drawArrowShape(t, e, u, c, s, h, r, i, a)
             }
         }
-    }, mu.drawArrowShape = function(e, t, n, r, i, a, o, s, l) {
+    }, Yu.drawArrowShape = function(e, t, n, r, i, a, o, s, l) {
         var u, c = this,
             d = this.usePaths() && "triangle-cross" !== i,
             h = !1,
             p = t,
             f = {
                 x: o,
                 y: s
             },
             g = e.pstyle("arrow-scale").value,
             v = this.getArrowWidth(r, g),
             y = c.arrowShapes[i];
         if (d) {
             var m = c.arrowPathCache = c.arrowPathCache || [],
-                b = Pe(i),
+                b = De(i),
                 x = m[b];
             null != x ? (u = t = x, h = !0) : (u = t = new Path2D, m[b] = u)
         }
         h || (t.beginPath && t.beginPath(), d ? y.draw(t, 1, 0, {
             x: 0,
             y: 0
         }, 1) : y.draw(t, v, l, f, r), t.closePath && t.closePath()), t = p, d && (t.translate(o, s), t.rotate(l), t.scale(v, v)), "filled" !== n && "both" !== n || (d ? t.fill(u) : t.fill()), "hollow" !== n && "both" !== n || (t.lineWidth = a / (d ? v : 1), t.lineJoin = "miter", d ? t.stroke(u) : t.stroke()), d && (t.scale(1 / v, 1 / v), t.rotate(-l), t.translate(-o, -s))
     };
-    var xu = {
+    var Wu = {
             safeDrawImage: function(e, t, n, r, i, a, o, s, l, u) {
                 if (!(i <= 0 || a <= 0 || l <= 0 || u <= 0)) try {
                     e.drawImage(t, n, r, i, a, o, s, l, u)
                 } catch (e) {
-                    Ve(e)
+                    Fe(e)
                 }
             },
             drawInscribedImage: function(e, t, n, r, i) {
                 var a = this,
                     o = n.position(),
                     s = o.x,
                     l = o.y,
@@ -14965,68 +15209,70 @@
                     g = 2 * n.padding(),
                     v = p + ("inner" === c(n, "background-width-relative-to", "value", r) ? 0 : g),
                     y = f + ("inner" === c(n, "background-height-relative-to", "value", r) ? 0 : g),
                     m = n._private.rscratch,
                     b = "node" === c(n, "background-clip", "value", r),
                     x = c(n, "background-image-opacity", "value", r) * i,
                     w = c(n, "background-image-smoothing", "value", r),
-                    E = t.width || t.cachedW,
-                    k = t.height || t.cachedH;
-                null != E && null != k || (document.body.appendChild(t), E = t.cachedW = t.width || t.offsetWidth, k = t.cachedH = t.height || t.offsetHeight, document.body.removeChild(t));
-                var C = E,
-                    S = k;
-                if ("auto" !== c(n, "background-width", "value", r) && (C = "%" === c(n, "background-width", "units", r) ? c(n, "background-width", "pfValue", r) * v : c(n, "background-width", "pfValue", r)), "auto" !== c(n, "background-height", "value", r) && (S = "%" === c(n, "background-height", "units", r) ? c(n, "background-height", "pfValue", r) * y : c(n, "background-height", "pfValue", r)), 0 !== C && 0 !== S) {
-                    if ("contain" === d) C *= P = Math.min(v / C, y / S), S *= P;
+                    E = n.pstyle("corner-radius").value;
+                "auto" !== E && (E = n.pstyle("corner-radius").pfValue);
+                var k = t.width || t.cachedW,
+                    C = t.height || t.cachedH;
+                null != k && null != C || (document.body.appendChild(t), k = t.cachedW = t.width || t.offsetWidth, C = t.cachedH = t.height || t.offsetHeight, document.body.removeChild(t));
+                var S = k,
+                    P = C;
+                if ("auto" !== c(n, "background-width", "value", r) && (S = "%" === c(n, "background-width", "units", r) ? c(n, "background-width", "pfValue", r) * v : c(n, "background-width", "pfValue", r)), "auto" !== c(n, "background-height", "value", r) && (P = "%" === c(n, "background-height", "units", r) ? c(n, "background-height", "pfValue", r) * y : c(n, "background-height", "pfValue", r)), 0 !== S && 0 !== P) {
+                    if ("contain" === d) S *= D = Math.min(v / S, y / P), P *= D;
                     else if ("cover" === d) {
-                        var P;
-                        C *= P = Math.max(v / C, y / S), S *= P
+                        var D;
+                        S *= D = Math.max(v / S, y / P), P *= D
                     }
-                    var D = s - v / 2,
-                        T = c(n, "background-position-x", "units", r),
-                        _ = c(n, "background-position-x", "pfValue", r);
-                    D += "%" === T ? (v - C) * _ : _;
-                    var M = c(n, "background-offset-x", "units", r),
-                        B = c(n, "background-offset-x", "pfValue", r);
-                    D += "%" === M ? (v - C) * B : B;
-                    var N = l - y / 2,
-                        z = c(n, "background-position-y", "units", r),
-                        I = c(n, "background-position-y", "pfValue", r);
-                    N += "%" === z ? (y - S) * I : I;
+                    var T = s - v / 2,
+                        _ = c(n, "background-position-x", "units", r),
+                        M = c(n, "background-position-x", "pfValue", r);
+                    T += "%" === _ ? (v - S) * M : M;
+                    var B = c(n, "background-offset-x", "units", r),
+                        N = c(n, "background-offset-x", "pfValue", r);
+                    T += "%" === B ? (v - S) * N : N;
+                    var z = l - y / 2,
+                        I = c(n, "background-position-y", "units", r),
+                        A = c(n, "background-position-y", "pfValue", r);
+                    z += "%" === I ? (y - P) * A : A;
                     var L = c(n, "background-offset-y", "units", r),
-                        A = c(n, "background-offset-y", "pfValue", r);
-                    N += "%" === L ? (y - S) * A : A, m.pathCache && (D -= s, N -= l, s = 0, l = 0);
-                    var O = e.globalAlpha;
+                        O = c(n, "background-offset-y", "pfValue", r);
+                    z += "%" === L ? (y - P) * O : O, m.pathCache && (T -= s, z -= l, s = 0, l = 0);
+                    var R = e.globalAlpha;
                     e.globalAlpha = x;
-                    var R = a.getImgSmoothing(e),
-                        V = !1;
-                    if ("no" === w && R ? (a.setImgSmoothing(e, !1), V = !0) : "yes" !== w || R || (a.setImgSmoothing(e, !0), V = !0), "no-repeat" === h) b && (e.save(), m.pathCache ? e.clip(m.pathCache) : (a.nodeShapes[a.getNodeShape(n)].draw(e, s, l, v, y), e.clip())), a.safeDrawImage(e, t, 0, 0, E, k, D, N, C, S), b && e.restore();
+                    var V = a.getImgSmoothing(e),
+                        F = !1;
+                    if ("no" === w && V ? (a.setImgSmoothing(e, !1), F = !0) : "yes" !== w || V || (a.setImgSmoothing(e, !0), F = !0), "no-repeat" === h) b && (e.save(), m.pathCache ? e.clip(m.pathCache) : (a.nodeShapes[a.getNodeShape(n)].draw(e, s, l, v, y, E, m), e.clip())), a.safeDrawImage(e, t, 0, 0, k, C, T, z, S, P), b && e.restore();
                     else {
-                        var F = e.createPattern(t, h);
-                        e.fillStyle = F, a.nodeShapes[a.getNodeShape(n)].draw(e, s, l, v, y), e.translate(D, N), e.fill(), e.translate(-D, -N)
+                        var j = e.createPattern(t, h);
+                        e.fillStyle = j, a.nodeShapes[a.getNodeShape(n)].draw(e, s, l, v, y, E, m), e.translate(T, z), e.fill(), e.translate(-T, -z)
                     }
-                    e.globalAlpha = O, V && a.setImgSmoothing(e, R)
+                    e.globalAlpha = R, F && a.setImgSmoothing(e, V)
                 }
             }
         },
-        wu = {};
+        Hu = {};
 
-    function Eu(e, t, n, r, i) {
+    function Ku(e, t, n, r, i) {
         var a = arguments.length > 5 && void 0 !== arguments[5] ? arguments[5] : 5,
             o = arguments.length > 6 ? arguments[6] : void 0;
         e.beginPath(), e.moveTo(t + a, n), e.lineTo(t + r - a, n), e.quadraticCurveTo(t + r, n, t + r, n + a), e.lineTo(t + r, n + i - a), e.quadraticCurveTo(t + r, n + i, t + r - a, n + i), e.lineTo(t + a, n + i), e.quadraticCurveTo(t, n + i, t, n + i - a), e.lineTo(t, n + a), e.quadraticCurveTo(t, n, t + a, n), e.closePath(), o ? e.stroke() : e.fill()
     }
-    wu.eleTextBiggerThanMin = function(e, t) {
+    Hu.eleTextBiggerThanMin = function(e, t) {
         if (!t) {
             var n = e.cy().zoom(),
                 r = this.getPixelRatio(),
-                i = Math.ceil(bt(n * r));
+                i = Math.ceil(xt(n * r));
             t = Math.pow(2, i)
         }
         return !(e.pstyle("font-size").pfValue * t < e.pstyle("min-zoomed-font-size").pfValue)
-    }, wu.drawElementText = function(e, t, n, r, i) {
+    }, Hu.drawElementText = function(e, t, n, r, i) {
         var a = !(arguments.length > 5 && void 0 !== arguments[5]) || arguments[5],
             o = this;
         if (null == r) {
             if (a && !o.eleTextBiggerThanMin(t)) return
         } else if (!1 === r) return;
         if (t.isNode()) {
             var s = t.pstyle("label");
@@ -15039,55 +15285,55 @@
                 d = t.pstyle("source-label"),
                 h = t.pstyle("target-label");
             if (u || (!c || !c.value) && (!d || !d.value) && (!h || !h.value)) return;
             e.textAlign = "center", e.textBaseline = "bottom"
         }
         var p, f = !n;
         n && (p = n, e.translate(-p.x1, -p.y1)), null == i ? (o.drawText(e, t, null, f, a), t.isEdge() && (o.drawText(e, t, "source", f, a), o.drawText(e, t, "target", f, a))) : o.drawText(e, t, i, f, a), n && e.translate(p.x1, p.y1)
-    }, wu.getFontCache = function(e) {
+    }, Hu.getFontCache = function(e) {
         var t;
         this.fontCaches = this.fontCaches || [];
         for (var n = 0; n < this.fontCaches.length; n++)
             if ((t = this.fontCaches[n]).context === e) return t;
         return t = {
             context: e
         }, this.fontCaches.push(t), t
-    }, wu.setupTextStyle = function(e, t) {
+    }, Hu.setupTextStyle = function(e, t) {
         var n = !(arguments.length > 2 && void 0 !== arguments[2]) || arguments[2],
             r = t.pstyle("font-style").strValue,
             i = t.pstyle("font-size").pfValue + "px",
             a = t.pstyle("font-family").strValue,
             o = t.pstyle("font-weight").strValue,
             s = n ? t.effectiveOpacity() * t.pstyle("text-opacity").value : 1,
             l = t.pstyle("text-outline-opacity").value * s,
             u = t.pstyle("color").value,
             c = t.pstyle("text-outline-color").value;
         e.font = r + " " + o + " " + i + " " + a, e.lineJoin = "round", this.colorFillStyle(e, u[0], u[1], u[2], s), this.colorStrokeStyle(e, c[0], c[1], c[2], l)
-    }, wu.getTextAngle = function(e, t) {
+    }, Hu.getTextAngle = function(e, t) {
         var n = e._private.rscratch,
             r = t ? t + "-" : "",
             i = e.pstyle(r + "text-rotation"),
-            a = Ke(n, "labelAngle", t);
+            a = Ge(n, "labelAngle", t);
         return "autorotate" === i.strValue ? e.isEdge() ? a : 0 : "none" === i.strValue ? 0 : i.pfValue
-    }, wu.drawText = function(e, t, n) {
+    }, Hu.drawText = function(e, t, n) {
         var r = !(arguments.length > 3 && void 0 !== arguments[3]) || arguments[3],
             i = !(arguments.length > 4 && void 0 !== arguments[4]) || arguments[4],
             a = t._private,
             o = a.rscratch,
             s = i ? t.effectiveOpacity() : 1;
         if (!i || 0 !== s && 0 !== t.pstyle("text-opacity").value) {
             "main" === n && (n = null);
-            var l, u, c = Ke(o, "labelX", n),
-                d = Ke(o, "labelY", n),
+            var l, u, c = Ge(o, "labelX", n),
+                d = Ge(o, "labelY", n),
                 h = this.getLabelText(t, n);
             if (null != h && "" !== h && !isNaN(c) && !isNaN(d)) {
                 this.setupTextStyle(e, t, i);
                 var p, f = n ? n + "-" : "",
-                    g = Ke(o, "labelWidth", n),
-                    v = Ke(o, "labelHeight", n),
+                    g = Ge(o, "labelWidth", n),
+                    v = Ge(o, "labelHeight", n),
                     y = t.pstyle(f + "text-margin-x").pfValue,
                     m = t.pstyle(f + "text-margin-y").pfValue,
                     b = t.isEdge(),
                     x = t.pstyle("text-halign").value,
                     w = t.pstyle("text-valign").value;
                 switch (b && (x = "center", w = "center"), c += y, d += m, 0 !== (p = r ? this.getTextAngle(t, n) : 0) && (l = c, u = d, e.translate(l, u), e.rotate(p), c = 0, d = 0), w) {
                     case "top":
@@ -15116,19 +15362,19 @@
                     }
                     var M = d - v - S,
                         B = g + 2 * S,
                         N = v + 2 * S;
                     if (E > 0) {
                         var z = e.fillStyle,
                             I = t.pstyle("text-background-color").value;
-                        e.fillStyle = "rgba(" + I[0] + "," + I[1] + "," + I[2] + "," + E * s + ")", D ? Eu(e, _, M, B, N, T) : e.fillRect(_, M, B, N), e.fillStyle = z
+                        e.fillStyle = "rgba(" + I[0] + "," + I[1] + "," + I[2] + "," + E * s + ")", D ? Ku(e, _, M, B, N, T) : e.fillRect(_, M, B, N), e.fillStyle = z
                     }
                     if (C > 0 && k > 0) {
-                        var L = e.strokeStyle,
-                            A = e.lineWidth,
+                        var A = e.strokeStyle,
+                            L = e.lineWidth,
                             O = t.pstyle("text-border-color").value,
                             R = t.pstyle("text-border-style").value;
                         if (e.strokeStyle = "rgba(" + O[0] + "," + O[1] + "," + O[2] + "," + k * s + ")", e.lineWidth = C, e.setLineDash) switch (R) {
                             case "dotted":
                                 e.setLineDash([1, 1]);
                                 break;
                             case "dashed":
@@ -15136,25 +15382,25 @@
                                 break;
                             case "double":
                                 e.lineWidth = C / 4, e.setLineDash([]);
                                 break;
                             case "solid":
                                 e.setLineDash([])
                         }
-                        if (D ? Eu(e, _, M, B, N, T, "stroke") : e.strokeRect(_, M, B, N), "double" === R) {
+                        if (D ? Ku(e, _, M, B, N, T, "stroke") : e.strokeRect(_, M, B, N), "double" === R) {
                             var V = C / 2;
-                            D ? Eu(e, _ + V, M + V, B - 2 * V, N - 2 * V, T, "stroke") : e.strokeRect(_ + V, M + V, B - 2 * V, N - 2 * V)
+                            D ? Ku(e, _ + V, M + V, B - 2 * V, N - 2 * V, T, "stroke") : e.strokeRect(_ + V, M + V, B - 2 * V, N - 2 * V)
                         }
-                        e.setLineDash && e.setLineDash([]), e.lineWidth = A, e.strokeStyle = L
+                        e.setLineDash && e.setLineDash([]), e.lineWidth = L, e.strokeStyle = A
                     }
                 }
                 var F = 2 * t.pstyle("text-outline-width").pfValue;
                 if (F > 0 && (e.lineWidth = F), "wrap" === t.pstyle("text-wrap").value) {
-                    var j = Ke(o, "labelWrapCachedLines", n),
-                        q = Ke(o, "labelLineHeight", n),
+                    var j = Ge(o, "labelWrapCachedLines", n),
+                        q = Ge(o, "labelLineHeight", n),
                         Y = g / 2,
                         X = this.getLabelJustification(t);
                     switch ("auto" === X || ("left" === x ? "left" === X ? c += -g : "center" === X && (c += -Y) : "center" === x ? "left" === X ? c += -Y : "right" === X && (c += Y) : "right" === x && ("center" === X ? c += Y : "right" === X && (c += g))), w) {
                         case "top":
                             d -= (j.length - 1) * q;
                             break;
                         case "center":
@@ -15163,132 +15409,146 @@
                     }
                     for (var W = 0; W < j.length; W++) F > 0 && e.strokeText(j[W], c, d), e.fillText(j[W], c, d), d += q
                 } else F > 0 && e.strokeText(h, c, d), e.fillText(h, c, d);
                 0 !== p && (e.rotate(-p), e.translate(-l, -u))
             }
         }
     };
-    var ku = {
+    var Gu = {
             drawNode: function(e, t, n) {
                 var r, i, a = !(arguments.length > 3 && void 0 !== arguments[3]) || arguments[3],
                     o = !(arguments.length > 4 && void 0 !== arguments[4]) || arguments[4],
                     s = !(arguments.length > 5 && void 0 !== arguments[5]) || arguments[5],
                     l = this,
                     u = t._private,
                     c = u.rscratch,
                     d = t.position();
-                if (m(d.x) && m(d.y) && (!s || t.visible())) {
+                if (b(d.x) && b(d.y) && (!s || t.visible())) {
                     var h, p, f = s ? t.effectiveOpacity() : 1,
                         g = l.usePaths(),
                         v = !1,
                         y = t.padding();
                     r = t.width() + 2 * y, i = t.height() + 2 * y, n && (p = n, e.translate(-p.x1, -p.y1));
-                    for (var b = t.pstyle("background-image"), x = b.value, w = new Array(x.length), E = new Array(x.length), k = 0, C = 0; C < x.length; C++) {
+                    for (var m = t.pstyle("background-image"), x = m.value, w = new Array(x.length), E = new Array(x.length), k = 0, C = 0; C < x.length; C++) {
                         var S = x[C],
                             P = w[C] = null != S && "none" !== S;
                         if (P) {
                             var D = t.cy().style().getIndexedStyle(t, "background-image-crossorigin", "value", C);
                             k++, E[C] = l.getCachedImage(S, D, (function() {
                                 u.backgroundTimestamp = Date.now(), t.emitAndNotify("background")
                             }))
                         }
                     }
                     var T = t.pstyle("background-blacken").value,
                         _ = t.pstyle("border-width").pfValue,
                         M = t.pstyle("background-opacity").value * f,
                         B = t.pstyle("border-color").value,
                         N = t.pstyle("border-style").value,
-                        z = t.pstyle("border-opacity").value * f,
-                        I = t.pstyle("outline-width").pfValue,
-                        L = t.pstyle("outline-color").value,
-                        A = t.pstyle("outline-style").value,
-                        O = t.pstyle("outline-opacity").value * f,
-                        R = t.pstyle("outline-offset").value;
-                    e.lineJoin = "miter";
-                    var V = function() {
+                        z = t.pstyle("border-join").value,
+                        I = t.pstyle("border-cap").value,
+                        A = t.pstyle("border-position").value,
+                        L = t.pstyle("border-dash-pattern").pfValue,
+                        O = t.pstyle("border-dash-offset").pfValue,
+                        R = t.pstyle("border-opacity").value * f,
+                        V = t.pstyle("outline-width").pfValue,
+                        F = t.pstyle("outline-color").value,
+                        j = t.pstyle("outline-style").value,
+                        q = t.pstyle("outline-opacity").value * f,
+                        Y = t.pstyle("outline-offset").value,
+                        X = t.pstyle("corner-radius").value;
+                    "auto" !== X && (X = t.pstyle("corner-radius").pfValue);
+                    var W = function() {
                             var n = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : M;
                             l.eleFillStyle(e, t, n)
                         },
-                        F = function() {
-                            var t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : z;
+                        H = function() {
+                            var t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : R;
                             l.colorStrokeStyle(e, B[0], B[1], B[2], t)
                         },
-                        j = function() {
-                            var t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : O;
-                            l.colorStrokeStyle(e, L[0], L[1], L[2], t)
+                        K = function() {
+                            var t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : q;
+                            l.colorStrokeStyle(e, F[0], F[1], F[2], t)
                         },
-                        q = function(e, t, n, r) {
+                        G = function(e, t, n, r) {
                             var i, a = l.nodePathCache = l.nodePathCache || [],
-                                o = De("polygon" === n ? n + "," + r.join(",") : n, "" + t, "" + e),
+                                o = Te("polygon" === n ? n + "," + r.join(",") : n, "" + t, "" + e, "" + X),
                                 s = a[o],
                                 u = !1;
                             return null != s ? (i = s, u = !0, c.pathCache = i) : (i = new Path2D, a[o] = c.pathCache = i), {
                                 path: i,
                                 cacheHit: u
                             }
                         },
-                        Y = t.pstyle("shape").strValue,
-                        X = t.pstyle("shape-polygon-points").pfValue;
+                        U = t.pstyle("shape").strValue,
+                        Z = t.pstyle("shape-polygon-points").pfValue;
                     if (g) {
                         e.translate(d.x, d.y);
-                        var W = q(r, i, Y, X);
-                        h = W.path, v = W.cacheHit
+                        var $ = G(r, i, U, Z);
+                        h = $.path, v = $.cacheHit
                     }
-                    var H = function() {
+                    var Q = function() {
                             if (!v) {
                                 var n = d;
                                 g && (n = {
                                     x: 0,
                                     y: 0
-                                }), l.nodeShapes[l.getNodeShape(t)].draw(h || e, n.x, n.y, r, i)
+                                }), l.nodeShapes[l.getNodeShape(t)].draw(h || e, n.x, n.y, r, i, X, c)
                             }
                             g ? e.fill(h) : e.fill()
                         },
-                        K = function() {
+                        J = function() {
                             for (var n = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : f, r = !(arguments.length > 1 && void 0 !== arguments[1]) || arguments[1], i = u.backgrounding, a = 0, o = 0; o < E.length; o++) {
                                 var s = t.cy().style().getIndexedStyle(t, "background-image-containment", "value", o);
                                 r && "over" === s || !r && "inside" === s ? a++ : w[o] && E[o].complete && !E[o].error && (a++, l.drawInscribedImage(e, E[o], t, o, n))
                             }
                             u.backgrounding = !(a === k), i !== u.backgrounding && t.updateStyle(!1)
                         },
-                        G = function() {
+                        ee = function() {
                             var n = arguments.length > 0 && void 0 !== arguments[0] && arguments[0],
                                 a = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : f;
-                            l.hasPie(t) && (l.drawPie(e, t, a), n && (g || l.nodeShapes[l.getNodeShape(t)].draw(e, d.x, d.y, r, i)))
+                            l.hasPie(t) && (l.drawPie(e, t, a), n && (g || l.nodeShapes[l.getNodeShape(t)].draw(e, d.x, d.y, r, i, X, c)))
                         },
-                        U = function() {
+                        te = function() {
                             var t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : f,
                                 n = (T > 0 ? T : -T) * t,
                                 r = T > 0 ? 0 : 255;
                             0 !== T && (l.colorFillStyle(e, r, r, r, n), g ? e.fill(h) : e.fill())
                         },
-                        Z = function() {
+                        ne = function() {
                             if (_ > 0) {
-                                if (e.lineWidth = _, e.lineCap = "butt", e.setLineDash) switch (N) {
+                                if (e.lineWidth = _, e.lineCap = I, e.lineJoin = z, e.setLineDash) switch (N) {
                                     case "dotted":
                                         e.setLineDash([1, 1]);
                                         break;
                                     case "dashed":
-                                        e.setLineDash([4, 2]);
+                                        e.setLineDash(L), e.lineDashOffset = O;
                                         break;
                                     case "solid":
                                     case "double":
                                         e.setLineDash([])
                                 }
-                                if (g ? e.stroke(h) : e.stroke(), "double" === N) {
+                                if ("center" !== A) {
+                                    if (e.save(), e.lineWidth *= 2, "inside" === A) g ? e.clip(h) : e.clip();
+                                    else {
+                                        var t = new Path2D;
+                                        t.rect(-r / 2 - _, -i / 2 - _, r + 2 * _, i + 2 * _), t.addPath(h), e.clip(t, "evenodd")
+                                    }
+                                    g ? e.stroke(h) : e.stroke(), e.restore()
+                                } else g ? e.stroke(h) : e.stroke();
+                                if ("double" === N) {
                                     e.lineWidth = _ / 3;
-                                    var t = e.globalCompositeOperation;
-                                    e.globalCompositeOperation = "destination-out", g ? e.stroke(h) : e.stroke(), e.globalCompositeOperation = t
+                                    var n = e.globalCompositeOperation;
+                                    e.globalCompositeOperation = "destination-out", g ? e.stroke(h) : e.stroke(), e.globalCompositeOperation = n
                                 }
                                 e.setLineDash && e.setLineDash([])
                             }
                         },
-                        $ = function() {
-                            if (I > 0) {
-                                if (e.lineWidth = I, e.lineCap = "butt", e.setLineDash) switch (A) {
+                        re = function() {
+                            if (V > 0) {
+                                if (e.lineWidth = V, e.lineCap = "butt", e.setLineDash) switch (j) {
                                     case "dotted":
                                         e.setLineDash([1, 1]);
                                         break;
                                     case "dashed":
                                         e.setLineDash([4, 2]);
                                         break;
                                     case "solid":
@@ -15296,86 +15556,96 @@
                                         e.setLineDash([])
                                 }
                                 var n = d;
                                 g && (n = {
                                     x: 0,
                                     y: 0
                                 });
-                                var a, o = l.getNodeShape(t),
-                                    s = (r + _ + (I + R)) / r,
-                                    u = (i + _ + (I + R)) / i,
-                                    c = r * s,
-                                    h = i * u,
-                                    p = l.nodeShapes[o].points;
-                                if (g) a = q(c, h, o, p).path;
-                                if ("ellipse" === o) l.drawEllipsePath(a || e, n.x, n.y, c, h);
-                                else if (["round-diamond", "round-heptagon", "round-hexagon", "round-octagon", "round-pentagon", "round-polygon", "round-triangle", "round-tag"].includes(o)) {
-                                    var f = 0,
-                                        v = 0,
-                                        y = 0;
-                                    "round-diamond" === o ? f = 1.4 * (_ + R + I) : "round-heptagon" === o ? (f = 1.075 * (_ + R + I), y = -(_ / 2 + R + I) / 35) : "round-hexagon" === o ? f = 1.12 * (_ + R + I) : "round-pentagon" === o ? (f = 1.13 * (_ + R + I), y = -(_ / 2 + R + I) / 15) : "round-tag" === o ? (f = 1.12 * (_ + R + I), v = .07 * (_ / 2 + I + R)) : "round-triangle" === o && (f = (_ + R + I) * (Math.PI / 2), y = -(_ + R / 2 + I) / Math.PI), 0 !== f && (s = (r + f) / r, u = (i + f) / i), l.drawRoundPolygonPath(a || e, n.x + v, n.y + y, r * s, i * u, p)
-                                } else if (["roundrectangle", "round-rectangle"].includes(o)) l.drawRoundRectanglePath(a || e, n.x, n.y, c, h);
-                                else if (["cutrectangle", "cut-rectangle"].includes(o)) l.drawCutRectanglePath(a || e, n.x, n.y, c, h);
-                                else if (["bottomroundrectangle", "bottom-round-rectangle"].includes(o)) l.drawBottomRoundRectanglePath(a || e, n.x, n.y, c, h);
-                                else if ("barrel" === o) l.drawBarrelPath(a || e, n.x, n.y, c, h);
-                                else if (o.startsWith("polygon") || ["rhomboid", "right-rhomboid", "round-tag", "tag", "vee"].includes(o)) {
-                                    p = Yt(Xt(p, (_ + I + R) / r)), l.drawPolygonPath(a || e, n.x, n.y, r, i, p)
+                                var a = l.getNodeShape(t),
+                                    o = _;
+                                "inside" === A && (o = 0), "outside" === A && (o *= 2);
+                                var s, u = (r + o + (V + Y)) / r,
+                                    c = (i + o + (V + Y)) / i,
+                                    h = r * u,
+                                    p = i * c,
+                                    f = l.nodeShapes[a].points;
+                                if (g) s = G(h, p, a, f).path;
+                                if ("ellipse" === a) l.drawEllipsePath(s || e, n.x, n.y, h, p);
+                                else if (["round-diamond", "round-heptagon", "round-hexagon", "round-octagon", "round-pentagon", "round-polygon", "round-triangle", "round-tag"].includes(a)) {
+                                    var v = 0,
+                                        y = 0,
+                                        m = 0;
+                                    "round-diamond" === a ? v = 1.4 * (o + Y + V) : "round-heptagon" === a ? (v = 1.075 * (o + Y + V), m = -(o / 2 + Y + V) / 35) : "round-hexagon" === a ? v = 1.12 * (o + Y + V) : "round-pentagon" === a ? (v = 1.13 * (o + Y + V), m = -(o / 2 + Y + V) / 15) : "round-tag" === a ? (v = 1.12 * (o + Y + V), y = .07 * (o / 2 + V + Y)) : "round-triangle" === a && (v = (o + Y + V) * (Math.PI / 2), m = -(o + Y / 2 + V) / Math.PI), 0 !== v && (h = r * (u = (r + v) / r), ["round-hexagon", "round-tag"].includes(a) || (p = i * (c = (i + v) / i)));
+                                    for (var b = h / 2, x = p / 2, w = (X = "auto" === X ? nn(h, p) : X) + (o + V + Y) / 2, E = new Array(f.length / 2), k = new Array(f.length / 2), C = 0; C < f.length / 2; C++) E[C] = {
+                                        x: n.x + y + b * f[2 * C],
+                                        y: n.y + m + x * f[2 * C + 1]
+                                    };
+                                    var S, P, D, T, M = E.length;
+                                    for (P = E[M - 1], S = 0; S < M; S++) D = E[S % M], T = E[(S + 1) % M], k[S] = Ql(P, D, T, w), P = D, D = T;
+                                    l.drawRoundPolygonPath(s || e, n.x + y, n.y + m, r * u, i * c, f, k)
+                                } else if (["roundrectangle", "round-rectangle"].includes(a)) X = "auto" === X ? tn(h, p) : X, l.drawRoundRectanglePath(s || e, n.x, n.y, h, p, X + (o + V + Y) / 2);
+                                else if (["cutrectangle", "cut-rectangle"].includes(a)) X = "auto" === X ? 8 : X, l.drawCutRectanglePath(s || e, n.x, n.y, h, p, null, X + (o + V + Y) / 4);
+                                else if (["bottomroundrectangle", "bottom-round-rectangle"].includes(a)) X = "auto" === X ? tn(h, p) : X, l.drawBottomRoundRectanglePath(s || e, n.x, n.y, h, p, X + (o + V + Y) / 2);
+                                else if ("barrel" === a) l.drawBarrelPath(s || e, n.x, n.y, h, p);
+                                else if (a.startsWith("polygon") || ["rhomboid", "right-rhomboid", "round-tag", "tag", "vee"].includes(a)) {
+                                    f = Xt(Wt(f, (o + V + Y) / r)), l.drawPolygonPath(s || e, n.x, n.y, r, i, f)
                                 } else {
-                                    p = Yt(Xt(p, -((_ + I + R) / r))), l.drawPolygonPath(a || e, n.x, n.y, r, i, p)
+                                    f = Xt(Wt(f, -((o + V + Y) / r))), l.drawPolygonPath(s || e, n.x, n.y, r, i, f)
                                 }
-                                if (g ? e.stroke(a) : e.stroke(), "double" === A) {
-                                    e.lineWidth = _ / 3;
-                                    var m = e.globalCompositeOperation;
-                                    e.globalCompositeOperation = "destination-out", g ? e.stroke(a) : e.stroke(), e.globalCompositeOperation = m
+                                if (g ? e.stroke(s) : e.stroke(), "double" === j) {
+                                    e.lineWidth = o / 3;
+                                    var B = e.globalCompositeOperation;
+                                    e.globalCompositeOperation = "destination-out", g ? e.stroke(s) : e.stroke(), e.globalCompositeOperation = B
                                 }
                                 e.setLineDash && e.setLineDash([])
                             }
                         },
-                        Q = function() {
+                        ie = function() {
                             o && l.drawNodeOverlay(e, t, d, r, i)
                         },
-                        J = function() {
+                        ae = function() {
                             o && l.drawNodeUnderlay(e, t, d, r, i)
                         },
-                        ee = function() {
+                        oe = function() {
                             l.drawElementText(e, t, null, a)
                         },
-                        te = "yes" === t.pstyle("ghost").value;
-                    if (te) {
-                        var ne = t.pstyle("ghost-offset-x").pfValue,
-                            re = t.pstyle("ghost-offset-y").pfValue,
-                            ie = t.pstyle("ghost-opacity").value,
-                            ae = ie * f;
-                        e.translate(ne, re), j(), $(), V(ie * M), H(), K(ae, !0), F(ie * z), Z(), G(0 !== T || 0 !== _), K(ae, !1), U(ae), e.translate(-ne, -re)
+                        se = "yes" === t.pstyle("ghost").value;
+                    if (se) {
+                        var le = t.pstyle("ghost-offset-x").pfValue,
+                            ue = t.pstyle("ghost-offset-y").pfValue,
+                            ce = t.pstyle("ghost-opacity").value,
+                            de = ce * f;
+                        e.translate(le, ue), K(), re(), W(ce * M), Q(), J(de, !0), H(ce * R), ne(), ee(0 !== T || 0 !== _), J(de, !1), te(de), e.translate(-le, -ue)
                     }
-                    g && e.translate(-d.x, -d.y), J(), g && e.translate(d.x, d.y), j(), $(), V(), H(), K(f, !0), F(), Z(), G(0 !== T || 0 !== _), K(f, !1), U(), g && e.translate(-d.x, -d.y), ee(), Q(), n && e.translate(p.x1, p.y1)
+                    g && e.translate(-d.x, -d.y), ae(), g && e.translate(d.x, d.y), K(), re(), W(), Q(), J(f, !0), H(), ne(), ee(0 !== T || 0 !== _), J(f, !1), te(), g && e.translate(-d.x, -d.y), oe(), ie(), n && e.translate(p.x1, p.y1)
                 }
             }
         },
-        Cu = function(e) {
+        Uu = function(e) {
             if (!["overlay", "underlay"].includes(e)) throw new Error("Invalid state");
             return function(t, n, r, i, a) {
                 if (n.visible()) {
                     var o = n.pstyle("".concat(e, "-padding")).pfValue,
                         s = n.pstyle("".concat(e, "-opacity")).value,
                         l = n.pstyle("".concat(e, "-color")).value,
-                        u = n.pstyle("".concat(e, "-shape")).value;
+                        u = n.pstyle("".concat(e, "-shape")).value,
+                        c = n.pstyle("".concat(e, "-corner-radius")).value;
                     if (s > 0) {
                         if (r = r || n.position(), null == i || null == a) {
-                            var c = n.padding();
-                            i = n.width() + 2 * c, a = n.height() + 2 * c
+                            var d = n.padding();
+                            i = n.width() + 2 * d, a = n.height() + 2 * d
                         }
-                        this.colorFillStyle(t, l[0], l[1], l[2], s), this.nodeShapes[u].draw(t, r.x, r.y, i + 2 * o, a + 2 * o), t.fill()
+                        this.colorFillStyle(t, l[0], l[1], l[2], s), this.nodeShapes[u].draw(t, r.x, r.y, i + 2 * o, a + 2 * o, c), t.fill()
                     }
                 }
             }
         };
-    ku.drawNodeOverlay = Cu("overlay"), ku.drawNodeUnderlay = Cu("underlay"), ku.hasPie = function(e) {
+    Gu.drawNodeOverlay = Uu("overlay"), Gu.drawNodeUnderlay = Uu("underlay"), Gu.hasPie = function(e) {
         return (e = e[0])._private.hasPie
-    }, ku.drawPie = function(e, t, n, r) {
+    }, Gu.drawPie = function(e, t, n, r) {
         t = t[0], r = r || t.position();
         var i = t.cy().style(),
             a = t.pstyle("pie-size"),
             o = r.x,
             s = r.y,
             l = t.width(),
             u = t.height(),
@@ -15389,39 +15659,39 @@
                 v = p / 100;
             v + d > 1 && (v = 1 - d);
             var y = 1.5 * Math.PI + 2 * Math.PI * d,
                 m = y + 2 * Math.PI * v;
             0 === p || d >= 1 || d + v > 1 || (e.beginPath(), e.moveTo(o, s), e.arc(o, s, c, y, m), e.closePath(), this.colorFillStyle(e, f[0], f[1], f[2], g), e.fill(), d += v)
         }
     };
-    var Su = {};
-    Su.getPixelRatio = function() {
+    var Zu = {};
+    Zu.getPixelRatio = function() {
         var e = this.data.contexts[0];
         if (null != this.forcedPixelRatio) return this.forcedPixelRatio;
         var t = e.backingStorePixelRatio || e.webkitBackingStorePixelRatio || e.mozBackingStorePixelRatio || e.msBackingStorePixelRatio || e.oBackingStorePixelRatio || e.backingStorePixelRatio || 1;
         return (window.devicePixelRatio || 1) / t
-    }, Su.paintCache = function(e) {
+    }, Zu.paintCache = function(e) {
         for (var t, n = this.paintCaches = this.paintCaches || [], r = !0, i = 0; i < n.length; i++)
             if ((t = n[i]).context === e) {
                 r = !1;
                 break
             } return r && (t = {
             context: e
         }, n.push(t)), t
-    }, Su.createGradientStyleFor = function(e, t, n, r, i) {
+    }, Zu.createGradientStyleFor = function(e, t, n, r, i) {
         var a, o = this.usePaths(),
             s = n.pstyle(t + "-gradient-stop-colors").value,
             l = n.pstyle(t + "-gradient-stop-positions").pfValue;
         if ("radial-gradient" === r)
             if (n.isEdge()) {
                 var u = n.sourceEndpoint(),
                     c = n.targetEndpoint(),
                     d = n.midpoint(),
-                    h = wt(u, d),
-                    p = wt(c, d);
+                    h = Et(u, d),
+                    p = Et(c, d);
                 a = e.createRadialGradient(d.x, d.y, 0, d.x, d.y, Math.max(h, p))
             } else {
                 var f = o ? {
                         x: 0,
                         y: 0
                     } : n.position(),
                     g = n.paddedWidth(),
@@ -15468,41 +15738,41 @@
                 case "to-left-top":
                     a = e.createLinearGradient(b.x + x, b.y + w, b.x - x, b.y - w)
             }
         }
         if (!a) return null;
         for (var E = l.length === s.length, k = s.length, C = 0; C < k; C++) a.addColorStop(E ? l[C] : C / (k - 1), "rgba(" + s[C][0] + "," + s[C][1] + "," + s[C][2] + "," + i + ")");
         return a
-    }, Su.gradientFillStyle = function(e, t, n, r) {
+    }, Zu.gradientFillStyle = function(e, t, n, r) {
         var i = this.createGradientStyleFor(e, "background", t, n, r);
         if (!i) return null;
         e.fillStyle = i
-    }, Su.colorFillStyle = function(e, t, n, r, i) {
+    }, Zu.colorFillStyle = function(e, t, n, r, i) {
         e.fillStyle = "rgba(" + t + "," + n + "," + r + "," + i + ")"
-    }, Su.eleFillStyle = function(e, t, n) {
+    }, Zu.eleFillStyle = function(e, t, n) {
         var r = t.pstyle("background-fill").value;
         if ("linear-gradient" === r || "radial-gradient" === r) this.gradientFillStyle(e, t, r, n);
         else {
             var i = t.pstyle("background-color").value;
             this.colorFillStyle(e, i[0], i[1], i[2], n)
         }
-    }, Su.gradientStrokeStyle = function(e, t, n, r) {
+    }, Zu.gradientStrokeStyle = function(e, t, n, r) {
         var i = this.createGradientStyleFor(e, "line", t, n, r);
         if (!i) return null;
         e.strokeStyle = i
-    }, Su.colorStrokeStyle = function(e, t, n, r, i) {
+    }, Zu.colorStrokeStyle = function(e, t, n, r, i) {
         e.strokeStyle = "rgba(" + t + "," + n + "," + r + "," + i + ")"
-    }, Su.eleStrokeStyle = function(e, t, n) {
+    }, Zu.eleStrokeStyle = function(e, t, n) {
         var r = t.pstyle("line-fill").value;
         if ("linear-gradient" === r || "radial-gradient" === r) this.gradientStrokeStyle(e, t, r, n);
         else {
             var i = t.pstyle("line-color").value;
             this.colorStrokeStyle(e, i[0], i[1], i[2], n)
         }
-    }, Su.matchCanvasSize = function(e) {
+    }, Zu.matchCanvasSize = function(e) {
         var t = this,
             n = t.data,
             r = t.findContainerClientCoords(),
             i = r[2],
             a = r[3],
             o = t.getPixelRatio(),
             s = t.motionBlurPxRatio;
@@ -15513,24 +15783,24 @@
             t.fontCaches = null;
             var d = n.canvasContainer;
             d.style.width = i + "px", d.style.height = a + "px";
             for (var h = 0; h < t.CANVAS_LAYERS; h++)(l = n.canvases[h]).width = u, l.height = c, l.style.width = i + "px", l.style.height = a + "px";
             for (h = 0; h < t.BUFFER_COUNT; h++)(l = n.bufferCanvases[h]).width = u, l.height = c, l.style.width = i + "px", l.style.height = a + "px";
             t.textureMult = 1, o <= 1 && (l = n.bufferCanvases[t.TEXTURE_BUFFER], t.textureMult = 2, l.width = u * t.textureMult, l.height = c * t.textureMult), t.canvasWidth = u, t.canvasHeight = c
         }
-    }, Su.renderTo = function(e, t, n, r) {
+    }, Zu.renderTo = function(e, t, n, r) {
         this.render({
             forcedContext: e,
             forcedZoom: t,
             forcedPan: n,
             drawAllLayers: !0,
             forcedPxRatio: r
         })
-    }, Su.render = function(e) {
-        var t = (e = e || Ye()).forcedContext,
+    }, Zu.render = function(e) {
+        var t = (e = e || Xe()).forcedContext,
             n = e.drawAllLayers,
             r = e.drawOnlyNodeLayer,
             i = e.forcedZoom,
             a = e.forcedPan,
             o = this,
             s = void 0 === e.forcedPxRatio ? this.getPixelRatio() : e.forcedPxRatio,
             l = o.cy,
@@ -15602,23 +15872,23 @@
                 N = m.core("outside-texture-bg-opacity").value;
             o.colorFillStyle(_, B[0], B[1], B[2], N), _.fillRect(0, 0, k.width, k.height);
             b = l.zoom();
             D(_, !1), _.clearRect(k.mpan.x, k.mpan.y, k.width / k.zoom / s, k.height / k.zoom / s), _.drawImage(M, k.mpan.x, k.mpan.y, k.width / k.zoom / s, k.height / k.zoom / s)
         } else o.textureOnViewport && !t && (o.textureCache = null);
         var z = l.extent(),
             I = o.pinching || o.hoverData.dragging || o.swipePanning || o.data.wheelZooming || o.hoverData.draggingEles || o.cy.animated(),
-            L = o.hideEdgesOnViewport && I,
-            A = [];
-        if (A[o.NODE] = !c[o.NODE] && h && !o.clearedForMotionBlur[o.NODE] || o.clearingMotionBlur, A[o.NODE] && (o.clearedForMotionBlur[o.NODE] = !0), A[o.DRAG] = !c[o.DRAG] && h && !o.clearedForMotionBlur[o.DRAG] || o.clearingMotionBlur, A[o.DRAG] && (o.clearedForMotionBlur[o.DRAG] = !0), c[o.NODE] || n || r || A[o.NODE]) {
-            var O = h && !A[o.NODE] && 1 !== p;
-            D(_ = t || (O ? o.data.bufferContexts[o.MOTIONBLUR_BUFFER_NODE] : u.contexts[o.NODE]), h && !O ? "motionBlur" : void 0), L ? o.drawCachedNodes(_, S.nondrag, s, z) : o.drawLayeredElements(_, S.nondrag, s, z), o.debug && o.drawDebugPoints(_, S.nondrag), n || h || (c[o.NODE] = !1)
-        }
-        if (!r && (c[o.DRAG] || n || A[o.DRAG])) {
-            O = h && !A[o.DRAG] && 1 !== p;
-            D(_ = t || (O ? o.data.bufferContexts[o.MOTIONBLUR_BUFFER_DRAG] : u.contexts[o.DRAG]), h && !O ? "motionBlur" : void 0), L ? o.drawCachedNodes(_, S.drag, s, z) : o.drawCachedElements(_, S.drag, s, z), o.debug && o.drawDebugPoints(_, S.drag), n || h || (c[o.DRAG] = !1)
+            A = o.hideEdgesOnViewport && I,
+            L = [];
+        if (L[o.NODE] = !c[o.NODE] && h && !o.clearedForMotionBlur[o.NODE] || o.clearingMotionBlur, L[o.NODE] && (o.clearedForMotionBlur[o.NODE] = !0), L[o.DRAG] = !c[o.DRAG] && h && !o.clearedForMotionBlur[o.DRAG] || o.clearingMotionBlur, L[o.DRAG] && (o.clearedForMotionBlur[o.DRAG] = !0), c[o.NODE] || n || r || L[o.NODE]) {
+            var O = h && !L[o.NODE] && 1 !== p;
+            D(_ = t || (O ? o.data.bufferContexts[o.MOTIONBLUR_BUFFER_NODE] : u.contexts[o.NODE]), h && !O ? "motionBlur" : void 0), A ? o.drawCachedNodes(_, S.nondrag, s, z) : o.drawLayeredElements(_, S.nondrag, s, z), o.debug && o.drawDebugPoints(_, S.nondrag), n || h || (c[o.NODE] = !1)
+        }
+        if (!r && (c[o.DRAG] || n || L[o.DRAG])) {
+            O = h && !L[o.DRAG] && 1 !== p;
+            D(_ = t || (O ? o.data.bufferContexts[o.MOTIONBLUR_BUFFER_DRAG] : u.contexts[o.DRAG]), h && !O ? "motionBlur" : void 0), A ? o.drawCachedNodes(_, S.drag, s, z) : o.drawCachedElements(_, S.drag, s, z), o.debug && o.drawDebugPoints(_, S.drag), n || h || (c[o.DRAG] = !1)
         }
         if (o.showFps || !r && c[o.SELECT_BOX] && !n) {
             if (D(_ = t || u.contexts[o.SELECT_BOX]), 1 == o.selection[4] && (o.hoverData.selecting || o.touchData.selecting)) {
                 b = o.cy.zoom();
                 var R = m.core("selection-box-border-width").value / b;
                 _.lineWidth = R, _.fillStyle = "rgba(" + m.core("selection-box-color").value[0] + "," + m.core("selection-box-color").value[1] + "," + m.core("selection-box-color").value[2] + "," + m.core("selection-box-opacity").value + ")", _.fillRect(o.selection[0], o.selection[1], o.selection[2] - o.selection[0], o.selection[3] - o.selection[1]), R > 0 && (_.strokeStyle = "rgba(" + m.core("selection-box-border-color").value[0] + "," + m.core("selection-box-border-color").value[1] + "," + m.core("selection-box-border-color").value[2] + "," + m.core("selection-box-opacity").value + ")", _.strokeRect(o.selection[0], o.selection[1], o.selection[2] - o.selection[0], o.selection[3] - o.selection[1]))
             }
@@ -15642,138 +15912,124 @@
                 X = u.contexts[o.DRAG],
                 W = o.data.bufferCanvases[o.MOTIONBLUR_BUFFER_DRAG],
                 H = function(e, t, n) {
                     e.setTransform(1, 0, 0, 1, 0, 0), n || !y ? e.clearRect(0, 0, o.canvasWidth, o.canvasHeight) : P(e, 0, 0, o.canvasWidth, o.canvasHeight);
                     var r = p;
                     e.drawImage(t, 0, 0, o.canvasWidth * r, o.canvasHeight * r, 0, 0, o.canvasWidth, o.canvasHeight)
                 };
-            (c[o.NODE] || A[o.NODE]) && (H(q, Y, A[o.NODE]), c[o.NODE] = !1), (c[o.DRAG] || A[o.DRAG]) && (H(X, W, A[o.DRAG]), c[o.DRAG] = !1)
+            (c[o.NODE] || L[o.NODE]) && (H(q, Y, L[o.NODE]), c[o.NODE] = !1), (c[o.DRAG] || L[o.DRAG]) && (H(X, W, L[o.DRAG]), c[o.DRAG] = !1)
         }
         o.prevViewport = k, o.clearingMotionBlur && (o.clearingMotionBlur = !1, o.motionBlurCleared = !0, o.motionBlur = !0), h && (o.motionBlurTimeout = setTimeout((function() {
             o.motionBlurTimeout = null, o.clearedForMotionBlur[o.NODE] = !1, o.clearedForMotionBlur[o.DRAG] = !1, o.motionBlur = !1, o.clearingMotionBlur = !d, o.mbFrames = 0, c[o.NODE] = !0, c[o.DRAG] = !0, o.redraw()
         }), 100)), t || l.emit("render")
     };
-    for (var Pu = {
+    for (var $u = {
             drawPolygonPath: function(e, t, n, r, i, a) {
                 var o = r / 2,
                     s = i / 2;
                 e.beginPath && e.beginPath(), e.moveTo(t + o * a[0], n + s * a[1]);
                 for (var l = 1; l < a.length / 2; l++) e.lineTo(t + o * a[2 * l], n + s * a[2 * l + 1]);
                 e.closePath()
             },
-            drawRoundPolygonPath: function(e, t, n, r, i, a) {
+            drawRoundPolygonPath: function(e, t, n, r, i, a, o) {
+                o.forEach((function(t) {
+                    return $l(e, t)
+                })), e.closePath()
+            },
+            drawRoundRectanglePath: function(e, t, n, r, i, a) {
                 var o = r / 2,
                     s = i / 2,
-                    l = tn(r, i);
-                e.beginPath && e.beginPath();
-                for (var u = 0; u < a.length / 4; u++) {
-                    var c, d = void 0;
-                    d = 0 === u ? a.length - 2 : 4 * u - 2, c = 4 * u + 2;
-                    var h = t + o * a[4 * u],
-                        p = n + s * a[4 * u + 1],
-                        f = -a[d] * a[c] - a[d + 1] * a[c + 1],
-                        g = l / Math.tan(Math.acos(f) / 2),
-                        v = h - g * a[d],
-                        y = p - g * a[d + 1],
-                        m = h + g * a[c],
-                        b = p + g * a[c + 1];
-                    0 === u ? e.moveTo(v, y) : e.lineTo(v, y), e.arcTo(h, p, m, b, l)
-                }
-                e.closePath()
-            },
-            drawRoundRectanglePath: function(e, t, n, r, i) {
-                var a = r / 2,
-                    o = i / 2,
-                    s = en(r, i);
-                e.beginPath && e.beginPath(), e.moveTo(t, n - o), e.arcTo(t + a, n - o, t + a, n, s), e.arcTo(t + a, n + o, t, n + o, s), e.arcTo(t - a, n + o, t - a, n, s), e.arcTo(t - a, n - o, t, n - o, s), e.lineTo(t, n - o), e.closePath()
+                    l = "auto" === a ? tn(r, i) : Math.min(a, s, o);
+                e.beginPath && e.beginPath(), e.moveTo(t, n - s), e.arcTo(t + o, n - s, t + o, n, l), e.arcTo(t + o, n + s, t, n + s, l), e.arcTo(t - o, n + s, t - o, n, l), e.arcTo(t - o, n - s, t, n - s, l), e.lineTo(t, n - s), e.closePath()
             },
-            drawBottomRoundRectanglePath: function(e, t, n, r, i) {
-                var a = r / 2,
-                    o = i / 2,
-                    s = en(r, i);
-                e.beginPath && e.beginPath(), e.moveTo(t, n - o), e.lineTo(t + a, n - o), e.lineTo(t + a, n), e.arcTo(t + a, n + o, t, n + o, s), e.arcTo(t - a, n + o, t - a, n, s), e.lineTo(t - a, n - o), e.lineTo(t, n - o), e.closePath()
+            drawBottomRoundRectanglePath: function(e, t, n, r, i, a) {
+                var o = r / 2,
+                    s = i / 2,
+                    l = "auto" === a ? tn(r, i) : a;
+                e.beginPath && e.beginPath(), e.moveTo(t, n - s), e.lineTo(t + o, n - s), e.lineTo(t + o, n), e.arcTo(t + o, n + s, t, n + s, l), e.arcTo(t - o, n + s, t - o, n, l), e.lineTo(t - o, n - s), e.lineTo(t, n - s), e.closePath()
             },
-            drawCutRectanglePath: function(e, t, n, r, i) {
-                var a = r / 2,
-                    o = i / 2;
-                e.beginPath && e.beginPath(), e.moveTo(t - a + 8, n - o), e.lineTo(t + a - 8, n - o), e.lineTo(t + a, n - o + 8), e.lineTo(t + a, n + o - 8), e.lineTo(t + a - 8, n + o), e.lineTo(t - a + 8, n + o), e.lineTo(t - a, n + o - 8), e.lineTo(t - a, n - o + 8), e.closePath()
+            drawCutRectanglePath: function(e, t, n, r, i, a, o) {
+                var s = r / 2,
+                    l = i / 2,
+                    u = "auto" === o ? 8 : o;
+                e.beginPath && e.beginPath(), e.moveTo(t - s + u, n - l), e.lineTo(t + s - u, n - l), e.lineTo(t + s, n - l + u), e.lineTo(t + s, n + l - u), e.lineTo(t + s - u, n + l), e.lineTo(t - s + u, n + l), e.lineTo(t - s, n + l - u), e.lineTo(t - s, n - l + u), e.closePath()
             },
             drawBarrelPath: function(e, t, n, r, i) {
                 var a = r / 2,
                     o = i / 2,
                     s = t - a,
                     l = t + a,
                     u = n - o,
                     c = n + o,
-                    d = nn(r, i),
+                    d = rn(r, i),
                     h = d.widthOffset,
                     p = d.heightOffset,
                     f = d.ctrlPtOffsetPct * h;
                 e.beginPath && e.beginPath(), e.moveTo(s, u + p), e.lineTo(s, c - p), e.quadraticCurveTo(s + f, c, s + h, c), e.lineTo(l - h, c), e.quadraticCurveTo(l - f, c, l, c - p), e.lineTo(l, u + p), e.quadraticCurveTo(l - f, u, l - h, u), e.lineTo(s + h, u), e.quadraticCurveTo(s + f, u, s, u + p), e.closePath()
             }
-        }, Du = Math.sin(0), Tu = Math.cos(0), _u = {}, Mu = {}, Bu = Math.PI / 40, Nu = 0 * Math.PI; Nu < 2 * Math.PI; Nu += Bu) _u[Nu] = Math.sin(Nu), Mu[Nu] = Math.cos(Nu);
-    Pu.drawEllipsePath = function(e, t, n, r, i) {
+        }, Qu = Math.sin(0), Ju = Math.cos(0), ec = {}, tc = {}, nc = Math.PI / 40, rc = 0 * Math.PI; rc < 2 * Math.PI; rc += nc) ec[rc] = Math.sin(rc), tc[rc] = Math.cos(rc);
+    $u.drawEllipsePath = function(e, t, n, r, i) {
         if (e.beginPath && e.beginPath(), e.ellipse) e.ellipse(t, n, r / 2, i / 2, 0, 0, 2 * Math.PI);
         else
-            for (var a, o, s = r / 2, l = i / 2, u = 0 * Math.PI; u < 2 * Math.PI; u += Bu) a = t - s * _u[u] * Du + s * Mu[u] * Tu, o = n + l * Mu[u] * Du + l * _u[u] * Tu, 0 === u ? e.moveTo(a, o) : e.lineTo(a, o);
+            for (var a, o, s = r / 2, l = i / 2, u = 0 * Math.PI; u < 2 * Math.PI; u += nc) a = t - s * ec[u] * Qu + s * tc[u] * Ju, o = n + l * tc[u] * Qu + l * ec[u] * Ju, 0 === u ? e.moveTo(a, o) : e.lineTo(a, o);
         e.closePath()
     };
-    var zu = {};
+    var ic = {};
 
-    function Iu(e) {
+    function ac(e) {
         var t = e.indexOf(",");
         return e.substr(t + 1)
     }
 
-    function Lu(e, t, n) {
+    function oc(e, t, n) {
         var r = function() {
             return t.toDataURL(n, e.quality)
         };
         switch (e.output) {
             case "blob-promise":
-                return new pr((function(r, i) {
+                return new gr((function(r, i) {
                     try {
                         t.toBlob((function(e) {
                             null != e ? r(e) : i(new Error("`canvas.toBlob()` sent a null value in its callback"))
                         }), n, e.quality)
                     } catch (e) {
                         i(e)
                     }
                 }));
             case "blob":
                 return function(e, t) {
                     for (var n = atob(e), r = new ArrayBuffer(n.length), i = new Uint8Array(r), a = 0; a < n.length; a++) i[a] = n.charCodeAt(a);
                     return new Blob([r], {
                         type: t
                     })
-                }(Iu(r()), n);
+                }(ac(r()), n);
             case "base64":
-                return Iu(r());
+                return ac(r());
             case "base64uri":
             default:
                 return r()
         }
     }
-    zu.createBuffer = function(e, t) {
+    ic.createBuffer = function(e, t) {
         var n = document.createElement("canvas");
         return n.width = e, n.height = t, [n, n.getContext("2d")]
-    }, zu.bufferCanvasImage = function(e) {
+    }, ic.bufferCanvasImage = function(e) {
         var t = this.cy,
             n = t.mutableElements().boundingBox(),
             r = this.findContainerClientCoords(),
             i = e.full ? Math.ceil(n.w) : r[2],
             a = e.full ? Math.ceil(n.h) : r[3],
-            o = m(e.maxWidth) || m(e.maxHeight),
+            o = b(e.maxWidth) || b(e.maxHeight),
             s = this.getPixelRatio(),
             l = 1;
         if (void 0 !== e.scale) i *= e.scale, a *= e.scale, l = e.scale;
         else if (o) {
             var u = 1 / 0,
                 c = 1 / 0;
-            m(e.maxWidth) && (u = l * e.maxWidth / i), m(e.maxHeight) && (c = l * e.maxHeight / a), i *= l = Math.min(u, c), a *= l
+            b(e.maxWidth) && (u = l * e.maxWidth / i), b(e.maxHeight) && (c = l * e.maxHeight / a), i *= l = Math.min(u, c), a *= l
         }
         o || (i *= s, a *= s, l *= s);
         var d = document.createElement("canvas");
         d.width = i, d.height = a, d.style.width = i + "px", d.style.height = a + "px";
         var h = d.getContext("2d");
         if (i > 0 && a > 0) {
             h.clearRect(0, 0, i, a), h.globalCompositeOperation = "source-over";
@@ -15786,78 +16042,78 @@
                         y: f.y * l
                     };
                 l *= t.zoom(), h.translate(g.x, g.y), h.scale(l, l), this.drawElements(h, p), h.scale(1 / l, 1 / l), h.translate(-g.x, -g.y)
             }
             e.bg && (h.globalCompositeOperation = "destination-over", h.fillStyle = e.bg, h.rect(0, 0, i, a), h.fill())
         }
         return d
-    }, zu.png = function(e) {
-        return Lu(e, this.bufferCanvasImage(e), "image/png")
-    }, zu.jpg = function(e) {
-        return Lu(e, this.bufferCanvasImage(e), "image/jpeg")
+    }, ic.png = function(e) {
+        return oc(e, this.bufferCanvasImage(e), "image/png")
+    }, ic.jpg = function(e) {
+        return oc(e, this.bufferCanvasImage(e), "image/jpeg")
     };
-    var Au = {
-            nodeShapeImpl: function(e, t, n, r, i, a, o) {
+    var sc = {
+            nodeShapeImpl: function(e, t, n, r, i, a, o, s) {
                 switch (e) {
                     case "ellipse":
                         return this.drawEllipsePath(t, n, r, i, a);
                     case "polygon":
                         return this.drawPolygonPath(t, n, r, i, a, o);
                     case "round-polygon":
-                        return this.drawRoundPolygonPath(t, n, r, i, a, o);
+                        return this.drawRoundPolygonPath(t, n, r, i, a, o, s);
                     case "roundrectangle":
                     case "round-rectangle":
-                        return this.drawRoundRectanglePath(t, n, r, i, a);
+                        return this.drawRoundRectanglePath(t, n, r, i, a, s);
                     case "cutrectangle":
                     case "cut-rectangle":
-                        return this.drawCutRectanglePath(t, n, r, i, a);
+                        return this.drawCutRectanglePath(t, n, r, i, a, o, s);
                     case "bottomroundrectangle":
                     case "bottom-round-rectangle":
-                        return this.drawBottomRoundRectanglePath(t, n, r, i, a);
+                        return this.drawBottomRoundRectanglePath(t, n, r, i, a, s);
                     case "barrel":
                         return this.drawBarrelPath(t, n, r, i, a)
                 }
             }
         },
-        Ou = Vu,
-        Ru = Vu.prototype;
+        lc = cc,
+        uc = cc.prototype;
 
-    function Vu(e) {
+    function cc(e) {
         var t = this;
         t.data = {
-            canvases: new Array(Ru.CANVAS_LAYERS),
-            contexts: new Array(Ru.CANVAS_LAYERS),
-            canvasNeedsRedraw: new Array(Ru.CANVAS_LAYERS),
-            bufferCanvases: new Array(Ru.BUFFER_COUNT),
-            bufferContexts: new Array(Ru.CANVAS_LAYERS)
+            canvases: new Array(uc.CANVAS_LAYERS),
+            contexts: new Array(uc.CANVAS_LAYERS),
+            canvasNeedsRedraw: new Array(uc.CANVAS_LAYERS),
+            bufferCanvases: new Array(uc.BUFFER_COUNT),
+            bufferContexts: new Array(uc.CANVAS_LAYERS)
         };
         t.data.canvasContainer = document.createElement("div");
         var n = t.data.canvasContainer.style;
         t.data.canvasContainer.style["-webkit-tap-highlight-color"] = "rgba(0,0,0,0)", n.position = "relative", n.zIndex = "0", n.overflow = "hidden";
         var r = e.cy.container();
         r.appendChild(t.data.canvasContainer), r.style["-webkit-tap-highlight-color"] = "rgba(0,0,0,0)";
         var i = {
             "-webkit-user-select": "none",
             "-moz-user-select": "-moz-none",
             "user-select": "none",
             "-webkit-tap-highlight-color": "rgba(0,0,0,0)",
             "outline-style": "none"
         };
-        l && l.userAgent.match(/msie|trident|edge/i) && (i["-ms-touch-action"] = "none", i["touch-action"] = "none");
-        for (var a = 0; a < Ru.CANVAS_LAYERS; a++) {
+        u && u.userAgent.match(/msie|trident|edge/i) && (i["-ms-touch-action"] = "none", i["touch-action"] = "none");
+        for (var a = 0; a < uc.CANVAS_LAYERS; a++) {
             var o = t.data.canvases[a] = document.createElement("canvas");
             t.data.contexts[a] = o.getContext("2d"), Object.keys(i).forEach((function(e) {
                 o.style[e] = i[e]
-            })), o.style.position = "absolute", o.setAttribute("data-id", "layer" + a), o.style.zIndex = String(Ru.CANVAS_LAYERS - a), t.data.canvasContainer.appendChild(o), t.data.canvasNeedsRedraw[a] = !1
+            })), o.style.position = "absolute", o.setAttribute("data-id", "layer" + a), o.style.zIndex = String(uc.CANVAS_LAYERS - a), t.data.canvasContainer.appendChild(o), t.data.canvasNeedsRedraw[a] = !1
         }
-        t.data.topCanvas = t.data.canvases[0], t.data.canvases[Ru.NODE].setAttribute("data-id", "layer" + Ru.NODE + "-node"), t.data.canvases[Ru.SELECT_BOX].setAttribute("data-id", "layer" + Ru.SELECT_BOX + "-selectbox"), t.data.canvases[Ru.DRAG].setAttribute("data-id", "layer" + Ru.DRAG + "-drag");
-        for (a = 0; a < Ru.BUFFER_COUNT; a++) t.data.bufferCanvases[a] = document.createElement("canvas"), t.data.bufferContexts[a] = t.data.bufferCanvases[a].getContext("2d"), t.data.bufferCanvases[a].style.position = "absolute", t.data.bufferCanvases[a].setAttribute("data-id", "buffer" + a), t.data.bufferCanvases[a].style.zIndex = String(-a - 1), t.data.bufferCanvases[a].style.visibility = "hidden";
+        t.data.topCanvas = t.data.canvases[0], t.data.canvases[uc.NODE].setAttribute("data-id", "layer" + uc.NODE + "-node"), t.data.canvases[uc.SELECT_BOX].setAttribute("data-id", "layer" + uc.SELECT_BOX + "-selectbox"), t.data.canvases[uc.DRAG].setAttribute("data-id", "layer" + uc.DRAG + "-drag");
+        for (a = 0; a < uc.BUFFER_COUNT; a++) t.data.bufferCanvases[a] = document.createElement("canvas"), t.data.bufferContexts[a] = t.data.bufferCanvases[a].getContext("2d"), t.data.bufferCanvases[a].style.position = "absolute", t.data.bufferCanvases[a].setAttribute("data-id", "buffer" + a), t.data.bufferCanvases[a].style.zIndex = String(-a - 1), t.data.bufferCanvases[a].style.visibility = "hidden";
         t.pathsEnabled = !0;
-        var s = Dt(),
-            u = function(e) {
+        var s = Tt(),
+            l = function(e) {
                 return {
                     x: -e.w / 2,
                     y: -e.h / 2
                 }
             },
             c = function(e) {
                 return e.boundingBox(), e[0]._private.bodyBounds
@@ -15884,15 +16140,15 @@
             v = function(e, t, n) {
                 var r = e[0]._private.rscratch;
                 return {
                     x: r[t],
                     y: r[n]
                 }
             },
-            y = t.data.eleTxrCache = new Ql(t, {
+            y = t.data.eleTxrCache = new ku(t, {
                 getKey: function(e) {
                     return e[0]._private.nodeKey
                 },
                 doesEleInvalidateKey: function(e) {
                     var t = e[0]._private;
                     return !(t.oldBackgroundTimestamp === t.backgroundTimestamp)
                 },
@@ -15904,33 +16160,33 @@
                     return {
                         x: ((t = c(e)).x1 + t.x2) / 2,
                         y: (t.y1 + t.y2) / 2
                     };
                     var t
                 },
                 getRotationOffset: function(e) {
-                    return u(c(e))
+                    return l(c(e))
                 },
                 allowEdgeTxrCaching: !1,
                 allowParentTxrCaching: !1
             }),
-            m = t.data.lblTxrCache = new Ql(t, {
+            m = t.data.lblTxrCache = new ku(t, {
                 getKey: function(e) {
                     return e[0]._private.labelStyleKey
                 },
                 drawElement: function(e, n, r, i, a) {
                     return t.drawElementText(e, n, r, i, "main", a)
                 },
                 getBoundingBox: d,
                 getRotationPoint: function(e) {
                     return g("", v(e, "labelX", "labelY"), e)
                 },
                 getRotationOffset: function(e) {
                     var t = d(e),
-                        n = u(d(e));
+                        n = l(d(e));
                     if (e.isNode()) {
                         switch (e.pstyle("text-halign").value) {
                             case "left":
                                 n.x = -t.w;
                                 break;
                             case "right":
                                 n.x = 0
@@ -15943,121 +16199,121 @@
                                 n.y = 0
                         }
                     }
                     return n
                 },
                 isVisible: f
             }),
-            b = t.data.slbTxrCache = new Ql(t, {
+            b = t.data.slbTxrCache = new ku(t, {
                 getKey: function(e) {
                     return e[0]._private.sourceLabelStyleKey
                 },
                 drawElement: function(e, n, r, i, a) {
                     return t.drawElementText(e, n, r, i, "source", a)
                 },
                 getBoundingBox: h,
                 getRotationPoint: function(e) {
                     return g("source", v(e, "sourceLabelX", "sourceLabelY"), e)
                 },
                 getRotationOffset: function(e) {
-                    return u(h(e))
+                    return l(h(e))
                 },
                 isVisible: f
             }),
-            x = t.data.tlbTxrCache = new Ql(t, {
+            x = t.data.tlbTxrCache = new ku(t, {
                 getKey: function(e) {
                     return e[0]._private.targetLabelStyleKey
                 },
                 drawElement: function(e, n, r, i, a) {
                     return t.drawElementText(e, n, r, i, "target", a)
                 },
                 getBoundingBox: p,
                 getRotationPoint: function(e) {
                     return g("target", v(e, "targetLabelX", "targetLabelY"), e)
                 },
                 getRotationOffset: function(e) {
-                    return u(p(e))
+                    return l(p(e))
                 },
                 isVisible: f
             }),
-            w = t.data.lyrTxrCache = new eu(t);
+            w = t.data.lyrTxrCache = new Su(t);
         t.onUpdateEleCalcs((function(e, t) {
             y.invalidateElements(t), m.invalidateElements(t), b.invalidateElements(t), x.invalidateElements(t), w.invalidateElements(t);
             for (var n = 0; n < t.length; n++) {
                 var r = t[n]._private;
                 r.oldBackgroundTimestamp = r.backgroundTimestamp
             }
         }));
         var E = function(e) {
             for (var t = 0; t < e.length; t++) w.enqueueElementRefinement(e[t].ele)
         };
         y.onDequeue(E), m.onDequeue(E), b.onDequeue(E), x.onDequeue(E)
     }
-    Ru.CANVAS_LAYERS = 3, Ru.SELECT_BOX = 0, Ru.DRAG = 1, Ru.NODE = 2, Ru.BUFFER_COUNT = 3, Ru.TEXTURE_BUFFER = 0, Ru.MOTIONBLUR_BUFFER_NODE = 1, Ru.MOTIONBLUR_BUFFER_DRAG = 2, Ru.redrawHint = function(e, t) {
+    uc.CANVAS_LAYERS = 3, uc.SELECT_BOX = 0, uc.DRAG = 1, uc.NODE = 2, uc.BUFFER_COUNT = 3, uc.TEXTURE_BUFFER = 0, uc.MOTIONBLUR_BUFFER_NODE = 1, uc.MOTIONBLUR_BUFFER_DRAG = 2, uc.redrawHint = function(e, t) {
         var n = this;
         switch (e) {
             case "eles":
-                n.data.canvasNeedsRedraw[Ru.NODE] = t;
+                n.data.canvasNeedsRedraw[uc.NODE] = t;
                 break;
             case "drag":
-                n.data.canvasNeedsRedraw[Ru.DRAG] = t;
+                n.data.canvasNeedsRedraw[uc.DRAG] = t;
                 break;
             case "select":
-                n.data.canvasNeedsRedraw[Ru.SELECT_BOX] = t
+                n.data.canvasNeedsRedraw[uc.SELECT_BOX] = t
         }
     };
-    var Fu = "undefined" != typeof Path2D;
-    Ru.path2dEnabled = function(e) {
+    var dc = "undefined" != typeof Path2D;
+    uc.path2dEnabled = function(e) {
         if (void 0 === e) return this.pathsEnabled;
         this.pathsEnabled = !!e
-    }, Ru.usePaths = function() {
-        return Fu && this.pathsEnabled
-    }, Ru.setImgSmoothing = function(e, t) {
+    }, uc.usePaths = function() {
+        return dc && this.pathsEnabled
+    }, uc.setImgSmoothing = function(e, t) {
         null != e.imageSmoothingEnabled ? e.imageSmoothingEnabled = t : (e.webkitImageSmoothingEnabled = t, e.mozImageSmoothingEnabled = t, e.msImageSmoothingEnabled = t)
-    }, Ru.getImgSmoothing = function(e) {
+    }, uc.getImgSmoothing = function(e) {
         return null != e.imageSmoothingEnabled ? e.imageSmoothingEnabled : e.webkitImageSmoothingEnabled || e.mozImageSmoothingEnabled || e.msImageSmoothingEnabled
-    }, Ru.makeOffscreenCanvas = function(t, n) {
+    }, uc.makeOffscreenCanvas = function(t, n) {
         var r;
         return "undefined" !== ("undefined" == typeof OffscreenCanvas ? "undefined" : e(OffscreenCanvas)) ? r = new OffscreenCanvas(t, n) : ((r = document.createElement("canvas")).width = t, r.height = n), r
-    }, [au, du, mu, xu, wu, ku, Su, Pu, zu, Au].forEach((function(e) {
-        I(Ru, e)
+    }, [Mu, Lu, Yu, Wu, Hu, Gu, Zu, $u, ic, sc].forEach((function(e) {
+        A(uc, e)
     }));
-    var ju = [{
+    var hc = [{
             type: "layout",
-            extensions: wl
+            extensions: kl
         }, {
             type: "renderer",
             extensions: [{
                 name: "null",
-                impl: El
+                impl: Cl
             }, {
                 name: "base",
-                impl: Hl
+                impl: yu
             }, {
                 name: "canvas",
-                impl: Ou
+                impl: lc
             }]
         }],
-        qu = {},
-        Yu = {};
+        pc = {},
+        fc = {};
 
-    function Xu(e, t, n) {
+    function gc(e, t, n) {
         var r = n,
             i = function(n) {
-                Ve("Can not register `" + t + "` for `" + e + "` since `" + n + "` already exists in the prototype and can not be overridden")
+                Fe("Can not register `" + t + "` for `" + e + "` since `" + n + "` already exists in the prototype and can not be overridden")
             };
         if ("core" === e) {
-            if (Is.prototype[t]) return i(t);
-            Is.prototype[t] = n
+            if (Ls.prototype[t]) return i(t);
+            Ls.prototype[t] = n
         } else if ("collection" === e) {
-            if (Qo.prototype[t]) return i(t);
-            Qo.prototype[t] = n
+            if (es.prototype[t]) return i(t);
+            es.prototype[t] = n
         } else if ("layout" === e) {
             for (var a = function(e) {
-                    this.options = e, n.call(this, e), y(this._private) || (this._private = {}), this._private.cy = e.cy, this._private.listeners = [], this.createEmitter()
+                    this.options = e, n.call(this, e), m(this._private) || (this._private = {}), this._private.cy = e.cy, this._private.listeners = [], this.createEmitter()
                 }, o = a.prototype = Object.create(n.prototype), s = [], l = 0; l < s.length; l++) {
                 var u = s[l];
                 o[u] = o[u] || function() {
                     return this
                 }
             }
             o.start && !o.run ? o.run = function() {
@@ -16089,17 +16345,17 @@
                     bubble: function() {
                         return !0
                     },
                     parent: function(e) {
                         return d(e)
                     }
                 };
-            I(o, {
+            A(o, {
                 createEmitter: function() {
-                    return this._private.emitter = new yo(h, this), this
+                    return this._private.emitter = new bo(h, this), this
                 },
                 emitter: function() {
                     return this._private.emitter
                 },
                 on: function(e, t) {
                     return this.emitter().on(e, t), this
                 },
@@ -16114,126 +16370,126 @@
                 },
                 removeAllListeners: function() {
                     return this.emitter().removeAllListeners(), this
                 },
                 emit: function(e, t) {
                     return this.emitter().emit(e, t), this
                 }
-            }), Oi.eventAliasesOn(o), r = a
+            }), Vi.eventAliasesOn(o), r = a
         } else if ("renderer" === e && "null" !== t && "base" !== t) {
-            var p = Wu("renderer", "base"),
+            var p = vc("renderer", "base"),
                 f = p.prototype,
                 g = n,
                 v = n.prototype,
-                m = function() {
+                y = function() {
                     p.apply(this, arguments), g.apply(this, arguments)
                 },
-                b = m.prototype;
+                b = y.prototype;
             for (var x in f) {
                 var w = f[x];
                 if (null != v[x]) return i(x);
                 b[x] = w
             }
             for (var E in v) b[E] = v[E];
             f.clientFunctions.forEach((function(e) {
                 b[e] = b[e] || function() {
-                    Oe("Renderer does not implement `renderer." + e + "()` on its prototype")
+                    Re("Renderer does not implement `renderer." + e + "()` on its prototype")
                 }
-            })), r = m
-        } else if ("__proto__" === e || "constructor" === e || "prototype" === e) return Oe(e + " is an illegal type to be registered, possibly lead to prototype pollutions");
-        return O({
-            map: qu,
+            })), r = y
+        } else if ("__proto__" === e || "constructor" === e || "prototype" === e) return Re(e + " is an illegal type to be registered, possibly lead to prototype pollutions");
+        return R({
+            map: pc,
             keys: [e, t],
             value: r
         })
     }
 
-    function Wu(e, t) {
-        return R({
-            map: qu,
+    function vc(e, t) {
+        return V({
+            map: pc,
             keys: [e, t]
         })
     }
 
-    function Hu(e, t, n, r, i) {
-        return O({
-            map: Yu,
+    function yc(e, t, n, r, i) {
+        return R({
+            map: fc,
             keys: [e, t, n, r],
             value: i
         })
     }
 
-    function Ku(e, t, n, r) {
-        return R({
-            map: Yu,
+    function mc(e, t, n, r) {
+        return V({
+            map: fc,
             keys: [e, t, n, r]
         })
     }
-    var Gu = function() {
-        return 2 === arguments.length ? Wu.apply(null, arguments) : 3 === arguments.length ? Xu.apply(null, arguments) : 4 === arguments.length ? Ku.apply(null, arguments) : 5 === arguments.length ? Hu.apply(null, arguments) : void Oe("Invalid extension access syntax")
+    var bc = function() {
+        return 2 === arguments.length ? vc.apply(null, arguments) : 3 === arguments.length ? gc.apply(null, arguments) : 4 === arguments.length ? mc.apply(null, arguments) : 5 === arguments.length ? yc.apply(null, arguments) : void Re("Invalid extension access syntax")
     };
-    Is.prototype.extension = Gu, ju.forEach((function(e) {
+    Ls.prototype.extension = bc, hc.forEach((function(e) {
         e.extensions.forEach((function(t) {
-            Xu(e.type, t.name, t.impl)
+            gc(e.type, t.name, t.impl)
         }))
     }));
-    var Uu = function e() {
+    var xc = function e() {
             if (!(this instanceof e)) return new e;
             this.length = 0
         },
-        Zu = Uu.prototype;
-    Zu.instanceString = function() {
+        wc = xc.prototype;
+    wc.instanceString = function() {
         return "stylesheet"
-    }, Zu.selector = function(e) {
+    }, wc.selector = function(e) {
         return this[this.length++] = {
             selector: e,
             properties: []
         }, this
-    }, Zu.css = function(e, t) {
+    }, wc.css = function(e, t) {
         var n = this.length - 1;
-        if (f(e)) this[n].properties.push({
+        if (g(e)) this[n].properties.push({
             name: e,
             value: t
         });
-        else if (y(e))
+        else if (m(e))
             for (var r = e, i = Object.keys(r), a = 0; a < i.length; a++) {
                 var o = i[a],
                     s = r[o];
                 if (null != s) {
-                    var l = _s.properties[o] || _s.properties[_(o)];
+                    var l = Bs.properties[o] || Bs.properties[M(o)];
                     if (null != l) {
                         var u = l.name,
                             c = s;
                         this[n].properties.push({
                             name: u,
                             value: c
                         })
                     }
                 }
             }
         return this
-    }, Zu.style = Zu.css, Zu.generateStyle = function(e) {
-        var t = new _s(e);
+    }, wc.style = wc.css, wc.generateStyle = function(e) {
+        var t = new Bs(e);
         return this.appendToStyle(t)
-    }, Zu.appendToStyle = function(e) {
+    }, wc.appendToStyle = function(e) {
         for (var t = 0; t < this.length; t++) {
             var n = this[t],
                 r = n.selector,
                 i = n.properties;
             e.selector(r);
             for (var a = 0; a < i.length; a++) {
                 var o = i[a];
                 e.css(o.name, o.value)
             }
         }
         return e
     };
-    var $u = function(e) {
-        return void 0 === e && (e = {}), y(e) ? new Is(e) : f(e) ? Gu.apply(Gu, arguments) : void 0
+    var Ec = function(e) {
+        return void 0 === e && (e = {}), m(e) ? new Ls(e) : g(e) ? bc.apply(bc, arguments) : void 0
     };
-    return $u.use = function(e) {
+    return Ec.use = function(e) {
         var t = Array.prototype.slice.call(arguments, 1);
-        return t.unshift($u), e.apply(null, t), this
-    }, $u.warnings = function(e) {
-        return Re(e)
-    }, $u.version = "3.28.1", $u.stylesheet = $u.Stylesheet = Uu, $u
+        return t.unshift(Ec), e.apply(null, t), this
+    }, Ec.warnings = function(e) {
+        return Ve(e)
+    }, Ec.version = "3.29.2", Ec.stylesheet = Ec.Stylesheet = xc, Ec
 }));
```

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net/js/jquery.dataTables.min.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-bs4/css/dataTables.bootstrap4.min.css` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-bs4/css/dataTables.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-bs4/js/dataTables.bootstrap4.min.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-bs4/js/dataTables.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-buttons/js/dataTables.buttons.min.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-buttons/js/dataTables.buttons.min.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-buttons-bs4/css/buttons.bootstrap4.min.css` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-buttons-bs4/css/buttons.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-dt/js/dataTables.dataTables.min.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-dt/js/dataTables.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-select/js/dataTables.select.min.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-select/js/dataTables.select.min.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/datatables.net-select-dt/css/select.dataTables.min.css` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-select-dt/css/select.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/jquery/dist/jquery.min.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jquery/dist/jquery.min.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/jquery-csv/src/jquery.csv.min.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jquery-csv/src/jquery.csv.min.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/jstree/dist/jstree.min.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/jstree.min.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/jstree/dist/themes/default/32px.png` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/themes/default/32px.png`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/jstree/dist/themes/default/style.css` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/themes/default/style.css`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/jstree/dist/themes/default/throbber.gif` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/themes/default/throbber.gif`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/ngl/dist/ngl.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/ngl/dist/ngl.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/pace-progress/pace.min.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/pace-progress/pace.min.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/perfect-scrollbar/dist/perfect-scrollbar.min.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/perfect-scrollbar/dist/perfect-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/plotly.js-dist-min/plotly.min.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/plotly.js-dist-min/plotly.min.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/node_modules/popper.js/dist/umd/popper.min.js` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/popper.js/dist/umd/popper.min.js`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/only_needed_files.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/only_needed_files.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/package-lock.json` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981436567164179%*

 * *Differences: {"'packages'": "{'node_modules/buble': {delete: ['license']}, 'node_modules/core-js': {'version': "*

 * *               "'3.37.1', 'resolved': 'https://registry.npmjs.org/core-js/-/core-js-3.37.1.tgz', "*

 * *               "'integrity': "*

 * *               "'sha512-Xn6qmxrQZyB0FFY8E3bgRXei3lWDJHhvI+u0q9TKIYM49G8pAr0FgnnrFRAmsbptZL1yxRADVXn+x5AGsbBfyw=='}, "*

 * *               "'node_modules/cytoscape': {'version': '3.29.2', 'resolved': "*

 * *               "'https://registry.npmjs.org/cytoscape/-/cytoscape-3.29.2.tgz', 'integr […]*

```diff
@@ -84,19 +84,14 @@
             "engines": {
                 "node": "*"
             },
             "integrity": "sha512-E+iruNOY8VV9s4JEbe1aNEm6MiszPRr/UfcHMz0TQh1BXSxHK+ASV1R6W4HpjBhSeS+54PIsAMCBmwD06LLsqQ==",
             "resolved": "https://registry.npmjs.org/JSONStream/-/JSONStream-1.3.5.tgz",
             "version": "1.3.5"
         },
-        "node_modules/abbrev": {
-            "integrity": "sha512-nne9/IiQ/hzIhY6pdDnbBtz7DjPTKrY00P/zvPSm5pOFkl6xuGrGnXn/VtTNNfNtAfZ9/1RtehkszU9qcTii0Q==",
-            "resolved": "https://registry.npmjs.org/abbrev/-/abbrev-1.1.1.tgz",
-            "version": "1.1.1"
-        },
         "node_modules/accepts": {
             "dependencies": {
                 "mime-types": "~2.1.34",
                 "negotiator": "0.6.3"
             },
             "engines": {
                 "node": ">= 0.6"
@@ -479,15 +474,14 @@
                 "acorn5-object-spread": "^4.0.0",
                 "chalk": "^2.1.0",
                 "magic-string": "^0.22.4",
                 "minimist": "^1.2.0",
                 "os-homedir": "^1.0.1",
                 "vlq": "^0.2.2"
             },
-            "license": "MIT",
             "resolved": "git+ssh://git@github.com/pemrouz/buble.git#4e639aeeb64712ac95dc30a52750d1ee4432c9c8",
             "version": "0.18.0"
         },
         "node_modules/buble/node_modules/acorn": {
             "bin": {
                 "acorn": "bin/acorn"
             },
@@ -730,17 +724,17 @@
         },
         "node_modules/core-js": {
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/core-js"
             },
             "hasInstallScript": true,
-            "integrity": "sha512-BTvUrwxVBezj5SZ3f10ImnX2oRByMxql3EimVqMysepbC9EeMUOpLwdy6Eoili2x6E4kf+ZUB5k/+Jv55alPfA==",
-            "resolved": "https://registry.npmjs.org/core-js/-/core-js-3.36.1.tgz",
-            "version": "3.36.1"
+            "integrity": "sha512-Xn6qmxrQZyB0FFY8E3bgRXei3lWDJHhvI+u0q9TKIYM49G8pAr0FgnnrFRAmsbptZL1yxRADVXn+x5AGsbBfyw==",
+            "resolved": "https://registry.npmjs.org/core-js/-/core-js-3.37.1.tgz",
+            "version": "3.37.1"
         },
         "node_modules/core-util-is": {
             "integrity": "sha512-ZQBvi1DcpJ4GDqanjucZ2Hj3wEO5pZDS89BWbkcrvdxksJorwUDDZamX9ldFkp9aw2lmBDLgkObEA4DWNJ9FYQ==",
             "resolved": "https://registry.npmjs.org/core-util-is/-/core-util-is-1.0.3.tgz",
             "version": "1.0.3"
         },
         "node_modules/create-ecdh": {
@@ -800,24 +794,20 @@
                 "node": "*"
             },
             "integrity": "sha512-fz4spIh+znjO2VjL+IdhEpRJ3YN6sMzITSBijk6FK2UvTqruSQW+/cCZTSNsMiZNvUeq0CqurF+dAbyiGOY6Wg==",
             "resolved": "https://registry.npmjs.org/crypto-browserify/-/crypto-browserify-3.12.0.tgz",
             "version": "3.12.0"
         },
         "node_modules/cytoscape": {
-            "dependencies": {
-                "heap": "^0.2.6",
-                "lodash": "^4.17.21"
-            },
             "engines": {
                 "node": ">=0.10"
             },
-            "integrity": "sha512-xyItz4O/4zp9/239wCcH8ZcFuuZooEeF8KHRmzjDfGdXsj3OG9MFSMA0pJE0uX3uCN/ygof6hHf4L7lst+JaDg==",
-            "resolved": "https://registry.npmjs.org/cytoscape/-/cytoscape-3.28.1.tgz",
-            "version": "3.28.1"
+            "integrity": "sha512-2G1ycU28Nh7OHT9rkXRLpCDP30MKH1dXJORZuBhtEhEW7pKwgPi77ImqlCWinouyE1PNepIOGZBOrE84DG7LyQ==",
+            "resolved": "https://registry.npmjs.org/cytoscape/-/cytoscape-3.29.2.tgz",
+            "version": "3.29.2"
         },
         "node_modules/dash-ast": {
             "integrity": "sha512-Vy4dx7gquTeMcQR/hDkYLGUnwVil6vk4FOOct+djUnHOUWt+zJPJAaRIXaAFkPXtJjvlY7o3rfRu0/3hpnwoUA==",
             "resolved": "https://registry.npmjs.org/dash-ast/-/dash-ast-1.0.0.tgz",
             "version": "1.0.0"
         },
         "node_modules/datatables.net": {
@@ -1340,19 +1330,14 @@
             "engines": {
                 "node": ">= 0.4"
             },
             "integrity": "sha512-0hJU9SCPvmMzIBdZFqNPXWa6dqh7WdH0cII9y+CyS8rG3nL48Bclra9HmKhVVUHyPWNH5Y7xDwAB7bfgSjkUMQ==",
             "resolved": "https://registry.npmjs.org/hasown/-/hasown-2.0.2.tgz",
             "version": "2.0.2"
         },
-        "node_modules/heap": {
-            "integrity": "sha512-2bsegYkkHO+h/9MGbn6KWcE45cHZgPANo5LXF7EvWdT0yT2EguSVO1nDgU5c8+ZOPwp2vMNa7YFsJhVcDR9Sdg==",
-            "resolved": "https://registry.npmjs.org/heap/-/heap-0.2.7.tgz",
-            "version": "0.2.7"
-        },
         "node_modules/hmac-drbg": {
             "dependencies": {
                 "hash.js": "^1.0.3",
                 "minimalistic-assert": "^1.0.0",
                 "minimalistic-crypto-utils": "^1.0.1"
             },
             "integrity": "sha512-Tti3gMqLdZfhOQY1Mzf/AanLiqh1WTiJgEj26ZuYQ9fbkLomzGchCws4FyrSd4VkpBfiNhaE1On+lOz894jvXg==",
@@ -1423,14 +1408,15 @@
             "version": "0.0.1"
         },
         "node_modules/inflight": {
             "dependencies": {
                 "once": "^1.3.0",
                 "wrappy": "1"
             },
+            "deprecated": "This module is not supported, and leaks memory. Do not use it. Check out lru-cache if you want a good and tested way to coalesce async requests by a key value, which is much more comprehensive and powerful.",
             "integrity": "sha512-k92I/b08q4wvFscXCLvqfsHCrjrF7yiXsQuIVvVE7N82W3+aqpzuUdBbfhWcy/FZR3/4IgflMgKLOsvPDrGCJA==",
             "resolved": "https://registry.npmjs.org/inflight/-/inflight-1.0.6.tgz",
             "version": "1.0.6"
         },
         "node_modules/inherits": {
             "integrity": "sha512-k/vGaX4/Yla3WzyMCvTQOXYeIHvqOKtnqBduzTHpzpQZzAskKMhZ2K+EnBiSM9zGSoIFeMpXKxa4dYeZIQqewQ==",
             "resolved": "https://registry.npmjs.org/inherits/-/inherits-2.0.4.tgz",
@@ -1556,19 +1542,14 @@
                 "inherits": "^2.0.1",
                 "stream-splicer": "^2.0.0"
             },
             "integrity": "sha512-Ca4LSXFFZUjPScRaqOcFxneA0VpKZr4MMYCljyQr4LIewTLb3Y0IUTIsnBBsVubIeEfxeSZpSjSsRM8APEQaAw==",
             "resolved": "https://registry.npmjs.org/labeled-stream-splicer/-/labeled-stream-splicer-2.0.2.tgz",
             "version": "2.0.2"
         },
-        "node_modules/lodash": {
-            "integrity": "sha512-v2kDEe57lecTulaDIuNTPy3Ry4gLGJ6Z1O3vE1krgXZNrsQ+LFTGHVxVjcXPs17LhbZVGedAJv8XZ1tvj5FvSg==",
-            "resolved": "https://registry.npmjs.org/lodash/-/lodash-4.17.21.tgz",
-            "version": "4.17.21"
-        },
         "node_modules/lodash.memoize": {
             "integrity": "sha512-eDn9kqrAmVUC1wmZvlQ6Uhde44n+tXpqPrN8olQJbttgh0oKclk+SF54P47VEGE9CEiMeRwAP8BaM7UHvBkz2A==",
             "resolved": "https://registry.npmjs.org/lodash.memoize/-/lodash.memoize-3.0.4.tgz",
             "version": "3.0.4"
         },
         "node_modules/lru_map": {
             "integrity": "sha512-Pn9cox5CsMYngeDbmChANltQl+5pi6XmTrraMSzhPmMBbmgcxmqWry0U3PGapCU1yB4/LqCcom7qhHZiF/jGfQ==",
@@ -1737,28 +1718,14 @@
             "version": "0.6.3"
         },
         "node_modules/ngl": {
             "integrity": "sha512-o08sEPEQ4AAEYvN7WIp7O1mF2X9v4Kk1zslTfGiM4mqvz6vB70Sb5t4OmrWUZ5AiSs78BF2NsrKVduzajA74og==",
             "resolved": "https://registry.npmjs.org/ngl/-/ngl-0.10.4.tgz",
             "version": "0.10.4"
         },
-        "node_modules/nopt": {
-            "bin": {
-                "nopt": "bin/nopt.js"
-            },
-            "dependencies": {
-                "abbrev": "1"
-            },
-            "engines": {
-                "node": "*"
-            },
-            "integrity": "sha512-NWmpvLSqUrgrAC9HCuxEvb+PSloHpqVu+FqcO4eeF2h5qYRhA7ev6KvelyQAKtegUbC6RypJnlEOhd8vloNKYg==",
-            "resolved": "https://registry.npmjs.org/nopt/-/nopt-1.0.10.tgz",
-            "version": "1.0.10"
-        },
         "node_modules/notifyjs": {
             "integrity": "sha512-N3OZt+DsTClAG9DiWrbWBGlsDpDrc50F1qQ+iFl3DBeQg7W7nS4vXmD8WQrGK13RGRyXOGlqsDIenTbK6EJw7A==",
             "resolved": "https://registry.npmjs.org/notifyjs/-/notifyjs-3.0.0.tgz",
             "version": "3.0.0"
         },
         "node_modules/object-inspect": {
             "funding": {
@@ -2414,20 +2381,17 @@
             "resolved": "https://registry.npmjs.org/toidentifier/-/toidentifier-1.0.1.tgz",
             "version": "1.0.1"
         },
         "node_modules/touch": {
             "bin": {
                 "nodetouch": "bin/nodetouch.js"
             },
-            "dependencies": {
-                "nopt": "~1.0.10"
-            },
-            "integrity": "sha512-WBx8Uy5TLtOSRtIq+M03/sKDrXCLHxwDcquSP2c43Le03/9serjQBIztjRz6FkJez9D/hleyAXTBGLwwZUw9lA==",
-            "resolved": "https://registry.npmjs.org/touch/-/touch-3.1.0.tgz",
-            "version": "3.1.0"
+            "integrity": "sha512-r0eojU4bI8MnHr8c5bNo7lJDdI2qXlWWJk6a9EAFG7vbhTjElYhBVS3/miuE0uOuoLdb8Mc/rVfsmm6eo5o9GA==",
+            "resolved": "https://registry.npmjs.org/touch/-/touch-3.1.1.tgz",
+            "version": "3.1.1"
         },
         "node_modules/tty-browserify": {
             "integrity": "sha512-C3TaO7K81YvjCgQH9Q1S3R3P3BtN3RIM8n+OvX4il1K1zgE8ZhI0op7kClgkxtutIE8hQrcrHBXvIheqKUUCxw==",
             "resolved": "https://registry.npmjs.org/tty-browserify/-/tty-browserify-0.0.1.tgz",
             "version": "0.0.1"
         },
         "node_modules/type-is": {
@@ -2496,17 +2460,17 @@
             },
             "engines": {
                 "node": ">=0.6"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
-            "integrity": "sha512-trVZiI6RMOkO476zLGaBIzszOdFPnCCXHPG9kn0yuS1uz6xdVxPfZdB3vUig9pxPFDM9BRAgz/YUIVQ1/vuiUg==",
-            "resolved": "https://registry.npmjs.org/qs/-/qs-6.12.0.tgz",
-            "version": "6.12.0"
+            "integrity": "sha512-zWmv4RSuB9r2mYQw3zxQuHWeU+42aKi1wWig/j4ele4ygELZ7PEO6MM7rim9oAQH2A5MWfsAVf/jPvTPgCbvUQ==",
+            "resolved": "https://registry.npmjs.org/qs/-/qs-6.12.1.tgz",
+            "version": "6.12.1"
         },
         "node_modules/util": {
             "dependencies": {
                 "inherits": "2.0.3"
             },
             "integrity": "sha512-0Pm9hTQ3se5ll1XihRic3FDIku70C+iHUdT/W926rSgHV5QgXsYbKZN8MSC3tJtSkhuROzvsQjAaFENRXr+19A==",
             "resolved": "https://registry.npmjs.org/util/-/util-0.10.4.tgz",
```

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/static/package.json` & `seamm_dashboard-2024.5.24/seamm_dashboard/static/package.json`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/swagger.yml` & `seamm_dashboard-2024.5.24/seamm_dashboard/swagger.yml`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/401.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/401.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/404.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/404.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/500.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/500.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/base.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/create_group.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/create_group.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/create_user.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/create_user.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/delete_group.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/delete_group.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/delete_user.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/delete_user.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/email/reset_password.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/email/reset_password.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/manage_groups.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/manage_groups.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/manage_users.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/manage_users.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/admin/unconfirmed.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/unconfirmed.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/auth/base.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/auth/base.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/auth/manage_account.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/auth/manage_account.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/flowcharts/flowchart_list.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/flowcharts/flowchart_list.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/flowcharts/render_flowchart.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/flowcharts/render_flowchart.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/index.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/index_full.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/index_full.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/jobs/edit_job.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/jobs/edit_job.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/jobs/job_report.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/jobs/job_report.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/jobs/jobs_list.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/jobs/jobs_list.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/login_coreui.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/login_coreui.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/projects/project_access.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/projects/project_access.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/projects/project_list.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/projects/project_list.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/register.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/register.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/breadcrumb.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/breadcrumb.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/card.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/card.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/cards.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/cards.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/carousel.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/carousel.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/collapse.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/collapse.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/forms.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/forms.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/jumbotron.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/jumbotron.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/list-group.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/list-group.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/navbar.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/navbar.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/navs.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/navs.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/pagination.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/pagination.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/popovers.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/popovers.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/progress.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/progress.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/scrollspy.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/scrollspy.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/switches.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/switches.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/tables.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/tables.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/tabs.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/tabs.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/base/tooltips.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/tooltips.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/buttons/brand-buttons.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/brand-buttons.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/buttons/button-group.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/button-group.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/buttons/buttons.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/buttons.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/buttons/dropdowns.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/dropdowns.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/buttons/social-buttons.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/social-buttons.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/charts.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/charts.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/colors.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/colors.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/icons/flags.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/icons/flags.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/icons/font-awesome.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/icons/font-awesome.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/icons/simple-line-icons.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/icons/simple-line-icons.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/login.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/login.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/main.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/main.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/notifications/alerts.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/notifications/alerts.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/notifications/badge.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/notifications/badge.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/notifications/modals.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/notifications/modals.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/typography.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/typography.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/templates/views/widgets.html` & `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/widgets.html`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/tests/conftest.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/tests/test_api.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/tests/test_api_admin.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/tests/test_api_admin.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/tests/test_api_authenticated.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/tests/test_api_authenticated.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/tests/test_views.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard/util.py` & `seamm_dashboard-2024.5.24/seamm_dashboard/util.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard.egg-info/PKG-INFO` & `seamm_dashboard-2024.5.24/seamm_dashboard.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamm-dashboard
-Version: 2024.3.27
+Version: 2024.5.24
 Summary: The Web Dashboard for SEAMM (Simulation Environment for Atomistic and Molecular Simulations).
 Home-page: https://github.com/molssi-seamm/seamm_dashboard.git
 Author: Jessica Nash
 Author-email: janash@vt.edu
 License: BSD-3C
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `seamm-dashboard-2024.3.27/seamm_dashboard.egg-info/SOURCES.txt` & `seamm_dashboard-2024.5.24/seamm_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/setup.py` & `seamm_dashboard-2024.5.24/setup.py`

 * *Files identical despite different names*

### Comparing `seamm-dashboard-2024.3.27/versioneer.py` & `seamm_dashboard-2024.5.24/versioneer.py`

 * *Files identical despite different names*


# Comparing `tmp/robot-soccer-kit-2.1.7.tar.gz` & `tmp/robot-soccer-kit-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robot-soccer-kit-2.1.7.tar", last modified: Wed Nov 22 10:48:40 2023, max compression
+gzip compressed data, was "robot-soccer-kit-2.1.8.tar", last modified: Fri May 24 13:34:47 2024, max compression
```

## Comparing `robot-soccer-kit-2.1.7.tar` & `robot-soccer-kit-2.1.8.tar`

### file list

```diff
@@ -1,161 +1,162 @@
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-11-22 10:48:40.152060 robot-soccer-kit-2.1.7/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      262 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/LICENSE
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1161 2023-11-22 10:48:40.152060 robot-soccer-kit-2.1.7/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      588 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/README.md
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-11-22 10:48:40.104060 robot-soccer-kit-2.1.7/robot_soccer_kit.egg-info/
--rw-r--r--   0 gregwar   (1000) gregwar   (1000)     1161 2023-11-22 10:48:40.000000 robot-soccer-kit-2.1.7/robot_soccer_kit.egg-info/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4865 2023-11-22 10:48:40.000000 robot-soccer-kit-2.1.7/robot_soccer_kit.egg-info/SOURCES.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2023-11-22 10:48:40.000000 robot-soccer-kit-2.1.7/robot_soccer_kit.egg-info/dependency_links.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      176 2023-11-22 10:48:40.000000 robot-soccer-kit-2.1.7/robot_soccer_kit.egg-info/requires.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        4 2023-11-22 10:48:40.000000 robot-soccer-kit-2.1.7/robot_soccer_kit.egg-info/top_level.txt
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-11-22 10:48:40.108060 robot-soccer-kit-2.1.7/rsk/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      102 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/__init__.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/api.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5578 2023-11-10 16:33:26.000000 robot-soccer-kit-2.1.7/rsk/backend.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    14312 2023-11-10 16:33:26.000000 robot-soccer-kit-2.1.7/rsk/client.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      277 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/config.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3696 2023-11-10 16:33:26.000000 robot-soccer-kit-2.1.7/rsk/constants.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13616 2023-06-26 12:24:11.000000 robot-soccer-kit-2.1.7/rsk/control.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    18552 2023-04-29 10:39:09.000000 robot-soccer-kit-2.1.7/rsk/detection.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/dump_referee.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10173 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/field.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2462 2023-11-10 16:33:26.000000 robot-soccer-kit-2.1.7/rsk/game_controller.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2462 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/kinematics.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      445 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/logger.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      602 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/place.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    24336 2023-11-22 10:48:11.000000 robot-soccer-kit-2.1.7/rsk/referee.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2362 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/robot.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11752 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/robot_serial.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6030 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/robots.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10208 2023-11-10 16:33:26.000000 robot-soccer-kit-2.1.7/rsk/simulator.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2321 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/state.py
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-11-22 10:48:40.108060 robot-soccer-kit-2.1.7/rsk/static/
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-11-22 10:48:40.104060 robot-soccer-kit-2.1.7/rsk/static/bootstrap/
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-11-22 10:48:40.124060 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75616 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-grid.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226018 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-grid.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56464 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-grid.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142342 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-grid.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75690 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-grid.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226022 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56539 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142419 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11735 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-reboot.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126626 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-reboot.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9817 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-reboot.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    51406 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11728 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126641 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9889 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    63643 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96254 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-utilities.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250681 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-utilities.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-utilities.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163881 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96121 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250622 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163716 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267476 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658460 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220780 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   568408 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267055 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658305 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   567947 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-11-22 10:48:40.136060 robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   208288 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.bundle.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   448884 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.bundle.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80599 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   333974 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   136243 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.esm.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   305274 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.esm.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74135 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.esm.min.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   222070 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.esm.min.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   145819 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   306458 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    60554 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.min.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   217885 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.min.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      215 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/camera-setting.html
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-11-22 10:48:40.136060 robot-soccer-kit-2.1.7/rsk/static/css/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3471 2023-11-10 16:33:26.000000 robot-soccer-kit-2.1.7/rsk/static/css/app.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1150 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/favicon.ico
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-11-22 10:48:40.140060 robot-soccer-kit-2.1.7/rsk/static/icons/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      376 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/.browserslistrc
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      167 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/.editorconfig
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       40 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/.eslintignore
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      375 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/.eslintrc.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      922 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/.fantasticonrc.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       43 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/.gitattributes
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-11-22 10:48:40.140060 robot-soccer-kit-2.1.7/rsk/static/icons/.github/
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-11-22 10:48:40.140060 robot-soccer-kit-2.1.7/rsk/static/icons/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      583 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      122 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/.github/ISSUE_TEMPLATE/icon-request.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      433 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/.github/dependabot.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   248086 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/.github/preview.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      572 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/.github/release-drafter.yml
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-11-22 10:48:40.140060 robot-soccer-kit-2.1.7/rsk/static/icons/.github/workflows/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      662 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/.github/workflows/codeql.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1190 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/.github/workflows/deploy.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      243 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/.github/workflows/release-notes.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      575 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/.github/workflows/test.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       63 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/.gitignore
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      125 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/.stylelintrc
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1093 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/LICENSE.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3312 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/README.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   881772 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/bootstrap-icons.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      425 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/composer.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2052 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/config.yml
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-11-22 10:48:40.144060 robot-soccer-kit-2.1.7/rsk/static/icons/font/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80510 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/font/bootstrap-icons.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    42897 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/font/bootstrap-icons.json
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-11-22 10:48:40.144060 robot-soccer-kit-2.1.7/rsk/static/icons/font/fonts/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   137124 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/font/fonts/bootstrap-icons.woff
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   102536 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/font/fonts/bootstrap-icons.woff2
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   200995 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/font/index.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   643115 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/package-lock.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3152 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/package.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3085 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/svg-sprite.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/icons/svgo.config.js
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-11-22 10:48:40.148060 robot-soccer-kit-2.1.7/rsk/static/imgs/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3287 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/imgs/ball.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1251 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/imgs/ball_16x16.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1856 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/imgs/ball_24x24.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    43069 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/imgs/ball_256x256.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/imgs/ball_32x32.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4470 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/imgs/ball_48x48.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    19402 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/imgs/field.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    17815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/imgs/field.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   249649 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/imgs/robot.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   507520 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/imgs/robotblue1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   524385 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/imgs/robotblue2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   498488 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/imgs/robotgreen1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   522425 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/imgs/robotgreen2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    33772 2023-11-10 16:33:26.000000 robot-soccer-kit-2.1.7/rsk/static/index.html
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-11-22 10:48:40.148060 robot-soccer-kit-2.1.7/rsk/static/jquery/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   288580 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/jquery/jquery.js
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-11-22 10:48:40.152060 robot-soccer-kit-2.1.7/rsk/static/js/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2396 2023-11-10 16:33:26.000000 robot-soccer-kit-2.1.7/rsk/static/js/app.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1738 2023-06-26 12:35:06.000000 robot-soccer-kit-2.1.7/rsk/static/js/competition.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1567 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/js/control.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13475 2023-11-10 16:33:26.000000 robot-soccer-kit-2.1.7/rsk/static/js/referee.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6005 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/js/robots.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    14606 2023-06-26 12:35:04.000000 robot-soccer-kit-2.1.7/rsk/static/js/simulator.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      426 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/js/tabs.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      329 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/js/utils.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5997 2023-06-26 12:24:11.000000 robot-soccer-kit-2.1.7/rsk/static/js/video.js
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-11-22 10:48:40.152060 robot-soccer-kit-2.1.7/rsk/static/markers/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6021 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/markers/blue1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6023 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/markers/blue2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6009 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/markers/green1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5098 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/markers/green2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      337 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/referee_event_neutral.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      632 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/referee_event_team.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1029 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/static/robot.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      569 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.7/rsk/static/team.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4186 2023-11-10 16:33:26.000000 robot-soccer-kit-2.1.7/rsk/tasks.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4154 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/utils.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9469 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.7/rsk/video.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2023-11-22 10:48:40.152060 robot-soccer-kit-2.1.7/setup.cfg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1420 2023-11-22 10:48:30.000000 robot-soccer-kit-2.1.7/setup.py
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.300004 robot-soccer-kit-2.1.8/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      262 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/LICENSE
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1161 2024-05-24 13:34:47.300004 robot-soccer-kit-2.1.8/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      588 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/README.md
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.292004 robot-soccer-kit-2.1.8/robot_soccer_kit.egg-info/
+-rw-r--r--   0 gregwar   (1000) gregwar   (1000)     1161 2024-05-24 13:34:47.000000 robot-soccer-kit-2.1.8/robot_soccer_kit.egg-info/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4883 2024-05-24 13:34:47.000000 robot-soccer-kit-2.1.8/robot_soccer_kit.egg-info/SOURCES.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2024-05-24 13:34:47.000000 robot-soccer-kit-2.1.8/robot_soccer_kit.egg-info/dependency_links.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      176 2024-05-24 13:34:47.000000 robot-soccer-kit-2.1.8/robot_soccer_kit.egg-info/requires.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        4 2024-05-24 13:34:47.000000 robot-soccer-kit-2.1.8/robot_soccer_kit.egg-info/top_level.txt
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.292004 robot-soccer-kit-2.1.8/rsk/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      102 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/__init__.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/api.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5578 2024-05-21 08:27:22.000000 robot-soccer-kit-2.1.8/rsk/backend.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    14312 2023-11-10 16:33:26.000000 robot-soccer-kit-2.1.8/rsk/client.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      277 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/config.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3696 2023-11-10 16:33:26.000000 robot-soccer-kit-2.1.8/rsk/constants.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13616 2023-06-26 12:24:11.000000 robot-soccer-kit-2.1.8/rsk/control.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    18552 2023-04-29 10:39:09.000000 robot-soccer-kit-2.1.8/rsk/detection.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/dump_referee.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10173 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/field.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2462 2023-11-10 16:33:26.000000 robot-soccer-kit-2.1.8/rsk/game_controller.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2462 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/kinematics.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      445 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/logger.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      602 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/place.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    24336 2023-11-22 10:48:11.000000 robot-soccer-kit-2.1.8/rsk/referee.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2368 2024-05-21 08:26:43.000000 robot-soccer-kit-2.1.8/rsk/robot.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11630 2024-05-21 08:24:01.000000 robot-soccer-kit-2.1.8/rsk/robot_serial.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      142 2024-05-21 08:25:36.000000 robot-soccer-kit-2.1.8/rsk/robot_wifi.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6030 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/robots.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10208 2024-05-21 08:24:28.000000 robot-soccer-kit-2.1.8/rsk/simulator.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2321 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/state.py
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.292004 robot-soccer-kit-2.1.8/rsk/static/
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.292004 robot-soccer-kit-2.1.8/rsk/static/bootstrap/
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.296004 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75616 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226018 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56464 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142342 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75690 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226022 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56539 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142419 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11735 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126626 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9817 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    51406 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11728 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126641 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9889 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    63643 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96254 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250681 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163881 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96121 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250622 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163716 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267476 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658460 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220780 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   568408 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267055 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658305 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   567947 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.296004 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   208288 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.bundle.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   448884 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.bundle.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80599 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   333974 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   136243 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.esm.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   305274 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.esm.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74135 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.esm.min.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   222070 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.esm.min.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   145819 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   306458 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    60554 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.min.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   217885 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.min.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      215 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/camera-setting.html
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.296004 robot-soccer-kit-2.1.8/rsk/static/css/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3721 2024-05-24 13:31:39.000000 robot-soccer-kit-2.1.8/rsk/static/css/app.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1150 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/favicon.ico
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.296004 robot-soccer-kit-2.1.8/rsk/static/icons/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      376 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.browserslistrc
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      167 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.editorconfig
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       40 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.eslintignore
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      375 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.eslintrc.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      922 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.fantasticonrc.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       43 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.gitattributes
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.296004 robot-soccer-kit-2.1.8/rsk/static/icons/.github/
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.296004 robot-soccer-kit-2.1.8/rsk/static/icons/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      583 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      122 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.github/ISSUE_TEMPLATE/icon-request.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      433 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.github/dependabot.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   248086 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.github/preview.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      572 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.github/release-drafter.yml
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.296004 robot-soccer-kit-2.1.8/rsk/static/icons/.github/workflows/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      662 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.github/workflows/codeql.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1190 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.github/workflows/deploy.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      243 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.github/workflows/release-notes.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      575 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.github/workflows/test.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       63 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.gitignore
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      125 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.stylelintrc
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1093 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/LICENSE.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3312 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/README.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   881772 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/bootstrap-icons.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      425 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/composer.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2052 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/config.yml
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.300004 robot-soccer-kit-2.1.8/rsk/static/icons/font/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80510 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/font/bootstrap-icons.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    42897 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/font/bootstrap-icons.json
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.300004 robot-soccer-kit-2.1.8/rsk/static/icons/font/fonts/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   137124 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/font/fonts/bootstrap-icons.woff
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   102536 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/font/fonts/bootstrap-icons.woff2
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   200995 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/font/index.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   643115 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/package-lock.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3152 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/package.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3085 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/svg-sprite.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/svgo.config.js
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.300004 robot-soccer-kit-2.1.8/rsk/static/imgs/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3287 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/ball.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1251 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/ball_16x16.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1856 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/ball_24x24.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    43069 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/ball_256x256.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/ball_32x32.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4470 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/ball_48x48.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    19402 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/field.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    17815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/field.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   249649 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/robot.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   507520 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/robotblue1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   524385 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/robotblue2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   498488 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/robotgreen1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   522425 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/robotgreen2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    33731 2024-05-24 13:33:34.000000 robot-soccer-kit-2.1.8/rsk/static/index.html
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.300004 robot-soccer-kit-2.1.8/rsk/static/jquery/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   288580 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/jquery/jquery.js
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.300004 robot-soccer-kit-2.1.8/rsk/static/js/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2225 2024-05-24 13:33:49.000000 robot-soccer-kit-2.1.8/rsk/static/js/app.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1738 2023-06-26 12:35:06.000000 robot-soccer-kit-2.1.8/rsk/static/js/competition.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1585 2024-04-11 05:52:39.000000 robot-soccer-kit-2.1.8/rsk/static/js/control.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13475 2023-11-10 16:33:26.000000 robot-soccer-kit-2.1.8/rsk/static/js/referee.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6005 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/js/robots.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    14606 2023-06-26 12:35:04.000000 robot-soccer-kit-2.1.8/rsk/static/js/simulator.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      426 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/js/tabs.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      329 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/js/utils.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5997 2023-06-26 12:24:11.000000 robot-soccer-kit-2.1.8/rsk/static/js/video.js
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.300004 robot-soccer-kit-2.1.8/rsk/static/markers/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6021 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/markers/blue1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6023 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/markers/blue2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6009 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/markers/green1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5098 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/markers/green2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      337 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/referee_event_neutral.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      632 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/referee_event_team.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1029 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/robot.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      569 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/team.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4186 2023-11-10 16:33:26.000000 robot-soccer-kit-2.1.8/rsk/tasks.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4154 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/utils.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9469 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/video.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2024-05-24 13:34:47.300004 robot-soccer-kit-2.1.8/setup.cfg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1420 2024-05-24 13:34:34.000000 robot-soccer-kit-2.1.8/setup.py
```

### Comparing `robot-soccer-kit-2.1.7/PKG-INFO` & `robot-soccer-kit-2.1.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robot-soccer-kit
-Version: 2.1.7
+Version: 2.1.8
 Summary: Robot Soccer Kit
 Home-page: https://github.com/rhoban/robot-soccer-kit/
 Author: Rhoban team
 Author-email: team@rhoban.com
 License: UNKNOWN
 Keywords: robot holonomic omniwheel ssl sct robocup junior soccer standard localized tracking
 Platform: UNKNOWN
```

### Comparing `robot-soccer-kit-2.1.7/README.md` & `robot-soccer-kit-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/robot_soccer_kit.egg-info/PKG-INFO` & `robot-soccer-kit-2.1.8/robot_soccer_kit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robot-soccer-kit
-Version: 2.1.7
+Version: 2.1.8
 Summary: Robot Soccer Kit
 Home-page: https://github.com/rhoban/robot-soccer-kit/
 Author: Rhoban team
 Author-email: team@rhoban.com
 License: UNKNOWN
 Keywords: robot holonomic omniwheel ssl sct robocup junior soccer standard localized tracking
 Platform: UNKNOWN
```

### Comparing `robot-soccer-kit-2.1.7/robot_soccer_kit.egg-info/SOURCES.txt` & `robot-soccer-kit-2.1.8/robot_soccer_kit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 rsk/game_controller.py
 rsk/kinematics.py
 rsk/logger.py
 rsk/place.py
 rsk/referee.py
 rsk/robot.py
 rsk/robot_serial.py
+rsk/robot_wifi.py
 rsk/robots.py
 rsk/simulator.py
 rsk/state.py
 rsk/tasks.py
 rsk/utils.py
 rsk/video.py
 rsk/static/camera-setting.html
```

### Comparing `robot-soccer-kit-2.1.7/rsk/api.py` & `robot-soccer-kit-2.1.8/rsk/api.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/backend.py` & `robot-soccer-kit-2.1.8/rsk/backend.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/client.py` & `robot-soccer-kit-2.1.8/rsk/client.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/constants.py` & `robot-soccer-kit-2.1.8/rsk/constants.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/control.py` & `robot-soccer-kit-2.1.8/rsk/control.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/detection.py` & `robot-soccer-kit-2.1.8/rsk/detection.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/dump_referee.py` & `robot-soccer-kit-2.1.8/rsk/dump_referee.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/field.py` & `robot-soccer-kit-2.1.8/rsk/field.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/game_controller.py` & `robot-soccer-kit-2.1.8/rsk/game_controller.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/kinematics.py` & `robot-soccer-kit-2.1.8/rsk/kinematics.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/place.py` & `robot-soccer-kit-2.1.8/rsk/place.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/referee.py` & `robot-soccer-kit-2.1.8/rsk/referee.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/robot.py` & `robot-soccer-kit-2.1.8/rsk/robot.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         """
         Sets the robot's marker
 
         :param str marker: the robot marker
         """
         self.marker = marker
 
-    def kick(self, power: float) -> None:
+    def kick(self, power: float = 1.0) -> None:
         """
         Kicks
 
         :param float power: kick power (0-1)
         :raises RobotError: if the operation is not supported
         """
         raise RobotError("This robot can't kick")
```

### Comparing `robot-soccer-kit-2.1.7/rsk/robot_serial.py` & `robot-soccer-kit-2.1.8/rsk/robot_serial.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,14 @@
         self.thread.start()
 
         # Pending packets queued
         self.pending_packets = {}
         self.lock = threading.Lock()
 
     def available_urls() -> list:
-        devs = [entry.device for entry in list_ports.comports()]
         return [entry.device for entry in list_ports.comports()]
 
     def monitor(self, frequency: int) -> None:
         """
         Send a monitor command to the robot
 
         :param int frequency: monitor frequency (Hz)
@@ -339,15 +338,14 @@
                 if self.last_sent_message is None or time.time() - self.last_sent_message > 1.0:
                     self.monitor(1)
 
                 # Sending pending packets
                 packet = self.pop_packet()
                 while packet is not None:
                     self.last_sent_message = time.time()
-                    self.last_sent_message = time.time()
                     if self.bt is not None and self.bt.is_open:
                         self.bt.write(packet.to_raw())
                     packet = self.pop_packet()
 
             except (OSError, serial.serialutil.SerialException) as e:
                 # In case of exception, we re-init the connection
                 logger.error(f"Error: {e}")
```

### Comparing `robot-soccer-kit-2.1.7/rsk/robots.py` & `robot-soccer-kit-2.1.8/rsk/robots.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/simulator.py` & `robot-soccer-kit-2.1.8/rsk/simulator.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/state.py` & `robot-soccer-kit-2.1.8/rsk/state.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-grid.css` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-grid.css.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-grid.min.css` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-grid.min.css.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-grid.rtl.css` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-reboot.css` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-reboot.css.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-reboot.min.css` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-utilities.css` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-utilities.css.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-utilities.min.css` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap.css` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap.css.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap.min.css` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap.min.css.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap.rtl.css` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap.rtl.css.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap.rtl.min.css` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.bundle.js` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.bundle.js.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.bundle.min.js` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.esm.js` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.esm.js.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.esm.min.js` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.esm.min.js.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.js` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.js.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.min.js` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/bootstrap/js/bootstrap.min.js.map` & `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/css/app.css` & `robot-soccer-kit-2.1.8/rsk/static/css/app.css`

 * *Files 17% similar despite different names*

```diff
@@ -1,232 +1,264 @@
 html {
     scroll-behavior: smooth;
-  }
-  
+}
+
 body {
-    font-size:20px;
+    font-size: 20px;
     position: relative;
 }
 
 
-.waiting-screen{
+.waiting-screen {
     position: fixed;
     z-index: 1;
     background-color: rgba(0, 0, 0, 0.8);
     width: 100%;
     height: 100%;
     display: inherit;
 }
-.loader-text{
+
+.loader-text {
     position: fixed;
     text-align: center;
     left: 50%;
     transform: translate(-50%, -50%);
     z-index: 2;
     top: calc(80%);
     font-size: 50px;
     color: white;
 }
 
-.loader-robot{
+.loader-robot {
     position: fixed;
     z-index: 2;
     left: calc(50% - 240px);
     top: calc(40% - 240px);
     width: 470px;
     height: 470px;
     animation: spin 5s linear infinite;
     animation-play-state: running;
 }
 
 @keyframes spin {
-    0% { transform: rotate(0deg); content: url("../imgs/robotblue1.svg"); }
-    25% { content: url("../imgs/robotgreen1.svg"); }
-    50% { content: url("../imgs/robotblue2.svg"); }
-    75% { content: url("../imgs/robotgreen2.svg"); }
-    100% { transform: rotate(360deg); }
+    0% {
+        transform: rotate(0deg);
+        content: url("../imgs/robotblue1.svg");
+    }
+
+    25% {
+        content: url("../imgs/robotgreen1.svg");
+    }
+
+    50% {
+        content: url("../imgs/robotblue2.svg");
+    }
+
+    75% {
+        content: url("../imgs/robotgreen2.svg");
+    }
+
+    100% {
+        transform: rotate(360deg);
+    }
 }
 
 .sim_vim {
     position: absolute;
     z-index: 0;
     opacity: 100;
 }
 
 .style_fps {
-    background-color:#333;
+    background-color: #333;
     margin-left: 0px;
-    font-size:28px;
-    text-align:center;
+    font-size: 28px;
+    text-align: center;
     min-width: 5em;
-  }
+}
 
 .card {
     filter: drop-shadow(-5px 5px 5px #ccc);
-    margin-bottom:20px;
+    margin-bottom: 20px;
 }
 
 .camera-area-referee {
-    width: 100%; 
+    width: 100%;
     height: calc(100vh - 357px);
 }
 
 .tchat-dim {
     height: calc(100vh - 477px)
 }
 
 .emergency-button {
-    position:fixed;
-    right:5px;
-    bottom:5px;
+    position: fixed;
+    right: 5px;
+    bottom: 5px;
 }
 
 .settings-button {
-    position:absolute;
-    left:18px;
-    top:84px;
+    position: absolute;
+    left: 18px;
+    top: 84px;
 }
 
 .camera-setting label {
-    text-align:right;
-    font-weight:bold;
+    text-align: right;
+    font-weight: bold;
 }
+
 .invisible {
-    opacity:0;
+    opacity: 0;
 }
 
 .vision-show-running {
-    display:none;
+    display: none;
 }
 
 .vision-running .vision-show-running {
-    display:block;
+    display: block;
 }
 
 .vision-running .vision-hide-running {
-    display:none;
+    display: none;
 }
 
 .vision-has-no-error {
-    display:none;
+    display: none;
 }
 
 .vision-no-error .vision-has-no-error {
-    display:inline;
+    display: inline;
 }
 
 .vision-no-error .vision-has-error {
-    display:none;
+    display: none;
 }
 
 
 .nav-item {
-    background-color:#333;
-    margin-right:5px;
+    background-color: #333;
+    margin-right: 5px;
 }
 
 .nav-link {
-    border-radius:5px;
-    border:2px solid transparent;
+    border-radius: 5px;
+    border: 2px solid transparent;
 }
 
 .nav-link.active {
-    background-color:#444;
-    border:2px solid white;
+    background-color: #444;
+    border: 2px solid white;
 }
 
 .robots-show-warning {
-    display:none;
+    display: none;
 }
 
 .control-show-warning {
-    display:none;
+    display: none;
 }
 
 .robots-warning .robots-show-warning {
-    display:inline;
+    display: inline;
 }
 
 .control-warning .control-show-warning {
-    display:inline;
+    display: inline;
 }
 
 .detection-wrapper {
-    min-height:150px;
+    min-height: 150px;
 }
 
-.bg-head-green{
+.bg-head-green {
     background-color: rgb(10, 148, 0);
 }
-.bg-body-green{
+
+.bg-body-green {
     background-color: rgba(10, 148, 0, 0.205);
 }
-.border-green{
-    border:1px solid rgb(10, 148, 0);
+
+.border-green {
+    border: 1px solid rgb(10, 148, 0);
 }
 
 /* .green-toast-position{
 } */
 
-.form_green_border:focus{
+.form_green_border:focus {
     border-color: #28a745;
     box-shadow: 0 0 0 0.2rem rgba(40, 167, 69, 0.25);
 }
 
 
 
 /* .bg-head-neutral{
 }
 .bg-body-neutral{
 }
 .border-neutral{
 } */
 
-.neutral-toast-position{
+.neutral-toast-position {
     margin-left: auto;
     margin-right: auto;
 }
 
 
 
-.bg-head-blue{
+.bg-head-blue {
     background-color: rgb(3, 102, 184);
 }
-.bg-body-blue{
-    background-color: rgb(3, 102, 184,0.205);
+
+.bg-body-blue {
+    background-color: rgb(3, 102, 184, 0.205);
 }
-.border-blue{
-    border:1px solid rgb(3, 102, 184);
+
+.border-blue {
+    border: 1px solid rgb(3, 102, 184);
 }
 
-.blue-toast-position{
-    margin-left: auto; 
+.blue-toast-position {
+    margin-left: auto;
     margin-right: 0;
 }
 
-.bg-body-grey{
+.bg-body-grey {
     background-color: rgba(180, 180, 180, 0.205);
 }
-.bg-body-red{
+
+.bg-body-red {
     background-color: rgba(250, 53, 69, 1);
 }
 
-.vert-align{
-  display:flex;
-  align-items:center;
+.vert-align {
+    display: flex;
+    align-items: center;
 }
 
-div.progress{
-  margin:0;
+div.progress {
+    margin: 0;
 }
 
-.progress-large{
+.progress-large {
     height: 20px;
 }
 
 .card-header {
     text-transform: capitalize;
 }
 
 .competition-mode {
-    display:none;
+    display: none;
+}
+
+.blinking {
+    animation: blinker 1s linear infinite;
+}
+
+@keyframes blinker {
+    50% {
+        opacity: 0;
+    }
 }
```

### Comparing `robot-soccer-kit-2.1.7/rsk/static/favicon.ico` & `robot-soccer-kit-2.1.8/rsk/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/icons/.fantasticonrc.js` & `robot-soccer-kit-2.1.8/rsk/static/icons/.fantasticonrc.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md` & `robot-soccer-kit-2.1.8/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/icons/.github/preview.png` & `robot-soccer-kit-2.1.8/rsk/static/icons/.github/preview.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/icons/.github/release-drafter.yml` & `robot-soccer-kit-2.1.8/rsk/static/icons/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/icons/.github/workflows/codeql.yml` & `robot-soccer-kit-2.1.8/rsk/static/icons/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/icons/.github/workflows/deploy.yml` & `robot-soccer-kit-2.1.8/rsk/static/icons/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/icons/.github/workflows/test.yml` & `robot-soccer-kit-2.1.8/rsk/static/icons/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/icons/LICENSE.md` & `robot-soccer-kit-2.1.8/rsk/static/icons/LICENSE.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/icons/README.md` & `robot-soccer-kit-2.1.8/rsk/static/icons/README.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/icons/bootstrap-icons.svg` & `robot-soccer-kit-2.1.8/rsk/static/icons/bootstrap-icons.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/icons/config.yml` & `robot-soccer-kit-2.1.8/rsk/static/icons/config.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/icons/font/bootstrap-icons.css` & `robot-soccer-kit-2.1.8/rsk/static/icons/font/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/icons/font/bootstrap-icons.json` & `robot-soccer-kit-2.1.8/rsk/static/icons/font/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/icons/font/fonts/bootstrap-icons.woff` & `robot-soccer-kit-2.1.8/rsk/static/icons/font/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/icons/font/fonts/bootstrap-icons.woff2` & `robot-soccer-kit-2.1.8/rsk/static/icons/font/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/icons/font/index.html` & `robot-soccer-kit-2.1.8/rsk/static/icons/font/index.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/icons/package-lock.json` & `robot-soccer-kit-2.1.8/rsk/static/icons/package-lock.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/icons/package.json` & `robot-soccer-kit-2.1.8/rsk/static/icons/package.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/icons/svg-sprite.json` & `robot-soccer-kit-2.1.8/rsk/static/icons/svg-sprite.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/icons/svgo.config.js` & `robot-soccer-kit-2.1.8/rsk/static/icons/svgo.config.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/imgs/ball.png` & `robot-soccer-kit-2.1.8/rsk/static/imgs/ball.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/imgs/ball_16x16.png` & `robot-soccer-kit-2.1.8/rsk/static/imgs/ball_16x16.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/imgs/ball_24x24.png` & `robot-soccer-kit-2.1.8/rsk/static/imgs/ball_24x24.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/imgs/ball_256x256.png` & `robot-soccer-kit-2.1.8/rsk/static/imgs/ball_256x256.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/imgs/ball_32x32.png` & `robot-soccer-kit-2.1.8/rsk/static/imgs/ball_32x32.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/imgs/ball_48x48.png` & `robot-soccer-kit-2.1.8/rsk/static/imgs/ball_48x48.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/imgs/field.png` & `robot-soccer-kit-2.1.8/rsk/static/imgs/field.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/imgs/field.svg` & `robot-soccer-kit-2.1.8/rsk/static/imgs/field.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/imgs/robot.svg` & `robot-soccer-kit-2.1.8/rsk/static/imgs/robot.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/imgs/robotblue1.svg` & `robot-soccer-kit-2.1.8/rsk/static/imgs/robotblue1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/imgs/robotblue2.svg` & `robot-soccer-kit-2.1.8/rsk/static/imgs/robotblue2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/imgs/robotgreen1.svg` & `robot-soccer-kit-2.1.8/rsk/static/imgs/robotgreen1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/imgs/robotgreen2.svg` & `robot-soccer-kit-2.1.8/rsk/static/imgs/robotgreen2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/index.html` & `robot-soccer-kit-2.1.8/rsk/static/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -16,28 +16,26 @@
 <script type="text/javascript" src="static/js/control.js"></script>
 <script type="text/javascript" src="static/js/tabs.js"></script>
 <script type="text/javascript" src="static/js/app.js"></script>
 <link rel="shortcut icon" href="static/favicon.ico" type="image/x-icon">
 <title>Robot Soccer Kit</title>
 </head>
 
-<div class="waiting-screen">
-    <div class="opacifier"></div>
-    <img class="loader-robot" src="static/imgs/robotblue1.svg">
-    <b class="loader-text" class="bi bi-play-fill"> No Python Back-End </b>
-</div>
-
-
 
 <nav class="navbar navbar-expand navbar-dark bg-dark">
     <div class="container-fluid">
-        <a class="navbar-brand" href="#">
-            <img src="static/imgs/ball.png" width="32" />
-            Robot Soccer Kit
-        </a>
+        <div>
+            <a class="navbar-brand" href="#">
+                <img src="static/imgs/ball.png" width="32" />
+                Robot Soccer Kit
+            </a>
+            <div class="text-danger blinking no-backend">
+                <small>No Python Backend</small>
+            </div>
+        </div>
 
         <ul class="navbar-nav">
             <li class="nav-item rounded nav-tab not_show_simulated" rel="vision">
                 <a class="nav-link active" aria-current="page" href="#">
                     <span class="input-group">
                         <i class="bi bi-webcam"></i>&nbsp;
                         Vision&nbsp;
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-[static/imgs/robotblue1.svg]NNoo PPyytthhoonn BBaacckk--EEnndd
 _[_s_t_a_t_i_c_/_i_m_g_s_/_b_a_l_l_._p_n_g_]_R_o_b_o_t_ _S_o_c_c_e_r_ _K_i_t
+No Python Backend
     * _ _ _V_i_s_i_o_n_ 
     * _ _ _R_o_b_o_t_s_ _ _[_0_/_0_]
     * _ _ _C_o_n_t_r_o_l
     * _ _ _R_e_f_e_r_e_e
     * _ _ _C_o_m_p_e_t_i_t_i_o_n
 CCaammeerraa ddeetteeccttiioonn
 Refresh cameras Start Vision
```

### Comparing `robot-soccer-kit-2.1.7/rsk/static/jquery/jquery.js` & `robot-soccer-kit-2.1.8/rsk/static/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/js/app.js` & `robot-soccer-kit-2.1.8/rsk/static/js/app.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -16,30 +16,28 @@
                     $.get({
                         "url": url,
                         "data": {
                             'command': name,
                             'args': JSON.stringify(args)
                         },
                         'success': function(result) {
-                            $('.waiting-screen').css("display", 'None')
-                            $('.loader-robot').css("animation-play-state", 'paused')
+                            $('.no-backend').css("display", 'none')
                             if (result) {
                                 if (result[0]) {
                                     if (callback) {
                                         callback(result[1]);
                                     }
                                 } else {
                                     console.log('Error: ' + result[1]);
                                 }
                             }
                         },
                         "timeout": timeout
                     }).fail(function() {
-                        $('.waiting-screen').css("display", 'inherit')
-                        $('.loader-robot').css("animation-play-state", 'running')
+                        $('.no-backend').css("display", 'inherit')
                     });;
                 }
             }
         });
     }
 }
```

### Comparing `robot-soccer-kit-2.1.7/rsk/static/js/competition.js` & `robot-soccer-kit-2.1.8/rsk/static/js/competition.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/js/control.js` & `robot-soccer-kit-2.1.8/rsk/static/js/control.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -8,20 +8,20 @@
                 backend.allow_team_control(team, $(this).is(':checked'));
             });
 
             $('.key-' + team).change(function() {
                 backend.set_key(team, $(this).val());
             });
 
-            $('.key-' + team).focus(function() {
-                $(this).attr('type', 'text');
-            });
-            $('.key-' + team).blur(function() {
-                $(this).attr('type', 'password');
-            });
+            // $('.key-'+team).focus(function() {
+            //     $(this).attr('type', 'text');
+            // });
+            // $('.key-'+team).blur(function() {
+            //     $(this).attr('type', 'password');
+            // });
         }
 
         $('.emergency').click(function() {
             backend.emergency();
         });
 
         setInterval(function() {
```

### Comparing `robot-soccer-kit-2.1.7/rsk/static/js/referee.js` & `robot-soccer-kit-2.1.8/rsk/static/js/referee.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/js/robots.js` & `robot-soccer-kit-2.1.8/rsk/static/js/robots.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/js/simulator.js` & `robot-soccer-kit-2.1.8/rsk/static/js/simulator.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/js/video.js` & `robot-soccer-kit-2.1.8/rsk/static/js/video.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/markers/blue1.svg` & `robot-soccer-kit-2.1.8/rsk/static/markers/blue1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/markers/blue2.svg` & `robot-soccer-kit-2.1.8/rsk/static/markers/blue2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/markers/green1.svg` & `robot-soccer-kit-2.1.8/rsk/static/markers/green1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/markers/green2.svg` & `robot-soccer-kit-2.1.8/rsk/static/markers/green2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/referee_event_team.html` & `robot-soccer-kit-2.1.8/rsk/static/referee_event_team.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/robot.html` & `robot-soccer-kit-2.1.8/rsk/static/robot.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/static/team.html` & `robot-soccer-kit-2.1.8/rsk/static/team.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/tasks.py` & `robot-soccer-kit-2.1.8/rsk/tasks.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/utils.py` & `robot-soccer-kit-2.1.8/rsk/utils.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/rsk/video.py` & `robot-soccer-kit-2.1.8/rsk/video.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.7/setup.py` & `robot-soccer-kit-2.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         for filename in filenames:
             if "__pycache__" not in path:
                 paths.append(os.path.join("..", path, filename))
     return paths
 
 setuptools.setup(
     name="robot-soccer-kit",
-    version="2.1.7",
+    version="2.1.8",
     author="Rhoban team",
     author_email="team@rhoban.com",
     description="Robot Soccer Kit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rhoban/robot-soccer-kit/",
     packages=setuptools.find_packages(),
```


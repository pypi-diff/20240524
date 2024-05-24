# Comparing `tmp/qtica-0.4.3.tar.gz` & `tmp/qtica-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtica-0.4.3.tar", max compression
+gzip compressed data, was "qtica-0.5.0.tar", max compression
```

## Comparing `qtica-0.4.3.tar` & `qtica-0.5.0.tar`

### file list

```diff
@@ -1,394 +1,394 @@
--rw-r--r--   0        0        0    16187 2024-03-05 01:57:26.430473 qtica-0.4.3/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2023-09-14 22:18:47.247695 qtica-0.4.3/LICENSE
--rw-r--r--   0        0        0      212 2024-03-05 01:49:44.234853 qtica-0.4.3/Qtica/__init__.py
--rw-r--r--   0        0        0      175 2024-01-05 15:19:55.230374 qtica-0.4.3/Qtica/animations/__init__.py
--rw-r--r--   0        0        0      705 2024-01-11 22:54:05.655130 qtica-0.4.3/Qtica/animations/parallel_animation_group.py
--rw-r--r--   0        0        0      533 2024-01-05 15:19:26.149384 qtica-0.4.3/Qtica/animations/property_animation.py
--rw-r--r--   0        0        0      713 2024-01-05 15:19:22.549261 qtica-0.4.3/Qtica/animations/sequential_animation_group.py
--rw-r--r--   0        0        0      579 2024-01-18 19:06:04.263963 qtica-0.4.3/Qtica/core/__init__.py
--rw-r--r--   0        0        0      923 2024-01-25 21:21:57.052922 qtica-0.4.3/Qtica/core/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7545 2024-02-19 11:13:10.419471 qtica-0.4.3/Qtica/core/__pycache__/_base.cpython-310.pyc
--rw-r--r--   0        0        0     1434 2024-01-25 21:21:57.685539 qtica-0.4.3/Qtica/core/__pycache__/_config.cpython-310.pyc
--rw-r--r--   0        0        0     2891 2024-01-25 21:21:57.673527 qtica-0.4.3/Qtica/core/__pycache__/_declarative.cpython-310.pyc
--rw-r--r--   0        0        0     2107 2024-01-25 21:21:57.685539 qtica-0.4.3/Qtica/core/__pycache__/_dialog.cpython-310.pyc
--rw-r--r--   0        0        0     1836 2024-01-25 21:21:57.685539 qtica-0.4.3/Qtica/core/__pycache__/_icons.cpython-310.pyc
--rw-r--r--   0        0        0     1657 2024-01-25 21:21:57.685539 qtica-0.4.3/Qtica/core/__pycache__/_painter.cpython-310.pyc
--rw-r--r--   0        0        0      542 2024-01-25 21:21:57.681535 qtica-0.4.3/Qtica/core/__pycache__/_qobject.cpython-310.pyc
--rw-r--r--   0        0        0     1806 2024-02-18 20:16:45.707284 qtica-0.4.3/Qtica/core/__pycache__/_tool.cpython-310.pyc
--rw-r--r--   0        0        0     3186 2024-01-25 21:21:57.681535 qtica-0.4.3/Qtica/core/__pycache__/_widget.cpython-310.pyc
--rw-r--r--   0        0        0     3221 2024-02-03 21:25:57.155488 qtica-0.4.3/Qtica/core/__pycache__/api.cpython-310.pyc
--rw-r--r--   0        0        0      878 2024-01-25 21:21:57.689543 qtica-0.4.3/Qtica/core/__pycache__/exception_handler.cpython-310.pyc
--rw-r--r--   0        0        0     9335 2024-02-23 20:45:00.442205 qtica-0.4.3/Qtica/core/__pycache__/qstyle_sheet.cpython-310.pyc
--rw-r--r--   0        0        0     2372 2024-01-25 21:21:57.689543 qtica-0.4.3/Qtica/core/__pycache__/routes.cpython-310.pyc
--rw-r--r--   0        0        0     7606 2024-02-18 20:32:17.363264 qtica-0.4.3/Qtica/core/_base.py
--rw-r--r--   0        0        0      643 2024-01-08 19:18:09.498861 qtica-0.4.3/Qtica/core/_config.py
--rw-r--r--   0        0        0     1959 2024-01-04 02:21:46.887848 qtica-0.4.3/Qtica/core/_declarative.py
--rw-r--r--   0        0        0     1513 2024-01-23 18:48:11.987820 qtica-0.4.3/Qtica/core/_dialog.py
--rw-r--r--   0        0        0     1410 2024-01-08 21:41:19.748815 qtica-0.4.3/Qtica/core/_icons.py
--rw-r--r--   0        0        0      748 2024-01-03 15:08:05.410277 qtica-0.4.3/Qtica/core/_painter.py
--rw-r--r--   0        0        0      196 2023-12-25 20:16:29.144530 qtica-0.4.3/Qtica/core/_qobject.py
--rw-r--r--   0        0        0     1299 2024-02-18 20:16:11.295285 qtica-0.4.3/Qtica/core/_tool.py
--rw-r--r--   0        0        0     2695 2024-01-23 18:46:53.212010 qtica-0.4.3/Qtica/core/_widget.py
--rw-r--r--   0        0        0     3335 2024-02-03 20:51:32.215532 qtica-0.4.3/Qtica/core/api.py
--rw-r--r--   0        0        0      702 2024-01-18 19:05:19.140292 qtica-0.4.3/Qtica/core/exception_handler.py
--rw-r--r--   0        0        0     9463 2024-02-19 18:12:29.534835 qtica-0.4.3/Qtica/core/qstyle_sheet.py
--rw-r--r--   0        0        0     1336 2024-01-08 20:43:54.389124 qtica-0.4.3/Qtica/core/routes.py
--rw-r--r--   0        0        0       23 2024-01-11 22:51:54.923036 qtica-0.4.3/Qtica/effects/__init__.py
--rw-r--r--   0        0        0      200 2024-01-12 10:41:21.758783 qtica-0.4.3/Qtica/effects/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      372 2024-01-09 16:19:44.099527 qtica-0.4.3/Qtica/effects/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     1545 2024-01-12 10:41:21.770838 qtica-0.4.3/Qtica/effects/__pycache__/_effects.cpython-310.pyc
--rw-r--r--   0        0        0      688 2024-01-11 17:21:56.306866 qtica-0.4.3/Qtica/effects/__pycache__/blur.cpython-310.pyc
--rw-r--r--   0        0        0      818 2024-01-09 16:19:44.103527 qtica-0.4.3/Qtica/effects/__pycache__/blur.cpython-312.pyc
--rw-r--r--   0        0        0      704 2023-12-26 19:43:34.947780 qtica-0.4.3/Qtica/effects/__pycache__/colorize.cpython-310.pyc
--rw-r--r--   0        0        0      834 2024-01-09 16:19:44.099527 qtica-0.4.3/Qtica/effects/__pycache__/colorize.cpython-312.pyc
--rw-r--r--   0        0        0      676 2023-12-26 19:43:34.947780 qtica-0.4.3/Qtica/effects/__pycache__/drop_shadow.cpython-310.pyc
--rw-r--r--   0        0        0      799 2024-01-09 16:19:44.099527 qtica-0.4.3/Qtica/effects/__pycache__/drop_shadow.cpython-312.pyc
--rw-r--r--   0        0        0    13226 2024-01-02 22:50:03.747969 qtica-0.4.3/Qtica/effects/__pycache__/neumorphism.cpython-310.pyc
--rw-r--r--   0        0        0      700 2023-12-26 19:43:34.947780 qtica-0.4.3/Qtica/effects/__pycache__/opacity.cpython-310.pyc
--rw-r--r--   0        0        0      830 2024-01-09 16:19:44.099527 qtica-0.4.3/Qtica/effects/__pycache__/opacity.cpython-312.pyc
--rw-r--r--   0        0        0      966 2024-01-11 22:53:08.395089 qtica-0.4.3/Qtica/effects/_effects.py
--rw-r--r--   0        0        0      319 2024-01-08 18:17:03.666028 qtica-0.4.3/Qtica/enums/__init__.py
--rw-r--r--   0        0        0      619 2024-01-09 16:49:43.271749 qtica-0.4.3/Qtica/enums/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      638 2024-01-08 18:17:07.270386 qtica-0.4.3/Qtica/enums/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     1845 2023-11-08 02:29:24.001067 qtica-0.4.3/Qtica/enums/__pycache__/_abs_icons.cpython-310.pyc
--rw-r--r--   0        0        0      461 2023-11-04 22:14:44.127618 qtica-0.4.3/Qtica/enums/__pycache__/animation.cpython-310.pyc
--rw-r--r--   0        0        0      458 2023-11-04 22:14:44.127618 qtica-0.4.3/Qtica/enums/__pycache__/clipboard.cpython-310.pyc
--rw-r--r--   0        0        0    70891 2024-01-13 03:14:56.143252 qtica-0.4.3/Qtica/enums/__pycache__/colors.cpython-310.pyc
--rw-r--r--   0        0        0   106081 2024-01-08 18:16:32.442869 qtica-0.4.3/Qtica/enums/__pycache__/colors.cpython-312.pyc
--rw-r--r--   0        0        0     2476 2023-12-25 20:05:00.112545 qtica-0.4.3/Qtica/enums/__pycache__/env_vars.cpython-310.pyc
--rw-r--r--   0        0        0     2823 2024-01-08 18:16:32.718897 qtica-0.4.3/Qtica/enums/__pycache__/env_vars.cpython-312.pyc
--rw-r--r--   0        0        0     2169 2024-01-25 21:16:05.106523 qtica-0.4.3/Qtica/enums/__pycache__/events.cpython-310.pyc
--rw-r--r--   0        0        0     4487 2024-01-08 21:45:19.215511 qtica-0.4.3/Qtica/enums/__pycache__/events.cpython-312.pyc
--rw-r--r--   0        0        0      511 2023-12-26 19:32:50.343794 qtica-0.4.3/Qtica/enums/__pycache__/position.cpython-310.pyc
--rw-r--r--   0        0        0      616 2024-01-08 18:16:32.730898 qtica-0.4.3/Qtica/enums/__pycache__/position.cpython-312.pyc
--rw-r--r--   0        0        0      802 2023-11-04 22:14:44.127618 qtica-0.4.3/Qtica/enums/__pycache__/qpa_plugins.cpython-310.pyc
--rw-r--r--   0        0        0      979 2024-01-08 18:16:32.730898 qtica-0.4.3/Qtica/enums/__pycache__/qpa_plugins.cpython-312.pyc
--rw-r--r--   0        0        0    10087 2023-11-04 22:14:43.383580 qtica-0.4.3/Qtica/enums/__pycache__/signals.cpython-310.pyc
--rw-r--r--   0        0        0    19942 2024-01-08 18:16:32.606886 qtica-0.4.3/Qtica/enums/__pycache__/signals.cpython-312.pyc
--rw-r--r--   0        0        0      449 2024-01-09 16:49:43.755755 qtica-0.4.3/Qtica/enums/__pycache__/size.cpython-310.pyc
--rw-r--r--   0        0        0      522 2024-01-08 18:16:32.750900 qtica-0.4.3/Qtica/enums/__pycache__/size.cpython-312.pyc
--rw-r--r--   0        0        0      503 2023-11-04 22:14:44.127618 qtica-0.4.3/Qtica/enums/__pycache__/smooth_scroll.cpython-310.pyc
--rw-r--r--   0        0        0      945 2024-01-03 03:22:33.775041 qtica-0.4.3/Qtica/enums/__pycache__/teaching_tip_tails.cpython-310.pyc
--rw-r--r--   0        0        0      406 2024-01-09 16:49:43.803755 qtica-0.4.3/Qtica/enums/__pycache__/theme.cpython-310.pyc
--rw-r--r--   0        0        0      460 2024-01-08 18:17:07.430402 qtica-0.4.3/Qtica/enums/__pycache__/theme.cpython-312.pyc
--rw-r--r--   0        0        0    11452 2024-01-25 21:16:05.026543 qtica-0.4.3/Qtica/enums/__pycache__/widgets.cpython-310.pyc
--rw-r--r--   0        0        0    18255 2024-01-08 18:16:32.670892 qtica-0.4.3/Qtica/enums/__pycache__/widgets.cpython-312.pyc
--rw-r--r--   0        0        0    65688 2024-01-12 10:55:38.251360 qtica-0.4.3/Qtica/enums/colors.py
--rw-r--r--   0        0        0     1894 2023-12-18 12:17:46.147253 qtica-0.4.3/Qtica/enums/env_vars.py
--rw-r--r--   0        0        0     1931 2024-01-23 18:57:02.170893 qtica-0.4.3/Qtica/enums/events.py
--rw-r--r--   0        0        0      221 2023-12-25 20:41:14.660498 qtica-0.4.3/Qtica/enums/position.py
--rw-r--r--   0        0        0      457 2023-10-20 20:59:31.512597 qtica-0.4.3/Qtica/enums/qpa_plugins.py
--rw-r--r--   0        0        0    10582 2023-10-20 20:58:21.160688 qtica-0.4.3/Qtica/enums/signals.py
--rw-r--r--   0        0        0      151 2024-01-06 00:13:48.065418 qtica-0.4.3/Qtica/enums/size.py
--rw-r--r--   0        0        0       85 2024-01-05 23:36:52.732478 qtica-0.4.3/Qtica/enums/theme.py
--rw-r--r--   0        0        0    11181 2024-01-23 19:11:15.515182 qtica-0.4.3/Qtica/enums/widgets.py
--rw-r--r--   0        0        0      294 2024-01-06 00:22:24.430372 qtica-0.4.3/Qtica/layouts/__init__.py
--rw-r--r--   0        0        0      531 2024-01-11 17:21:56.198866 qtica-0.4.3/Qtica/layouts/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      552 2024-01-08 21:14:34.756360 qtica-0.4.3/Qtica/layouts/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     5477 2024-01-12 10:41:21.710566 qtica-0.4.3/Qtica/layouts/__pycache__/border_layout.cpython-310.pyc
--rw-r--r--   0        0        0    10477 2024-01-08 21:14:34.764360 qtica-0.4.3/Qtica/layouts/__pycache__/border_layout.cpython-312.pyc
--rw-r--r--   0        0        0     4534 2024-01-02 22:57:20.982628 qtica-0.4.3/Qtica/layouts/__pycache__/expand_layout.cpython-310.pyc
--rw-r--r--   0        0        0     7670 2024-01-26 22:00:39.598621 qtica-0.4.3/Qtica/layouts/__pycache__/flow_layout.cpython-310.pyc
--rw-r--r--   0        0        0    12304 2024-01-08 21:14:34.768360 qtica-0.4.3/Qtica/layouts/__pycache__/flow_layout.cpython-312.pyc
--rw-r--r--   0        0        0     1283 2024-01-26 22:00:39.594621 qtica-0.4.3/Qtica/layouts/__pycache__/form_layout.cpython-310.pyc
--rw-r--r--   0        0        0     2071 2024-01-08 21:14:34.760360 qtica-0.4.3/Qtica/layouts/__pycache__/form_layout.cpython-312.pyc
--rw-r--r--   0        0        0     1405 2024-01-11 17:21:56.202866 qtica-0.4.3/Qtica/layouts/__pycache__/grid_layout.cpython-310.pyc
--rw-r--r--   0        0        0     2314 2024-01-08 21:14:34.760360 qtica-0.4.3/Qtica/layouts/__pycache__/grid_layout.cpython-312.pyc
--rw-r--r--   0        0        0     1597 2024-01-26 22:00:39.594621 qtica-0.4.3/Qtica/layouts/__pycache__/h_layout.cpython-310.pyc
--rw-r--r--   0        0        0     2576 2024-01-08 21:14:34.760360 qtica-0.4.3/Qtica/layouts/__pycache__/h_layout.cpython-312.pyc
--rw-r--r--   0        0        0     1129 2024-01-26 22:00:39.594621 qtica-0.4.3/Qtica/layouts/__pycache__/stacked.cpython-310.pyc
--rw-r--r--   0        0        0     1721 2024-01-08 21:14:34.764360 qtica-0.4.3/Qtica/layouts/__pycache__/stacked.cpython-312.pyc
--rw-r--r--   0        0        0     1591 2024-01-26 22:00:39.594621 qtica-0.4.3/Qtica/layouts/__pycache__/v_layout.cpython-310.pyc
--rw-r--r--   0        0        0     2570 2024-01-08 21:14:34.764360 qtica-0.4.3/Qtica/layouts/__pycache__/v_layout.cpython-312.pyc
--rw-r--r--   0        0        0     6615 2024-01-11 22:58:24.419318 qtica-0.4.3/Qtica/layouts/border_layout.py
--rw-r--r--   0        0        0     7477 2024-01-26 21:59:56.853300 qtica-0.4.3/Qtica/layouts/flow_layout.py
--rw-r--r--   0        0        0     1453 2024-01-26 21:58:10.501833 qtica-0.4.3/Qtica/layouts/form_layout.py
--rw-r--r--   0        0        0     1834 2024-01-10 17:17:48.310835 qtica-0.4.3/Qtica/layouts/grid_layout.py
--rw-r--r--   0        0        0     1863 2024-01-26 21:57:33.516549 qtica-0.4.3/Qtica/layouts/h_layout.py
--rw-r--r--   0        0        0     1057 2024-01-26 21:59:36.824668 qtica-0.4.3/Qtica/layouts/stacked.py
--rw-r--r--   0        0        0     1854 2024-01-26 21:55:25.847683 qtica-0.4.3/Qtica/layouts/v_layout.py
--rw-r--r--   0        0        0       93 2024-01-03 23:21:20.488233 qtica-0.4.3/Qtica/painters/__init__.py
--rw-r--r--   0        0        0      296 2024-01-03 23:21:59.861489 qtica-0.4.3/Qtica/painters/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      302 2024-01-08 21:34:02.103270 qtica-0.4.3/Qtica/painters/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0    12804 2024-01-03 15:48:57.470679 qtica-0.4.3/Qtica/painters/__pycache__/_tails.cpython-310.pyc
--rw-r--r--   0        0        0     3680 2024-02-07 22:28:14.820701 qtica-0.4.3/Qtica/painters/__pycache__/circular_progress.cpython-310.pyc
--rw-r--r--   0        0        0     6465 2024-01-08 21:34:02.103270 qtica-0.4.3/Qtica/painters/__pycache__/circular_progress.cpython-312.pyc
--rw-r--r--   0        0        0     3157 2024-02-14 21:22:24.140184 qtica-0.4.3/Qtica/painters/__pycache__/status_edge.cpython-310.pyc
--rw-r--r--   0        0        0     4447 2024-01-08 22:46:03.445258 qtica-0.4.3/Qtica/painters/__pycache__/status_edge.cpython-312.pyc
--rw-r--r--   0        0        0     1583 2024-01-03 15:57:26.454986 qtica-0.4.3/Qtica/painters/__pycache__/teaching_tip.cpython-310.pyc
--rw-r--r--   0        0        0     3218 2024-01-30 23:56:24.180177 qtica-0.4.3/Qtica/painters/circular_progress.py
--rw-r--r--   0        0        0     3438 2024-02-14 21:22:18.647958 qtica-0.4.3/Qtica/painters/status_edge.py
--rw-r--r--   0        0        0      364 2024-01-25 22:53:45.089782 qtica-0.4.3/Qtica/services/__init__.py
--rw-r--r--   0        0        0      637 2024-01-25 22:55:08.082550 qtica-0.4.3/Qtica/services/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      638 2024-01-09 22:33:14.059975 qtica-0.4.3/Qtica/services/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     5540 2024-02-03 21:25:57.519488 qtica-0.4.3/Qtica/services/__pycache__/_methods.cpython-310.pyc
--rw-r--r--   0        0        0     7881 2024-01-09 23:00:50.721630 qtica-0.4.3/Qtica/services/__pycache__/_methods.cpython-312.pyc
--rw-r--r--   0        0        0     1841 2024-01-10 15:38:23.900699 qtica-0.4.3/Qtica/services/__pycache__/clipboard.cpython-310.pyc
--rw-r--r--   0        0        0     2934 2024-01-08 20:53:27.464991 qtica-0.4.3/Qtica/services/__pycache__/clipboard.cpython-312.pyc
--rw-r--r--   0        0        0      424 2023-12-30 23:29:51.645175 qtica-0.4.3/Qtica/services/__pycache__/dialogs.cpython-310.pyc
--rw-r--r--   0        0        0     2062 2024-01-10 15:38:23.936698 qtica-0.4.3/Qtica/services/__pycache__/launche_url.cpython-310.pyc
--rw-r--r--   0        0        0     2902 2024-01-08 20:53:27.468991 qtica-0.4.3/Qtica/services/__pycache__/launche_url.cpython-312.pyc
--rw-r--r--   0        0        0     3715 2024-01-10 15:38:23.916699 qtica-0.4.3/Qtica/services/__pycache__/message_handler.cpython-310.pyc
--rw-r--r--   0        0        0     5190 2024-01-08 20:53:27.464991 qtica-0.4.3/Qtica/services/__pycache__/message_handler.cpython-312.pyc
--rw-r--r--   0        0        0     4482 2024-02-03 20:59:04.859522 qtica-0.4.3/Qtica/services/_methods.py
--rw-r--r--   0        0        0     1459 2024-01-05 15:32:29.184574 qtica-0.4.3/Qtica/services/clipboard.py
--rw-r--r--   0        0        0     1584 2024-01-05 19:43:31.326908 qtica-0.4.3/Qtica/services/launche_url.py
--rw-r--r--   0        0        0     3066 2024-01-05 22:05:02.546983 qtica-0.4.3/Qtica/services/message_handler.py
--rw-r--r--   0        0        0      556 2024-02-23 21:06:58.288180 qtica-0.4.3/Qtica/tools/__init__.py
--rw-r--r--   0        0        0      871 2024-02-23 21:10:10.751616 qtica-0.4.3/Qtica/tools/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      989 2024-01-09 20:38:36.585517 qtica-0.4.3/Qtica/tools/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     3309 2024-02-03 21:25:57.511488 qtica-0.4.3/Qtica/tools/__pycache__/action.cpython-310.pyc
--rw-r--r--   0        0        0     5523 2024-01-08 20:53:27.420990 qtica-0.4.3/Qtica/tools/__pycache__/action.cpython-312.pyc
--rw-r--r--   0        0        0      754 2023-12-28 21:18:56.132086 qtica-0.4.3/Qtica/tools/__pycache__/alignment.cpython-310.pyc
--rw-r--r--   0        0        0      933 2024-01-08 20:53:27.416990 qtica-0.4.3/Qtica/tools/__pycache__/alignment.cpython-312.pyc
--rw-r--r--   0        0        0      620 2024-01-10 15:38:23.748707 qtica-0.4.3/Qtica/tools/__pycache__/brush.cpython-310.pyc
--rw-r--r--   0        0        0      742 2024-01-08 21:47:19.287555 qtica-0.4.3/Qtica/tools/__pycache__/brush.cpython-312.pyc
--rw-r--r--   0        0        0      858 2023-10-24 03:26:38.665477 qtica-0.4.3/Qtica/tools/__pycache__/center.cpython-310.pyc
--rw-r--r--   0        0        0      750 2024-01-09 16:49:45.043770 qtica-0.4.3/Qtica/tools/__pycache__/color.cpython-310.pyc
--rw-r--r--   0        0        0      968 2024-01-08 20:53:27.408990 qtica-0.4.3/Qtica/tools/__pycache__/color.cpython-312.pyc
--rw-r--r--   0        0        0     5053 2024-01-11 17:21:33.738867 qtica-0.4.3/Qtica/tools/__pycache__/copy_progress.cpython-310.pyc
--rw-r--r--   0        0        0     8627 2024-01-08 20:53:27.384990 qtica-0.4.3/Qtica/tools/__pycache__/copy_progress.cpython-312.pyc
--rw-r--r--   0        0        0     2084 2024-01-25 22:48:10.494644 qtica-0.4.3/Qtica/tools/__pycache__/elided_text.cpython-310.pyc
--rw-r--r--   0        0        0     3016 2024-01-08 20:53:27.376990 qtica-0.4.3/Qtica/tools/__pycache__/elided_text.cpython-312.pyc
--rw-r--r--   0        0        0     1420 2023-12-15 19:46:03.309951 qtica-0.4.3/Qtica/tools/__pycache__/env_var.cpython-310.pyc
--rw-r--r--   0        0        0     2590 2024-01-04 00:30:03.155692 qtica-0.4.3/Qtica/tools/__pycache__/icon.cpython-310.pyc
--rw-r--r--   0        0        0     4253 2024-01-08 20:53:27.408990 qtica-0.4.3/Qtica/tools/__pycache__/icon.cpython-312.pyc
--rw-r--r--   0        0        0      657 2024-01-10 15:38:23.768706 qtica-0.4.3/Qtica/tools/__pycache__/linear_gradient.cpython-310.pyc
--rw-r--r--   0        0        0      781 2024-01-09 20:38:36.613517 qtica-0.4.3/Qtica/tools/__pycache__/linear_gradient.cpython-312.pyc
--rw-r--r--   0        0        0     1120 2023-10-20 21:31:44.954090 qtica-0.4.3/Qtica/tools/__pycache__/modifiers.cpython-310.pyc
--rw-r--r--   0        0        0     1790 2024-01-08 20:53:27.412990 qtica-0.4.3/Qtica/tools/__pycache__/modifiers.cpython-312.pyc
--rw-r--r--   0        0        0     3549 2024-02-03 21:25:57.459488 qtica-0.4.3/Qtica/tools/__pycache__/movie.cpython-310.pyc
--rw-r--r--   0        0        0     5372 2024-01-08 20:53:27.424991 qtica-0.4.3/Qtica/tools/__pycache__/movie.cpython-312.pyc
--rw-r--r--   0        0        0     3107 2023-12-12 00:58:38.762160 qtica-0.4.3/Qtica/tools/__pycache__/movie_view.cpython-310.pyc
--rw-r--r--   0        0        0     1097 2023-11-25 19:52:04.430529 qtica-0.4.3/Qtica/tools/__pycache__/painter.cpython-310.pyc
--rw-r--r--   0        0        0      612 2024-01-10 15:38:23.748707 qtica-0.4.3/Qtica/tools/__pycache__/pen.cpython-310.pyc
--rw-r--r--   0        0        0      734 2024-01-08 21:47:19.287555 qtica-0.4.3/Qtica/tools/__pycache__/pen.cpython-312.pyc
--rw-r--r--   0        0        0     2151 2023-12-07 21:52:01.116620 qtica-0.4.3/Qtica/tools/__pycache__/picker.cpython-310.pyc
--rw-r--r--   0        0        0     5334 2023-12-26 19:35:47.115790 qtica-0.4.3/Qtica/tools/__pycache__/qstyle_sheet.cpython-310.pyc
--rw-r--r--   0        0        0     1287 2024-02-14 20:13:11.603835 qtica-0.4.3/Qtica/tools/__pycache__/qt_file_open.cpython-310.pyc
--rw-r--r--   0        0        0     1490 2024-01-08 20:53:27.372990 qtica-0.4.3/Qtica/tools/__pycache__/qt_file_open.cpython-312.pyc
--rw-r--r--   0        0        0     5399 2024-02-14 20:13:11.611836 qtica-0.4.3/Qtica/tools/__pycache__/settings.cpython-310.pyc
--rw-r--r--   0        0        0     7778 2024-01-08 20:53:27.428990 qtica-0.4.3/Qtica/tools/__pycache__/settings.cpython-312.pyc
--rw-r--r--   0        0        0     1165 2024-02-03 21:25:57.467488 qtica-0.4.3/Qtica/tools/__pycache__/size_policy.cpython-310.pyc
--rw-r--r--   0        0        0     1681 2024-01-08 20:53:27.412990 qtica-0.4.3/Qtica/tools/__pycache__/size_policy.cpython-312.pyc
--rw-r--r--   0        0        0     4170 2024-01-09 16:49:44.975769 qtica-0.4.3/Qtica/tools/__pycache__/smooth_scroll.cpython-310.pyc
--rw-r--r--   0        0        0     7792 2024-01-08 20:53:27.392990 qtica-0.4.3/Qtica/tools/__pycache__/smooth_scroll.cpython-312.pyc
--rw-r--r--   0        0        0     1625 2023-10-14 15:42:21.017644 qtica-0.4.3/Qtica/tools/__pycache__/svg_color.cpython-310.pyc
--rw-r--r--   0        0        0     1275 2024-01-09 16:49:45.179771 qtica-0.4.3/Qtica/tools/__pycache__/system_tray.cpython-310.pyc
--rw-r--r--   0        0        0     1744 2024-01-08 20:53:27.420990 qtica-0.4.3/Qtica/tools/__pycache__/system_tray.cpython-312.pyc
--rw-r--r--   0        0        0      977 2024-01-11 17:21:33.606867 qtica-0.4.3/Qtica/tools/__pycache__/ui_loader.cpython-310.pyc
--rw-r--r--   0        0        0     1100 2024-01-08 20:53:27.268989 qtica-0.4.3/Qtica/tools/__pycache__/ui_loader.cpython-312.pyc
--rw-r--r--   0        0        0     2358 2024-02-03 20:33:56.351554 qtica-0.4.3/Qtica/tools/action.py
--rw-r--r--   0        0        0      367 2024-01-05 22:40:37.553867 qtica-0.4.3/Qtica/tools/color.py
--rwxr-xr-x   0        0        0     5159 2024-01-10 17:35:50.234877 qtica-0.4.3/Qtica/tools/copy_progress.py
--rw-r--r--   0        0        0     2873 2024-01-04 00:27:21.814009 qtica-0.4.3/Qtica/tools/icon.py
--rw-r--r--   0        0        0      299 2024-02-23 21:11:01.536301 qtica-0.4.3/Qtica/tools/list_widget_item.py
--rw-r--r--   0        0        0      551 2024-02-19 18:23:21.195464 qtica-0.4.3/Qtica/tools/media_player.py
--rw-r--r--   0        0        0     2579 2024-02-03 20:29:22.499560 qtica-0.4.3/Qtica/tools/movie.py
--rw-r--r--   0        0        0      586 2024-02-14 20:08:53.334132 qtica-0.4.3/Qtica/tools/qt_file_open.py
--rw-r--r--   0        0        0       63 2024-01-19 16:22:59.600859 qtica-0.4.3/Qtica/tools/qtcore/__init__.py
--rw-r--r--   0        0        0      221 2024-01-19 16:24:36.376855 qtica-0.4.3/Qtica/tools/qtcore/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7842 2024-01-30 23:06:34.297316 qtica-0.4.3/Qtica/tools/qtcore/__pycache__/objects.cpython-310.pyc
--rw-r--r--   0        0        0     5753 2024-01-30 22:56:04.576511 qtica-0.4.3/Qtica/tools/qtcore/objects.py
--rw-r--r--   0        0        0     6294 2024-03-05 01:42:30.538833 qtica-0.4.3/Qtica/tools/qtcore/tools.py
--rw-r--r--   0        0        0       63 2024-01-11 17:03:17.454911 qtica-0.4.3/Qtica/tools/qtgui/__init__.py
--rw-r--r--   0        0        0      220 2024-01-11 17:21:33.538867 qtica-0.4.3/Qtica/tools/qtgui/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     8761 2024-01-30 23:06:34.357316 qtica-0.4.3/Qtica/tools/qtgui/__pycache__/objects.cpython-310.pyc
--rw-r--r--   0        0        0    20542 2024-03-05 01:55:52.657632 qtica-0.4.3/Qtica/tools/qtgui/__pycache__/tools.cpython-310.pyc
--rw-r--r--   0        0        0     6373 2024-01-30 22:57:27.101139 qtica-0.4.3/Qtica/tools/qtgui/objects.py
--rw-r--r--   0        0        0    15623 2024-03-05 01:48:08.930849 qtica-0.4.3/Qtica/tools/qtgui/tools.py
--rw-r--r--   0        0        0     4228 2024-02-14 20:10:08.623882 qtica-0.4.3/Qtica/tools/settings.py
--rw-r--r--   0        0        0      978 2024-02-03 20:26:10.731564 qtica-0.4.3/Qtica/tools/size_policy.py
--rw-r--r--   0        0        0     5073 2024-01-05 16:47:52.546347 qtica-0.4.3/Qtica/tools/smooth_scroll.py
--rw-r--r--   0        0        0      327 2024-02-07 22:32:29.616714 qtica-0.4.3/Qtica/tools/spacer_item.py
--rwxr-xr-x   0        0        0      920 2024-01-08 19:19:47.884624 qtica-0.4.3/Qtica/tools/system_tray.py
--rw-r--r--   0        0        0      503 2024-01-10 17:22:18.093342 qtica-0.4.3/Qtica/tools/ui_loader.py
--rw-r--r--   0        0        0      406 2024-01-19 18:57:31.241727 qtica-0.4.3/Qtica/tools/wrappers/__init__.py
--rw-r--r--   0        0        0      705 2024-01-19 18:57:57.371356 qtica-0.4.3/Qtica/tools/wrappers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      723 2024-01-08 20:53:27.432990 qtica-0.4.3/Qtica/tools/wrappers/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      777 2024-01-09 16:49:44.595764 qtica-0.4.3/Qtica/tools/wrappers/__pycache__/border_layout.cpython-310.pyc
--rw-r--r--   0        0        0      943 2024-01-08 20:53:27.456991 qtica-0.4.3/Qtica/tools/wrappers/__pycache__/border_layout.cpython-312.pyc
--rw-r--r--   0        0        0      832 2024-01-09 16:49:44.611765 qtica-0.4.3/Qtica/tools/wrappers/__pycache__/dock_widgets.cpython-310.pyc
--rw-r--r--   0        0        0     1042 2024-01-08 20:53:27.456991 qtica-0.4.3/Qtica/tools/wrappers/__pycache__/dock_widgets.cpython-312.pyc
--rw-r--r--   0        0        0      774 2024-01-09 16:49:44.655765 qtica-0.4.3/Qtica/tools/wrappers/__pycache__/form_layout.cpython-310.pyc
--rw-r--r--   0        0        0      914 2024-01-08 20:53:27.456991 qtica-0.4.3/Qtica/tools/wrappers/__pycache__/form_layout.cpython-312.pyc
--rw-r--r--   0        0        0      963 2024-01-09 16:49:44.635765 qtica-0.4.3/Qtica/tools/wrappers/__pycache__/grid_layout.cpython-310.pyc
--rw-r--r--   0        0        0     1213 2024-01-08 20:53:27.456991 qtica-0.4.3/Qtica/tools/wrappers/__pycache__/grid_layout.cpython-312.pyc
--rw-r--r--   0        0        0     1092 2024-01-09 16:49:44.579764 qtica-0.4.3/Qtica/tools/wrappers/__pycache__/h_layout.cpython-310.pyc
--rw-r--r--   0        0        0     1346 2024-01-08 20:53:27.452991 qtica-0.4.3/Qtica/tools/wrappers/__pycache__/h_layout.cpython-312.pyc
--rw-r--r--   0        0        0      862 2024-01-09 16:49:44.463763 qtica-0.4.3/Qtica/tools/wrappers/__pycache__/menu.cpython-310.pyc
--rw-r--r--   0        0        0      952 2024-01-08 20:53:27.432990 qtica-0.4.3/Qtica/tools/wrappers/__pycache__/menu.cpython-312.pyc
--rw-r--r--   0        0        0      758 2024-01-09 16:49:44.487763 qtica-0.4.3/Qtica/tools/wrappers/__pycache__/tool_bar.cpython-310.pyc
--rw-r--r--   0        0        0      907 2024-01-08 20:53:27.432990 qtica-0.4.3/Qtica/tools/wrappers/__pycache__/tool_bar.cpython-312.pyc
--rw-r--r--   0        0        0     1089 2024-01-09 16:49:44.579764 qtica-0.4.3/Qtica/tools/wrappers/__pycache__/v_layout.cpython-310.pyc
--rw-r--r--   0        0        0     1343 2024-01-08 20:53:27.456991 qtica-0.4.3/Qtica/tools/wrappers/__pycache__/v_layout.cpython-312.pyc
--rw-r--r--   0        0        0      571 2023-12-06 02:20:12.074653 qtica-0.4.3/Qtica/tools/wrappers/__pycache__/water_progress_bar.cpython-310.pyc
--rw-r--r--   0        0        0      408 2024-01-06 00:15:08.651564 qtica-0.4.3/Qtica/tools/wrappers/border_layout.py
--rw-r--r--   0        0        0      369 2024-01-05 19:36:18.305969 qtica-0.4.3/Qtica/tools/wrappers/dock_widgets.py
--rw-r--r--   0        0        0      394 2024-01-05 23:47:27.369612 qtica-0.4.3/Qtica/tools/wrappers/form_layout.py
--rw-r--r--   0        0        0      554 2024-01-06 00:02:38.132729 qtica-0.4.3/Qtica/tools/wrappers/grid_layout.py
--rw-r--r--   0        0        0      612 2024-01-08 18:41:14.882554 qtica-0.4.3/Qtica/tools/wrappers/h_layout.py
--rw-r--r--   0        0        0      345 2024-01-08 20:22:06.442801 qtica-0.4.3/Qtica/tools/wrappers/menu.py
--rw-r--r--   0        0        0      276 2024-01-05 19:36:30.302033 qtica-0.4.3/Qtica/tools/wrappers/tool_bar.py
--rw-r--r--   0        0        0      610 2024-01-06 00:10:09.900030 qtica-0.4.3/Qtica/tools/wrappers/v_layout.py
--rw-r--r--   0        0        0      151 2024-01-18 19:07:18.443698 qtica-0.4.3/Qtica/utils/__init__.py
--rw-r--r--   0        0        0      366 2024-01-18 19:07:22.260274 qtica-0.4.3/Qtica/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      598 2024-01-08 20:53:27.072988 qtica-0.4.3/Qtica/utils/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      184 2024-01-08 18:17:07.446404 qtica-0.4.3/Qtica/utils/__pycache__/_check_none.cpython-312.pyc
--rw-r--r--   0        0        0     3061 2024-01-18 18:52:23.718971 qtica-0.4.3/Qtica/utils/__pycache__/_classes.cpython-310.pyc
--rw-r--r--   0        0        0     5263 2024-01-08 20:53:27.168989 qtica-0.4.3/Qtica/utils/__pycache__/_classes.cpython-312.pyc
--rw-r--r--   0        0        0     4030 2023-10-10 15:17:33.773698 qtica-0.4.3/Qtica/utils/__pycache__/_ensure_thread.cpython-310.pyc
--rw-r--r--   0        0        0     1432 2024-01-09 16:49:43.979757 qtica-0.4.3/Qtica/utils/__pycache__/_env_var.cpython-310.pyc
--rw-r--r--   0        0        0     1875 2024-01-08 20:53:27.076988 qtica-0.4.3/Qtica/utils/__pycache__/_env_var.cpython-312.pyc
--rw-r--r--   0        0        0      902 2024-01-18 19:01:08.648313 qtica-0.4.3/Qtica/utils/__pycache__/_exception_handler.cpython-310.pyc
--rw-r--r--   0        0        0     1145 2024-01-08 20:53:27.160989 qtica-0.4.3/Qtica/utils/__pycache__/_exception_handler.cpython-312.pyc
--rw-r--r--   0        0        0     1368 2023-11-07 22:10:24.611217 qtica-0.4.3/Qtica/utils/__pycache__/_import.cpython-310.pyc
--rw-r--r--   0        0        0     3707 2023-10-10 15:18:15.261924 qtica-0.4.3/Qtica/utils/__pycache__/_message_handler.cpython-310.pyc
--rw-r--r--   0        0        0      969 2023-12-25 20:05:00.304545 qtica-0.4.3/Qtica/utils/__pycache__/_none_check.cpython-310.pyc
--rw-r--r--   0        0        0     1937 2023-12-28 21:14:07.216964 qtica-0.4.3/Qtica/utils/__pycache__/_routes.cpython-310.pyc
--rw-r--r--   0        0        0     2716 2024-01-09 16:49:44.031758 qtica-0.4.3/Qtica/utils/__pycache__/_text_wrap.cpython-310.pyc
--rw-r--r--   0        0        0     3776 2024-01-08 20:53:27.088988 qtica-0.4.3/Qtica/utils/__pycache__/_text_wrap.cpython-312.pyc
--rw-r--r--   0        0        0      754 2024-01-11 17:21:33.254867 qtica-0.4.3/Qtica/utils/__pycache__/alignment.cpython-310.pyc
--rw-r--r--   0        0        0     2708 2023-09-25 12:17:07.616295 qtica-0.4.3/Qtica/utils/__pycache__/auto_wrap.cpython-310.pyc
--rw-r--r--   0        0        0     5403 2023-11-11 01:22:23.745200 qtica-0.4.3/Qtica/utils/__pycache__/color.cpython-310.pyc
--rw-r--r--   0        0        0      485 2023-12-26 22:32:06.735730 qtica-0.4.3/Qtica/utils/__pycache__/dialogs.cpython-310.pyc
--rw-r--r--   0        0        0     1422 2023-12-31 19:49:03.787973 qtica-0.4.3/Qtica/utils/__pycache__/env_var.cpython-310.pyc
--rw-r--r--   0        0        0      922 2023-09-25 12:17:07.580295 qtica-0.4.3/Qtica/utils/__pycache__/exception_handler.cpython-310.pyc
--rw-r--r--   0        0        0     1810 2023-12-26 19:38:29.807787 qtica-0.4.3/Qtica/utils/__pycache__/methods.cpython-310.pyc
--rw-r--r--   0        0        0     1119 2024-01-11 17:21:33.258867 qtica-0.4.3/Qtica/utils/__pycache__/modifiers.cpython-310.pyc
--rw-r--r--   0        0        0     2265 2023-10-02 22:43:31.865968 qtica-0.4.3/Qtica/utils/__pycache__/multimethod.cpython-310.pyc
--rw-r--r--   0        0        0     4423 2023-10-20 21:31:47.218122 qtica-0.4.3/Qtica/utils/__pycache__/overload.cpython-310.pyc
--rw-r--r--   0        0        0     5334 2024-01-11 17:21:33.218867 qtica-0.4.3/Qtica/utils/__pycache__/qstyle_sheet.cpython-310.pyc
--rw-r--r--   0        0        0     8753 2024-01-08 20:53:27.092988 qtica-0.4.3/Qtica/utils/__pycache__/qstyle_sheet.cpython-312.pyc
--rw-r--r--   0        0        0     2373 2024-01-09 16:49:43.967757 qtica-0.4.3/Qtica/utils/__pycache__/routes.cpython-310.pyc
--rw-r--r--   0        0        0     3404 2024-01-08 20:53:27.076988 qtica-0.4.3/Qtica/utils/__pycache__/routes.cpython-312.pyc
--rw-r--r--   0        0        0     5267 2023-10-16 11:38:26.513552 qtica-0.4.3/Qtica/utils/__pycache__/system.cpython-310.pyc
--rw-r--r--   0        0        0     1852 2024-01-18 18:50:22.741771 qtica-0.4.3/Qtica/utils/_classes.py
--rw-r--r--   0        0        0     1000 2024-01-05 22:19:49.638271 qtica-0.4.3/Qtica/utils/_env_var.py
--rw-r--r--   0        0        0     3531 2023-08-25 23:14:12.080003 qtica-0.4.3/Qtica/utils/_text_wrap.py
--rw-r--r--   0        0        0      386 2023-12-28 21:18:40.864073 qtica-0.4.3/Qtica/utils/alignment.py
--rw-r--r--   0        0        0      305 2023-04-14 05:53:29.635829 qtica-0.4.3/Qtica/utils/caseconverter/__init__.py
--rw-r--r--   0        0        0      644 2024-01-09 16:49:44.191760 qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      665 2024-01-08 20:53:27.172989 qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     4924 2024-01-09 16:49:44.251761 qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/boundaries.cpython-310.pyc
--rw-r--r--   0        0        0     6612 2024-01-08 20:53:27.204989 qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/boundaries.cpython-312.pyc
--rw-r--r--   0        0        0     1214 2024-01-09 16:49:44.247761 qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/camel.cpython-310.pyc
--rw-r--r--   0        0        0     1553 2024-01-08 20:53:27.200989 qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/camel.cpython-312.pyc
--rw-r--r--   0        0        0     6731 2024-01-09 16:49:44.195760 qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/caseconverter.cpython-310.pyc
--rw-r--r--   0        0        0     8791 2024-01-08 20:53:27.176989 qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/caseconverter.cpython-312.pyc
--rw-r--r--   0        0        0     1383 2024-01-09 16:49:44.255761 qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/cobol.cpython-310.pyc
--rw-r--r--   0        0        0     2029 2024-01-08 20:53:27.208989 qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/cobol.cpython-312.pyc
--rw-r--r--   0        0        0     1208 2024-01-09 16:49:44.255761 qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/flat.cpython-310.pyc
--rw-r--r--   0        0        0     1547 2024-01-08 20:53:27.208989 qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/flat.cpython-312.pyc
--rw-r--r--   0        0        0     1253 2024-01-09 16:49:44.259761 qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/kebab.cpython-310.pyc
--rw-r--r--   0        0        0     1643 2024-01-08 20:53:27.212989 qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/kebab.cpython-312.pyc
--rw-r--r--   0        0        0     1686 2024-01-09 16:49:44.263761 qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/macro.cpython-310.pyc
--rw-r--r--   0        0        0     2506 2024-01-08 20:53:27.216989 qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/macro.cpython-312.pyc
--rw-r--r--   0        0        0     1501 2024-01-09 16:49:44.263761 qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/pascal.cpython-310.pyc
--rw-r--r--   0        0        0     2007 2024-01-08 20:53:27.216989 qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/pascal.cpython-312.pyc
--rw-r--r--   0        0        0     1254 2024-01-09 16:49:44.267761 qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/snake.cpython-310.pyc
--rw-r--r--   0        0        0     1644 2024-01-08 20:53:27.216989 qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/snake.cpython-312.pyc
--rw-r--r--   0        0        0     3384 2023-04-14 05:53:29.635829 qtica-0.4.3/Qtica/utils/caseconverter/boundaries.py
--rw-r--r--   0        0        0      658 2023-04-14 05:53:29.635829 qtica-0.4.3/Qtica/utils/caseconverter/camel.py
--rw-r--r--   0        0        0     6043 2023-04-14 05:53:29.635829 qtica-0.4.3/Qtica/utils/caseconverter/caseconverter.py
--rw-r--r--   0        0        0      902 2023-04-14 05:53:29.635829 qtica-0.4.3/Qtica/utils/caseconverter/cobol.py
--rw-r--r--   0        0        0      655 2023-04-14 05:53:29.635829 qtica-0.4.3/Qtica/utils/caseconverter/flat.py
--rw-r--r--   0        0        0      734 2023-04-14 05:53:29.635829 qtica-0.4.3/Qtica/utils/caseconverter/kebab.py
--rw-r--r--   0        0        0     1236 2023-04-14 05:53:29.635829 qtica-0.4.3/Qtica/utils/caseconverter/macro.py
--rw-r--r--   0        0        0      932 2023-04-14 05:53:29.635829 qtica-0.4.3/Qtica/utils/caseconverter/pascal.py
--rw-r--r--   0        0        0      735 2023-04-14 05:53:29.639829 qtica-0.4.3/Qtica/utils/caseconverter/snake.py
--rw-r--r--   0        0        0     2612 2024-01-09 22:28:05.841998 qtica-0.4.3/Qtica/utils/maths/__init__.py
--rw-r--r--   0        0        0     3000 2024-01-10 15:38:23.968696 qtica-0.4.3/Qtica/utils/maths/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3514 2024-01-09 22:33:14.063975 qtica-0.4.3/Qtica/utils/maths/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     3580 2024-01-10 15:38:23.972696 qtica-0.4.3/Qtica/utils/maths/__pycache__/geometry.cpython-310.pyc
--rw-r--r--   0        0        0     5513 2024-01-09 22:33:14.063975 qtica-0.4.3/Qtica/utils/maths/__pycache__/geometry.cpython-312.pyc
--rw-r--r--   0        0        0    16234 2024-01-10 15:38:23.992695 qtica-0.4.3/Qtica/utils/maths/__pycache__/vector.cpython-310.pyc
--rw-r--r--   0        0        0    22140 2024-01-09 22:33:14.067975 qtica-0.4.3/Qtica/utils/maths/__pycache__/vector.cpython-312.pyc
--rw-r--r--   0        0        0     3788 2023-10-10 14:54:54.637867 qtica-0.4.3/Qtica/utils/maths/geometry.py
--rw-r--r--   0        0        0    13540 2024-01-05 22:01:09.346451 qtica-0.4.3/Qtica/utils/maths/vector.py
--rw-r--r--   0        0        0      610 2023-10-20 19:26:19.412422 qtica-0.4.3/Qtica/utils/modifiers.py
--rw-r--r--   0        0        0      613 2024-02-06 15:28:39.255195 qtica-0.4.3/Qtica/widgets/__init__.py
--rw-r--r--   0        0        0      955 2024-02-06 15:29:00.747194 qtica-0.4.3/Qtica/widgets/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      918 2024-01-09 20:38:36.585517 qtica-0.4.3/Qtica/widgets/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0    15554 2024-02-23 21:14:48.069514 qtica-0.4.3/Qtica/widgets/__pycache__/_widgets.cpython-310.pyc
--rw-r--r--   0        0        0     4240 2024-02-14 18:57:33.896415 qtica-0.4.3/Qtica/widgets/__pycache__/application.cpython-310.pyc
--rw-r--r--   0        0        0     6224 2024-01-09 16:19:44.091527 qtica-0.4.3/Qtica/widgets/__pycache__/application.cpython-312.pyc
--rw-r--r--   0        0        0     1804 2024-01-19 15:27:34.556994 qtica-0.4.3/Qtica/widgets/__pycache__/buttons.cpython-310.pyc
--rw-r--r--   0        0        0     1348 2024-01-10 15:38:24.292680 qtica-0.4.3/Qtica/widgets/__pycache__/frame.cpython-310.pyc
--rw-r--r--   0        0        0     1984 2024-01-08 21:14:34.756360 qtica-0.4.3/Qtica/widgets/__pycache__/frame.cpython-312.pyc
--rw-r--r--   0        0        0     2457 2024-01-26 21:27:49.435621 qtica-0.4.3/Qtica/widgets/__pycache__/icon_widget.cpython-310.pyc
--rw-r--r--   0        0        0     3835 2024-01-08 21:14:34.744359 qtica-0.4.3/Qtica/widgets/__pycache__/icon_widget.cpython-312.pyc
--rw-r--r--   0        0        0      900 2024-01-10 15:38:24.204685 qtica-0.4.3/Qtica/widgets/__pycache__/label.cpython-310.pyc
--rw-r--r--   0        0        0     1148 2024-01-08 21:14:34.728359 qtica-0.4.3/Qtica/widgets/__pycache__/label.cpython-312.pyc
--rw-r--r--   0        0        0     1206 2024-01-10 15:38:24.268682 qtica-0.4.3/Qtica/widgets/__pycache__/line.cpython-310.pyc
--rw-r--r--   0        0        0     1852 2024-01-08 21:14:34.748360 qtica-0.4.3/Qtica/widgets/__pycache__/line.cpython-312.pyc
--rw-r--r--   0        0        0      641 2024-01-10 15:38:24.232683 qtica-0.4.3/Qtica/widgets/__pycache__/line_edit.cpython-310.pyc
--rw-r--r--   0        0        0      763 2024-01-08 21:14:34.740359 qtica-0.4.3/Qtica/widgets/__pycache__/line_edit.cpython-312.pyc
--rw-r--r--   0        0        0     1183 2024-01-10 15:38:24.204685 qtica-0.4.3/Qtica/widgets/__pycache__/menu.cpython-310.pyc
--rw-r--r--   0        0        0     1700 2024-01-08 21:14:34.724359 qtica-0.4.3/Qtica/widgets/__pycache__/menu.cpython-312.pyc
--rw-r--r--   0        0        0     1281 2024-01-10 15:38:24.280681 qtica-0.4.3/Qtica/widgets/__pycache__/push_button.cpython-310.pyc
--rw-r--r--   0        0        0     2065 2024-01-08 22:30:38.193588 qtica-0.4.3/Qtica/widgets/__pycache__/push_button.cpython-312.pyc
--rw-r--r--   0        0        0     1293 2024-01-10 15:38:24.232683 qtica-0.4.3/Qtica/widgets/__pycache__/scroll_area.cpython-310.pyc
--rw-r--r--   0        0        0     2040 2024-01-08 21:14:34.740359 qtica-0.4.3/Qtica/widgets/__pycache__/scroll_area.cpython-312.pyc
--rw-r--r--   0        0        0     2280 2024-01-12 10:41:21.071686 qtica-0.4.3/Qtica/widgets/__pycache__/size_grip.cpython-310.pyc
--rw-r--r--   0        0        0     4717 2024-01-08 20:53:27.460991 qtica-0.4.3/Qtica/widgets/__pycache__/size_grip.cpython-312.pyc
--rw-r--r--   0        0        0      888 2024-01-10 15:38:24.292680 qtica-0.4.3/Qtica/widgets/__pycache__/spin_box.cpython-310.pyc
--rw-r--r--   0        0        0     1172 2024-01-09 20:38:36.629517 qtica-0.4.3/Qtica/widgets/__pycache__/spin_box.cpython-312.pyc
--rw-r--r--   0        0        0     3101 2024-02-03 21:25:57.535488 qtica-0.4.3/Qtica/widgets/__pycache__/stack.cpython-310.pyc
--rw-r--r--   0        0        0     6006 2024-01-08 21:14:34.732359 qtica-0.4.3/Qtica/widgets/__pycache__/stack.cpython-312.pyc
--rw-r--r--   0        0        0     1072 2024-01-26 20:01:11.773359 qtica-0.4.3/Qtica/widgets/__pycache__/stacked_widget.cpython-310.pyc
--rw-r--r--   0        0        0     1554 2024-01-08 21:14:34.756360 qtica-0.4.3/Qtica/widgets/__pycache__/stacked_widget.cpython-312.pyc
--rw-r--r--   0        0        0     1281 2024-01-10 15:38:24.252682 qtica-0.4.3/Qtica/widgets/__pycache__/tool_button.cpython-310.pyc
--rw-r--r--   0        0        0     2065 2024-01-08 21:14:34.748360 qtica-0.4.3/Qtica/widgets/__pycache__/tool_button.cpython-312.pyc
--rw-r--r--   0        0        0      889 2024-01-10 15:38:24.224684 qtica-0.4.3/Qtica/widgets/__pycache__/widget.cpython-310.pyc
--rw-r--r--   0        0        0     1201 2024-01-08 21:14:34.736359 qtica-0.4.3/Qtica/widgets/__pycache__/widget.cpython-312.pyc
--rw-r--r--   0        0        0    10904 2024-02-23 21:14:45.105707 qtica-0.4.3/Qtica/widgets/_widgets.py
--rw-r--r--   0        0        0     3396 2024-02-14 18:57:24.932073 qtica-0.4.3/Qtica/widgets/application.py
--rw-r--r--   0        0        0     1275 2024-01-19 15:21:48.697008 qtica-0.4.3/Qtica/widgets/buttons.py
--rw-r--r--   0        0        0     1438 2024-02-03 20:43:22.551542 qtica-0.4.3/Qtica/widgets/container.py
--rw-r--r--   0        0        0      114 2024-01-05 17:16:11.467069 qtica-0.4.3/Qtica/widgets/dialogs/__init__.py
--rw-r--r--   0        0        0      328 2024-01-10 15:38:24.024693 qtica-0.4.3/Qtica/widgets/dialogs/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      341 2024-01-08 20:53:27.468991 qtica-0.4.3/Qtica/widgets/dialogs/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     1873 2024-01-03 00:16:32.516166 qtica-0.4.3/Qtica/widgets/dialogs/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     2609 2024-01-03 00:16:32.592168 qtica-0.4.3/Qtica/widgets/dialogs/__pycache__/large_text.cpython-310.pyc
--rw-r--r--   0        0        0     5124 2024-01-30 23:06:34.901321 qtica-0.4.3/Qtica/widgets/dialogs/__pycache__/mask.cpython-310.pyc
--rw-r--r--   0        0        0    10088 2024-01-09 18:38:18.598559 qtica-0.4.3/Qtica/widgets/dialogs/__pycache__/mask.cpython-312.pyc
--rw-r--r--   0        0        0     2278 2024-01-10 15:38:24.108689 qtica-0.4.3/Qtica/widgets/dialogs/__pycache__/silent.cpython-310.pyc
--rw-r--r--   0        0        0     3601 2024-01-08 21:14:34.548353 qtica-0.4.3/Qtica/widgets/dialogs/__pycache__/silent.cpython-312.pyc
--rw-r--r--   0        0        0     3936 2024-01-03 00:16:51.004672 qtica-0.4.3/Qtica/widgets/dialogs/__pycache__/teaching_tip.cpython-310.pyc
--rw-r--r--   0        0        0     2794 2024-01-03 00:16:32.516166 qtica-0.4.3/Qtica/widgets/dialogs/__pycache__/text.cpython-310.pyc
--rw-r--r--   0        0        0     4761 2024-01-30 22:34:46.218899 qtica-0.4.3/Qtica/widgets/dialogs/mask.py
--rwxr-xr-x   0        0        0     1977 2024-01-05 19:58:29.964501 qtica-0.4.3/Qtica/widgets/dialogs/silent.py
--rw-r--r--   0        0        0    14689 2024-01-10 15:38:24.104689 qtica-0.4.3/Qtica/widgets/dialogs/teaching_tip/__pycache__/tails.cpython-310.pyc
--rw-r--r--   0        0        0    28937 2024-01-09 18:54:58.400518 qtica-0.4.3/Qtica/widgets/dialogs/teaching_tip/__pycache__/tails.cpython-312.pyc
--rw-r--r--   0        0        0     3967 2024-01-10 15:38:24.076691 qtica-0.4.3/Qtica/widgets/dialogs/teaching_tip/__pycache__/tool_tip.cpython-310.pyc
--rw-r--r--   0        0        0     7115 2024-01-09 18:50:32.343688 qtica-0.4.3/Qtica/widgets/dialogs/teaching_tip/__pycache__/tool_tip.cpython-312.pyc
--rw-r--r--   0        0        0    13367 2024-01-09 18:54:53.360501 qtica-0.4.3/Qtica/widgets/dialogs/teaching_tip/tails.py
--rw-r--r--   0        0        0     3114 2024-01-09 18:49:55.579584 qtica-0.4.3/Qtica/widgets/dialogs/teaching_tip/tool_tip.py
--rw-r--r--   0        0        0     4180 2024-01-30 23:02:54.923640 qtica-0.4.3/Qtica/widgets/eliding_label.py
--rw-r--r--   0        0        0      564 2024-01-19 15:21:36.657008 qtica-0.4.3/Qtica/widgets/group_box.py
--rw-r--r--   0        0        0     2352 2024-01-26 21:27:46.686318 qtica-0.4.3/Qtica/widgets/icon_widget.py
--rw-r--r--   0        0        0      388 2023-12-26 19:29:47.031798 qtica-0.4.3/Qtica/widgets/label.py
--rw-r--r--   0        0        0      582 2024-01-05 20:04:13.311864 qtica-0.4.3/Qtica/widgets/line.py
--rw-r--r--   0        0        0     1257 2024-01-08 20:51:10.080131 qtica-0.4.3/Qtica/widgets/menu.py
--rw-r--r--   0        0        0     1169 2024-01-08 20:47:49.382811 qtica-0.4.3/Qtica/widgets/quick_widget.py
--rw-r--r--   0        0        0      986 2024-01-08 20:47:34.978712 qtica-0.4.3/Qtica/widgets/scroll_area.py
--rw-r--r--   0        0        0     1999 2024-01-11 18:18:59.194727 qtica-0.4.3/Qtica/widgets/size_grip.py
--rw-r--r--   0        0        0     3952 2024-02-03 20:39:57.223547 qtica-0.4.3/Qtica/widgets/stack.py
--rw-r--r--   0        0        0      830 2024-01-26 20:00:20.440515 qtica-0.4.3/Qtica/widgets/stacked_widget.py
--rw-r--r--   0        0        0      647 2024-02-14 19:18:15.910409 qtica-0.4.3/Qtica/widgets/video_widget.py
--rw-r--r--   0        0        0      102 2024-01-13 16:32:35.376140 qtica-0.4.3/Qtica/widgets/window/__init__.py
--rw-r--r--   0        0        0      315 2024-01-13 16:34:16.977749 qtica-0.4.3/Qtica/widgets/window/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      288 2024-01-08 20:53:27.264989 qtica-0.4.3/Qtica/widgets/window/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     2768 2024-02-06 15:29:00.747194 qtica-0.4.3/Qtica/widgets/window/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     3699 2024-02-03 21:25:57.515488 qtica-0.4.3/Qtica/widgets/window/__pycache__/frameless.cpython-310.pyc
--rw-r--r--   0        0        0     6387 2024-01-08 20:53:27.460991 qtica-0.4.3/Qtica/widgets/window/__pycache__/frameless.cpython-312.pyc
--rw-r--r--   0        0        0      649 2024-01-14 06:19:43.142189 qtica-0.4.3/Qtica/widgets/window/__pycache__/mainwindow.cpython-310.pyc
--rw-r--r--   0        0        0     4189 2024-01-08 20:53:27.264989 qtica-0.4.3/Qtica/widgets/window/__pycache__/mainwindow.cpython-312.pyc
--rw-r--r--   0        0        0     3294 2023-12-26 19:38:29.799787 qtica-0.4.3/Qtica/widgets/window/__pycache__/routes.cpython-310.pyc
--rw-r--r--   0        0        0     2490 2024-02-06 15:20:04.943215 qtica-0.4.3/Qtica/widgets/window/base.py
--rw-r--r--   0        0        0     3883 2024-02-03 21:17:22.707499 qtica-0.4.3/Qtica/widgets/window/frameless.py
--rw-r--r--   0        0        0      244 2024-01-14 06:19:22.430665 qtica-0.4.3/Qtica/widgets/window/mainwindow.py
--rw-r--r--   0        0        0     3170 2024-03-05 01:49:20.078852 qtica-0.4.3/README.md
--rw-r--r--   0        0        0     1650 2024-03-05 01:48:50.906851 qtica-0.4.3/pyproject.toml
--rw-r--r--   0        0        0    21057 1970-01-01 00:00:00.000000 qtica-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    17089 2024-05-24 19:45:19.067851 qtica-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-09-14 22:18:47.247695 qtica-0.5.0/LICENSE
+-rw-r--r--   0        0        0      212 2024-05-24 19:41:04.064344 qtica-0.5.0/Qtica/__init__.py
+-rw-r--r--   0        0        0      175 2024-01-05 15:19:55.230374 qtica-0.5.0/Qtica/animations/__init__.py
+-rw-r--r--   0        0        0      705 2024-01-11 22:54:05.655130 qtica-0.5.0/Qtica/animations/parallel_animation_group.py
+-rw-r--r--   0        0        0      533 2024-01-05 15:19:26.149384 qtica-0.5.0/Qtica/animations/property_animation.py
+-rw-r--r--   0        0        0      713 2024-01-05 15:19:22.549261 qtica-0.5.0/Qtica/animations/sequential_animation_group.py
+-rw-r--r--   0        0        0      638 2024-03-21 21:10:44.844377 qtica-0.5.0/Qtica/core/__init__.py
+-rw-r--r--   0        0        0     1018 2024-03-21 21:16:00.832365 qtica-0.5.0/Qtica/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7545 2024-03-06 01:35:31.342501 qtica-0.5.0/Qtica/core/__pycache__/_base.cpython-310.pyc
+-rw-r--r--   0        0        0     1434 2024-01-25 21:21:57.685539 qtica-0.5.0/Qtica/core/__pycache__/_config.cpython-310.pyc
+-rw-r--r--   0        0        0     2891 2024-01-25 21:21:57.673527 qtica-0.5.0/Qtica/core/__pycache__/_declarative.cpython-310.pyc
+-rw-r--r--   0        0        0     2056 2024-03-06 19:05:55.620006 qtica-0.5.0/Qtica/core/__pycache__/_dialog.cpython-310.pyc
+-rw-r--r--   0        0        0     1836 2024-01-25 21:21:57.685539 qtica-0.5.0/Qtica/core/__pycache__/_icons.cpython-310.pyc
+-rw-r--r--   0        0        0     1657 2024-01-25 21:21:57.685539 qtica-0.5.0/Qtica/core/__pycache__/_painter.cpython-310.pyc
+-rw-r--r--   0        0        0      542 2024-01-25 21:21:57.681535 qtica-0.5.0/Qtica/core/__pycache__/_qobject.cpython-310.pyc
+-rw-r--r--   0        0        0     1806 2024-02-18 20:16:45.707284 qtica-0.5.0/Qtica/core/__pycache__/_tool.cpython-310.pyc
+-rw-r--r--   0        0        0     6628 2024-03-21 22:06:38.192242 qtica-0.5.0/Qtica/core/__pycache__/_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     3221 2024-02-03 21:25:57.155488 qtica-0.5.0/Qtica/core/__pycache__/api.cpython-310.pyc
+-rw-r--r--   0        0        0      878 2024-01-25 21:21:57.689543 qtica-0.5.0/Qtica/core/__pycache__/exception_handler.cpython-310.pyc
+-rw-r--r--   0        0        0     9335 2024-02-23 20:45:00.442205 qtica-0.5.0/Qtica/core/__pycache__/qstyle_sheet.cpython-310.pyc
+-rw-r--r--   0        0        0     2372 2024-01-25 21:21:57.689543 qtica-0.5.0/Qtica/core/__pycache__/routes.cpython-310.pyc
+-rw-r--r--   0        0        0     7602 2024-03-06 01:34:44.645888 qtica-0.5.0/Qtica/core/_base.py
+-rw-r--r--   0        0        0      643 2024-01-08 19:18:09.498861 qtica-0.5.0/Qtica/core/_config.py
+-rw-r--r--   0        0        0     1959 2024-01-04 02:21:46.887848 qtica-0.5.0/Qtica/core/_declarative.py
+-rw-r--r--   0        0        0     1657 2024-03-06 19:05:27.696007 qtica-0.5.0/Qtica/core/_dialog.py
+-rw-r--r--   0        0        0     1410 2024-01-08 21:41:19.748815 qtica-0.5.0/Qtica/core/_icons.py
+-rw-r--r--   0        0        0      748 2024-01-03 15:08:05.410277 qtica-0.5.0/Qtica/core/_painter.py
+-rw-r--r--   0        0        0      196 2023-12-25 20:16:29.144530 qtica-0.5.0/Qtica/core/_qobject.py
+-rw-r--r--   0        0        0     1299 2024-02-18 20:16:11.295285 qtica-0.5.0/Qtica/core/_tool.py
+-rw-r--r--   0        0        0     5671 2024-03-21 22:06:12.496243 qtica-0.5.0/Qtica/core/_widget.py
+-rw-r--r--   0        0        0     3335 2024-02-03 20:51:32.215532 qtica-0.5.0/Qtica/core/api.py
+-rw-r--r--   0        0        0      702 2024-01-18 19:05:19.140292 qtica-0.5.0/Qtica/core/exception_handler.py
+-rw-r--r--   0        0        0     9463 2024-02-19 18:12:29.534835 qtica-0.5.0/Qtica/core/qstyle_sheet.py
+-rw-r--r--   0        0        0     1336 2024-01-08 20:43:54.389124 qtica-0.5.0/Qtica/core/routes.py
+-rw-r--r--   0        0        0       23 2024-01-11 22:51:54.923036 qtica-0.5.0/Qtica/effects/__init__.py
+-rw-r--r--   0        0        0      200 2024-01-12 10:41:21.758783 qtica-0.5.0/Qtica/effects/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      372 2024-01-09 16:19:44.099527 qtica-0.5.0/Qtica/effects/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     1545 2024-01-12 10:41:21.770838 qtica-0.5.0/Qtica/effects/__pycache__/_effects.cpython-310.pyc
+-rw-r--r--   0        0        0      688 2024-01-11 17:21:56.306866 qtica-0.5.0/Qtica/effects/__pycache__/blur.cpython-310.pyc
+-rw-r--r--   0        0        0      818 2024-01-09 16:19:44.103527 qtica-0.5.0/Qtica/effects/__pycache__/blur.cpython-312.pyc
+-rw-r--r--   0        0        0      704 2023-12-26 19:43:34.947780 qtica-0.5.0/Qtica/effects/__pycache__/colorize.cpython-310.pyc
+-rw-r--r--   0        0        0      834 2024-01-09 16:19:44.099527 qtica-0.5.0/Qtica/effects/__pycache__/colorize.cpython-312.pyc
+-rw-r--r--   0        0        0      676 2023-12-26 19:43:34.947780 qtica-0.5.0/Qtica/effects/__pycache__/drop_shadow.cpython-310.pyc
+-rw-r--r--   0        0        0      799 2024-01-09 16:19:44.099527 qtica-0.5.0/Qtica/effects/__pycache__/drop_shadow.cpython-312.pyc
+-rw-r--r--   0        0        0    13226 2024-01-02 22:50:03.747969 qtica-0.5.0/Qtica/effects/__pycache__/neumorphism.cpython-310.pyc
+-rw-r--r--   0        0        0      700 2023-12-26 19:43:34.947780 qtica-0.5.0/Qtica/effects/__pycache__/opacity.cpython-310.pyc
+-rw-r--r--   0        0        0      830 2024-01-09 16:19:44.099527 qtica-0.5.0/Qtica/effects/__pycache__/opacity.cpython-312.pyc
+-rw-r--r--   0        0        0      966 2024-01-11 22:53:08.395089 qtica-0.5.0/Qtica/effects/_effects.py
+-rw-r--r--   0        0        0      319 2024-01-08 18:17:03.666028 qtica-0.5.0/Qtica/enums/__init__.py
+-rw-r--r--   0        0        0      619 2024-01-09 16:49:43.271749 qtica-0.5.0/Qtica/enums/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      638 2024-01-08 18:17:07.270386 qtica-0.5.0/Qtica/enums/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     1845 2023-11-08 02:29:24.001067 qtica-0.5.0/Qtica/enums/__pycache__/_abs_icons.cpython-310.pyc
+-rw-r--r--   0        0        0      461 2023-11-04 22:14:44.127618 qtica-0.5.0/Qtica/enums/__pycache__/animation.cpython-310.pyc
+-rw-r--r--   0        0        0      458 2023-11-04 22:14:44.127618 qtica-0.5.0/Qtica/enums/__pycache__/clipboard.cpython-310.pyc
+-rw-r--r--   0        0        0    70891 2024-01-13 03:14:56.143252 qtica-0.5.0/Qtica/enums/__pycache__/colors.cpython-310.pyc
+-rw-r--r--   0        0        0   106081 2024-01-08 18:16:32.442869 qtica-0.5.0/Qtica/enums/__pycache__/colors.cpython-312.pyc
+-rw-r--r--   0        0        0     2476 2023-12-25 20:05:00.112545 qtica-0.5.0/Qtica/enums/__pycache__/env_vars.cpython-310.pyc
+-rw-r--r--   0        0        0     2823 2024-01-08 18:16:32.718897 qtica-0.5.0/Qtica/enums/__pycache__/env_vars.cpython-312.pyc
+-rw-r--r--   0        0        0     2169 2024-01-25 21:16:05.106523 qtica-0.5.0/Qtica/enums/__pycache__/events.cpython-310.pyc
+-rw-r--r--   0        0        0     4487 2024-01-08 21:45:19.215511 qtica-0.5.0/Qtica/enums/__pycache__/events.cpython-312.pyc
+-rw-r--r--   0        0        0      511 2023-12-26 19:32:50.343794 qtica-0.5.0/Qtica/enums/__pycache__/position.cpython-310.pyc
+-rw-r--r--   0        0        0      616 2024-01-08 18:16:32.730898 qtica-0.5.0/Qtica/enums/__pycache__/position.cpython-312.pyc
+-rw-r--r--   0        0        0      903 2024-03-06 18:25:55.448103 qtica-0.5.0/Qtica/enums/__pycache__/qpa_plugins.cpython-310.pyc
+-rw-r--r--   0        0        0      979 2024-01-08 18:16:32.730898 qtica-0.5.0/Qtica/enums/__pycache__/qpa_plugins.cpython-312.pyc
+-rw-r--r--   0        0        0    10087 2023-11-04 22:14:43.383580 qtica-0.5.0/Qtica/enums/__pycache__/signals.cpython-310.pyc
+-rw-r--r--   0        0        0    19942 2024-01-08 18:16:32.606886 qtica-0.5.0/Qtica/enums/__pycache__/signals.cpython-312.pyc
+-rw-r--r--   0        0        0      449 2024-01-09 16:49:43.755755 qtica-0.5.0/Qtica/enums/__pycache__/size.cpython-310.pyc
+-rw-r--r--   0        0        0      522 2024-01-08 18:16:32.750900 qtica-0.5.0/Qtica/enums/__pycache__/size.cpython-312.pyc
+-rw-r--r--   0        0        0      503 2023-11-04 22:14:44.127618 qtica-0.5.0/Qtica/enums/__pycache__/smooth_scroll.cpython-310.pyc
+-rw-r--r--   0        0        0      945 2024-01-03 03:22:33.775041 qtica-0.5.0/Qtica/enums/__pycache__/teaching_tip_tails.cpython-310.pyc
+-rw-r--r--   0        0        0      406 2024-01-09 16:49:43.803755 qtica-0.5.0/Qtica/enums/__pycache__/theme.cpython-310.pyc
+-rw-r--r--   0        0        0      460 2024-01-08 18:17:07.430402 qtica-0.5.0/Qtica/enums/__pycache__/theme.cpython-312.pyc
+-rw-r--r--   0        0        0    11452 2024-01-25 21:16:05.026543 qtica-0.5.0/Qtica/enums/__pycache__/widgets.cpython-310.pyc
+-rw-r--r--   0        0        0    18255 2024-01-08 18:16:32.670892 qtica-0.5.0/Qtica/enums/__pycache__/widgets.cpython-312.pyc
+-rw-r--r--   0        0        0    65688 2024-01-12 10:55:38.251360 qtica-0.5.0/Qtica/enums/colors.py
+-rw-r--r--   0        0        0     1894 2023-12-18 12:17:46.147253 qtica-0.5.0/Qtica/enums/env_vars.py
+-rw-r--r--   0        0        0     1931 2024-01-23 18:57:02.170893 qtica-0.5.0/Qtica/enums/events.py
+-rw-r--r--   0        0        0      221 2023-12-25 20:41:14.660498 qtica-0.5.0/Qtica/enums/position.py
+-rw-r--r--   0        0        0      556 2024-03-06 18:21:16.064114 qtica-0.5.0/Qtica/enums/qpa_plugins.py
+-rw-r--r--   0        0        0    10582 2023-10-20 20:58:21.160688 qtica-0.5.0/Qtica/enums/signals.py
+-rw-r--r--   0        0        0      151 2024-01-06 00:13:48.065418 qtica-0.5.0/Qtica/enums/size.py
+-rw-r--r--   0        0        0       85 2024-01-05 23:36:52.732478 qtica-0.5.0/Qtica/enums/theme.py
+-rw-r--r--   0        0        0    11181 2024-01-23 19:11:15.515182 qtica-0.5.0/Qtica/enums/widgets.py
+-rw-r--r--   0        0        0      294 2024-01-06 00:22:24.430372 qtica-0.5.0/Qtica/layouts/__init__.py
+-rw-r--r--   0        0        0      531 2024-01-11 17:21:56.198866 qtica-0.5.0/Qtica/layouts/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      552 2024-01-08 21:14:34.756360 qtica-0.5.0/Qtica/layouts/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     5477 2024-01-12 10:41:21.710566 qtica-0.5.0/Qtica/layouts/__pycache__/border_layout.cpython-310.pyc
+-rw-r--r--   0        0        0    10477 2024-01-08 21:14:34.764360 qtica-0.5.0/Qtica/layouts/__pycache__/border_layout.cpython-312.pyc
+-rw-r--r--   0        0        0     4534 2024-01-02 22:57:20.982628 qtica-0.5.0/Qtica/layouts/__pycache__/expand_layout.cpython-310.pyc
+-rw-r--r--   0        0        0     7670 2024-01-26 22:00:39.598621 qtica-0.5.0/Qtica/layouts/__pycache__/flow_layout.cpython-310.pyc
+-rw-r--r--   0        0        0    12304 2024-01-08 21:14:34.768360 qtica-0.5.0/Qtica/layouts/__pycache__/flow_layout.cpython-312.pyc
+-rw-r--r--   0        0        0     1283 2024-01-26 22:00:39.594621 qtica-0.5.0/Qtica/layouts/__pycache__/form_layout.cpython-310.pyc
+-rw-r--r--   0        0        0     2071 2024-01-08 21:14:34.760360 qtica-0.5.0/Qtica/layouts/__pycache__/form_layout.cpython-312.pyc
+-rw-r--r--   0        0        0     1405 2024-01-11 17:21:56.202866 qtica-0.5.0/Qtica/layouts/__pycache__/grid_layout.cpython-310.pyc
+-rw-r--r--   0        0        0     2314 2024-01-08 21:14:34.760360 qtica-0.5.0/Qtica/layouts/__pycache__/grid_layout.cpython-312.pyc
+-rw-r--r--   0        0        0     1071 2024-05-24 19:31:38.593448 qtica-0.5.0/Qtica/layouts/__pycache__/h_layout.cpython-310.pyc
+-rw-r--r--   0        0        0     2576 2024-01-08 21:14:34.760360 qtica-0.5.0/Qtica/layouts/__pycache__/h_layout.cpython-312.pyc
+-rw-r--r--   0        0        0     1332 2024-03-06 01:06:08.150738 qtica-0.5.0/Qtica/layouts/__pycache__/stacked.cpython-310.pyc
+-rw-r--r--   0        0        0     1721 2024-01-08 21:14:34.764360 qtica-0.5.0/Qtica/layouts/__pycache__/stacked.cpython-312.pyc
+-rw-r--r--   0        0        0     1068 2024-05-24 19:31:38.613451 qtica-0.5.0/Qtica/layouts/__pycache__/v_layout.cpython-310.pyc
+-rw-r--r--   0        0        0     2570 2024-01-08 21:14:34.764360 qtica-0.5.0/Qtica/layouts/__pycache__/v_layout.cpython-312.pyc
+-rw-r--r--   0        0        0     6615 2024-01-11 22:58:24.419318 qtica-0.5.0/Qtica/layouts/border_layout.py
+-rw-r--r--   0        0        0     7477 2024-01-26 21:59:56.853300 qtica-0.5.0/Qtica/layouts/flow_layout.py
+-rw-r--r--   0        0        0     1453 2024-01-26 21:58:10.501833 qtica-0.5.0/Qtica/layouts/form_layout.py
+-rw-r--r--   0        0        0     1834 2024-01-10 17:17:48.310835 qtica-0.5.0/Qtica/layouts/grid_layout.py
+-rw-r--r--   0        0        0      653 2024-05-24 19:15:46.420575 qtica-0.5.0/Qtica/layouts/h_layout.py
+-rw-r--r--   0        0        0     1434 2024-03-06 01:03:24.721415 qtica-0.5.0/Qtica/layouts/stacked.py
+-rw-r--r--   0        0        0      650 2024-05-24 19:15:37.212575 qtica-0.5.0/Qtica/layouts/v_layout.py
+-rw-r--r--   0        0        0     1741 2024-04-15 21:13:58.605794 qtica-0.5.0/Qtica/layouts/vh_layout.py
+-rw-r--r--   0        0        0       93 2024-01-03 23:21:20.488233 qtica-0.5.0/Qtica/painters/__init__.py
+-rw-r--r--   0        0        0      296 2024-01-03 23:21:59.861489 qtica-0.5.0/Qtica/painters/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      302 2024-01-08 21:34:02.103270 qtica-0.5.0/Qtica/painters/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0    12804 2024-01-03 15:48:57.470679 qtica-0.5.0/Qtica/painters/__pycache__/_tails.cpython-310.pyc
+-rw-r--r--   0        0        0     3680 2024-02-07 22:28:14.820701 qtica-0.5.0/Qtica/painters/__pycache__/circular_progress.cpython-310.pyc
+-rw-r--r--   0        0        0     6465 2024-01-08 21:34:02.103270 qtica-0.5.0/Qtica/painters/__pycache__/circular_progress.cpython-312.pyc
+-rw-r--r--   0        0        0     3157 2024-02-14 21:22:24.140184 qtica-0.5.0/Qtica/painters/__pycache__/status_edge.cpython-310.pyc
+-rw-r--r--   0        0        0     4447 2024-01-08 22:46:03.445258 qtica-0.5.0/Qtica/painters/__pycache__/status_edge.cpython-312.pyc
+-rw-r--r--   0        0        0     1583 2024-01-03 15:57:26.454986 qtica-0.5.0/Qtica/painters/__pycache__/teaching_tip.cpython-310.pyc
+-rw-r--r--   0        0        0     3218 2024-01-30 23:56:24.180177 qtica-0.5.0/Qtica/painters/circular_progress.py
+-rw-r--r--   0        0        0     3438 2024-02-14 21:22:18.647958 qtica-0.5.0/Qtica/painters/status_edge.py
+-rw-r--r--   0        0        0      364 2024-01-25 22:53:45.089782 qtica-0.5.0/Qtica/services/__init__.py
+-rw-r--r--   0        0        0      637 2024-01-25 22:55:08.082550 qtica-0.5.0/Qtica/services/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      638 2024-01-09 22:33:14.059975 qtica-0.5.0/Qtica/services/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     5540 2024-03-06 18:55:45.168030 qtica-0.5.0/Qtica/services/__pycache__/_methods.cpython-310.pyc
+-rw-r--r--   0        0        0     7881 2024-01-09 23:00:50.721630 qtica-0.5.0/Qtica/services/__pycache__/_methods.cpython-312.pyc
+-rw-r--r--   0        0        0     1841 2024-01-10 15:38:23.900699 qtica-0.5.0/Qtica/services/__pycache__/clipboard.cpython-310.pyc
+-rw-r--r--   0        0        0     2934 2024-01-08 20:53:27.464991 qtica-0.5.0/Qtica/services/__pycache__/clipboard.cpython-312.pyc
+-rw-r--r--   0        0        0      424 2023-12-30 23:29:51.645175 qtica-0.5.0/Qtica/services/__pycache__/dialogs.cpython-310.pyc
+-rw-r--r--   0        0        0     2062 2024-01-10 15:38:23.936698 qtica-0.5.0/Qtica/services/__pycache__/launche_url.cpython-310.pyc
+-rw-r--r--   0        0        0     2902 2024-01-08 20:53:27.468991 qtica-0.5.0/Qtica/services/__pycache__/launche_url.cpython-312.pyc
+-rw-r--r--   0        0        0     3715 2024-01-10 15:38:23.916699 qtica-0.5.0/Qtica/services/__pycache__/message_handler.cpython-310.pyc
+-rw-r--r--   0        0        0     5190 2024-01-08 20:53:27.464991 qtica-0.5.0/Qtica/services/__pycache__/message_handler.cpython-312.pyc
+-rw-r--r--   0        0        0     4482 2024-03-06 18:54:48.048033 qtica-0.5.0/Qtica/services/_methods.py
+-rw-r--r--   0        0        0     1459 2024-01-05 15:32:29.184574 qtica-0.5.0/Qtica/services/clipboard.py
+-rw-r--r--   0        0        0     1584 2024-01-05 19:43:31.326908 qtica-0.5.0/Qtica/services/launche_url.py
+-rw-r--r--   0        0        0     3066 2024-01-05 22:05:02.546983 qtica-0.5.0/Qtica/services/message_handler.py
+-rw-r--r--   0        0        0      571 2024-03-29 23:07:12.932005 qtica-0.5.0/Qtica/tools/__init__.py
+-rw-r--r--   0        0        0      894 2024-03-29 23:09:29.403193 qtica-0.5.0/Qtica/tools/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      989 2024-01-09 20:38:36.585517 qtica-0.5.0/Qtica/tools/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     3309 2024-02-03 21:25:57.511488 qtica-0.5.0/Qtica/tools/__pycache__/action.cpython-310.pyc
+-rw-r--r--   0        0        0     5523 2024-01-08 20:53:27.420990 qtica-0.5.0/Qtica/tools/__pycache__/action.cpython-312.pyc
+-rw-r--r--   0        0        0      754 2023-12-28 21:18:56.132086 qtica-0.5.0/Qtica/tools/__pycache__/alignment.cpython-310.pyc
+-rw-r--r--   0        0        0      933 2024-01-08 20:53:27.416990 qtica-0.5.0/Qtica/tools/__pycache__/alignment.cpython-312.pyc
+-rw-r--r--   0        0        0      620 2024-01-10 15:38:23.748707 qtica-0.5.0/Qtica/tools/__pycache__/brush.cpython-310.pyc
+-rw-r--r--   0        0        0      742 2024-01-08 21:47:19.287555 qtica-0.5.0/Qtica/tools/__pycache__/brush.cpython-312.pyc
+-rw-r--r--   0        0        0      858 2023-10-24 03:26:38.665477 qtica-0.5.0/Qtica/tools/__pycache__/center.cpython-310.pyc
+-rw-r--r--   0        0        0      750 2024-01-09 16:49:45.043770 qtica-0.5.0/Qtica/tools/__pycache__/color.cpython-310.pyc
+-rw-r--r--   0        0        0      968 2024-01-08 20:53:27.408990 qtica-0.5.0/Qtica/tools/__pycache__/color.cpython-312.pyc
+-rw-r--r--   0        0        0     5053 2024-01-11 17:21:33.738867 qtica-0.5.0/Qtica/tools/__pycache__/copy_progress.cpython-310.pyc
+-rw-r--r--   0        0        0     8627 2024-01-08 20:53:27.384990 qtica-0.5.0/Qtica/tools/__pycache__/copy_progress.cpython-312.pyc
+-rw-r--r--   0        0        0     2084 2024-01-25 22:48:10.494644 qtica-0.5.0/Qtica/tools/__pycache__/elided_text.cpython-310.pyc
+-rw-r--r--   0        0        0     3016 2024-01-08 20:53:27.376990 qtica-0.5.0/Qtica/tools/__pycache__/elided_text.cpython-312.pyc
+-rw-r--r--   0        0        0     1420 2023-12-15 19:46:03.309951 qtica-0.5.0/Qtica/tools/__pycache__/env_var.cpython-310.pyc
+-rw-r--r--   0        0        0     2590 2024-01-04 00:30:03.155692 qtica-0.5.0/Qtica/tools/__pycache__/icon.cpython-310.pyc
+-rw-r--r--   0        0        0     4253 2024-01-08 20:53:27.408990 qtica-0.5.0/Qtica/tools/__pycache__/icon.cpython-312.pyc
+-rw-r--r--   0        0        0      657 2024-01-10 15:38:23.768706 qtica-0.5.0/Qtica/tools/__pycache__/linear_gradient.cpython-310.pyc
+-rw-r--r--   0        0        0      781 2024-01-09 20:38:36.613517 qtica-0.5.0/Qtica/tools/__pycache__/linear_gradient.cpython-312.pyc
+-rw-r--r--   0        0        0     1120 2023-10-20 21:31:44.954090 qtica-0.5.0/Qtica/tools/__pycache__/modifiers.cpython-310.pyc
+-rw-r--r--   0        0        0     1790 2024-01-08 20:53:27.412990 qtica-0.5.0/Qtica/tools/__pycache__/modifiers.cpython-312.pyc
+-rw-r--r--   0        0        0     3549 2024-02-03 21:25:57.459488 qtica-0.5.0/Qtica/tools/__pycache__/movie.cpython-310.pyc
+-rw-r--r--   0        0        0     5372 2024-01-08 20:53:27.424991 qtica-0.5.0/Qtica/tools/__pycache__/movie.cpython-312.pyc
+-rw-r--r--   0        0        0     3107 2023-12-12 00:58:38.762160 qtica-0.5.0/Qtica/tools/__pycache__/movie_view.cpython-310.pyc
+-rw-r--r--   0        0        0     1097 2023-11-25 19:52:04.430529 qtica-0.5.0/Qtica/tools/__pycache__/painter.cpython-310.pyc
+-rw-r--r--   0        0        0      612 2024-01-10 15:38:23.748707 qtica-0.5.0/Qtica/tools/__pycache__/pen.cpython-310.pyc
+-rw-r--r--   0        0        0      734 2024-01-08 21:47:19.287555 qtica-0.5.0/Qtica/tools/__pycache__/pen.cpython-312.pyc
+-rw-r--r--   0        0        0     2151 2023-12-07 21:52:01.116620 qtica-0.5.0/Qtica/tools/__pycache__/picker.cpython-310.pyc
+-rw-r--r--   0        0        0     5334 2023-12-26 19:35:47.115790 qtica-0.5.0/Qtica/tools/__pycache__/qstyle_sheet.cpython-310.pyc
+-rw-r--r--   0        0        0     2264 2024-03-29 23:11:57.666656 qtica-0.5.0/Qtica/tools/__pycache__/qt_file_open.cpython-310.pyc
+-rw-r--r--   0        0        0     1490 2024-01-08 20:53:27.372990 qtica-0.5.0/Qtica/tools/__pycache__/qt_file_open.cpython-312.pyc
+-rw-r--r--   0        0        0     5399 2024-02-14 20:13:11.611836 qtica-0.5.0/Qtica/tools/__pycache__/settings.cpython-310.pyc
+-rw-r--r--   0        0        0     7778 2024-01-08 20:53:27.428990 qtica-0.5.0/Qtica/tools/__pycache__/settings.cpython-312.pyc
+-rw-r--r--   0        0        0     1165 2024-02-03 21:25:57.467488 qtica-0.5.0/Qtica/tools/__pycache__/size_policy.cpython-310.pyc
+-rw-r--r--   0        0        0     1681 2024-01-08 20:53:27.412990 qtica-0.5.0/Qtica/tools/__pycache__/size_policy.cpython-312.pyc
+-rw-r--r--   0        0        0     4170 2024-01-09 16:49:44.975769 qtica-0.5.0/Qtica/tools/__pycache__/smooth_scroll.cpython-310.pyc
+-rw-r--r--   0        0        0     7792 2024-01-08 20:53:27.392990 qtica-0.5.0/Qtica/tools/__pycache__/smooth_scroll.cpython-312.pyc
+-rw-r--r--   0        0        0     1625 2023-10-14 15:42:21.017644 qtica-0.5.0/Qtica/tools/__pycache__/svg_color.cpython-310.pyc
+-rw-r--r--   0        0        0     1275 2024-01-09 16:49:45.179771 qtica-0.5.0/Qtica/tools/__pycache__/system_tray.cpython-310.pyc
+-rw-r--r--   0        0        0     1744 2024-01-08 20:53:27.420990 qtica-0.5.0/Qtica/tools/__pycache__/system_tray.cpython-312.pyc
+-rw-r--r--   0        0        0      977 2024-01-11 17:21:33.606867 qtica-0.5.0/Qtica/tools/__pycache__/ui_loader.cpython-310.pyc
+-rw-r--r--   0        0        0     1100 2024-01-08 20:53:27.268989 qtica-0.5.0/Qtica/tools/__pycache__/ui_loader.cpython-312.pyc
+-rw-r--r--   0        0        0     2358 2024-02-03 20:33:56.351554 qtica-0.5.0/Qtica/tools/action.py
+-rw-r--r--   0        0        0      367 2024-01-05 22:40:37.553867 qtica-0.5.0/Qtica/tools/color.py
+-rwxr-xr-x   0        0        0     5159 2024-01-10 17:35:50.234877 qtica-0.5.0/Qtica/tools/copy_progress.py
+-rw-r--r--   0        0        0     2873 2024-01-04 00:27:21.814009 qtica-0.5.0/Qtica/tools/icon.py
+-rw-r--r--   0        0        0      299 2024-02-23 21:11:01.536301 qtica-0.5.0/Qtica/tools/list_widget_item.py
+-rw-r--r--   0        0        0      551 2024-02-19 18:23:21.195464 qtica-0.5.0/Qtica/tools/media_player.py
+-rw-r--r--   0        0        0     2579 2024-02-03 20:29:22.499560 qtica-0.5.0/Qtica/tools/movie.py
+-rw-r--r--   0        0        0     1322 2024-03-29 23:11:46.982406 qtica-0.5.0/Qtica/tools/qt_file_open.py
+-rw-r--r--   0        0        0       63 2024-01-19 16:22:59.600859 qtica-0.5.0/Qtica/tools/qtcore/__init__.py
+-rw-r--r--   0        0        0      221 2024-01-19 16:24:36.376855 qtica-0.5.0/Qtica/tools/qtcore/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     8064 2024-03-29 23:09:29.427193 qtica-0.5.0/Qtica/tools/qtcore/__pycache__/objects.cpython-310.pyc
+-rw-r--r--   0        0        0     5917 2024-03-29 23:02:57.302034 qtica-0.5.0/Qtica/tools/qtcore/objects.py
+-rw-r--r--   0        0        0     6294 2024-03-29 23:02:27.389335 qtica-0.5.0/Qtica/tools/qtcore/tools.py
+-rw-r--r--   0        0        0       63 2024-01-11 17:03:17.454911 qtica-0.5.0/Qtica/tools/qtgui/__init__.py
+-rw-r--r--   0        0        0      220 2024-01-11 17:21:33.538867 qtica-0.5.0/Qtica/tools/qtgui/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     8761 2024-01-30 23:06:34.357316 qtica-0.5.0/Qtica/tools/qtgui/__pycache__/objects.cpython-310.pyc
+-rw-r--r--   0        0        0    20542 2024-03-05 01:55:52.657632 qtica-0.5.0/Qtica/tools/qtgui/__pycache__/tools.cpython-310.pyc
+-rw-r--r--   0        0        0     6373 2024-01-30 22:57:27.101139 qtica-0.5.0/Qtica/tools/qtgui/objects.py
+-rw-r--r--   0        0        0    15623 2024-03-05 01:48:08.930849 qtica-0.5.0/Qtica/tools/qtgui/tools.py
+-rw-r--r--   0        0        0     4228 2024-02-14 20:10:08.623882 qtica-0.5.0/Qtica/tools/settings.py
+-rw-r--r--   0        0        0      978 2024-02-03 20:26:10.731564 qtica-0.5.0/Qtica/tools/size_policy.py
+-rw-r--r--   0        0        0     5073 2024-01-05 16:47:52.546347 qtica-0.5.0/Qtica/tools/smooth_scroll.py
+-rw-r--r--   0        0        0      327 2024-02-07 22:32:29.616714 qtica-0.5.0/Qtica/tools/spacer_item.py
+-rwxr-xr-x   0        0        0      920 2024-01-08 19:19:47.884624 qtica-0.5.0/Qtica/tools/system_tray.py
+-rw-r--r--   0        0        0      503 2024-01-10 17:22:18.093342 qtica-0.5.0/Qtica/tools/ui_loader.py
+-rw-r--r--   0        0        0      327 2024-04-15 21:03:32.009211 qtica-0.5.0/Qtica/tools/wrappers/__init__.py
+-rw-r--r--   0        0        0      598 2024-04-15 21:15:46.082223 qtica-0.5.0/Qtica/tools/wrappers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      723 2024-01-08 20:53:27.432990 qtica-0.5.0/Qtica/tools/wrappers/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      777 2024-01-09 16:49:44.595764 qtica-0.5.0/Qtica/tools/wrappers/__pycache__/border_layout.cpython-310.pyc
+-rw-r--r--   0        0        0      943 2024-01-08 20:53:27.456991 qtica-0.5.0/Qtica/tools/wrappers/__pycache__/border_layout.cpython-312.pyc
+-rw-r--r--   0        0        0      832 2024-01-09 16:49:44.611765 qtica-0.5.0/Qtica/tools/wrappers/__pycache__/dock_widgets.cpython-310.pyc
+-rw-r--r--   0        0        0     1042 2024-01-08 20:53:27.456991 qtica-0.5.0/Qtica/tools/wrappers/__pycache__/dock_widgets.cpython-312.pyc
+-rw-r--r--   0        0        0      774 2024-01-09 16:49:44.655765 qtica-0.5.0/Qtica/tools/wrappers/__pycache__/form_layout.cpython-310.pyc
+-rw-r--r--   0        0        0      914 2024-01-08 20:53:27.456991 qtica-0.5.0/Qtica/tools/wrappers/__pycache__/form_layout.cpython-312.pyc
+-rw-r--r--   0        0        0      963 2024-01-09 16:49:44.635765 qtica-0.5.0/Qtica/tools/wrappers/__pycache__/grid_layout.cpython-310.pyc
+-rw-r--r--   0        0        0     1213 2024-01-08 20:53:27.456991 qtica-0.5.0/Qtica/tools/wrappers/__pycache__/grid_layout.cpython-312.pyc
+-rw-r--r--   0        0        0     1092 2024-01-09 16:49:44.579764 qtica-0.5.0/Qtica/tools/wrappers/__pycache__/h_layout.cpython-310.pyc
+-rw-r--r--   0        0        0     1346 2024-01-08 20:53:27.452991 qtica-0.5.0/Qtica/tools/wrappers/__pycache__/h_layout.cpython-312.pyc
+-rw-r--r--   0        0        0      862 2024-01-09 16:49:44.463763 qtica-0.5.0/Qtica/tools/wrappers/__pycache__/menu.cpython-310.pyc
+-rw-r--r--   0        0        0      952 2024-01-08 20:53:27.432990 qtica-0.5.0/Qtica/tools/wrappers/__pycache__/menu.cpython-312.pyc
+-rw-r--r--   0        0        0      758 2024-01-09 16:49:44.487763 qtica-0.5.0/Qtica/tools/wrappers/__pycache__/tool_bar.cpython-310.pyc
+-rw-r--r--   0        0        0      907 2024-01-08 20:53:27.432990 qtica-0.5.0/Qtica/tools/wrappers/__pycache__/tool_bar.cpython-312.pyc
+-rw-r--r--   0        0        0     1089 2024-01-09 16:49:44.579764 qtica-0.5.0/Qtica/tools/wrappers/__pycache__/v_layout.cpython-310.pyc
+-rw-r--r--   0        0        0     1343 2024-01-08 20:53:27.456991 qtica-0.5.0/Qtica/tools/wrappers/__pycache__/v_layout.cpython-312.pyc
+-rw-r--r--   0        0        0      571 2023-12-06 02:20:12.074653 qtica-0.5.0/Qtica/tools/wrappers/__pycache__/water_progress_bar.cpython-310.pyc
+-rw-r--r--   0        0        0      408 2024-01-06 00:15:08.651564 qtica-0.5.0/Qtica/tools/wrappers/border_layout.py
+-rw-r--r--   0        0        0      369 2024-01-05 19:36:18.305969 qtica-0.5.0/Qtica/tools/wrappers/dock_widgets.py
+-rw-r--r--   0        0        0      394 2024-01-05 23:47:27.369612 qtica-0.5.0/Qtica/tools/wrappers/form_layout.py
+-rw-r--r--   0        0        0      554 2024-01-06 00:02:38.132729 qtica-0.5.0/Qtica/tools/wrappers/grid_layout.py
+-rw-r--r--   0        0        0      559 2024-04-15 21:02:59.469475 qtica-0.5.0/Qtica/tools/wrappers/layout.py
+-rw-r--r--   0        0        0      345 2024-01-08 20:22:06.442801 qtica-0.5.0/Qtica/tools/wrappers/menu.py
+-rw-r--r--   0        0        0      276 2024-01-05 19:36:30.302033 qtica-0.5.0/Qtica/tools/wrappers/tool_bar.py
+-rw-r--r--   0        0        0      280 2024-04-01 22:30:33.427551 qtica-0.5.0/Qtica/utils/__init__.py
+-rw-r--r--   0        0        0      518 2024-04-01 22:33:32.355544 qtica-0.5.0/Qtica/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      598 2024-01-08 20:53:27.072988 qtica-0.5.0/Qtica/utils/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      184 2024-01-08 18:17:07.446404 qtica-0.5.0/Qtica/utils/__pycache__/_check_none.cpython-312.pyc
+-rw-r--r--   0        0        0     4298 2024-05-24 19:31:35.901069 qtica-0.5.0/Qtica/utils/__pycache__/_classes.cpython-310.pyc
+-rw-r--r--   0        0        0     5263 2024-01-08 20:53:27.168989 qtica-0.5.0/Qtica/utils/__pycache__/_classes.cpython-312.pyc
+-rw-r--r--   0        0        0     4030 2023-10-10 15:17:33.773698 qtica-0.5.0/Qtica/utils/__pycache__/_ensure_thread.cpython-310.pyc
+-rw-r--r--   0        0        0     1429 2024-05-24 19:31:35.857063 qtica-0.5.0/Qtica/utils/__pycache__/_env_var.cpython-310.pyc
+-rw-r--r--   0        0        0     1875 2024-01-08 20:53:27.076988 qtica-0.5.0/Qtica/utils/__pycache__/_env_var.cpython-312.pyc
+-rw-r--r--   0        0        0      902 2024-01-18 19:01:08.648313 qtica-0.5.0/Qtica/utils/__pycache__/_exception_handler.cpython-310.pyc
+-rw-r--r--   0        0        0     1145 2024-01-08 20:53:27.160989 qtica-0.5.0/Qtica/utils/__pycache__/_exception_handler.cpython-312.pyc
+-rw-r--r--   0        0        0     1368 2023-11-07 22:10:24.611217 qtica-0.5.0/Qtica/utils/__pycache__/_import.cpython-310.pyc
+-rw-r--r--   0        0        0     3707 2023-10-10 15:18:15.261924 qtica-0.5.0/Qtica/utils/__pycache__/_message_handler.cpython-310.pyc
+-rw-r--r--   0        0        0      969 2023-12-25 20:05:00.304545 qtica-0.5.0/Qtica/utils/__pycache__/_none_check.cpython-310.pyc
+-rw-r--r--   0        0        0     1937 2023-12-28 21:14:07.216964 qtica-0.5.0/Qtica/utils/__pycache__/_routes.cpython-310.pyc
+-rw-r--r--   0        0        0     2716 2024-01-09 16:49:44.031758 qtica-0.5.0/Qtica/utils/__pycache__/_text_wrap.cpython-310.pyc
+-rw-r--r--   0        0        0     3776 2024-01-08 20:53:27.088988 qtica-0.5.0/Qtica/utils/__pycache__/_text_wrap.cpython-312.pyc
+-rw-r--r--   0        0        0      754 2024-01-11 17:21:33.254867 qtica-0.5.0/Qtica/utils/__pycache__/alignment.cpython-310.pyc
+-rw-r--r--   0        0        0     2708 2023-09-25 12:17:07.616295 qtica-0.5.0/Qtica/utils/__pycache__/auto_wrap.cpython-310.pyc
+-rw-r--r--   0        0        0     5403 2023-11-11 01:22:23.745200 qtica-0.5.0/Qtica/utils/__pycache__/color.cpython-310.pyc
+-rw-r--r--   0        0        0      485 2023-12-26 22:32:06.735730 qtica-0.5.0/Qtica/utils/__pycache__/dialogs.cpython-310.pyc
+-rw-r--r--   0        0        0     1422 2023-12-31 19:49:03.787973 qtica-0.5.0/Qtica/utils/__pycache__/env_var.cpython-310.pyc
+-rw-r--r--   0        0        0      922 2023-09-25 12:17:07.580295 qtica-0.5.0/Qtica/utils/__pycache__/exception_handler.cpython-310.pyc
+-rw-r--r--   0        0        0     1810 2023-12-26 19:38:29.807787 qtica-0.5.0/Qtica/utils/__pycache__/methods.cpython-310.pyc
+-rw-r--r--   0        0        0     1119 2024-01-11 17:21:33.258867 qtica-0.5.0/Qtica/utils/__pycache__/modifiers.cpython-310.pyc
+-rw-r--r--   0        0        0     2265 2023-10-02 22:43:31.865968 qtica-0.5.0/Qtica/utils/__pycache__/multimethod.cpython-310.pyc
+-rw-r--r--   0        0        0     4423 2023-10-20 21:31:47.218122 qtica-0.5.0/Qtica/utils/__pycache__/overload.cpython-310.pyc
+-rw-r--r--   0        0        0     5334 2024-01-11 17:21:33.218867 qtica-0.5.0/Qtica/utils/__pycache__/qstyle_sheet.cpython-310.pyc
+-rw-r--r--   0        0        0     8753 2024-01-08 20:53:27.092988 qtica-0.5.0/Qtica/utils/__pycache__/qstyle_sheet.cpython-312.pyc
+-rw-r--r--   0        0        0     2373 2024-01-09 16:49:43.967757 qtica-0.5.0/Qtica/utils/__pycache__/routes.cpython-310.pyc
+-rw-r--r--   0        0        0     3404 2024-01-08 20:53:27.076988 qtica-0.5.0/Qtica/utils/__pycache__/routes.cpython-312.pyc
+-rw-r--r--   0        0        0     5267 2023-10-16 11:38:26.513552 qtica-0.5.0/Qtica/utils/__pycache__/system.cpython-310.pyc
+-rw-r--r--   0        0        0     2979 2024-05-24 19:21:52.937888 qtica-0.5.0/Qtica/utils/_classes.py
+-rw-r--r--   0        0        0      997 2024-05-24 19:24:08.276394 qtica-0.5.0/Qtica/utils/_env_var.py
+-rw-r--r--   0        0        0     3531 2023-08-25 23:14:12.080003 qtica-0.5.0/Qtica/utils/_text_wrap.py
+-rw-r--r--   0        0        0      386 2023-12-28 21:18:40.864073 qtica-0.5.0/Qtica/utils/alignment.py
+-rw-r--r--   0        0        0      305 2023-04-14 05:53:29.635829 qtica-0.5.0/Qtica/utils/caseconverter/__init__.py
+-rw-r--r--   0        0        0      644 2024-01-09 16:49:44.191760 qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      665 2024-01-08 20:53:27.172989 qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     4924 2024-01-09 16:49:44.251761 qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/boundaries.cpython-310.pyc
+-rw-r--r--   0        0        0     6612 2024-01-08 20:53:27.204989 qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/boundaries.cpython-312.pyc
+-rw-r--r--   0        0        0     1214 2024-01-09 16:49:44.247761 qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/camel.cpython-310.pyc
+-rw-r--r--   0        0        0     1553 2024-01-08 20:53:27.200989 qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/camel.cpython-312.pyc
+-rw-r--r--   0        0        0     6731 2024-01-09 16:49:44.195760 qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/caseconverter.cpython-310.pyc
+-rw-r--r--   0        0        0     8791 2024-01-08 20:53:27.176989 qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/caseconverter.cpython-312.pyc
+-rw-r--r--   0        0        0     1383 2024-01-09 16:49:44.255761 qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/cobol.cpython-310.pyc
+-rw-r--r--   0        0        0     2029 2024-01-08 20:53:27.208989 qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/cobol.cpython-312.pyc
+-rw-r--r--   0        0        0     1208 2024-01-09 16:49:44.255761 qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/flat.cpython-310.pyc
+-rw-r--r--   0        0        0     1547 2024-01-08 20:53:27.208989 qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/flat.cpython-312.pyc
+-rw-r--r--   0        0        0     1253 2024-01-09 16:49:44.259761 qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/kebab.cpython-310.pyc
+-rw-r--r--   0        0        0     1643 2024-01-08 20:53:27.212989 qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/kebab.cpython-312.pyc
+-rw-r--r--   0        0        0     1686 2024-01-09 16:49:44.263761 qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/macro.cpython-310.pyc
+-rw-r--r--   0        0        0     2506 2024-01-08 20:53:27.216989 qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/macro.cpython-312.pyc
+-rw-r--r--   0        0        0     1501 2024-01-09 16:49:44.263761 qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/pascal.cpython-310.pyc
+-rw-r--r--   0        0        0     2007 2024-01-08 20:53:27.216989 qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/pascal.cpython-312.pyc
+-rw-r--r--   0        0        0     1254 2024-01-09 16:49:44.267761 qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/snake.cpython-310.pyc
+-rw-r--r--   0        0        0     1644 2024-01-08 20:53:27.216989 qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/snake.cpython-312.pyc
+-rw-r--r--   0        0        0     3384 2023-04-14 05:53:29.635829 qtica-0.5.0/Qtica/utils/caseconverter/boundaries.py
+-rw-r--r--   0        0        0      658 2023-04-14 05:53:29.635829 qtica-0.5.0/Qtica/utils/caseconverter/camel.py
+-rw-r--r--   0        0        0     6043 2023-04-14 05:53:29.635829 qtica-0.5.0/Qtica/utils/caseconverter/caseconverter.py
+-rw-r--r--   0        0        0      902 2023-04-14 05:53:29.635829 qtica-0.5.0/Qtica/utils/caseconverter/cobol.py
+-rw-r--r--   0        0        0      655 2023-04-14 05:53:29.635829 qtica-0.5.0/Qtica/utils/caseconverter/flat.py
+-rw-r--r--   0        0        0      734 2023-04-14 05:53:29.635829 qtica-0.5.0/Qtica/utils/caseconverter/kebab.py
+-rw-r--r--   0        0        0     1236 2023-04-14 05:53:29.635829 qtica-0.5.0/Qtica/utils/caseconverter/macro.py
+-rw-r--r--   0        0        0      932 2023-04-14 05:53:29.635829 qtica-0.5.0/Qtica/utils/caseconverter/pascal.py
+-rw-r--r--   0        0        0      735 2023-04-14 05:53:29.639829 qtica-0.5.0/Qtica/utils/caseconverter/snake.py
+-rw-r--r--   0        0        0     2601 2024-04-01 22:26:25.839561 qtica-0.5.0/Qtica/utils/key_events.py
+-rw-r--r--   0        0        0     2612 2024-01-09 22:28:05.841998 qtica-0.5.0/Qtica/utils/maths/__init__.py
+-rw-r--r--   0        0        0     3000 2024-01-10 15:38:23.968696 qtica-0.5.0/Qtica/utils/maths/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3514 2024-01-09 22:33:14.063975 qtica-0.5.0/Qtica/utils/maths/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     3580 2024-01-10 15:38:23.972696 qtica-0.5.0/Qtica/utils/maths/__pycache__/geometry.cpython-310.pyc
+-rw-r--r--   0        0        0     5513 2024-01-09 22:33:14.063975 qtica-0.5.0/Qtica/utils/maths/__pycache__/geometry.cpython-312.pyc
+-rw-r--r--   0        0        0    16234 2024-01-10 15:38:23.992695 qtica-0.5.0/Qtica/utils/maths/__pycache__/vector.cpython-310.pyc
+-rw-r--r--   0        0        0    22140 2024-01-09 22:33:14.067975 qtica-0.5.0/Qtica/utils/maths/__pycache__/vector.cpython-312.pyc
+-rw-r--r--   0        0        0     3788 2023-10-10 14:54:54.637867 qtica-0.5.0/Qtica/utils/maths/geometry.py
+-rw-r--r--   0        0        0    13540 2024-01-05 22:01:09.346451 qtica-0.5.0/Qtica/utils/maths/vector.py
+-rw-r--r--   0        0        0      651 2024-03-29 20:17:25.161273 qtica-0.5.0/Qtica/widgets/__init__.py
+-rw-r--r--   0        0        0     1003 2024-03-29 20:28:00.512804 qtica-0.5.0/Qtica/widgets/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      918 2024-01-09 20:38:36.585517 qtica-0.5.0/Qtica/widgets/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0    15554 2024-02-23 21:14:48.069514 qtica-0.5.0/Qtica/widgets/__pycache__/_widgets.cpython-310.pyc
+-rw-r--r--   0        0        0     4221 2024-03-29 20:28:02.476825 qtica-0.5.0/Qtica/widgets/__pycache__/application.cpython-310.pyc
+-rw-r--r--   0        0        0     6224 2024-01-09 16:19:44.091527 qtica-0.5.0/Qtica/widgets/__pycache__/application.cpython-312.pyc
+-rw-r--r--   0        0        0     1804 2024-01-19 15:27:34.556994 qtica-0.5.0/Qtica/widgets/__pycache__/buttons.cpython-310.pyc
+-rw-r--r--   0        0        0     1348 2024-01-10 15:38:24.292680 qtica-0.5.0/Qtica/widgets/__pycache__/frame.cpython-310.pyc
+-rw-r--r--   0        0        0     1984 2024-01-08 21:14:34.756360 qtica-0.5.0/Qtica/widgets/__pycache__/frame.cpython-312.pyc
+-rw-r--r--   0        0        0     2457 2024-01-26 21:27:49.435621 qtica-0.5.0/Qtica/widgets/__pycache__/icon_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     3835 2024-01-08 21:14:34.744359 qtica-0.5.0/Qtica/widgets/__pycache__/icon_widget.cpython-312.pyc
+-rw-r--r--   0        0        0      900 2024-01-10 15:38:24.204685 qtica-0.5.0/Qtica/widgets/__pycache__/label.cpython-310.pyc
+-rw-r--r--   0        0        0     1148 2024-01-08 21:14:34.728359 qtica-0.5.0/Qtica/widgets/__pycache__/label.cpython-312.pyc
+-rw-r--r--   0        0        0     1206 2024-01-10 15:38:24.268682 qtica-0.5.0/Qtica/widgets/__pycache__/line.cpython-310.pyc
+-rw-r--r--   0        0        0     1852 2024-01-08 21:14:34.748360 qtica-0.5.0/Qtica/widgets/__pycache__/line.cpython-312.pyc
+-rw-r--r--   0        0        0      641 2024-01-10 15:38:24.232683 qtica-0.5.0/Qtica/widgets/__pycache__/line_edit.cpython-310.pyc
+-rw-r--r--   0        0        0      763 2024-01-08 21:14:34.740359 qtica-0.5.0/Qtica/widgets/__pycache__/line_edit.cpython-312.pyc
+-rw-r--r--   0        0        0     1183 2024-01-10 15:38:24.204685 qtica-0.5.0/Qtica/widgets/__pycache__/menu.cpython-310.pyc
+-rw-r--r--   0        0        0     1700 2024-01-08 21:14:34.724359 qtica-0.5.0/Qtica/widgets/__pycache__/menu.cpython-312.pyc
+-rw-r--r--   0        0        0     1281 2024-01-10 15:38:24.280681 qtica-0.5.0/Qtica/widgets/__pycache__/push_button.cpython-310.pyc
+-rw-r--r--   0        0        0     2065 2024-01-08 22:30:38.193588 qtica-0.5.0/Qtica/widgets/__pycache__/push_button.cpython-312.pyc
+-rw-r--r--   0        0        0     1294 2024-03-06 00:22:49.159530 qtica-0.5.0/Qtica/widgets/__pycache__/scroll_area.cpython-310.pyc
+-rw-r--r--   0        0        0     2040 2024-01-08 21:14:34.740359 qtica-0.5.0/Qtica/widgets/__pycache__/scroll_area.cpython-312.pyc
+-rw-r--r--   0        0        0     2280 2024-01-12 10:41:21.071686 qtica-0.5.0/Qtica/widgets/__pycache__/size_grip.cpython-310.pyc
+-rw-r--r--   0        0        0     4717 2024-01-08 20:53:27.460991 qtica-0.5.0/Qtica/widgets/__pycache__/size_grip.cpython-312.pyc
+-rw-r--r--   0        0        0      888 2024-01-10 15:38:24.292680 qtica-0.5.0/Qtica/widgets/__pycache__/spin_box.cpython-310.pyc
+-rw-r--r--   0        0        0     1172 2024-01-09 20:38:36.629517 qtica-0.5.0/Qtica/widgets/__pycache__/spin_box.cpython-312.pyc
+-rw-r--r--   0        0        0     3053 2024-03-29 20:28:02.360824 qtica-0.5.0/Qtica/widgets/__pycache__/stack.cpython-310.pyc
+-rw-r--r--   0        0        0     6006 2024-01-08 21:14:34.732359 qtica-0.5.0/Qtica/widgets/__pycache__/stack.cpython-312.pyc
+-rw-r--r--   0        0        0     1072 2024-01-26 20:01:11.773359 qtica-0.5.0/Qtica/widgets/__pycache__/stacked_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     1554 2024-01-08 21:14:34.756360 qtica-0.5.0/Qtica/widgets/__pycache__/stacked_widget.cpython-312.pyc
+-rw-r--r--   0        0        0     1281 2024-01-10 15:38:24.252682 qtica-0.5.0/Qtica/widgets/__pycache__/tool_button.cpython-310.pyc
+-rw-r--r--   0        0        0     2065 2024-01-08 21:14:34.748360 qtica-0.5.0/Qtica/widgets/__pycache__/tool_button.cpython-312.pyc
+-rw-r--r--   0        0        0      889 2024-01-10 15:38:24.224684 qtica-0.5.0/Qtica/widgets/__pycache__/widget.cpython-310.pyc
+-rw-r--r--   0        0        0     1201 2024-01-08 21:14:34.736359 qtica-0.5.0/Qtica/widgets/__pycache__/widget.cpython-312.pyc
+-rw-r--r--   0        0        0    10904 2024-02-23 21:14:45.105707 qtica-0.5.0/Qtica/widgets/_widgets.py
+-rw-r--r--   0        0        0     3386 2024-03-29 20:18:00.114275 qtica-0.5.0/Qtica/widgets/application.py
+-rw-r--r--   0        0        0     1275 2024-01-19 15:21:48.697008 qtica-0.5.0/Qtica/widgets/buttons.py
+-rw-r--r--   0        0        0     1431 2024-03-06 00:36:56.343443 qtica-0.5.0/Qtica/widgets/container.py
+-rw-r--r--   0        0        0      114 2024-01-05 17:16:11.467069 qtica-0.5.0/Qtica/widgets/dialogs/__init__.py
+-rw-r--r--   0        0        0      328 2024-01-10 15:38:24.024693 qtica-0.5.0/Qtica/widgets/dialogs/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      341 2024-01-08 20:53:27.468991 qtica-0.5.0/Qtica/widgets/dialogs/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     1873 2024-01-03 00:16:32.516166 qtica-0.5.0/Qtica/widgets/dialogs/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     2609 2024-01-03 00:16:32.592168 qtica-0.5.0/Qtica/widgets/dialogs/__pycache__/large_text.cpython-310.pyc
+-rw-r--r--   0        0        0     5124 2024-01-30 23:06:34.901321 qtica-0.5.0/Qtica/widgets/dialogs/__pycache__/mask.cpython-310.pyc
+-rw-r--r--   0        0        0    10088 2024-01-09 18:38:18.598559 qtica-0.5.0/Qtica/widgets/dialogs/__pycache__/mask.cpython-312.pyc
+-rw-r--r--   0        0        0     2278 2024-01-10 15:38:24.108689 qtica-0.5.0/Qtica/widgets/dialogs/__pycache__/silent.cpython-310.pyc
+-rw-r--r--   0        0        0     3601 2024-01-08 21:14:34.548353 qtica-0.5.0/Qtica/widgets/dialogs/__pycache__/silent.cpython-312.pyc
+-rw-r--r--   0        0        0     3936 2024-01-03 00:16:51.004672 qtica-0.5.0/Qtica/widgets/dialogs/__pycache__/teaching_tip.cpython-310.pyc
+-rw-r--r--   0        0        0     2794 2024-01-03 00:16:32.516166 qtica-0.5.0/Qtica/widgets/dialogs/__pycache__/text.cpython-310.pyc
+-rw-r--r--   0        0        0     4761 2024-01-30 22:34:46.218899 qtica-0.5.0/Qtica/widgets/dialogs/mask.py
+-rwxr-xr-x   0        0        0     1977 2024-01-05 19:58:29.964501 qtica-0.5.0/Qtica/widgets/dialogs/silent.py
+-rw-r--r--   0        0        0    14689 2024-01-10 15:38:24.104689 qtica-0.5.0/Qtica/widgets/dialogs/teaching_tip/__pycache__/tails.cpython-310.pyc
+-rw-r--r--   0        0        0    28937 2024-01-09 18:54:58.400518 qtica-0.5.0/Qtica/widgets/dialogs/teaching_tip/__pycache__/tails.cpython-312.pyc
+-rw-r--r--   0        0        0     3779 2024-05-24 19:31:37.233257 qtica-0.5.0/Qtica/widgets/dialogs/teaching_tip/__pycache__/tool_tip.cpython-310.pyc
+-rw-r--r--   0        0        0     7115 2024-01-09 18:50:32.343688 qtica-0.5.0/Qtica/widgets/dialogs/teaching_tip/__pycache__/tool_tip.cpython-312.pyc
+-rw-r--r--   0        0        0    13367 2024-01-09 18:54:53.360501 qtica-0.5.0/Qtica/widgets/dialogs/teaching_tip/tails.py
+-rw-r--r--   0        0        0     2897 2024-05-24 19:28:32.040294 qtica-0.5.0/Qtica/widgets/dialogs/teaching_tip/tool_tip.py
+-rw-r--r--   0        0        0     4180 2024-01-30 23:02:54.923640 qtica-0.5.0/Qtica/widgets/eliding_label.py
+-rw-r--r--   0        0        0      564 2024-01-19 15:21:36.657008 qtica-0.5.0/Qtica/widgets/group_box.py
+-rw-r--r--   0        0        0     2352 2024-01-26 21:27:46.686318 qtica-0.5.0/Qtica/widgets/icon_widget.py
+-rw-r--r--   0        0        0      388 2023-12-26 19:29:47.031798 qtica-0.5.0/Qtica/widgets/label.py
+-rw-r--r--   0        0        0      582 2024-01-05 20:04:13.311864 qtica-0.5.0/Qtica/widgets/line.py
+-rw-r--r--   0        0        0     1257 2024-01-08 20:51:10.080131 qtica-0.5.0/Qtica/widgets/menu.py
+-rw-r--r--   0        0        0     1572 2024-03-29 23:14:49.706674 qtica-0.5.0/Qtica/widgets/quick_widget.py
+-rw-r--r--   0        0        0      987 2024-03-06 00:22:38.111156 qtica-0.5.0/Qtica/widgets/scroll_area.py
+-rw-r--r--   0        0        0     1999 2024-01-11 18:18:59.194727 qtica-0.5.0/Qtica/widgets/size_grip.py
+-rw-r--r--   0        0        0     3777 2024-03-21 22:24:46.088198 qtica-0.5.0/Qtica/widgets/stack.py
+-rw-r--r--   0        0        0      830 2024-01-26 20:00:20.440515 qtica-0.5.0/Qtica/widgets/stacked_widget.py
+-rw-r--r--   0        0        0      647 2024-02-14 19:18:15.910409 qtica-0.5.0/Qtica/widgets/video_widget.py
+-rw-r--r--   0        0        0      102 2024-01-13 16:32:35.376140 qtica-0.5.0/Qtica/widgets/window/__init__.py
+-rw-r--r--   0        0        0      315 2024-01-13 16:34:16.977749 qtica-0.5.0/Qtica/widgets/window/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      288 2024-01-08 20:53:27.264989 qtica-0.5.0/Qtica/widgets/window/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     2768 2024-02-06 15:29:00.747194 qtica-0.5.0/Qtica/widgets/window/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     3699 2024-02-03 21:25:57.515488 qtica-0.5.0/Qtica/widgets/window/__pycache__/frameless.cpython-310.pyc
+-rw-r--r--   0        0        0     6387 2024-01-08 20:53:27.460991 qtica-0.5.0/Qtica/widgets/window/__pycache__/frameless.cpython-312.pyc
+-rw-r--r--   0        0        0      649 2024-01-14 06:19:43.142189 qtica-0.5.0/Qtica/widgets/window/__pycache__/mainwindow.cpython-310.pyc
+-rw-r--r--   0        0        0     4189 2024-01-08 20:53:27.264989 qtica-0.5.0/Qtica/widgets/window/__pycache__/mainwindow.cpython-312.pyc
+-rw-r--r--   0        0        0     3294 2023-12-26 19:38:29.799787 qtica-0.5.0/Qtica/widgets/window/__pycache__/routes.cpython-310.pyc
+-rw-r--r--   0        0        0     2490 2024-02-06 15:20:04.943215 qtica-0.5.0/Qtica/widgets/window/base.py
+-rw-r--r--   0        0        0     3883 2024-02-03 21:17:22.707499 qtica-0.5.0/Qtica/widgets/window/frameless.py
+-rw-r--r--   0        0        0      244 2024-01-14 06:19:22.430665 qtica-0.5.0/Qtica/widgets/window/mainwindow.py
+-rw-r--r--   0        0        0     3166 2024-05-24 19:40:35.393413 qtica-0.5.0/README.md
+-rw-r--r--   0        0        0     1650 2024-05-24 19:40:16.649616 qtica-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    21955 1970-01-01 00:00:00.000000 qtica-0.5.0/PKG-INFO
```

### Comparing `qtica-0.4.3/CHANGELOG.md` & `qtica-0.5.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -667,8 +667,45 @@
   - `LinearGradient`
   - `BoxShadow`
 - `tools.ListWidgetItem`
 - `widgets.ListWidget` addItemWidget, addItemDelegate methods
 
 ### Fixed
 
-- `tools.qtcore.tools`, `tools.qtgui.tools` has no attribute, in aarch64 machines
+- `tools.qtcore.tools`, `tools.qtgui.tools` has no attribute, in aarch64 machines
+
+## 0.5.0 (2024-05-24)
+
+### Added
+
+- `layout.stacked.StackedLayout` Routes, dict types support.
+- `enums.QPA_Platforms` vnc, wayland_egl, vkkhrdisplay
+- `core.AbstractWidget` **PosEventsRange**, **PosEventsArg**, **PosEvents** classes
+- `core.AbstractWidget` **at_pos** argument.
+- `widgets.QuickWidget`
+- `tools.qtcore.objects.File`
+- `tools.TempFile`
+- `utils.BaseDir`
+- `utils.Modifiers`, `utils.Keys`, `utils.KeySequence`
+- `tools.LayoutWrapper`
+
+### Fixed
+
+- `core.AbstractBase` value type error when insert MArgs class type to add[Methods]
+
+### Changed
+
+- `tools.File` has been renamed to `tools.OpenFile`
+- `utils.modifiers.py` has been renamed to `utils.key_events.py`
+
+### Updated
+
+- `widgets.QuickWidget` **qml** argument can accept QML code from string.
+
+### Removed
+
+- `utils.CheckNone`
+- `tools.`
+  - `HLayoutWrapper`
+  - `ColumnLayoutWrapper`
+  - `RowLayoutWrapper`
+  - `VLayoutWrapper`
```

### Comparing `qtica-0.4.3/LICENSE` & `qtica-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/animations/parallel_animation_group.py` & `qtica-0.5.0/Qtica/animations/parallel_animation_group.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/animations/property_animation.py` & `qtica-0.5.0/Qtica/animations/property_animation.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/animations/sequential_animation_group.py` & `qtica-0.5.0/Qtica/animations/sequential_animation_group.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/core/__pycache__/_base.cpython-310.pyc` & `qtica-0.5.0/Qtica/core/__pycache__/_base.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Feb 18 20:32:17 2024 UTC, .py size: 7606 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5169 d265 b61d 0000  o.......Qi.e....
+00000000: 6f0d 0d0a 0000 0000 34c8 e765 b21d 0000  o.......4..e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6400 6402 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 6d07 5a07 0100 6400 6403 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6404 6405 6c0a 6d0b 5a0b 6d0c 5a0c  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6404 6406 6c0d 6d0e 5a0e 6d0f 5a0f  ..d.d.l.m.Z.m.Z.
@@ -382,15 +382,15 @@
 000017d0: 686f 6473 6303 0000 0000 0000 0000 0000  hodsc...........
 000017e0: 0005 0000 0006 0000 0043 0000 0073 9800  .........C...s..
 000017f0: 0000 7c00 a000 7c01 a101 0400 7d03 6400  ..|...|.....}.d.
 00001800: 7501 7248 7401 7c03 8301 724a 7402 7c02  u.rHt.|...rJt.|.
 00001810: 7403 8302 7230 7c02 a004 a100 4400 5d17  t...r0|.....D.].
 00001820: 7d04 7402 7c04 7405 8302 7229 7c03 7c04  }.t.|.t...r)|.|.
 00001830: a004 a100 6900 7c04 a006 a100 a401 8e01  ....i.|.........
-00001840: 0100 7116 7c03 7c02 8301 0100 7116 6400  ..q.|.|.....q.d.
+00001840: 0100 7116 7c03 7c04 8301 0100 7116 6400  ..q.|.|.....q.d.
 00001850: 5300 7402 7c02 7405 8302 7242 7c03 7c02  S.t.|.t...rB|.|.
 00001860: a004 a100 6900 7c02 a006 a100 a401 8e01  ....i.|.........
 00001870: 0100 6400 5300 7c03 7c02 8301 0100 6400  ..d.S.|.|.....d.
 00001880: 5300 6400 5300 6400 5300 7213 0000 0029  S.d.S.d.S.r....)
 00001890: 0772 4000 0000 7246 0000 0072 4400 0000  .r@...rF...rD...
 000018a0: 722c 0000 0072 1900 0000 722a 0000 0072  r,...r....r*...r
 000018b0: 1a00 0000 2905 7217 0000 0072 3d00 0000  ....).r....r=...
```

### Comparing `qtica-0.4.3/Qtica/core/__pycache__/_config.cpython-310.pyc` & `qtica-0.5.0/Qtica/core/__pycache__/_config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/core/__pycache__/_declarative.cpython-310.pyc` & `qtica-0.5.0/Qtica/core/__pycache__/_declarative.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/core/__pycache__/_dialog.cpython-310.pyc` & `qtica-0.5.0/Qtica/core/__pycache__/_dialog.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jan 23 18:48:11 2024 UTC, .py size: 1513 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,132 +1,129 @@
-00000000: 6f0d 0d0a 0000 0000 eb09 b065 e905 0000  o..........e....
+00000000: 6f0d 0d0a 0000 0000 77be e865 7906 0000  o.......w..ey...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
+00000020: 0005 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6400 6403 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
-00000060: 0100 6404 6405 6c0a 6d0b 5a0b 0100 4700  ..d.d.l.m.Z...G.
-00000070: 6406 6407 8400 6407 650b 6502 8304 5a0c  d.d...d.e.e...Z.
-00000080: 6408 5300 2909 e900 0000 0029 03da 0c51  d.S.)......)...Q
-00000090: 4170 706c 6963 6174 696f 6eda 0751 4469  Application..QDi
-000000a0: 616c 6f67 da07 5157 6964 6765 7429 03da  alog..QWidget)..
-000000b0: 0651 4576 656e 74da 0751 4f62 6a65 6374  .QEvent..QObject
-000000c0: da06 5154 696d 6572 2901 da0a 5153 686f  ..QTimer)...QSho
-000000d0: 7745 7665 6e74 e901 0000 0029 01da 0e41  wEvent.....)...A
-000000e0: 6273 7472 6163 7457 6964 6765 7463 0000  bstractWidgetc..
-000000f0: 0000 0000 0000 0000 0000 0000 0000 0600  ................
-00000100: 0000 0000 0000 736e 0000 0065 005a 0164  ......sn...e.Z.d
-00000110: 005a 0209 0109 0264 1164 0365 0364 0465  .Z.....d.d.e.d.e
-00000120: 0466 0487 0066 0164 0564 0684 0d5a 0565  .f...f.d.d...Z.e
-00000130: 0664 0765 0766 0264 0864 0984 0483 015a  .d.e.f.d.d.....Z
-00000140: 0864 0a65 0964 0764 0166 0487 0066 0164  .d.e.d.d.f...f.d
-00000150: 0b64 0c84 0c5a 0a64 0d65 0b64 0e65 0c64  .d...Z.d.e.d.e.d
-00000160: 0765 0466 0687 0066 0164 0f64 1084 0c5a  .e.f...f.d.d...Z
-00000170: 0d87 0004 005a 0e53 0029 12da 0e41 6273  .....Z.S.)...Abs
-00000180: 7472 6163 7444 6961 6c6f 674e 46da 0774  tractDialogNF..t
-00000190: 696d 656f 7574 da0a 6175 746f 5f63 6c6f  imeout..auto_clo
-000001a0: 7365 6303 0000 0000 0000 0000 0000 0005  sec.............
-000001b0: 0000 0004 0000 000b 0000 0073 7a00 0000  ...........sz...
-000001c0: 7400 a001 a100 7d04 7c02 7314 8700 6601  t.....}.|.s...f.
-000001d0: 6401 6402 8408 7c04 5f02 8700 6601 6403  d.d...|._...f.d.
-000001e0: 6402 8408 7c04 5f03 7404 a005 8800 7c04  d...|._.t.....|.
-000001f0: a102 0100 7406 8300 6a05 6404 6900 7c03  ....t...j.d.i.|.
-00000200: a401 8e01 0100 8800 a007 a100 a008 8800  ................
-00000210: a101 0100 8800 6a09 6400 7501 7235 8800  ......j.d.u.r5..
-00000220: 6a09 a008 8800 a101 0100 7c01 8800 5f0a  j.........|..._.
-00000230: 7c02 8800 5f0b 6400 5300 2905 4e63 0100  |..._.d.S.).Nc..
-00000240: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00000250: 0000 1300 0000 f308 0000 0088 00a0 00a1  ................
-00000260: 0053 00a9 014e 2901 da04 6869 6465 a901  .S...N)...hide..
-00000270: da01 5fa9 01da 0473 656c 66a9 00fa 4e2f  .._....self...N/
-00000280: 686f 6d65 2f6f 7361 6d61 2f57 6f72 6b73  home/osama/Works
-00000290: 7061 6365 2f2e 7665 6e76 2f6c 6962 2f70  pace/.venv/lib/p
-000002a0: 7974 686f 6e33 2e31 302f 7369 7465 2d70  ython3.10/site-p
-000002b0: 6163 6b61 6765 732f 5174 6963 612f 636f  ackages/Qtica/co
-000002c0: 7265 2f5f 6469 616c 6f67 2e70 79da 083c  re/_dialog.py..<
-000002d0: 6c61 6d62 6461 3e11 0000 00f3 0200 0000  lambda>.........
-000002e0: 0800 7a29 4162 7374 7261 6374 4469 616c  ..z)AbstractDial
-000002f0: 6f67 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63  og.__init__.<loc
-00000300: 616c 733e 2e3c 6c61 6d62 6461 3e63 0100  als>.<lambda>c..
-00000310: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00000320: 0000 1300 0000 720e 0000 0072 0f00 0000  ......r....r....
-00000330: 2901 da04 7368 6f77 7211 0000 0072 1300  )...showr....r..
-00000340: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00000350: 0012 0000 0072 1800 0000 7215 0000 0029  .....r....r....)
-00000360: 0c72 0200 0000 da0c 6163 7469 7665 5769  .r......activeWi
-00000370: 6e64 6f77 da09 6869 6465 4576 656e 74da  ndow..hideEvent.
-00000380: 0973 686f 7745 7665 6e74 7203 0000 00da  .showEventr.....
-00000390: 085f 5f69 6e69 745f 5fda 0573 7570 6572  .__init__..super
-000003a0: da06 7769 6e64 6f77 da12 696e 7374 616c  ..window..instal
-000003b0: 6c45 7665 6e74 4669 6c74 6572 da07 5f70  lEventFilter.._p
-000003c0: 6172 656e 74da 085f 7469 6d65 6f75 74da  arent.._timeout.
-000003d0: 0b5f 6175 746f 5f63 6c6f 7365 2905 7214  ._auto_close).r.
-000003e0: 0000 0072 0c00 0000 720d 0000 00da 066b  ...r....r......k
-000003f0: 7761 7267 7372 2100 0000 a901 da09 5f5f  wargsr!.......__
-00000400: 636c 6173 735f 5f72 1300 0000 7216 0000  class__r....r...
-00000410: 0072 1d00 0000 0a00 0000 7316 0000 0008  .r........s.....
-00000420: 0504 010e 010e 010c 0212 010e 020a 010c  ................
-00000430: 0106 020a 017a 1741 6273 7472 6163 7444  .....z.AbstractD
-00000440: 6961 6c6f 672e 5f5f 696e 6974 5f5f da06  ialog.__init__..
-00000450: 7265 7475 726e 6301 0000 0000 0000 0000  returnc.........
-00000460: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
-00000470: 0800 0000 7c00 a000 a100 5300 720f 0000  ....|.....S.r...
-00000480: 0029 01da 0670 6172 656e 7472 1300 0000  .)...parentr....
-00000490: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-000004a0: 2100 0000 1e00 0000 7302 0000 0008 027a  !.......s......z
-000004b0: 1641 6273 7472 6163 7444 6961 6c6f 672e  .AbstractDialog.
-000004c0: 5f70 6172 656e 74da 0165 6302 0000 0000  _parent..ec.....
-000004d0: 0000 0000 0000 0002 0000 0004 0000 0003  ................
-000004e0: 0000 0073 4600 0000 7c00 a000 a100 7308  ...sF...|.....s.
-000004f0: 7c00 a001 a100 7321 7c00 6a02 6400 7501  |.....s!|.j.d.u.
-00000500: 7215 7403 a004 7c00 6a02 7c00 6a05 a102  r.t...|.j.|.j...
-00000510: 0100 7406 8300 a007 7c01 a101 0100 7c00  ..t.....|.....|.
-00000520: a008 a100 0100 6400 5300 6400 5300 720f  ......d.S.d.S.r.
-00000530: 0000 0029 09da 0869 7348 6964 6465 6eda  ...)...isHidden.
-00000540: 0e69 7341 6374 6976 6557 696e 646f 7772  .isActiveWindowr
-00000550: 2200 0000 7207 0000 00da 0a73 696e 676c  "...r......singl
-00000560: 6553 686f 74da 0563 6c6f 7365 721e 0000  eShot..closer...
-00000570: 0072 1c00 0000 da0e 6163 7469 7661 7465  .r......activate
-00000580: 5769 6e64 6f77 2902 7214 0000 0072 2900  Window).r....r).
-00000590: 0000 7225 0000 0072 1500 0000 7216 0000  ..r%...r....r...
-000005a0: 0072 1c00 0000 2200 0000 730c 0000 0010  .r...."...s.....
-000005b0: 010a 0110 010c 020c 0104 fb7a 1841 6273  ...........z.Abs
-000005c0: 7472 6163 7444 6961 6c6f 672e 7368 6f77  tractDialog.show
-000005d0: 4576 656e 74da 0661 7267 5f5f 31da 0661  Event..arg__1..a
-000005e0: 7267 5f5f 3263 0300 0000 0000 0000 0000  rg__2c..........
-000005f0: 0000 0300 0000 0400 0000 0300 0000 7340  ..............s@
-00000600: 0000 007c 017c 00a0 00a1 0075 0072 197c  ...|.|.....u.r.|
-00000610: 006a 0172 197c 02a0 02a1 0074 036a 046a  .j.r.|.....t.j.j
-00000620: 0574 036a 046a 0666 0276 0072 197c 00a0  .t.j.j.f.v.r.|..
-00000630: 07a1 0001 0074 0883 00a0 097c 017c 02a1  .....t.....|.|..
-00000640: 0253 0072 0f00 0000 290a 721f 0000 0072  .S.r....).r....r
-00000650: 2300 0000 da04 7479 7065 7205 0000 00da  #.....typer.....
-00000660: 0454 7970 65da 1057 696e 646f 7744 6561  .Type..WindowDea
-00000670: 6374 6976 6174 65da 0448 6964 6572 2d00  ctivate..Hider-.
-00000680: 0000 721e 0000 00da 0b65 7665 6e74 4669  ..r......eventFi
-00000690: 6c74 6572 2903 7214 0000 0072 2f00 0000  lter).r....r/...
-000006a0: 7230 0000 0072 2500 0000 7215 0000 0072  r0...r%...r....r
-000006b0: 1600 0000 7235 0000 002a 0000 0073 0a00  ....r5...*...s..
-000006c0: 0000 0c01 0601 1801 0801 0e02 7a1a 4162  ............z.Ab
-000006d0: 7374 7261 6374 4469 616c 6f67 2e65 7665  stractDialog.eve
-000006e0: 6e74 4669 6c74 6572 2902 4e46 290f da08  ntFilter).NF)...
-000006f0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000700: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000710: 5f5f da05 666c 6f61 74da 0462 6f6f 6c72  __..float..boolr
-00000720: 1d00 0000 da08 7072 6f70 6572 7479 7204  ......propertyr.
-00000730: 0000 0072 2100 0000 7208 0000 0072 1c00  ...r!...r....r..
-00000740: 0000 7206 0000 0072 0500 0000 7235 0000  ..r....r....r5..
-00000750: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
-00000760: 7215 0000 0072 1500 0000 7225 0000 0072  r....r....r%...r
-00000770: 1600 0000 720b 0000 0009 0000 0073 1800  ....r........s..
-00000780: 0000 0800 0202 0201 04fe 0201 02ff 0202  ................
-00000790: 0efe 0214 1001 1603 2208 720b 0000 004e  ........".r....N
-000007a0: 290d da11 5079 5369 6465 362e 5174 5769  )...PySide6.QtWi
-000007b0: 6467 6574 7372 0200 0000 7203 0000 0072  dgetsr....r....r
-000007c0: 0400 0000 da0e 5079 5369 6465 362e 5174  ......PySide6.Qt
-000007d0: 436f 7265 7205 0000 0072 0600 0000 7207  Corer....r....r.
-000007e0: 0000 00da 0d50 7953 6964 6536 2e51 7447  .....PySide6.QtG
-000007f0: 7569 7208 0000 00da 075f 7769 6467 6574  uir......_widget
-00000800: 720a 0000 0072 0b00 0000 7215 0000 0072  r....r....r....r
-00000810: 1500 0000 7215 0000 0072 1600 0000 da08  ....r....r......
-00000820: 3c6d 6f64 756c 653e 0100 0000 730a 0000  <module>....s...
-00000830: 0014 0214 010c 010c 0116 03              ...........
+00000060: 6d0a 5a0a 0100 6404 6405 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
+00000070: 0100 4700 6406 6407 8400 6407 650c 6502  ..G.d.d...d.e.e.
+00000080: 8304 5a0d 6408 5300 2909 e900 0000 0029  ..Z.d.S.)......)
+00000090: 03da 0c51 4170 706c 6963 6174 696f 6eda  ...QApplication.
+000000a0: 0751 4469 616c 6f67 da07 5157 6964 6765  .QDialog..QWidge
+000000b0: 7429 03da 0651 4576 656e 74da 0751 4f62  t)...QEvent..QOb
+000000c0: 6a65 6374 da06 5154 696d 6572 2902 da0b  ject..QTimer)...
+000000d0: 5143 6c6f 7365 4576 656e 74da 0a51 5368  QCloseEvent..QSh
+000000e0: 6f77 4576 656e 74e9 0100 0000 2901 da0e  owEvent.....)...
+000000f0: 4162 7374 7261 6374 5769 6467 6574 6300  AbstractWidgetc.
+00000100: 0000 0000 0000 0000 0000 0000 0000 0006  ................
+00000110: 0000 0000 0000 0073 8400 0000 6500 5a01  .......s....e.Z.
+00000120: 6400 5a02 0901 0902 6413 6403 6503 6404  d.Z.....d.d.e.d.
+00000130: 6504 6604 8700 6601 6405 6406 840d 5a05  e.f...f.d.d...Z.
+00000140: 6506 6407 6507 6602 6408 6409 8404 8301  e.d.e.f.d.d.....
+00000150: 5a08 640a 6509 6407 6401 6604 8700 6601  Z.d.e.d.d.f...f.
+00000160: 640b 640c 840c 5a0a 640d 650b 6407 6401  d.d...Z.d.e.d.d.
+00000170: 6604 8700 6601 640e 640f 840c 5a0c 640d  f...f.d.d...Z.d.
+00000180: 650d 6410 650e 6407 6504 6606 8700 6601  e.d.e.d.e.f...f.
+00000190: 6411 6412 840c 5a0f 8700 0400 5a10 5300  d.d...Z.....Z.S.
+000001a0: 2914 da0e 4162 7374 7261 6374 4469 616c  )...AbstractDial
+000001b0: 6f67 4e46 da07 7469 6d65 6f75 74da 0a61  ogNF..timeout..a
+000001c0: 7574 6f5f 636c 6f73 6563 0300 0000 0000  uto_closec......
+000001d0: 0000 0000 0000 0500 0000 0400 0000 0b00  ................
+000001e0: 0000 735a 0000 0074 00a0 01a1 007d 0474  ..sZ...t.....}.t
+000001f0: 02a0 037c 007c 04a1 0201 0074 0483 006a  ...|.|.....t...j
+00000200: 0364 0169 007c 03a4 018e 0101 007c 00a0  .d.i.|.......|..
+00000210: 05a1 00a0 067c 00a1 0101 007c 006a 0764  .....|.....|.j.d
+00000220: 0075 0172 257c 006a 07a0 067c 00a1 0101  .u.r%|.j...|....
+00000230: 007c 017c 005f 087c 027c 005f 0964 0053  .|.|._.|.|._.d.S
+00000240: 0029 024e a900 290a 7202 0000 00da 0c61  .).N..).r......a
+00000250: 6374 6976 6557 696e 646f 7772 0300 0000  ctiveWindowr....
+00000260: da08 5f5f 696e 6974 5f5f da05 7375 7065  ..__init__..supe
+00000270: 72da 0677 696e 646f 77da 1269 6e73 7461  r..window..insta
+00000280: 6c6c 4576 656e 7446 696c 7465 72da 075f  llEventFilter.._
+00000290: 7061 7265 6e74 da08 5f74 696d 656f 7574  parent.._timeout
+000002a0: da0b 5f61 7574 6f5f 636c 6f73 6529 05da  .._auto_close)..
+000002b0: 0473 656c 6672 0d00 0000 720e 0000 00da  .selfr....r.....
+000002c0: 066b 7761 7267 7372 1500 0000 a901 da09  .kwargsr........
+000002d0: 5f5f 636c 6173 735f 5f72 0f00 0000 fa4e  __class__r.....N
+000002e0: 2f68 6f6d 652f 6f73 616d 612f 576f 726b  /home/osama/Work
+000002f0: 7370 6163 652f 2e76 656e 762f 6c69 622f  space/.venv/lib/
+00000300: 7079 7468 6f6e 332e 3130 2f73 6974 652d  python3.10/site-
+00000310: 7061 636b 6167 6573 2f51 7469 6361 2f63  packages/Qtica/c
+00000320: 6f72 652f 5f64 6961 6c6f 672e 7079 7211  ore/_dialog.pyr.
+00000330: 0000 000a 0000 0073 1000 0000 0805 0c05  .......s........
+00000340: 1201 0e02 0a01 0c01 0602 0a01 7a17 4162  ............z.Ab
+00000350: 7374 7261 6374 4469 616c 6f67 2e5f 5f69  stractDialog.__i
+00000360: 6e69 745f 5fda 0672 6574 7572 6e63 0100  nit__..returnc..
+00000370: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00000380: 0000 4300 0000 7308 0000 007c 00a0 00a1  ..C...s....|....
+00000390: 0053 00a9 014e 2901 da06 7061 7265 6e74  .S...N)...parent
+000003a0: 2901 7218 0000 0072 0f00 0000 720f 0000  ).r....r....r...
+000003b0: 0072 1c00 0000 7215 0000 001e 0000 0073  .r....r........s
+000003c0: 0200 0000 0802 7a16 4162 7374 7261 6374  ......z.Abstract
+000003d0: 4469 616c 6f67 2e5f 7061 7265 6e74 da01  Dialog._parent..
+000003e0: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
+000003f0: 0000 0400 0000 0300 0000 7346 0000 007c  ..........sF...|
+00000400: 00a0 00a1 0073 087c 00a0 01a1 0073 217c  .....s.|.....s!|
+00000410: 006a 0264 0075 0172 1574 03a0 047c 006a  .j.d.u.r.t...|.j
+00000420: 027c 006a 05a1 0201 0074 0683 00a0 077c  .|.j.....t.....|
+00000430: 01a1 0101 007c 00a0 08a1 0001 0064 0053  .....|.......d.S
+00000440: 0064 0053 0072 1e00 0000 2909 da08 6973  .d.S.r....)...is
+00000450: 4869 6464 656e da0e 6973 4163 7469 7665  Hidden..isActive
+00000460: 5769 6e64 6f77 7216 0000 0072 0700 0000  Windowr....r....
+00000470: da0a 7369 6e67 6c65 5368 6f74 da05 636c  ..singleShot..cl
+00000480: 6f73 6572 1200 0000 da09 7368 6f77 4576  oser......showEv
+00000490: 656e 74da 0e61 6374 6976 6174 6557 696e  ent..activateWin
+000004a0: 646f 7729 0272 1800 0000 7220 0000 0072  dow).r....r ...r
+000004b0: 1a00 0000 720f 0000 0072 1c00 0000 7225  ....r....r....r%
+000004c0: 0000 0022 0000 0073 0c00 0000 1001 0a01  ..."...s........
+000004d0: 1001 0c02 0c01 04fb 7a18 4162 7374 7261  ........z.Abstra
+000004e0: 6374 4469 616c 6f67 2e73 686f 7745 7665  ctDialog.showEve
+000004f0: 6e74 da06 6172 675f 5f31 6302 0000 0000  nt..arg__1c.....
+00000500: 0000 0000 0000 0002 0000 0003 0000 0003  ................
+00000510: 0000 0073 1400 0000 7c00 a000 a100 0100  ...s....|.......
+00000520: 7401 8300 a002 7c01 a101 5300 721e 0000  t.....|...S.r...
+00000530: 0029 03da 0b64 656c 6574 654c 6174 6572  .)...deleteLater
+00000540: 7212 0000 00da 0a63 6c6f 7365 4576 656e  r......closeEven
+00000550: 7429 0272 1800 0000 7227 0000 0072 1a00  t).r....r'...r..
+00000560: 0000 720f 0000 0072 1c00 0000 7229 0000  ..r....r....r)..
+00000570: 002a 0000 0073 0400 0000 0801 0c01 7a19  .*...s........z.
+00000580: 4162 7374 7261 6374 4469 616c 6f67 2e63  AbstractDialog.c
+00000590: 6c6f 7365 4576 656e 74da 0661 7267 5f5f  loseEvent..arg__
+000005a0: 3263 0300 0000 0000 0000 0000 0000 0300  2c..............
+000005b0: 0000 0400 0000 0300 0000 7340 0000 007c  ..........s@...|
+000005c0: 017c 00a0 00a1 0075 0072 197c 006a 0172  .|.....u.r.|.j.r
+000005d0: 197c 02a0 02a1 0074 036a 046a 0574 036a  .|.....t.j.j.t.j
+000005e0: 046a 0666 0276 0072 197c 00a0 07a1 0001  .j.f.v.r.|......
+000005f0: 0074 0883 00a0 097c 017c 02a1 0253 0072  .t.....|.|...S.r
+00000600: 1e00 0000 290a 7213 0000 0072 1700 0000  ....).r....r....
+00000610: da04 7479 7065 7205 0000 00da 0454 7970  ..typer......Typ
+00000620: 65da 1057 696e 646f 7744 6561 6374 6976  e..WindowDeactiv
+00000630: 6174 65da 0448 6964 6572 2400 0000 7212  ate..Hider$...r.
+00000640: 0000 00da 0b65 7665 6e74 4669 6c74 6572  .....eventFilter
+00000650: 2903 7218 0000 0072 2700 0000 722a 0000  ).r....r'...r*..
+00000660: 0072 1a00 0000 720f 0000 0072 1c00 0000  .r....r....r....
+00000670: 722f 0000 002e 0000 0073 0a00 0000 0c01  r/.......s......
+00000680: 0601 1801 0801 0e02 7a1a 4162 7374 7261  ........z.Abstra
+00000690: 6374 4469 616c 6f67 2e65 7665 6e74 4669  ctDialog.eventFi
+000006a0: 6c74 6572 2902 4e46 2911 da08 5f5f 6e61  lter).NF)...__na
+000006b0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+000006c0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da05  ..__qualname__..
+000006d0: 666c 6f61 74da 0462 6f6f 6c72 1100 0000  float..boolr....
+000006e0: da08 7072 6f70 6572 7479 7204 0000 0072  ..propertyr....r
+000006f0: 1500 0000 7209 0000 0072 2500 0000 7208  ....r....r%...r.
+00000700: 0000 0072 2900 0000 7206 0000 0072 0500  ...r)...r....r..
+00000710: 0000 722f 0000 00da 0d5f 5f63 6c61 7373  ..r/.....__class
+00000720: 6365 6c6c 5f5f 720f 0000 0072 0f00 0000  cell__r....r....
+00000730: 721a 0000 0072 1c00 0000 720c 0000 0009  r....r....r.....
+00000740: 0000 0073 1a00 0000 0800 0202 0201 04fe  ...s............
+00000750: 0201 02ff 0202 0efe 0214 1001 1603 1608  ................
+00000760: 2204 720c 0000 004e 290e da11 5079 5369  ".r....N)...PySi
+00000770: 6465 362e 5174 5769 6467 6574 7372 0200  de6.QtWidgetsr..
+00000780: 0000 7203 0000 0072 0400 0000 da0e 5079  ..r....r......Py
+00000790: 5369 6465 362e 5174 436f 7265 7205 0000  Side6.QtCorer...
+000007a0: 0072 0600 0000 7207 0000 00da 0d50 7953  .r....r......PyS
+000007b0: 6964 6536 2e51 7447 7569 7208 0000 0072  ide6.QtGuir....r
+000007c0: 0900 0000 da07 5f77 6964 6765 7472 0b00  ......_widgetr..
+000007d0: 0000 720c 0000 0072 0f00 0000 720f 0000  ..r....r....r...
+000007e0: 0072 0f00 0000 721c 0000 00da 083c 6d6f  .r....r......<mo
+000007f0: 6475 6c65 3e01 0000 0073 0a00 0000 1402  dule>....s......
+00000800: 1401 1001 0c01 1603                      ........
```

### Comparing `qtica-0.4.3/Qtica/core/__pycache__/_icons.cpython-310.pyc` & `qtica-0.5.0/Qtica/core/__pycache__/_icons.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/core/__pycache__/_painter.cpython-310.pyc` & `qtica-0.5.0/Qtica/core/__pycache__/_painter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/core/__pycache__/_qobject.cpython-310.pyc` & `qtica-0.5.0/Qtica/core/__pycache__/_qobject.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/core/__pycache__/_tool.cpython-310.pyc` & `qtica-0.5.0/Qtica/core/__pycache__/_tool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/core/__pycache__/api.cpython-310.pyc` & `qtica-0.5.0/Qtica/core/__pycache__/api.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/core/__pycache__/exception_handler.cpython-310.pyc` & `qtica-0.5.0/Qtica/core/__pycache__/exception_handler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/core/__pycache__/qstyle_sheet.cpython-310.pyc` & `qtica-0.5.0/Qtica/core/__pycache__/qstyle_sheet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/core/__pycache__/routes.cpython-310.pyc` & `qtica-0.5.0/Qtica/core/__pycache__/routes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/core/_base.py` & `qtica-0.5.0/Qtica/core/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,15 @@
     def _handle_add_methods(self, name: str, value: Any) -> None:
         if (func := self._getattr(name)) is not None and callable(func):
             if isinstance(value, MArgs):
                 for v in value.args():
                     if isinstance(v, Args):
                         func(*v.args(), **v.kwargs())
                     else:
-                        func(value)
+                        func(v)
             elif isinstance(value, Args):
                 func(*value.args(), **value.kwargs())
             else:
                 func(value)
 
     def __setattr__(self, __name: str, __value: Any) -> None:
         if hasattr(self, "_enable_event_stack") and self._enable_event_stack:
```

### Comparing `qtica-0.4.3/Qtica/core/_config.py` & `qtica-0.5.0/Qtica/core/_config.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/core/_declarative.py` & `qtica-0.5.0/Qtica/core/_declarative.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/core/_dialog.py` & `qtica-0.5.0/Qtica/core/_dialog.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/python3
 
 from PySide6.QtWidgets import QApplication, QDialog, QWidget
 from PySide6.QtCore import QEvent, QObject, QTimer
-from PySide6.QtGui import QShowEvent
+from PySide6.QtGui import QCloseEvent, QShowEvent
 from ._widget import AbstractWidget
 
 
 class AbstractDialog(AbstractWidget, QDialog):
     def __init__(self,
                  timeout: float = None,
                  auto_close: bool = False,
                  **kwargs):
 
         _parent = QApplication.activeWindow()
-        if not auto_close:
-            _parent.hideEvent = lambda _: self.hide()
-            _parent.showEvent = lambda _: self.show()
+        # if not auto_close:
+        #     _parent.hideEvent = lambda _: self.hide()
+        #     _parent.showEvent = lambda _: self.show()
 
         QDialog.__init__(self, _parent)
         super().__init__(**kwargs)
 
         self.window().installEventFilter(self)
         if self._parent is not None:
             self._parent.installEventFilter(self)
@@ -35,14 +35,18 @@
         if self.isHidden() or not self.isActiveWindow():
             if self._timeout is not None:
                 QTimer.singleShot(self._timeout, self.close)
 
             super().showEvent(e)
             self.activateWindow()
 
+    def closeEvent(self, arg__1: QCloseEvent) -> None:
+        self.deleteLater()
+        return super().closeEvent(arg__1)
+
     def eventFilter(self, arg__1: QObject, arg__2: QEvent) -> bool:
         if arg__1 is self.window():
             if (self._auto_close
                 and arg__2.type() in (QEvent.Type.WindowDeactivate, QEvent.Type.Hide)):
                 self.close()
 
         return super().eventFilter(arg__1, arg__2)
```

### Comparing `qtica-0.4.3/Qtica/core/_icons.py` & `qtica-0.5.0/Qtica/core/_icons.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/core/_painter.py` & `qtica-0.5.0/Qtica/core/_painter.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/core/_tool.py` & `qtica-0.5.0/Qtica/core/_tool.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/core/api.py` & `qtica-0.5.0/Qtica/core/api.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/core/exception_handler.py` & `qtica-0.5.0/Qtica/core/exception_handler.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/core/qstyle_sheet.py` & `qtica-0.5.0/Qtica/core/qstyle_sheet.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/core/routes.py` & `qtica-0.5.0/Qtica/core/routes.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/effects/__pycache__/_effects.cpython-310.pyc` & `qtica-0.5.0/Qtica/effects/__pycache__/_effects.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/effects/__pycache__/blur.cpython-310.pyc` & `qtica-0.5.0/Qtica/effects/__pycache__/blur.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/effects/__pycache__/blur.cpython-312.pyc` & `qtica-0.5.0/Qtica/effects/__pycache__/blur.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/effects/__pycache__/colorize.cpython-310.pyc` & `qtica-0.5.0/Qtica/effects/__pycache__/colorize.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/effects/__pycache__/colorize.cpython-312.pyc` & `qtica-0.5.0/Qtica/effects/__pycache__/colorize.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/effects/__pycache__/drop_shadow.cpython-310.pyc` & `qtica-0.5.0/Qtica/effects/__pycache__/drop_shadow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/effects/__pycache__/drop_shadow.cpython-312.pyc` & `qtica-0.5.0/Qtica/effects/__pycache__/drop_shadow.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/effects/__pycache__/neumorphism.cpython-310.pyc` & `qtica-0.5.0/Qtica/effects/__pycache__/neumorphism.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/effects/__pycache__/opacity.cpython-310.pyc` & `qtica-0.5.0/Qtica/effects/__pycache__/opacity.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/effects/__pycache__/opacity.cpython-312.pyc` & `qtica-0.5.0/Qtica/effects/__pycache__/opacity.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/effects/_effects.py` & `qtica-0.5.0/Qtica/effects/_effects.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/__pycache__/__init__.cpython-310.pyc` & `qtica-0.5.0/Qtica/enums/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/__pycache__/__init__.cpython-312.pyc` & `qtica-0.5.0/Qtica/enums/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/__pycache__/_abs_icons.cpython-310.pyc` & `qtica-0.5.0/Qtica/enums/__pycache__/_abs_icons.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/__pycache__/colors.cpython-310.pyc` & `qtica-0.5.0/Qtica/enums/__pycache__/colors.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/__pycache__/colors.cpython-312.pyc` & `qtica-0.5.0/Qtica/enums/__pycache__/colors.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/__pycache__/env_vars.cpython-310.pyc` & `qtica-0.5.0/Qtica/enums/__pycache__/env_vars.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/__pycache__/env_vars.cpython-312.pyc` & `qtica-0.5.0/Qtica/enums/__pycache__/env_vars.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/__pycache__/events.cpython-310.pyc` & `qtica-0.5.0/Qtica/enums/__pycache__/events.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/__pycache__/events.cpython-312.pyc` & `qtica-0.5.0/Qtica/enums/__pycache__/events.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/__pycache__/position.cpython-312.pyc` & `qtica-0.5.0/Qtica/enums/__pycache__/position.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/__pycache__/qpa_plugins.cpython-310.pyc` & `qtica-0.5.0/Qtica/enums/__pycache__/qpa_plugins.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Oct 20 20:59:31 2023 UTC, .py size: 457 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,57 @@
-00000000: 6f0d 0d0a 0000 0000 33ea 3265 c901 0000  o.......3.2e....
+00000000: 6f0d 0d0a 0000 0000 1cb4 e865 2c02 0000  o..........e,...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 8303 5a02 6404 5300 2905  ..d.e...Z.d.S.).
 00000050: e900 0000 0029 01da 0445 6e75 6d63 0000  .....)...Enumc..
 00000060: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00000070: 0000 4000 0000 73c2 0000 0065 005a 0164  ..@...s....e.Z.d
+00000070: 0000 4000 0000 73e6 0000 0065 005a 0164  ..@...s....e.Z.d
 00000080: 005a 0255 0064 015a 0365 0465 0564 013c  .Z.U.d.Z.e.e.d.<
 00000090: 0064 025a 0665 0465 0564 023c 0064 035a  .d.Z.e.e.d.<.d.Z
 000000a0: 0765 0465 0564 033c 0064 045a 0865 0465  .e.e.d.<.d.Z.e.e
 000000b0: 0564 043c 0064 055a 0965 0465 0564 053c  .d.<.d.Z.e.e.d.<
 000000c0: 0064 065a 0a65 0465 0564 063c 0064 075a  .d.Z.e.e.d.<.d.Z
 000000d0: 0b65 0465 0564 073c 0064 085a 0c65 0465  .e.e.d.<.d.Z.e.e
 000000e0: 0564 083c 0064 095a 0d65 0465 0564 093c  .d.<.d.Z.e.e.d.<
 000000f0: 0064 0a5a 0e65 0465 0564 0a3c 0064 0b5a  .d.Z.e.e.d.<.d.Z
 00000100: 0f65 0465 0564 0b3c 0064 0c5a 1065 0465  .e.e.d.<.d.Z.e.e
 00000110: 0564 0c3c 0064 0d5a 1165 0465 0564 0d3c  .d.<.d.Z.e.e.d.<
 00000120: 0064 0e5a 1265 0465 0564 0e3c 0064 0f5a  .d.Z.e.e.d.<.d.Z
-00000130: 1365 0465 0564 0f3c 0064 1053 0029 11da  .e.e.d.<.d.S.)..
-00000140: 0d51 5041 5f50 6c61 7466 6f72 6d73 da07  .QPA_Platforms..
-00000150: 616e 6472 6f69 64da 0563 6f63 6f61 da08  android..cocoa..
-00000160: 6469 7265 6374 6662 da05 6567 6c66 73da  directfb..eglfs.
-00000170: 0369 6f73 da03 6b6d 73da 076c 696e 7578  .ios..kms..linux
-00000180: 6662 da07 6d69 6e69 6d61 6cda 0a6d 696e  fb..minimal..min
-00000190: 696d 616c 6567 6cda 096f 6666 7363 7265  imalegl..offscre
-000001a0: 656e da07 6f70 656e 7766 64da 0371 6e78  en..openwfd..qnx
-000001b0: da07 7769 6e64 6f77 73da 0777 6179 6c61  ..windows..wayla
-000001c0: 6e64 da03 7863 624e 2914 da08 5f5f 6e61  nd..xcbN)...__na
-000001d0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-000001e0: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7204  ..__qualname__r.
-000001f0: 0000 00da 0373 7472 da0f 5f5f 616e 6e6f  .....str..__anno
-00000200: 7461 7469 6f6e 735f 5f72 0500 0000 7206  tations__r....r.
-00000210: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
-00000220: 0000 720a 0000 0072 0b00 0000 720c 0000  ..r....r....r...
-00000230: 0072 0d00 0000 720e 0000 0072 0f00 0000  .r....r....r....
-00000240: 7210 0000 0072 1100 0000 7212 0000 00a9  r....r....r.....
-00000250: 0072 1800 0000 7218 0000 00fa 542f 686f  .r....r.....T/ho
-00000260: 6d65 2f6f 7361 6d61 2f57 6f72 6b73 7061  me/osama/Workspa
-00000270: 6365 2f2e 7665 6e76 2f6c 6962 2f70 7974  ce/.venv/lib/pyt
-00000280: 686f 6e33 2e31 302f 7369 7465 2d70 6163  hon3.10/site-pac
-00000290: 6b61 6765 732f 6d69 6661 7374 2f65 6e75  kages/mifast/enu
-000002a0: 6d73 2f71 7061 5f70 6c75 6769 6e73 2e70  ms/qpa_plugins.p
-000002b0: 7972 0300 0000 0400 0000 7320 0000 000a  yr........s ....
-000002c0: 000c 010c 010c 010c 010c 010c 010c 010c  ................
-000002d0: 010c 010c 010c 010c 010c 010c 0110 0172  ...............r
-000002e0: 0300 0000 4e29 03da 0465 6e75 6d72 0200  ....N)...enumr..
-000002f0: 0000 7203 0000 0072 1800 0000 7218 0000  ..r....r....r...
-00000300: 0072 1800 0000 7219 0000 00da 083c 6d6f  .r....r......<mo
-00000310: 6475 6c65 3e01 0000 0073 0400 0000 0c00  dule>....s......
-00000320: 1403                                     ..
+00000130: 1365 0465 0564 0f3c 0064 105a 1465 0465  .e.e.d.<.d.Z.e.e
+00000140: 0564 103c 0064 115a 1565 0465 0564 123c  .d.<.d.Z.e.e.d.<
+00000150: 0064 135a 1665 0465 0564 133c 0064 1453  .d.Z.e.e.d.<.d.S
+00000160: 0029 15da 0d51 5041 5f50 6c61 7466 6f72  .)...QPA_Platfor
+00000170: 6d73 da07 616e 6472 6f69 64da 0563 6f63  ms..android..coc
+00000180: 6f61 da08 6469 7265 6374 6662 da05 6567  oa..directfb..eg
+00000190: 6c66 73da 0369 6f73 da03 6b6d 73da 076c  lfs..ios..kms..l
+000001a0: 696e 7578 6662 da07 6d69 6e69 6d61 6cda  inuxfb..minimal.
+000001b0: 0a6d 696e 696d 616c 6567 6cda 096f 6666  .minimalegl..off
+000001c0: 7363 7265 656e da07 6f70 656e 7766 64da  screen..openwfd.
+000001d0: 0371 6e78 da07 7769 6e64 6f77 73da 0777  .qnx..windows..w
+000001e0: 6179 6c61 6e64 da03 7863 62da 0376 6e63  ayland..xcb..vnc
+000001f0: 7a0b 7761 796c 616e 642d 6567 6cda 0b77  z.wayland-egl..w
+00000200: 6179 6c61 6e64 5f65 676c da0c 766b 6b68  ayland_egl..vkkh
+00000210: 7264 6973 706c 6179 4e29 17da 085f 5f6e  rdisplayN)...__n
+00000220: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000230: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
+00000240: 0400 0000 da03 7374 72da 0f5f 5f61 6e6e  ......str..__ann
+00000250: 6f74 6174 696f 6e73 5f5f 7205 0000 0072  otations__r....r
+00000260: 0600 0000 7207 0000 0072 0800 0000 7209  ....r....r....r.
+00000270: 0000 0072 0a00 0000 720b 0000 0072 0c00  ...r....r....r..
+00000280: 0000 720d 0000 0072 0e00 0000 720f 0000  ..r....r....r...
+00000290: 0072 1000 0000 7211 0000 0072 1200 0000  .r....r....r....
+000002a0: 7213 0000 0072 1400 0000 7215 0000 00a9  r....r....r.....
+000002b0: 0072 1b00 0000 721b 0000 00fa 532f 686f  .r....r.....S/ho
+000002c0: 6d65 2f6f 7361 6d61 2f57 6f72 6b73 7061  me/osama/Workspa
+000002d0: 6365 2f2e 7665 6e76 2f6c 6962 2f70 7974  ce/.venv/lib/pyt
+000002e0: 686f 6e33 2e31 302f 7369 7465 2d70 6163  hon3.10/site-pac
+000002f0: 6b61 6765 732f 5174 6963 612f 656e 756d  kages/Qtica/enum
+00000300: 732f 7170 615f 706c 7567 696e 732e 7079  s/qpa_plugins.py
+00000310: 7203 0000 0004 0000 0073 2600 0000 0a00  r........s&.....
+00000320: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00000330: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00000340: 0c01 1001 7203 0000 004e 2903 da04 656e  ....r....N)...en
+00000350: 756d 7202 0000 0072 0300 0000 721b 0000  umr....r....r...
+00000360: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
+00000370: da08 3c6d 6f64 756c 653e 0100 0000 7304  ..<module>....s.
+00000380: 0000 000c 0014 03                        .......
```

### Comparing `qtica-0.4.3/Qtica/enums/__pycache__/qpa_plugins.cpython-312.pyc` & `qtica-0.5.0/Qtica/enums/__pycache__/qpa_plugins.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/__pycache__/signals.cpython-310.pyc` & `qtica-0.5.0/Qtica/enums/__pycache__/signals.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/__pycache__/signals.cpython-312.pyc` & `qtica-0.5.0/Qtica/enums/__pycache__/signals.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/__pycache__/size.cpython-312.pyc` & `qtica-0.5.0/Qtica/enums/__pycache__/size.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/__pycache__/teaching_tip_tails.cpython-310.pyc` & `qtica-0.5.0/Qtica/enums/__pycache__/teaching_tip_tails.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/__pycache__/widgets.cpython-310.pyc` & `qtica-0.5.0/Qtica/enums/__pycache__/widgets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/__pycache__/widgets.cpython-312.pyc` & `qtica-0.5.0/Qtica/enums/__pycache__/widgets.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/colors.py` & `qtica-0.5.0/Qtica/enums/colors.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/env_vars.py` & `qtica-0.5.0/Qtica/enums/env_vars.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/events.py` & `qtica-0.5.0/Qtica/enums/events.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/signals.py` & `qtica-0.5.0/Qtica/enums/signals.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/enums/widgets.py` & `qtica-0.5.0/Qtica/enums/widgets.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/layouts/__pycache__/__init__.cpython-310.pyc` & `qtica-0.5.0/Qtica/layouts/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/layouts/__pycache__/__init__.cpython-312.pyc` & `qtica-0.5.0/Qtica/layouts/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/layouts/__pycache__/border_layout.cpython-310.pyc` & `qtica-0.5.0/Qtica/layouts/__pycache__/border_layout.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/layouts/__pycache__/border_layout.cpython-312.pyc` & `qtica-0.5.0/Qtica/layouts/__pycache__/border_layout.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/layouts/__pycache__/expand_layout.cpython-310.pyc` & `qtica-0.5.0/Qtica/layouts/__pycache__/expand_layout.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/layouts/__pycache__/flow_layout.cpython-310.pyc` & `qtica-0.5.0/Qtica/layouts/__pycache__/flow_layout.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/layouts/__pycache__/flow_layout.cpython-312.pyc` & `qtica-0.5.0/Qtica/layouts/__pycache__/flow_layout.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/layouts/__pycache__/form_layout.cpython-310.pyc` & `qtica-0.5.0/Qtica/layouts/__pycache__/form_layout.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/layouts/__pycache__/form_layout.cpython-312.pyc` & `qtica-0.5.0/Qtica/layouts/__pycache__/form_layout.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/layouts/__pycache__/grid_layout.cpython-310.pyc` & `qtica-0.5.0/Qtica/layouts/__pycache__/grid_layout.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/layouts/__pycache__/grid_layout.cpython-312.pyc` & `qtica-0.5.0/Qtica/layouts/__pycache__/grid_layout.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/layouts/__pycache__/h_layout.cpython-312.pyc` & `qtica-0.5.0/Qtica/layouts/__pycache__/h_layout.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/layouts/__pycache__/stacked.cpython-310.pyc` & `qtica-0.5.0/Qtica/layouts/__pycache__/stacked.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jan 26 21:59:36 2024 UTC, .py size: 1057 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,84 @@
-00000000: 6f0d 0d0a 0000 0000 482b b465 2104 0000  o.......H+.e!...
+00000000: 6f0d 0d0a 0000 0000 dcc0 e765 9a05 0000  o..........e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
+00000020: 0005 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6403  m.Z.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6403 6405 6c08  d.l.m.Z...d.d.l.
-00000060: 6d09 5a09 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
-00000070: 6509 6503 8304 5a0a 6408 5300 2909 e900  e.e...Z.d.S.)...
-00000080: 0000 0029 01da 0555 6e69 6f6e 2903 da0e  ...)...Union)...
-00000090: 5153 7461 636b 6564 4c61 796f 7574 da07  QStackedLayout..
-000000a0: 5157 6964 6765 74da 0b51 4c61 796f 7574  QWidget..QLayout
-000000b0: 4974 656d e902 0000 0029 01da 0941 6c69  Item.....)...Ali
-000000c0: 676e 6d65 6e74 2901 da0f 4162 7374 7261  gnment)...Abstra
-000000d0: 6374 514f 626a 6563 7463 0000 0000 0000  ctQObjectc......
-000000e0: 0000 0000 0000 0000 0000 0700 0000 0000  ................
-000000f0: 0000 7336 0000 0065 005a 0164 005a 0264  ..s6...e.Z.d.Z.d
-00000100: 0164 029c 0164 0365 0365 0465 0565 0665  .d...d.e.e.e.e.e
-00000110: 0766 0319 0019 0066 0287 0066 0164 0464  .f.....f...f.d.d
-00000120: 0584 0e5a 0887 0004 005a 0953 0029 06da  ...Z.....Z.S.)..
-00000130: 0d53 7461 636b 6564 4c61 796f 7574 4e29  .StackedLayoutN)
-00000140: 01da 0863 6869 6c64 7265 6e72 0a00 0000  ...childrenr....
-00000150: 6301 0000 0000 0000 0001 0000 0006 0000  c...............
-00000160: 0005 0000 000b 0000 0073 a600 0000 7400  .........s....t.
-00000170: a001 7c00 a101 0100 7402 8300 6a01 6401  ..|.....t...j.d.
-00000180: 6900 7c02 a401 8e01 0100 7c01 7312 6400  i.|.......|.s.d.
-00000190: 5300 7c01 4400 5d3c 7d03 7403 7c03 7404  S.|.D.]<}.t.|.t.
-000001a0: 8302 723b 7c03 6a05 7d04 7403 7c04 7406  ..r;|.j.}.t.|.t.
-000001b0: 8302 7227 7c00 6a07 7d05 6e08 7403 7c04  ..r'|.j.}.n.t.|.
-000001c0: 7408 8302 722f 7c00 6a09 7d05 7c05 7c04  t...r/|.j.}.|.|.
-000001d0: 8301 0100 7c00 a00a 7c04 7c03 6a0b a102  ....|...|.|.j...
-000001e0: 0100 7114 7403 7c03 7408 8302 7246 7c00  ..q.t.|.t...rF|.
-000001f0: a009 7c03 a101 0100 7114 7403 7c03 7406  ..|.....q.t.|.t.
-00000200: 8302 7250 7c00 a007 7c03 a101 0100 7114  ..rP|...|.....q.
-00000210: 6400 5300 2902 4ea9 0029 0c72 0300 0000  d.S.).N..).r....
-00000220: da08 5f5f 696e 6974 5f5f da05 7375 7065  ..__init__..supe
-00000230: 72da 0a69 7369 6e73 7461 6e63 6572 0700  r..isinstancer..
-00000240: 0000 da05 6368 696c 6472 0400 0000 da09  ....childr......
-00000250: 6164 6457 6964 6765 7472 0500 0000 da07  addWidgetr......
-00000260: 6164 6449 7465 6dda 0c73 6574 416c 6967  addItem..setAlig
-00000270: 6e6d 656e 74da 0961 6c69 676e 6d65 6e74  nment..alignment
-00000280: 2906 da04 7365 6c66 720a 0000 00da 066b  )...selfr......k
-00000290: 7761 7267 7372 0f00 0000 da07 5f77 6964  wargsr......_wid
-000002a0: 6765 74da 055f 6675 6e63 a901 da09 5f5f  get.._func....__
-000002b0: 636c 6173 735f 5f72 0b00 0000 fa51 2f68  class__r.....Q/h
-000002c0: 6f6d 652f 6f73 616d 612f 576f 726b 7370  ome/osama/Worksp
-000002d0: 6163 652f 2e76 656e 762f 6c69 622f 7079  ace/.venv/lib/py
-000002e0: 7468 6f6e 332e 3130 2f73 6974 652d 7061  thon3.10/site-pa
-000002f0: 636b 6167 6573 2f51 7469 6361 2f6c 6179  ckages/Qtica/lay
-00000300: 6f75 7473 2f73 7461 636b 6564 2e70 7972  outs/stacked.pyr
-00000310: 0c00 0000 0800 0000 7326 0000 000a 0412  ........s&......
-00000320: 0104 0204 0108 020a 0106 010a 0208 010a  ................
-00000330: 0106 0108 0210 010a 020c 010a 020a 0102  ................
-00000340: 8004 f07a 1653 7461 636b 6564 4c61 796f  ...z.StackedLayo
-00000350: 7574 2e5f 5f69 6e69 745f 5f29 0ada 085f  ut.__init__)..._
-00000360: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000370: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000380: 5fda 046c 6973 7472 0200 0000 7204 0000  _..listr....r...
-00000390: 0072 0500 0000 7207 0000 0072 0c00 0000  .r....r....r....
-000003a0: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
-000003b0: 0b00 0000 720b 0000 0072 1800 0000 721a  ....r....r....r.
-000003c0: 0000 0072 0900 0000 0700 0000 730a 0000  ...r........s...
-000003d0: 0008 0002 0306 fe10 0216 fe72 0900 0000  ...........r....
-000003e0: 4e29 0bda 0674 7970 696e 6772 0200 0000  N)...typingr....
-000003f0: da11 5079 5369 6465 362e 5174 5769 6467  ..PySide6.QtWidg
-00000400: 6574 7372 0300 0000 7204 0000 0072 0500  etsr....r....r..
-00000410: 0000 da0f 7574 696c 732e 616c 6967 6e6d  ....utils.alignm
-00000420: 656e 7472 0700 0000 da04 636f 7265 7208  entr......corer.
-00000430: 0000 0072 0900 0000 720b 0000 0072 0b00  ...r....r....r..
-00000440: 0000 720b 0000 0072 1a00 0000 da08 3c6d  ..r....r......<m
-00000450: 6f64 756c 653e 0100 0000 730a 0000 000c  odule>....s.....
-00000460: 0014 010c 010c 0116 03                   .........
+00000060: 6d09 5a09 6d0a 5a0a 0100 4700 6406 6407  m.Z.m.Z...G.d.d.
+00000070: 8400 6407 6509 6503 8304 5a0b 6408 5300  ..d.e.e...Z.d.S.
+00000080: 2909 e900 0000 0029 01da 0555 6e69 6f6e  )......)...Union
+00000090: 2903 da0e 5153 7461 636b 6564 4c61 796f  )...QStackedLayo
+000000a0: 7574 da07 5157 6964 6765 74da 0b51 4c61  ut..QWidget..QLa
+000000b0: 796f 7574 4974 656d e902 0000 0029 01da  youtItem.....)..
+000000c0: 0941 6c69 676e 6d65 6e74 2902 da0f 4162  .Alignment)...Ab
+000000d0: 7374 7261 6374 514f 626a 6563 74da 0652  stractQObject..R
+000000e0: 6f75 7465 7363 0000 0000 0000 0000 0000  outesc..........
+000000f0: 0000 0000 0000 0800 0000 0000 0000 7340  ..............s@
+00000100: 0000 0065 005a 0164 005a 0264 0164 029c  ...e.Z.d.Z.d.d..
+00000110: 0164 0365 0365 0465 0365 0565 0665 0766  .d.e.e.e.e.e.e.f
+00000120: 0319 0019 0065 0865 0966 0319 0066 0287  .....e.e.f...f..
+00000130: 0066 0164 0464 0584 0e5a 0a87 0004 005a  .f.d.d...Z.....Z
+00000140: 0b53 0029 06da 0d53 7461 636b 6564 4c61  .S.)...StackedLa
+00000150: 796f 7574 4e29 01da 0863 6869 6c64 7265  youtN)...childre
+00000160: 6e72 0b00 0000 6301 0000 0000 0000 0001  nr....c.........
+00000170: 0000 0007 0000 0005 0000 000b 0000 0073  ...............s
+00000180: 0201 0000 7400 a001 7c00 a101 0100 7402  ....t...|.....t.
+00000190: 8300 6a01 6402 6900 7c02 a401 8e01 0100  ..j.d.i.|.......
+000001a0: 7c01 7312 6400 5300 7403 7c01 7404 7405  |.s.d.S.t.|.t.t.
+000001b0: 6602 8302 7240 7403 7c01 7405 8302 7225  f...r@t.|.t...r%
+000001c0: 7404 6403 6900 7c01 a401 8e01 6e01 7c01  t.d.i.|.....n.|.
+000001d0: 7c00 5f06 7c00 6a06 a007 7c00 a101 0100  |._.|.j...|.....
+000001e0: 7c01 a008 a100 4400 5d0b 5c02 7d03 7d04  |.....D.].\.}.}.
+000001f0: 7c00 6a06 a009 7c03 7c04 a102 0100 7132  |.j...|.|.....q2
+00000200: 6400 5300 7c01 4400 5d3c 7d04 7403 7c04  d.S.|.D.]<}.t.|.
+00000210: 740a 8302 7269 7c04 6a0b 7d05 7403 7c05  t...ri|.j.}.t.|.
+00000220: 740c 8302 7255 7c00 6a0d 7d06 6e08 7403  t...rU|.j.}.n.t.
+00000230: 7c05 740e 8302 725d 7c00 6a0f 7d06 7c06  |.t...r]|.j.}.|.
+00000240: 7c05 8301 0100 7c00 a010 7c05 7c04 6a11  |.....|...|.|.j.
+00000250: a102 0100 7142 7403 7c04 740e 8302 7274  ....qBt.|.t...rt
+00000260: 7c00 a00f 7c04 a101 0100 7142 7403 7c04  |...|.....qBt.|.
+00000270: 740c 8302 727e 7c00 a00d 7c04 a101 0100  t...r~|...|.....
+00000280: 7142 6400 5300 2904 4efa 012f a900 2901  qBd.S.).N../..).
+00000290: 720c 0000 0029 1272 0300 0000 da08 5f5f  r....).r......__
+000002a0: 696e 6974 5f5f da05 7375 7065 72da 0a69  init__..super..i
+000002b0: 7369 6e73 7461 6e63 6572 0900 0000 da04  sinstancer......
+000002c0: 6469 6374 da06 726f 7574 6573 da0c 5f73  dict..routes.._s
+000002d0: 6574 5f73 7461 636b 6564 da05 6974 656d  et_stacked..item
+000002e0: 73da 0361 6464 7207 0000 00da 0563 6869  s..addr......chi
+000002f0: 6c64 7204 0000 00da 0961 6464 5769 6467  ldr......addWidg
+00000300: 6574 7205 0000 00da 0761 6464 4974 656d  etr......addItem
+00000310: da0c 7365 7441 6c69 676e 6d65 6e74 da09  ..setAlignment..
+00000320: 616c 6967 6e6d 656e 7429 07da 0473 656c  alignment)...sel
+00000330: 6672 0b00 0000 da06 6b77 6172 6773 da05  fr......kwargs..
+00000340: 726f 7574 6572 1600 0000 da07 5f77 6964  router......_wid
+00000350: 6765 74da 055f 6675 6e63 a901 da09 5f5f  get.._func....__
+00000360: 636c 6173 735f 5f72 0d00 0000 fa51 2f68  class__r.....Q/h
+00000370: 6f6d 652f 6f73 616d 612f 576f 726b 7370  ome/osama/Worksp
+00000380: 6163 652f 2e76 656e 762f 6c69 622f 7079  ace/.venv/lib/py
+00000390: 7468 6f6e 332e 3130 2f73 6974 652d 7061  thon3.10/site-pa
+000003a0: 636b 6167 6573 2f51 7469 6361 2f6c 6179  ckages/Qtica/lay
+000003b0: 6f75 7473 2f73 7461 636b 6564 2e70 7972  outs/stacked.pyr
+000003c0: 0e00 0000 0800 0000 7332 0000 000a 0412  ........s2......
+000003d0: 0104 0204 010e 021e 010c 0110 0110 0104  ................
+000003e0: ff08 030a 0106 010a 0208 010a 0106 0108  ................
+000003f0: 0210 010a 020c 010a 020a 0102 8004 f07a  ...............z
+00000400: 1653 7461 636b 6564 4c61 796f 7574 2e5f  .StackedLayout._
+00000410: 5f69 6e69 745f 5f29 0cda 085f 5f6e 616d  _init__)...__nam
+00000420: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000430: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0200  .__qualname__r..
+00000440: 0000 da04 6c69 7374 7204 0000 0072 0500  ....listr....r..
+00000450: 0000 7207 0000 0072 0900 0000 7211 0000  ..r....r....r...
+00000460: 0072 0e00 0000 da0d 5f5f 636c 6173 7363  .r......__classc
+00000470: 656c 6c5f 5f72 0d00 0000 720d 0000 0072  ell__r....r....r
+00000480: 2000 0000 7222 0000 0072 0a00 0000 0700   ...r"...r......
+00000490: 0000 730a 0000 0008 0002 0306 fe1a 0216  ..s.............
+000004a0: fe72 0a00 0000 4e29 0cda 0674 7970 696e  .r....N)...typin
+000004b0: 6772 0200 0000 da11 5079 5369 6465 362e  gr......PySide6.
+000004c0: 5174 5769 6467 6574 7372 0300 0000 7204  QtWidgetsr....r.
+000004d0: 0000 0072 0500 0000 da0f 7574 696c 732e  ...r......utils.
+000004e0: 616c 6967 6e6d 656e 7472 0700 0000 da04  alignmentr......
+000004f0: 636f 7265 7208 0000 0072 0900 0000 720a  corer....r....r.
+00000500: 0000 0072 0d00 0000 720d 0000 0072 0d00  ...r....r....r..
+00000510: 0000 7222 0000 00da 083c 6d6f 6475 6c65  ..r".....<module
+00000520: 3e01 0000 0073 0a00 0000 0c00 1401 0c01  >....s..........
+00000530: 1001 1603                                ....
```

### Comparing `qtica-0.4.3/Qtica/layouts/__pycache__/stacked.cpython-312.pyc` & `qtica-0.5.0/Qtica/layouts/__pycache__/stacked.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/layouts/__pycache__/v_layout.cpython-312.pyc` & `qtica-0.5.0/Qtica/layouts/__pycache__/v_layout.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/layouts/border_layout.py` & `qtica-0.5.0/Qtica/layouts/border_layout.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/layouts/flow_layout.py` & `qtica-0.5.0/Qtica/layouts/flow_layout.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/layouts/form_layout.py` & `qtica-0.5.0/Qtica/layouts/form_layout.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/layouts/grid_layout.py` & `qtica-0.5.0/Qtica/layouts/grid_layout.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/layouts/h_layout.py` & `qtica-0.5.0/Qtica/layouts/vh_layout.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 from typing import Union
-from PySide6.QtWidgets import QHBoxLayout, QLayoutItem, QSpacerItem, QWidget, QLayout
-from ..tools.wrappers.h_layout import HLayoutWrapper, ColumnLayoutWrapper
+from PySide6.QtWidgets import QLayoutItem, QSpacerItem, QWidget, QLayout
+from ..tools.wrappers.layout import LayoutWrapper
 from ..utils.alignment import Alignment
 from ..core import AbstractQObject
 
 
-class HLayout(AbstractQObject, QHBoxLayout):
+
+class VHLayout(AbstractQObject):
     def __init__(self,
                  *,
                  children: list[Union[QWidget, 
                                       QLayout, 
-                                      HLayoutWrapper,
-                                      ColumnLayoutWrapper,
+                                      LayoutWrapper,
                                       Alignment]] = None,
                  **kwargs):
-        QHBoxLayout.__init__(self)
         super().__init__(**kwargs)
 
         if not children:
             return
 
         for child in children:
-            if isinstance(child, Alignment):
-                _widget = child.child
+            self._add_child(child)
+
+    def _add_child(self, child):
+        if isinstance(child, Alignment):
+            _widget = child.child
 
-                if isinstance(_widget, QWidget):
-                    _func = self.addWidget
-                elif isinstance(_widget, QLayoutItem):
-                    _func = self.addItem
+            if isinstance(_widget, QWidget):
+                _func = self.addWidget
+            elif isinstance(_widget, QLayoutItem):
+                _func = self.addItem
 
-                _func(_widget)
-                self.setAlignment(_widget, child.alignment)
+            _func(_widget)
+            self.setAlignment(_widget, child.alignment)
 
-            elif isinstance(child, HLayoutWrapper):
-                _widget = child.child
+        elif isinstance(child, LayoutWrapper):
+            _widget = child.child
 
-                if isinstance(_widget, QWidget):
-                    _func = self.addWidget
-                elif isinstance(_widget, QLayout):
-                    _func = self.addLayout
+            if isinstance(_widget, QWidget):
+                _func = self.addWidget
+            elif isinstance(_widget, QLayout):
+                _func = self.addLayout
 
-                _func(*child._yield_attr())
+            _func(*child._yield_attr())
 
-            elif isinstance(child, QSpacerItem):
-                self.addSpacerItem(child)
+        elif isinstance(child, QSpacerItem):
+            self.addSpacerItem(child)
 
-            elif isinstance(child, QLayoutItem):
-                self.addItem(child)
+        elif isinstance(child, QLayoutItem):
+            self.addItem(child)
 
-            elif isinstance(child, QWidget):
-                self.addWidget(child)
+        elif isinstance(child, QWidget):
+            self.addWidget(child)
 
-            elif isinstance(child, QLayout):
-                self.addLayout(child)
+        elif isinstance(child, QLayout):
+            self.addLayout(child)
 
 
-class ColumnLayout(HLayout):
-    ...
+    def __iadd__(self, other):
+        self._add_child(other)
+        return self
```

### Comparing `qtica-0.4.3/Qtica/layouts/v_layout.py` & `qtica-0.5.0/Qtica/layouts/stacked.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,40 @@
 from typing import Union
-from PySide6.QtWidgets import QLayoutItem, QSpacerItem, QVBoxLayout, QWidget, QLayout
-from ..tools.wrappers.v_layout import VLayoutWrapper, RowLayoutWrapper
+from PySide6.QtWidgets import QStackedLayout, QWidget, QLayoutItem
 from ..utils.alignment import Alignment
-from ..core import AbstractQObject
+from ..core import AbstractQObject, Routes
 
 
-class VLayout(AbstractQObject, QVBoxLayout):
+class StackedLayout(AbstractQObject, QStackedLayout):
     def __init__(self,
                  *,
-                 children: list[Union[QWidget, 
-                                      QLayout, 
-                                      VLayoutWrapper,
-                                      RowLayoutWrapper,
-                                      Alignment]] = None,
+                 children: Union[list[Union[QWidget, QLayoutItem, Alignment]], Routes, dict] = None,
                  **kwargs):
-        QVBoxLayout.__init__(self)
+        QStackedLayout.__init__(self)
         super().__init__(**kwargs)
 
         if not children:
             return
 
-        for child in children:
-            if isinstance(child, Alignment):
-                _widget = child.child
+        if isinstance(children, (Routes, dict)):
+            self.routes = Routes("/", **children) if isinstance(children, dict) else children
+            self.routes._set_stacked(self)
+            for route, child in children.items():
+                self.routes.add(route, child)
+        else:
+            for child in children:
+                if isinstance(child, Alignment):
+                    _widget = child.child
+
+                    if isinstance(_widget, QWidget):
+                        _func = self.addWidget
+                    elif isinstance(_widget, QLayoutItem):
+                        _func = self.addItem
 
-                if isinstance(_widget, QWidget):
-                    _func = self.addWidget
-                elif isinstance(_widget, QLayoutItem):
-                    _func = self.addItem
+                    _func(_widget)
+                    self.setAlignment(_widget, child.alignment)
 
-                _func(_widget)
-                self.setAlignment(_widget, child.alignment)
+                elif isinstance(child, QLayoutItem):
+                    self.addItem(child)
 
-            elif isinstance(child, VLayoutWrapper):
-                _widget = child.child
-
-                if isinstance(_widget, QWidget):
-                    _func = self.addWidget
-                elif isinstance(_widget, QLayout):
-                    _func = self.addLayout
-
-                _func(*child._yield_attr())
-
-            elif isinstance(child, QSpacerItem):
-                self.addSpacerItem(child)
-
-            elif isinstance(child, QLayoutItem):
-                self.addItem(child)
-
-            elif isinstance(child, QWidget):
-                self.addWidget(child)
-
-            elif isinstance(child, QLayout):
-                self.addLayout(child)
-
-
-class RowLayout(VLayout):
-    ...
+                elif isinstance(child, QWidget):
+                    self.addWidget(child)
```

### Comparing `qtica-0.4.3/Qtica/painters/__pycache__/_tails.cpython-310.pyc` & `qtica-0.5.0/Qtica/painters/__pycache__/_tails.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/painters/__pycache__/circular_progress.cpython-310.pyc` & `qtica-0.5.0/Qtica/painters/__pycache__/circular_progress.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/painters/__pycache__/circular_progress.cpython-312.pyc` & `qtica-0.5.0/Qtica/painters/__pycache__/circular_progress.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/painters/__pycache__/status_edge.cpython-310.pyc` & `qtica-0.5.0/Qtica/painters/__pycache__/status_edge.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/painters/__pycache__/status_edge.cpython-312.pyc` & `qtica-0.5.0/Qtica/painters/__pycache__/status_edge.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/painters/__pycache__/teaching_tip.cpython-310.pyc` & `qtica-0.5.0/Qtica/painters/__pycache__/teaching_tip.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/painters/circular_progress.py` & `qtica-0.5.0/Qtica/painters/circular_progress.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/painters/status_edge.py` & `qtica-0.5.0/Qtica/painters/status_edge.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/services/__pycache__/__init__.cpython-310.pyc` & `qtica-0.5.0/Qtica/services/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/services/__pycache__/__init__.cpython-312.pyc` & `qtica-0.5.0/Qtica/services/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/services/__pycache__/_methods.cpython-310.pyc` & `qtica-0.5.0/Qtica/services/__pycache__/_methods.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Feb  3 20:59:04 2024 UTC, .py size: 4482 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 18a9 be65 8211 0000  o..........e....
+00000000: 6f0d 0d0a 0000 0000 f8bb e865 8211 0000  o..........e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000e 0000 0040 0000 0073 3202 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d03 5a03 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c04 6d05 5a05 0100 6400 6405 6c06  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 6d08 5a08 0100 6400 6406 6c09  m.Z.m.Z...d.d.l.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `qtica-0.4.3/Qtica/services/__pycache__/_methods.cpython-312.pyc` & `qtica-0.5.0/Qtica/services/__pycache__/_methods.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/services/__pycache__/clipboard.cpython-310.pyc` & `qtica-0.5.0/Qtica/services/__pycache__/clipboard.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/services/__pycache__/clipboard.cpython-312.pyc` & `qtica-0.5.0/Qtica/services/__pycache__/clipboard.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/services/__pycache__/launche_url.cpython-310.pyc` & `qtica-0.5.0/Qtica/services/__pycache__/launche_url.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/services/__pycache__/launche_url.cpython-312.pyc` & `qtica-0.5.0/Qtica/services/__pycache__/launche_url.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/services/__pycache__/message_handler.cpython-310.pyc` & `qtica-0.5.0/Qtica/services/__pycache__/message_handler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/services/__pycache__/message_handler.cpython-312.pyc` & `qtica-0.5.0/Qtica/services/__pycache__/message_handler.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/services/_methods.py` & `qtica-0.5.0/Qtica/services/_methods.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/services/clipboard.py` & `qtica-0.5.0/Qtica/services/clipboard.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/services/launche_url.py` & `qtica-0.5.0/Qtica/services/launche_url.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/services/message_handler.py` & `qtica-0.5.0/Qtica/services/message_handler.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__init__.py` & `qtica-0.5.0/Qtica/tools/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from .wrappers import *
 from .qtcore import *
 from .qtgui import *
 
 from .icon import Icon
 from .movie import Movie
 from .color import Color
-from .qt_file_open import File
+from .qt_file_open import OpenFile, TempFile
 from .settings import Settings
 from .ui_loader import UiLoader
 from .system_tray import SystemTray
 from .size_policy import SizePolicy
 from .smooth_scroll import SmoothScroll
 from .copy_progress import CopyProgress
 from .spacer_item import SpacerItem
 from .action import LinePasswordAction, MenuAction
 from .media_player import MediaPlayer
-from .list_widget_item import ListWidgetItem
+from .list_widget_item import ListWidgetItem
```

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/__init__.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Feb 23 21:06:58 2024 UTC, .py size: 556 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,56 @@
-00000000: 6f0d 0d0a 0000 0000 f208 d965 2c02 0000  o..........e,...
+00000000: 6f0d 0d0a 0000 0000 a049 0766 3b02 0000  o........I.f;...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 c800 0000 6400  .....@...s....d.
+00000020: 0002 0000 0040 0000 0073 cc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5400 6400 6401 6c01 5400 6400  d.l.T.d.d.l.T.d.
 00000040: 6401 6c02 5400 6400 6402 6c03 6d04 5a04  d.l.T.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 0100 6400 6405 6c09  d.l.m.Z...d.d.l.
-00000070: 6d0a 5a0a 0100 6400 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
-00000080: 0100 6400 6407 6c0d 6d0e 5a0e 0100 6400  ..d.d.l.m.Z...d.
-00000090: 6408 6c0f 6d10 5a10 0100 6400 6409 6c11  d.l.m.Z...d.d.l.
-000000a0: 6d12 5a12 0100 6400 640a 6c13 6d14 5a14  m.Z...d.d.l.m.Z.
-000000b0: 0100 6400 640b 6c15 6d16 5a16 0100 6400  ..d.d.l.m.Z...d.
-000000c0: 640c 6c17 6d18 5a18 0100 6400 640d 6c19  d.l.m.Z...d.d.l.
-000000d0: 6d1a 5a1a 6d1b 5a1b 0100 6400 640e 6c1c  m.Z.m.Z...d.d.l.
-000000e0: 6d1d 5a1d 0100 6400 640f 6c1e 6d1f 5a1f  m.Z...d.d.l.m.Z.
-000000f0: 0100 6410 5300 2911 e901 0000 0029 01da  ..d.S.)......)..
-00000100: 012a 2901 da04 4963 6f6e 2901 da05 4d6f  .*)...Icon)...Mo
-00000110: 7669 6529 01da 0543 6f6c 6f72 2901 da04  vie)...Color)...
-00000120: 4669 6c65 2901 da08 5365 7474 696e 6773  File)...Settings
-00000130: 2901 da08 5569 4c6f 6164 6572 2901 da0a  )...UiLoader)...
-00000140: 5379 7374 656d 5472 6179 2901 da0a 5369  SystemTray)...Si
-00000150: 7a65 506f 6c69 6379 2901 da0c 536d 6f6f  zePolicy)...Smoo
-00000160: 7468 5363 726f 6c6c 2901 da0c 436f 7079  thScroll)...Copy
-00000170: 5072 6f67 7265 7373 2901 da0a 5370 6163  Progress)...Spac
-00000180: 6572 4974 656d 2902 da12 4c69 6e65 5061  erItem)...LinePa
-00000190: 7373 776f 7264 4163 7469 6f6e da0a 4d65  sswordAction..Me
-000001a0: 6e75 4163 7469 6f6e 2901 da0b 4d65 6469  nuAction)...Medi
-000001b0: 6150 6c61 7965 7229 01da 0e4c 6973 7457  aPlayer)...ListW
-000001c0: 6964 6765 7449 7465 6d4e 2920 da08 7772  idgetItemN) ..wr
-000001d0: 6170 7065 7273 da06 7174 636f 7265 da05  appers..qtcore..
-000001e0: 7174 6775 69da 0469 636f 6e72 0300 0000  qtgui..iconr....
-000001f0: da05 6d6f 7669 6572 0400 0000 da05 636f  ..movier......co
-00000200: 6c6f 7272 0500 0000 da0c 7174 5f66 696c  lorr......qt_fil
-00000210: 655f 6f70 656e 7206 0000 00da 0873 6574  e_openr......set
-00000220: 7469 6e67 7372 0700 0000 da09 7569 5f6c  tingsr......ui_l
-00000230: 6f61 6465 7272 0800 0000 da0b 7379 7374  oaderr......syst
-00000240: 656d 5f74 7261 7972 0900 0000 da0b 7369  em_trayr......si
-00000250: 7a65 5f70 6f6c 6963 7972 0a00 0000 da0d  ze_policyr......
-00000260: 736d 6f6f 7468 5f73 6372 6f6c 6c72 0b00  smooth_scrollr..
-00000270: 0000 da0d 636f 7079 5f70 726f 6772 6573  ....copy_progres
-00000280: 7372 0c00 0000 da0b 7370 6163 6572 5f69  sr......spacer_i
-00000290: 7465 6d72 0d00 0000 da06 6163 7469 6f6e  temr......action
-000002a0: 720e 0000 0072 0f00 0000 da0c 6d65 6469  r....r......medi
-000002b0: 615f 706c 6179 6572 7210 0000 00da 106c  a_playerr......l
-000002c0: 6973 745f 7769 6467 6574 5f69 7465 6d72  ist_widget_itemr
-000002d0: 1100 0000 a900 7223 0000 0072 2300 0000  ......r#...r#...
-000002e0: fa50 2f68 6f6d 652f 6f73 616d 612f 576f  .P/home/osama/Wo
-000002f0: 726b 7370 6163 652f 2e76 656e 762f 6c69  rkspace/.venv/li
-00000300: 622f 7079 7468 6f6e 332e 3130 2f73 6974  b/python3.10/sit
-00000310: 652d 7061 636b 6167 6573 2f51 7469 6361  e-packages/Qtica
-00000320: 2f74 6f6f 6c73 2f5f 5f69 6e69 745f 5f2e  /tools/__init__.
-00000330: 7079 da08 3c6d 6f64 756c 653e 0100 0000  py..<module>....
-00000340: 7322 0000 0008 0008 0108 010c 020c 010c  s"..............
-00000350: 010c 010c 010c 010c 010c 010c 010c 010c  ................
-00000360: 0110 010c 0110 01                        .......
+00000070: 6d0a 5a0a 6d0b 5a0b 0100 6400 6406 6c0c  m.Z.m.Z...d.d.l.
+00000080: 6d0d 5a0d 0100 6400 6407 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
+00000090: 0100 6400 6408 6c10 6d11 5a11 0100 6400  ..d.d.l.m.Z...d.
+000000a0: 6409 6c12 6d13 5a13 0100 6400 640a 6c14  d.l.m.Z...d.d.l.
+000000b0: 6d15 5a15 0100 6400 640b 6c16 6d17 5a17  m.Z...d.d.l.m.Z.
+000000c0: 0100 6400 640c 6c18 6d19 5a19 0100 6400  ..d.d.l.m.Z...d.
+000000d0: 640d 6c1a 6d1b 5a1b 6d1c 5a1c 0100 6400  d.l.m.Z.m.Z...d.
+000000e0: 640e 6c1d 6d1e 5a1e 0100 6400 640f 6c1f  d.l.m.Z...d.d.l.
+000000f0: 6d20 5a20 0100 6410 5300 2911 e901 0000  m Z ..d.S.).....
+00000100: 0029 01da 012a 2901 da04 4963 6f6e 2901  .)...*)...Icon).
+00000110: da05 4d6f 7669 6529 01da 0543 6f6c 6f72  ..Movie)...Color
+00000120: 2902 da08 4f70 656e 4669 6c65 da08 5465  )...OpenFile..Te
+00000130: 6d70 4669 6c65 2901 da08 5365 7474 696e  mpFile)...Settin
+00000140: 6773 2901 da08 5569 4c6f 6164 6572 2901  gs)...UiLoader).
+00000150: da0a 5379 7374 656d 5472 6179 2901 da0a  ..SystemTray)...
+00000160: 5369 7a65 506f 6c69 6379 2901 da0c 536d  SizePolicy)...Sm
+00000170: 6f6f 7468 5363 726f 6c6c 2901 da0c 436f  oothScroll)...Co
+00000180: 7079 5072 6f67 7265 7373 2901 da0a 5370  pyProgress)...Sp
+00000190: 6163 6572 4974 656d 2902 da12 4c69 6e65  acerItem)...Line
+000001a0: 5061 7373 776f 7264 4163 7469 6f6e da0a  PasswordAction..
+000001b0: 4d65 6e75 4163 7469 6f6e 2901 da0b 4d65  MenuAction)...Me
+000001c0: 6469 6150 6c61 7965 7229 01da 0e4c 6973  diaPlayer)...Lis
+000001d0: 7457 6964 6765 7449 7465 6d4e 2921 da08  tWidgetItemN)!..
+000001e0: 7772 6170 7065 7273 da06 7174 636f 7265  wrappers..qtcore
+000001f0: da05 7174 6775 69da 0469 636f 6e72 0300  ..qtgui..iconr..
+00000200: 0000 da05 6d6f 7669 6572 0400 0000 da05  ....movier......
+00000210: 636f 6c6f 7272 0500 0000 da0c 7174 5f66  colorr......qt_f
+00000220: 696c 655f 6f70 656e 7206 0000 0072 0700  ile_openr....r..
+00000230: 0000 da08 7365 7474 696e 6773 7208 0000  ....settingsr...
+00000240: 00da 0975 695f 6c6f 6164 6572 7209 0000  ...ui_loaderr...
+00000250: 00da 0b73 7973 7465 6d5f 7472 6179 720a  ...system_trayr.
+00000260: 0000 00da 0b73 697a 655f 706f 6c69 6379  .....size_policy
+00000270: 720b 0000 00da 0d73 6d6f 6f74 685f 7363  r......smooth_sc
+00000280: 726f 6c6c 720c 0000 00da 0d63 6f70 795f  rollr......copy_
+00000290: 7072 6f67 7265 7373 720d 0000 00da 0b73  progressr......s
+000002a0: 7061 6365 725f 6974 656d 720e 0000 00da  pacer_itemr.....
+000002b0: 0661 6374 696f 6e72 0f00 0000 7210 0000  .actionr....r...
+000002c0: 00da 0c6d 6564 6961 5f70 6c61 7965 7272  ...media_playerr
+000002d0: 1100 0000 da10 6c69 7374 5f77 6964 6765  ......list_widge
+000002e0: 745f 6974 656d 7212 0000 00a9 0072 2400  t_itemr......r$.
+000002f0: 0000 7224 0000 00fa 502f 686f 6d65 2f6f  ..r$....P/home/o
+00000300: 7361 6d61 2f57 6f72 6b73 7061 6365 2f2e  sama/Workspace/.
+00000310: 7665 6e76 2f6c 6962 2f70 7974 686f 6e33  venv/lib/python3
+00000320: 2e31 302f 7369 7465 2d70 6163 6b61 6765  .10/site-package
+00000330: 732f 5174 6963 612f 746f 6f6c 732f 5f5f  s/Qtica/tools/__
+00000340: 696e 6974 5f5f 2e70 79da 083c 6d6f 6475  init__.py..<modu
+00000350: 6c65 3e01 0000 0073 2200 0000 0800 0801  le>....s".......
+00000360: 0801 0c02 0c01 0c01 1001 0c01 0c01 0c01  ................
+00000370: 0c01 0c01 0c01 0c01 1001 0c01 1001       ..............
```

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/__init__.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/action.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/action.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/action.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/action.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/alignment.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/alignment.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/alignment.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/alignment.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/brush.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/brush.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/brush.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/brush.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/center.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/center.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/color.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/color.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/color.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/color.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/copy_progress.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/copy_progress.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/copy_progress.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/copy_progress.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/elided_text.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/elided_text.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/elided_text.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/elided_text.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/env_var.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/env_var.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/icon.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/icon.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/icon.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/icon.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/linear_gradient.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/linear_gradient.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/linear_gradient.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/linear_gradient.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/modifiers.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/modifiers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/modifiers.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/modifiers.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/movie.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/movie.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/movie.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/movie.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/movie_view.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/movie_view.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/painter.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/painter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/pen.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/pen.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/pen.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/pen.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/picker.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/picker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/qstyle_sheet.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/qstyle_sheet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/qt_file_open.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/wrappers/__pycache__/v_layout.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Feb 14 20:08:53 2024 UTC, .py size: 586 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,69 @@
-00000000: 6f0d 0d0a 0000 0000 d51d cd65 4a02 0000  o..........eJ...
+00000000: 6f0d 0d0a 0000 0000 619a 9865 6202 0000  o.......a..eb...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
-00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
-00000040: 8400 6403 6501 8303 5a02 6404 5300 2905  ..d.e...Z.d.S.).
-00000050: e900 0000 0029 01da 0551 4669 6c65 6300  .....)...QFilec.
-00000060: 0000 0000 0000 0000 0000 0000 0000 0005  ................
-00000070: 0000 0000 0000 0073 5e00 0000 6500 5a01  .......s^...e.Z.
-00000080: 6400 5a02 6503 6a04 6a05 6601 6401 6506  d.Z.e.j.j.f.d.e.
-00000090: 6402 6503 6a04 6604 8700 6601 6403 6404  d.e.j.f...f.d.d.
-000000a0: 840d 5a07 6405 6406 8400 5a08 640f 6409  ..Z.d.d...Z.d.d.
-000000b0: 640a 8404 5a09 6407 6506 6602 640b 640c  d...Z.d.e.f.d.d.
-000000c0: 8404 5a0a 6407 6506 6602 640d 640e 8404  ..Z.d.e.f.d.d...
-000000d0: 5a0b 8700 0400 5a0c 5300 2910 da04 4669  Z.....Z.S.)...Fi
-000000e0: 6c65 da04 6669 6c65 da04 6d6f 6465 6303  le..file..modec.
-000000f0: 0000 0000 0000 0000 0000 0003 0000 0003  ................
-00000100: 0000 0003 0000 0073 1600 0000 7400 8300  .......s....t...
-00000110: a001 7c01 a101 0100 7c02 7c00 5f02 6400  ..|.....|.|._.d.
-00000120: 5300 a901 4e29 03da 0573 7570 6572 da08  S...N)...super..
-00000130: 5f5f 696e 6974 5f5f da05 5f6d 6f64 6529  __init__.._mode)
-00000140: 03da 0473 656c 6672 0400 0000 7205 0000  ...selfr....r...
-00000150: 00a9 01da 095f 5f63 6c61 7373 5f5f a900  .....__class__..
-00000160: fa54 2f68 6f6d 652f 6f73 616d 612f 576f  .T/home/osama/Wo
-00000170: 726b 7370 6163 652f 2e76 656e 762f 6c69  rkspace/.venv/li
-00000180: 622f 7079 7468 6f6e 332e 3130 2f73 6974  b/python3.10/sit
-00000190: 652d 7061 636b 6167 6573 2f51 7469 6361  e-packages/Qtica
-000001a0: 2f74 6f6f 6c73 2f71 745f 6669 6c65 5f6f  /tools/qt_file_o
-000001b0: 7065 6e2e 7079 7208 0000 0005 0000 0073  pen.pyr........s
-000001c0: 0400 0000 0c03 0a01 7a0d 4669 6c65 2e5f  ........z.File._
-000001d0: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
-000001e0: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
-000001f0: 7310 0000 007c 00a0 007c 006a 01a1 0101  s....|...|.j....
-00000200: 007c 0053 0072 0600 0000 2902 da04 6f70  .|.S.r....)...op
-00000210: 656e 7209 0000 00a9 0172 0a00 0000 720d  enr......r....r.
-00000220: 0000 0072 0d00 0000 720e 0000 00da 095f  ...r....r......_
-00000230: 5f65 6e74 6572 5f5f 0b00 0000 7304 0000  _enter__....s...
-00000240: 000c 0104 017a 0e46 696c 652e 5f5f 656e  .....z.File.__en
-00000250: 7465 725f 5fda 0672 6574 7572 6e4e 6304  ter__..returnNc.
-00000260: 0000 0000 0000 0000 0000 0004 0000 0002  ................
-00000270: 0000 0043 0000 0073 0c00 0000 7c00 a000  ...C...s....|...
-00000280: a100 0100 6400 5300 7206 0000 0029 01da  ....d.S.r....)..
-00000290: 0563 6c6f 7365 2904 720a 0000 00da 0e65  .close).r......e
-000002a0: 7863 6570 7469 6f6e 5f74 7970 65da 0f65  xception_type..e
-000002b0: 7863 6570 7469 6f6e 5f76 616c 7565 da13  xception_value..
-000002c0: 6578 6365 7074 696f 6e5f 7472 6163 6562  exception_traceb
-000002d0: 6163 6b72 0d00 0000 720d 0000 0072 0e00  ackr....r....r..
-000002e0: 0000 da08 5f5f 6578 6974 5f5f 0f00 0000  ....__exit__....
-000002f0: 7302 0000 000c 017a 0d46 696c 652e 5f5f  s......z.File.__
-00000300: 6578 6974 5f5f 6301 0000 0000 0000 0000  exit__c.........
-00000310: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
-00000320: 1000 0000 7400 7c00 a001 a100 6401 6402  ....t.|.....d.d.
-00000330: 8d02 5300 2903 4e7a 0575 7466 2d38 2901  ..S.).Nz.utf-8).
-00000340: da08 656e 636f 6469 6e67 2902 da03 7374  ..encoding)...st
-00000350: 72da 0772 6561 6441 6c6c 7210 0000 0072  r..readAllr....r
-00000360: 0d00 0000 720d 0000 0072 0e00 0000 da0f  ....r....r......
-00000370: 7265 6164 5f77 6974 685f 7574 665f 3812  read_with_utf_8.
-00000380: 0000 0073 0200 0000 1001 7a14 4669 6c65  ...s......z.File
-00000390: 2e72 6561 645f 7769 7468 5f75 7466 5f38  .read_with_utf_8
-000003a0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000003b0: 0002 0000 0043 0000 0073 0800 0000 7c00  .....C...s....|.
-000003c0: a000 a100 5300 7206 0000 0029 0172 1b00  ....S.r....).r..
-000003d0: 0000 7210 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-000003e0: 0072 0e00 0000 da08 7265 6164 5574 6638  .r......readUtf8
-000003f0: 1500 0000 7302 0000 0008 017a 0d46 696c  ....s......z.Fil
-00000400: 652e 7265 6164 5574 6638 2902 7212 0000  e.readUtf8).r...
-00000410: 004e 290d da08 5f5f 6e61 6d65 5f5f da0a  .N)...__name__..
-00000420: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00000430: 616c 6e61 6d65 5f5f 7202 0000 00da 0c4f  alname__r......O
-00000440: 7065 6e4d 6f64 6546 6c61 67da 0852 6561  penModeFlag..Rea
-00000450: 644f 6e6c 7972 1900 0000 7208 0000 0072  dOnlyr....r....r
-00000460: 1100 0000 7217 0000 0072 1b00 0000 721c  ....r....r....r.
-00000470: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-00000480: 5f5f 720d 0000 0072 0d00 0000 720b 0000  __r....r....r...
-00000490: 0072 0e00 0000 7203 0000 0004 0000 0073  .r....r........s
-000004a0: 1600 0000 0800 0603 04fe 0201 02ff 0402  ................
-000004b0: 0efe 0806 0a04 0e03 1603 7203 0000 004e  ..........r....N
-000004c0: 2903 da0e 5079 5369 6465 362e 5174 436f  )...PySide6.QtCo
-000004d0: 7265 7202 0000 0072 0300 0000 720d 0000  rer....r....r...
-000004e0: 0072 0d00 0000 720d 0000 0072 0e00 0000  .r....r....r....
-000004f0: da08 3c6d 6f64 756c 653e 0100 0000 7304  ..<module>....s.
-00000500: 0000 000c 0014 03                        .......
+00000020: 0004 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
+00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
+00000040: 6402 6c03 6d04 5a04 0100 4700 6403 6404  d.l.m.Z...G.d.d.
+00000050: 8400 6404 8302 5a05 4700 6405 6406 8400  ..d...Z.G.d.d...
+00000060: 6406 6505 8303 5a06 6407 5300 2908 e900  d.e...Z.d.S.)...
+00000070: 0000 0029 02da 0751 5769 6467 6574 da07  ...)...QWidget..
+00000080: 514c 6179 6f75 7429 01da 0251 7463 0000  QLayout)...Qtc..
+00000090: 0000 0000 0000 0000 0000 0000 0000 0900  ................
+000000a0: 0000 4000 0000 733a 0000 0065 005a 0164  ..@...s:...e.Z.d
+000000b0: 005a 0209 0109 0164 0a64 0265 0365 0442  .Z.....d.d.e.e.B
+000000c0: 0064 0365 0564 0465 066a 0764 0564 0166  .d.e.d.e.j.d.d.f
+000000d0: 0864 0664 0784 055a 0864 0864 0984 005a  .d.d...Z.d.d...Z
+000000e0: 0964 0153 0029 0bda 0e56 4c61 796f 7574  .d.S.)...VLayout
+000000f0: 5772 6170 7065 724e da05 6368 696c 64da  WrapperN..child.
+00000100: 0773 7472 6574 6368 da09 616c 6967 6e6d  .stretch..alignm
+00000110: 656e 74da 0672 6574 7572 6e63 0400 0000  ent..returnc....
+00000120: 0000 0000 0000 0000 0400 0000 0200 0000  ................
+00000130: 4300 0000 7316 0000 007c 017c 005f 007c  C...s....|.|._.|
+00000140: 027c 005f 017c 037c 005f 0264 0053 00a9  .|._.|.|._.d.S..
+00000150: 014e a903 7206 0000 0072 0700 0000 7208  .N..r....r....r.
+00000160: 0000 0029 04da 0473 656c 6672 0600 0000  ...)...selfr....
+00000170: 7207 0000 0072 0800 0000 a900 720d 0000  r....r......r...
+00000180: 00fa 592f 686f 6d65 2f6f 7361 6d61 2f57  ..Y/home/osama/W
+00000190: 6f72 6b73 7061 6365 2f2e 7665 6e76 2f6c  orkspace/.venv/l
+000001a0: 6962 2f70 7974 686f 6e33 2e31 302f 7369  ib/python3.10/si
+000001b0: 7465 2d70 6163 6b61 6765 732f 5174 6963  te-packages/Qtic
+000001c0: 612f 746f 6f6c 732f 7772 6170 7065 7273  a/tools/wrappers
+000001d0: 2f76 5f6c 6179 6f75 742e 7079 da08 5f5f  /v_layout.py..__
+000001e0: 696e 6974 5f5f 0600 0000 7306 0000 0006  init__....s.....
+000001f0: 0506 010a 017a 1756 4c61 796f 7574 5772  .....z.VLayoutWr
+00000200: 6170 7065 722e 5f5f 696e 6974 5f5f 6301  apper.__init__c.
+00000210: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00000220: 0000 0063 0000 0073 2a00 0000 8100 7c00  ...c...s*.....|.
+00000230: 6a00 7c00 6a01 7c00 6a02 6603 4400 5d09  j.|.j.|.j.f.D.].
+00000240: 7d01 7c01 6400 7501 7212 7c01 5600 0100  }.|.d.u.r.|.V...
+00000250: 7109 6400 5300 720a 0000 0072 0b00 0000  q.d.S.r....r....
+00000260: 2902 720c 0000 00da 0461 7474 7272 0d00  ).r......attrr..
+00000270: 0000 720d 0000 0072 0e00 0000 da0b 5f79  ..r....r......_y
+00000280: 6965 6c64 5f61 7474 720f 0000 0073 1200  ield_attr....s..
+00000290: 0000 0280 0402 0401 0401 08fd 0805 0601  ................
+000002a0: 0280 04fa 7a1a 564c 6179 6f75 7457 7261  ....z.VLayoutWra
+000002b0: 7070 6572 2e5f 7969 656c 645f 6174 7472  pper._yield_attr
+000002c0: 2902 4e4e 290a da08 5f5f 6e61 6d65 5f5f  ).NN)...__name__
+000002d0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+000002e0: 7175 616c 6e61 6d65 5f5f 7202 0000 0072  qualname__r....r
+000002f0: 0300 0000 da03 696e 7472 0400 0000 da0d  ......intr......
+00000300: 416c 6967 6e6d 656e 7446 6c61 6772 0f00  AlignmentFlagr..
+00000310: 0000 7211 0000 0072 0d00 0000 720d 0000  ..r....r....r...
+00000320: 0072 0d00 0000 720e 0000 0072 0500 0000  .r....r....r....
+00000330: 0500 0000 731a 0000 0008 0002 0302 0104  ....s...........
+00000340: fd06 0102 ff02 0202 fe04 0302 fd02 030a  ................
+00000350: fd0c 0972 0500 0000 6300 0000 0000 0000  ...r....c.......
+00000360: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
+00000370: 0073 0c00 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+00000380: 5300 2902 da10 526f 774c 6179 6f75 7457  S.)...RowLayoutW
+00000390: 7261 7070 6572 4e29 0372 1200 0000 7213  rapperN).r....r.
+000003a0: 0000 0072 1400 0000 720d 0000 0072 0d00  ...r....r....r..
+000003b0: 0000 720d 0000 0072 0e00 0000 7217 0000  ..r....r....r...
+000003c0: 0019 0000 0073 0400 0000 0800 0401 7217  .....s........r.
+000003d0: 0000 004e 2907 da11 5079 5369 6465 362e  ...N)...PySide6.
+000003e0: 5174 5769 6467 6574 7372 0200 0000 7203  QtWidgetsr....r.
+000003f0: 0000 00da 0e50 7953 6964 6536 2e51 7443  .....PySide6.QtC
+00000400: 6f72 6572 0400 0000 7205 0000 0072 1700  orer....r....r..
+00000410: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
+00000420: 0072 0e00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000430: 0100 0000 7308 0000 0010 000c 010e 0314  ....s...........
+00000440: 14                                       .
```

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/qt_file_open.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/qt_file_open.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/settings.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/settings.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/settings.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/size_policy.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/size_policy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/size_policy.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/size_policy.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/smooth_scroll.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/smooth_scroll.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/smooth_scroll.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/smooth_scroll.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/svg_color.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/svg_color.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/system_tray.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/system_tray.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/system_tray.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/system_tray.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/ui_loader.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/ui_loader.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/__pycache__/ui_loader.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/__pycache__/ui_loader.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/action.py` & `qtica-0.5.0/Qtica/tools/action.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/copy_progress.py` & `qtica-0.5.0/Qtica/tools/copy_progress.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/icon.py` & `qtica-0.5.0/Qtica/tools/icon.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/media_player.py` & `qtica-0.5.0/Qtica/tools/media_player.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/movie.py` & `qtica-0.5.0/Qtica/tools/movie.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/qtcore/__pycache__/objects.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/qtcore/__pycache__/objects.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jan 30 22:56:04 2024 UTC, .py size: 5753 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 6f0d 0d0a 0000 0000 847e b965 7916 0000  o........~.ey...
+00000000: 6f0d 0d0a 0000 0000 a148 0766 1d17 0000  o........H.f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 7402 0000 6400  .....@...st...d.
+00000020: 0005 0000 0040 0000 0073 8802 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000050: 6503 6501 6a04 8304 5a05 4700 6406 6407  e.e.j...Z.G.d.d.
 00000060: 8400 6407 6503 6501 6a06 8304 5a07 4700  ..d.e.e.j...Z.G.
 00000070: 6408 6409 8400 6409 6503 6501 6a08 8304  d.d...d.e.e.j...
 00000080: 5a09 4700 640a 640b 8400 640b 6503 6501  Z.G.d.d...d.e.e.
 00000090: 6a0a 8304 5a0b 4700 640c 640d 8400 640d  j...Z.G.d.d...d.
@@ -35,457 +35,470 @@
 00000220: 6a32 8304 5a33 4700 6434 6435 8400 6435  j2..Z3G.d4d5..d5
 00000230: 6503 6501 6a34 8304 5a35 4700 6436 6437  e.e.j4..Z5G.d6d7
 00000240: 8400 6437 6503 6501 6a36 8304 5a37 4700  ..d7e.e.j6..Z7G.
 00000250: 6438 6439 8400 6439 6503 6501 6a38 8304  d8d9..d9e.e.j8..
 00000260: 5a39 4700 643a 643b 8400 643b 6503 6501  Z9G.d:d;..d;e.e.
 00000270: 6a3a 8304 5a3b 4700 643c 643d 8400 643d  j:..Z;G.d<d=..d=
 00000280: 6503 6501 6a3c 8304 5a3d 4700 643e 643f  e.e.j<..Z=G.d>d?
-00000290: 8400 643f 6503 6501 6a3e 8304 5a3f 6440  ..d?e.e.j>..Z?d@
-000002a0: 5300 2941 e900 0000 0029 01da 0651 7443  S.)A.....)...QtC
-000002b0: 6f72 65e9 0300 0000 2901 da0f 4162 7374  ore.....)...Abst
-000002c0: 7261 6374 514f 626a 6563 7463 0000 0000  ractQObjectc....
-000002d0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-000002e0: 0000 0000 f31c 0000 0065 005a 0164 005a  .........e.Z.d.Z
-000002f0: 0287 0066 0164 0164 0284 085a 0387 0004  ...f.d.d...Z....
-00000300: 005a 0453 0029 03da 0e41 6e69 6d61 7469  .Z.S.)...Animati
-00000310: 6f6e 4772 6f75 7063 0100 0000 0000 0000  onGroupc........
-00000320: 0000 0000 0300 0000 0400 0000 0f00 0000  ................
-00000330: f32a 0000 0074 006a 016a 027c 0067 017c  .*...t.j.j.|.g.|
-00000340: 01a2 0152 008e 0001 0074 0383 006a 0264  ...R.....t...j.d
-00000350: 0169 007c 02a4 018e 0101 0064 0053 00a9  .i.|.......d.S..
-00000360: 024e a900 2904 7202 0000 00da 0f51 416e  .N..).r......QAn
-00000370: 696d 6174 696f 6e47 726f 7570 da08 5f5f  imationGroup..__
-00000380: 696e 6974 5f5f da05 7375 7065 72a9 03da  init__..super...
-00000390: 0473 656c 66da 0461 7267 73da 066b 7761  .self..args..kwa
-000003a0: 7267 73a9 01da 095f 5f63 6c61 7373 5f5f  rgs....__class__
-000003b0: 7209 0000 00fa 562f 686f 6d65 2f6f 7361  r.....V/home/osa
-000003c0: 6d61 2f57 6f72 6b73 7061 6365 2f2e 7665  ma/Workspace/.ve
-000003d0: 6e76 2f6c 6962 2f70 7974 686f 6e33 2e31  nv/lib/python3.1
-000003e0: 302f 7369 7465 2d70 6163 6b61 6765 732f  0/site-packages/
-000003f0: 5174 6963 612f 746f 6f6c 732f 7174 636f  Qtica/tools/qtco
-00000400: 7265 2f6f 626a 6563 7473 2e70 7972 0b00  re/objects.pyr..
-00000410: 0000 0800 0000 f304 0000 0014 0116 017a  ...............z
-00000420: 1741 6e69 6d61 7469 6f6e 4772 6f75 702e  .AnimationGroup.
-00000430: 5f5f 696e 6974 5f5f a905 da08 5f5f 6e61  __init__....__na
-00000440: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000450: da0c 5f5f 7175 616c 6e61 6d65 5f5f 720b  ..__qualname__r.
-00000460: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-00000470: 5f5f 7209 0000 0072 0900 0000 7211 0000  __r....r....r...
-00000480: 0072 1300 0000 7206 0000 0007 0000 00f3  .r....r.........
-00000490: 0400 0000 0800 1401 7206 0000 0063 0000  ........r....c..
-000004a0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-000004b0: 0000 0000 0000 7205 0000 0029 03da 0642  ......r....)...B
-000004c0: 7566 6665 7263 0100 0000 0000 0000 0000  ufferc..........
-000004d0: 0000 0300 0000 0400 0000 0f00 0000 7207  ..............r.
-000004e0: 0000 0072 0800 0000 2904 7202 0000 00da  ...r....).r.....
-000004f0: 0751 4275 6666 6572 720b 0000 0072 0c00  .QBufferr....r..
-00000500: 0000 720d 0000 0072 1100 0000 7209 0000  ..r....r....r...
-00000510: 0072 1300 0000 720b 0000 000e 0000 0072  .r....r........r
-00000520: 1400 0000 7a0f 4275 6666 6572 2e5f 5f69  ....z.Buffer.__i
-00000530: 6e69 745f 5f72 1500 0000 7209 0000 0072  nit__r....r....r
-00000540: 0900 0000 7211 0000 0072 1300 0000 721b  ....r....r....r.
-00000550: 0000 000d 0000 0072 1a00 0000 721b 0000  .......r....r...
-00000560: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000570: 0000 0300 0000 0000 0000 7205 0000 0029  ..........r....)
-00000580: 03da 1b43 6f6e 6361 7465 6e61 7465 5461  ...ConcatenateTa
-00000590: 626c 6573 5072 6f78 794d 6f64 656c 6301  blesProxyModelc.
-000005a0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-000005b0: 0000 000f 0000 0072 0700 0000 7208 0000  .......r....r...
-000005c0: 0029 0472 0200 0000 da1c 5143 6f6e 6361  .).r......QConca
-000005d0: 7465 6e61 7465 5461 626c 6573 5072 6f78  tenateTablesProx
-000005e0: 794d 6f64 656c 720b 0000 0072 0c00 0000  yModelr....r....
-000005f0: 720d 0000 0072 1100 0000 7209 0000 0072  r....r....r....r
-00000600: 1300 0000 720b 0000 0014 0000 0072 1400  ....r........r..
-00000610: 0000 7a24 436f 6e63 6174 656e 6174 6554  ..z$ConcatenateT
-00000620: 6162 6c65 7350 726f 7879 4d6f 6465 6c2e  ablesProxyModel.
-00000630: 5f5f 696e 6974 5f5f 7215 0000 0072 0900  __init__r....r..
-00000640: 0000 7209 0000 0072 1100 0000 7213 0000  ..r....r....r...
-00000650: 0072 1d00 0000 1300 0000 721a 0000 0072  .r........r....r
-00000660: 1d00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000670: 0000 0000 0003 0000 0000 0000 0072 0500  .............r..
-00000680: 0000 2903 da0f 436f 7265 4170 706c 6963  ..)...CoreApplic
-00000690: 6174 696f 6e63 0100 0000 0000 0000 0000  ationc..........
-000006a0: 0000 0300 0000 0400 0000 0f00 0000 7207  ..............r.
-000006b0: 0000 0072 0800 0000 2904 7202 0000 00da  ...r....).r.....
-000006c0: 1051 436f 7265 4170 706c 6963 6174 696f  .QCoreApplicatio
-000006d0: 6e72 0b00 0000 720c 0000 0072 0d00 0000  nr....r....r....
-000006e0: 7211 0000 0072 0900 0000 7213 0000 0072  r....r....r....r
-000006f0: 0b00 0000 1a00 0000 7214 0000 007a 1843  ........r....z.C
-00000700: 6f72 6541 7070 6c69 6361 7469 6f6e 2e5f  oreApplication._
-00000710: 5f69 6e69 745f 5f72 1500 0000 7209 0000  _init__r....r...
-00000720: 0072 0900 0000 7211 0000 0072 1300 0000  .r....r....r....
-00000730: 721f 0000 0019 0000 0072 1a00 0000 721f  r........r....r.
-00000740: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000750: 0000 0000 0300 0000 0000 0000 7205 0000  ............r...
-00000760: 0029 03da 0945 7665 6e74 4c6f 6f70 6301  .)...EventLoopc.
-00000770: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-00000780: 0000 000f 0000 0072 0700 0000 7208 0000  .......r....r...
-00000790: 0029 0472 0200 0000 da0a 5145 7665 6e74  .).r......QEvent
-000007a0: 4c6f 6f70 720b 0000 0072 0c00 0000 720d  Loopr....r....r.
-000007b0: 0000 0072 1100 0000 7209 0000 0072 1300  ...r....r....r..
-000007c0: 0000 720b 0000 0020 0000 0072 1400 0000  ..r.... ...r....
-000007d0: 7a12 4576 656e 744c 6f6f 702e 5f5f 696e  z.EventLoop.__in
-000007e0: 6974 5f5f 7215 0000 0072 0900 0000 7209  it__r....r....r.
-000007f0: 0000 0072 1100 0000 7213 0000 0072 2100  ...r....r....r!.
-00000800: 0000 1f00 0000 721a 0000 0072 2100 0000  ......r....r!...
-00000810: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000820: 0003 0000 0000 0000 0072 0500 0000 2903  .........r....).
-00000830: da0a 4669 6c65 4465 7669 6365 6301 0000  ..FileDevicec...
-00000840: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00000850: 000f 0000 0072 0700 0000 7208 0000 0029  .....r....r....)
-00000860: 0472 0200 0000 da0b 5146 696c 6544 6576  .r......QFileDev
-00000870: 6963 6572 0b00 0000 720c 0000 0072 0d00  icer....r....r..
-00000880: 0000 7211 0000 0072 0900 0000 7213 0000  ..r....r....r...
-00000890: 0072 0b00 0000 2600 0000 7214 0000 007a  .r....&...r....z
-000008a0: 1346 696c 6544 6576 6963 652e 5f5f 696e  .FileDevice.__in
-000008b0: 6974 5f5f 7215 0000 0072 0900 0000 7209  it__r....r....r.
-000008c0: 0000 0072 1100 0000 7213 0000 0072 2300  ...r....r....r#.
-000008d0: 0000 2500 0000 721a 0000 0072 2300 0000  ..%...r....r#...
-000008e0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000008f0: 0003 0000 0000 0000 0072 0500 0000 2903  .........r....).
-00000900: da0c 4669 6c65 5365 6c65 6374 6f72 6301  ..FileSelectorc.
+00000290: 8400 643f 6503 6501 6a3e 8304 5a3f 4700  ..d?e.e.j>..Z?G.
+000002a0: 6440 6441 8400 6441 6503 6501 6a40 8304  d@dA..dAe.e.j@..
+000002b0: 5a41 6442 5300 2943 e900 0000 0029 01da  ZAdBS.)C.....)..
+000002c0: 0651 7443 6f72 65e9 0300 0000 2901 da0f  .QtCore.....)...
+000002d0: 4162 7374 7261 6374 514f 626a 6563 7463  AbstractQObjectc
+000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002f0: 0300 0000 0000 0000 f31c 0000 0065 005a  .............e.Z
+00000300: 0164 005a 0287 0066 0164 0164 0284 085a  .d.Z...f.d.d...Z
+00000310: 0387 0004 005a 0453 0029 03da 0e41 6e69  .....Z.S.)...Ani
+00000320: 6d61 7469 6f6e 4772 6f75 7063 0100 0000  mationGroupc....
+00000330: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00000340: 0f00 0000 f32a 0000 0074 006a 016a 027c  .....*...t.j.j.|
+00000350: 0067 017c 01a2 0152 008e 0001 0074 0383  .g.|...R.....t..
+00000360: 006a 0264 0169 007c 02a4 018e 0101 0064  .j.d.i.|.......d
+00000370: 0053 00a9 024e a900 2904 7202 0000 00da  .S...N..).r.....
+00000380: 0f51 416e 696d 6174 696f 6e47 726f 7570  .QAnimationGroup
+00000390: da08 5f5f 696e 6974 5f5f da05 7375 7065  ..__init__..supe
+000003a0: 72a9 03da 0473 656c 66da 0461 7267 73da  r....self..args.
+000003b0: 066b 7761 7267 73a9 01da 095f 5f63 6c61  .kwargs....__cla
+000003c0: 7373 5f5f 7209 0000 00fa 562f 686f 6d65  ss__r.....V/home
+000003d0: 2f6f 7361 6d61 2f57 6f72 6b73 7061 6365  /osama/Workspace
+000003e0: 2f2e 7665 6e76 2f6c 6962 2f70 7974 686f  /.venv/lib/pytho
+000003f0: 6e33 2e31 302f 7369 7465 2d70 6163 6b61  n3.10/site-packa
+00000400: 6765 732f 5174 6963 612f 746f 6f6c 732f  ges/Qtica/tools/
+00000410: 7174 636f 7265 2f6f 626a 6563 7473 2e70  qtcore/objects.p
+00000420: 7972 0b00 0000 0800 0000 f304 0000 0014  yr..............
+00000430: 0116 017a 1741 6e69 6d61 7469 6f6e 4772  ...z.AnimationGr
+00000440: 6f75 702e 5f5f 696e 6974 5f5f a905 da08  oup.__init__....
+00000450: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000460: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000470: 5f5f 720b 0000 00da 0d5f 5f63 6c61 7373  __r......__class
+00000480: 6365 6c6c 5f5f 7209 0000 0072 0900 0000  cell__r....r....
+00000490: 7211 0000 0072 1300 0000 7206 0000 0007  r....r....r.....
+000004a0: 0000 00f3 0400 0000 0800 1401 7206 0000  ............r...
+000004b0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+000004c0: 0000 0300 0000 0000 0000 7205 0000 0029  ..........r....)
+000004d0: 03da 0642 7566 6665 7263 0100 0000 0000  ...Bufferc......
+000004e0: 0000 0000 0000 0300 0000 0400 0000 0f00  ................
+000004f0: 0000 7207 0000 0072 0800 0000 2904 7202  ..r....r....).r.
+00000500: 0000 00da 0751 4275 6666 6572 720b 0000  .....QBufferr...
+00000510: 0072 0c00 0000 720d 0000 0072 1100 0000  .r....r....r....
+00000520: 7209 0000 0072 1300 0000 720b 0000 000e  r....r....r.....
+00000530: 0000 0072 1400 0000 7a0f 4275 6666 6572  ...r....z.Buffer
+00000540: 2e5f 5f69 6e69 745f 5f72 1500 0000 7209  .__init__r....r.
+00000550: 0000 0072 0900 0000 7211 0000 0072 1300  ...r....r....r..
+00000560: 0000 721b 0000 000d 0000 0072 1a00 0000  ..r........r....
+00000570: 721b 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000580: 0000 0000 0000 0300 0000 0000 0000 7205  ..............r.
+00000590: 0000 0029 03da 1b43 6f6e 6361 7465 6e61  ...)...Concatena
+000005a0: 7465 5461 626c 6573 5072 6f78 794d 6f64  teTablesProxyMod
+000005b0: 656c 6301 0000 0000 0000 0000 0000 0003  elc.............
+000005c0: 0000 0004 0000 000f 0000 0072 0700 0000  ...........r....
+000005d0: 7208 0000 0029 0472 0200 0000 da1c 5143  r....).r......QC
+000005e0: 6f6e 6361 7465 6e61 7465 5461 626c 6573  oncatenateTables
+000005f0: 5072 6f78 794d 6f64 656c 720b 0000 0072  ProxyModelr....r
+00000600: 0c00 0000 720d 0000 0072 1100 0000 7209  ....r....r....r.
+00000610: 0000 0072 1300 0000 720b 0000 0014 0000  ...r....r.......
+00000620: 0072 1400 0000 7a24 436f 6e63 6174 656e  .r....z$Concaten
+00000630: 6174 6554 6162 6c65 7350 726f 7879 4d6f  ateTablesProxyMo
+00000640: 6465 6c2e 5f5f 696e 6974 5f5f 7215 0000  del.__init__r...
+00000650: 0072 0900 0000 7209 0000 0072 1100 0000  .r....r....r....
+00000660: 7213 0000 0072 1d00 0000 1300 0000 721a  r....r........r.
+00000670: 0000 0072 1d00 0000 6300 0000 0000 0000  ...r....c.......
+00000680: 0000 0000 0000 0000 0003 0000 0000 0000  ................
+00000690: 0072 0500 0000 2903 da0f 436f 7265 4170  .r....)...CoreAp
+000006a0: 706c 6963 6174 696f 6e63 0100 0000 0000  plicationc......
+000006b0: 0000 0000 0000 0300 0000 0400 0000 0f00  ................
+000006c0: 0000 7207 0000 0072 0800 0000 2904 7202  ..r....r....).r.
+000006d0: 0000 00da 1051 436f 7265 4170 706c 6963  .....QCoreApplic
+000006e0: 6174 696f 6e72 0b00 0000 720c 0000 0072  ationr....r....r
+000006f0: 0d00 0000 7211 0000 0072 0900 0000 7213  ....r....r....r.
+00000700: 0000 0072 0b00 0000 1a00 0000 7214 0000  ...r........r...
+00000710: 007a 1843 6f72 6541 7070 6c69 6361 7469  .z.CoreApplicati
+00000720: 6f6e 2e5f 5f69 6e69 745f 5f72 1500 0000  on.__init__r....
+00000730: 7209 0000 0072 0900 0000 7211 0000 0072  r....r....r....r
+00000740: 1300 0000 721f 0000 0019 0000 0072 1a00  ....r........r..
+00000750: 0000 721f 0000 0063 0000 0000 0000 0000  ..r....c........
+00000760: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+00000770: 7205 0000 0029 03da 0945 7665 6e74 4c6f  r....)...EventLo
+00000780: 6f70 6301 0000 0000 0000 0000 0000 0003  opc.............
+00000790: 0000 0004 0000 000f 0000 0072 0700 0000  ...........r....
+000007a0: 7208 0000 0029 0472 0200 0000 da0a 5145  r....).r......QE
+000007b0: 7665 6e74 4c6f 6f70 720b 0000 0072 0c00  ventLoopr....r..
+000007c0: 0000 720d 0000 0072 1100 0000 7209 0000  ..r....r....r...
+000007d0: 0072 1300 0000 720b 0000 0020 0000 0072  .r....r.... ...r
+000007e0: 1400 0000 7a12 4576 656e 744c 6f6f 702e  ....z.EventLoop.
+000007f0: 5f5f 696e 6974 5f5f 7215 0000 0072 0900  __init__r....r..
+00000800: 0000 7209 0000 0072 1100 0000 7213 0000  ..r....r....r...
+00000810: 0072 2100 0000 1f00 0000 721a 0000 0072  .r!.......r....r
+00000820: 2100 0000 6300 0000 0000 0000 0000 0000  !...c...........
+00000830: 0000 0000 0003 0000 0000 0000 0072 0500  .............r..
+00000840: 0000 2903 da04 4669 6c65 6301 0000 0000  ..)...Filec.....
+00000850: 0000 0000 0000 0003 0000 0004 0000 000f  ................
+00000860: 0000 0072 0700 0000 7208 0000 0029 0472  ...r....r....).r
+00000870: 0200 0000 da05 5146 696c 6572 0b00 0000  ......QFiler....
+00000880: 720c 0000 0072 0d00 0000 7211 0000 0072  r....r....r....r
+00000890: 0900 0000 7213 0000 0072 0b00 0000 2600  ....r....r....&.
+000008a0: 0000 7214 0000 007a 0d46 696c 652e 5f5f  ..r....z.File.__
+000008b0: 696e 6974 5f5f 7215 0000 0072 0900 0000  init__r....r....
+000008c0: 7209 0000 0072 1100 0000 7213 0000 0072  r....r....r....r
+000008d0: 2300 0000 2500 0000 721a 0000 0072 2300  #...%...r....r#.
+000008e0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000008f0: 0000 0003 0000 0000 0000 0072 0500 0000  ...........r....
+00000900: 2903 da0a 4669 6c65 4465 7669 6365 6301  )...FileDevicec.
 00000910: 0000 0000 0000 0000 0000 0003 0000 0004  ................
 00000920: 0000 000f 0000 0072 0700 0000 7208 0000  .......r....r...
-00000930: 0029 0472 0200 0000 da0d 5146 696c 6553  .).r......QFileS
-00000940: 656c 6563 746f 7272 0b00 0000 720c 0000  electorr....r...
-00000950: 0072 0d00 0000 7211 0000 0072 0900 0000  .r....r....r....
-00000960: 7213 0000 0072 0b00 0000 2c00 0000 7214  r....r....,...r.
-00000970: 0000 007a 1546 696c 6553 656c 6563 746f  ...z.FileSelecto
-00000980: 722e 5f5f 696e 6974 5f5f 7215 0000 0072  r.__init__r....r
-00000990: 0900 0000 7209 0000 0072 1100 0000 7213  ....r....r....r.
-000009a0: 0000 0072 2500 0000 2b00 0000 721a 0000  ...r%...+...r...
-000009b0: 0072 2500 0000 6300 0000 0000 0000 0000  .r%...c.........
-000009c0: 0000 0000 0000 0003 0000 0000 0000 0072  ...............r
-000009d0: 0500 0000 2903 da11 4669 6c65 5379 7374  ....)...FileSyst
-000009e0: 656d 5761 7463 6865 7263 0100 0000 0000  emWatcherc......
-000009f0: 0000 0000 0000 0300 0000 0400 0000 0f00  ................
-00000a00: 0000 7207 0000 0072 0800 0000 2904 7202  ..r....r....).r.
-00000a10: 0000 00da 1251 4669 6c65 5379 7374 656d  .....QFileSystem
-00000a20: 5761 7463 6865 7272 0b00 0000 720c 0000  Watcherr....r...
-00000a30: 0072 0d00 0000 7211 0000 0072 0900 0000  .r....r....r....
-00000a40: 7213 0000 0072 0b00 0000 3200 0000 7214  r....r....2...r.
-00000a50: 0000 007a 1a46 696c 6553 7973 7465 6d57  ...z.FileSystemW
-00000a60: 6174 6368 6572 2e5f 5f69 6e69 745f 5f72  atcher.__init__r
-00000a70: 1500 0000 7209 0000 0072 0900 0000 7211  ....r....r....r.
-00000a80: 0000 0072 1300 0000 7227 0000 0031 0000  ...r....r'...1..
-00000a90: 0072 1a00 0000 7227 0000 0063 0000 0000  .r....r'...c....
-00000aa0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00000ab0: 0000 0000 7205 0000 0029 03da 0849 4f44  ....r....)...IOD
-00000ac0: 6576 6963 6563 0100 0000 0000 0000 0000  evicec..........
-00000ad0: 0000 0300 0000 0400 0000 0f00 0000 7207  ..............r.
-00000ae0: 0000 0072 0800 0000 2904 7202 0000 00da  ...r....).r.....
-00000af0: 0951 494f 4465 7669 6365 720b 0000 0072  .QIODevicer....r
-00000b00: 0c00 0000 720d 0000 0072 1100 0000 7209  ....r....r....r.
-00000b10: 0000 0072 1300 0000 720b 0000 0038 0000  ...r....r....8..
-00000b20: 0072 1400 0000 7a11 494f 4465 7669 6365  .r....z.IODevice
-00000b30: 2e5f 5f69 6e69 745f 5f72 1500 0000 7209  .__init__r....r.
-00000b40: 0000 0072 0900 0000 7211 0000 0072 1300  ...r....r....r..
-00000b50: 0000 7229 0000 0037 0000 0072 1a00 0000  ..r)...7...r....
-00000b60: 7229 0000 0063 0000 0000 0000 0000 0000  r)...c..........
-00000b70: 0000 0000 0000 0300 0000 0000 0000 7205  ..............r.
-00000b80: 0000 0029 03da 1249 6465 6e74 6974 7950  ...)...IdentityP
-00000b90: 726f 7879 4d6f 6465 6c63 0100 0000 0000  roxyModelc......
-00000ba0: 0000 0000 0000 0300 0000 0400 0000 0f00  ................
-00000bb0: 0000 7207 0000 0072 0800 0000 2904 7202  ..r....r....).r.
-00000bc0: 0000 00da 1351 4964 656e 7469 7479 5072  .....QIdentityPr
-00000bd0: 6f78 794d 6f64 656c 720b 0000 0072 0c00  oxyModelr....r..
-00000be0: 0000 720d 0000 0072 1100 0000 7209 0000  ..r....r....r...
-00000bf0: 0072 1300 0000 720b 0000 003e 0000 0072  .r....r....>...r
-00000c00: 1400 0000 7a1b 4964 656e 7469 7479 5072  ....z.IdentityPr
-00000c10: 6f78 794d 6f64 656c 2e5f 5f69 6e69 745f  oxyModel.__init_
-00000c20: 5f72 1500 0000 7209 0000 0072 0900 0000  _r....r....r....
-00000c30: 7211 0000 0072 1300 0000 722b 0000 003d  r....r....r+...=
-00000c40: 0000 0072 1a00 0000 722b 0000 0063 0000  ...r....r+...c..
-00000c50: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00000c60: 0000 0000 0000 7205 0000 0029 03da 1249  ......r....)...I
-00000c70: 7465 6d53 656c 6563 7469 6f6e 4d6f 6465  temSelectionMode
-00000c80: 6c63 0100 0000 0000 0000 0000 0000 0300  lc..............
-00000c90: 0000 0400 0000 0f00 0000 7207 0000 0072  ..........r....r
-00000ca0: 0800 0000 2904 7202 0000 00da 1351 4974  ....).r......QIt
-00000cb0: 656d 5365 6c65 6374 696f 6e4d 6f64 656c  emSelectionModel
-00000cc0: 720b 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
-00000cd0: 1100 0000 7209 0000 0072 1300 0000 720b  ....r....r....r.
-00000ce0: 0000 0044 0000 0072 1400 0000 7a1b 4974  ...D...r....z.It
-00000cf0: 656d 5365 6c65 6374 696f 6e4d 6f64 656c  emSelectionModel
-00000d00: 2e5f 5f69 6e69 745f 5f72 1500 0000 7209  .__init__r....r.
-00000d10: 0000 0072 0900 0000 7211 0000 0072 1300  ...r....r....r..
-00000d20: 0000 722d 0000 0043 0000 0072 1a00 0000  ..r-...C...r....
-00000d30: 722d 0000 0063 0000 0000 0000 0000 0000  r-...c..........
-00000d40: 0000 0000 0000 0300 0000 0000 0000 7205  ..............r.
-00000d50: 0000 0029 03da 074c 6962 7261 7279 6301  ...)...Libraryc.
-00000d60: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-00000d70: 0000 000f 0000 0072 0700 0000 7208 0000  .......r....r...
-00000d80: 0029 0472 0200 0000 da08 514c 6962 7261  .).r......QLibra
-00000d90: 7279 720b 0000 0072 0c00 0000 720d 0000  ryr....r....r...
+00000930: 0029 0472 0200 0000 da0b 5146 696c 6544  .).r......QFileD
+00000940: 6576 6963 6572 0b00 0000 720c 0000 0072  evicer....r....r
+00000950: 0d00 0000 7211 0000 0072 0900 0000 7213  ....r....r....r.
+00000960: 0000 0072 0b00 0000 2c00 0000 7214 0000  ...r....,...r...
+00000970: 007a 1346 696c 6544 6576 6963 652e 5f5f  .z.FileDevice.__
+00000980: 696e 6974 5f5f 7215 0000 0072 0900 0000  init__r....r....
+00000990: 7209 0000 0072 1100 0000 7213 0000 0072  r....r....r....r
+000009a0: 2500 0000 2b00 0000 721a 0000 0072 2500  %...+...r....r%.
+000009b0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000009c0: 0000 0003 0000 0000 0000 0072 0500 0000  ...........r....
+000009d0: 2903 da0c 4669 6c65 5365 6c65 6374 6f72  )...FileSelector
+000009e0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+000009f0: 0004 0000 000f 0000 0072 0700 0000 7208  .........r....r.
+00000a00: 0000 0029 0472 0200 0000 da0d 5146 696c  ...).r......QFil
+00000a10: 6553 656c 6563 746f 7272 0b00 0000 720c  eSelectorr....r.
+00000a20: 0000 0072 0d00 0000 7211 0000 0072 0900  ...r....r....r..
+00000a30: 0000 7213 0000 0072 0b00 0000 3200 0000  ..r....r....2...
+00000a40: 7214 0000 007a 1546 696c 6553 656c 6563  r....z.FileSelec
+00000a50: 746f 722e 5f5f 696e 6974 5f5f 7215 0000  tor.__init__r...
+00000a60: 0072 0900 0000 7209 0000 0072 1100 0000  .r....r....r....
+00000a70: 7213 0000 0072 2700 0000 3100 0000 721a  r....r'...1...r.
+00000a80: 0000 0072 2700 0000 6300 0000 0000 0000  ...r'...c.......
+00000a90: 0000 0000 0000 0000 0003 0000 0000 0000  ................
+00000aa0: 0072 0500 0000 2903 da11 4669 6c65 5379  .r....)...FileSy
+00000ab0: 7374 656d 5761 7463 6865 7263 0100 0000  stemWatcherc....
+00000ac0: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00000ad0: 0f00 0000 7207 0000 0072 0800 0000 2904  ....r....r....).
+00000ae0: 7202 0000 00da 1251 4669 6c65 5379 7374  r......QFileSyst
+00000af0: 656d 5761 7463 6865 7272 0b00 0000 720c  emWatcherr....r.
+00000b00: 0000 0072 0d00 0000 7211 0000 0072 0900  ...r....r....r..
+00000b10: 0000 7213 0000 0072 0b00 0000 3800 0000  ..r....r....8...
+00000b20: 7214 0000 007a 1a46 696c 6553 7973 7465  r....z.FileSyste
+00000b30: 6d57 6174 6368 6572 2e5f 5f69 6e69 745f  mWatcher.__init_
+00000b40: 5f72 1500 0000 7209 0000 0072 0900 0000  _r....r....r....
+00000b50: 7211 0000 0072 1300 0000 7229 0000 0037  r....r....r)...7
+00000b60: 0000 0072 1a00 0000 7229 0000 0063 0000  ...r....r)...c..
+00000b70: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+00000b80: 0000 0000 0000 7205 0000 0029 03da 0849  ......r....)...I
+00000b90: 4f44 6576 6963 6563 0100 0000 0000 0000  ODevicec........
+00000ba0: 0000 0000 0300 0000 0400 0000 0f00 0000  ................
+00000bb0: 7207 0000 0072 0800 0000 2904 7202 0000  r....r....).r...
+00000bc0: 00da 0951 494f 4465 7669 6365 720b 0000  ...QIODevicer...
+00000bd0: 0072 0c00 0000 720d 0000 0072 1100 0000  .r....r....r....
+00000be0: 7209 0000 0072 1300 0000 720b 0000 003e  r....r....r....>
+00000bf0: 0000 0072 1400 0000 7a11 494f 4465 7669  ...r....z.IODevi
+00000c00: 6365 2e5f 5f69 6e69 745f 5f72 1500 0000  ce.__init__r....
+00000c10: 7209 0000 0072 0900 0000 7211 0000 0072  r....r....r....r
+00000c20: 1300 0000 722b 0000 003d 0000 0072 1a00  ....r+...=...r..
+00000c30: 0000 722b 0000 0063 0000 0000 0000 0000  ..r+...c........
+00000c40: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+00000c50: 7205 0000 0029 03da 1249 6465 6e74 6974  r....)...Identit
+00000c60: 7950 726f 7879 4d6f 6465 6c63 0100 0000  yProxyModelc....
+00000c70: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00000c80: 0f00 0000 7207 0000 0072 0800 0000 2904  ....r....r....).
+00000c90: 7202 0000 00da 1351 4964 656e 7469 7479  r......QIdentity
+00000ca0: 5072 6f78 794d 6f64 656c 720b 0000 0072  ProxyModelr....r
+00000cb0: 0c00 0000 720d 0000 0072 1100 0000 7209  ....r....r....r.
+00000cc0: 0000 0072 1300 0000 720b 0000 0044 0000  ...r....r....D..
+00000cd0: 0072 1400 0000 7a1b 4964 656e 7469 7479  .r....z.Identity
+00000ce0: 5072 6f78 794d 6f64 656c 2e5f 5f69 6e69  ProxyModel.__ini
+00000cf0: 745f 5f72 1500 0000 7209 0000 0072 0900  t__r....r....r..
+00000d00: 0000 7211 0000 0072 1300 0000 722d 0000  ..r....r....r-..
+00000d10: 0043 0000 0072 1a00 0000 722d 0000 0063  .C...r....r-...c
+00000d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000d30: 0300 0000 0000 0000 7205 0000 0029 03da  ........r....)..
+00000d40: 1249 7465 6d53 656c 6563 7469 6f6e 4d6f  .ItemSelectionMo
+00000d50: 6465 6c63 0100 0000 0000 0000 0000 0000  delc............
+00000d60: 0300 0000 0400 0000 0f00 0000 7207 0000  ............r...
+00000d70: 0072 0800 0000 2904 7202 0000 00da 1351  .r....).r......Q
+00000d80: 4974 656d 5365 6c65 6374 696f 6e4d 6f64  ItemSelectionMod
+00000d90: 656c 720b 0000 0072 0c00 0000 720d 0000  elr....r....r...
 00000da0: 0072 1100 0000 7209 0000 0072 1300 0000  .r....r....r....
-00000db0: 720b 0000 004a 0000 0072 1400 0000 7a10  r....J...r....z.
-00000dc0: 4c69 6272 6172 792e 5f5f 696e 6974 5f5f  Library.__init__
-00000dd0: 7215 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
-00000de0: 1100 0000 7213 0000 0072 2f00 0000 4900  ....r....r/...I.
-00000df0: 0000 721a 0000 0072 2f00 0000 6300 0000  ..r....r/...c...
-00000e00: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00000e10: 0000 0000 0072 0500 0000 2903 da08 4d69  .....r....)...Mi
-00000e20: 6d65 4461 7461 6301 0000 0000 0000 0000  meDatac.........
-00000e30: 0000 0003 0000 0004 0000 000f 0000 0072  ...............r
-00000e40: 0700 0000 7208 0000 0029 0472 0200 0000  ....r....).r....
-00000e50: da09 514d 696d 6544 6174 6172 0b00 0000  ..QMimeDatar....
-00000e60: 720c 0000 0072 0d00 0000 7211 0000 0072  r....r....r....r
-00000e70: 0900 0000 7213 0000 0072 0b00 0000 5000  ....r....r....P.
-00000e80: 0000 7214 0000 007a 114d 696d 6544 6174  ..r....z.MimeDat
-00000e90: 612e 5f5f 696e 6974 5f5f 7215 0000 0072  a.__init__r....r
-00000ea0: 0900 0000 7209 0000 0072 1100 0000 7213  ....r....r....r.
-00000eb0: 0000 0072 3100 0000 4f00 0000 721a 0000  ...r1...O...r...
-00000ec0: 0072 3100 0000 6300 0000 0000 0000 0000  .r1...c.........
-00000ed0: 0000 0000 0000 0003 0000 0000 0000 0072  ...............r
-00000ee0: 0500 0000 2903 da0e 5061 7573 6541 6e69  ....)...PauseAni
-00000ef0: 6d61 7469 6f6e 6301 0000 0000 0000 0000  mationc.........
-00000f00: 0000 0003 0000 0004 0000 000f 0000 0072  ...............r
-00000f10: 0700 0000 7208 0000 0029 0472 0200 0000  ....r....).r....
-00000f20: da0f 5150 6175 7365 416e 696d 6174 696f  ..QPauseAnimatio
-00000f30: 6e72 0b00 0000 720c 0000 0072 0d00 0000  nr....r....r....
-00000f40: 7211 0000 0072 0900 0000 7213 0000 0072  r....r....r....r
-00000f50: 0b00 0000 5600 0000 7214 0000 007a 1750  ....V...r....z.P
-00000f60: 6175 7365 416e 696d 6174 696f 6e2e 5f5f  auseAnimation.__
-00000f70: 696e 6974 5f5f 7215 0000 0072 0900 0000  init__r....r....
-00000f80: 7209 0000 0072 1100 0000 7213 0000 0072  r....r....r....r
-00000f90: 3300 0000 5500 0000 721a 0000 0072 3300  3...U...r....r3.
-00000fa0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000fb0: 0000 0003 0000 0000 0000 0072 0500 0000  ...........r....
-00000fc0: 2903 da0c 506c 7567 696e 4c6f 6164 6572  )...PluginLoader
-00000fd0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00000fe0: 0004 0000 000f 0000 0072 0700 0000 7208  .........r....r.
-00000ff0: 0000 0029 0472 0200 0000 da0d 5150 6c75  ...).r......QPlu
-00001000: 6769 6e4c 6f61 6465 7272 0b00 0000 720c  ginLoaderr....r.
-00001010: 0000 0072 0d00 0000 7211 0000 0072 0900  ...r....r....r..
-00001020: 0000 7213 0000 0072 0b00 0000 5c00 0000  ..r....r....\...
-00001030: 7214 0000 007a 1550 6c75 6769 6e4c 6f61  r....z.PluginLoa
-00001040: 6465 722e 5f5f 696e 6974 5f5f 7215 0000  der.__init__r...
-00001050: 0072 0900 0000 7209 0000 0072 1100 0000  .r....r....r....
-00001060: 7213 0000 0072 3500 0000 5b00 0000 721a  r....r5...[...r.
-00001070: 0000 0072 3500 0000 6300 0000 0000 0000  ...r5...c.......
-00001080: 0000 0000 0000 0000 0003 0000 0000 0000  ................
-00001090: 0072 0500 0000 2903 da07 5072 6f63 6573  .r....)...Proces
-000010a0: 7363 0100 0000 0000 0000 0000 0000 0300  sc..............
-000010b0: 0000 0400 0000 0f00 0000 7207 0000 0072  ..........r....r
-000010c0: 0800 0000 2904 7202 0000 00da 0851 5072  ....).r......QPr
-000010d0: 6f63 6573 7372 0b00 0000 720c 0000 0072  ocessr....r....r
-000010e0: 0d00 0000 7211 0000 0072 0900 0000 7213  ....r....r....r.
-000010f0: 0000 0072 0b00 0000 6200 0000 7214 0000  ...r....b...r...
-00001100: 007a 1050 726f 6365 7373 2e5f 5f69 6e69  .z.Process.__ini
-00001110: 745f 5f72 1500 0000 7209 0000 0072 0900  t__r....r....r..
-00001120: 0000 7211 0000 0072 1300 0000 7237 0000  ..r....r....r7..
-00001130: 0061 0000 0072 1a00 0000 7237 0000 0063  .a...r....r7...c
-00001140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001150: 0300 0000 0000 0000 7205 0000 0029 03da  ........r....)..
-00001160: 0853 6176 6546 696c 6563 0100 0000 0000  .SaveFilec......
-00001170: 0000 0000 0000 0300 0000 0400 0000 0f00  ................
-00001180: 0000 7207 0000 0072 0800 0000 2904 7202  ..r....r....).r.
-00001190: 0000 00da 0951 5361 7665 4669 6c65 720b  .....QSaveFiler.
-000011a0: 0000 0072 0c00 0000 720d 0000 0072 1100  ...r....r....r..
-000011b0: 0000 7209 0000 0072 1300 0000 720b 0000  ..r....r....r...
-000011c0: 0068 0000 0072 1400 0000 7a11 5361 7665  .h...r....z.Save
-000011d0: 4669 6c65 2e5f 5f69 6e69 745f 5f72 1500  File.__init__r..
-000011e0: 0000 7209 0000 0072 0900 0000 7211 0000  ..r....r....r...
-000011f0: 0072 1300 0000 7239 0000 0067 0000 0072  .r....r9...g...r
-00001200: 1a00 0000 7239 0000 0063 0000 0000 0000  ....r9...c......
-00001210: 0000 0000 0000 0000 0000 0300 0000 0000  ................
-00001220: 0000 7205 0000 0029 03da 0c53 6861 7265  ..r....)...Share
-00001230: 644d 656d 6f72 7963 0100 0000 0000 0000  dMemoryc........
-00001240: 0000 0000 0300 0000 0400 0000 0f00 0000  ................
-00001250: 7207 0000 0072 0800 0000 2904 7202 0000  r....r....).r...
-00001260: 00da 0d51 5368 6172 6564 4d65 6d6f 7279  ...QSharedMemory
+00000db0: 720b 0000 004a 0000 0072 1400 0000 7a1b  r....J...r....z.
+00000dc0: 4974 656d 5365 6c65 6374 696f 6e4d 6f64  ItemSelectionMod
+00000dd0: 656c 2e5f 5f69 6e69 745f 5f72 1500 0000  el.__init__r....
+00000de0: 7209 0000 0072 0900 0000 7211 0000 0072  r....r....r....r
+00000df0: 1300 0000 722f 0000 0049 0000 0072 1a00  ....r/...I...r..
+00000e00: 0000 722f 0000 0063 0000 0000 0000 0000  ..r/...c........
+00000e10: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+00000e20: 7205 0000 0029 03da 074c 6962 7261 7279  r....)...Library
+00000e30: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00000e40: 0004 0000 000f 0000 0072 0700 0000 7208  .........r....r.
+00000e50: 0000 0029 0472 0200 0000 da08 514c 6962  ...).r......QLib
+00000e60: 7261 7279 720b 0000 0072 0c00 0000 720d  raryr....r....r.
+00000e70: 0000 0072 1100 0000 7209 0000 0072 1300  ...r....r....r..
+00000e80: 0000 720b 0000 0050 0000 0072 1400 0000  ..r....P...r....
+00000e90: 7a10 4c69 6272 6172 792e 5f5f 696e 6974  z.Library.__init
+00000ea0: 5f5f 7215 0000 0072 0900 0000 7209 0000  __r....r....r...
+00000eb0: 0072 1100 0000 7213 0000 0072 3100 0000  .r....r....r1...
+00000ec0: 4f00 0000 721a 0000 0072 3100 0000 6300  O...r....r1...c.
+00000ed0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000ee0: 0000 0000 0000 0072 0500 0000 2903 da08  .......r....)...
+00000ef0: 4d69 6d65 4461 7461 6301 0000 0000 0000  MimeDatac.......
+00000f00: 0000 0000 0003 0000 0004 0000 000f 0000  ................
+00000f10: 0072 0700 0000 7208 0000 0029 0472 0200  .r....r....).r..
+00000f20: 0000 da09 514d 696d 6544 6174 6172 0b00  ....QMimeDatar..
+00000f30: 0000 720c 0000 0072 0d00 0000 7211 0000  ..r....r....r...
+00000f40: 0072 0900 0000 7213 0000 0072 0b00 0000  .r....r....r....
+00000f50: 5600 0000 7214 0000 007a 114d 696d 6544  V...r....z.MimeD
+00000f60: 6174 612e 5f5f 696e 6974 5f5f 7215 0000  ata.__init__r...
+00000f70: 0072 0900 0000 7209 0000 0072 1100 0000  .r....r....r....
+00000f80: 7213 0000 0072 3300 0000 5500 0000 721a  r....r3...U...r.
+00000f90: 0000 0072 3300 0000 6300 0000 0000 0000  ...r3...c.......
+00000fa0: 0000 0000 0000 0000 0003 0000 0000 0000  ................
+00000fb0: 0072 0500 0000 2903 da0e 5061 7573 6541  .r....)...PauseA
+00000fc0: 6e69 6d61 7469 6f6e 6301 0000 0000 0000  nimationc.......
+00000fd0: 0000 0000 0003 0000 0004 0000 000f 0000  ................
+00000fe0: 0072 0700 0000 7208 0000 0029 0472 0200  .r....r....).r..
+00000ff0: 0000 da0f 5150 6175 7365 416e 696d 6174  ....QPauseAnimat
+00001000: 696f 6e72 0b00 0000 720c 0000 0072 0d00  ionr....r....r..
+00001010: 0000 7211 0000 0072 0900 0000 7213 0000  ..r....r....r...
+00001020: 0072 0b00 0000 5c00 0000 7214 0000 007a  .r....\...r....z
+00001030: 1750 6175 7365 416e 696d 6174 696f 6e2e  .PauseAnimation.
+00001040: 5f5f 696e 6974 5f5f 7215 0000 0072 0900  __init__r....r..
+00001050: 0000 7209 0000 0072 1100 0000 7213 0000  ..r....r....r...
+00001060: 0072 3500 0000 5b00 0000 721a 0000 0072  .r5...[...r....r
+00001070: 3500 0000 6300 0000 0000 0000 0000 0000  5...c...........
+00001080: 0000 0000 0003 0000 0000 0000 0072 0500  .............r..
+00001090: 0000 2903 da0c 506c 7567 696e 4c6f 6164  ..)...PluginLoad
+000010a0: 6572 6301 0000 0000 0000 0000 0000 0003  erc.............
+000010b0: 0000 0004 0000 000f 0000 0072 0700 0000  ...........r....
+000010c0: 7208 0000 0029 0472 0200 0000 da0d 5150  r....).r......QP
+000010d0: 6c75 6769 6e4c 6f61 6465 7272 0b00 0000  luginLoaderr....
+000010e0: 720c 0000 0072 0d00 0000 7211 0000 0072  r....r....r....r
+000010f0: 0900 0000 7213 0000 0072 0b00 0000 6200  ....r....r....b.
+00001100: 0000 7214 0000 007a 1550 6c75 6769 6e4c  ..r....z.PluginL
+00001110: 6f61 6465 722e 5f5f 696e 6974 5f5f 7215  oader.__init__r.
+00001120: 0000 0072 0900 0000 7209 0000 0072 1100  ...r....r....r..
+00001130: 0000 7213 0000 0072 3700 0000 6100 0000  ..r....r7...a...
+00001140: 721a 0000 0072 3700 0000 6300 0000 0000  r....r7...c.....
+00001150: 0000 0000 0000 0000 0000 0003 0000 0000  ................
+00001160: 0000 0072 0500 0000 2903 da07 5072 6f63  ...r....)...Proc
+00001170: 6573 7363 0100 0000 0000 0000 0000 0000  essc............
+00001180: 0300 0000 0400 0000 0f00 0000 7207 0000  ............r...
+00001190: 0072 0800 0000 2904 7202 0000 00da 0851  .r....).r......Q
+000011a0: 5072 6f63 6573 7372 0b00 0000 720c 0000  Processr....r...
+000011b0: 0072 0d00 0000 7211 0000 0072 0900 0000  .r....r....r....
+000011c0: 7213 0000 0072 0b00 0000 6800 0000 7214  r....r....h...r.
+000011d0: 0000 007a 1050 726f 6365 7373 2e5f 5f69  ...z.Process.__i
+000011e0: 6e69 745f 5f72 1500 0000 7209 0000 0072  nit__r....r....r
+000011f0: 0900 0000 7211 0000 0072 1300 0000 7239  ....r....r....r9
+00001200: 0000 0067 0000 0072 1a00 0000 7239 0000  ...g...r....r9..
+00001210: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00001220: 0000 0300 0000 0000 0000 7205 0000 0029  ..........r....)
+00001230: 03da 0853 6176 6546 696c 6563 0100 0000  ...SaveFilec....
+00001240: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00001250: 0f00 0000 7207 0000 0072 0800 0000 2904  ....r....r....).
+00001260: 7202 0000 00da 0951 5361 7665 4669 6c65  r......QSaveFile
 00001270: 720b 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
 00001280: 1100 0000 7209 0000 0072 1300 0000 720b  ....r....r....r.
-00001290: 0000 006e 0000 0072 1400 0000 7a15 5368  ...n...r....z.Sh
-000012a0: 6172 6564 4d65 6d6f 7279 2e5f 5f69 6e69  aredMemory.__ini
-000012b0: 745f 5f72 1500 0000 7209 0000 0072 0900  t__r....r....r..
-000012c0: 0000 7211 0000 0072 1300 0000 723b 0000  ..r....r....r;..
-000012d0: 006d 0000 0072 1a00 0000 723b 0000 0063  .m...r....r;...c
-000012e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000012f0: 0300 0000 0000 0000 7205 0000 0029 03da  ........r....)..
-00001300: 0c53 6967 6e61 6c4d 6170 7065 7263 0100  .SignalMapperc..
-00001310: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00001320: 0000 0f00 0000 7207 0000 0072 0800 0000  ......r....r....
-00001330: 2904 7202 0000 00da 0d51 5369 676e 616c  ).r......QSignal
-00001340: 4d61 7070 6572 720b 0000 0072 0c00 0000  Mapperr....r....
-00001350: 720d 0000 0072 1100 0000 7209 0000 0072  r....r....r....r
-00001360: 1300 0000 720b 0000 0074 0000 0072 1400  ....r....t...r..
-00001370: 0000 7a15 5369 676e 616c 4d61 7070 6572  ..z.SignalMapper
-00001380: 2e5f 5f69 6e69 745f 5f72 1500 0000 7209  .__init__r....r.
-00001390: 0000 0072 0900 0000 7211 0000 0072 1300  ...r....r....r..
-000013a0: 0000 723d 0000 0073 0000 0072 1a00 0000  ..r=...s...r....
-000013b0: 723d 0000 0063 0000 0000 0000 0000 0000  r=...c..........
-000013c0: 0000 0000 0000 0300 0000 0000 0000 7205  ..............r.
-000013d0: 0000 0029 03da 0e53 6f63 6b65 744e 6f74  ...)...SocketNot
-000013e0: 6966 6965 7263 0100 0000 0000 0000 0000  ifierc..........
-000013f0: 0000 0300 0000 0400 0000 0f00 0000 7207  ..............r.
-00001400: 0000 0072 0800 0000 2904 7202 0000 00da  ...r....).r.....
-00001410: 0f51 536f 636b 6574 4e6f 7469 6669 6572  .QSocketNotifier
-00001420: 720b 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
-00001430: 1100 0000 7209 0000 0072 1300 0000 720b  ....r....r....r.
-00001440: 0000 007a 0000 0072 1400 0000 7a17 536f  ...z...r....z.So
-00001450: 636b 6574 4e6f 7469 6669 6572 2e5f 5f69  cketNotifier.__i
-00001460: 6e69 745f 5f72 1500 0000 7209 0000 0072  nit__r....r....r
-00001470: 0900 0000 7211 0000 0072 1300 0000 723f  ....r....r....r?
-00001480: 0000 0079 0000 0072 1a00 0000 723f 0000  ...y...r....r?..
-00001490: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-000014a0: 0000 0300 0000 0000 0000 7205 0000 0029  ..........r....)
-000014b0: 03da 1453 6f72 7446 696c 7465 7250 726f  ...SortFilterPro
-000014c0: 7879 4d6f 6465 6c63 0100 0000 0000 0000  xyModelc........
-000014d0: 0000 0000 0300 0000 0400 0000 0f00 0000  ................
-000014e0: 7207 0000 0072 0800 0000 2904 7202 0000  r....r....).r...
-000014f0: 00da 1551 536f 7274 4669 6c74 6572 5072  ...QSortFilterPr
-00001500: 6f78 794d 6f64 656c 720b 0000 0072 0c00  oxyModelr....r..
-00001510: 0000 720d 0000 0072 1100 0000 7209 0000  ..r....r....r...
-00001520: 0072 1300 0000 720b 0000 0080 0000 0072  .r....r........r
-00001530: 1400 0000 7a1d 536f 7274 4669 6c74 6572  ....z.SortFilter
-00001540: 5072 6f78 794d 6f64 656c 2e5f 5f69 6e69  ProxyModel.__ini
-00001550: 745f 5f72 1500 0000 7209 0000 0072 0900  t__r....r....r..
-00001560: 0000 7211 0000 0072 1300 0000 7241 0000  ..r....r....rA..
-00001570: 007f 0000 0072 1a00 0000 7241 0000 0063  .....r....rA...c
-00001580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001590: 0300 0000 0000 0000 7205 0000 0029 03da  ........r....)..
-000015a0: 0f53 7472 696e 674c 6973 744d 6f64 656c  .StringListModel
-000015b0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-000015c0: 0004 0000 000f 0000 0072 0700 0000 7208  .........r....r.
-000015d0: 0000 0029 0472 0200 0000 da10 5153 7472  ...).r......QStr
-000015e0: 696e 674c 6973 744d 6f64 656c 720b 0000  ingListModelr...
-000015f0: 0072 0c00 0000 720d 0000 0072 1100 0000  .r....r....r....
-00001600: 7209 0000 0072 1300 0000 720b 0000 0086  r....r....r.....
-00001610: 0000 0072 1400 0000 7a18 5374 7269 6e67  ...r....z.String
-00001620: 4c69 7374 4d6f 6465 6c2e 5f5f 696e 6974  ListModel.__init
-00001630: 5f5f 7215 0000 0072 0900 0000 7209 0000  __r....r....r...
-00001640: 0072 1100 0000 7213 0000 0072 4300 0000  .r....r....rC...
-00001650: 8500 0000 721a 0000 0072 4300 0000 6300  ....r....rC...c.
-00001660: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-00001670: 0000 0000 0000 0072 0500 0000 2903 da0d  .......r....)...
-00001680: 5465 6d70 6f72 6172 7946 696c 6563 0100  TemporaryFilec..
-00001690: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-000016a0: 0000 0f00 0000 7207 0000 0072 0800 0000  ......r....r....
-000016b0: 2904 7202 0000 00da 0e51 5465 6d70 6f72  ).r......QTempor
-000016c0: 6172 7946 696c 6572 0b00 0000 720c 0000  aryFiler....r...
-000016d0: 0072 0d00 0000 7211 0000 0072 0900 0000  .r....r....r....
-000016e0: 7213 0000 0072 0b00 0000 8c00 0000 7214  r....r........r.
-000016f0: 0000 007a 1654 656d 706f 7261 7279 4669  ...z.TemporaryFi
-00001700: 6c65 2e5f 5f69 6e69 745f 5f72 1500 0000  le.__init__r....
-00001710: 7209 0000 0072 0900 0000 7211 0000 0072  r....r....r....r
-00001720: 1300 0000 7245 0000 008b 0000 0072 1a00  ....rE.......r..
-00001730: 0000 7245 0000 0063 0000 0000 0000 0000  ..rE...c........
-00001740: 0000 0000 0000 0000 0300 0000 0000 0000  ................
-00001750: 7205 0000 0029 03da 0654 6872 6561 6463  r....)...Threadc
+00001290: 0000 006e 0000 0072 1400 0000 7a11 5361  ...n...r....z.Sa
+000012a0: 7665 4669 6c65 2e5f 5f69 6e69 745f 5f72  veFile.__init__r
+000012b0: 1500 0000 7209 0000 0072 0900 0000 7211  ....r....r....r.
+000012c0: 0000 0072 1300 0000 723b 0000 006d 0000  ...r....r;...m..
+000012d0: 0072 1a00 0000 723b 0000 0063 0000 0000  .r....r;...c....
+000012e0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+000012f0: 0000 0000 7205 0000 0029 03da 0c53 6861  ....r....)...Sha
+00001300: 7265 644d 656d 6f72 7963 0100 0000 0000  redMemoryc......
+00001310: 0000 0000 0000 0300 0000 0400 0000 0f00  ................
+00001320: 0000 7207 0000 0072 0800 0000 2904 7202  ..r....r....).r.
+00001330: 0000 00da 0d51 5368 6172 6564 4d65 6d6f  .....QSharedMemo
+00001340: 7279 720b 0000 0072 0c00 0000 720d 0000  ryr....r....r...
+00001350: 0072 1100 0000 7209 0000 0072 1300 0000  .r....r....r....
+00001360: 720b 0000 0074 0000 0072 1400 0000 7a15  r....t...r....z.
+00001370: 5368 6172 6564 4d65 6d6f 7279 2e5f 5f69  SharedMemory.__i
+00001380: 6e69 745f 5f72 1500 0000 7209 0000 0072  nit__r....r....r
+00001390: 0900 0000 7211 0000 0072 1300 0000 723d  ....r....r....r=
+000013a0: 0000 0073 0000 0072 1a00 0000 723d 0000  ...s...r....r=..
+000013b0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+000013c0: 0000 0300 0000 0000 0000 7205 0000 0029  ..........r....)
+000013d0: 03da 0c53 6967 6e61 6c4d 6170 7065 7263  ...SignalMapperc
+000013e0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+000013f0: 0400 0000 0f00 0000 7207 0000 0072 0800  ........r....r..
+00001400: 0000 2904 7202 0000 00da 0d51 5369 676e  ..).r......QSign
+00001410: 616c 4d61 7070 6572 720b 0000 0072 0c00  alMapperr....r..
+00001420: 0000 720d 0000 0072 1100 0000 7209 0000  ..r....r....r...
+00001430: 0072 1300 0000 720b 0000 007a 0000 0072  .r....r....z...r
+00001440: 1400 0000 7a15 5369 676e 616c 4d61 7070  ....z.SignalMapp
+00001450: 6572 2e5f 5f69 6e69 745f 5f72 1500 0000  er.__init__r....
+00001460: 7209 0000 0072 0900 0000 7211 0000 0072  r....r....r....r
+00001470: 1300 0000 723f 0000 0079 0000 0072 1a00  ....r?...y...r..
+00001480: 0000 723f 0000 0063 0000 0000 0000 0000  ..r?...c........
+00001490: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+000014a0: 7205 0000 0029 03da 0e53 6f63 6b65 744e  r....)...SocketN
+000014b0: 6f74 6966 6965 7263 0100 0000 0000 0000  otifierc........
+000014c0: 0000 0000 0300 0000 0400 0000 0f00 0000  ................
+000014d0: 7207 0000 0072 0800 0000 2904 7202 0000  r....r....).r...
+000014e0: 00da 0f51 536f 636b 6574 4e6f 7469 6669  ...QSocketNotifi
+000014f0: 6572 720b 0000 0072 0c00 0000 720d 0000  err....r....r...
+00001500: 0072 1100 0000 7209 0000 0072 1300 0000  .r....r....r....
+00001510: 720b 0000 0080 0000 0072 1400 0000 7a17  r........r....z.
+00001520: 536f 636b 6574 4e6f 7469 6669 6572 2e5f  SocketNotifier._
+00001530: 5f69 6e69 745f 5f72 1500 0000 7209 0000  _init__r....r...
+00001540: 0072 0900 0000 7211 0000 0072 1300 0000  .r....r....r....
+00001550: 7241 0000 007f 0000 0072 1a00 0000 7241  rA.......r....rA
+00001560: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00001570: 0000 0000 0300 0000 0000 0000 7205 0000  ............r...
+00001580: 0029 03da 1453 6f72 7446 696c 7465 7250  .)...SortFilterP
+00001590: 726f 7879 4d6f 6465 6c63 0100 0000 0000  roxyModelc......
+000015a0: 0000 0000 0000 0300 0000 0400 0000 0f00  ................
+000015b0: 0000 7207 0000 0072 0800 0000 2904 7202  ..r....r....).r.
+000015c0: 0000 00da 1551 536f 7274 4669 6c74 6572  .....QSortFilter
+000015d0: 5072 6f78 794d 6f64 656c 720b 0000 0072  ProxyModelr....r
+000015e0: 0c00 0000 720d 0000 0072 1100 0000 7209  ....r....r....r.
+000015f0: 0000 0072 1300 0000 720b 0000 0086 0000  ...r....r.......
+00001600: 0072 1400 0000 7a1d 536f 7274 4669 6c74  .r....z.SortFilt
+00001610: 6572 5072 6f78 794d 6f64 656c 2e5f 5f69  erProxyModel.__i
+00001620: 6e69 745f 5f72 1500 0000 7209 0000 0072  nit__r....r....r
+00001630: 0900 0000 7211 0000 0072 1300 0000 7243  ....r....r....rC
+00001640: 0000 0085 0000 0072 1a00 0000 7243 0000  .......r....rC..
+00001650: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00001660: 0000 0300 0000 0000 0000 7205 0000 0029  ..........r....)
+00001670: 03da 0f53 7472 696e 674c 6973 744d 6f64  ...StringListMod
+00001680: 656c 6301 0000 0000 0000 0000 0000 0003  elc.............
+00001690: 0000 0004 0000 000f 0000 0072 0700 0000  ...........r....
+000016a0: 7208 0000 0029 0472 0200 0000 da10 5153  r....).r......QS
+000016b0: 7472 696e 674c 6973 744d 6f64 656c 720b  tringListModelr.
+000016c0: 0000 0072 0c00 0000 720d 0000 0072 1100  ...r....r....r..
+000016d0: 0000 7209 0000 0072 1300 0000 720b 0000  ..r....r....r...
+000016e0: 008c 0000 0072 1400 0000 7a18 5374 7269  .....r....z.Stri
+000016f0: 6e67 4c69 7374 4d6f 6465 6c2e 5f5f 696e  ngListModel.__in
+00001700: 6974 5f5f 7215 0000 0072 0900 0000 7209  it__r....r....r.
+00001710: 0000 0072 1100 0000 7213 0000 0072 4500  ...r....r....rE.
+00001720: 0000 8b00 0000 721a 0000 0072 4500 0000  ......r....rE...
+00001730: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00001740: 0003 0000 0000 0000 0072 0500 0000 2903  .........r....).
+00001750: da0d 5465 6d70 6f72 6172 7946 696c 6563  ..TemporaryFilec
 00001760: 0100 0000 0000 0000 0000 0000 0300 0000  ................
 00001770: 0400 0000 0f00 0000 7207 0000 0072 0800  ........r....r..
-00001780: 0000 2904 7202 0000 00da 0751 5468 7265  ..).r......QThre
-00001790: 6164 720b 0000 0072 0c00 0000 720d 0000  adr....r....r...
-000017a0: 0072 1100 0000 7209 0000 0072 1300 0000  .r....r....r....
-000017b0: 720b 0000 0092 0000 0072 1400 0000 7a0f  r........r....z.
-000017c0: 5468 7265 6164 2e5f 5f69 6e69 745f 5f72  Thread.__init__r
-000017d0: 1500 0000 7209 0000 0072 0900 0000 7211  ....r....r....r.
-000017e0: 0000 0072 1300 0000 7247 0000 0091 0000  ...r....rG......
-000017f0: 0072 1a00 0000 7247 0000 0063 0000 0000  .r....rG...c....
-00001800: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00001810: 0000 0000 7205 0000 0029 03da 0a54 6872  ....r....)...Thr
-00001820: 6561 6450 6f6f 6c63 0100 0000 0000 0000  eadPoolc........
-00001830: 0000 0000 0300 0000 0400 0000 0f00 0000  ................
-00001840: 7207 0000 0072 0800 0000 2904 7202 0000  r....r....).r...
-00001850: 00da 0b51 5468 7265 6164 506f 6f6c 720b  ...QThreadPoolr.
-00001860: 0000 0072 0c00 0000 720d 0000 0072 1100  ...r....r....r..
-00001870: 0000 7209 0000 0072 1300 0000 720b 0000  ..r....r....r...
-00001880: 0098 0000 0072 1400 0000 7a13 5468 7265  .....r....z.Thre
-00001890: 6164 506f 6f6c 2e5f 5f69 6e69 745f 5f72  adPool.__init__r
-000018a0: 1500 0000 7209 0000 0072 0900 0000 7211  ....r....r....r.
-000018b0: 0000 0072 1300 0000 7249 0000 0097 0000  ...r....rI......
-000018c0: 0072 1a00 0000 7249 0000 0063 0000 0000  .r....rI...c....
-000018d0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-000018e0: 0000 0000 7205 0000 0029 03da 0854 696d  ....r....)...Tim
-000018f0: 654c 696e 6563 0100 0000 0000 0000 0000  eLinec..........
-00001900: 0000 0300 0000 0400 0000 0f00 0000 7207  ..............r.
-00001910: 0000 0072 0800 0000 2904 7202 0000 00da  ...r....).r.....
-00001920: 0951 5469 6d65 4c69 6e65 720b 0000 0072  .QTimeLiner....r
-00001930: 0c00 0000 720d 0000 0072 1100 0000 7209  ....r....r....r.
-00001940: 0000 0072 1300 0000 720b 0000 009e 0000  ...r....r.......
-00001950: 0072 1400 0000 7a11 5469 6d65 4c69 6e65  .r....z.TimeLine
-00001960: 2e5f 5f69 6e69 745f 5f72 1500 0000 7209  .__init__r....r.
-00001970: 0000 0072 0900 0000 7211 0000 0072 1300  ...r....r....r..
-00001980: 0000 724b 0000 009d 0000 0072 1a00 0000  ..rK.......r....
-00001990: 724b 0000 0063 0000 0000 0000 0000 0000  rK...c..........
-000019a0: 0000 0000 0000 0300 0000 0000 0000 7205  ..............r.
-000019b0: 0000 0029 03da 0554 696d 6572 6301 0000  ...)...Timerc...
-000019c0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-000019d0: 000f 0000 0072 0700 0000 7208 0000 0029  .....r....r....)
-000019e0: 0472 0200 0000 da06 5154 696d 6572 720b  .r......QTimerr.
-000019f0: 0000 0072 0c00 0000 720d 0000 0072 1100  ...r....r....r..
-00001a00: 0000 7209 0000 0072 1300 0000 720b 0000  ..r....r....r...
-00001a10: 00a4 0000 0072 1400 0000 7a0e 5469 6d65  .....r....z.Time
-00001a20: 722e 5f5f 696e 6974 5f5f 7215 0000 0072  r.__init__r....r
-00001a30: 0900 0000 7209 0000 0072 1100 0000 7213  ....r....r....r.
-00001a40: 0000 0072 4d00 0000 a300 0000 721a 0000  ...rM.......r...
-00001a50: 0072 4d00 0000 6300 0000 0000 0000 0000  .rM...c.........
-00001a60: 0000 0000 0000 0003 0000 0000 0000 0072  ...............r
-00001a70: 0500 0000 2903 da0a 5472 616e 736c 6174  ....)...Translat
-00001a80: 6f72 6301 0000 0000 0000 0000 0000 0003  orc.............
-00001a90: 0000 0004 0000 000f 0000 0072 0700 0000  ...........r....
-00001aa0: 7208 0000 0029 0472 0200 0000 da0b 5154  r....).r......QT
-00001ab0: 7261 6e73 6c61 746f 7272 0b00 0000 720c  ranslatorr....r.
-00001ac0: 0000 0072 0d00 0000 7211 0000 0072 0900  ...r....r....r..
-00001ad0: 0000 7213 0000 0072 0b00 0000 aa00 0000  ..r....r........
-00001ae0: 7214 0000 007a 1354 7261 6e73 6c61 746f  r....z.Translato
-00001af0: 722e 5f5f 696e 6974 5f5f 7215 0000 0072  r.__init__r....r
-00001b00: 0900 0000 7209 0000 0072 1100 0000 7213  ....r....r....r.
-00001b10: 0000 0072 4f00 0000 a900 0000 721a 0000  ...rO.......r...
-00001b20: 0072 4f00 0000 6300 0000 0000 0000 0000  .rO...c.........
-00001b30: 0000 0000 0000 0003 0000 0000 0000 0072  ...............r
-00001b40: 0500 0000 2903 da13 5472 616e 7370 6f73  ....)...Transpos
-00001b50: 6550 726f 7879 4d6f 6465 6c63 0100 0000  eProxyModelc....
-00001b60: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00001b70: 0f00 0000 7207 0000 0072 0800 0000 2904  ....r....r....).
-00001b80: 7202 0000 00da 1451 5472 616e 7370 6f73  r......QTranspos
-00001b90: 6550 726f 7879 4d6f 6465 6c72 0b00 0000  eProxyModelr....
-00001ba0: 720c 0000 0072 0d00 0000 7211 0000 0072  r....r....r....r
-00001bb0: 0900 0000 7213 0000 0072 0b00 0000 b000  ....r....r......
-00001bc0: 0000 7214 0000 007a 1c54 7261 6e73 706f  ..r....z.Transpo
-00001bd0: 7365 5072 6f78 794d 6f64 656c 2e5f 5f69  seProxyModel.__i
-00001be0: 6e69 745f 5f72 1500 0000 7209 0000 0072  nit__r....r....r
-00001bf0: 0900 0000 7211 0000 0072 1300 0000 7251  ....r....r....rQ
-00001c00: 0000 00af 0000 0072 1a00 0000 7251 0000  .......r....rQ..
-00001c10: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00001c20: 0000 0300 0000 0000 0000 7205 0000 0029  ..........r....)
-00001c30: 03da 1056 6172 6961 6e74 416e 696d 6174  ...VariantAnimat
-00001c40: 696f 6e63 0100 0000 0000 0000 0000 0000  ionc............
-00001c50: 0300 0000 0400 0000 0f00 0000 7207 0000  ............r...
-00001c60: 0072 0800 0000 2904 7202 0000 00da 1151  .r....).r......Q
-00001c70: 5661 7269 616e 7441 6e69 6d61 7469 6f6e  VariantAnimation
-00001c80: 720b 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
-00001c90: 1100 0000 7209 0000 0072 1300 0000 720b  ....r....r....r.
-00001ca0: 0000 00b6 0000 0072 1400 0000 7a19 5661  .......r....z.Va
-00001cb0: 7269 616e 7441 6e69 6d61 7469 6f6e 2e5f  riantAnimation._
-00001cc0: 5f69 6e69 745f 5f72 1500 0000 7209 0000  _init__r....r...
-00001cd0: 0072 0900 0000 7211 0000 0072 1300 0000  .r....r....r....
-00001ce0: 7253 0000 00b5 0000 0072 1a00 0000 7253  rS.......r....rS
-00001cf0: 0000 004e 2940 da07 5079 5369 6465 3672  ...N)@..PySide6r
-00001d00: 0200 0000 da04 636f 7265 7204 0000 0072  ......corer....r
-00001d10: 0a00 0000 7206 0000 0072 1c00 0000 721b  ....r....r....r.
-00001d20: 0000 0072 1e00 0000 721d 0000 0072 2000  ...r....r....r .
-00001d30: 0000 721f 0000 0072 2200 0000 7221 0000  ..r....r"...r!..
-00001d40: 0072 2400 0000 7223 0000 0072 2600 0000  .r$...r#...r&...
-00001d50: 7225 0000 0072 2800 0000 7227 0000 0072  r%...r(...r'...r
-00001d60: 2a00 0000 7229 0000 0072 2c00 0000 722b  *...r)...r,...r+
-00001d70: 0000 0072 2e00 0000 722d 0000 0072 3000  ...r....r-...r0.
-00001d80: 0000 722f 0000 0072 3200 0000 7231 0000  ..r/...r2...r1..
-00001d90: 0072 3400 0000 7233 0000 0072 3600 0000  .r4...r3...r6...
-00001da0: 7235 0000 0072 3800 0000 7237 0000 0072  r5...r8...r7...r
-00001db0: 3a00 0000 7239 0000 0072 3c00 0000 723b  :...r9...r<...r;
-00001dc0: 0000 0072 3e00 0000 723d 0000 0072 4000  ...r>...r=...r@.
-00001dd0: 0000 723f 0000 0072 4200 0000 7241 0000  ..r?...rB...rA..
-00001de0: 0072 4400 0000 7243 0000 0072 4600 0000  .rD...rC...rF...
-00001df0: 7245 0000 0072 4800 0000 7247 0000 0072  rE...rH...rG...r
-00001e00: 4a00 0000 7249 0000 0072 4c00 0000 724b  J...rI...rL...rK
-00001e10: 0000 0072 4e00 0000 724d 0000 0072 5000  ...rN...rM...rP.
-00001e20: 0000 724f 0000 0072 5200 0000 7251 0000  ..rO...rR...rQ..
-00001e30: 0072 5400 0000 7253 0000 0072 0900 0000  .rT...rS...r....
-00001e40: 7209 0000 0072 0900 0000 7213 0000 00da  r....r....r.....
-00001e50: 083c 6d6f 6475 6c65 3e01 0000 0073 4000  .<module>....s@.
-00001e60: 0000 0c02 0c01 1403 1406 1406 1406 1406  ................
-00001e70: 1406 1406 1406 1406 1406 1406 1406 1406  ................
-00001e80: 1406 1406 1406 1406 1406 1406 1406 1406  ................
-00001e90: 1406 1406 1406 1406 1406 1406 1406 1406  ................
-00001ea0: 1806                                     ..
+00001780: 0000 2904 7202 0000 00da 0e51 5465 6d70  ..).r......QTemp
+00001790: 6f72 6172 7946 696c 6572 0b00 0000 720c  oraryFiler....r.
+000017a0: 0000 0072 0d00 0000 7211 0000 0072 0900  ...r....r....r..
+000017b0: 0000 7213 0000 0072 0b00 0000 9200 0000  ..r....r........
+000017c0: 7214 0000 007a 1654 656d 706f 7261 7279  r....z.Temporary
+000017d0: 4669 6c65 2e5f 5f69 6e69 745f 5f72 1500  File.__init__r..
+000017e0: 0000 7209 0000 0072 0900 0000 7211 0000  ..r....r....r...
+000017f0: 0072 1300 0000 7247 0000 0091 0000 0072  .r....rG.......r
+00001800: 1a00 0000 7247 0000 0063 0000 0000 0000  ....rG...c......
+00001810: 0000 0000 0000 0000 0000 0300 0000 0000  ................
+00001820: 0000 7205 0000 0029 03da 0654 6872 6561  ..r....)...Threa
+00001830: 6463 0100 0000 0000 0000 0000 0000 0300  dc..............
+00001840: 0000 0400 0000 0f00 0000 7207 0000 0072  ..........r....r
+00001850: 0800 0000 2904 7202 0000 00da 0751 5468  ....).r......QTh
+00001860: 7265 6164 720b 0000 0072 0c00 0000 720d  readr....r....r.
+00001870: 0000 0072 1100 0000 7209 0000 0072 1300  ...r....r....r..
+00001880: 0000 720b 0000 0098 0000 0072 1400 0000  ..r........r....
+00001890: 7a0f 5468 7265 6164 2e5f 5f69 6e69 745f  z.Thread.__init_
+000018a0: 5f72 1500 0000 7209 0000 0072 0900 0000  _r....r....r....
+000018b0: 7211 0000 0072 1300 0000 7249 0000 0097  r....r....rI....
+000018c0: 0000 0072 1a00 0000 7249 0000 0063 0000  ...r....rI...c..
+000018d0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+000018e0: 0000 0000 0000 7205 0000 0029 03da 0a54  ......r....)...T
+000018f0: 6872 6561 6450 6f6f 6c63 0100 0000 0000  hreadPoolc......
+00001900: 0000 0000 0000 0300 0000 0400 0000 0f00  ................
+00001910: 0000 7207 0000 0072 0800 0000 2904 7202  ..r....r....).r.
+00001920: 0000 00da 0b51 5468 7265 6164 506f 6f6c  .....QThreadPool
+00001930: 720b 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+00001940: 1100 0000 7209 0000 0072 1300 0000 720b  ....r....r....r.
+00001950: 0000 009e 0000 0072 1400 0000 7a13 5468  .......r....z.Th
+00001960: 7265 6164 506f 6f6c 2e5f 5f69 6e69 745f  readPool.__init_
+00001970: 5f72 1500 0000 7209 0000 0072 0900 0000  _r....r....r....
+00001980: 7211 0000 0072 1300 0000 724b 0000 009d  r....r....rK....
+00001990: 0000 0072 1a00 0000 724b 0000 0063 0000  ...r....rK...c..
+000019a0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+000019b0: 0000 0000 0000 7205 0000 0029 03da 0854  ......r....)...T
+000019c0: 696d 654c 696e 6563 0100 0000 0000 0000  imeLinec........
+000019d0: 0000 0000 0300 0000 0400 0000 0f00 0000  ................
+000019e0: 7207 0000 0072 0800 0000 2904 7202 0000  r....r....).r...
+000019f0: 00da 0951 5469 6d65 4c69 6e65 720b 0000  ...QTimeLiner...
+00001a00: 0072 0c00 0000 720d 0000 0072 1100 0000  .r....r....r....
+00001a10: 7209 0000 0072 1300 0000 720b 0000 00a4  r....r....r.....
+00001a20: 0000 0072 1400 0000 7a11 5469 6d65 4c69  ...r....z.TimeLi
+00001a30: 6e65 2e5f 5f69 6e69 745f 5f72 1500 0000  ne.__init__r....
+00001a40: 7209 0000 0072 0900 0000 7211 0000 0072  r....r....r....r
+00001a50: 1300 0000 724d 0000 00a3 0000 0072 1a00  ....rM.......r..
+00001a60: 0000 724d 0000 0063 0000 0000 0000 0000  ..rM...c........
+00001a70: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+00001a80: 7205 0000 0029 03da 0554 696d 6572 6301  r....)...Timerc.
+00001a90: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+00001aa0: 0000 000f 0000 0072 0700 0000 7208 0000  .......r....r...
+00001ab0: 0029 0472 0200 0000 da06 5154 696d 6572  .).r......QTimer
+00001ac0: 720b 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+00001ad0: 1100 0000 7209 0000 0072 1300 0000 720b  ....r....r....r.
+00001ae0: 0000 00aa 0000 0072 1400 0000 7a0e 5469  .......r....z.Ti
+00001af0: 6d65 722e 5f5f 696e 6974 5f5f 7215 0000  mer.__init__r...
+00001b00: 0072 0900 0000 7209 0000 0072 1100 0000  .r....r....r....
+00001b10: 7213 0000 0072 4f00 0000 a900 0000 721a  r....rO.......r.
+00001b20: 0000 0072 4f00 0000 6300 0000 0000 0000  ...rO...c.......
+00001b30: 0000 0000 0000 0000 0003 0000 0000 0000  ................
+00001b40: 0072 0500 0000 2903 da0a 5472 616e 736c  .r....)...Transl
+00001b50: 6174 6f72 6301 0000 0000 0000 0000 0000  atorc...........
+00001b60: 0003 0000 0004 0000 000f 0000 0072 0700  .............r..
+00001b70: 0000 7208 0000 0029 0472 0200 0000 da0b  ..r....).r......
+00001b80: 5154 7261 6e73 6c61 746f 7272 0b00 0000  QTranslatorr....
+00001b90: 720c 0000 0072 0d00 0000 7211 0000 0072  r....r....r....r
+00001ba0: 0900 0000 7213 0000 0072 0b00 0000 b000  ....r....r......
+00001bb0: 0000 7214 0000 007a 1354 7261 6e73 6c61  ..r....z.Transla
+00001bc0: 746f 722e 5f5f 696e 6974 5f5f 7215 0000  tor.__init__r...
+00001bd0: 0072 0900 0000 7209 0000 0072 1100 0000  .r....r....r....
+00001be0: 7213 0000 0072 5100 0000 af00 0000 721a  r....rQ.......r.
+00001bf0: 0000 0072 5100 0000 6300 0000 0000 0000  ...rQ...c.......
+00001c00: 0000 0000 0000 0000 0003 0000 0000 0000  ................
+00001c10: 0072 0500 0000 2903 da13 5472 616e 7370  .r....)...Transp
+00001c20: 6f73 6550 726f 7879 4d6f 6465 6c63 0100  oseProxyModelc..
+00001c30: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00001c40: 0000 0f00 0000 7207 0000 0072 0800 0000  ......r....r....
+00001c50: 2904 7202 0000 00da 1451 5472 616e 7370  ).r......QTransp
+00001c60: 6f73 6550 726f 7879 4d6f 6465 6c72 0b00  oseProxyModelr..
+00001c70: 0000 720c 0000 0072 0d00 0000 7211 0000  ..r....r....r...
+00001c80: 0072 0900 0000 7213 0000 0072 0b00 0000  .r....r....r....
+00001c90: b600 0000 7214 0000 007a 1c54 7261 6e73  ....r....z.Trans
+00001ca0: 706f 7365 5072 6f78 794d 6f64 656c 2e5f  poseProxyModel._
+00001cb0: 5f69 6e69 745f 5f72 1500 0000 7209 0000  _init__r....r...
+00001cc0: 0072 0900 0000 7211 0000 0072 1300 0000  .r....r....r....
+00001cd0: 7253 0000 00b5 0000 0072 1a00 0000 7253  rS.......r....rS
+00001ce0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00001cf0: 0000 0000 0300 0000 0000 0000 7205 0000  ............r...
+00001d00: 0029 03da 1056 6172 6961 6e74 416e 696d  .)...VariantAnim
+00001d10: 6174 696f 6e63 0100 0000 0000 0000 0000  ationc..........
+00001d20: 0000 0300 0000 0400 0000 0f00 0000 7207  ..............r.
+00001d30: 0000 0072 0800 0000 2904 7202 0000 00da  ...r....).r.....
+00001d40: 1151 5661 7269 616e 7441 6e69 6d61 7469  .QVariantAnimati
+00001d50: 6f6e 720b 0000 0072 0c00 0000 720d 0000  onr....r....r...
+00001d60: 0072 1100 0000 7209 0000 0072 1300 0000  .r....r....r....
+00001d70: 720b 0000 00bc 0000 0072 1400 0000 7a19  r........r....z.
+00001d80: 5661 7269 616e 7441 6e69 6d61 7469 6f6e  VariantAnimation
+00001d90: 2e5f 5f69 6e69 745f 5f72 1500 0000 7209  .__init__r....r.
+00001da0: 0000 0072 0900 0000 7211 0000 0072 1300  ...r....r....r..
+00001db0: 0000 7255 0000 00bb 0000 0072 1a00 0000  ..rU.......r....
+00001dc0: 7255 0000 004e 2942 da07 5079 5369 6465  rU...N)B..PySide
+00001dd0: 3672 0200 0000 da04 636f 7265 7204 0000  6r......corer...
+00001de0: 0072 0a00 0000 7206 0000 0072 1c00 0000  .r....r....r....
+00001df0: 721b 0000 0072 1e00 0000 721d 0000 0072  r....r....r....r
+00001e00: 2000 0000 721f 0000 0072 2200 0000 7221   ...r....r"...r!
+00001e10: 0000 0072 2400 0000 7223 0000 0072 2600  ...r$...r#...r&.
+00001e20: 0000 7225 0000 0072 2800 0000 7227 0000  ..r%...r(...r'..
+00001e30: 0072 2a00 0000 7229 0000 0072 2c00 0000  .r*...r)...r,...
+00001e40: 722b 0000 0072 2e00 0000 722d 0000 0072  r+...r....r-...r
+00001e50: 3000 0000 722f 0000 0072 3200 0000 7231  0...r/...r2...r1
+00001e60: 0000 0072 3400 0000 7233 0000 0072 3600  ...r4...r3...r6.
+00001e70: 0000 7235 0000 0072 3800 0000 7237 0000  ..r5...r8...r7..
+00001e80: 0072 3a00 0000 7239 0000 0072 3c00 0000  .r:...r9...r<...
+00001e90: 723b 0000 0072 3e00 0000 723d 0000 0072  r;...r>...r=...r
+00001ea0: 4000 0000 723f 0000 0072 4200 0000 7241  @...r?...rB...rA
+00001eb0: 0000 0072 4400 0000 7243 0000 0072 4600  ...rD...rC...rF.
+00001ec0: 0000 7245 0000 0072 4800 0000 7247 0000  ..rE...rH...rG..
+00001ed0: 0072 4a00 0000 7249 0000 0072 4c00 0000  .rJ...rI...rL...
+00001ee0: 724b 0000 0072 4e00 0000 724d 0000 0072  rK...rN...rM...r
+00001ef0: 5000 0000 724f 0000 0072 5200 0000 7251  P...rO...rR...rQ
+00001f00: 0000 0072 5400 0000 7253 0000 0072 5600  ...rT...rS...rV.
+00001f10: 0000 7255 0000 0072 0900 0000 7209 0000  ..rU...r....r...
+00001f20: 0072 0900 0000 7213 0000 00da 083c 6d6f  .r....r......<mo
+00001f30: 6475 6c65 3e01 0000 0073 4200 0000 0c02  dule>....sB.....
+00001f40: 0c01 1403 1406 1406 1406 1406 1406 1406  ................
+00001f50: 1406 1406 1406 1406 1406 1406 1406 1406  ................
+00001f60: 1406 1406 1406 1406 1406 1406 1406 1406  ................
+00001f70: 1406 1406 1406 1406 1406 1406 1406 1806  ................
```

### Comparing `qtica-0.4.3/Qtica/tools/qtcore/objects.py` & `qtica-0.5.0/Qtica/tools/qtcore/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,20 @@
 
 class EventLoop(AbstractQObject, QtCore.QEventLoop):
     def __init__(self, *args, **kwargs):
         QtCore.QEventLoop.__init__(self, *args)
         super().__init__(**kwargs)
 
 
+class File(AbstractQObject, QtCore.QFile):
+    def __init__(self, *args, **kwargs):
+        QtCore.QFile.__init__(self, *args)
+        super().__init__(**kwargs)
+
+
 class FileDevice(AbstractQObject, QtCore.QFileDevice):
     def __init__(self, *args, **kwargs):
         QtCore.QFileDevice.__init__(self, *args)
         super().__init__(**kwargs)
 
 
 class FileSelector(AbstractQObject, QtCore.QFileSelector):
```

### Comparing `qtica-0.4.3/Qtica/tools/qtcore/tools.py` & `qtica-0.5.0/Qtica/tools/qtcore/tools.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/qtgui/__pycache__/objects.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/qtgui/__pycache__/objects.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/qtgui/__pycache__/tools.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/qtgui/__pycache__/tools.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/qtgui/objects.py` & `qtica-0.5.0/Qtica/tools/qtgui/objects.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/qtgui/tools.py` & `qtica-0.5.0/Qtica/tools/qtgui/tools.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/settings.py` & `qtica-0.5.0/Qtica/tools/settings.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/size_policy.py` & `qtica-0.5.0/Qtica/tools/size_policy.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/smooth_scroll.py` & `qtica-0.5.0/Qtica/tools/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/system_tray.py` & `qtica-0.5.0/Qtica/tools/system_tray.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/wrappers/__pycache__/__init__.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/wrappers/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/wrappers/__pycache__/border_layout.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/wrappers/__pycache__/border_layout.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/wrappers/__pycache__/border_layout.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/wrappers/__pycache__/border_layout.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/wrappers/__pycache__/dock_widgets.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/wrappers/__pycache__/dock_widgets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/wrappers/__pycache__/dock_widgets.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/wrappers/__pycache__/dock_widgets.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/wrappers/__pycache__/form_layout.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/wrappers/__pycache__/form_layout.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/wrappers/__pycache__/form_layout.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/wrappers/__pycache__/form_layout.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/wrappers/__pycache__/grid_layout.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/wrappers/__pycache__/grid_layout.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/wrappers/__pycache__/grid_layout.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/wrappers/__pycache__/grid_layout.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/wrappers/__pycache__/h_layout.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/wrappers/__pycache__/h_layout.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/wrappers/__pycache__/h_layout.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/wrappers/__pycache__/h_layout.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/wrappers/__pycache__/menu.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/wrappers/__pycache__/menu.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/wrappers/__pycache__/menu.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/wrappers/__pycache__/menu.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/wrappers/__pycache__/tool_bar.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/wrappers/__pycache__/tool_bar.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/wrappers/__pycache__/tool_bar.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/wrappers/__pycache__/tool_bar.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/wrappers/__pycache__/v_layout.cpython-310.pyc` & `qtica-0.5.0/Qtica/layouts/__pycache__/v_layout.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Jan  6 00:10:09 2024 UTC, .py size: 610 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,67 @@
-00000000: 6f0d 0d0a 0000 0000 619a 9865 6202 0000  o.......a..eb...
+00000000: 6f0d 0d0a 0000 0000 59e7 5066 8a02 0000  o.......Y.Pf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
-00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
-00000040: 6402 6c03 6d04 5a04 0100 4700 6403 6404  d.l.m.Z...G.d.d.
-00000050: 8400 6404 8302 5a05 4700 6405 6406 8400  ..d...Z.G.d.d...
-00000060: 6406 6505 8303 5a06 6407 5300 2908 e900  d.e...Z.d.S.)...
-00000070: 0000 0029 02da 0751 5769 6467 6574 da07  ...)...QWidget..
-00000080: 514c 6179 6f75 7429 01da 0251 7463 0000  QLayout)...Qtc..
-00000090: 0000 0000 0000 0000 0000 0000 0000 0900  ................
-000000a0: 0000 4000 0000 733a 0000 0065 005a 0164  ..@...s:...e.Z.d
-000000b0: 005a 0209 0109 0164 0a64 0265 0365 0442  .Z.....d.d.e.e.B
-000000c0: 0064 0365 0564 0465 066a 0764 0564 0166  .d.e.d.e.j.d.d.f
-000000d0: 0864 0664 0784 055a 0864 0864 0984 005a  .d.d...Z.d.d...Z
-000000e0: 0964 0153 0029 0bda 0e56 4c61 796f 7574  .d.S.)...VLayout
-000000f0: 5772 6170 7065 724e da05 6368 696c 64da  WrapperN..child.
-00000100: 0773 7472 6574 6368 da09 616c 6967 6e6d  .stretch..alignm
-00000110: 656e 74da 0672 6574 7572 6e63 0400 0000  ent..returnc....
-00000120: 0000 0000 0000 0000 0400 0000 0200 0000  ................
-00000130: 4300 0000 7316 0000 007c 017c 005f 007c  C...s....|.|._.|
-00000140: 027c 005f 017c 037c 005f 0264 0053 00a9  .|._.|.|._.d.S..
-00000150: 014e a903 7206 0000 0072 0700 0000 7208  .N..r....r....r.
-00000160: 0000 0029 04da 0473 656c 6672 0600 0000  ...)...selfr....
-00000170: 7207 0000 0072 0800 0000 a900 720d 0000  r....r......r...
-00000180: 00fa 592f 686f 6d65 2f6f 7361 6d61 2f57  ..Y/home/osama/W
-00000190: 6f72 6b73 7061 6365 2f2e 7665 6e76 2f6c  orkspace/.venv/l
-000001a0: 6962 2f70 7974 686f 6e33 2e31 302f 7369  ib/python3.10/si
-000001b0: 7465 2d70 6163 6b61 6765 732f 5174 6963  te-packages/Qtic
-000001c0: 612f 746f 6f6c 732f 7772 6170 7065 7273  a/tools/wrappers
-000001d0: 2f76 5f6c 6179 6f75 742e 7079 da08 5f5f  /v_layout.py..__
-000001e0: 696e 6974 5f5f 0600 0000 7306 0000 0006  init__....s.....
-000001f0: 0506 010a 017a 1756 4c61 796f 7574 5772  .....z.VLayoutWr
-00000200: 6170 7065 722e 5f5f 696e 6974 5f5f 6301  apper.__init__c.
-00000210: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00000220: 0000 0063 0000 0073 2a00 0000 8100 7c00  ...c...s*.....|.
-00000230: 6a00 7c00 6a01 7c00 6a02 6603 4400 5d09  j.|.j.|.j.f.D.].
-00000240: 7d01 7c01 6400 7501 7212 7c01 5600 0100  }.|.d.u.r.|.V...
-00000250: 7109 6400 5300 720a 0000 0072 0b00 0000  q.d.S.r....r....
-00000260: 2902 720c 0000 00da 0461 7474 7272 0d00  ).r......attrr..
-00000270: 0000 720d 0000 0072 0e00 0000 da0b 5f79  ..r....r......_y
-00000280: 6965 6c64 5f61 7474 720f 0000 0073 1200  ield_attr....s..
-00000290: 0000 0280 0402 0401 0401 08fd 0805 0601  ................
-000002a0: 0280 04fa 7a1a 564c 6179 6f75 7457 7261  ....z.VLayoutWra
-000002b0: 7070 6572 2e5f 7969 656c 645f 6174 7472  pper._yield_attr
-000002c0: 2902 4e4e 290a da08 5f5f 6e61 6d65 5f5f  ).NN)...__name__
-000002d0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-000002e0: 7175 616c 6e61 6d65 5f5f 7202 0000 0072  qualname__r....r
-000002f0: 0300 0000 da03 696e 7472 0400 0000 da0d  ......intr......
-00000300: 416c 6967 6e6d 656e 7446 6c61 6772 0f00  AlignmentFlagr..
-00000310: 0000 7211 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-00000320: 0072 0d00 0000 720e 0000 0072 0500 0000  .r....r....r....
-00000330: 0500 0000 731a 0000 0008 0002 0302 0104  ....s...........
-00000340: fd06 0102 ff02 0202 fe04 0302 fd02 030a  ................
-00000350: fd0c 0972 0500 0000 6300 0000 0000 0000  ...r....c.......
-00000360: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
-00000370: 0073 0c00 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
-00000380: 5300 2902 da10 526f 774c 6179 6f75 7457  S.)...RowLayoutW
-00000390: 7261 7070 6572 4e29 0372 1200 0000 7213  rapperN).r....r.
-000003a0: 0000 0072 1400 0000 720d 0000 0072 0d00  ...r....r....r..
-000003b0: 0000 720d 0000 0072 0e00 0000 7217 0000  ..r....r....r...
-000003c0: 0019 0000 0073 0400 0000 0800 0401 7217  .....s........r.
-000003d0: 0000 004e 2907 da11 5079 5369 6465 362e  ...N)...PySide6.
-000003e0: 5174 5769 6467 6574 7372 0200 0000 7203  QtWidgetsr....r.
-000003f0: 0000 00da 0e50 7953 6964 6536 2e51 7443  .....PySide6.QtC
-00000400: 6f72 6572 0400 0000 7205 0000 0072 1700  orer....r....r..
-00000410: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-00000420: 0072 0e00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000430: 0100 0000 7308 0000 0010 000c 010e 0314  ....s...........
-00000440: 14                                       .
+00000020: 0005 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
+00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
+00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6403  m.Z.m.Z.m.Z...d.
+00000050: 6404 6c06 6d07 5a07 0100 6403 6405 6c08  d.l.m.Z...d.d.l.
+00000060: 6d09 5a09 0100 6406 6407 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
+00000070: 0100 4700 6408 6409 8400 6409 650b 6503  ..G.d.d...d.e.e.
+00000080: 8304 5a0c 4700 640a 640b 8400 640b 650c  ..Z.G.d.d...d.e.
+00000090: 8303 5a0d 640c 5300 290d e900 0000 0029  ..Z.d.S.)......)
+000000a0: 01da 0555 6e69 6f6e 2903 da0b 5156 426f  ...Union)...QVBo
+000000b0: 784c 6179 6f75 74da 0751 5769 6467 6574  xLayout..QWidget
+000000c0: da07 514c 6179 6f75 74e9 0200 0000 2901  ..QLayout.....).
+000000d0: da0d 4c61 796f 7574 5772 6170 7065 7229  ..LayoutWrapper)
+000000e0: 01da 0941 6c69 676e 6d65 6e74 e901 0000  ...Alignment....
+000000f0: 0029 01da 0856 484c 6179 6f75 7463 0000  .)...VHLayoutc..
+00000100: 0000 0000 0000 0000 0000 0000 0000 0800  ................
+00000110: 0000 0000 0000 7338 0000 0065 005a 0164  ......s8...e.Z.d
+00000120: 005a 0264 0164 029c 0164 0365 0365 0465  .Z.d.d...d.e.e.e
+00000130: 0565 0665 0765 0866 0419 0019 0066 0287  .e.e.e.f.....f..
+00000140: 0066 0164 0464 0584 0e5a 0987 0004 005a  .f.d.d...Z.....Z
+00000150: 0a53 0029 06da 0756 4c61 796f 7574 4e29  .S.)...VLayoutN)
+00000160: 01da 0863 6869 6c64 7265 6e72 0c00 0000  ...childrenr....
+00000170: 6301 0000 0000 0000 0001 0000 0003 0000  c...............
+00000180: 0004 0000 000b 0000 0073 2400 0000 7400  .........s$...t.
+00000190: a001 7c00 a101 0100 7402 8300 6a01 6402  ..|.....t...j.d.
+000001a0: 6401 7c01 6901 7c02 a401 8e01 0100 6400  d.|.i.|.......d.
+000001b0: 5300 2903 4e72 0c00 0000 a900 2903 7203  S.).Nr......).r.
+000001c0: 0000 00da 085f 5f69 6e69 745f 5fda 0573  .....__init__..s
+000001d0: 7570 6572 2903 da04 7365 6c66 720c 0000  uper)...selfr...
+000001e0: 00da 066b 7761 7267 73a9 01da 095f 5f63  ...kwargs....__c
+000001f0: 6c61 7373 5f5f 720d 0000 00fa 522f 686f  lass__r.....R/ho
+00000200: 6d65 2f6f 7361 6d61 2f57 6f72 6b73 7061  me/osama/Workspa
+00000210: 6365 2f2e 7665 6e76 2f6c 6962 2f70 7974  ce/.venv/lib/pyt
+00000220: 686f 6e33 2e31 302f 7369 7465 2d70 6163  hon3.10/site-pac
+00000230: 6b61 6765 732f 5174 6963 612f 6c61 796f  kages/Qtica/layo
+00000240: 7574 732f 765f 6c61 796f 7574 2e70 7972  uts/v_layout.pyr
+00000250: 0e00 0000 0a00 0000 7304 0000 000a 071a  ........s.......
+00000260: 017a 1056 4c61 796f 7574 2e5f 5f69 6e69  .z.VLayout.__ini
+00000270: 745f 5f29 0bda 085f 5f6e 616d 655f 5fda  t__)...__name__.
+00000280: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000290: 7561 6c6e 616d 655f 5fda 046c 6973 7472  ualname__..listr
+000002a0: 0200 0000 7204 0000 0072 0500 0000 7207  ....r....r....r.
+000002b0: 0000 0072 0800 0000 720e 0000 00da 0d5f  ...r....r......_
+000002c0: 5f63 6c61 7373 6365 6c6c 5f5f 720d 0000  _classcell__r...
+000002d0: 0072 0d00 0000 7212 0000 0072 1400 0000  .r....r....r....
+000002e0: 720b 0000 0009 0000 0073 1200 0000 0800  r........s......
+000002f0: 0206 06fb 0602 0201 0201 0201 06fd 16fe  ................
+00000300: 720b 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000310: 0000 0000 0000 0100 0000 4000 0000 730c  ..........@...s.
+00000320: 0000 0065 005a 0164 005a 0264 0153 0029  ...e.Z.d.Z.d.S.)
+00000330: 02da 0952 6f77 4c61 796f 7574 4e29 0372  ...RowLayoutN).r
+00000340: 1500 0000 7216 0000 0072 1700 0000 720d  ....r....r....r.
+00000350: 0000 0072 0d00 0000 720d 0000 0072 1400  ...r....r....r..
+00000360: 0000 721a 0000 0015 0000 0073 0400 0000  ..r........s....
+00000370: 0800 0401 721a 0000 004e 290e da06 7479  ....r....N)...ty
+00000380: 7069 6e67 7202 0000 00da 1150 7953 6964  pingr......PySid
+00000390: 6536 2e51 7457 6964 6765 7473 7203 0000  e6.QtWidgetsr...
+000003a0: 0072 0400 0000 7205 0000 00da 1574 6f6f  .r....r......too
+000003b0: 6c73 2e77 7261 7070 6572 732e 6c61 796f  ls.wrappers.layo
+000003c0: 7574 7207 0000 00da 0f75 7469 6c73 2e61  utr......utils.a
+000003d0: 6c69 676e 6d65 6e74 7208 0000 00da 0976  lignmentr......v
+000003e0: 685f 6c61 796f 7574 720a 0000 0072 0b00  h_layoutr....r..
+000003f0: 0000 721a 0000 0072 0d00 0000 720d 0000  ..r....r....r...
+00000400: 0072 0d00 0000 7214 0000 00da 083c 6d6f  .r....r......<mo
+00000410: 6475 6c65 3e01 0000 0073 0e00 0000 0c00  dule>....s......
+00000420: 1401 0c01 0c01 0c01 1204 140c            ............
```

### Comparing `qtica-0.4.3/Qtica/tools/wrappers/__pycache__/v_layout.cpython-312.pyc` & `qtica-0.5.0/Qtica/tools/wrappers/__pycache__/v_layout.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/wrappers/__pycache__/water_progress_bar.cpython-310.pyc` & `qtica-0.5.0/Qtica/tools/wrappers/__pycache__/water_progress_bar.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/wrappers/grid_layout.py` & `qtica-0.5.0/Qtica/tools/wrappers/grid_layout.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/tools/wrappers/h_layout.py` & `qtica-0.5.0/Qtica/tools/wrappers/layout.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from PySide6.QtWidgets import QWidget, QLayout
 from PySide6.QtCore import Qt
 
 
-class HLayoutWrapper:
-    def __init__(self,
+class LayoutWrapper:
+    def __init__(self, 
                  child: QWidget | QLayout, 
                  stretch: int = None,
                  alignment: Qt.AlignmentFlag = None) -> None:
 
         self.child = child
         self.stretch = stretch
         self.alignment = alignment
@@ -15,12 +15,8 @@
     def _yield_attr(self):
         for attr in (
             self.child,
             self.stretch,
             self.alignment
         ):
             if attr is not None:
-                yield attr
-
-
-class ColumnLayoutWrapper(HLayoutWrapper):
-    ...
+                yield attr
```

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/__init__.cpython-312.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/_classes.cpython-312.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/_classes.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/_ensure_thread.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/_ensure_thread.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/_env_var.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/_env_var.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jan  5 22:19:49 2024 UTC, .py size: 1000 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8580 9865 e803 0000  o..........e....
+00000000: 6f0d 0d0a 0000 0000 58e9 5066 e503 0000  o.......X.Pf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6403 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6405 6c07 5a07 4700  m.Z...d.d.l.Z.G.
 00000060: 6406 6407 8400 6407 8302 5a08 6405 5300  d.d...d...Z.d.S.
 00000070: 2908 e900 0000 0029 01da 0445 6e75 6d29  )......)...Enum)
@@ -13,78 +13,78 @@
 000000c0: 6400 5a02 6401 5a03 640d 6403 6504 6505  d.Z.d.Z.d.d.e.e.
 000000d0: 6506 6602 1900 6404 6507 6405 6507 6606  e.f...d.e.d.e.f.
 000000e0: 6406 6407 8405 5a08 6509 6403 6504 6505  d.d...Z.e.d.e.e.
 000000f0: 6506 6602 1900 6408 6507 6405 6402 6606  e.f...d.e.d.d.f.
 00000100: 6409 640a 8404 8301 5a0a 6509 640d 6403  d.d.....Z.e.d.d.
 00000110: 6504 6505 6506 6602 1900 6404 6507 6405  e.e.e.f...d.e.d.
 00000120: 6507 6606 640b 640c 8405 8301 5a0b 6402  e.f.d.d.....Z.d.
-00000130: 5300 290e da06 456e 7656 6172 6125 0100  S.)...EnvVara%..
-00000140: 000a 2020 2020 2323 2320 5365 7420 4b65  ..    ### Set Ke
-00000150: 792c 2061 6e64 2056 616c 7565 0a20 2020  y, and Value.   
-00000160: 202d 2065 2e67 2c20 456e 7656 6172 2e73   - e.g, EnvVar.s
-00000170: 6574 2845 6e76 5661 7273 2e73 6361 6c65  et(EnvVars.scale
-00000180: 5f66 6163 746f 722c 2022 3022 290a 2020  _factor, "0").  
-00000190: 2020 2d20 652e 672c 2045 6e76 5661 722e    - e.g, EnvVar.
-000001a0: 7365 7428 2251 545f 5343 414c 455f 4641  set("QT_SCALE_FA
-000001b0: 4354 4f52 222c 2022 3022 290a 0a20 2020  CTOR", "0")..   
-000001c0: 2023 2323 2047 6574 2056 616c 7565 2c20   ### Get Value, 
-000001d0: 6672 6f6d 204b 6579 0a20 2020 202d 2065  from Key.    - e
-000001e0: 2e67 2c20 456e 7656 6172 2e67 6574 2845  .g, EnvVar.get(E
-000001f0: 6e76 5661 7273 2e73 6361 6c65 5f66 6163  nvVars.scale_fac
-00000200: 746f 722c 2022 3022 290a 2020 2020 2d20  tor, "0").    - 
-00000210: 652e 672c 2045 6e76 5661 722e 6765 7428  e.g, EnvVar.get(
-00000220: 2251 545f 5343 414c 455f 4641 4354 4f52  "QT_SCALE_FACTOR
-00000230: 222c 2022 3022 290a 2020 2020 2d20 652e  ", "0").    - e.
-00000240: 672c 2045 6e76 5661 7228 2251 545f 5343  g, EnvVar("QT_SC
-00000250: 414c 455f 4641 4354 4f52 222c 2022 3022  ALE_FACTOR", "0"
-00000260: 290a 2020 2020 4eda 036b 6579 da07 6465  ).    N..key..de
-00000270: 6661 756c 74da 0672 6574 7572 6e63 0300  fault..returnc..
-00000280: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00000290: 0000 4300 0000 730c 0000 007c 00a0 007c  ..C...s....|...|
-000002a0: 017c 02a1 0253 00a9 014e 2901 da03 6765  .|...S...N)...ge
-000002b0: 7429 03da 0473 656c 6672 0800 0000 7209  t)...selfr....r.
-000002c0: 0000 00a9 0072 0e00 0000 fa50 2f68 6f6d  .....r.....P/hom
-000002d0: 652f 6f73 616d 612f 576f 726b 7370 6163  e/osama/Workspac
-000002e0: 652f 2e76 656e 762f 6c69 622f 7079 7468  e/.venv/lib/pyth
-000002f0: 6f6e 332e 3130 2f73 6974 652d 7061 636b  on3.10/site-pack
-00000300: 6167 6573 2f51 7469 6361 2f75 7469 6c73  ages/Qtica/utils
-00000310: 2f5f 656e 765f 7661 722e 7079 da08 5f5f  /_env_var.py..__
-00000320: 6361 6c6c 5f5f 1600 0000 7302 0000 000c  call__....s.....
-00000330: 017a 0f45 6e76 5661 722e 5f5f 6361 6c6c  .z.EnvVar.__call
-00000340: 5f5f da05 7661 6c75 6563 0300 0000 0000  __..valuec......
-00000350: 0000 0000 0000 0300 0000 0500 0000 4300  ..............C.
-00000360: 0000 7332 0000 0074 007c 0274 0183 0272  ..s2...t.|.t...r
-00000370: 087c 026a 026e 017c 0274 036a 0474 007c  .|.j.n.|.t.j.t.|
-00000380: 0174 0583 0272 157c 016a 023c 0064 0053  .t...r.|.j.<.d.S
-00000390: 007c 013c 0064 0053 0072 0b00 0000 2906  .|.<.d.S.r....).
-000003a0: da0a 6973 696e 7374 616e 6365 7202 0000  ..isinstancer...
-000003b0: 0072 1100 0000 da02 6f73 da07 656e 7669  .r......os..envi
-000003c0: 726f 6e72 0600 0000 2903 da03 636c 7372  ronr....)...clsr
-000003d0: 0800 0000 7211 0000 0072 0e00 0000 720e  ....r....r....r.
-000003e0: 0000 0072 0f00 0000 da03 7365 7419 0000  ...r......set...
-000003f0: 0073 1000 0000 0805 08ff 0202 04fc 0801  .s..............
-00000400: 0cff 0202 06fe 7a0a 456e 7656 6172 2e73  ......z.EnvVar.s
-00000410: 6574 6303 0000 0000 0000 0000 0000 0003  etc.............
-00000420: 0000 0004 0000 0043 0000 0073 0e00 0000  .......C...s....
-00000430: 7400 6a01 a002 7c01 7c02 a102 5300 720b  t.j...|.|...S.r.
-00000440: 0000 0029 0372 1300 0000 7214 0000 0072  ...).r....r....r
-00000450: 0c00 0000 2903 7215 0000 0072 0800 0000  ....).r....r....
-00000460: 7209 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
-00000470: 0f00 0000 720c 0000 0021 0000 0073 0200  ....r....!...s..
-00000480: 0000 0e02 7a0a 456e 7656 6172 2e67 6574  ....z.EnvVar.get
-00000490: 720b 0000 0029 0cda 085f 5f6e 616d 655f  r....)...__name_
-000004a0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-000004b0: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
-000004c0: 6f63 5f5f 7204 0000 0072 0600 0000 da03  oc__r....r......
-000004d0: 7374 7272 0300 0000 7210 0000 00da 0b63  strr....r......c
-000004e0: 6c61 7373 6d65 7468 6f64 7216 0000 0072  lassmethodr....r
-000004f0: 0c00 0000 720e 0000 0072 0e00 0000 720e  ....r....r....r.
-00000500: 0000 0072 0f00 0000 7207 0000 000a 0000  ...r....r.......
-00000510: 0073 0e00 0000 0800 0401 200b 0203 2001  .s........ ... .
-00000520: 0207 2601 7207 0000 0029 09da 0465 6e75  ..&.r....)...enu
-00000530: 6d72 0200 0000 da06 7479 7069 6e67 7203  mr......typingr.
-00000540: 0000 0072 0400 0000 da0e 656e 756d 732e  ...r......enums.
-00000550: 656e 765f 7661 7273 7206 0000 0072 1300  env_varsr....r..
-00000560: 0000 7207 0000 0072 0e00 0000 720e 0000  ..r....r....r...
-00000570: 0072 0e00 0000 720f 0000 00da 083c 6d6f  .r....r......<mo
-00000580: 6475 6c65 3e01 0000 0073 0a00 0000 0c03  dule>....s......
-00000590: 1001 0c01 0801 1203                      ........
+00000130: 5300 290e da06 456e 7656 6172 6122 0100  S.)...EnvVara"..
+00000140: 000a 2020 2020 5365 7420 4b65 792c 2061  ..    Set Key, a
+00000150: 6e64 2056 616c 7565 0a20 2020 203e 3e3e  nd Value.    >>>
+00000160: 2045 6e76 5661 722e 7365 7428 456e 7656   EnvVar.set(EnvV
+00000170: 6172 732e 7363 616c 655f 6661 6374 6f72  ars.scale_factor
+00000180: 2c20 2230 2229 0a20 2020 203e 3e3e 2045  , "0").    >>> E
+00000190: 6e76 5661 722e 7365 7428 2251 545f 5343  nvVar.set("QT_SC
+000001a0: 414c 455f 4641 4354 4f52 222c 2022 3022  ALE_FACTOR", "0"
+000001b0: 290a 0a20 2020 2047 6574 2056 616c 7565  )..    Get Value
+000001c0: 2c20 6672 6f6d 204b 6579 0a20 2020 203e  , from Key.    >
+000001d0: 3e3e 2045 6e76 5661 722e 6765 7428 456e  >> EnvVar.get(En
+000001e0: 7656 6172 732e 7363 616c 655f 6661 6374  vVars.scale_fact
+000001f0: 6f72 2c20 2230 2229 0a20 2020 203e 3e3e  or, "0").    >>>
+00000200: 2045 6e76 5661 722e 6765 7428 2251 545f   EnvVar.get("QT_
+00000210: 5343 414c 455f 4641 4354 4f52 222c 2022  SCALE_FACTOR", "
+00000220: 3022 290a 2020 2020 3e3e 3e20 656e 7620  0").    >>> env 
+00000230: 3d20 456e 7656 6172 2829 0a20 2020 203e  = EnvVar().    >
+00000240: 3e3e 2065 6e76 2822 5154 5f53 4341 4c45  >> env("QT_SCALE
+00000250: 5f46 4143 544f 5222 2c20 2230 2229 0a20  _FACTOR", "0"). 
+00000260: 2020 204e da03 6b65 79da 0764 6566 6175     N..key..defau
+00000270: 6c74 da06 7265 7475 726e 6303 0000 0000  lt..returnc.....
+00000280: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
+00000290: 0000 0073 0c00 0000 7c00 a000 7c01 7c02  ...s....|...|.|.
+000002a0: a102 5300 a901 4e29 01da 0367 6574 2903  ..S...N)...get).
+000002b0: da04 7365 6c66 7208 0000 0072 0900 0000  ..selfr....r....
+000002c0: a900 720e 0000 00fa 502f 686f 6d65 2f6f  ..r.....P/home/o
+000002d0: 7361 6d61 2f57 6f72 6b73 7061 6365 2f2e  sama/Workspace/.
+000002e0: 7665 6e76 2f6c 6962 2f70 7974 686f 6e33  venv/lib/python3
+000002f0: 2e31 302f 7369 7465 2d70 6163 6b61 6765  .10/site-package
+00000300: 732f 5174 6963 612f 7574 696c 732f 5f65  s/Qtica/utils/_e
+00000310: 6e76 5f76 6172 2e70 79da 085f 5f63 616c  nv_var.py..__cal
+00000320: 6c5f 5f17 0000 0073 0200 0000 0c01 7a0f  l__....s......z.
+00000330: 456e 7656 6172 2e5f 5f63 616c 6c5f 5fda  EnvVar.__call__.
+00000340: 0576 616c 7565 6303 0000 0000 0000 0000  .valuec.........
+00000350: 0000 0003 0000 0005 0000 0043 0000 0073  ...........C...s
+00000360: 3200 0000 7400 7c02 7401 8302 7208 7c02  2...t.|.t...r.|.
+00000370: 6a02 6e01 7c02 7403 6a04 7400 7c01 7405  j.n.|.t.j.t.|.t.
+00000380: 8302 7215 7c01 6a02 3c00 6400 5300 7c01  ..r.|.j.<.d.S.|.
+00000390: 3c00 6400 5300 720b 0000 0029 06da 0a69  <.d.S.r....)...i
+000003a0: 7369 6e73 7461 6e63 6572 0200 0000 7211  sinstancer....r.
+000003b0: 0000 00da 026f 73da 0765 6e76 6972 6f6e  .....os..environ
+000003c0: 7206 0000 0029 03da 0363 6c73 7208 0000  r....)...clsr...
+000003d0: 0072 1100 0000 720e 0000 0072 0e00 0000  .r....r....r....
+000003e0: 720f 0000 00da 0373 6574 1a00 0000 7310  r......set....s.
+000003f0: 0000 0008 0508 ff02 0204 fc08 010c ff02  ................
+00000400: 0206 fe7a 0a45 6e76 5661 722e 7365 7463  ...z.EnvVar.setc
+00000410: 0300 0000 0000 0000 0000 0000 0300 0000  ................
+00000420: 0400 0000 4300 0000 730e 0000 0074 006a  ....C...s....t.j
+00000430: 01a0 027c 017c 02a1 0253 0072 0b00 0000  ...|.|...S.r....
+00000440: 2903 7213 0000 0072 1400 0000 720c 0000  ).r....r....r...
+00000450: 0029 0372 1500 0000 7208 0000 0072 0900  .).r....r....r..
+00000460: 0000 720e 0000 0072 0e00 0000 720f 0000  ..r....r....r...
+00000470: 0072 0c00 0000 2200 0000 7302 0000 000e  .r...."...s.....
+00000480: 027a 0a45 6e76 5661 722e 6765 7472 0b00  .z.EnvVar.getr..
+00000490: 0000 290c da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
+000004a0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+000004b0: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
+000004c0: 5f72 0400 0000 7206 0000 00da 0373 7472  _r....r......str
+000004d0: 7203 0000 0072 1000 0000 da0b 636c 6173  r....r......clas
+000004e0: 736d 6574 686f 6472 1600 0000 720c 0000  smethodr....r...
+000004f0: 0072 0e00 0000 720e 0000 0072 0e00 0000  .r....r....r....
+00000500: 720f 0000 0072 0700 0000 0a00 0000 730e  r....r........s.
+00000510: 0000 0008 0004 0120 0c02 0320 0102 0726  ....... ... ...&
+00000520: 0172 0700 0000 2909 da04 656e 756d 7202  .r....)...enumr.
+00000530: 0000 00da 0674 7970 696e 6772 0300 0000  .....typingr....
+00000540: 7204 0000 00da 0e65 6e75 6d73 2e65 6e76  r......enums.env
+00000550: 5f76 6172 7372 0600 0000 7213 0000 0072  _varsr....r....r
+00000560: 0700 0000 720e 0000 0072 0e00 0000 720e  ....r....r....r.
+00000570: 0000 0072 0f00 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000580: 653e 0100 0000 730a 0000 000c 0310 010c  e>....s.........
+00000590: 0108 0112 03                             .....
```

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/_env_var.cpython-312.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/_env_var.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/_exception_handler.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/_exception_handler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/_exception_handler.cpython-312.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/_exception_handler.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/_import.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/_import.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/_message_handler.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/_message_handler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/_none_check.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/_none_check.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/_routes.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/_routes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/_text_wrap.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/_text_wrap.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/_text_wrap.cpython-312.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/_text_wrap.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/alignment.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/alignment.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/auto_wrap.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/auto_wrap.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/color.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/color.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/env_var.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/env_var.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/exception_handler.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/exception_handler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/methods.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/methods.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/modifiers.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/modifiers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/multimethod.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/multimethod.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/overload.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/overload.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/qstyle_sheet.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/qstyle_sheet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/qstyle_sheet.cpython-312.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/qstyle_sheet.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/routes.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/routes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/routes.cpython-312.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/routes.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/__pycache__/system.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/__pycache__/system.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/_env_var.py` & `qtica-0.5.0/Qtica/utils/_env_var.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 from typing import Any, Union
 from ..enums.env_vars import EnvVars
 import os
 
 
 class EnvVar:
     '''
-    ### Set Key, and Value
-    - e.g, EnvVar.set(EnvVars.scale_factor, "0")
-    - e.g, EnvVar.set("QT_SCALE_FACTOR", "0")
+    Set Key, and Value
+    >>> EnvVar.set(EnvVars.scale_factor, "0")
+    >>> EnvVar.set("QT_SCALE_FACTOR", "0")
 
-    ### Get Value, from Key
-    - e.g, EnvVar.get(EnvVars.scale_factor, "0")
-    - e.g, EnvVar.get("QT_SCALE_FACTOR", "0")
-    - e.g, EnvVar("QT_SCALE_FACTOR", "0")
+    Get Value, from Key
+    >>> EnvVar.get(EnvVars.scale_factor, "0")
+    >>> EnvVar.get("QT_SCALE_FACTOR", "0")
+    >>> env = EnvVar()
+    >>> env("QT_SCALE_FACTOR", "0")
     '''
 
     def __call__(self, key: Union[EnvVars, str], default: Any = None) -> Any:
         return self.get(key, default)
 
     @classmethod
     def set(cls, key: Union[EnvVars, str], value: Any) -> None:
```

### Comparing `qtica-0.4.3/Qtica/utils/_text_wrap.py` & `qtica-0.5.0/Qtica/utils/_text_wrap.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/__init__.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/__init__.cpython-312.pyc` & `qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/boundaries.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/boundaries.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/boundaries.cpython-312.pyc` & `qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/boundaries.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/camel.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/camel.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/camel.cpython-312.pyc` & `qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/camel.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/caseconverter.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/caseconverter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/caseconverter.cpython-312.pyc` & `qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/caseconverter.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/cobol.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/cobol.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/cobol.cpython-312.pyc` & `qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/cobol.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/flat.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/flat.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/flat.cpython-312.pyc` & `qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/flat.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/kebab.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/kebab.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/kebab.cpython-312.pyc` & `qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/kebab.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/macro.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/macro.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/macro.cpython-312.pyc` & `qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/macro.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/pascal.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/pascal.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/pascal.cpython-312.pyc` & `qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/pascal.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/snake.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/snake.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/__pycache__/snake.cpython-312.pyc` & `qtica-0.5.0/Qtica/utils/caseconverter/__pycache__/snake.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/boundaries.py` & `qtica-0.5.0/Qtica/utils/caseconverter/boundaries.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/camel.py` & `qtica-0.5.0/Qtica/utils/caseconverter/camel.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/caseconverter.py` & `qtica-0.5.0/Qtica/utils/caseconverter/caseconverter.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/cobol.py` & `qtica-0.5.0/Qtica/utils/caseconverter/cobol.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/flat.py` & `qtica-0.5.0/Qtica/utils/caseconverter/flat.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/kebab.py` & `qtica-0.5.0/Qtica/utils/caseconverter/kebab.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/macro.py` & `qtica-0.5.0/Qtica/utils/caseconverter/macro.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/pascal.py` & `qtica-0.5.0/Qtica/utils/caseconverter/pascal.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/caseconverter/snake.py` & `qtica-0.5.0/Qtica/utils/caseconverter/snake.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/maths/__init__.py` & `qtica-0.5.0/Qtica/utils/maths/__init__.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/maths/__pycache__/__init__.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/maths/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/maths/__pycache__/__init__.cpython-312.pyc` & `qtica-0.5.0/Qtica/utils/maths/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/maths/__pycache__/geometry.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/maths/__pycache__/geometry.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/maths/__pycache__/geometry.cpython-312.pyc` & `qtica-0.5.0/Qtica/utils/maths/__pycache__/geometry.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/maths/__pycache__/vector.cpython-310.pyc` & `qtica-0.5.0/Qtica/utils/maths/__pycache__/vector.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/maths/__pycache__/vector.cpython-312.pyc` & `qtica-0.5.0/Qtica/utils/maths/__pycache__/vector.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/maths/geometry.py` & `qtica-0.5.0/Qtica/utils/maths/geometry.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/utils/maths/vector.py` & `qtica-0.5.0/Qtica/utils/maths/vector.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/__init__.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb  6 15:28:39 2024 UTC, .py size: 613 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,63 @@
-00000000: 6f0d 0d0a 0000 0000 2750 c265 6502 0000  o.......'P.ee...
+00000000: 6f0d 0d0a 0000 0000 d521 0766 8b02 0000  o........!.f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 dc00 0000 6400  .....@...s....d.
+00000020: 0002 0000 0040 0000 0073 e800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5400 6400 6401 6c01 5400 6400  d.l.T.d.d.l.T.d.
 00000040: 6401 6c02 5400 6400 6402 6c03 6d04 5a04  d.l.T.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 0100 6400 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6400 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000080: 0100 6400 6407 6c0d 6d0e 5a0e 6d0f 5a0f  ..d.d.l.m.Z.m.Z.
 00000090: 6d10 5a10 0100 6400 6408 6c11 6d12 5a12  m.Z...d.d.l.m.Z.
 000000a0: 6d13 5a13 0100 6400 6409 6c14 6d15 5a15  m.Z...d.d.l.m.Z.
 000000b0: 6d16 5a16 0100 6400 640a 6c17 6d18 5a18  m.Z...d.d.l.m.Z.
 000000c0: 0100 6400 640b 6c19 6d1a 5a1a 6d1b 5a1b  ..d.d.l.m.Z.m.Z.
 000000d0: 6d1c 5a1c 0100 6400 640c 6c1d 6d1e 5a1e  m.Z...d.d.l.m.Z.
 000000e0: 0100 6400 640d 6c1f 6d20 5a20 0100 6400  ..d.d.l.m Z ..d.
 000000f0: 640e 6c21 6d22 5a22 0100 6400 640f 6c23  d.l!m"Z"..d.d.l#
-00000100: 6d24 5a24 0100 6410 5300 2911 e901 0000  m$Z$..d.S.).....
-00000110: 0029 01da 012a 2901 da04 4d65 6e75 2901  .)...*)...Menu).
-00000120: da05 4c61 6265 6c29 01da 0553 7461 636b  ..Label)...Stack
-00000130: 2901 da0a 5363 726f 6c6c 4172 6561 2901  )...ScrollArea).
-00000140: da0a 4963 6f6e 5769 6467 6574 2903 da04  ..IconWidget)...
-00000150: 4c69 6e65 da05 484c 696e 65da 0556 4c69  Line..HLine..VLi
-00000160: 6e65 2902 da0a 5075 7368 4275 7474 6f6e  ne)...PushButton
-00000170: da0a 546f 6f6c 4275 7474 6f6e 2902 da0b  ..ToolButton)...
-00000180: 4170 706c 6963 6174 696f 6eda 0341 7070  Application..App
-00000190: 2901 da0d 5374 6163 6b65 6457 6964 6765  )...StackedWidge
-000001a0: 7429 03da 0943 6f6e 7461 696e 6572 da0e  t)...Container..
-000001b0: 4672 616d 6543 6f6e 7461 696e 6572 da0f  FrameContainer..
-000001c0: 5769 6467 6574 436f 6e74 6169 6e65 7229  WidgetContainer)
-000001d0: 01da 0e57 696e 646f 7753 697a 6547 7269  ...WindowSizeGri
-000001e0: 7029 01da 0847 726f 7570 426f 7829 01da  p)...GroupBox)..
-000001f0: 0c45 6c69 6469 6e67 4c61 6265 6c29 01da  .ElidingLabel)..
-00000200: 0b56 6964 656f 5769 6467 6574 4e29 25da  .VideoWidgetN)%.
-00000210: 0677 696e 646f 77da 0764 6961 6c6f 6773  .window..dialogs
-00000220: da08 5f77 6964 6765 7473 da04 6d65 6e75  .._widgets..menu
-00000230: 7203 0000 00da 056c 6162 656c 7204 0000  r......labelr...
-00000240: 00da 0573 7461 636b 7205 0000 00da 0b73  ...stackr......s
-00000250: 6372 6f6c 6c5f 6172 6561 7206 0000 00da  croll_arear.....
-00000260: 0b69 636f 6e5f 7769 6467 6574 7207 0000  .icon_widgetr...
-00000270: 00da 046c 696e 6572 0800 0000 7209 0000  ...liner....r...
-00000280: 0072 0a00 0000 da07 6275 7474 6f6e 7372  .r......buttonsr
-00000290: 0b00 0000 720c 0000 00da 0b61 7070 6c69  ....r......appli
-000002a0: 6361 7469 6f6e 720d 0000 0072 0e00 0000  cationr....r....
-000002b0: da0e 7374 6163 6b65 645f 7769 6467 6574  ..stacked_widget
-000002c0: 720f 0000 00da 0963 6f6e 7461 696e 6572  r......container
-000002d0: 7210 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
-000002e0: 0973 697a 655f 6772 6970 7213 0000 00da  .size_gripr.....
-000002f0: 0967 726f 7570 5f62 6f78 7214 0000 00da  .group_boxr.....
-00000300: 0d65 6c69 6469 6e67 5f6c 6162 656c 7215  .eliding_labelr.
-00000310: 0000 00da 0c76 6964 656f 5f77 6964 6765  .....video_widge
-00000320: 7472 1600 0000 a900 7228 0000 0072 2800  tr......r(...r(.
-00000330: 0000 fa52 2f68 6f6d 652f 6f73 616d 612f  ...R/home/osama/
-00000340: 576f 726b 7370 6163 652f 2e76 656e 762f  Workspace/.venv/
-00000350: 6c69 622f 7079 7468 6f6e 332e 3130 2f73  lib/python3.10/s
-00000360: 6974 652d 7061 636b 6167 6573 2f51 7469  ite-packages/Qti
-00000370: 6361 2f77 6964 6765 7473 2f5f 5f69 6e69  ca/widgets/__ini
-00000380: 745f 5f2e 7079 da08 3c6d 6f64 756c 653e  t__.py..<module>
-00000390: 0100 0000 7322 0000 0008 0208 0108 010c  ....s"..........
-000003a0: 020c 010c 010c 010c 0114 0110 0110 010c  ................
-000003b0: 0114 010c 010c 010c 0110 01              ...........
+00000100: 6d24 5a24 0100 6400 6410 6c25 6d26 5a26  m$Z$..d.d.l%m&Z&
+00000110: 0100 6411 5300 2912 e901 0000 0029 01da  ..d.S.)......)..
+00000120: 012a 2901 da04 4d65 6e75 2901 da05 4c61  .*)...Menu)...La
+00000130: 6265 6c29 01da 0553 7461 636b 2901 da0a  bel)...Stack)...
+00000140: 5363 726f 6c6c 4172 6561 2901 da0a 4963  ScrollArea)...Ic
+00000150: 6f6e 5769 6467 6574 2903 da04 4c69 6e65  onWidget)...Line
+00000160: da05 484c 696e 65da 0556 4c69 6e65 2902  ..HLine..VLine).
+00000170: da0a 5075 7368 4275 7474 6f6e da0a 546f  ..PushButton..To
+00000180: 6f6c 4275 7474 6f6e 2902 da0b 4170 706c  olButton)...Appl
+00000190: 6963 6174 696f 6eda 0341 7070 2901 da0d  ication..App)...
+000001a0: 5374 6163 6b65 6457 6964 6765 7429 03da  StackedWidget)..
+000001b0: 0943 6f6e 7461 696e 6572 da0e 4672 616d  .Container..Fram
+000001c0: 6543 6f6e 7461 696e 6572 da0f 5769 6467  eContainer..Widg
+000001d0: 6574 436f 6e74 6169 6e65 7229 01da 0e57  etContainer)...W
+000001e0: 696e 646f 7753 697a 6547 7269 7029 01da  indowSizeGrip)..
+000001f0: 0847 726f 7570 426f 7829 01da 0c45 6c69  .GroupBox)...Eli
+00000200: 6469 6e67 4c61 6265 6c29 01da 0b56 6964  dingLabel)...Vid
+00000210: 656f 5769 6467 6574 2901 da0b 5175 6963  eoWidget)...Quic
+00000220: 6b57 6964 6765 744e 2927 da06 7769 6e64  kWidgetN)'..wind
+00000230: 6f77 da07 6469 616c 6f67 73da 085f 7769  ow..dialogs.._wi
+00000240: 6467 6574 73da 046d 656e 7572 0300 0000  dgets..menur....
+00000250: da05 6c61 6265 6c72 0400 0000 da05 7374  ..labelr......st
+00000260: 6163 6b72 0500 0000 da0b 7363 726f 6c6c  ackr......scroll
+00000270: 5f61 7265 6172 0600 0000 da0b 6963 6f6e  _arear......icon
+00000280: 5f77 6964 6765 7472 0700 0000 da04 6c69  _widgetr......li
+00000290: 6e65 7208 0000 0072 0900 0000 720a 0000  ner....r....r...
+000002a0: 00da 0762 7574 746f 6e73 720b 0000 0072  ...buttonsr....r
+000002b0: 0c00 0000 da0b 6170 706c 6963 6174 696f  ......applicatio
+000002c0: 6e72 0d00 0000 720e 0000 00da 0e73 7461  nr....r......sta
+000002d0: 636b 6564 5f77 6964 6765 7472 0f00 0000  cked_widgetr....
+000002e0: da09 636f 6e74 6169 6e65 7272 1000 0000  ..containerr....
+000002f0: 7211 0000 0072 1200 0000 da09 7369 7a65  r....r......size
+00000300: 5f67 7269 7072 1300 0000 da09 6772 6f75  _gripr......grou
+00000310: 705f 626f 7872 1400 0000 da0d 656c 6964  p_boxr......elid
+00000320: 696e 675f 6c61 6265 6c72 1500 0000 da0c  ing_labelr......
+00000330: 7669 6465 6f5f 7769 6467 6574 7216 0000  video_widgetr...
+00000340: 00da 0c71 7569 636b 5f77 6964 6765 7472  ...quick_widgetr
+00000350: 1700 0000 a900 722a 0000 0072 2a00 0000  ......r*...r*...
+00000360: fa52 2f68 6f6d 652f 6f73 616d 612f 576f  .R/home/osama/Wo
+00000370: 726b 7370 6163 652f 2e76 656e 762f 6c69  rkspace/.venv/li
+00000380: 622f 7079 7468 6f6e 332e 3130 2f73 6974  b/python3.10/sit
+00000390: 652d 7061 636b 6167 6573 2f51 7469 6361  e-packages/Qtica
+000003a0: 2f77 6964 6765 7473 2f5f 5f69 6e69 745f  /widgets/__init_
+000003b0: 5f2e 7079 da08 3c6d 6f64 756c 653e 0100  _.py..<module>..
+000003c0: 0000 7324 0000 0008 0208 0108 010c 020c  ..s$............
+000003d0: 010c 010c 010c 0114 0110 0110 010c 0114  ................
+000003e0: 010c 010c 010c 010c 0110 01              ...........
```

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/__init__.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/_widgets.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/_widgets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/application.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/application.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Feb 14 18:57:24 2024 UTC, .py size: 3396 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,265 +1,264 @@
-00000000: 6f0d 0d0a 0000 0000 140d cd65 440d 0000  o..........eD...
+00000000: 6f0d 0d0a 0000 0000 f821 0766 3a0d 0000  o........!.f:...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
+00000020: 0005 0000 0040 0000 0073 9a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
-00000050: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
-00000060: 0100 6400 6403 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
-00000070: 6d0c 5a0c 6d0d 5a0d 0100 6400 6404 6c0e  m.Z.m.Z...d.d.l.
-00000080: 6d0f 5a0f 6d10 5a10 6d11 5a11 0100 6400  m.Z.m.Z.m.Z...d.
-00000090: 6405 6c12 6d13 5a13 0100 6406 6407 6c14  d.l.m.Z...d.d.l.
-000000a0: 6d15 5a15 0100 4700 6408 6409 8400 6409  m.Z...G.d.d...d.
-000000b0: 6515 650f 8304 5a16 4700 640a 640b 8400  e.e...Z.G.d.d...
-000000c0: 640b 6516 8303 5a17 6401 5300 290c e900  d.e...Z.d.S.)...
-000000d0: 0000 004e 2905 da08 4361 6c6c 6162 6c65  ...N)...Callable
-000000e0: da08 4e6f 5265 7475 726e da08 4f70 7469  ..NoReturn..Opti
-000000f0: 6f6e 616c da08 5365 7175 656e 6365 da05  onal..Sequence..
-00000100: 556e 696f 6e29 04da 0951 5265 736f 7572  Union)...QResour
-00000110: 6365 da02 5174 da06 5369 676e 616c da15  ce..Qt..Signal..
-00000120: 7152 6567 6973 7465 7252 6573 6f75 7263  qRegisterResourc
-00000130: 6544 6174 6129 03da 0c51 4170 706c 6963  eData)...QApplic
-00000140: 6174 696f 6eda 0d51 5374 796c 6546 6163  ation..QStyleFac
-00000150: 746f 7279 da07 5157 6964 6765 7429 01da  tory..QWidget)..
-00000160: 0d51 466f 6e74 4461 7461 6261 7365 e902  .QFontDatabase..
-00000170: 0000 0029 01da 0f41 6273 7472 6163 7451  ...)...AbstractQ
-00000180: 4f62 6a65 6374 6300 0000 0000 0000 0000  Objectc.........
-00000190: 0000 0000 0000 000a 0000 0000 0000 0073  ...............s
-000001a0: 4201 0000 6500 5a01 6400 5a02 6503 8300  B...e.Z.d.Z.e...
-000001b0: 5a04 6503 8300 5a05 6503 8300 5a06 6503  Z.e...Z.e...Z.e.
-000001c0: 8300 5a07 6401 6401 6402 9c02 6403 6508  ..Z.d.d.d...d.e.
-000001d0: 6509 650a 650b 650c 650d 1900 650e 650e  e.e.e.e.e...e.e.
-000001e0: 650e 6604 1900 6602 1900 1900 6404 6508  e.f...f.....d.e.
-000001f0: 650a 1900 6604 8700 6601 6405 6406 840e  e...f...f.d.d...
-00000200: 5a0f 6423 6408 6409 8404 5a10 6424 640b  Z.d#d.d...Z.d$d.
-00000210: 6511 6407 6512 6604 640c 640d 8405 5a13  e.d.e.f.d.d...Z.
-00000220: 6407 6508 650a 1900 6602 640e 640f 8404  d.e.e...f.d.d...
-00000230: 5a14 6407 650a 6602 6410 6411 8404 5a15  Z.d.e.f.d.d...Z.
-00000240: 0901 6425 6412 650a 6413 650a 6407 6511  ..d%d.e.d.e.d.e.
-00000250: 6606 6414 6415 8405 5a16 6416 650a 6407  f.d.d...Z.d.e.d.
-00000260: 650d 6604 6417 6418 8404 5a17 6404 6508  e.f.d.d...Z.d.e.
-00000270: 650a 1900 6602 6419 641a 8404 5a18 6403  e...f.d.d...Z.d.
-00000280: 6508 6509 6519 650b 650c 650d 1900 650e  e.e.e.e.e.e...e.
-00000290: 650e 650e 6604 1900 6602 1900 1900 6602  e.e.f...f.....f.
-000002a0: 641b 641c 8404 5a1a 651b 6407 651c 6602  d.d...Z.e.d.e.f.
-000002b0: 641d 641e 8404 8301 5a1d 651b 6407 651c  d.d.....Z.e.d.e.
-000002c0: 6602 641f 6420 8404 8301 5a1e 651b 6407  f.d.d ....Z.e.d.
-000002d0: 651c 6602 6421 6422 8404 8301 5a1f 8700  e.f.d!d"....Z...
-000002e0: 0400 5a20 5300 2926 da0b 4170 706c 6963  ..Z S.)&..Applic
-000002f0: 6174 696f 6e4e 2902 da09 7265 736f 7572  ationN)...resour
-00000300: 6365 73da 0566 6f6e 7473 7212 0000 0072  ces..fontsr....r
-00000310: 1300 0000 6301 0000 0000 0000 0002 0000  ....c...........
-00000320: 0005 0000 0004 0000 000f 0000 0073 5a00  .............sZ.
-00000330: 0000 7400 6a01 7c00 6701 7c03 a201 5200  ..t.j.|.g.|...R.
-00000340: 8e00 0100 7c01 6400 7501 7212 7c00 a002  ....|.d.u.r.|...
-00000350: 7c01 a101 0100 7c02 6400 7501 721b 7c00  |.....|.d.u.r.|.
-00000360: a003 7c02 a101 0100 7404 8300 6a01 6401  ..|.....t...j.d.
-00000370: 6900 7c04 a401 8e01 0100 7c00 6a05 a006  i.|.......|.j...
-00000380: 7c00 6a07 a101 0100 6400 5300 2902 4ea9  |.j.....d.S.).N.
-00000390: 0029 0872 0b00 0000 da08 5f5f 696e 6974  .).r......__init
-000003a0: 5f5f da0e 5f73 6574 5f72 6573 6f75 7263  __.._set_resourc
-000003b0: 6573 da0a 5f73 6574 5f66 6f6e 7473 da05  es.._set_fonts..
-000003c0: 7375 7065 72da 1761 7070 6c69 6361 7469  super..applicati
-000003d0: 6f6e 5374 6174 6543 6861 6e67 6564 da07  onStateChanged..
-000003e0: 636f 6e6e 6563 74da 185f 6170 706c 6963  connect.._applic
-000003f0: 6174 696f 6e53 7461 7465 4368 616e 6765  ationStateChange
-00000400: 6429 05da 0473 656c 6672 1200 0000 7213  d)...selfr....r.
-00000410: 0000 00da 0461 7267 73da 066b 7761 7267  .....args..kwarg
-00000420: 73a9 01da 095f 5f63 6c61 7373 5f5f 7214  s....__class__r.
-00000430: 0000 00fa 552f 686f 6d65 2f6f 7361 6d61  ....U/home/osama
-00000440: 2f57 6f72 6b73 7061 6365 2f2e 7665 6e76  /Workspace/.venv
-00000450: 2f6c 6962 2f70 7974 686f 6e33 2e31 302f  /lib/python3.10/
-00000460: 7369 7465 2d70 6163 6b61 6765 732f 5174  site-packages/Qt
-00000470: 6963 612f 7769 6467 6574 732f 6170 706c  ica/widgets/appl
-00000480: 6963 6174 696f 6e2e 7079 7215 0000 0013  ication.pyr.....
-00000490: 0000 0073 0e00 0000 1205 0802 0a01 0802  ...s............
-000004a0: 0a01 1202 1202 7a14 4170 706c 6963 6174  ......z.Applicat
-000004b0: 696f 6e2e 5f5f 696e 6974 5f5f da06 7265  ion.__init__..re
-000004c0: 7475 726e 6302 0000 0000 0000 0000 0000  turnc...........
-000004d0: 0002 0000 0002 0000 0043 0000 0073 6c00  .........C...sl.
-000004e0: 0000 7c01 7400 6a01 6a02 6b02 720d 7c00  ..|.t.j.j.k.r.|.
-000004f0: 6a03 a004 a100 0100 6400 5300 7c01 7400  j.......d.S.|.t.
-00000500: 6a01 6a05 6b02 721a 7c00 6a06 a004 a100  j.j.k.r.|.j.....
-00000510: 0100 6400 5300 7c01 7400 6a01 6a07 6b02  ..d.S.|.t.j.j.k.
-00000520: 7227 7c00 6a08 a004 a100 0100 6400 5300  r'|.j.......d.S.
-00000530: 7c01 7400 6a01 6a09 6b02 7234 7c00 6a0a  |.t.j.j.k.r4|.j.
-00000540: a004 a100 0100 6400 5300 6400 5300 a901  ......d.S.d.S...
-00000550: 4e29 0b72 0800 0000 da10 4170 706c 6963  N).r......Applic
-00000560: 6174 696f 6e53 7461 7465 da13 4170 706c  ationState..Appl
-00000570: 6963 6174 696f 6e49 6e61 6374 6976 65da  icationInactive.
-00000580: 0b6f 6e5f 696e 6163 7469 7665 da04 656d  .on_inactive..em
-00000590: 6974 da11 4170 706c 6963 6174 696f 6e41  it..ApplicationA
-000005a0: 6374 6976 65da 096f 6e5f 6163 7469 7665  ctive..on_active
-000005b0: da11 4170 706c 6963 6174 696f 6e48 6964  ..ApplicationHid
-000005c0: 6465 6eda 096f 6e5f 6869 6464 656e da14  den..on_hidden..
-000005d0: 4170 706c 6963 6174 696f 6e53 7573 7065  ApplicationSuspe
-000005e0: 6e64 6564 da0a 6f6e 5f73 7573 7065 6e64  nded..on_suspend
-000005f0: 2902 721c 0000 00da 0565 7665 6e74 7214  ).r......eventr.
-00000600: 0000 0072 1400 0000 7221 0000 0072 1b00  ...r....r!...r..
-00000610: 0000 2400 0000 7312 0000 000c 010e 010c  ..$...s.........
-00000620: 010e 010c 010e 010c 010e 0104 ff7a 2441  .............z$A
-00000630: 7070 6c69 6361 7469 6f6e 2e5f 6170 706c  pplication._appl
-00000640: 6963 6174 696f 6e53 7461 7465 4368 616e  icationStateChan
-00000650: 6765 6446 da09 7465 726d 5f65 7869 7463  gedF..term_exitc
-00000660: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000670: 0400 0000 4300 0000 7322 0000 007c 0172  ....C...s"...|.r
-00000680: 0a74 00a0 0074 006a 0174 006a 02a1 0201  .t...t.j.t.j....
-00000690: 0074 03a0 047c 00a0 05a1 00a1 0153 0072  .t...|.......S.r
-000006a0: 2300 0000 2906 da06 7369 676e 616c da06  #...)...signal..
-000006b0: 5349 4749 4e54 da07 5349 475f 4446 4cda  SIGINT..SIG_DFL.
-000006c0: 0373 7973 da04 6578 6974 da04 6578 6563  .sys..exit..exec
-000006d0: 2902 721c 0000 0072 2f00 0000 7214 0000  ).r....r/...r...
-000006e0: 0072 1400 0000 7221 0000 00da 0372 756e  .r....r!.....run
-000006f0: 2e00 0000 7306 0000 0004 0110 010e 017a  ....s..........z
-00000700: 0f41 7070 6c69 6361 7469 6f6e 2e72 756e  .Application.run
-00000710: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000720: 0002 0000 0043 0000 00f3 0800 0000 7400  .....C........t.
-00000730: a001 a100 5300 7223 0000 0029 0272 0c00  ....S.r#...).r..
-00000740: 0000 da04 6b65 7973 a901 721c 0000 0072  ....keys..r....r
-00000750: 1400 0000 7214 0000 0072 2100 0000 da0a  ....r....r!.....
-00000760: 7374 796c 655f 6c69 7374 3300 0000 7302  style_list3...s.
-00000770: 0000 0008 017a 1641 7070 6c69 6361 7469  .....z.Applicati
-00000780: 6f6e 2e73 7479 6c65 5f6c 6973 7463 0100  on.style_listc..
-00000790: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-000007a0: 0000 4300 0000 730c 0000 007c 00a0 00a1  ..C...s....|....
-000007b0: 00a0 01a1 0053 0072 2300 0000 2902 da05  .....S.r#...)...
-000007c0: 7374 796c 65da 046e 616d 6572 3900 0000  style..namer9...
-000007d0: 7214 0000 0072 1400 0000 7221 0000 00da  r....r....r!....
-000007e0: 0d63 7572 7265 6e74 5f73 7479 6c65 3600  .current_style6.
-000007f0: 0000 7302 0000 000c 017a 1941 7070 6c69  ..s......z.Appli
-00000800: 6361 7469 6f6e 2e63 7572 7265 6e74 5f73  cation.current_s
-00000810: 7479 6c65 da08 7263 635f 6669 6c65 da08  tyle..rcc_file..
-00000820: 7263 635f 726f 6f74 6303 0000 0000 0000  rcc_rootc.......
-00000830: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
-00000840: 0073 1e00 0000 7c02 6400 7501 720a 7400  .s....|.d.u.r.t.
-00000850: a001 7c01 7c02 a102 5300 7400 a001 7c01  ..|.|...S.t...|.
-00000860: a101 5300 7223 0000 0029 0272 0700 0000  ..S.r#...).r....
-00000870: da10 7265 6769 7374 6572 5265 736f 7572  ..registerResour
-00000880: 6365 2903 721c 0000 0072 3e00 0000 723f  ce).r....r>...r?
-00000890: 0000 0072 1400 0000 7214 0000 0072 2100  ...r....r....r!.
-000008a0: 0000 da0c 6164 645f 7263 635f 6669 6c65  ....add_rcc_file
-000008b0: 3900 0000 7306 0000 0008 030c 010a 017a  9...s..........z
-000008c0: 1841 7070 6c69 6361 7469 6f6e 2e61 6464  .Application.add
-000008d0: 5f72 6363 5f66 696c 65da 0866 6f6e 7470  _rcc_file..fontp
-000008e0: 6174 6863 0200 0000 0000 0000 0000 0000  athc............
-000008f0: 0200 0000 0300 0000 4300 0000 730a 0000  ........C...s...
-00000900: 0074 00a0 017c 01a1 0153 0072 2300 0000  .t...|...S.r#...
-00000910: 2902 720e 0000 00da 1261 6464 4170 706c  ).r......addAppl
-00000920: 6963 6174 696f 6e46 6f6e 7429 0272 1c00  icationFont).r..
-00000930: 0000 7242 0000 0072 1400 0000 7214 0000  ..rB...r....r...
-00000940: 0072 2100 0000 da08 6164 645f 666f 6e74  .r!.....add_font
-00000950: 4000 0000 7302 0000 000a 017a 1441 7070  @...s......z.App
-00000960: 6c69 6361 7469 6f6e 2e61 6464 5f66 6f6e  lication.add_fon
-00000970: 7463 0200 0000 0000 0000 0000 0000 0300  tc..............
-00000980: 0000 0500 0000 4300 0000 7334 0000 007c  ......C...s4...|
-00000990: 0144 005d 157d 0274 006a 01a0 027c 02a1  .D.].}.t.j...|..
-000009a0: 0173 1274 0364 017c 029b 0064 029d 0383  .s.t.d.|...d....
-000009b0: 0182 017c 00a0 047c 01a1 0101 0071 0264  ...|...|.....q.d
-000009c0: 0053 0029 034e fa01 277a 1627 2066 6f6e  .S.).N..'z.' fon
-000009d0: 7420 6669 6c65 206e 6f74 2066 6f75 6e64  t file not found
-000009e0: 2129 05da 026f 73da 0470 6174 68da 0665  !)...os..path..e
-000009f0: 7869 7374 73da 1146 696c 654e 6f74 466f  xists..FileNotFo
-00000a00: 756e 6445 7272 6f72 7244 0000 0029 0372  undErrorrD...).r
-00000a10: 1c00 0000 7213 0000 00da 0466 6f6e 7472  ....r......fontr
-00000a20: 1400 0000 7214 0000 0072 2100 0000 7217  ....r....r!...r.
-00000a30: 0000 0043 0000 0073 0a00 0000 0801 0c01  ...C...s........
-00000a40: 1001 0c02 04fc 7a16 4170 706c 6963 6174  ......z.Applicat
-00000a50: 696f 6e2e 5f73 6574 5f66 6f6e 7473 6302  ion._set_fontsc.
-00000a60: 0000 0000 0000 0000 0000 0003 0000 0009  ................
-00000a70: 0000 0043 0000 0073 9200 0000 7c01 4400  ...C...s....|.D.
-00000a80: 5d44 7d02 7400 7c02 7401 7402 7403 6603  ]D}.t.|.t.t.t.f.
-00000a90: 8302 7233 7404 7c02 8301 6401 6b00 721c  ..r3t.|...d.k.r.
-00000aa0: 7402 7c02 8301 7d02 7c02 a005 6402 6403  t.|...}.|...d.d.
-00000ab0: a102 0100 7406 7c02 6402 1900 6404 7501  ....t.|.d...d.u.
-00000ac0: 7227 7c02 6402 1900 6e01 6403 6701 7c02  r'|.d...n.d.g.|.
-00000ad0: 6405 6404 8502 1900 a201 5200 8e00 0100  d.d.......R.....
-00000ae0: 7102 7407 7c02 8301 7246 7a05 7c02 8300  q.t.|...rFz.|...
-00000af0: 0100 5700 7102 0400 7408 7945 0100 0100  ..W.q...t.yE....
-00000b00: 0100 5900 7102 7700 7102 6404 5300 2906  ..Y.q.w.q.d.S.).
-00000b10: 7aa2 0a20 2020 2020 2020 203a 7061 7261  z..        :para
-00000b20: 6d3a 2072 6573 6f75 7263 650a 2020 2020  m: resource.    
-00000b30: 2020 2020 2020 2020 6361 6c6c 6162 6c65          callable
-00000b40: 203d 2071 496e 6974 5265 736f 7572 6365   = qInitResource
-00000b50: 730a 2020 2020 2020 2020 2020 2020 7475  s.            tu
-00000b60: 706c 6520 3d20 2830 7830 3320 7c20 4e6f  ple = (0x03 | No
-00000b70: 6e65 2c20 7174 5f72 6573 6f75 7263 655f  ne, qt_resource_
-00000b80: 7374 7275 6374 2c20 7174 5f72 6573 6f75  struct, qt_resou
-00000b90: 7263 655f 6e61 6d65 2c20 7174 5f72 6573  rce_name, qt_res
-00000ba0: 6f75 7263 655f 6461 7461 290a 2020 2020  ource_data).    
-00000bb0: 2020 2020 e904 0000 0072 0100 0000 e903      .....r......
-00000bc0: 0000 004e e901 0000 0029 09da 0a69 7369  ...N.....)...isi
-00000bd0: 6e73 7461 6e63 65da 0574 7570 6c65 da04  nstance..tuple..
-00000be0: 6c69 7374 da03 7365 74da 036c 656e da06  list..set..len..
-00000bf0: 696e 7365 7274 720a 0000 00da 0863 616c  insertr......cal
-00000c00: 6c61 626c 65da 0945 7863 6570 7469 6f6e  lable..Exception
-00000c10: 2903 721c 0000 0072 1200 0000 da03 7265  ).r....r......re
-00000c20: 7372 1400 0000 7214 0000 0072 2100 0000  sr....r....r!...
-00000c30: 7216 0000 004a 0000 0073 1c00 0000 0806  r....J...s......
-00000c40: 1001 0c01 0801 0c01 2e01 0801 0201 0a01  ................
-00000c50: 0c01 0401 02ff 02fd 04fa 7a1a 4170 706c  ..........z.Appl
-00000c60: 6963 6174 696f 6e2e 5f73 6574 5f72 6573  ication._set_res
-00000c70: 6f75 7263 6573 6300 0000 0000 0000 0000  ourcesc.........
-00000c80: 0000 0000 0000 0002 0000 0043 0000 0072  ...........C...r
-00000c90: 3700 0000 7223 0000 0029 0272 0b00 0000  7...r#...).r....
-00000ca0: da0c 6163 7469 7665 5769 6e64 6f77 7214  ..activeWindowr.
-00000cb0: 0000 0072 1400 0000 7214 0000 0072 2100  ...r....r....r!.
-00000cc0: 0000 da0d 6163 7469 7665 5f77 696e 646f  ....active_windo
-00000cd0: 775c 0000 00f3 0200 0000 0802 7a19 4170  w\..........z.Ap
-00000ce0: 706c 6963 6174 696f 6e2e 6163 7469 7665  plication.active
-00000cf0: 5f77 696e 646f 7763 0000 0000 0000 0000  _windowc........
-00000d00: 0000 0000 0000 0000 0200 0000 4300 0000  ............C...
-00000d10: 7237 0000 0072 2300 0000 2902 720b 0000  r7...r#...).r...
-00000d20: 00da 1161 6374 6976 654d 6f64 616c 5769  ...activeModalWi
-00000d30: 6467 6574 7214 0000 0072 1400 0000 7214  dgetr....r....r.
-00000d40: 0000 0072 2100 0000 da0c 6163 7469 7665  ...r!.....active
-00000d50: 5f6d 6f64 616c 6000 0000 7259 0000 007a  _modal`...rY...z
-00000d60: 1841 7070 6c69 6361 7469 6f6e 2e61 6374  .Application.act
-00000d70: 6976 655f 6d6f 6461 6c63 0000 0000 0000  ive_modalc......
-00000d80: 0000 0000 0000 0000 0000 0200 0000 4300  ..............C.
-00000d90: 0000 7237 0000 0072 2300 0000 2902 720b  ..r7...r#...).r.
-00000da0: 0000 00da 1161 6374 6976 6550 6f70 7570  .....activePopup
-00000db0: 5769 6467 6574 7214 0000 0072 1400 0000  Widgetr....r....
-00000dc0: 7214 0000 0072 2100 0000 da0c 6163 7469  r....r!.....acti
-00000dd0: 7665 5f70 6f70 7570 6400 0000 7259 0000  ve_popupd...rY..
-00000de0: 007a 1841 7070 6c69 6361 7469 6f6e 2e61  .z.Application.a
-00000df0: 6374 6976 655f 706f 7075 7029 0272 2200  ctive_popup).r".
-00000e00: 0000 4e29 0146 7223 0000 0029 21da 085f  ..N).Fr#...)!.._
-00000e10: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000e20: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000e30: 5f72 0900 0000 7226 0000 0072 2900 0000  _r....r&...r)...
-00000e40: 722b 0000 0072 2d00 0000 7250 0000 0072  r+...r-...rP...r
-00000e50: 0600 0000 da03 7374 7272 4f00 0000 7204  ......strrO...r.
-00000e60: 0000 00da 0369 6e74 da05 6279 7465 7372  .....int..bytesr
-00000e70: 1500 0000 721b 0000 00da 0462 6f6f 6c72  ....r......boolr
-00000e80: 0300 0000 7236 0000 0072 3a00 0000 723d  ....r6...r:...r=
-00000e90: 0000 0072 4100 0000 7244 0000 0072 1700  ...rA...rD...r..
-00000ea0: 0000 7202 0000 0072 1600 0000 da0c 7374  ..r....r......st
-00000eb0: 6174 6963 6d65 7468 6f64 720d 0000 0072  aticmethodr....r
-00000ec0: 5800 0000 725b 0000 0072 5d00 0000 da0d  X...r[...r].....
-00000ed0: 5f5f 636c 6173 7363 656c 6c5f 5f72 1400  __classcell__r..
-00000ee0: 0000 7214 0000 0072 1f00 0000 7221 0000  ..r....r....r!..
-00000ef0: 0072 1100 0000 0d00 0000 7342 0000 0008  .r........sB....
-00000f00: 0006 0106 0106 0106 0102 0402 0106 fd1e  ................
-00000f10: 0202 fe06 030e fd0a 1114 0a12 050e 0302  ................
-00000f20: 0504 fe02 0102 ff02 0202 fe02 020a fe12  ................
-00000f30: 0712 032a 0702 1210 0102 0310 0102 0318  ...*............
-00000f40: 0172 1100 0000 6300 0000 0000 0000 0000  .r....c.........
-00000f50: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
-00000f60: 0c00 0000 6500 5a01 6400 5a02 6401 5300  ....e.Z.d.Z.d.S.
-00000f70: 2902 da03 4170 704e 2903 725e 0000 0072  )...AppN).r^...r
-00000f80: 5f00 0000 7260 0000 0072 1400 0000 7214  _...r`...r....r.
-00000f90: 0000 0072 1400 0000 7221 0000 0072 6700  ...r....r!...rg.
-00000fa0: 0000 6900 0000 7304 0000 0008 0004 0172  ..i...s........r
-00000fb0: 6700 0000 2918 7246 0000 0072 3300 0000  g...).rF...r3...
-00000fc0: 7230 0000 00da 0674 7970 696e 6772 0200  r0.....typingr..
-00000fd0: 0000 7203 0000 0072 0400 0000 7205 0000  ..r....r....r...
-00000fe0: 0072 0600 0000 da0e 5079 5369 6465 362e  .r......PySide6.
-00000ff0: 5174 436f 7265 7207 0000 0072 0800 0000  QtCorer....r....
-00001000: 7209 0000 0072 0a00 0000 da11 5079 5369  r....r......PySi
-00001010: 6465 362e 5174 5769 6467 6574 7372 0b00  de6.QtWidgetsr..
-00001020: 0000 720c 0000 0072 0d00 0000 da0d 5079  ..r....r......Py
-00001030: 5369 6465 362e 5174 4775 6972 0e00 0000  Side6.QtGuir....
-00001040: da04 636f 7265 7210 0000 0072 1100 0000  ..corer....r....
-00001050: 7267 0000 0072 1400 0000 7214 0000 0072  rg...r....r....r
-00001060: 1400 0000 7221 0000 00da 083c 6d6f 6475  ....r!.....<modu
-00001070: 6c65 3e01 0000 0073 1400 0000 0802 0801  le>....s........
-00001080: 0801 1c01 1801 1401 0c01 0c01 1203 145c  ...............\
+00000050: 6d05 5a05 6d06 5a06 6d07 5a07 0100 6400  m.Z.m.Z.m.Z...d.
+00000060: 6403 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
+00000070: 6d0c 5a0c 0100 6400 6404 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
+00000080: 6d0f 5a0f 6d10 5a10 0100 6400 6405 6c11  m.Z.m.Z...d.d.l.
+00000090: 6d12 5a12 0100 6406 6407 6c13 6d14 5a14  m.Z...d.d.l.m.Z.
+000000a0: 0100 4700 6408 6409 8400 6409 6514 650e  ..G.d.d...d.e.e.
+000000b0: 8304 5a15 4700 640a 640b 8400 640b 6515  ..Z.G.d.d...d.e.
+000000c0: 8303 5a16 6401 5300 290c e900 0000 004e  ..Z.d.S.)......N
+000000d0: 2904 da08 4361 6c6c 6162 6c65 da08 4e6f  )...Callable..No
+000000e0: 5265 7475 726e da08 4f70 7469 6f6e 616c  Return..Optional
+000000f0: da05 556e 696f 6e29 04da 0951 5265 736f  ..Union)...QReso
+00000100: 7572 6365 da02 5174 da06 5369 676e 616c  urce..Qt..Signal
+00000110: da15 7152 6567 6973 7465 7252 6573 6f75  ..qRegisterResou
+00000120: 7263 6544 6174 6129 03da 0c51 4170 706c  rceData)...QAppl
+00000130: 6963 6174 696f 6eda 0d51 5374 796c 6546  ication..QStyleF
+00000140: 6163 746f 7279 da07 5157 6964 6765 7429  actory..QWidget)
+00000150: 01da 0d51 466f 6e74 4461 7461 6261 7365  ...QFontDatabase
+00000160: e902 0000 0029 01da 0f41 6273 7472 6163  .....)...Abstrac
+00000170: 7451 4f62 6a65 6374 6300 0000 0000 0000  tQObjectc.......
+00000180: 0000 0000 0000 0000 000a 0000 0000 0000  ................
+00000190: 0073 4201 0000 6500 5a01 6400 5a02 6503  .sB...e.Z.d.Z.e.
+000001a0: 8300 5a04 6503 8300 5a05 6503 8300 5a06  ..Z.e...Z.e...Z.
+000001b0: 6503 8300 5a07 6401 6401 6402 9c02 6403  e...Z.d.d.d...d.
+000001c0: 6508 6509 650a 650b 650c 650d 1900 650e  e.e.e.e.e.e...e.
+000001d0: 650e 650e 6604 1900 6602 1900 1900 6404  e.e.f...f.....d.
+000001e0: 6508 650a 1900 6604 8700 6601 6405 6406  e.e...f...f.d.d.
+000001f0: 840e 5a0f 6423 6408 6409 8404 5a10 6424  ..Z.d#d.d...Z.d$
+00000200: 640b 6511 6407 6512 6604 640c 640d 8405  d.e.d.e.f.d.d...
+00000210: 5a13 6407 6508 650a 1900 6602 640e 640f  Z.d.e.e...f.d.d.
+00000220: 8404 5a14 6407 650a 6602 6410 6411 8404  ..Z.d.e.f.d.d...
+00000230: 5a15 0901 6425 6412 650a 6413 650a 6407  Z...d%d.e.d.e.d.
+00000240: 6511 6606 6414 6415 8405 5a16 6416 650a  e.f.d.d...Z.d.e.
+00000250: 6407 650d 6604 6417 6418 8404 5a17 6404  d.e.f.d.d...Z.d.
+00000260: 6508 650a 1900 6602 6419 641a 8404 5a18  e.e...f.d.d...Z.
+00000270: 6403 6508 6509 6519 650b 650c 650d 1900  d.e.e.e.e.e.e...
+00000280: 650e 650e 650e 6604 1900 6602 1900 1900  e.e.e.f...f.....
+00000290: 6602 641b 641c 8404 5a1a 651b 6407 651c  f.d.d...Z.e.d.e.
+000002a0: 6602 641d 641e 8404 8301 5a1d 651b 6407  f.d.d.....Z.e.d.
+000002b0: 651c 6602 641f 6420 8404 8301 5a1e 651b  e.f.d.d ....Z.e.
+000002c0: 6407 651c 6602 6421 6422 8404 8301 5a1f  d.e.f.d!d"....Z.
+000002d0: 8700 0400 5a20 5300 2926 da0b 4170 706c  ....Z S.)&..Appl
+000002e0: 6963 6174 696f 6e4e 2902 da09 7265 736f  icationN)...reso
+000002f0: 7572 6365 73da 0566 6f6e 7473 7211 0000  urces..fontsr...
+00000300: 0072 1200 0000 6301 0000 0000 0000 0002  .r....c.........
+00000310: 0000 0005 0000 0004 0000 000f 0000 0073  ...............s
+00000320: 5a00 0000 7400 6a01 7c00 6701 7c03 a201  Z...t.j.|.g.|...
+00000330: 5200 8e00 0100 7c01 6400 7501 7212 7c00  R.....|.d.u.r.|.
+00000340: a002 7c01 a101 0100 7c02 6400 7501 721b  ..|.....|.d.u.r.
+00000350: 7c00 a003 7c02 a101 0100 7404 8300 6a01  |...|.....t...j.
+00000360: 6401 6900 7c04 a401 8e01 0100 7c00 6a05  d.i.|.......|.j.
+00000370: a006 7c00 6a07 a101 0100 6400 5300 2902  ..|.j.....d.S.).
+00000380: 4ea9 0029 0872 0a00 0000 da08 5f5f 696e  N..).r......__in
+00000390: 6974 5f5f da0e 5f73 6574 5f72 6573 6f75  it__.._set_resou
+000003a0: 7263 6573 da0a 5f73 6574 5f66 6f6e 7473  rces.._set_fonts
+000003b0: da05 7375 7065 72da 1761 7070 6c69 6361  ..super..applica
+000003c0: 7469 6f6e 5374 6174 6543 6861 6e67 6564  tionStateChanged
+000003d0: da07 636f 6e6e 6563 74da 185f 6170 706c  ..connect.._appl
+000003e0: 6963 6174 696f 6e53 7461 7465 4368 616e  icationStateChan
+000003f0: 6765 6429 05da 0473 656c 6672 1100 0000  ged)...selfr....
+00000400: 7212 0000 00da 0461 7267 73da 066b 7761  r......args..kwa
+00000410: 7267 73a9 01da 095f 5f63 6c61 7373 5f5f  rgs....__class__
+00000420: 7213 0000 00fa 552f 686f 6d65 2f6f 7361  r.....U/home/osa
+00000430: 6d61 2f57 6f72 6b73 7061 6365 2f2e 7665  ma/Workspace/.ve
+00000440: 6e76 2f6c 6962 2f70 7974 686f 6e33 2e31  nv/lib/python3.1
+00000450: 302f 7369 7465 2d70 6163 6b61 6765 732f  0/site-packages/
+00000460: 5174 6963 612f 7769 6467 6574 732f 6170  Qtica/widgets/ap
+00000470: 706c 6963 6174 696f 6e2e 7079 7214 0000  plication.pyr...
+00000480: 0013 0000 0073 0e00 0000 1205 0802 0a01  .....s..........
+00000490: 0802 0a01 1202 1202 7a14 4170 706c 6963  ........z.Applic
+000004a0: 6174 696f 6e2e 5f5f 696e 6974 5f5f da06  ation.__init__..
+000004b0: 7265 7475 726e 6302 0000 0000 0000 0000  returnc.........
+000004c0: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+000004d0: 6c00 0000 7c01 7400 6a01 6a02 6b02 720d  l...|.t.j.j.k.r.
+000004e0: 7c00 6a03 a004 a100 0100 6400 5300 7c01  |.j.......d.S.|.
+000004f0: 7400 6a01 6a05 6b02 721a 7c00 6a06 a004  t.j.j.k.r.|.j...
+00000500: a100 0100 6400 5300 7c01 7400 6a01 6a07  ....d.S.|.t.j.j.
+00000510: 6b02 7227 7c00 6a08 a004 a100 0100 6400  k.r'|.j.......d.
+00000520: 5300 7c01 7400 6a01 6a09 6b02 7234 7c00  S.|.t.j.j.k.r4|.
+00000530: 6a0a a004 a100 0100 6400 5300 6400 5300  j.......d.S.d.S.
+00000540: a901 4e29 0b72 0700 0000 da10 4170 706c  ..N).r......Appl
+00000550: 6963 6174 696f 6e53 7461 7465 da13 4170  icationState..Ap
+00000560: 706c 6963 6174 696f 6e49 6e61 6374 6976  plicationInactiv
+00000570: 65da 0b6f 6e5f 696e 6163 7469 7665 da04  e..on_inactive..
+00000580: 656d 6974 da11 4170 706c 6963 6174 696f  emit..Applicatio
+00000590: 6e41 6374 6976 65da 096f 6e5f 6163 7469  nActive..on_acti
+000005a0: 7665 da11 4170 706c 6963 6174 696f 6e48  ve..ApplicationH
+000005b0: 6964 6465 6eda 096f 6e5f 6869 6464 656e  idden..on_hidden
+000005c0: da14 4170 706c 6963 6174 696f 6e53 7573  ..ApplicationSus
+000005d0: 7065 6e64 6564 da0a 6f6e 5f73 7573 7065  pended..on_suspe
+000005e0: 6e64 2902 721b 0000 00da 0565 7665 6e74  nd).r......event
+000005f0: 7213 0000 0072 1300 0000 7220 0000 0072  r....r....r ...r
+00000600: 1a00 0000 2400 0000 7312 0000 000c 010e  ....$...s.......
+00000610: 010c 010e 010c 010e 010c 010e 0104 ff7a  ...............z
+00000620: 2441 7070 6c69 6361 7469 6f6e 2e5f 6170  $Application._ap
+00000630: 706c 6963 6174 696f 6e53 7461 7465 4368  plicationStateCh
+00000640: 616e 6765 6446 da09 7465 726d 5f65 7869  angedF..term_exi
+00000650: 7463 0200 0000 0000 0000 0000 0000 0200  tc..............
+00000660: 0000 0400 0000 4300 0000 7322 0000 007c  ......C...s"...|
+00000670: 0172 0a74 00a0 0074 006a 0174 006a 02a1  .r.t...t.j.t.j..
+00000680: 0201 0074 03a0 047c 00a0 05a1 00a1 0153  ...t...|.......S
+00000690: 0072 2200 0000 2906 da06 7369 676e 616c  .r"...)...signal
+000006a0: da06 5349 4749 4e54 da07 5349 475f 4446  ..SIGINT..SIG_DF
+000006b0: 4cda 0373 7973 da04 6578 6974 da04 6578  L..sys..exit..ex
+000006c0: 6563 2902 721b 0000 0072 2e00 0000 7213  ec).r....r....r.
+000006d0: 0000 0072 1300 0000 7220 0000 00da 0372  ...r....r .....r
+000006e0: 756e 2e00 0000 7306 0000 0004 0110 010e  un....s.........
+000006f0: 017a 0f41 7070 6c69 6361 7469 6f6e 2e72  .z.Application.r
+00000700: 756e 6301 0000 0000 0000 0000 0000 0001  unc.............
+00000710: 0000 0002 0000 0043 0000 00f3 0800 0000  .......C........
+00000720: 7400 a001 a100 5300 7222 0000 0029 0272  t.....S.r"...).r
+00000730: 0b00 0000 da04 6b65 7973 a901 721b 0000  ......keys..r...
+00000740: 0072 1300 0000 7213 0000 0072 2000 0000  .r....r....r ...
+00000750: da0a 7374 796c 655f 6c69 7374 3300 0000  ..style_list3...
+00000760: 7302 0000 0008 017a 1641 7070 6c69 6361  s......z.Applica
+00000770: 7469 6f6e 2e73 7479 6c65 5f6c 6973 7463  tion.style_listc
+00000780: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000790: 0200 0000 4300 0000 730c 0000 007c 00a0  ....C...s....|..
+000007a0: 00a1 00a0 01a1 0053 0072 2200 0000 2902  .......S.r"...).
+000007b0: da05 7374 796c 65da 046e 616d 6572 3800  ..style..namer8.
+000007c0: 0000 7213 0000 0072 1300 0000 7220 0000  ..r....r....r ..
+000007d0: 00da 0d63 7572 7265 6e74 5f73 7479 6c65  ...current_style
+000007e0: 3600 0000 7302 0000 000c 017a 1941 7070  6...s......z.App
+000007f0: 6c69 6361 7469 6f6e 2e63 7572 7265 6e74  lication.current
+00000800: 5f73 7479 6c65 da08 7263 635f 6669 6c65  _style..rcc_file
+00000810: da08 7263 635f 726f 6f74 6303 0000 0000  ..rcc_rootc.....
+00000820: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
+00000830: 0000 0073 1e00 0000 7c02 6400 7501 720a  ...s....|.d.u.r.
+00000840: 7400 a001 7c01 7c02 a102 5300 7400 a001  t...|.|...S.t...
+00000850: 7c01 a101 5300 7222 0000 0029 0272 0600  |...S.r"...).r..
+00000860: 0000 da10 7265 6769 7374 6572 5265 736f  ....registerReso
+00000870: 7572 6365 2903 721b 0000 0072 3d00 0000  urce).r....r=...
+00000880: 723e 0000 0072 1300 0000 7213 0000 0072  r>...r....r....r
+00000890: 2000 0000 da0c 6164 645f 7263 635f 6669   .....add_rcc_fi
+000008a0: 6c65 3900 0000 7306 0000 0008 030c 010a  le9...s.........
+000008b0: 017a 1841 7070 6c69 6361 7469 6f6e 2e61  .z.Application.a
+000008c0: 6464 5f72 6363 5f66 696c 65da 0866 6f6e  dd_rcc_file..fon
+000008d0: 7470 6174 6863 0200 0000 0000 0000 0000  tpathc..........
+000008e0: 0000 0200 0000 0300 0000 4300 0000 730a  ..........C...s.
+000008f0: 0000 0074 00a0 017c 01a1 0153 0072 2200  ...t...|...S.r".
+00000900: 0000 2902 720d 0000 00da 1261 6464 4170  ..).r......addAp
+00000910: 706c 6963 6174 696f 6e46 6f6e 7429 0272  plicationFont).r
+00000920: 1b00 0000 7241 0000 0072 1300 0000 7213  ....rA...r....r.
+00000930: 0000 0072 2000 0000 da08 6164 645f 666f  ...r .....add_fo
+00000940: 6e74 4000 0000 7302 0000 000a 017a 1441  nt@...s......z.A
+00000950: 7070 6c69 6361 7469 6f6e 2e61 6464 5f66  pplication.add_f
+00000960: 6f6e 7463 0200 0000 0000 0000 0000 0000  ontc............
+00000970: 0300 0000 0500 0000 4300 0000 7334 0000  ........C...s4..
+00000980: 007c 0144 005d 157d 0274 006a 01a0 027c  .|.D.].}.t.j...|
+00000990: 02a1 0173 1274 0364 017c 029b 0064 029d  ...s.t.d.|...d..
+000009a0: 0383 0182 017c 00a0 047c 01a1 0101 0071  .....|...|.....q
+000009b0: 0264 0053 0029 034e fa01 277a 1627 2066  .d.S.).N..'z.' f
+000009c0: 6f6e 7420 6669 6c65 206e 6f74 2066 6f75  ont file not fou
+000009d0: 6e64 2129 05da 026f 73da 0470 6174 68da  nd!)...os..path.
+000009e0: 0665 7869 7374 73da 1146 696c 654e 6f74  .exists..FileNot
+000009f0: 466f 756e 6445 7272 6f72 7243 0000 0029  FoundErrorrC...)
+00000a00: 0372 1b00 0000 7212 0000 00da 0466 6f6e  .r....r......fon
+00000a10: 7472 1300 0000 7213 0000 0072 2000 0000  tr....r....r ...
+00000a20: 7216 0000 0043 0000 0073 0a00 0000 0801  r....C...s......
+00000a30: 0c01 1001 0c02 04fc 7a16 4170 706c 6963  ........z.Applic
+00000a40: 6174 696f 6e2e 5f73 6574 5f66 6f6e 7473  ation._set_fonts
+00000a50: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+00000a60: 0009 0000 0043 0000 0073 9200 0000 7c01  .....C...s....|.
+00000a70: 4400 5d44 7d02 7400 7c02 7401 7402 7403  D.]D}.t.|.t.t.t.
+00000a80: 6603 8302 7233 7404 7c02 8301 6401 6b00  f...r3t.|...d.k.
+00000a90: 721c 7402 7c02 8301 7d02 7c02 a005 6402  r.t.|...}.|...d.
+00000aa0: 6403 a102 0100 7406 7c02 6402 1900 6404  d.....t.|.d...d.
+00000ab0: 7501 7227 7c02 6402 1900 6e01 6403 6701  u.r'|.d...n.d.g.
+00000ac0: 7c02 6405 6404 8502 1900 a201 5200 8e00  |.d.d.......R...
+00000ad0: 0100 7102 7407 7c02 8301 7246 7a05 7c02  ..q.t.|...rFz.|.
+00000ae0: 8300 0100 5700 7102 0400 7408 7945 0100  ....W.q...t.yE..
+00000af0: 0100 0100 5900 7102 7700 7102 6404 5300  ....Y.q.w.q.d.S.
+00000b00: 2906 7aa2 0a20 2020 2020 2020 203a 7061  ).z..        :pa
+00000b10: 7261 6d3a 2072 6573 6f75 7263 650a 2020  ram: resource.  
+00000b20: 2020 2020 2020 2020 2020 6361 6c6c 6162            callab
+00000b30: 6c65 203d 2071 496e 6974 5265 736f 7572  le = qInitResour
+00000b40: 6365 730a 2020 2020 2020 2020 2020 2020  ces.            
+00000b50: 7475 706c 6520 3d20 2830 7830 3320 7c20  tuple = (0x03 | 
+00000b60: 4e6f 6e65 2c20 7174 5f72 6573 6f75 7263  None, qt_resourc
+00000b70: 655f 7374 7275 6374 2c20 7174 5f72 6573  e_struct, qt_res
+00000b80: 6f75 7263 655f 6e61 6d65 2c20 7174 5f72  ource_name, qt_r
+00000b90: 6573 6f75 7263 655f 6461 7461 290a 2020  esource_data).  
+00000ba0: 2020 2020 2020 e904 0000 0072 0100 0000        .....r....
+00000bb0: e903 0000 004e e901 0000 0029 09da 0a69  .....N.....)...i
+00000bc0: 7369 6e73 7461 6e63 65da 0574 7570 6c65  sinstance..tuple
+00000bd0: da04 6c69 7374 da03 7365 74da 036c 656e  ..list..set..len
+00000be0: da06 696e 7365 7274 7209 0000 00da 0863  ..insertr......c
+00000bf0: 616c 6c61 626c 65da 0945 7863 6570 7469  allable..Excepti
+00000c00: 6f6e 2903 721b 0000 0072 1100 0000 da03  on).r....r......
+00000c10: 7265 7372 1300 0000 7213 0000 0072 2000  resr....r....r .
+00000c20: 0000 7215 0000 004a 0000 0073 1c00 0000  ..r....J...s....
+00000c30: 0806 1001 0c01 0801 0c01 2e01 0801 0201  ................
+00000c40: 0a01 0c01 0401 02ff 02fd 04fa 7a1a 4170  ............z.Ap
+00000c50: 706c 6963 6174 696f 6e2e 5f73 6574 5f72  plication._set_r
+00000c60: 6573 6f75 7263 6573 6300 0000 0000 0000  esourcesc.......
+00000c70: 0000 0000 0000 0000 0002 0000 0043 0000  .............C..
+00000c80: 0072 3600 0000 7222 0000 0029 0272 0a00  .r6...r"...).r..
+00000c90: 0000 da0c 6163 7469 7665 5769 6e64 6f77  ....activeWindow
+00000ca0: 7213 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
+00000cb0: 2000 0000 da0d 6163 7469 7665 5f77 696e   .....active_win
+00000cc0: 646f 775c 0000 00f3 0200 0000 0802 7a19  dow\..........z.
+00000cd0: 4170 706c 6963 6174 696f 6e2e 6163 7469  Application.acti
+00000ce0: 7665 5f77 696e 646f 7763 0000 0000 0000  ve_windowc......
+00000cf0: 0000 0000 0000 0000 0000 0200 0000 4300  ..............C.
+00000d00: 0000 7236 0000 0072 2200 0000 2902 720a  ..r6...r"...).r.
+00000d10: 0000 00da 1161 6374 6976 654d 6f64 616c  .....activeModal
+00000d20: 5769 6467 6574 7213 0000 0072 1300 0000  Widgetr....r....
+00000d30: 7213 0000 0072 2000 0000 da0c 6163 7469  r....r .....acti
+00000d40: 7665 5f6d 6f64 616c 6000 0000 7258 0000  ve_modal`...rX..
+00000d50: 007a 1841 7070 6c69 6361 7469 6f6e 2e61  .z.Application.a
+00000d60: 6374 6976 655f 6d6f 6461 6c63 0000 0000  ctive_modalc....
+00000d70: 0000 0000 0000 0000 0000 0000 0200 0000  ................
+00000d80: 4300 0000 7236 0000 0072 2200 0000 2902  C...r6...r"...).
+00000d90: 720a 0000 00da 1161 6374 6976 6550 6f70  r......activePop
+00000da0: 7570 5769 6467 6574 7213 0000 0072 1300  upWidgetr....r..
+00000db0: 0000 7213 0000 0072 2000 0000 da0c 6163  ..r....r .....ac
+00000dc0: 7469 7665 5f70 6f70 7570 6400 0000 7258  tive_popupd...rX
+00000dd0: 0000 007a 1841 7070 6c69 6361 7469 6f6e  ...z.Application
+00000de0: 2e61 6374 6976 655f 706f 7075 7029 0272  .active_popup).r
+00000df0: 2100 0000 4e29 0146 7222 0000 0029 21da  !...N).Fr"...)!.
+00000e00: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00000e10: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00000e20: 655f 5f72 0800 0000 7225 0000 0072 2800  e__r....r%...r(.
+00000e30: 0000 722a 0000 0072 2c00 0000 724f 0000  ..r*...r,...rO..
+00000e40: 0072 0500 0000 da03 7374 7272 4e00 0000  .r......strrN...
+00000e50: 7204 0000 00da 0369 6e74 da05 6279 7465  r......int..byte
+00000e60: 7372 1400 0000 721a 0000 00da 0462 6f6f  sr....r......boo
+00000e70: 6c72 0300 0000 7235 0000 0072 3900 0000  lr....r5...r9...
+00000e80: 723c 0000 0072 4000 0000 7243 0000 0072  r<...r@...rC...r
+00000e90: 1600 0000 7202 0000 0072 1500 0000 da0c  ....r....r......
+00000ea0: 7374 6174 6963 6d65 7468 6f64 720c 0000  staticmethodr...
+00000eb0: 0072 5700 0000 725a 0000 0072 5c00 0000  .rW...rZ...r\...
+00000ec0: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
+00000ed0: 1300 0000 7213 0000 0072 1e00 0000 7220  ....r....r....r 
+00000ee0: 0000 0072 1000 0000 0d00 0000 7342 0000  ...r........sB..
+00000ef0: 0008 0006 0106 0106 0106 0102 0402 0106  ................
+00000f00: fd1e 0202 fe06 030e fd0a 1114 0a12 050e  ................
+00000f10: 0302 0504 fe02 0102 ff02 0202 fe02 020a  ................
+00000f20: fe12 0712 032a 0702 1210 0102 0310 0102  .....*..........
+00000f30: 0318 0172 1000 0000 6300 0000 0000 0000  ...r....c.......
+00000f40: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
+00000f50: 0073 0c00 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+00000f60: 5300 2902 da03 4170 704e 2903 725d 0000  S.)...AppN).r]..
+00000f70: 0072 5e00 0000 725f 0000 0072 1300 0000  .r^...r_...r....
+00000f80: 7213 0000 0072 1300 0000 7220 0000 0072  r....r....r ...r
+00000f90: 6600 0000 6900 0000 7304 0000 0008 0004  f...i...s.......
+00000fa0: 0172 6600 0000 2917 7245 0000 0072 3200  .rf...).rE...r2.
+00000fb0: 0000 722f 0000 00da 0674 7970 696e 6772  ..r/.....typingr
+00000fc0: 0200 0000 7203 0000 0072 0400 0000 7205  ....r....r....r.
+00000fd0: 0000 00da 0e50 7953 6964 6536 2e51 7443  .....PySide6.QtC
+00000fe0: 6f72 6572 0600 0000 7207 0000 0072 0800  orer....r....r..
+00000ff0: 0000 7209 0000 00da 1150 7953 6964 6536  ..r......PySide6
+00001000: 2e51 7457 6964 6765 7473 720a 0000 0072  .QtWidgetsr....r
+00001010: 0b00 0000 720c 0000 00da 0d50 7953 6964  ....r......PySid
+00001020: 6536 2e51 7447 7569 720d 0000 00da 0463  e6.QtGuir......c
+00001030: 6f72 6572 0f00 0000 7210 0000 0072 6600  orer....r....rf.
+00001040: 0000 7213 0000 0072 1300 0000 7213 0000  ..r....r....r...
+00001050: 0072 2000 0000 da08 3c6d 6f64 756c 653e  .r .....<module>
+00001060: 0100 0000 7314 0000 0008 0208 0108 0118  ....s...........
+00001070: 0118 0114 010c 010c 0112 0314 5c         ............\
```

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/application.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/application.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/buttons.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/buttons.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/frame.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/frame.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/frame.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/frame.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/icon_widget.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/icon_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/icon_widget.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/icon_widget.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/label.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/label.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/label.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/label.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/line.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/line.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/line.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/line.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/line_edit.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/line_edit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/line_edit.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/line_edit.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/menu.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/menu.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/menu.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/menu.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/push_button.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/push_button.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/push_button.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/push_button.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/scroll_area.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/scroll_area.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jan  8 20:47:34 2024 UTC, .py size: 986 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 665f 9c65 da03 0000  o.......f_.e....
+00000000: 6f0d 0d0a 0000 0000 4eb7 e765 db03 0000  o.......N..e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6404  m.Z.m.Z.m.Z...d.
 00000060: 6405 6c09 6d0a 5a0a 0100 4700 6406 6407  d.l.m.Z...G.d.d.
 00000070: 8400 6407 650a 6507 8304 5a0b 6408 5300  ..d.e.e...Z.d.S.
@@ -41,41 +41,41 @@
 00000280: da13 7365 7453 697a 6541 646a 7573 7450  ..setSizeAdjustP
 00000290: 6f6c 6963 79da 1053 697a 6541 646a 7573  olicy..SizeAdjus
 000002a0: 7450 6f6c 6963 79da 1041 646a 7573 7454  tPolicy..AdjustT
 000002b0: 6f43 6f6e 7465 6e74 73da 0d73 6574 4672  oContents..setFr
 000002c0: 616d 6553 6861 7065 7204 0000 00da 0553  ameShaper......S
 000002d0: 6861 7065 da07 4e6f 4672 616d 65da 0e73  hape..NoFrame..s
 000002e0: 6574 4672 616d 6553 6861 646f 77da 0653  etFrameShadow..S
-000002f0: 6861 646f 77da 0550 6c61 696e da05 7375  hadow..Plain..su
-00000300: 7065 72da 0a69 7369 6e73 7461 6e63 6572  per..isinstancer
-00000310: 0500 0000 7207 0000 00da 0b73 6574 5072  ....r......setPr
-00000320: 6f70 6572 7479 da09 7365 744c 6179 6f75  operty..setLayou
-00000330: 74da 0973 6574 5769 6467 6574 2904 da04  t..setWidget)...
-00000340: 7365 6c66 720b 0000 00da 066b 7761 7267  selfr......kwarg
-00000350: 73da 075f 7769 6467 6574 a901 da09 5f5f  s.._widget....__
-00000360: 636c 6173 735f 5f72 0d00 0000 fa55 2f68  class__r.....U/h
-00000370: 6f6d 652f 6f73 616d 612f 576f 726b 7370  ome/osama/Worksp
-00000380: 6163 652f 2e76 656e 762f 6c69 622f 7079  ace/.venv/lib/py
-00000390: 7468 6f6e 332e 3130 2f73 6974 652d 7061  thon3.10/site-pa
-000003a0: 636b 6167 6573 2f51 7469 6361 2f77 6964  ckages/Qtica/wid
-000003b0: 6765 7473 2f73 6372 6f6c 6c5f 6172 6561  gets/scroll_area
-000003c0: 2e70 7972 0e00 0000 0800 0000 7320 0000  .pyr........s ..
-000003d0: 000a 040a 020a 010e 020e 010e 020e 0112  ................
-000003e0: 0208 020a 0106 010c 010a 0104 010e 0104  ................
-000003f0: fa7a 1353 6372 6f6c 6c41 7265 612e 5f5f  .z.ScrollArea.__
-00000400: 696e 6974 5f5f 2908 da08 5f5f 6e61 6d65  init__)...__name
-00000410: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00000420: 5f5f 7175 616c 6e61 6d65 5f5f 7202 0000  __qualname__r...
-00000430: 0072 0700 0000 7205 0000 0072 0e00 0000  .r....r....r....
-00000440: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
-00000450: 0d00 0000 720d 0000 0072 2500 0000 7227  ....r....r%...r'
-00000460: 0000 0072 0a00 0000 0700 0000 730a 0000  ...r........s...
-00000470: 0008 0002 0306 fe0a 0216 fe72 0a00 0000  ...........r....
-00000480: 4e29 0cda 0674 7970 696e 6772 0200 0000  N)...typingr....
-00000490: da0e 5079 5369 6465 362e 5174 436f 7265  ..PySide6.QtCore
-000004a0: 7203 0000 00da 1150 7953 6964 6536 2e51  r......PySide6.Q
-000004b0: 7457 6964 6765 7473 7204 0000 0072 0500  tWidgetsr....r..
-000004c0: 0000 7206 0000 0072 0700 0000 da04 636f  ..r....r......co
-000004d0: 7265 7209 0000 0072 0a00 0000 720d 0000  rer....r....r...
-000004e0: 0072 0d00 0000 720d 0000 0072 2700 0000  .r....r....r'...
-000004f0: da08 3c6d 6f64 756c 653e 0100 0000 730a  ..<module>....s.
-00000500: 0000 000c 000c 0118 010c 0116 03         .............
+000002f0: 6861 646f 77da 0652 6169 7365 64da 0573  hadow..Raised..s
+00000300: 7570 6572 da0a 6973 696e 7374 616e 6365  uper..isinstance
+00000310: 7205 0000 0072 0700 0000 da0b 7365 7450  r....r......setP
+00000320: 726f 7065 7274 79da 0973 6574 4c61 796f  roperty..setLayo
+00000330: 7574 da09 7365 7457 6964 6765 7429 04da  ut..setWidget)..
+00000340: 0473 656c 6672 0b00 0000 da06 6b77 6172  .selfr......kwar
+00000350: 6773 da07 5f77 6964 6765 74a9 01da 095f  gs.._widget...._
+00000360: 5f63 6c61 7373 5f5f 720d 0000 00fa 552f  _class__r.....U/
+00000370: 686f 6d65 2f6f 7361 6d61 2f57 6f72 6b73  home/osama/Works
+00000380: 7061 6365 2f2e 7665 6e76 2f6c 6962 2f70  pace/.venv/lib/p
+00000390: 7974 686f 6e33 2e31 302f 7369 7465 2d70  ython3.10/site-p
+000003a0: 6163 6b61 6765 732f 5174 6963 612f 7769  ackages/Qtica/wi
+000003b0: 6467 6574 732f 7363 726f 6c6c 5f61 7265  dgets/scroll_are
+000003c0: 612e 7079 720e 0000 0008 0000 0073 2000  a.pyr........s .
+000003d0: 0000 0a04 0a02 0a01 0e02 0e01 0e02 0e01  ................
+000003e0: 1202 0802 0a01 0601 0c01 0a01 0401 0e01  ................
+000003f0: 04fa 7a13 5363 726f 6c6c 4172 6561 2e5f  ..z.ScrollArea._
+00000400: 5f69 6e69 745f 5f29 08da 085f 5f6e 616d  _init__)...__nam
+00000410: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000420: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0200  .__qualname__r..
+00000430: 0000 7207 0000 0072 0500 0000 720e 0000  ..r....r....r...
+00000440: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
+00000450: 720d 0000 0072 0d00 0000 7225 0000 0072  r....r....r%...r
+00000460: 2700 0000 720a 0000 0007 0000 0073 0a00  '...r........s..
+00000470: 0000 0800 0203 06fe 0a02 16fe 720a 0000  ............r...
+00000480: 004e 290c da06 7479 7069 6e67 7202 0000  .N)...typingr...
+00000490: 00da 0e50 7953 6964 6536 2e51 7443 6f72  ...PySide6.QtCor
+000004a0: 6572 0300 0000 da11 5079 5369 6465 362e  er......PySide6.
+000004b0: 5174 5769 6467 6574 7372 0400 0000 7205  QtWidgetsr....r.
+000004c0: 0000 0072 0600 0000 7207 0000 00da 0463  ...r....r......c
+000004d0: 6f72 6572 0900 0000 720a 0000 0072 0d00  orer....r....r..
+000004e0: 0000 720d 0000 0072 0d00 0000 7227 0000  ..r....r....r'..
+000004f0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000500: 0a00 0000 0c00 0c01 1801 0c01 1603       ..............
```

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/scroll_area.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/scroll_area.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/size_grip.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/size_grip.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/size_grip.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/size_grip.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/spin_box.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/spin_box.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/spin_box.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/spin_box.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/stack.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/stack.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Feb  3 20:39:57 2024 UTC, .py size: 3952 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9da4 be65 700f 0000  o..........ep...
+00000000: 6f0d 0d0a 0000 0000 aeb3 fc65 c10e 0000  o..........e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6404 6405 6c0a 6d0b 5a0b 0100 6404  ..d.d.l.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 0100 6404 6407 6c0e  d.l.m.Z...d.d.l.
@@ -112,83 +112,80 @@
 000006f0: 0000 0073 3200 0000 0801 0a01 0601 0a02  ...s2...........
 00000700: 0a01 0a01 0a01 0a01 0801 0c01 0a01 0801  ................
 00000710: 0802 1001 0a02 0e01 0a02 0e01 0a02 0801  ................
 00000720: 0c01 0a01 0c01 0280 04e5 7a1d 5374 6163  ..........z.Stac
 00000730: 6b2e 5f73 6574 5f63 6869 6c64 7265 6e5f  k._set_children_
 00000740: 6672 6f6d 5f6c 6973 7463 0200 0000 0000  from_listc......
 00000750: 0000 0000 0000 0500 0000 0500 0000 4300  ..............C.
-00000760: 0000 73d0 0000 0074 007c 0174 0183 0272  ..s....t.|.t...r
+00000760: 0000 73a8 0000 0074 007c 0174 0183 0272  ..s....t.|.t...r
 00000770: 0e74 0264 0269 007c 01a0 03a1 00a4 018e  .t.d.i.|........
 00000780: 016e 017c 017c 005f 047c 006a 04a0 057c  .n.|.|._.|.j...|
-00000790: 00a1 0101 007c 006a 046a 0644 005d 4a5c  .....|.j.j.D.]J\
-000007a0: 027d 027d 0374 007c 0374 0783 0272 5e7c  .}.}.t.|.t...r^|
-000007b0: 036a 087d 0474 007c 0474 0983 0272 4a74  .j.}.t.|.t...rJt
+00000790: 00a1 0101 007c 006a 046a 0644 005d 365c  .....|.j.j.D.]6\
+000007a0: 027d 027d 0374 007c 0374 0783 0272 4a7c  .}.}.t.|.t...rJ|
+000007b0: 036a 087d 0474 007c 0474 0983 0272 3b74  .j.}.t.|.t...r;t
 000007c0: 0a7c 0083 017d 047c 04a0 0b64 017c 04a1  .|...}.|...d.|..
 000007d0: 0201 007c 04a0 0c7c 04a1 0101 007c 006a  ...|...|.....|.j
 000007e0: 04a0 0d7c 027c 04a1 0201 007c 00a0 0e7c  ...|.|.....|...|
-000007f0: 047c 036a 0fa1 0201 0071 1b74 007c 0474  .|.j.....q.t.|.t
-00000800: 0a83 0272 5d7c 006a 04a0 0d7c 027c 04a1  ...r]|.j...|.|..
-00000810: 0201 007c 00a0 0e7c 047c 036a 0fa1 0201  ...|...|.|.j....
-00000820: 0071 1b7c 006a 04a0 0d7c 027c 03a1 0201  .q.|.j...|.|....
-00000830: 0071 1b64 0053 0029 034e 722e 0000 0072  .q.d.S.).Nr....r
-00000840: 1600 0000 2910 7221 0000 00da 0464 6963  ....).r!.....dic
-00000850: 7472 0b00 0000 da05 6974 656d 73da 0672  tr......items..r
-00000860: 6f75 7465 73da 0c5f 7365 745f 7374 6163  outes.._set_stac
-00000870: 6b65 64da 0777 6964 6765 7473 720a 0000  ked..widgetsr...
-00000880: 0072 2f00 0000 7206 0000 0072 0500 0000  .r/...r....r....
-00000890: 7232 0000 0072 2800 0000 da03 6164 6472  r2...r(.....addr
-000008a0: 3300 0000 7234 0000 0029 0572 2900 0000  3...r4...).r)...
-000008b0: 7210 0000 00da 0572 6f75 7465 722f 0000  r......router/..
-000008c0: 0072 3500 0000 7216 0000 0072 1600 0000  .r5...r....r....
-000008d0: 722d 0000 00da 175f 7365 745f 6368 696c  r-....._set_chil
-000008e0: 6472 656e 5f66 726f 6d5f 6469 6374 5000  dren_from_dictP.
-000008f0: 0000 7322 0000 0022 010c 0110 020a 0106  ..s"..."........
-00000900: 010a 0208 010c 010a 010e 0110 010a 020e  ................
-00000910: 010e 0102 8010 0204 f17a 1d53 7461 636b  .........z.Stack
-00000920: 2e5f 7365 745f 6368 696c 6472 656e 5f66  ._set_children_f
-00000930: 726f 6d5f 6469 6374 6302 0000 0000 0000  rom_dictc.......
-00000940: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-00000950: 0073 2a00 0000 7c01 7304 6400 5300 7400  .s*...|.s.d.S.t.
-00000960: 7c01 7401 7402 6602 8302 7210 7c00 a003  |.t.t.f...r.|...
-00000970: 7c01 a101 5300 7c00 a004 7c01 a101 5300  |...S.|...|...S.
-00000980: a901 4e29 0572 2100 0000 720b 0000 0072  ..N).r!...r....r
-00000990: 3900 0000 7240 0000 0072 3800 0000 2902  9...r@...r8...).
-000009a0: 7229 0000 0072 1000 0000 7216 0000 0072  r)...r....r....r
-000009b0: 1600 0000 722d 0000 0072 2700 0000 6500  ....r-...r'...e.
-000009c0: 0000 730a 0000 0004 0104 010e 020a 010a  ..s.............
-000009d0: 017a 1353 7461 636b 2e5f 7365 745f 6368  .z.Stack._set_ch
-000009e0: 696c 6472 656e da06 7265 7475 726e 6301  ildren..returnc.
-000009f0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-00000a00: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
-00000a10: 5300 7241 0000 0029 0172 1f00 0000 2901  S.rA...).r....).
-00000a20: 7229 0000 0072 1600 0000 7216 0000 0072  r)...r....r....r
-00000a30: 2d00 0000 da07 7374 6163 6b65 646d 0000  -.....stackedm..
-00000a40: 0073 0200 0000 0602 7a0d 5374 6163 6b2e  .s......z.Stack.
-00000a50: 7374 6163 6b65 6429 19da 085f 5f6e 616d  stacked)...__nam
-00000a60: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000a70: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0800  .__qualname__r..
-00000a80: 0000 720e 0000 0072 0200 0000 da0f 5f5f  ..r....r......__
-00000a90: 616e 6e6f 7461 7469 6f6e 735f 5f72 0f00  annotations__r..
-00000aa0: 0000 da08 5374 6163 6b41 6c6c 7203 0000  ....StackAllr...
-00000ab0: 00da 046c 6973 7472 0500 0000 7206 0000  ...listr....r...
-00000ac0: 0072 0700 0000 720a 0000 0072 0b00 0000  .r....r....r....
-00000ad0: 7222 0000 00da 0373 7472 7217 0000 0072  r".....strr....r
-00000ae0: 3800 0000 7240 0000 0072 2700 0000 da08  8...r@...r'.....
-00000af0: 7072 6f70 6572 7479 7243 0000 00da 0d5f  propertyrC....._
-00000b00: 5f63 6c61 7373 6365 6c6c 5f5f 7216 0000  _classcell__r...
-00000b10: 0072 1600 0000 722b 0000 0072 2d00 0000  .r....r+...r-...
-00000b20: 720d 0000 000a 0000 0073 3600 0000 0a00  r........s6.....
-00000b30: 0e01 0e01 0204 0601 0201 0201 0201 0201  ................
-00000b40: 06f9 1a02 02fe 0403 02fd 0404 02fc 0205  ................
-00000b50: 02fb 0a06 02fa 0207 0ef9 0824 081e 0815  ...........$....
-00000b60: 0208 1801 720d 0000 004e 2911 da04 656e  ....r....N)...en
-00000b70: 756d 7202 0000 00da 0674 7970 696e 6772  umr......typingr
-00000b80: 0300 0000 da11 5079 5369 6465 362e 5174  ......PySide6.Qt
-00000b90: 5769 6467 6574 7372 0400 0000 7205 0000  Widgetsr....r...
-00000ba0: 0072 0600 0000 7207 0000 0072 0800 0000  .r....r....r....
-00000bb0: da0f 7574 696c 732e 616c 6967 6e6d 656e  ..utils.alignmen
-00000bc0: 7472 0a00 0000 da0b 636f 7265 2e72 6f75  tr......core.rou
-00000bd0: 7465 7372 0b00 0000 da04 636f 7265 720c  tesr......corer.
-00000be0: 0000 0072 0d00 0000 7216 0000 0072 1600  ...r....r....r..
-00000bf0: 0000 7216 0000 0072 2d00 0000 da08 3c6d  ..r....r-.....<m
-00000c00: 6f64 756c 653e 0100 0000 730e 0000 000c  odule>....s.....
-00000c10: 010c 011c 010c 010c 010c 0116 03         .............
+000007f0: 047c 036a 0fa1 0201 0071 1b7c 006a 04a0  .|.j.....q.|.j..
+00000800: 0d7c 027c 03a1 0201 0071 1b64 0053 0029  .|.|.....q.d.S.)
+00000810: 034e 722e 0000 0072 1600 0000 2910 7221  .Nr....r....).r!
+00000820: 0000 00da 0464 6963 7472 0b00 0000 da05  .....dictr......
+00000830: 6974 656d 73da 0672 6f75 7465 73da 0c5f  items..routes.._
+00000840: 7365 745f 7374 6163 6b65 64da 0777 6964  set_stacked..wid
+00000850: 6765 7473 720a 0000 0072 2f00 0000 7206  getsr....r/...r.
+00000860: 0000 0072 0500 0000 7232 0000 0072 2800  ...r....r2...r(.
+00000870: 0000 da03 6164 6472 3300 0000 7234 0000  ....addr3...r4..
+00000880: 0029 0572 2900 0000 7210 0000 00da 0572  .).r)...r......r
+00000890: 6f75 7465 722f 0000 0072 3500 0000 7216  outer/...r5...r.
+000008a0: 0000 0072 1600 0000 722d 0000 00da 175f  ...r....r-....._
+000008b0: 7365 745f 6368 696c 6472 656e 5f66 726f  set_children_fro
+000008c0: 6d5f 6469 6374 5000 0000 731a 0000 0022  m_dictP...s...."
+000008d0: 010c 0110 020a 0106 010a 0208 010c 010a  ................
+000008e0: 010e 0210 0110 0204 f47a 1d53 7461 636b  .........z.Stack
+000008f0: 2e5f 7365 745f 6368 696c 6472 656e 5f66  ._set_children_f
+00000900: 726f 6d5f 6469 6374 6302 0000 0000 0000  rom_dictc.......
+00000910: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+00000920: 0073 2a00 0000 7c01 7304 6400 5300 7400  .s*...|.s.d.S.t.
+00000930: 7c01 7401 7402 6602 8302 7210 7c00 a003  |.t.t.f...r.|...
+00000940: 7c01 a101 5300 7c00 a004 7c01 a101 5300  |...S.|...|...S.
+00000950: a901 4e29 0572 2100 0000 720b 0000 0072  ..N).r!...r....r
+00000960: 3900 0000 7240 0000 0072 3800 0000 2902  9...r@...r8...).
+00000970: 7229 0000 0072 1000 0000 7216 0000 0072  r)...r....r....r
+00000980: 1600 0000 722d 0000 0072 2700 0000 6200  ....r-...r'...b.
+00000990: 0000 730a 0000 0004 0104 010e 020a 010a  ..s.............
+000009a0: 017a 1353 7461 636b 2e5f 7365 745f 6368  .z.Stack._set_ch
+000009b0: 696c 6472 656e da06 7265 7475 726e 6301  ildren..returnc.
+000009c0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+000009d0: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
+000009e0: 5300 7241 0000 0029 0172 1f00 0000 2901  S.rA...).r....).
+000009f0: 7229 0000 0072 1600 0000 7216 0000 0072  r)...r....r....r
+00000a00: 2d00 0000 da07 7374 6163 6b65 646a 0000  -.....stackedj..
+00000a10: 0073 0200 0000 0602 7a0d 5374 6163 6b2e  .s......z.Stack.
+00000a20: 7374 6163 6b65 6429 19da 085f 5f6e 616d  stacked)...__nam
+00000a30: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000a40: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0800  .__qualname__r..
+00000a50: 0000 720e 0000 0072 0200 0000 da0f 5f5f  ..r....r......__
+00000a60: 616e 6e6f 7461 7469 6f6e 735f 5f72 0f00  annotations__r..
+00000a70: 0000 da08 5374 6163 6b41 6c6c 7203 0000  ....StackAllr...
+00000a80: 00da 046c 6973 7472 0500 0000 7206 0000  ...listr....r...
+00000a90: 0072 0700 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00000aa0: 7222 0000 00da 0373 7472 7217 0000 0072  r".....strr....r
+00000ab0: 3800 0000 7240 0000 0072 2700 0000 da08  8...r@...r'.....
+00000ac0: 7072 6f70 6572 7479 7243 0000 00da 0d5f  propertyrC....._
+00000ad0: 5f63 6c61 7373 6365 6c6c 5f5f 7216 0000  _classcell__r...
+00000ae0: 0072 1600 0000 722b 0000 0072 2d00 0000  .r....r+...r-...
+00000af0: 720d 0000 000a 0000 0073 3600 0000 0a00  r........s6.....
+00000b00: 0e01 0e01 0204 0601 0201 0201 0201 0201  ................
+00000b10: 06f9 1a02 02fe 0403 02fd 0404 02fc 0205  ................
+00000b20: 02fb 0a06 02fa 0207 0ef9 0824 081e 0812  ...........$....
+00000b30: 0208 1801 720d 0000 004e 2911 da04 656e  ....r....N)...en
+00000b40: 756d 7202 0000 00da 0674 7970 696e 6772  umr......typingr
+00000b50: 0300 0000 da11 5079 5369 6465 362e 5174  ......PySide6.Qt
+00000b60: 5769 6467 6574 7372 0400 0000 7205 0000  Widgetsr....r...
+00000b70: 0072 0600 0000 7207 0000 0072 0800 0000  .r....r....r....
+00000b80: da0f 7574 696c 732e 616c 6967 6e6d 656e  ..utils.alignmen
+00000b90: 7472 0a00 0000 da0b 636f 7265 2e72 6f75  tr......core.rou
+00000ba0: 7465 7372 0b00 0000 da04 636f 7265 720c  tesr......corer.
+00000bb0: 0000 0072 0d00 0000 7216 0000 0072 1600  ...r....r....r..
+00000bc0: 0000 7216 0000 0072 2d00 0000 da08 3c6d  ..r....r-.....<m
+00000bd0: 6f64 756c 653e 0100 0000 730e 0000 000c  odule>....s.....
+00000be0: 010c 011c 010c 010c 010c 0116 03         .............
```

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/stack.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/stack.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/stacked_widget.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/stacked_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/stacked_widget.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/stacked_widget.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/tool_button.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/tool_button.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/tool_button.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/tool_button.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/widget.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/__pycache__/widget.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/__pycache__/widget.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/_widgets.py` & `qtica-0.5.0/Qtica/widgets/_widgets.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/application.py` & `qtica-0.5.0/Qtica/widgets/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python3
 
 import os
 import sys
 import signal
-from typing import Callable, NoReturn, Optional, Sequence, Union
+from typing import Callable, NoReturn, Optional, Union
 from PySide6.QtCore import QResource, Qt, Signal, qRegisterResourceData
 from PySide6.QtWidgets import QApplication, QStyleFactory, QWidget
 from PySide6.QtGui import QFontDatabase
 from ..core import AbstractQObject
 
 
 class Application(AbstractQObject, QApplication):
```

### Comparing `qtica-0.4.3/Qtica/widgets/buttons.py` & `qtica-0.5.0/Qtica/widgets/buttons.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/container.py` & `qtica-0.5.0/Qtica/widgets/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         if child is not None:
             if isinstance(child, QWidget):
                 child.setParent(self)
             elif isinstance(child, QLayout):
                 child.setProperty("parent", self)
                 self.setLayout(child)
 
-            if padding is not None:
-                self.setContentsMargins(*padding if isinstance(padding, (tuple, list)) else padding)
+        if padding is not None:
+            self.setContentsMargins(*padding if isinstance(padding, (tuple, list)) else padding)
 
 
 class WidgetContainer(AbstractWidget, QWidget):
     def __init__(self, *, child: Union[QWidget, QLayout] = None, **kwargs):
         QWidget.__init__(self)
         super().__init__(**kwargs)
 
@@ -38,8 +38,8 @@
                 child.setParent(self)
             elif isinstance(child, QLayout):
                 child.setProperty("parent", self)
                 self.setLayout(child)
 
 
 class Container(FrameContainer):
-    ...
+    pass
```

### Comparing `qtica-0.4.3/Qtica/widgets/dialogs/__pycache__/base.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/dialogs/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/dialogs/__pycache__/large_text.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/dialogs/__pycache__/large_text.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/dialogs/__pycache__/mask.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/dialogs/__pycache__/mask.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/dialogs/__pycache__/mask.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/dialogs/__pycache__/mask.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/dialogs/__pycache__/silent.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/dialogs/__pycache__/silent.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/dialogs/__pycache__/silent.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/dialogs/__pycache__/silent.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/dialogs/__pycache__/teaching_tip.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/dialogs/__pycache__/teaching_tip.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/dialogs/__pycache__/text.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/dialogs/__pycache__/text.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/dialogs/mask.py` & `qtica-0.5.0/Qtica/widgets/dialogs/mask.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/dialogs/silent.py` & `qtica-0.5.0/Qtica/widgets/dialogs/silent.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/dialogs/teaching_tip/__pycache__/tails.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/dialogs/teaching_tip/__pycache__/tails.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/dialogs/teaching_tip/__pycache__/tails.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/dialogs/teaching_tip/__pycache__/tails.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/dialogs/teaching_tip/__pycache__/tool_tip.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/dialogs/teaching_tip/__pycache__/tool_tip.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jan  9 18:49:55 2024 UTC, .py size: 3114 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,248 +1,237 @@
-00000000: 6f0d 0d0a 0000 0000 5395 9d65 2a0c 0000  o.......S..e*...
+00000000: 6f0d 0d0a 0000 0000 60ea 5066 510b 0000  o.......`.PfQ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
+00000020: 0004 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
-00000060: 6d09 5a09 6d0a 5a0a 0100 6405 6406 6c0b  m.Z.m.Z...d.d.l.
-00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6407  m.Z.m.Z.m.Z...d.
-00000080: 6408 6c0f 6d10 5a10 0100 4700 6409 640a  d.l.m.Z...G.d.d.
-00000090: 8400 640a 6510 8303 5a11 640b 5300 290c  ..d.e...Z.d.S.).
-000000a0: e900 0000 0029 01da 0555 6e69 6f6e 2901  .....)...Union).
-000000b0: da08 5150 6169 6e74 6572 2902 da02 5174  ..QPainter)...Qt
-000000c0: da06 5145 7665 6e74 2903 da0b 5147 7269  ..QEvent)...QGri
-000000d0: 644c 6179 6f75 74da 0751 4c61 796f 7574  dLayout..QLayout
-000000e0: da07 5157 6964 6765 74e9 0100 0000 2903  ..QWidget.....).
-000000f0: da12 5465 6163 6869 6e67 5469 704d 616e  ..TeachingTipMan
-00000100: 6167 6572 da08 5f54 6169 6c50 6f73 da0e  ager.._TailPos..
-00000110: 5f54 6169 6c44 6972 6563 7469 6f6e e904  _TailDirection..
-00000120: 0000 0029 01da 0e41 6273 7472 6163 7444  ...)...AbstractD
-00000130: 6961 6c6f 6763 0000 0000 0000 0000 0000  ialogc..........
-00000140: 0000 0000 0000 0f00 0000 0000 0000 73aa  ..............s.
-00000150: 0000 0065 005a 0164 005a 0265 035a 0465  ...e.Z.d.Z.e.Z.e
-00000160: 055a 0664 0165 046a 0765 066a 0864 0264  .Z.d.e.j.e.j.d.d
-00000170: 0366 0564 0465 0965 0a65 0b66 0219 0064  .f.d.e.e.e.f...d
-00000180: 0565 0a64 0665 0464 0765 0664 0865 0c64  .e.d.e.d.e.d.e.d
-00000190: 0965 0d64 0a64 0166 0e87 0066 0164 0b64  .e.d.d.f...f.d.d
-000001a0: 0c84 0d5a 0e64 0d64 0e84 005a 0f64 0565  ...Z.d.d...Z.d.e
-000001b0: 0a66 0264 0f64 1084 045a 1064 1164 1284  .f.d.d...Z.d.d..
-000001c0: 005a 1187 0066 0164 1364 1484 085a 1264  .Z...f.d.d...Z.d
-000001d0: 1565 1366 0287 0066 0164 1664 1784 0c5a  .e.f...f.d.d...Z
-000001e0: 1464 1b64 1865 1566 0287 0066 0164 1964  .d.d.e.f...f.d.d
-000001f0: 1a84 0d5a 1687 0004 005a 1753 0029 1cda  ...Z.....Z.S.)..
-00000200: 1154 6561 6368 696e 6754 6970 4469 616c  .TeachingTipDial
-00000210: 6f67 4ee9 0800 0000 54da 0563 6869 6c64  ogN.....T..child
-00000220: da06 7461 7267 6574 da08 7461 696c 5f70  ..target..tail_p
-00000230: 6f73 da0e 7461 696c 5f64 6972 6563 7469  os..tail_directi
-00000240: 6f6e da08 7461 696c 5f6c 656e da0a 6175  on..tail_len..au
-00000250: 746f 5f63 6c6f 7365 da06 7265 7475 726e  to_close..return
-00000260: 6307 0000 0000 0000 0000 0000 0008 0000  c...............
-00000270: 0007 0000 000b 0000 0073 2601 0000 7400  .........s&...t.
-00000280: 8300 6a01 6407 6401 7c06 6901 7c07 a401  ..j.d.d.|.i.|...
-00000290: 8e01 0100 7c06 8800 5f02 7c01 8800 5f03  ....|..._.|..._.
-000002a0: 7c02 8800 5f04 7405 a006 7c03 a101 8800  |..._.t...|.....
-000002b0: 5f07 7c04 8800 6a07 5f08 7c05 8800 6a07  _.|...j._.|...j.
-000002c0: 5f09 740a 8800 8301 8800 5f0b 8800 6a0b  _.t......._...j.
-000002d0: a00c 6402 6402 6402 6402 a104 0100 8800  ..d.d.d.d.......
-000002e0: 6a0b a00d 6402 a101 0100 8800 6a07 a00e  j...d.......j...
-000002f0: 8800 a101 0100 740f 7c01 7410 8302 7251  ......t.|.t...rQ
-00000300: 8800 6a0b a011 7c01 6402 6402 7412 6a13  ..j...|.d.d.t.j.
-00000310: 6a14 7412 6a13 6a15 4200 a104 0100 6e06  j.t.j.j.B.....n.
-00000320: 8800 6a0b a016 7c01 a101 0100 8800 a017  ..j...|.........
-00000330: 7412 6a18 6a19 a101 0100 8800 a017 7412  t.j.j.........t.
-00000340: 6a18 6a1a a101 0100 8800 a01b 7412 6a1c  j.j.........t.j.
-00000350: 6a1d 7412 6a1c 6a1e 4200 a101 0100 8800  j.t.j.j.B.......
-00000360: 6a04 6400 7501 7291 8700 6601 6403 6404  j.d.u.r...f.d.d.
-00000370: 8408 8800 6a04 5f1f 8700 6601 6405 6404  ....j._...f.d.d.
-00000380: 8408 8800 6a04 5f20 8700 6601 6406 6404  ....j._ ..f.d.d.
-00000390: 8408 8800 6a04 a021 a100 5f20 6400 5300  ....j..!.._ d.S.
-000003a0: 6400 5300 2908 4e72 1600 0000 7201 0000  d.S.).Nr....r...
-000003b0: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-000003c0: 0000 0200 0000 1300 0000 f308 0000 0088  ................
-000003d0: 00a0 00a1 0053 00a9 014e a901 da0a 7570  .....S...N....up
-000003e0: 6461 7465 5f70 6f73 a901 da01 65a9 01da  date_pos....e...
-000003f0: 0473 656c 66a9 00fa 672f 686f 6d65 2f6f  .self...g/home/o
-00000400: 7361 6d61 2f57 6f72 6b73 7061 6365 2f2e  sama/Workspace/.
-00000410: 7665 6e76 2f6c 6962 2f70 7974 686f 6e33  venv/lib/python3
-00000420: 2e31 302f 7369 7465 2d70 6163 6b61 6765  .10/site-package
-00000430: 732f 5174 6963 612f 7769 6467 6574 732f  s/Qtica/widgets/
-00000440: 6469 616c 6f67 732f 7465 6163 6869 6e67  dialogs/teaching
-00000450: 5f74 6970 2f74 6f6f 6c5f 7469 702e 7079  _tip/tool_tip.py
-00000460: da08 3c6c 616d 6264 613e 3300 0000 f302  ..<lambda>3.....
-00000470: 0000 0008 007a 2c54 6561 6368 696e 6754  .....z,TeachingT
-00000480: 6970 4469 616c 6f67 2e5f 5f69 6e69 745f  ipDialog.__init_
-00000490: 5f2e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  _.<locals>.<lamb
-000004a0: 6461 3e63 0100 0000 0000 0000 0000 0000  da>c............
-000004b0: 0100 0000 0200 0000 1300 0000 7218 0000  ............r...
-000004c0: 0072 1900 0000 721a 0000 0072 1c00 0000  .r....r....r....
-000004d0: 721e 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
-000004e0: 2200 0000 3400 0000 7223 0000 0063 0100  "...4...r#...c..
-000004f0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00000500: 0000 1300 0000 7218 0000 0072 1900 0000  ......r....r....
-00000510: 721a 0000 0072 1c00 0000 721e 0000 0072  r....r....r....r
-00000520: 2000 0000 7221 0000 0072 2200 0000 3500   ...r!...r"...5.
-00000530: 0000 7223 0000 0072 2000 0000 2922 da05  ..r#...r ...)"..
-00000540: 7375 7065 72da 085f 5f69 6e69 745f 5fda  super..__init__.
-00000550: 0b5f 6175 746f 5f63 6c6f 7365 7211 0000  ._auto_closer...
-00000560: 0072 1200 0000 720a 0000 00da 046d 616b  .r....r......mak
-00000570: 65da 076d 616e 6167 6572 da09 6469 7265  e..manager..dire
-00000580: 6374 696f 6eda 066c 656e 6768 7472 0600  ction..lenghtr..
-00000590: 0000 da07 5f6c 6179 6f75 74da 1273 6574  ...._layout..set
-000005a0: 436f 6e74 656e 7473 4d61 7267 696e 73da  ContentsMargins.
-000005b0: 0a73 6574 5370 6163 696e 67da 0864 6f4c  .setSpacing..doL
-000005c0: 6179 6f75 74da 0a69 7369 6e73 7461 6e63  ayout..isinstanc
-000005d0: 6572 0700 0000 da09 6164 644c 6179 6f75  er......addLayou
-000005e0: 7472 0400 0000 da0d 416c 6967 6e6d 656e  tr......Alignmen
-000005f0: 7446 6c61 67da 0b41 6c69 676e 4365 6e74  tFlag..AlignCent
-00000600: 6572 da0c 416c 6967 6e48 4365 6e74 6572  er..AlignHCenter
-00000610: da09 6164 6457 6964 6765 74da 0c73 6574  ..addWidget..set
-00000620: 4174 7472 6962 7574 65da 0f57 6964 6765  Attribute..Widge
-00000630: 7441 7474 7269 6275 7465 da18 5741 5f54  tAttribute..WA_T
-00000640: 7261 6e73 6c75 6365 6e74 4261 636b 6772  ranslucentBackgr
-00000650: 6f75 6e64 da13 5741 5f53 7479 6c65 6442  ound..WA_StyledB
-00000660: 6163 6b67 726f 756e 64da 0e73 6574 5769  ackground..setWi
-00000670: 6e64 6f77 466c 6167 73da 0a57 696e 646f  ndowFlags..Windo
-00000680: 7754 7970 65da 0454 6f6f 6cda 1346 7261  wType..Tool..Fra
-00000690: 6d65 6c65 7373 5769 6e64 6f77 4869 6e74  melessWindowHint
-000006a0: da0b 7265 7369 7a65 4576 656e 74da 096d  ..resizeEvent..m
-000006b0: 6f76 6545 7665 6e74 da06 7769 6e64 6f77  oveEvent..window
-000006c0: 2908 721f 0000 0072 1100 0000 7212 0000  ).r....r....r...
-000006d0: 0072 1300 0000 7214 0000 0072 1500 0000  .r....r....r....
-000006e0: 7216 0000 00da 066b 7761 7267 73a9 01da  r......kwargs...
-000006f0: 095f 5f63 6c61 7373 5f5f 721e 0000 0072  .__class__r....r
-00000700: 2100 0000 7225 0000 000d 0000 0073 3400  !...r%.......s4.
-00000710: 0000 1608 0602 0602 0601 0c02 0801 0801  ................
-00000720: 0a02 1201 0c01 0c02 0a02 2001 0c02 0e03  .......... .....
-00000730: 0e01 0401 0601 0601 02ff 04ff 0a04 1001  ................
-00000740: 1001 1801 04fd 7a1a 5465 6163 6869 6e67  ......z.Teaching
-00000750: 5469 7044 6961 6c6f 672e 5f5f 696e 6974  TipDialog.__init
-00000760: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
-00000770: 0000 0003 0000 0043 0000 0073 0c00 0000  .......C...s....
-00000780: 7c00 6a00 a001 7c00 a101 5300 7219 0000  |.j...|...S.r...
-00000790: 0029 0272 2800 0000 da08 706f 7369 7469  .).r(.....positi
-000007a0: 6f6e 721e 0000 0072 2000 0000 7220 0000  onr....r ...r ..
-000007b0: 0072 2100 0000 da0b 746f 6f6c 7469 705f  .r!.....tooltip_
-000007c0: 706f 7337 0000 0073 0200 0000 0c01 7a1d  pos7...s......z.
-000007d0: 5465 6163 6869 6e67 5469 7044 6961 6c6f  TeachingTipDialo
-000007e0: 672e 746f 6f6c 7469 705f 706f 7363 0200  g.tooltip_posc..
-000007f0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00000800: 0000 0300 0000 733e 0000 007c 0188 005f  ......s>...|..._
-00000810: 0087 0066 0164 0164 0284 0888 006a 005f  ...f.d.d.....j._
-00000820: 0187 0066 0164 0364 0284 0888 006a 005f  ...f.d.d.....j._
-00000830: 0287 0066 0164 0464 0284 0888 006a 00a0  ...f.d.d.....j..
-00000840: 03a1 005f 0264 0053 0029 054e 6301 0000  ..._.d.S.).Nc...
-00000850: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-00000860: 0013 0000 0072 1800 0000 7219 0000 0072  .....r....r....r
-00000870: 1a00 0000 721c 0000 0072 1e00 0000 7220  ....r....r....r 
-00000880: 0000 0072 2100 0000 7222 0000 003c 0000  ...r!...r"...<..
-00000890: 0072 2300 0000 7a2e 5465 6163 6869 6e67  .r#...z.Teaching
-000008a0: 5469 7044 6961 6c6f 672e 7365 745f 7461  TipDialog.set_ta
-000008b0: 7267 6574 2e3c 6c6f 6361 6c73 3e2e 3c6c  rget.<locals>.<l
-000008c0: 616d 6264 613e 6301 0000 0000 0000 0000  ambda>c.........
-000008d0: 0000 0001 0000 0002 0000 0013 0000 0072  ...............r
-000008e0: 1800 0000 7219 0000 0072 1a00 0000 721c  ....r....r....r.
-000008f0: 0000 0072 1e00 0000 7220 0000 0072 2100  ...r....r ...r!.
-00000900: 0000 7222 0000 003d 0000 0072 2300 0000  ..r"...=...r#...
-00000910: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000920: 0002 0000 0013 0000 0072 1800 0000 7219  .........r....r.
-00000930: 0000 0072 1a00 0000 721c 0000 0072 1e00  ...r....r....r..
-00000940: 0000 7220 0000 0072 2100 0000 7222 0000  ..r ...r!...r"..
-00000950: 003e 0000 0072 2300 0000 2904 7212 0000  .>...r#...).r...
-00000960: 0072 3d00 0000 723e 0000 0072 3f00 0000  .r=...r>...r?...
-00000970: 2902 721f 0000 0072 1200 0000 7220 0000  ).r....r....r ..
-00000980: 0072 1e00 0000 7221 0000 00da 0a73 6574  .r....r!.....set
-00000990: 5f74 6172 6765 743a 0000 0073 0800 0000  _target:...s....
-000009a0: 0601 1001 1001 1801 7a1c 5465 6163 6869  ........z.Teachi
-000009b0: 6e67 5469 7044 6961 6c6f 672e 7365 745f  ngTipDialog.set_
-000009c0: 7461 7267 6574 6301 0000 0000 0000 0000  targetc.........
-000009d0: 0000 0001 0000 0005 0000 0043 0000 0073  ...........C...s
-000009e0: 1600 0000 7c00 a000 7c00 6a01 a002 7c00  ....|...|.j...|.
-000009f0: a101 a101 0100 6400 5300 7219 0000 0029  ......d.S.r....)
-00000a00: 03da 046d 6f76 6572 2800 0000 7243 0000  ...mover(...rC..
-00000a10: 0072 1e00 0000 7220 0000 0072 2000 0000  .r....r ...r ...
-00000a20: 7221 0000 0072 1b00 0000 4000 0000 7302  r!...r....@...s.
-00000a30: 0000 0016 017a 1c54 6561 6368 696e 6754  .....z.TeachingT
-00000a40: 6970 4469 616c 6f67 2e75 7064 6174 655f  ipDialog.update_
-00000a50: 706f 7363 0200 0000 0000 0000 0000 0000  posc............
-00000a60: 0200 0000 0300 0000 0300 0000 7318 0000  ............s...
-00000a70: 007c 00a0 00a1 0001 0074 0183 00a0 027c  .|.......t.....|
-00000a80: 01a1 0101 0064 0053 0072 1900 0000 2903  .....d.S.r....).
-00000a90: 721b 0000 0072 2400 0000 da09 7368 6f77  r....r$.....show
-00000aa0: 4576 656e 7429 0272 1f00 0000 721d 0000  Event).r....r...
-00000ab0: 0072 4100 0000 7220 0000 0072 2100 0000  .rA...r ...r!...
-00000ac0: 7247 0000 0043 0000 0073 0400 0000 0801  rG...C...s......
-00000ad0: 1001 7a1b 5465 6163 6869 6e67 5469 7044  ..z.TeachingTipD
-00000ae0: 6961 6c6f 672e 7368 6f77 4576 656e 7472  ialog.showEventr
-00000af0: 1d00 0000 6303 0000 0000 0000 0000 0000  ....c...........
-00000b00: 0003 0000 0005 0000 0003 0000 0073 5600  .............sV.
-00000b10: 0000 7c00 a000 a100 7224 7c01 7c00 a000  ..|.....r$|.|...
-00000b20: a100 a001 a100 7500 7224 7c02 a002 a100  ......u.r$|.....
-00000b30: 7403 6a04 6a05 7403 6a04 6a06 7403 6a04  t.j.j.t.j.j.t.j.
-00000b40: 6a07 6603 7600 7224 7c00 a008 7c00 6a09  j.f.v.r$|...|.j.
-00000b50: a00a 7c00 a101 a101 0100 740b 8300 a00c  ..|.......t.....
-00000b60: 7c01 7c02 a102 5300 7219 0000 0029 0dda  |.|...S.r....)..
-00000b70: 0670 6172 656e 7472 3f00 0000 da04 7479  .parentr?.....ty
-00000b80: 7065 7205 0000 00da 0454 7970 65da 0652  per......Type..R
-00000b90: 6573 697a 65da 1157 696e 646f 7753 7461  esize..WindowSta
-00000ba0: 7465 4368 616e 6765 da04 4d6f 7665 7246  teChange..MoverF
-00000bb0: 0000 0072 2800 0000 7243 0000 0072 2400  ...r(...rC...r$.
-00000bc0: 0000 da0b 6576 656e 7446 696c 7465 7229  ....eventFilter)
-00000bd0: 0372 1f00 0000 da03 6f62 6a72 1d00 0000  .r......objr....
-00000be0: 7241 0000 0072 2000 0000 7221 0000 0072  rA...r ...r!...r
-00000bf0: 4e00 0000 4700 0000 730e 0000 0018 010c  N...G...s.......
-00000c00: 0106 0106 0106 fe12 030e 017a 1d54 6561  ...........z.Tea
-00000c10: 6368 696e 6754 6970 4469 616c 6f67 2e65  chingTipDialog.e
-00000c20: 7665 6e74 4669 6c74 6572 da05 7363 616c  ventFilter..scal
-00000c30: 6563 0300 0000 0000 0000 0000 0000 0500  ec..............
-00000c40: 0000 0400 0000 0300 0000 7362 0000 0074  ..........sb...t
-00000c50: 0083 00a0 017c 01a1 0101 0074 027c 0083  .....|.....t.|..
-00000c60: 017d 037c 03a0 0374 026a 046a 05a1 0101  .}.|...t.j.j....
-00000c70: 007c 006a 06a0 07a1 00a0 087c 006a 06a0  .|.j.......|.j..
-00000c80: 09a1 00a1 017d 047c 03a0 0a7c 04a1 0101  .....}.|...|....
-00000c90: 007c 03a0 0b7c 04a0 0ca1 00a1 0101 007c  .|...|.........|
-00000ca0: 006a 0da0 0e7c 007c 03a1 0201 0064 0053  .j...|.|.....d.S
-00000cb0: 0072 1900 0000 290f 7224 0000 00da 0a70  .r....).r$.....p
-00000cc0: 6169 6e74 4576 656e 7472 0300 0000 da0e  aintEventr......
-00000cd0: 7365 7452 656e 6465 7248 696e 7473 da0a  setRenderHints..
-00000ce0: 5265 6e64 6572 4869 6e74 da0c 416e 7469  RenderHint..Anti
-00000cf0: 616c 6961 7369 6e67 7211 0000 00da 0770  aliasingr......p
-00000d00: 616c 6574 7465 da05 6272 7573 68da 0e62  alette..brush..b
-00000d10: 6163 6b67 726f 756e 6452 6f6c 65da 0873  ackgroundRole..s
-00000d20: 6574 4272 7573 68da 0673 6574 5065 6eda  etBrush..setPen.
-00000d30: 0563 6f6c 6f72 7228 0000 00da 0464 7261  .colorr(.....dra
-00000d40: 7729 0572 1f00 0000 721d 0000 0072 5000  w).r....r....rP.
-00000d50: 0000 da07 7061 696e 7465 72da 0862 675f  ....painter..bg_
-00000d60: 636f 6c6f 7272 4100 0000 7220 0000 0072  colorrA...r ...r
-00000d70: 2100 0000 7251 0000 004f 0000 0073 0e00  !...rQ...O...s..
-00000d80: 0000 0c01 0802 0e01 1602 0a02 0e01 1202  ................
-00000d90: 7a1c 5465 6163 6869 6e67 5469 7044 6961  z.TeachingTipDia
-00000da0: 6c6f 672e 7061 696e 7445 7665 6e74 7219  log.paintEventr.
-00000db0: 0000 0029 18da 085f 5f6e 616d 655f 5fda  ...)...__name__.
-00000dc0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000dd0: 7561 6c6e 616d 655f 5f72 0b00 0000 da07  ualname__r......
-00000de0: 5461 696c 506f 7372 0c00 0000 da0d 5461  TailPosr......Ta
-00000df0: 696c 4469 7265 6374 696f 6eda 0662 6f74  ilDirection..bot
-00000e00: 746f 6dda 0663 656e 7465 7272 0200 0000  tom..centerr....
-00000e10: 7208 0000 0072 0700 0000 da03 696e 74da  r....r......int.
-00000e20: 0462 6f6f 6c72 2500 0000 7244 0000 0072  .boolr%...rD...r
-00000e30: 4500 0000 721b 0000 0072 4700 0000 7205  E...r....rG...r.
-00000e40: 0000 0072 4e00 0000 da05 666c 6f61 7472  ...rN.....floatr
-00000e50: 5100 0000 da0d 5f5f 636c 6173 7363 656c  Q.....__classcel
-00000e60: 6c5f 5f72 2000 0000 7220 0000 0072 4100  l__r ...r ...rA.
-00000e70: 0000 7221 0000 0072 0f00 0000 0900 0000  ..r!...r........
-00000e80: 733a 0000 0008 0004 0104 0102 0404 0104  s:..............
-00000e90: 0102 0102 0104 fa0a 0102 ff02 0202 fe02  ................
-00000ea0: 0302 fd02 0402 fc02 0502 fb02 0602 fa02  ................
-00000eb0: 070e f908 2a0e 0308 060c 0312 041c 0872  ....*..........r
-00000ec0: 0f00 0000 4e29 12da 0674 7970 696e 6772  ....N)...typingr
-00000ed0: 0200 0000 da0d 5079 5369 6465 362e 5174  ......PySide6.Qt
-00000ee0: 4775 6972 0300 0000 da0e 5079 5369 6465  Guir......PySide
-00000ef0: 362e 5174 436f 7265 7204 0000 0072 0500  6.QtCorer....r..
-00000f00: 0000 da11 5079 5369 6465 362e 5174 5769  ....PySide6.QtWi
-00000f10: 6467 6574 7372 0600 0000 7207 0000 0072  dgetsr....r....r
-00000f20: 0800 0000 da05 7461 696c 7372 0a00 0000  ......tailsr....
-00000f30: 720b 0000 0072 0c00 0000 da04 636f 7265  r....r......core
-00000f40: 720e 0000 0072 0f00 0000 7220 0000 0072  r....r....r ...r
-00000f50: 2000 0000 7220 0000 0072 2100 0000 da08   ...r ...r!.....
-00000f60: 3c6d 6f64 756c 653e 0100 0000 730e 0000  <module>....s...
-00000f70: 000c 000c 0110 0114 0114 010c 0114 03    ...............
+00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
+00000050: 6d06 5a06 6d07 5a07 0100 6404 6405 6c08  m.Z.m.Z...d.d.l.
+00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6406  m.Z.m.Z.m.Z...d.
+00000070: 6407 6c0c 6d0d 5a0d 0100 4700 6408 6409  d.l.m.Z...G.d.d.
+00000080: 8400 6409 650d 8303 5a0e 640a 5300 290b  ..d.e...Z.d.S.).
+00000090: e900 0000 0029 01da 0851 5061 696e 7465  .....)...QPainte
+000000a0: 7229 02da 0251 74da 0651 4576 656e 7429  r)...Qt..QEvent)
+000000b0: 02da 0b51 4772 6964 4c61 796f 7574 da07  ...QGridLayout..
+000000c0: 5157 6964 6765 74e9 0100 0000 2903 da12  QWidget.....)...
+000000d0: 5465 6163 6869 6e67 5469 704d 616e 6167  TeachingTipManag
+000000e0: 6572 da08 5f54 6169 6c50 6f73 da0e 5f54  er.._TailPos.._T
+000000f0: 6169 6c44 6972 6563 7469 6f6e e904 0000  ailDirection....
+00000100: 0029 01da 0e41 6273 7472 6163 7444 6961  .)...AbstractDia
+00000110: 6c6f 6763 0000 0000 0000 0000 0000 0000  logc............
+00000120: 0000 0000 0f00 0000 0000 0000 73a2 0000  ............s...
+00000130: 0065 005a 0164 005a 0265 035a 0465 055a  .e.Z.d.Z.e.Z.e.Z
+00000140: 0664 0165 046a 0765 066a 0864 0264 0366  .d.e.j.e.j.d.d.f
+00000150: 0564 0465 0964 0565 0964 0665 0464 0765  .d.e.d.e.d.e.d.e
+00000160: 0664 0865 0a64 0965 0b64 0a64 0166 0e87  .d.e.d.e.d.d.f..
+00000170: 0066 0164 0b64 0c84 0d5a 0c64 0d64 0e84  .f.d.d...Z.d.d..
+00000180: 005a 0d64 0565 0966 0264 0f64 1084 045a  .Z.d.e.f.d.d...Z
+00000190: 0e64 1164 1284 005a 0f87 0066 0164 1364  .d.d...Z...f.d.d
+000001a0: 1484 085a 1064 1565 1166 0287 0066 0164  ...Z.d.e.f...f.d
+000001b0: 1664 1784 0c5a 1264 1b64 1865 1366 0287  .d...Z.d.d.e.f..
+000001c0: 0066 0164 1964 1a84 0d5a 1487 0004 005a  .f.d.d...Z.....Z
+000001d0: 1553 0029 1cda 1154 6561 6368 696e 6754  .S.)...TeachingT
+000001e0: 6970 4469 616c 6f67 4ee9 0800 0000 54da  ipDialogN.....T.
+000001f0: 0563 6869 6c64 da06 7461 7267 6574 da08  .child..target..
+00000200: 7461 696c 5f70 6f73 da0e 7461 696c 5f64  tail_pos..tail_d
+00000210: 6972 6563 7469 6f6e da08 7461 696c 5f6c  irection..tail_l
+00000220: 656e da0a 6175 746f 5f63 6c6f 7365 da06  en..auto_close..
+00000230: 7265 7475 726e 6307 0000 0000 0000 0000  returnc.........
+00000240: 0000 0008 0000 0006 0000 000b 0000 0073  ...............s
+00000250: fc00 0000 7400 8300 6a01 6407 6401 7c06  ....t...j.d.d.|.
+00000260: 6901 7c07 a401 8e01 0100 7c06 8800 5f02  i.|.......|..._.
+00000270: 7c01 8800 5f03 7c02 8800 5f04 7405 a006  |..._.|..._.t...
+00000280: 7c03 a101 8800 5f07 7c04 8800 6a07 5f08  |....._.|...j._.
+00000290: 7c05 8800 6a07 5f09 740a 8800 8301 8800  |...j._.t.......
+000002a0: 5f0b 8800 6a0b a00c 6402 6402 6402 6402  _...j...d.d.d.d.
+000002b0: a104 0100 8800 6a0b a00d 6402 a101 0100  ......j...d.....
+000002c0: 8800 6a07 a00e 8800 a101 0100 8800 6a0b  ..j...........j.
+000002d0: a00f 7c01 a101 0100 8800 a010 7411 6a12  ..|.........t.j.
+000002e0: 6a13 a101 0100 8800 a010 7411 6a12 6a14  j.........t.j.j.
+000002f0: a101 0100 8800 a015 7411 6a16 6a17 7411  ........t.j.j.t.
+00000300: 6a16 6a18 4200 a101 0100 8800 6a04 6400  j.j.B.......j.d.
+00000310: 7501 727c 8700 6601 6403 6404 8408 8800  u.r|..f.d.d.....
+00000320: 6a04 5f19 8700 6601 6405 6404 8408 8800  j._...f.d.d.....
+00000330: 6a04 5f1a 8700 6601 6406 6404 8408 8800  j._...f.d.d.....
+00000340: 6a04 a01b a100 5f1a 6400 5300 6400 5300  j....._.d.S.d.S.
+00000350: 2908 4e72 1400 0000 7201 0000 0063 0100  ).Nr....r....c..
+00000360: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00000370: 0000 1300 0000 f308 0000 0088 00a0 00a1  ................
+00000380: 0053 00a9 014e a901 da0a 7570 6461 7465  .S...N....update
+00000390: 5f70 6f73 a901 da01 65a9 01da 0473 656c  _pos....e....sel
+000003a0: 66a9 00fa 672f 686f 6d65 2f6f 7361 6d61  f...g/home/osama
+000003b0: 2f57 6f72 6b73 7061 6365 2f2e 7665 6e76  /Workspace/.venv
+000003c0: 2f6c 6962 2f70 7974 686f 6e33 2e31 302f  /lib/python3.10/
+000003d0: 7369 7465 2d70 6163 6b61 6765 732f 5174  site-packages/Qt
+000003e0: 6963 612f 7769 6467 6574 732f 6469 616c  ica/widgets/dial
+000003f0: 6f67 732f 7465 6163 6869 6e67 5f74 6970  ogs/teaching_tip
+00000400: 2f74 6f6f 6c5f 7469 702e 7079 da08 3c6c  /tool_tip.py..<l
+00000410: 616d 6264 613e 2f00 0000 f302 0000 0008  ambda>/.........
+00000420: 007a 2c54 6561 6368 696e 6754 6970 4469  .z,TeachingTipDi
+00000430: 616c 6f67 2e5f 5f69 6e69 745f 5f2e 3c6c  alog.__init__.<l
+00000440: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e63  ocals>.<lambda>c
+00000450: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000460: 0200 0000 1300 0000 7216 0000 0072 1700  ........r....r..
+00000470: 0000 7218 0000 0072 1a00 0000 721c 0000  ..r....r....r...
+00000480: 0072 1e00 0000 721f 0000 0072 2000 0000  .r....r....r ...
+00000490: 3000 0000 7221 0000 0063 0100 0000 0000  0...r!...c......
+000004a0: 0000 0000 0000 0100 0000 0200 0000 1300  ................
+000004b0: 0000 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
+000004c0: 0072 1a00 0000 721c 0000 0072 1e00 0000  .r....r....r....
+000004d0: 721f 0000 0072 2000 0000 3100 0000 7221  r....r ...1...r!
+000004e0: 0000 0072 1e00 0000 291c da05 7375 7065  ...r....)...supe
+000004f0: 72da 085f 5f69 6e69 745f 5fda 0b5f 6175  r..__init__.._au
+00000500: 746f 5f63 6c6f 7365 720f 0000 0072 1000  to_closer....r..
+00000510: 0000 7208 0000 00da 046d 616b 65da 076d  ..r......make..m
+00000520: 616e 6167 6572 da09 6469 7265 6374 696f  anager..directio
+00000530: 6eda 066c 656e 6768 7472 0500 0000 da07  n..lenghtr......
+00000540: 5f6c 6179 6f75 74da 1273 6574 436f 6e74  _layout..setCont
+00000550: 656e 7473 4d61 7267 696e 73da 0a73 6574  entsMargins..set
+00000560: 5370 6163 696e 67da 0864 6f4c 6179 6f75  Spacing..doLayou
+00000570: 74da 0961 6464 5769 6467 6574 da0c 7365  t..addWidget..se
+00000580: 7441 7474 7269 6275 7465 7203 0000 00da  tAttributer.....
+00000590: 0f57 6964 6765 7441 7474 7269 6275 7465  .WidgetAttribute
+000005a0: da18 5741 5f54 7261 6e73 6c75 6365 6e74  ..WA_Translucent
+000005b0: 4261 636b 6772 6f75 6e64 da13 5741 5f53  Background..WA_S
+000005c0: 7479 6c65 6442 6163 6b67 726f 756e 64da  tyledBackground.
+000005d0: 0e73 6574 5769 6e64 6f77 466c 6167 73da  .setWindowFlags.
+000005e0: 0a57 696e 646f 7754 7970 65da 0454 6f6f  .WindowType..Too
+000005f0: 6cda 1346 7261 6d65 6c65 7373 5769 6e64  l..FramelessWind
+00000600: 6f77 4869 6e74 da0b 7265 7369 7a65 4576  owHint..resizeEv
+00000610: 656e 74da 096d 6f76 6545 7665 6e74 da06  ent..moveEvent..
+00000620: 7769 6e64 6f77 2908 721d 0000 0072 0f00  window).r....r..
+00000630: 0000 7210 0000 0072 1100 0000 7212 0000  ..r....r....r...
+00000640: 0072 1300 0000 7214 0000 00da 066b 7761  .r....r......kwa
+00000650: 7267 73a9 01da 095f 5f63 6c61 7373 5f5f  rgs....__class__
+00000660: 721c 0000 0072 1f00 0000 7223 0000 000c  r....r....r#....
+00000670: 0000 0073 3000 0000 1608 0602 0602 0601  ...s0...........
+00000680: 0c02 0801 0801 0a02 1201 0c01 0c02 0c02  ................
+00000690: 0e03 0e01 0401 0601 0601 02ff 04ff 0a04  ................
+000006a0: 1001 1001 1801 04fd 7a1a 5465 6163 6869  ........z.Teachi
+000006b0: 6e67 5469 7044 6961 6c6f 672e 5f5f 696e  ngTipDialog.__in
+000006c0: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
+000006d0: 0001 0000 0003 0000 0043 0000 0073 0c00  .........C...s..
+000006e0: 0000 7c00 6a00 a001 7c00 a101 5300 7217  ..|.j...|...S.r.
+000006f0: 0000 0029 0272 2600 0000 da08 706f 7369  ...).r&.....posi
+00000700: 7469 6f6e 721c 0000 0072 1e00 0000 721e  tionr....r....r.
+00000710: 0000 0072 1f00 0000 da0b 746f 6f6c 7469  ...r......toolti
+00000720: 705f 706f 7333 0000 0073 0200 0000 0c01  p_pos3...s......
+00000730: 7a1d 5465 6163 6869 6e67 5469 7044 6961  z.TeachingTipDia
+00000740: 6c6f 672e 746f 6f6c 7469 705f 706f 7363  log.tooltip_posc
+00000750: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000760: 0300 0000 0300 0000 733e 0000 007c 0188  ........s>...|..
+00000770: 005f 0087 0066 0164 0164 0284 0888 006a  ._...f.d.d.....j
+00000780: 005f 0187 0066 0164 0364 0284 0888 006a  ._...f.d.d.....j
+00000790: 005f 0287 0066 0164 0464 0284 0888 006a  ._...f.d.d.....j
+000007a0: 00a0 03a1 005f 0264 0053 0029 054e 6301  ....._.d.S.).Nc.
+000007b0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+000007c0: 0000 0013 0000 0072 1600 0000 7217 0000  .......r....r...
+000007d0: 0072 1800 0000 721a 0000 0072 1c00 0000  .r....r....r....
+000007e0: 721e 0000 0072 1f00 0000 7220 0000 0038  r....r....r ...8
+000007f0: 0000 0072 2100 0000 7a2e 5465 6163 6869  ...r!...z.Teachi
+00000800: 6e67 5469 7044 6961 6c6f 672e 7365 745f  ngTipDialog.set_
+00000810: 7461 7267 6574 2e3c 6c6f 6361 6c73 3e2e  target.<locals>.
+00000820: 3c6c 616d 6264 613e 6301 0000 0000 0000  <lambda>c.......
+00000830: 0000 0000 0001 0000 0002 0000 0013 0000  ................
+00000840: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
+00000850: 721a 0000 0072 1c00 0000 721e 0000 0072  r....r....r....r
+00000860: 1f00 0000 7220 0000 0039 0000 0072 2100  ....r ...9...r!.
+00000870: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
+00000880: 0000 0002 0000 0013 0000 0072 1600 0000  ...........r....
+00000890: 7217 0000 0072 1800 0000 721a 0000 0072  r....r....r....r
+000008a0: 1c00 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
+000008b0: 0000 003a 0000 0072 2100 0000 2904 7210  ...:...r!...).r.
+000008c0: 0000 0072 3600 0000 7237 0000 0072 3800  ...r6...r7...r8.
+000008d0: 0000 2902 721d 0000 0072 1000 0000 721e  ..).r....r....r.
+000008e0: 0000 0072 1c00 0000 721f 0000 00da 0a73  ...r....r......s
+000008f0: 6574 5f74 6172 6765 7436 0000 0073 0800  et_target6...s..
+00000900: 0000 0601 1001 1001 1801 7a1c 5465 6163  ..........z.Teac
+00000910: 6869 6e67 5469 7044 6961 6c6f 672e 7365  hingTipDialog.se
+00000920: 745f 7461 7267 6574 6301 0000 0000 0000  t_targetc.......
+00000930: 0000 0000 0001 0000 0005 0000 0043 0000  .............C..
+00000940: 0073 1600 0000 7c00 a000 7c00 6a01 a002  .s....|...|.j...
+00000950: 7c00 a101 a101 0100 6400 5300 7217 0000  |.......d.S.r...
+00000960: 0029 03da 046d 6f76 6572 2600 0000 723c  .)...mover&...r<
+00000970: 0000 0072 1c00 0000 721e 0000 0072 1e00  ...r....r....r..
+00000980: 0000 721f 0000 0072 1900 0000 3c00 0000  ..r....r....<...
+00000990: 7302 0000 0016 017a 1c54 6561 6368 696e  s......z.Teachin
+000009a0: 6754 6970 4469 616c 6f67 2e75 7064 6174  gTipDialog.updat
+000009b0: 655f 706f 7363 0200 0000 0000 0000 0000  e_posc..........
+000009c0: 0000 0200 0000 0300 0000 0300 0000 7318  ..............s.
+000009d0: 0000 007c 00a0 00a1 0001 0074 0183 00a0  ...|.......t....
+000009e0: 027c 01a1 0101 0064 0053 0072 1700 0000  .|.....d.S.r....
+000009f0: 2903 7219 0000 0072 2200 0000 da09 7368  ).r....r".....sh
+00000a00: 6f77 4576 656e 7429 0272 1d00 0000 721b  owEvent).r....r.
+00000a10: 0000 0072 3a00 0000 721e 0000 0072 1f00  ...r:...r....r..
+00000a20: 0000 7240 0000 003f 0000 0073 0400 0000  ..r@...?...s....
+00000a30: 0801 1001 7a1b 5465 6163 6869 6e67 5469  ....z.TeachingTi
+00000a40: 7044 6961 6c6f 672e 7368 6f77 4576 656e  pDialog.showEven
+00000a50: 7472 1b00 0000 6303 0000 0000 0000 0000  tr....c.........
+00000a60: 0000 0003 0000 0005 0000 0003 0000 0073  ...............s
+00000a70: 5600 0000 7c00 a000 a100 7224 7c01 7c00  V...|.....r$|.|.
+00000a80: a000 a100 a001 a100 7500 7224 7c02 a002  ........u.r$|...
+00000a90: a100 7403 6a04 6a05 7403 6a04 6a06 7403  ..t.j.j.t.j.j.t.
+00000aa0: 6a04 6a07 6603 7600 7224 7c00 a008 7c00  j.j.f.v.r$|...|.
+00000ab0: 6a09 a00a 7c00 a101 a101 0100 740b 8300  j...|.......t...
+00000ac0: a00c 7c01 7c02 a102 5300 7217 0000 0029  ..|.|...S.r....)
+00000ad0: 0dda 0670 6172 656e 7472 3800 0000 da04  ...parentr8.....
+00000ae0: 7479 7065 7204 0000 00da 0454 7970 65da  typer......Type.
+00000af0: 0652 6573 697a 65da 1157 696e 646f 7753  .Resize..WindowS
+00000b00: 7461 7465 4368 616e 6765 da04 4d6f 7665  tateChange..Move
+00000b10: 723f 0000 0072 2600 0000 723c 0000 0072  r?...r&...r<...r
+00000b20: 2200 0000 da0b 6576 656e 7446 696c 7465  ".....eventFilte
+00000b30: 7229 0372 1d00 0000 da03 6f62 6a72 1b00  r).r......objr..
+00000b40: 0000 723a 0000 0072 1e00 0000 721f 0000  ..r:...r....r...
+00000b50: 0072 4700 0000 4300 0000 730e 0000 0018  .rG...C...s.....
+00000b60: 010c 0106 0106 0106 fe12 030e 017a 1d54  .............z.T
+00000b70: 6561 6368 696e 6754 6970 4469 616c 6f67  eachingTipDialog
+00000b80: 2e65 7665 6e74 4669 6c74 6572 da05 7363  .eventFilter..sc
+00000b90: 616c 6563 0300 0000 0000 0000 0000 0000  alec............
+00000ba0: 0500 0000 0400 0000 0300 0000 7362 0000  ............sb..
+00000bb0: 0074 0083 00a0 017c 01a1 0101 0074 027c  .t.....|.....t.|
+00000bc0: 0083 017d 037c 03a0 0374 026a 046a 05a1  ...}.|...t.j.j..
+00000bd0: 0101 007c 006a 06a0 07a1 00a0 087c 006a  ...|.j.......|.j
+00000be0: 06a0 09a1 00a1 017d 047c 03a0 0a7c 04a1  .......}.|...|..
+00000bf0: 0101 007c 03a0 0b7c 04a0 0ca1 00a1 0101  ...|...|........
+00000c00: 007c 006a 0da0 0e7c 007c 03a1 0201 0064  .|.j...|.|.....d
+00000c10: 0053 0072 1700 0000 290f 7222 0000 00da  .S.r....).r"....
+00000c20: 0a70 6169 6e74 4576 656e 7472 0200 0000  .paintEventr....
+00000c30: da0e 7365 7452 656e 6465 7248 696e 7473  ..setRenderHints
+00000c40: da0a 5265 6e64 6572 4869 6e74 da0c 416e  ..RenderHint..An
+00000c50: 7469 616c 6961 7369 6e67 720f 0000 00da  tialiasingr.....
+00000c60: 0770 616c 6574 7465 da05 6272 7573 68da  .palette..brush.
+00000c70: 0e62 6163 6b67 726f 756e 6452 6f6c 65da  .backgroundRole.
+00000c80: 0873 6574 4272 7573 68da 0673 6574 5065  .setBrush..setPe
+00000c90: 6eda 0563 6f6c 6f72 7226 0000 00da 0464  n..colorr&.....d
+00000ca0: 7261 7729 0572 1d00 0000 721b 0000 0072  raw).r....r....r
+00000cb0: 4900 0000 da07 7061 696e 7465 72da 0862  I.....painter..b
+00000cc0: 675f 636f 6c6f 7272 3a00 0000 721e 0000  g_colorr:...r...
+00000cd0: 0072 1f00 0000 724a 0000 004b 0000 0073  .r....rJ...K...s
+00000ce0: 0e00 0000 0c01 0802 0e01 1602 0a02 0e01  ................
+00000cf0: 1202 7a1c 5465 6163 6869 6e67 5469 7044  ..z.TeachingTipD
+00000d00: 6961 6c6f 672e 7061 696e 7445 7665 6e74  ialog.paintEvent
+00000d10: 7217 0000 0029 16da 085f 5f6e 616d 655f  r....)...__name_
+00000d20: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000d30: 5f71 7561 6c6e 616d 655f 5f72 0900 0000  _qualname__r....
+00000d40: da07 5461 696c 506f 7372 0a00 0000 da0d  ..TailPosr......
+00000d50: 5461 696c 4469 7265 6374 696f 6eda 0662  TailDirection..b
+00000d60: 6f74 746f 6dda 0663 656e 7465 7272 0600  ottom..centerr..
+00000d70: 0000 da03 696e 74da 0462 6f6f 6c72 2300  ....int..boolr#.
+00000d80: 0000 723d 0000 0072 3e00 0000 7219 0000  ..r=...r>...r...
+00000d90: 0072 4000 0000 7204 0000 0072 4700 0000  .r@...r....rG...
+00000da0: da05 666c 6f61 7472 4a00 0000 da0d 5f5f  ..floatrJ.....__
+00000db0: 636c 6173 7363 656c 6c5f 5f72 1e00 0000  classcell__r....
+00000dc0: 721e 0000 0072 3a00 0000 721f 0000 0072  r....r:...r....r
+00000dd0: 0d00 0000 0800 0000 733a 0000 0008 0004  ........s:......
+00000de0: 0104 0102 0404 0104 0102 0102 0104 fa02  ................
+00000df0: 0102 ff02 0202 fe02 0302 fd02 0402 fc02  ................
+00000e00: 0502 fb02 0602 fa02 070e f908 270e 0308  ............'...
+00000e10: 060c 0312 041c 0872 0d00 0000 4e29 0fda  .......r....N)..
+00000e20: 0d50 7953 6964 6536 2e51 7447 7569 7202  .PySide6.QtGuir.
+00000e30: 0000 00da 0e50 7953 6964 6536 2e51 7443  .....PySide6.QtC
+00000e40: 6f72 6572 0300 0000 7204 0000 00da 1150  orer....r......P
+00000e50: 7953 6964 6536 2e51 7457 6964 6765 7473  ySide6.QtWidgets
+00000e60: 7205 0000 0072 0600 0000 da05 7461 696c  r....r......tail
+00000e70: 7372 0800 0000 7209 0000 0072 0a00 0000  sr....r....r....
+00000e80: da04 636f 7265 720c 0000 0072 0d00 0000  ..corer....r....
+00000e90: 721e 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
+00000ea0: 1f00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000eb0: 0000 730c 0000 000c 0010 0110 0114 010c  ..s.............
+00000ec0: 0114 03                                  ...
```

### Comparing `qtica-0.4.3/Qtica/widgets/dialogs/teaching_tip/__pycache__/tool_tip.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/dialogs/teaching_tip/__pycache__/tool_tip.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/dialogs/teaching_tip/tails.py` & `qtica-0.5.0/Qtica/widgets/dialogs/teaching_tip/tails.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/dialogs/teaching_tip/tool_tip.py` & `qtica-0.5.0/Qtica/widgets/dialogs/teaching_tip/tool_tip.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from typing import Union
 from PySide6.QtGui import QPainter
 from PySide6.QtCore import Qt, QEvent
-from PySide6.QtWidgets import QGridLayout, QLayout, QWidget
+from PySide6.QtWidgets import QGridLayout, QWidget
 from .tails import TeachingTipManager, _TailPos, _TailDirection
 from ....core import AbstractDialog
 
 
 class TeachingTipDialog(AbstractDialog):
     TailPos = _TailPos
     TailDirection = _TailDirection
 
     def __init__(self,
-                 child: Union[QWidget, QLayout],
+                 child: QWidget,
                  target: QWidget = None,
                  tail_pos: TailPos = TailPos.bottom,
                  tail_direction: TailDirection = TailDirection.center,
                  tail_len: int = 8,
                  auto_close: bool = True,
                  **kwargs) -> None:
         super().__init__(auto_close=auto_close, **kwargs)
@@ -31,18 +30,15 @@
 
         self._layout = QGridLayout(self)
         self._layout.setContentsMargins(0, 0, 0, 0)
         self._layout.setSpacing(0)
 
         self.manager.doLayout(self)
 
-        if isinstance(child, QLayout):
-            self._layout.addLayout(child, 0, 0, Qt.AlignmentFlag.AlignCenter | Qt.AlignmentFlag.AlignHCenter)
-        else:
-            self._layout.addWidget(child)
+        self._layout.addWidget(child)
 
         # set style
         self.setAttribute(Qt.WidgetAttribute.WA_TranslucentBackground)
         self.setAttribute(Qt.WidgetAttribute.WA_StyledBackground)
         self.setWindowFlags(
             Qt.WindowType.Tool
             | Qt.WindowType.FramelessWindowHint)
```

### Comparing `qtica-0.4.3/Qtica/widgets/eliding_label.py` & `qtica-0.5.0/Qtica/widgets/eliding_label.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/group_box.py` & `qtica-0.5.0/Qtica/widgets/group_box.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/icon_widget.py` & `qtica-0.5.0/Qtica/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/line.py` & `qtica-0.5.0/Qtica/widgets/line.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/menu.py` & `qtica-0.5.0/Qtica/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/quick_widget.py` & `qtica-0.5.0/Qtica/widgets/quick_widget.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 #!/usr/bin/python3
 
+import os
 from typing import Any, Union
-from PySide6.QtCore import QUrl, Qt
+from PySide6.QtCore import QUrl
 from PySide6.QtQuickWidgets import QQuickWidget
 from ..core import AbstractWidget
+from ..tools.qt_file_open import TempFile
 
 
 class QuickWidget(AbstractWidget, QQuickWidget):
     def __init__(self, 
                  qml: Union[QUrl, str],
                  *,
-                 context: list[tuple[str, Any]] = None,
+                 context: Union[list[tuple[str, Any]], dict[str, Any]] = None,
                  **kwargs):
-        QQuickWidget.__init__(self, qml)
+
+        if not os.path.exists(qml):
+            with TempFile(TempFile.OpenModeFlag.ReadWrite) as tf:
+                tf.write(bytes(qml, encoding="utf-8"))
+                tf.readAll()
+                QQuickWidget.__init__(self, tf.fileName())
+            del tf
+        else:
+            QQuickWidget.__init__(self, qml)
 
         self._context = context
 
         self.setUpdatesEnabled(True)
         self.setTabletTracking(True)
         self.setMouseTracking(True)
 
         self.setResizeMode(QQuickWidget.ResizeMode.SizeRootObjectToView)
-        self.setAttribute(Qt.WidgetAttribute.WA_X11NetWmWindowTypeDesktop, True)
 
         super().__init__(**kwargs)
 
         self.statusChanged.connect(self.__on_statusChanged)
 
     @property
     def root_object(self):
@@ -33,9 +42,11 @@
 
     @property
     def root_context(self):
         return self.rootContext()
 
     def __on_statusChanged(self, status):
         if self._context is not None:
-            for name, value in self._context:
+            for name, value in (self._context.items() 
+                                if isinstance(self._context, dict) 
+                                else self._context):
                 self.rootContext().setContextProperty(name, value)
```

### Comparing `qtica-0.4.3/Qtica/widgets/scroll_area.py` & `qtica-0.5.0/Qtica/widgets/scroll_area.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self.setWidgetResizable(True)
         self.setUpdatesEnabled(True)
 
         self.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.setSizeAdjustPolicy(QScrollArea.SizeAdjustPolicy.AdjustToContents)
 
         self.setFrameShape(QFrame.Shape.NoFrame)
-        self.setFrameShadow(QFrame.Shadow.Plain)
+        self.setFrameShadow(QFrame.Shadow.Raised)
 
         super().__init__(**kwargs)
 
         if child is not None:
             if isinstance(child, QLayout):
                 _widget = QWidget()
                 child.setProperty("parent", _widget)
```

### Comparing `qtica-0.4.3/Qtica/widgets/size_grip.py` & `qtica-0.5.0/Qtica/widgets/size_grip.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/stack.py` & `qtica-0.5.0/Qtica/widgets/stack.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,20 +85,17 @@
             if isinstance(child, Alignment):
                 _widget = child.child
 
                 if isinstance(_widget, QLayout):
                     _widget = QWidget(self)
                     _widget.setProperty("parent", _widget)
                     _widget.setLayout(_widget)
-                    self.routes.add(route, _widget)
-                    self.setAlignment(_widget, child.alignment)
 
-                elif isinstance(_widget, QWidget):
-                    self.routes.add(route, _widget)
-                    self.setAlignment(_widget, child.alignment)
+                self.routes.add(route, _widget)
+                self.setAlignment(_widget, child.alignment)
             else:
                 self.routes.add(route, child)
 
     def _set_children(self, children):
         if not children:
             return
```

### Comparing `qtica-0.4.3/Qtica/widgets/stacked_widget.py` & `qtica-0.5.0/Qtica/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/video_widget.py` & `qtica-0.5.0/Qtica/widgets/video_widget.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/window/__pycache__/base.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/window/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/window/__pycache__/frameless.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/window/__pycache__/frameless.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/window/__pycache__/frameless.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/window/__pycache__/frameless.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/window/__pycache__/mainwindow.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/window/__pycache__/mainwindow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/window/__pycache__/mainwindow.cpython-312.pyc` & `qtica-0.5.0/Qtica/widgets/window/__pycache__/mainwindow.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/window/__pycache__/routes.cpython-310.pyc` & `qtica-0.5.0/Qtica/widgets/window/__pycache__/routes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/window/base.py` & `qtica-0.5.0/Qtica/widgets/window/base.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/Qtica/widgets/window/frameless.py` & `qtica-0.5.0/Qtica/widgets/window/frameless.py`

 * *Files identical despite different names*

### Comparing `qtica-0.4.3/README.md` & `qtica-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,39 +5,37 @@
 </p>
 
 <p align="center">
   A Fast Way to Done Your Idea!
 </p>
 
 <h2 align="center">
-  v0.4.3
+  v0.5.0
 </h2>
 
 # Qtica
 
 Qtica is a Python library that offers a lightweight API built around native PySide6. It enables swift GUI prototyping utilizing contemporary declarative UI methods, all within Python.
 
 Qtica is currently in active development and not yet ready for stable release.
 
 ## Features
 
 - **Lightweight API:** Built around PySide6, Qtica offers a streamlined interface for GUI development.
 - **Declarative UI Techniques:** Facilitates the use of modern UI techniques directly within Python.
 - **Swift Prototyping:** Enables rapid GUI prototyping for efficient development.
 
-
 ## Installation
 
 You can install **Qtica** via pip:
 
 ```bash
 pip install qtica
 ```
 
-
 ## Usage
 
 ```python
 import os
 import sys
 from PySide6.QtGui import QColor
 from PySide6.QtCore import QSize, Qt
@@ -80,25 +78,22 @@
 
 app = Application(sys.argv)
 window = Window()
 window.show()
 sys.exit(app.exec())
 ```
 
-
 ## Documentation
 
 For more information and detailed usage examples, refer to the [documentation](https://omamkaz.gitbook.io/qtica/).
 
-
 ## License
 
 This project is licensed under the [GPL3 License](https://github.com/qtica-project/Qtica/blob/main/LICENSE).
 
-
 ## NOTE
 
 Welcome to Qtica!
 
 Thank you for choosing Qtica! Please be aware that this library is continuously evolving and is not yet considered stable as it's actively under development. We encourage you to use it for experimentation and kindly ask for your feedback, bug reports, suggestions, or improvements that align with your preferences. Your input is invaluable! 😊
 
-Thank you for being a part of Qtica's development journey!
+Thank you for being a part of Qtica's development journey!
```

### Comparing `qtica-0.4.3/pyproject.toml` & `qtica-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Qtica"
-version = "0.4.3"
+version = "0.5.0"
 description = "Qtica is a Python library that offers a lightweight API built around native PySide6. It enables swift GUI prototyping utilizing contemporary declarative UI methods, all within Python."
 authors = ["Osama Mohammed Al-zabidi <qticaproject@gmail.com>"]
 license = "GPL-3.0"
 readme = ["README.md", "CHANGELOG.md"]
 keywords = [
     "qt",
     "pyside6",
```

### Comparing `qtica-0.4.3/PKG-INFO` & `qtica-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Qtica
-Version: 0.4.3
+Version: 0.5.0
 Summary: Qtica is a Python library that offers a lightweight API built around native PySide6. It enables swift GUI prototyping utilizing contemporary declarative UI methods, all within Python.
 Home-page: https://github.com/qtica-project/Qtica
 License: GPL-3.0
 Keywords: qt,pyside6,python,declarative,qml,Qtica,fast,easy,toolkit,tools
 Author: Osama Mohammed Al-zabidi
 Author-email: qticaproject@gmail.com
 Requires-Python: >=3.10,<3.13
@@ -39,39 +39,37 @@
 </p>
 
 <p align="center">
   A Fast Way to Done Your Idea!
 </p>
 
 <h2 align="center">
-  v0.4.3
+  v0.5.0
 </h2>
 
 # Qtica
 
 Qtica is a Python library that offers a lightweight API built around native PySide6. It enables swift GUI prototyping utilizing contemporary declarative UI methods, all within Python.
 
 Qtica is currently in active development and not yet ready for stable release.
 
 ## Features
 
 - **Lightweight API:** Built around PySide6, Qtica offers a streamlined interface for GUI development.
 - **Declarative UI Techniques:** Facilitates the use of modern UI techniques directly within Python.
 - **Swift Prototyping:** Enables rapid GUI prototyping for efficient development.
 
-
 ## Installation
 
 You can install **Qtica** via pip:
 
 ```bash
 pip install qtica
 ```
 
-
 ## Usage
 
 ```python
 import os
 import sys
 from PySide6.QtGui import QColor
 from PySide6.QtCore import QSize, Qt
@@ -114,32 +112,30 @@
 
 app = Application(sys.argv)
 window = Window()
 window.show()
 sys.exit(app.exec())
 ```
 
-
 ## Documentation
 
 For more information and detailed usage examples, refer to the [documentation](https://omamkaz.gitbook.io/qtica/).
 
-
 ## License
 
 This project is licensed under the [GPL3 License](https://github.com/qtica-project/Qtica/blob/main/LICENSE).
 
-
 ## NOTE
 
 Welcome to Qtica!
 
 Thank you for choosing Qtica! Please be aware that this library is continuously evolving and is not yet considered stable as it's actively under development. We encourage you to use it for experimentation and kindly ask for your feedback, bug reports, suggestions, or improvements that align with your preferences. Your input is invaluable! 😊
 
 Thank you for being a part of Qtica's development journey!
+
 # Changelog
 
 ## 0.1.1 - (2023-11-05)
 
 ### Added
 
 - #### PySide6 Built-in Widgets
@@ -806,7 +802,45 @@
   - `BoxShadow`
 - `tools.ListWidgetItem`
 - `widgets.ListWidget` addItemWidget, addItemDelegate methods
 
 ### Fixed
 
 - `tools.qtcore.tools`, `tools.qtgui.tools` has no attribute, in aarch64 machines
+
+## 0.5.0 (2024-05-24)
+
+### Added
+
+- `layout.stacked.StackedLayout` Routes, dict types support.
+- `enums.QPA_Platforms` vnc, wayland_egl, vkkhrdisplay
+- `core.AbstractWidget` **PosEventsRange**, **PosEventsArg**, **PosEvents** classes
+- `core.AbstractWidget` **at_pos** argument.
+- `widgets.QuickWidget`
+- `tools.qtcore.objects.File`
+- `tools.TempFile`
+- `utils.BaseDir`
+- `utils.Modifiers`, `utils.Keys`, `utils.KeySequence`
+- `tools.LayoutWrapper`
+
+### Fixed
+
+- `core.AbstractBase` value type error when insert MArgs class type to add[Methods]
+
+### Changed
+
+- `tools.File` has been renamed to `tools.OpenFile`
+- `utils.modifiers.py` has been renamed to `utils.key_events.py`
+
+### Updated
+
+- `widgets.QuickWidget` **qml** argument can accept QML code from string.
+
+### Removed
+
+- `utils.CheckNone`
+- `tools.`
+  - `HLayoutWrapper`
+  - `ColumnLayoutWrapper`
+  - `RowLayoutWrapper`
+  - `VLayoutWrapper`
+
```


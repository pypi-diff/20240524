# Comparing `tmp/ex4nicegui-0.6.6.tar.gz` & `tmp/ex4nicegui-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex4nicegui-0.6.6.tar", last modified: Wed May 15 16:42:52 2024, max compression
+gzip compressed data, was "ex4nicegui-0.6.7.tar", max compression
```

## Comparing `ex4nicegui-0.6.6.tar` & `ex4nicegui-0.6.7.tar`

### file list

```diff
@@ -1,183 +1,154 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:52.057506 ex4nicegui-0.6.6/
--rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.6.6/LICENSE
--rw-rw-rw-   0        0        0    28006 2024-05-15 16:42:52.057506 ex4nicegui-0.6.6/PKG-INFO
--rw-rw-rw-   0        0        0    26470 2024-05-14 17:54:39.000000 ex4nicegui-0.6.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.213421 ex4nicegui-0.6.6/ex4nicegui/
--rw-rw-rw-   0        0        0      886 2024-05-15 16:42:30.000000 ex4nicegui-0.6.6/ex4nicegui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.235826 ex4nicegui-0.6.6/ex4nicegui/bi/
--rw-rw-rw-   0        0        0      315 2023-10-18 15:44:54.000000 ex4nicegui-0.6.6/ex4nicegui/bi/__init__.py
--rw-rw-rw-   0        0        0     7644 2024-04-26 16:54:25.000000 ex4nicegui-0.6.6/ex4nicegui/bi/dataSource.py
--rw-rw-rw-   0        0        0     8186 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/bi/dataSourceFacade.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.289755 ex4nicegui-0.6.6/ex4nicegui/bi/elements/
--rw-rw-rw-   0        0        0        0 2023-10-18 15:44:54.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/__init__.py
--rw-rw-rw-   0        0        0      358 2023-10-18 15:44:54.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/containers.py
--rw-rw-rw-   0        0        0      898 2023-10-18 15:44:54.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/layouts.py
--rw-rw-rw-   0        0        0     1534 2023-12-04 18:30:56.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/models.py
--rw-rw-rw-   0        0        0      808 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/text.py
--rw-rw-rw-   0        0        0     2009 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_aggrid.py
--rw-rw-rw-   0        0        0      852 2023-10-18 15:44:54.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_date_picker.js
--rw-rw-rw-   0        0        0     2260 2023-12-06 09:33:56.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_date_picker.py
--rw-rw-rw-   0        0        0     2248 2024-05-15 16:41:01.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_echarts.py
--rw-rw-rw-   0        0        0     5447 2023-12-06 09:33:56.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_radio.py
--rw-rw-rw-   0        0        0     4128 2023-12-06 09:33:56.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_range.py
--rw-rw-rw-   0        0        0     3872 2023-12-08 12:43:57.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_select.py
--rw-rw-rw-   0        0        0     2165 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_slider.py
--rw-rw-rw-   0        0        0     1810 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_table.py
--rw-rw-rw-   0        0        0     2067 2024-01-07 17:28:53.000000 ex4nicegui-0.6.6/ex4nicegui/bi/index.py
--rw-rw-rw-   0        0        0     4529 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/bi/protocols.py
--rw-rw-rw-   0        0        0      355 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/bi/types.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.291984 ex4nicegui-0.6.6/ex4nicegui/experimental_/
--rw-rw-rw-   0        0        0       69 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/experimental_/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.291984 ex4nicegui-0.6.6/ex4nicegui/experimental_/gridLayout/
--rw-rw-rw-   0        0        0      125 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/experimental_/gridLayout/__init__.py
--rw-rw-rw-   0        0        0     4737 2023-10-18 15:44:54.000000 ex4nicegui-0.6.6/ex4nicegui/experimental_/gridLayout/index.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.340497 ex4nicegui-0.6.6/ex4nicegui/gsap/
--rw-rw-rw-   0        0        0      218 2024-02-27 20:13:02.000000 ex4nicegui-0.6.6/ex4nicegui/gsap/__init__.py
--rw-rw-rw-   0        0        0     4638 2024-04-26 16:54:25.000000 ex4nicegui-0.6.6/ex4nicegui/gsap/gsap.py
--rw-rw-rw-   0        0        0     1241 2024-02-27 20:13:02.000000 ex4nicegui-0.6.6/ex4nicegui/gsap/timeline.js
--rw-rw-rw-   0        0        0     2390 2024-04-26 16:54:25.000000 ex4nicegui-0.6.6/ex4nicegui/gsap/timeline.py
--rw-rw-rw-   0        0        0     1045 2024-02-02 15:27:35.000000 ex4nicegui-0.6.6/ex4nicegui/gsap/wrapGsap.js
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.350914 ex4nicegui-0.6.6/ex4nicegui/layout/
--rw-rw-rw-   0        0        0      278 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/layout/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.367467 ex4nicegui-0.6.6/ex4nicegui/layout/gridFlex/
--rw-rw-rw-   0        0        0     4468 2023-10-18 15:44:54.000000 ex4nicegui-0.6.6/ex4nicegui/layout/gridFlex/GridFlex.js
--rw-rw-rw-   0        0        0        2 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/layout/gridFlex/__init__.py
--rw-rw-rw-   0        0        0     7194 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/layout/gridFlex/gridFlex.py
--rw-rw-rw-   0        0        0     1236 2023-10-18 15:44:54.000000 ex4nicegui-0.6.6/ex4nicegui/layout/gridFlex/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.373543 ex4nicegui-0.6.6/ex4nicegui/layout/rxFlex/
--rw-rw-rw-   0        0        0        0 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/layout/rxFlex/__init__.py
--rw-rw-rw-   0        0        0     3672 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/layout/rxFlex/index.py
--rw-rw-rw-   0        0        0     1411 2023-10-18 15:44:54.000000 ex4nicegui-0.6.6/ex4nicegui/layout/rxFlex/types.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.375941 ex4nicegui-0.6.6/ex4nicegui/libs/
--rw-rw-rw-   0        0        0        0 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.485988 ex4nicegui-0.6.6/ex4nicegui/libs/d3/
--rw-rw-rw-   0        0        0        0 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/d3/__init__.py
--rw-rw-rw-   0        0        0    12795 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-color.ems.js
--rw-rw-rw-   0        0        0     2148 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-dispatch.ems.js
--rw-rw-rw-   0        0        0     4822 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-drag.ems.js
--rw-rw-rw-   0        0        0     3883 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-ease.ems.js
--rw-rw-rw-   0        0        0     9903 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-interpolate.ems.js
--rw-rw-rw-   0        0        0    16007 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-selection.ems.js
--rw-rw-rw-   0        0        0     2320 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-timer.ems.js
--rw-rw-rw-   0        0        0    14024 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-transition.ems.js
--rw-rw-rw-   0        0        0    11599 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-zoom.ems.js
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.633712 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/
--rw-rw-rw-   0        0        0    64907 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/CSSPlugin.js
--rw-rw-rw-   0        0        0     3674 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/CSSRulePlugin.js
--rw-rw-rw-   0        0        0    11588 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/CustomEase.js
--rw-rw-rw-   0        0        0   103102 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/Draggable.js
--rw-rw-rw-   0        0        0     5530 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/EasePack.js
--rw-rw-rw-   0        0        0     9125 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/EaselPlugin.js
--rw-rw-rw-   0        0        0    48981 2024-03-07 20:18:40.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/Flip.js
--rw-rw-rw-   0        0        0    12852 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/MotionPathPlugin.js
--rw-rw-rw-   0        0        0    26112 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/Observer.js
--rw-rw-rw-   0        0        0    15404 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/PixiPlugin.js
--rw-rw-rw-   0        0        0     9217 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/ScrollToPlugin.js
--rw-rw-rw-   0        0        0   112584 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/ScrollTrigger.js
--rw-rw-rw-   0        0        0     4877 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/TextPlugin.js
--rw-rw-rw-   0        0        0        0 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/__init__.py
--rw-rw-rw-   0        0        0     1585 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/all.js
--rw-rw-rw-   0        0        0   175009 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/gsap-core.js
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.667907 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/utils/
--rw-rw-rw-   0        0        0        0 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/utils/__init__.py
--rw-rw-rw-   0        0        0    15235 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/utils/matrix.js
--rw-rw-rw-   0        0        0    49314 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/utils/paths.js
--rw-rw-rw-   0        0        0    10472 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/libs/gsap/utils/strings.js
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.733449 ex4nicegui-0.6.6/ex4nicegui/reactive/
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.746480 ex4nicegui-0.6.6/ex4nicegui/reactive/EChartsComponent/
--rw-rw-rw-   0        0        0     3164 2024-05-15 16:41:01.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/EChartsComponent/ECharts.js
--rw-rw-rw-   0        0        0     4490 2024-05-15 16:41:01.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/EChartsComponent/ECharts.py
--rw-rw-rw-   0        0        0        0 2023-07-31 07:50:52.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/EChartsComponent/__init__.py
--rw-rw-rw-   0        0        0      570 2024-05-15 16:41:01.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/EChartsComponent/events.py
--rw-rw-rw-   0        0        0     1001 2024-05-15 16:41:01.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/EChartsComponent/types.py
--rw-rw-rw-   0        0        0     1463 2024-05-15 16:41:01.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/EChartsComponent/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.764733 ex4nicegui-0.6.6/ex4nicegui/reactive/UseDraggable/
--rw-rw-rw-   0        0        0     5473 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/UseDraggable/UseDraggable.js
--rw-rw-rw-   0        0        0     3929 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/UseDraggable/UseDraggable.py
--rw-rw-rw-   0        0        0        0 2023-07-17 16:36:22.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/UseDraggable/__init__.py
--rw-rw-rw-   0        0        0     3714 2024-03-25 14:45:22.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/__init__.py
--rw-rw-rw-   0        0        0      824 2024-05-15 08:33:29.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/deferredTask.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.801508 ex4nicegui-0.6.6/ex4nicegui/reactive/dropZone/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:45:08.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/dropZone/__init__.py
--rw-rw-rw-   0        0        0     2713 2023-07-29 10:16:25.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/dropZone/dropZone.js
--rw-rw-rw-   0        0        0     2590 2023-10-18 15:44:54.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/dropZone/dropZone.py
--rw-rw-rw-   0        0        0       50 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/empty.js
--rw-rw-rw-   0        0        0      132 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/empty.py
--rw-rw-rw-   0        0        0     1472 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/fileWatcher.py
--rw-rw-rw-   0        0        0     6225 2024-03-05 13:06:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/local_file_picker.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.821293 ex4nicegui-0.6.6/ex4nicegui/reactive/mermaid/
--rw-rw-rw-   0        0        0        0 2023-10-23 17:41:12.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/mermaid/__init__.py
--rw-rw-rw-   0        0        0     2308 2023-10-29 08:33:17.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/mermaid/mermaid.js
--rw-rw-rw-   0        0        0     2144 2024-02-05 16:01:34.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/mermaid/mermaid.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:52.001860 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/
--rw-rw-rw-   0        0        0        2 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/__init__.py
--rw-rw-rw-   0        0        0     2929 2024-03-07 20:18:40.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/aggrid.py
--rw-rw-rw-   0        0        0    10440 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/base.py
--rw-rw-rw-   0        0        0     1660 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/button.py
--rw-rw-rw-   0        0        0     1275 2023-07-21 14:29:40.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/card.py
--rw-rw-rw-   0        0        0     1562 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/checkbox.py
--rw-rw-rw-   0        0        0     1787 2024-02-29 13:12:44.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/circular_progress.py
--rw-rw-rw-   0        0        0     3402 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/color_picker.py
--rw-rw-rw-   0        0        0     1040 2024-02-29 12:25:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/column.py
--rw-rw-rw-   0        0        0     2681 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/date.py
--rw-rw-rw-   0        0        0     2370 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/drawer.py
--rw-rw-rw-   0        0        0     9495 2024-05-15 16:41:01.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/echarts.py
--rw-rw-rw-   0        0        0      412 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/element.py
--rw-rw-rw-   0        0        0     1873 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/expansion.py
--rw-rw-rw-   0        0        0      865 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/grid.py
--rw-rw-rw-   0        0        0      119 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/html.js
--rw-rw-rw-   0        0        0      675 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/html.py
--rw-rw-rw-   0        0        0     1559 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/icon.py
--rw-rw-rw-   0        0        0     1120 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/image.py
--rw-rw-rw-   0        0        0     4030 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/input.py
--rw-rw-rw-   0        0        0     2153 2024-02-29 11:46:48.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/knob.py
--rw-rw-rw-   0        0        0     1398 2024-03-04 19:14:43.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/label.py
--rw-rw-rw-   0        0        0     2128 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/linear_progress.py
--rw-rw-rw-   0        0        0     2236 2024-05-14 19:43:06.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/number.py
--rw-rw-rw-   0        0        0     1929 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/radio.py
--rw-rw-rw-   0        0        0     1029 2024-02-29 12:25:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/row.py
--rw-rw-rw-   0        0        0     2980 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/select.py
--rw-rw-rw-   0        0        0     2954 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/slider.py
--rw-rw-rw-   0        0        0     1605 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/switch.py
--rw-rw-rw-   0        0        0     1796 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/tab.py
--rw-rw-rw-   0        0        0      630 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/tab_panel.py
--rw-rw-rw-   0        0        0     1375 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/tab_panels.py
--rw-rw-rw-   0        0        0     6042 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/table.py
--rw-rw-rw-   0        0        0     1232 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/tabs.py
--rw-rw-rw-   0        0        0     3044 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/textarea.py
--rw-rw-rw-   0        0        0     2360 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/upload.py
--rw-rw-rw-   0        0        0      213 2024-02-21 13:27:29.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/officials/utils.py
--rw-rw-rw-   0        0        0     1505 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/q_pagination.py
--rw-rw-rw-   0        0        0       31 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/rxui.py
--rw-rw-rw-   0        0        0      898 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/transitionGroup.js
--rw-rw-rw-   0        0        0      597 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/transitionGroup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:52.025198 ex4nicegui-0.6.6/ex4nicegui/reactive/useMouse/
--rw-rw-rw-   0        0        0     2722 2023-07-17 15:14:14.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/useMouse/UseMouse.js
--rw-rw-rw-   0        0        0     2122 2024-02-23 16:33:09.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/useMouse/UseMouse.py
--rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/useMouse/__init__.py
--rw-rw-rw-   0        0        0     2598 2024-03-07 10:39:11.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/usePagination.py
--rw-rw-rw-   0        0        0     4360 2024-03-07 20:18:40.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/utils.py
--rw-rw-rw-   0        0        0      282 2024-03-21 14:24:33.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/vfor.js
--rw-rw-rw-   0        0        0     5778 2024-04-26 16:54:25.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/vfor.py
--rw-rw-rw-   0        0        0     5091 2024-03-05 13:12:27.000000 ex4nicegui-0.6.6/ex4nicegui/reactive/vmodel.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:52.028669 ex4nicegui-0.6.6/ex4nicegui/tools/
--rw-rw-rw-   0        0        0        0 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/tools/__init__.py
--rw-rw-rw-   0        0        0     4868 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/tools/debug.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:52.052490 ex4nicegui-0.6.6/ex4nicegui/utils/
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.6.6/ex4nicegui/utils/__init__.py
--rw-rw-rw-   0        0        0     2527 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/utils/apiEffect.py
--rw-rw-rw-   0        0        0     1505 2024-03-05 13:06:09.000000 ex4nicegui-0.6.6/ex4nicegui/utils/asyncComputed.py
--rw-rw-rw-   0        0        0     1719 2024-05-14 17:54:39.000000 ex4nicegui-0.6.6/ex4nicegui/utils/clientScope.py
--rw-rw-rw-   0        0        0      994 2024-02-20 10:06:17.000000 ex4nicegui-0.6.6/ex4nicegui/utils/common.py
--rw-rw-rw-   0        0        0     2310 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/utils/effect.py
--rw-rw-rw-   0        0        0     1218 2024-02-27 19:00:38.000000 ex4nicegui-0.6.6/ex4nicegui/utils/scheduler.py
--rw-rw-rw-   0        0        0    11346 2024-05-14 18:10:44.000000 ex4nicegui-0.6.6/ex4nicegui/utils/signals.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:42:51.224370 ex4nicegui-0.6.6/ex4nicegui.egg-info/
--rw-rw-rw-   0        0        0    28006 2024-05-15 16:42:50.000000 ex4nicegui-0.6.6/ex4nicegui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5635 2024-05-15 16:42:50.000000 ex4nicegui-0.6.6/ex4nicegui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 16:42:50.000000 ex4nicegui-0.6.6/ex4nicegui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-15 16:42:50.000000 ex4nicegui-0.6.6/ex4nicegui.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       58 2024-05-15 16:42:50.000000 ex4nicegui-0.6.6/ex4nicegui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-15 16:42:50.000000 ex4nicegui-0.6.6/ex4nicegui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 16:42:52.057506 ex4nicegui-0.6.6/setup.cfg
--rw-rw-rw-   0        0        0     1576 2024-04-26 16:54:25.000000 ex4nicegui-0.6.6/setup.py
+-rw-r--r--   0        0        0      886 2024-05-15 16:42:30.958325 ex4nicegui-0.6.7/ex4nicegui/__init__.py
+-rw-r--r--   0        0        0      315 2023-10-18 15:44:54.250598 ex4nicegui-0.6.7/ex4nicegui/bi/__init__.py
+-rw-r--r--   0        0        0     7644 2024-04-26 16:54:25.060834 ex4nicegui-0.6.7/ex4nicegui/bi/dataSource.py
+-rw-r--r--   0        0        0     8186 2024-02-27 19:00:38.846162 ex4nicegui-0.6.7/ex4nicegui/bi/dataSourceFacade.py
+-rw-r--r--   0        0        0        0 2023-10-18 15:44:54.265526 ex4nicegui-0.6.7/ex4nicegui/bi/elements/__init__.py
+-rw-r--r--   0        0        0      358 2023-10-18 15:44:54.266526 ex4nicegui-0.6.7/ex4nicegui/bi/elements/containers.py
+-rw-r--r--   0        0        0      898 2023-10-18 15:44:54.267522 ex4nicegui-0.6.7/ex4nicegui/bi/elements/layouts.py
+-rw-r--r--   0        0        0     1534 2023-12-04 18:30:56.007466 ex4nicegui-0.6.7/ex4nicegui/bi/elements/models.py
+-rw-r--r--   0        0        0      808 2024-02-27 19:00:38.846162 ex4nicegui-0.6.7/ex4nicegui/bi/elements/text.py
+-rw-r--r--   0        0        0     2009 2024-02-27 19:00:38.846162 ex4nicegui-0.6.7/ex4nicegui/bi/elements/ui_aggrid.py
+-rw-r--r--   0        0        0      852 2023-10-18 15:44:54.305691 ex4nicegui-0.6.7/ex4nicegui/bi/elements/ui_date_picker.js
+-rw-r--r--   0        0        0     2260 2023-12-06 09:33:56.911023 ex4nicegui-0.6.7/ex4nicegui/bi/elements/ui_date_picker.py
+-rw-r--r--   0        0        0     2248 2024-05-15 16:41:01.860980 ex4nicegui-0.6.7/ex4nicegui/bi/elements/ui_echarts.py
+-rw-r--r--   0        0        0     5447 2023-12-06 09:33:56.912069 ex4nicegui-0.6.7/ex4nicegui/bi/elements/ui_radio.py
+-rw-r--r--   0        0        0     4128 2023-12-06 09:33:56.912330 ex4nicegui-0.6.7/ex4nicegui/bi/elements/ui_range.py
+-rw-r--r--   0        0        0     3872 2023-12-08 12:43:57.167046 ex4nicegui-0.6.7/ex4nicegui/bi/elements/ui_select.py
+-rw-r--r--   0        0        0     2165 2024-02-27 19:00:38.846162 ex4nicegui-0.6.7/ex4nicegui/bi/elements/ui_slider.py
+-rw-r--r--   0        0        0     1810 2024-02-27 19:00:38.846162 ex4nicegui-0.6.7/ex4nicegui/bi/elements/ui_table.py
+-rw-r--r--   0        0        0     2067 2024-01-07 17:28:53.444520 ex4nicegui-0.6.7/ex4nicegui/bi/index.py
+-rw-r--r--   0        0        0     4529 2024-02-27 19:00:38.846162 ex4nicegui-0.6.7/ex4nicegui/bi/protocols.py
+-rw-r--r--   0        0        0      355 2024-02-27 19:00:38.846162 ex4nicegui-0.6.7/ex4nicegui/bi/types.py
+-rw-r--r--   0        0        0       69 2024-02-27 19:00:38.846162 ex4nicegui-0.6.7/ex4nicegui/experimental_/__init__.py
+-rw-r--r--   0        0        0      125 2024-02-27 19:00:38.846162 ex4nicegui-0.6.7/ex4nicegui/experimental_/gridLayout/__init__.py
+-rw-r--r--   0        0        0     4737 2023-10-18 15:44:54.427118 ex4nicegui-0.6.7/ex4nicegui/experimental_/gridLayout/index.py
+-rw-r--r--   0        0        0      218 2024-02-27 20:13:02.249493 ex4nicegui-0.6.7/ex4nicegui/gsap/__init__.py
+-rw-r--r--   0        0        0     4638 2024-04-26 16:54:25.060834 ex4nicegui-0.6.7/ex4nicegui/gsap/gsap.py
+-rw-r--r--   0        0        0     1241 2024-02-27 20:13:02.249493 ex4nicegui-0.6.7/ex4nicegui/gsap/timeline.js
+-rw-r--r--   0        0        0     2390 2024-04-26 16:54:25.060834 ex4nicegui-0.6.7/ex4nicegui/gsap/timeline.py
+-rw-r--r--   0        0        0     1045 2024-02-02 15:27:35.771126 ex4nicegui-0.6.7/ex4nicegui/gsap/wrapGsap.js
+-rw-r--r--   0        0        0      278 2024-02-27 19:00:38.846162 ex4nicegui-0.6.7/ex4nicegui/layout/__init__.py
+-rw-r--r--   0        0        0        2 2024-02-27 19:00:38.846162 ex4nicegui-0.6.7/ex4nicegui/layout/gridFlex/__init__.py
+-rw-r--r--   0        0        0     4468 2023-10-18 15:44:54.446995 ex4nicegui-0.6.7/ex4nicegui/layout/gridFlex/GridFlex.js
+-rw-r--r--   0        0        0     7194 2024-02-27 19:00:38.846162 ex4nicegui-0.6.7/ex4nicegui/layout/gridFlex/gridFlex.py
+-rw-r--r--   0        0        0     1236 2023-10-18 15:44:54.490034 ex4nicegui-0.6.7/ex4nicegui/layout/gridFlex/utils.py
+-rw-r--r--   0        0        0        0 2024-02-27 19:00:38.846162 ex4nicegui-0.6.7/ex4nicegui/layout/rxFlex/__init__.py
+-rw-r--r--   0        0        0     3672 2024-02-27 19:00:38.846162 ex4nicegui-0.6.7/ex4nicegui/layout/rxFlex/index.py
+-rw-r--r--   0        0        0     1411 2023-10-18 15:44:54.493709 ex4nicegui-0.6.7/ex4nicegui/layout/rxFlex/types.py
+-rw-r--r--   0        0        0        0 2024-02-05 16:01:34.537019 ex4nicegui-0.6.7/ex4nicegui/libs/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 16:01:34.537019 ex4nicegui-0.6.7/ex4nicegui/libs/d3/__init__.py
+-rw-r--r--   0        0        0    12795 2024-02-05 16:01:34.537019 ex4nicegui-0.6.7/ex4nicegui/libs/d3/d3-color.ems.js
+-rw-r--r--   0        0        0     2148 2024-02-05 16:01:34.537019 ex4nicegui-0.6.7/ex4nicegui/libs/d3/d3-dispatch.ems.js
+-rw-r--r--   0        0        0     4822 2024-02-05 16:01:34.537019 ex4nicegui-0.6.7/ex4nicegui/libs/d3/d3-drag.ems.js
+-rw-r--r--   0        0        0     3883 2024-02-05 16:01:34.537019 ex4nicegui-0.6.7/ex4nicegui/libs/d3/d3-ease.ems.js
+-rw-r--r--   0        0        0     9903 2024-02-05 16:01:34.541019 ex4nicegui-0.6.7/ex4nicegui/libs/d3/d3-interpolate.ems.js
+-rw-r--r--   0        0        0    16007 2024-02-05 16:01:34.541019 ex4nicegui-0.6.7/ex4nicegui/libs/d3/d3-selection.ems.js
+-rw-r--r--   0        0        0     2320 2024-02-05 16:01:34.541019 ex4nicegui-0.6.7/ex4nicegui/libs/d3/d3-timer.ems.js
+-rw-r--r--   0        0        0    14024 2024-02-05 16:01:34.541019 ex4nicegui-0.6.7/ex4nicegui/libs/d3/d3-transition.ems.js
+-rw-r--r--   0        0        0    11599 2024-02-05 16:01:34.541019 ex4nicegui-0.6.7/ex4nicegui/libs/d3/d3-zoom.ems.js
+-rw-r--r--   0        0        0     6148 2024-02-05 16:01:34.541019 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/.DS_Store
+-rw-r--r--   0        0        0        0 2024-02-05 16:01:34.553024 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/__init__.py
+-rw-r--r--   0        0        0     1585 2024-02-05 16:01:34.553024 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/all.js
+-rw-r--r--   0        0        0    64907 2024-02-05 16:01:34.545018 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/CSSPlugin.js
+-rw-r--r--   0        0        0     3674 2024-02-05 16:01:34.545018 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/CSSRulePlugin.js
+-rw-r--r--   0        0        0    11588 2024-02-05 16:01:34.545018 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/CustomEase.js
+-rw-r--r--   0        0        0   103102 2024-02-05 16:01:34.547413 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/Draggable.js
+-rw-r--r--   0        0        0     9125 2024-02-05 16:01:34.549024 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/EaselPlugin.js
+-rw-r--r--   0        0        0     5530 2024-02-05 16:01:34.549024 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/EasePack.js
+-rw-r--r--   0        0        0    48981 2024-03-07 20:18:40.905732 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/Flip.js
+-rw-r--r--   0        0        0   175009 2024-02-05 16:01:34.557024 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/gsap-core.js
+-rw-r--r--   0        0        0      669 2024-02-05 16:01:34.557024 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/gsap.mjs
+-rw-r--r--   0        0        0    12852 2024-02-05 16:01:34.549024 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/MotionPathPlugin.js
+-rw-r--r--   0        0        0    26112 2024-02-05 16:01:34.549024 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/Observer.js
+-rw-r--r--   0        0        0    15404 2024-02-05 16:01:34.549024 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/PixiPlugin.js
+-rw-r--r--   0        0        0     9217 2024-02-05 16:01:34.553024 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/ScrollToPlugin.js
+-rw-r--r--   0        0        0   112584 2024-02-05 16:01:34.553024 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/ScrollTrigger.js
+-rw-r--r--   0        0        0     4877 2024-02-05 16:01:34.553024 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/TextPlugin.js
+-rw-r--r--   0        0        0        0 2024-02-05 16:01:34.557024 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/utils/__init__.py
+-rw-r--r--   0        0        0    15235 2024-02-05 16:01:34.557024 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/utils/matrix.js
+-rw-r--r--   0        0        0    49314 2024-02-05 16:01:34.557024 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/utils/paths.js
+-rw-r--r--   0        0        0    10472 2024-02-05 16:01:34.561024 ex4nicegui-0.6.7/ex4nicegui/libs/gsap/utils/strings.js
+-rw-r--r--   0        0        0     3714 2024-03-25 14:45:22.344254 ex4nicegui-0.6.7/ex4nicegui/reactive/__init__.py
+-rw-r--r--   0        0        0      824 2024-05-15 08:33:29.337347 ex4nicegui-0.6.7/ex4nicegui/reactive/deferredTask.py
+-rw-r--r--   0        0        0        0 2023-07-31 07:45:08.861691 ex4nicegui-0.6.7/ex4nicegui/reactive/dropZone/__init__.py
+-rw-r--r--   0        0        0     2713 2023-07-29 10:16:25.563916 ex4nicegui-0.6.7/ex4nicegui/reactive/dropZone/dropZone.js
+-rw-r--r--   0        0        0     2590 2023-10-18 15:44:54.520163 ex4nicegui-0.6.7/ex4nicegui/reactive/dropZone/dropZone.py
+-rw-r--r--   0        0        0        0 2023-07-31 07:50:52.834725 ex4nicegui-0.6.7/ex4nicegui/reactive/EChartsComponent/__init__.py
+-rw-r--r--   0        0        0     3548 2024-05-24 11:08:07.607701 ex4nicegui-0.6.7/ex4nicegui/reactive/EChartsComponent/ECharts.js
+-rw-r--r--   0        0        0     4490 2024-05-15 16:41:01.862493 ex4nicegui-0.6.7/ex4nicegui/reactive/EChartsComponent/ECharts.py
+-rw-r--r--   0        0        0      570 2024-05-15 16:41:01.862493 ex4nicegui-0.6.7/ex4nicegui/reactive/EChartsComponent/events.py
+-rw-r--r--   0        0        0     1001 2024-05-15 16:41:01.862493 ex4nicegui-0.6.7/ex4nicegui/reactive/EChartsComponent/types.py
+-rw-r--r--   0        0        0     1463 2024-05-15 16:41:01.862493 ex4nicegui-0.6.7/ex4nicegui/reactive/EChartsComponent/utils.py
+-rw-r--r--   0        0        0       50 2024-03-21 14:24:33.887453 ex4nicegui-0.6.7/ex4nicegui/reactive/empty.js
+-rw-r--r--   0        0        0      132 2024-03-21 14:24:33.906291 ex4nicegui-0.6.7/ex4nicegui/reactive/empty.py
+-rw-r--r--   0        0        0     1472 2024-02-27 19:00:38.846162 ex4nicegui-0.6.7/ex4nicegui/reactive/fileWatcher.py
+-rw-r--r--   0        0        0     6225 2024-03-05 13:06:09.437440 ex4nicegui-0.6.7/ex4nicegui/reactive/local_file_picker.py
+-rw-r--r--   0        0        0        0 2023-10-23 17:41:12.427008 ex4nicegui-0.6.7/ex4nicegui/reactive/mermaid/__init__.py
+-rw-r--r--   0        0        0     2308 2023-10-29 08:33:17.515349 ex4nicegui-0.6.7/ex4nicegui/reactive/mermaid/mermaid.js
+-rw-r--r--   0        0        0     2144 2024-02-05 16:01:34.561024 ex4nicegui-0.6.7/ex4nicegui/reactive/mermaid/mermaid.py
+-rw-r--r--   0        0        0        2 2024-02-23 16:33:09.308742 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/__init__.py
+-rw-r--r--   0        0        0     2956 2024-05-16 16:48:25.034139 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/aggrid.py
+-rw-r--r--   0        0        0    10843 2024-05-16 16:57:19.453087 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/base.py
+-rw-r--r--   0        0        0     1701 2024-05-16 16:48:25.034139 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/button.py
+-rw-r--r--   0        0        0     1275 2023-07-21 14:29:40.665873 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/card.py
+-rw-r--r--   0        0        0     1589 2024-05-16 16:48:25.034139 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/checkbox.py
+-rw-r--r--   0        0        0     1814 2024-05-16 16:48:25.034139 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/circular_progress.py
+-rw-r--r--   0        0        0     3438 2024-05-16 16:48:25.034139 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/color_picker.py
+-rw-r--r--   0        0        0     1089 2024-05-16 16:48:25.034139 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/column.py
+-rw-r--r--   0        0        0     2539 2024-05-16 16:48:25.034139 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/date.py
+-rw-r--r--   0        0        0     2370 2024-02-23 16:33:09.312411 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/drawer.py
+-rw-r--r--   0        0        0    10045 2024-05-24 11:08:07.611703 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/echarts.py
+-rw-r--r--   0        0        0      412 2024-03-21 14:24:33.915934 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/element.py
+-rw-r--r--   0        0        0     1922 2024-05-16 16:48:25.034139 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/expansion.py
+-rw-r--r--   0        0        0      865 2024-02-23 16:33:09.312411 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/grid.py
+-rw-r--r--   0        0        0      119 2024-02-23 16:33:09.312411 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/html.js
+-rw-r--r--   0        0        0      675 2024-02-27 19:00:38.862516 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/html.py
+-rw-r--r--   0        0        0     1595 2024-05-16 16:48:25.034139 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/icon.py
+-rw-r--r--   0        0        0     1147 2024-05-16 16:48:25.034139 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/image.py
+-rw-r--r--   0        0        0     4066 2024-05-16 16:48:25.034139 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/input.py
+-rw-r--r--   0        0        0     2180 2024-05-16 16:48:25.034139 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/knob.py
+-rw-r--r--   0        0        0     1458 2024-05-19 18:23:49.816889 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/label.py
+-rw-r--r--   0        0        0     2164 2024-05-16 16:48:25.046835 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/linear_progress.py
+-rw-r--r--   0        0        0     2805 2024-05-24 11:08:07.612481 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/number.py
+-rw-r--r--   0        0        0     1965 2024-05-16 16:48:25.047878 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/radio.py
+-rw-r--r--   0        0        0     1029 2024-02-29 12:25:09.653951 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/row.py
+-rw-r--r--   0        0        0     3016 2024-05-16 16:48:25.047878 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/select.py
+-rw-r--r--   0        0        0     2981 2024-05-16 16:48:25.047878 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/slider.py
+-rw-r--r--   0        0        0     1632 2024-05-16 16:48:25.047878 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/switch.py
+-rw-r--r--   0        0        0     1796 2024-03-21 14:24:33.915934 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/tab.py
+-rw-r--r--   0        0        0      630 2024-03-21 14:24:33.920826 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/tab_panel.py
+-rw-r--r--   0        0        0     2103 2024-05-24 11:39:25.959154 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/tab_panels.py
+-rw-r--r--   0        0        0     6105 2024-05-16 16:48:25.047878 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/table.py
+-rw-r--r--   0        0        0     1281 2024-05-16 16:48:25.047878 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/tabs.py
+-rw-r--r--   0        0        0     3071 2024-05-16 16:48:25.047878 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/textarea.py
+-rw-r--r--   0        0        0     2360 2024-02-23 16:33:09.328748 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/upload.py
+-rw-r--r--   0        0        0      213 2024-02-21 13:27:29.151819 ex4nicegui-0.6.7/ex4nicegui/reactive/officials/utils.py
+-rw-r--r--   0        0        0     1554 2024-05-16 16:48:25.047878 ex4nicegui-0.6.7/ex4nicegui/reactive/q_pagination.py
+-rw-r--r--   0        0        0       31 2024-02-23 16:33:09.328748 ex4nicegui-0.6.7/ex4nicegui/reactive/rxui.py
+-rw-r--r--   0        0        0      898 2024-03-21 14:24:33.930894 ex4nicegui-0.6.7/ex4nicegui/reactive/transitionGroup.js
+-rw-r--r--   0        0        0      597 2024-03-21 14:24:33.930964 ex4nicegui-0.6.7/ex4nicegui/reactive/transitionGroup.py
+-rw-r--r--   0        0        0        0 2023-07-17 16:36:22.037136 ex4nicegui-0.6.7/ex4nicegui/reactive/UseDraggable/__init__.py
+-rw-r--r--   0        0        0     5473 2024-02-23 16:33:09.295358 ex4nicegui-0.6.7/ex4nicegui/reactive/UseDraggable/UseDraggable.js
+-rw-r--r--   0        0        0     3929 2024-02-23 16:33:09.295358 ex4nicegui-0.6.7/ex4nicegui/reactive/UseDraggable/UseDraggable.py
+-rw-r--r--   0        0        0        0 2023-07-08 17:55:18.326516 ex4nicegui-0.6.7/ex4nicegui/reactive/useMouse/__init__.py
+-rw-r--r--   0        0        0     2722 2023-07-17 15:14:14.622383 ex4nicegui-0.6.7/ex4nicegui/reactive/useMouse/UseMouse.js
+-rw-r--r--   0        0        0     2122 2024-02-23 16:33:09.360463 ex4nicegui-0.6.7/ex4nicegui/reactive/useMouse/UseMouse.py
+-rw-r--r--   0        0        0     2598 2024-03-07 10:39:11.607879 ex4nicegui-0.6.7/ex4nicegui/reactive/usePagination.py
+-rw-r--r--   0        0        0     4360 2024-03-07 20:18:40.954753 ex4nicegui-0.6.7/ex4nicegui/reactive/utils.py
+-rw-r--r--   0        0        0      282 2024-03-21 14:24:33.938595 ex4nicegui-0.6.7/ex4nicegui/reactive/vfor.js
+-rw-r--r--   0        0        0     5778 2024-04-26 16:54:25.065047 ex4nicegui-0.6.7/ex4nicegui/reactive/vfor.py
+-rw-r--r--   0        0        0     5091 2024-03-05 13:12:27.653865 ex4nicegui-0.6.7/ex4nicegui/reactive/vmodel.py
+-rw-r--r--   0        0        0        0 2024-02-27 19:00:38.862516 ex4nicegui-0.6.7/ex4nicegui/tools/__init__.py
+-rw-r--r--   0        0        0     4868 2024-02-27 19:00:38.862516 ex4nicegui-0.6.7/ex4nicegui/tools/debug.py
+-rw-r--r--   0        0        0        0 2023-07-05 06:10:00.104422 ex4nicegui-0.6.7/ex4nicegui/utils/__init__.py
+-rw-r--r--   0        0        0     2527 2024-02-27 19:00:38.877998 ex4nicegui-0.6.7/ex4nicegui/utils/apiEffect.py
+-rw-r--r--   0        0        0     1505 2024-03-05 13:06:09.437440 ex4nicegui-0.6.7/ex4nicegui/utils/asyncComputed.py
+-rw-r--r--   0        0        0     1719 2024-05-14 17:54:39.429168 ex4nicegui-0.6.7/ex4nicegui/utils/clientScope.py
+-rw-r--r--   0        0        0      994 2024-02-20 10:06:17.806243 ex4nicegui-0.6.7/ex4nicegui/utils/common.py
+-rw-r--r--   0        0        0     2310 2024-02-27 19:00:38.880863 ex4nicegui-0.6.7/ex4nicegui/utils/effect.py
+-rw-r--r--   0        0        0     1218 2024-02-27 19:00:38.880863 ex4nicegui-0.6.7/ex4nicegui/utils/scheduler.py
+-rw-r--r--   0        0        0    11346 2024-05-14 18:10:44.425976 ex4nicegui-0.6.7/ex4nicegui/utils/signals.py
+-rw-r--r--   0        0        0     1094 2023-06-30 08:17:10.111510 ex4nicegui-0.6.7/LICENSE
+-rw-r--r--   0        0        0      913 2024-05-24 11:41:56.171335 ex4nicegui-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0    28810 2024-05-24 11:39:25.954457 ex4nicegui-0.6.7/README.md
+-rw-r--r--   0        0        0    28517 1970-01-01 00:00:00.000000 ex4nicegui-0.6.7/PKG-INFO
```

### Comparing `ex4nicegui-0.6.6/LICENSE` & `ex4nicegui-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/PKG-INFO` & `ex4nicegui-0.6.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,73 @@
-Metadata-Version: 2.1
-Name: ex4nicegui
-Version: 0.6.6
-Summary: Extension library based on nicegui, providing data responsive,BI functionality modules
-Home-page: 
-Author: carson_jia
-Author-email: 568166495@qq.com
-License: MIT license
-Keywords: nicegui,ex4nicegui,webui
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ex4nicegui
-[中文 README](./README.md)
+[ENGLISH README](./README.en.md)
+
+
+- [教程](#教程)
+- [安装](#-安装)
+- [使用](#-使用)
+- [功能](#-功能)
+- [BI 模块](#bi-模块)
+
+对 [nicegui](https://github.com/zauberzeug/nicegui) 做的扩展库。内置响应式组件，完全实现数据响应式界面编程。
 
-- [Install](#-install)
-- [Usage](#-usage)
-- [Features](#-features)
-- [BI Module](#bi-module)
 
-An extension library for [nicegui](https://github.com/zauberzeug/nicegui). It has built-in responsive components and fully implements data-responsive interface programming.
+## 教程
+[头条文章-秒杀官方实现，python界面库，去掉90%事件代码的nicegui](https://www.toutiao.com/item/7253786340574265860/)
 
+[微信公众号-秒杀官方实现，python界面库，去掉90%事件代码的nicegui](https://mp.weixin.qq.com/s?__biz=MzUzNDk1MTc5Mw==&mid=2247486796&idx=1&sn=457ed6fb9d6a25145f7704d5197d670d&chksm=fa8daf52cdfa2644bede50ae7f2551162ecaedecafec231ee4ce8f28775a599f8669ecf06af1#rd)
 
-## 📦 Install
+
+## 📦 安装
 
 ```
 pip install ex4nicegui -U
 ```
 
-## examples
-- [basic](./examples/basic/)
+
+## 示例项目
+- [入门](./examples/basic/)
 - [todo list mvc](./examples/todomvc/)
 
+---
 
-## 🦄 Usage
+## 🦄 使用
 
 ```python
 from nicegui import ui
 from ex4nicegui import ref_computed, effect, to_ref
 from ex4nicegui.reactive import rxui
 
-# Define responsive data
+# 定义响应式数据
 r_input = to_ref("")
 
-# Pass in the responsive data according to the nicegui usage method.
+# 按照 nicegui 使用方式传入响应式数据即可
 rxui.input(value=r_input)
 rxui.label(r_input)
 
 ui.run()
 ```
 ![](./asset/sync_input.gif)
 
 
-## 🚀 Features
-
-### echarts components
+### 提供 echarts 图表组件
 
 ```python
 from nicegui import ui
 from ex4nicegui import ref_computed, effect, to_ref
 from ex4nicegui.reactive import rxui
 
 r_input = to_ref("")
 
-
-# ref_computed Creates a read-only reactive variable
-# Functions can use any other reactive variables automatically when they are associated
+# ref_computed 创建只读响应式变量
+# 函数中使用任意其他响应式变量，会自动关联
 @ref_computed
 def cp_echarts_opts():
     return {
-        "title": {"text": r_input.value}, #In the dictionary, use any reactive variable. Get the value by .value
+        "title": {"text": r_input.value}, #字典中使用任意响应式变量，通过 .value 获取值
         "xAxis": {
             "type": "category",
             "data": ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"],
         },
         "yAxis": {"type": "value"},
         "series": [
             {
@@ -85,33 +75,31 @@
                 "type": "bar",
                 "showBackground": True,
                 "backgroundStyle": {"color": "rgba(180, 180, 180, 0.2)"},
             }
         ],
     }
 
-
-input = rxui.input("Enter the content, and the chart title will be synchronized", value=r_input)
-
-# Get the native nicegui component object through the element attribute of the responsive component object
+input = rxui.input("输入内容，图表标题会同步", value=r_input)
+# 通过响应式组件对象的 element 属性，获取原生 nicegui 组件对象
 input.element.classes("w-full")
 
-rxui.echarts(cp_echarts_opts).classes('h-[20rem]')
+rxui.echarts(cp_echarts_opts)
 
 ui.run()
 ```
 ![](./asset/asyc_echarts_title.gif)
 
 
-### echarts mouse events
+### echarts 图表鼠标事件
 
-the `on` function parameters `event_name` and `query` to view the[echarts English Documentation](https://echarts.apache.org/handbook/en/concepts/event/)
+`on` 函数参数 `event_name` 以及 `query` 使用,查看[echarts 事件中文文档](https://echarts.apache.org/handbook/zh/concepts/event/)
 
 
-The following example binds the mouse click event
+以下例子绑定鼠标单击事件
 ```python
 from nicegui import ui
 from ex4nicegui.reactive import rxui
 
 opts = {
     "xAxis": {"type": "value", "boundaryGap": [0, 0.01]},
     "yAxis": {
@@ -133,19 +121,20 @@
 }
 
 bar = rxui.echarts(opts)
 
 def on_click(e: rxui.echarts.EChartsMouseEventArguments):
     ui.notify(f"on_click:{e.seriesName}:{e.name}:{e.value}")
 
+
 bar.on("click", on_click)
 ```
 
 
-The following example only triggers the mouseover event for a specified series.
+以下例子只针对指定系列触发鼠标划过事件
 ```python
 from nicegui import ui
 from ex4nicegui.reactive import rxui
 
 opts = {
     "xAxis": {"type": "value", "boundaryGap": [0, 0.01]},
     "yAxis": {
@@ -175,102 +164,105 @@
 bar.on("mouseover", on_first_series_mouseover, query={"seriesName": "first"})
 
 ui.run()
 ```
 ---
 
 
-## responsive
+## 响应式
 
 ```python
 from ex4nicegui import (
     to_ref,
     ref_computed,
     on,
     effect,
     effect_refreshable,
     batch,
     event_batch,
     deep_ref,
+    async_computed
 )
 ```
-Commonly used `to_ref`,`deep_ref`,`effect`,`ref_computed`,`on`
+常用 `to_ref`,`deep_ref`,`effect`,`ref_computed`,`on`,`async_computed`
+
+---
 
 ### `to_ref`
-Defines responsive objects, read and written by `.value`.
+定义响应式对象,通过 `.value` 读写
 ```python
 a = to_ref(1)
 b = to_ref("text")
 
 a.value =2
 b.value = 'new text'
 
 print(a.value)
 ```
 
-When the value is a complex object, responsiveness of nested objects is not maintained by default.
-
+当值为复杂对象时，默认不会保持嵌套对象的响应性。
 ```python
 a = to_ref([1,2])
 
 @effect
-def _().
-    print(len(a.value))
+def _():
+    print('len:',len(a.value))
 
-# doesn't trigger the effect
+# 不会触发 effect
 a.value.append(10)
 
-# the whole substitution will be triggered
+# 整个替换则会触发
 a.value = [1,2,10]
 ```
 
-Depth responsiveness is obtained when `is_deep` is set to `True`.
+参数 `is_deep` 设置为 `True` 时，能得到深度响应能力
 
 ```python
 a = to_ref([1,2],is_deep=True)
 
 @effect
 def _():
     print('len:',len(a.value))
 
 # print 3
 a.value.append(10)
 
 ```
 
-> `deep_ref` is equivalent to `to_ref` if `is_deep` is set to `True`.
+>  `deep_ref` 等价于 `is_deep` 设置为 `True` 时的 `to_ref`
+
 ---
 
 ### `deep_ref`
-Equivalent to `to_ref` when `is_deep` is set to `True`.
-
-Especially useful when the data source is a list, dictionary or custom class. Objects obtained via `.value` are proxies
+等价于 `is_deep` 设置为 `True` 时的 `to_ref`。
 
+当数据源为列表、字典或自定义类时，特别有用。通过 `.value` 获取的对象为代理对象
 ```python
 data = [1,2,3]
 data_ref = deep_ref(data)
 
 assert data_ref.value is not data
 ```
 
-You can get the raw object with `to_raw`.
+通过 `to_raw` 可以获取原始对象
 ```python
 from ex4nicegui import to_raw, deep_ref
 
 data = [1, 2, 3]
 data_ref = deep_ref(data)
 
 assert data_ref.value is not data
 assert to_raw(data_ref.value) is data
 ```
 
+
 ---
 
 ### `effect`
-Accepts a function and automatically monitors changes to the responsive objects used in the function to automatically execute the function.
+接受一个函数,自动监控函数中使用到的响应式对象变化,从而自动执行函数
 
 ```python
 a = to_ref(1)
 b = to_ref("text")
 
 
 @effect
@@ -282,22 +274,22 @@
     a.value = 2
     b.value = "new text"
 
 
 ui.button("change", on_click=change_value)
 ```
 
-The first time the effect is executed, the function `auto_run_when_ref_value` will be executed once. After that, clicking on the button changes the value of `a` (via `a.value`) and the function `auto_run_when_ref_value` is executed again.
+首次执行 effect ,函数`auto_run_when_ref_value`将被执行一次.之后点击按钮,改变 `a` 的值(通过 `a.value`),函数`auto_run_when_ref_value`再次执行
 
-> Never spread a lot of data processing logic across multiple `on`s or `effects`s, which should be mostly interface manipulation logic rather than responsive data processing logic
+> 切忌把大量数据处理逻辑分散在多个 `on` 或 `effect` 中，`on` 或 `effect` 中应该大部分为界面操作逻辑，而非响应式数据处理逻辑
 
 ---
 
 ### `ref_computed`
-As with `effect`, `ref_computed` can also return results from functions. Typically used for secondary computation from `to_ref`.
+与 `effect` 具备一样的功能，`ref_computed` 还能从函数中返回结果。一般用于从 `to_ref` 中进行二次计算
 
 ```python
 a = to_ref(1)
 a_square = ref_computed(lambda: a.value * 2)
 
 
 @effect
@@ -308,43 +300,43 @@
 def change_value():
     a.value = 2
 
 
 ui.button("change", on_click=change_value)
 ```
 
-When the button is clicked, the value of `a.value` is modified, triggering a recalculation of `a_square`. As the value of `a_square` is read in `effect1`, it triggers `effect1` to execute the
+点击按钮后，`a.value` 值被修改，从而触发 `a_square` 重新计算.由于 `effect1` 中读取了 `a_square` 的值，从而触发 `effect1` 执行
+
+> `ref_computed` 是只读的 `to_ref`
 
-> `ref_computed` is read-only `to_ref`
 
-If you prefer to organize your code by class, ``ref_computed`` also supports acting on instance methods
+如果你更喜欢通过类组织代码，`ref_computed` 同样支持作用到实例方法上
 
 ```python
-class MyState.
-    def __init__(self) -> None.
+class MyState:
+    def __init__(self) -> None:
         self.r_text = to_ref("")
 
     @ref_computed
-    def post_text(self): return self.r_text.value
+    def post_text(self):
         return self.r_text.value + "post"
 
 state = MyState()
 
 rxui.input(value=state.r_text)
 rxui.label(state.post_text)
 ```
 
 ---
 
 ### `async_computed`
-Use `async_computed` when asynchronous functions are required for computed.
-
+二次计算中需要使用异步函数时，使用 `async_computed`
 ```python
 
-# Simulate asynchronous functions that take a long time to execute
+# 模拟长时间执行的异步函数
 async def long_time_query(input: str):
     await asyncio.sleep(2)
     num = random.randint(20, 100)
     return f"query result[{input=}]:{num=}"
 
 
 search = to_ref("")
@@ -353,28 +345,29 @@
 @async_computed(search, evaluating=evaluating, init="")
 async def search_result():
     return await long_time_query(search.value)
 
 rxui.lazy_input(value=search)
 
 rxui.label(
-    lambda: "Query in progress" if evaluating.value else "Enter content in input box above and return to search"
+    lambda: "查询中" if evaluating.value else "上方输入框输入内容并回车搜索"
 )
 rxui.label(search_result)
 
 ```
 
-- The first argument to `async_computed` must explicitly specify the responsive data to be monitored. Multiple responses can be specified using a list.
-- Parameter `evaluating` is responsive data of type bool, which is `True` while the asynchronous function is executing, and `False` after the computation is finished.
-- Parameter `init` specifies the initial result
+- `async_computed` 第一个参数必须明确指定需要监控的响应式数据. 使用列表可以同时指定多个响应式数据
+- 参数 `evaluating` 为 bool 类型的响应式数据，当异步函数执行中，此变量值为 `True`，计算结束后为 `False`
+- 参数 `init` 指定初始结果
+
 
 ---
 
 ### `on`
-Similar to `effect`, but `on` needs to explicitly specify the responsive object to monitor.
+类似 `effect` 的功能,但是 `on` 需要明确指定监控的响应式对象
 
 ```python
 
 a1 = to_ref(1)
 a2 = to_ref(10)
 b = to_ref("text")
 
@@ -410,23 +403,24 @@
     ui.notify("change_b")
 
 
 ui.button("change b", on_click=change_b)
 
 ```
 
-- If the parameter `onchanges` is True (the default value is False), the specified function will not be executed at binding time.
+- 参数 `onchanges` 为 True 时(默认值为 False),指定的函数不会在绑定时执行 
+
 
-> Never spread a lot of data processing logic across multiple `on`s or `effects`s, which should be mostly interface manipulation logic rather than responsive data processing logic
+> 切忌把大量数据处理逻辑分散在多个 `on` 或 `effect` 中，`on` 或 `effect` 中应该大部分为界面操作逻辑，而非响应式数据处理逻辑
 
 ---
 
 ### `new_scope`
 
-By default, all watch functions are automatically destroyed when the client connection is disconnected. For finer-grained control, the `new_scope` function can be utilized.
+默认情况下，所有检测函数在客户端连接断开时自动销毁。如果需要更细粒度的控制，可以使用 `new_scope`
 
 ```python
 from nicegui import ui
 from ex4nicegui import rxui, to_ref, effect, new_scope
 
 a = to_ref(0.0)
 
@@ -441,57 +435,58 @@
 
 rxui.number(value=a)
 rxui.button("dispose scope 1", on_click=scope1.dispose)
 ```
 
 ---
 
-## functionality
+
+## 组件功能
 
 ### vmodel
-Create two-way bindings on form input elements or components.
+在表单输入元素或组件上创建双向绑定。
 
-Bidirectional bindings are supported by default for `ref` simple value types
+简单值类型的 `ref` 默认支持双向绑定
 ```python
 from ex4nicegui import rxui, to_ref, deep_ref
 
 data = to_ref("init")
 
 rxui.label(lambda: f"{data.value=}")
-# two-way binding 
+# 默认就是双向绑定
 rxui.input(value=data)
 ```
-- Simple value types are generally immutable values such as `str`, `int`, etc.
 
-When using complex data structures, `deep_ref` is used to keep nested values responsive.
+- 简单值类型一般是 `str`,`int` 等不可变值类型
+
+当使用复杂数据结构时，会使用 `deep_ref` 保持嵌套值的响应性
 ```python
 data = deep_ref({"a": 1, "b": [1, 2, 3, 4]})
 
 rxui.label(lambda: f"{data.value=!s}")
 
-# No binding effect
+# 当前版本没有任何绑定效果.或许未来的版本可以解决
 rxui.input(value=data.value["a"])
 
-# readonly binding
+# 只读绑定.其他途径修改了 `data.value["a"]` ，此输入框会同步，但反过来不行
 rxui.input(value=lambda: data.value["a"])
 
-# two-way binding
+# 要使用 vmodel 才能双向绑定
 rxui.input(value=rxui.vmodel(data.value["a"]))
 ```
 
-- The first input box will be completely unresponsive because the code is equivalent to passing in a value `1` directly
-- The second input box will get read responsiveness due to the use of a function.
-- The third input box, wrapped in `rxui.vmodel`, can be bi-directionally bound.
+- 第一个输入框将完全失去响应性，因为代码等价于直接传入一个数值`1`
+- 第二个输入框由于使用函数，将得到读取响应性(第三个输入框输入值，将得到同步)
+- 第三个输入框，使用 `rxui.vmodel` 包裹，即可实现双向绑定
 
-Most use `vmodel` with `vfor`, see [todo list examples](./examples/todomvc/)
+多数在配合 `vfor` 时使用 `vmodel`,可参考 [todo list 案例](./examples/todomvc/)
 
----
 
 ### vfor
-Render list components based on list responsive data. Each component is updated on demand. Data items support dictionaries or objects of any type
+基于列表响应式数据，渲染列表组件。每项组件按需更新。数据项支持字典或任意类型对象
 
 ```python
 from nicegui import ui
 from ex4nicegui.reactive import rxui
 from ex4nicegui import deep_ref, ref_computed
 from typing import Dict
 
@@ -517,83 +512,80 @@
 # ui
 rxui.label(done_count_info)
 ui.button("check", on_click=check)
 
 
 @rxui.vfor(items,key='id')
 def _(store: rxui.VforStore[Dict]):
-    # function to build the interface for each row of data
-    item = store.get()  # Get responsive object with `store.get`
-    mes = rxui.vmodel(item.value['message'])
+    # 函数中构建每一行数据的界面
+    item = store.get()  # 通过 store.get 获取对应行的响应式对象(相当于每行的数据 to_ref(...))
+    mes = rxui.vmodel(item.value['message']) # 复杂结构默认没有双向绑定，需要使用 `vmodel`
 
-    # Enter the content of the input box, 
-    # you can see the title of the radio box changes synchronously
+    # 输入框输入内容，可以看到单选框的标题同步变化
     with ui.card():
         with ui.row():
             rxui.input(value=mes)
             rxui.label(lambda: f"{mes.value=!s}")
         rxui.checkbox(text=mes, value=rxui.vmodel(item.value['done']))
 
 ```
 
-- `rxui.vfor` decorator to custom function
-    - The first argument is passed to the responsive list. Each item in the list can be a dictionary or other object (`dataclasses` etc.)
-    - Second parameter `key`: In order to be able to keep track of the identity of each node, and thus reuse and reorder existing elements, you can provide a unique key for the block corresponding to each element. The default(`None`) is to use the list element index.
-- The custom function takes one argument. The current row's  can be retrieved via `store.get`, which is a responsive object.
-
+- `rxui.vfor` 装饰器到自定义函数
+    - 第一个参数传入响应式列表。列表中每一项可以是字典或其他对象(`dataclasses` 等等)
+    - 第二个参数 `key`: 为了可以跟踪每个节点的标识，从而重用和重新排序现有的元素，你可以为每个元素对应的块提供一个唯一的 key 。默认情况使用列表元素索引。
+- 自定义函数带有一个参数。通过 `store.get` 可以获取当前行的响应式对象
 
-> vfor are created only when new data is added.
+> vfor 渲染的项目，只有在新增数据时，才会创建
 
 
 ---
 
+### 绑定类名
 
-### Bind class names
+所有的组件类提供 `bind_classes` 用于绑定 `class`，支持三种不同的数据结构。
 
-All component classes provide `bind_classes` for binding `class`, supporting three different data structures.
-
-Bind dictionaries
+绑定字典
 
 ```python
 bg_color = to_ref(False)
 has_error = to_ref(False)
 
 rxui.label("test").bind_classes({"bg-blue": bg_color, "text-red": has_error})
 
 rxui.switch("bg_color", value=bg_color)
 rxui.switch("has_error", value=has_error)
 ```
 
-Dictionary key  is the class name, and a dictionary value of  a responsive variable with value `bool`. When the responsive value is `True`, the class name is applied to the component `class`.
+字典键值为类名,对应值为 bool 的响应式变量。当响应式值为 `True`，类名应用到组件 class
+
 
 ---
 
-Bind a responsive variable whose return value is a dictionary.
+绑定返回值为字典的响应式变量
 
 ```python
 bg_color = to_ref(False)
 has_error = to_ref(False)
 
 class_obj = ref_computed(
     lambda: {"bg-blue": bg_color.value, "text-red": has_error.value}
 )
 
 rxui.switch("bg_color", value=bg_color)
 rxui.switch("has_error", value=has_error)
 rxui.label("bind to ref_computed").bind_classes(class_obj)
-
 # or direct function passing
 rxui.label("bind to ref_computed").bind_classes(
     lambda: {"bg-blue": bg_color.value, "text-red": has_error.value}
 )
 ```
 
 ---
 
-Bind to list
+绑定为列表
 
 ```python
 bg_color = to_ref("red")
 bg_color_class = ref_computed(lambda: f"bg-{bg_color.value}")
 
 text_color = to_ref("green")
 text_color_class = ref_computed(lambda: f"text-{text_color.value}")
@@ -601,15 +593,15 @@
 rxui.select(["red", "green", "yellow"], label="bg color", value=bg_color)
 rxui.select(["red", "green", "yellow"], label="text color", value=text_color)
 
 rxui.label("binding to arrays").bind_classes([bg_color_class, text_color_class])
 
 ```
 
-Each element in the list is a responsive variable that returns the class name
+列表中每个元素为返回类名的响应式变量
 
 ---
 
 ### bind-style
 
 ```python
 from nicegui import ui
@@ -627,25 +619,45 @@
     }
 )
 
 rxui.select(["blue", "green", "yellow"], label="bg color", value=bg_color)
 rxui.select(["red", "green", "yellow"], label="text color", value=text_color)
 ```
 
-`bind_style` passed into dictionary, `key` is style name, `value` is style value, responsive string
+`bind_style` 传入字典，`key` 为样式名字，`value` 为样式值，响应式字符串
+
+---
+
+### bind_prop
+
+绑定单个属性
+
+```python
+
+label = to_ref("hello")
+
+rxui.button("").bind_prop("label", label)
+# 允许使用函数
+rxui.button("").bind_prop(
+    "label", lambda: f"{label.value} world"
+)
+
+rxui.input(value=label)
+```
+
 
 ---
 
 ### rxui.echarts
-Charting with echarts
+使用 echarts 制作图表
 
 ---
 
 #### rxui.echarts.from_javascript
-Create echart from javascript code
+从 javascript 代码创建 echart
 
 ```python
 from pathlib import Path
 
 rxui.echarts.from_javascript(Path("code.js"))
 # or
 rxui.echarts.from_javascript(
@@ -670,119 +682,199 @@
 
     myChart.setOption(option);
 }
 """
 )
 ```
 
-- The first parameter of the function is the echart instance object. You need to configure the chart in the function with `setOption`.
+- 函数第一个参数为 echart 实例对象.你需要在函数中通过 `setOption` 完成图表配置
+
+函数也有第二个参数，为 `echarts` 全局对象，你可以通过 `echarts.registerMap` 注册地图。
+
+```python
+rxui.echarts.from_javascript(
+"""
+(chart,echarts) =>{
+
+    fetch('https://geo.datav.aliyun.com/areas_v3/bound/100000_full.json')
+    .then(response => response.json())
+    .then(data => {
+            echarts.registerMap('test_map', data);
+
+            chart.setOption({
+                geo: {
+                    map: 'test_map',
+                    roam: true,
+                },
+                tooltip: {},
+                legend: {},
+                series: [],
+            });
+    });
+}
+"""
+)
+```
 
 ---
 
 #### rxui.echarts.register_map
-Register a map.
+注册地图.
 
 ```python
 rxui.echarts.register_map(
     "china", "https://geo.datav.aliyun.com/areas_v3/bound/100000_full.json"
 )
 
 rxui.echarts(
     {
         "geo": {
             "map": "china",
             "roam": True,
         },
         "tooltip": {},
         "legend": {},
-        "series": [], }
+        "series": [],
     }
 )
 ```
 
-- The parameter `map_name` is a customized map name. Note that `map` must correspond to a registered name in the chart configuration.
-- The parameter `src` is a valid network link to the map data.
+- 参数 `map_name` 为自定义的地图名字。注意在图表配置中 `map` 必需对应注册的名字
+- 参数 `src` 为有效的地图数据网络链接。
+
 
-You can also provide the path to the local json file for the map data.
+如果是 svg 数据，需要设置参数 `type="svg"`
+```python
+rxui.echarts.register_map("svg-rect", "/test/svg", type="svg")
+```
+
+
+
+你也可以直接提供本地地图数据的json文件路径对象(Path)
 ```python
 from pathlib import Path
 
 rxui.echarts.register_map(
     "china", Path("map-data.json")
 )
 ```
 
 ---
 
 ### gsap
-
-js animation library. [gsap documentation](https://gsap.com/docs/v3/)
+js 动画库. [gsap文档](https://gsap.com/docs/v3/)
 
 ```python
 from nicegui import ui
 from ex4nicegui import gsap
 ```
 
 #### gsap.from_
 
-Set the start property, the animation will transition from the set property to the original position
+设置起始属性，动画将从设置的属性过渡到原始位置
 
 ```python
 
 ui.label("test from").classes("target")
 gsap.from_(".target", {"x": 50,'duration':1})
 
 ```
 
-After the screen is loaded, the starting position of the text is shifted to the right by 50px, and then moved to the original position within 1 second.
+画面加载后，文本起始位置在往右偏移 50px 处，在 1秒 内移动到原始位置上
 
-- Arguments `targets` are css selectors.
-- Arguments `vars` are attribute values
+- 参数 `targets` 为 css 选择器
+- 参数 `vars` 为属性值，具体参考 gsap 文档
 
 ---
 
 #### gsap.to
 
-Set the end property, the animation will transition from the original property to the set property.
+设置结束属性，动画将从原始属性过渡到设置的属性
 
 ```python
 
 ui.label("test to").classes("target")
 gsap.to(".target", {"x": 50,'duration':1})
 
 ```
 
-After loading the screen, the text will be moved back 50px from the original position within 1 second.
+画面加载后，文本在 1秒 内，从原始位置往后移动 50px
 
-- Arguments `targets` are css selectors.
-- Arguments `vars` are attribute values
+- 参数 `targets` 为 css 选择器
+- 参数 `vars` 为属性值，具体参考 gsap 文档
 
 ---
-
 #### gsap.run_script
 
-Setting up animations by writing js
+通过编写 js 设置动画
 
 ```python
 
 gsap.run_script(
             r"""function setGsap(gsap) {
     gsap.to('.target',{"duration": 0.3,y:60})
 }
 """)
 ```
 
-- The parameter `script` can be text or a file with a js extension `Path`.
-- The name of the defined js function doesn't matter, the first argument is a gsap object.
+- 参数 `script` 可以为文本或 js 后缀的文件 `Path`
+- 定义的 js 函数名字并不影响运行，第一个参数为 gsap 对象
 
 ---
 
-## BI Module
+### tab_panels
+
+相比较于 `nicegui.ui.tab_panels` , `rxui.tab_panels` 没有参数 `tabs`。在数据响应式机制下，`tabs` 与 `tab_panels` 联动只需要通过参数 `value` 即可。
+
+```python
+from nicegui import ui
+from ex4nicegui import rxui, to_ref
+
+names = ["Tab 1", "Tab 2", "Tab 3"]
+current_tab = to_ref(names[0])
+
+with rxui.tabs(current_tab):
+    for name in names:
+        rxui.tab(name)
+
+with rxui.tab_panels(current_tab):
+    for name in names:
+        with rxui.tab_panel(name):
+            ui.label(f"Content of {name}")
+```
+
+这是因为，数据响应机制下，组件联动是通过中间数据层(`to_ref`)实现的。因此，`tab_panels` 可以与其他组件联动(只需要保证使用同样的 `ref` 对象即可)
+
+```python
+names = ["Tab 1", "Tab 2", "Tab 3"]
+current_tab = to_ref(names[0])
+
 
-Create an interactive data visualization report using the minimal API.
+with rxui.tab_panels(current_tab):
+    for name in names:
+        with rxui.tab_panel(name):
+            ui.label(f"Content of {name}")
+
+# tabs 不必在 panels 前面
+with rxui.tabs(current_tab):
+    for name in names:
+        rxui.tab(name)
+
+rxui.select(names, value=current_tab)
+rxui.radio(names, value=current_tab).props("inline")
+
+rxui.label(lambda: f"当前 tab 为:{current_tab.value}")
+```
+
+
+---
+
+## BI 模块
+
+以最精简的 apis 创建可交互的数据可视化报表
 
 ![](./asset/bi_examples1.gif)
 
 ```python
 from nicegui import ui
 import pandas as pd
 import numpy as np
@@ -804,28 +896,28 @@
     )
     df[["idc1", "idc2"]] = np.random.randint(50, 1000, size=(len(df), 2))
     return df
 
 
 df = gen_data()
 
-# Create a data source.
+# 创建数据源
 ds = bi.data_source(df)
 
 # ui
 ui.query(".nicegui-content").classes("items-stretch no-wrap")
 
 with ui.row().classes("justify-evenly"):
-    # Create components based on the data source `ds`.
+    # 基于数据源 `ds` 创建界面组件
     ds.ui_select("cat").classes("min-w-[10rem]")
     ds.ui_select("name").classes("min-w-[10rem]")
 
 
 with ui.grid(columns=2):
-    # Configure the chart using a dictionary.
+    # 使用字典配置图表
     @ds.ui_echarts
     def bar1(data: pd.DataFrame):
         data = data.groupby("name").agg({"idc1": "sum", "idc2": "sum"}).reset_index()
 
         return {
             "xAxis": {"type": "value"},
             "yAxis": {
@@ -838,56 +930,56 @@
                 {"type": "bar", "name": "idc1", "data": data["idc1"].tolist()},
                 {"type": "bar", "name": "idc2", "data": data["idc2"].tolist()},
             ],
         }
 
     bar1.classes("h-[20rem]")
 
-    # Configure the chart using pyecharts.
+    # 使用pyecharts配置图表
     @ds.ui_echarts
     def bar2(data: pd.DataFrame):
         data = data.groupby("name").agg({"idc1": "sum", "idc2": "sum"}).reset_index()
 
         return (
             Bar()
             .add_xaxis(data["name"].tolist())
             .add_yaxis("idc1", data["idc1"].tolist())
             .add_yaxis("idc2", data["idc2"].tolist())
         )
 
     bar2.classes("h-[20rem]")
 
-    # Bind the click event to achieve navigation.
+    # 绑定点击事件，即可实现跳转
     @bar2.on_chart_click
     def _(e: rxui.echarts.EChartsMouseEventArguments):
         ui.open(f"/details/{e.name}", new_tab=True)
 
 
-# with response mechanisms, you can freely combine native nicegui components.
+# 利用响应式机制，你可以随意组合原生 nicegui 组件
 label_a1_total = ui.label("")
 
 
-# this function will be triggered when ds changed.
+# 当 ds 有变化，都会触发此函数
 @effect
 def _():
-    # prop `filtered_data` is the filtered DataFrame.
+    # filtered_data 为过滤后的 DataFrame
     df = ds.filtered_data
     total = df[df["cat"] == "a1"]["idc1"].sum()
     label_a1_total.text = f"idc1 total(cat==a1):{total}"
 
 
-# you can also use `effect_refreshable`, but you need to note that the components in the function are rebuilt each time.
+# 你也可以使用 `effect_refreshable`,但需要注意函数中的组件每次都被重建
 @effect_refreshable
 def _():
     df = ds.filtered_data
     total = df[df["cat"] == "a2"]["idc1"].sum()
     ui.label(f"idc1 total(cat==a2):{total}")
 
 
-# the page to be navigated when clicking on the chart series.
+# 当点击图表系列时，跳转的页面
 @ui.page("/details/{name}")
 def details_page(name: str):
     ui.label("This table data will not change")
     ui.aggrid.from_pandas(ds.data.query(f'name=="{name}"'))
 
     ui.label("This table will change when the homepage data changes. ")
 
@@ -897,20 +989,25 @@
 
     new_ds.ui_aggrid()
 
 
 ui.run()
 ```
 
-### Details
+
+
+### 细节
+
+
+
 
 #### `bi.data_source`
-The data source is the core concept of the BI module, and all data linkage is based on this. In the current version (0.4.3), there are two ways to create a data source.
+数据源是 BI 模块的核心概念，所有数据的联动基于此展开。当前版本(0.4.3)中，有两种创建数据源的方式
 
-Receive `pandas`'s `DataFrame`:
+接收 `pandas` 的 `DataFrame`:
 ```python
 from nicegui import ui
 from ex4nicegui import bi
 import pandas as pd
 
 df = pd.DataFrame(
     {
@@ -919,15 +1016,16 @@
         "value": range(6),
     }
 )
 
 ds =  bi.data_source(df)
 ```
 
-Sometimes, we want to create a new data source based on another data source, in which case we can use a decorator to create a linked data source:
+---
+有时候，我们希望基于另一个数据源创建新的数据源，此时可以使用装饰器创建联动数据源:
 ```python
 df = pd.DataFrame(
     {
         "name": list("aabcdf"),
         "cls": ["c1", "c2", "c1", "c1", "c3", None],
         "value": range(6),
     }
@@ -941,35 +1039,35 @@
     df = ds.filtered_data
     df=df.copy()
     df['value'] = df['value'] * 100
     return df
 
 ds.ui_select('name')
 new_ds.ui_aggrid()
+
 ```
 
-Note that since `new_ds` uses `ds.filtered_data`, changes to `ds` will trigger the linkage change of `new_ds`, causing the table component created by `new_ds` to change.
+注意，由于 `new_ds` 中使用了 `ds.filtered_data` ，因此 `ds` 的变动会触发 `new_ds` 的联动变化，从而导致 `new_ds` 创建的表格组件产生变化
 
 ---
-
-Remove all filter states through the `ds.remove_filters` method:
+通过 `ds.remove_filters` 方法，移除所有筛选状态:
 ```python
 ds = bi.data_source(df)
 
 def on_remove_filters():
     ds.remove_filters()
 
 ui.button("remove all filters", on_click=on_remove_filters)
 
 ds.ui_select("name")
 ds.ui_aggrid()
 ```
 ---
 
-Reset the data source through the `ds.reload` method:
+通过 `ds.reload` 方法，重设数据源:
 ```python
 
 df = pd.DataFrame(
     {
         "name": list("aabcdf"),
         "cls": ["c1", "c2", "c1", "c1", "c3", None],
         "value": range(6),
@@ -994,16 +1092,14 @@
 ds.ui_select("name")
 ds.ui_aggrid()
 ```
 
 ---
 #### ui_select
 
-Dropdown Select Box
-
 ```python
 from nicegui import ui
 from ex4nicegui import bi
 import pandas as pd
 
 df = pd.DataFrame(
     {
@@ -1014,51 +1110,56 @@
 )
 
 ds = bi.data_source(df)
 
 ds.ui_select("name")
 ```
 
-The first parameter column specifies the column name of the data source.
+第一个参数 column 指定数据源的列名
 
 ---
-Set the order of options using the parameter `sort_options`:
+通过参数 `sort_options` 设置选项顺序:
 ```python
 ds.ui_select("name", sort_options={"value": "desc", "name": "asc"})
+
 ```
 
 ---
-Set whether to exclude null values using the parameter `exclude_null_value`:
+参数 `exclude_null_value` 设置是否排除空值:
 ```python
 df = pd.DataFrame(
     {
         "cls": ["c1", "c2", "c1", "c1", "c3", None],
     }
 )
 
 ds = bi.data_source(df)
 ds.ui_select("cls", exclude_null_value=True)
 ```
 
 ---
-You can set the parameters of the native nicegui select component through keyword arguments.
 
-Set default values through the value attribute:
+你可以通过关键字参数，设置原生 nicegui select 组件的参数.
+
+通过 value 属性，设置默认值:
 ```python
 ds.ui_select("cls",value=['c1','c2'])
 ds.ui_select("cls",multiple=False,value='c1')
+
 ```
-For multiple selections (the parameter `multiple` is defaulted to True), `value` needs to be specified as a list. For single selections, `value` should be set to non-list.
 
----
+多选时(参数 `multiple` 默认为 True)，`value` 需要指定为 list
+
+单选时，`value` 设置为非 list
 
+---
 
 #### ui_table
 
-Table
+表格
 
 ```python
 from nicegui import ui
 from ex4nicegui import bi
 import pandas as pd
 
 data = pd.DataFrame({"name": ["f", "a", "c", "b"], "age": [1, 2, 3, 1]})
@@ -1068,16 +1169,16 @@
     columns=[
         {"label": "new colA", "field": "colA", "sortable": True},
     ]
 )
 
 ```
 
-- The parameter `columns` are consistent with nicegui `ui.table`. The key value `field` corresponds to the column name of the data source, and if it does not exist, this configuration will not take effect
-- The `rows` parameter will not take effect. Because the data source of the table is always controlled by the data source.
+- columns 与 nicegui `ui.table` 一致。其中 键值 `field` 对应数据源的列名，如果不存在，则该配置不会生效
+- rows 参数不会生效。因为表格的数据源始终由 data source 控制
 
 ---
 
 #### ui_aggrid
 
 
 ```python
@@ -1110,11 +1211,11 @@
             },
         ],
         "rowData": [{"colX": [1, 2, 3, 4, 5]}],
     }
 )
 ```
 
-- The parameter `options` is consistent with nicegui `ui.aggrid`. The key value `field` in columnDefs corresponds to the column name of the data source, and if it does not exist, this configuration will not take effect.
-- The `rowData` key value will not take effect. Because the data source of the table is always controlled by the data source.
+- 参数 options 与 nicegui `ui.aggrid` 一致。其中 `columnDefs` 中的键值 `field` 对应数据源的列名，如果不存在，则该配置不会生效
+- `rowData` 键值不会生效。因为表格的数据源始终由 data source 控制
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/__init__.py` & `ex4nicegui-0.6.7/ex4nicegui/__init__.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/bi/dataSource.py` & `ex4nicegui-0.6.7/ex4nicegui/bi/dataSource.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/bi/dataSourceFacade.py` & `ex4nicegui-0.6.7/ex4nicegui/bi/dataSourceFacade.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/bi/elements/layouts.py` & `ex4nicegui-0.6.7/ex4nicegui/bi/elements/layouts.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/bi/elements/models.py` & `ex4nicegui-0.6.7/ex4nicegui/bi/elements/models.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/bi/elements/text.py` & `ex4nicegui-0.6.7/ex4nicegui/bi/elements/text.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_aggrid.py` & `ex4nicegui-0.6.7/ex4nicegui/bi/elements/ui_aggrid.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_date_picker.js` & `ex4nicegui-0.6.7/ex4nicegui/bi/elements/ui_date_picker.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_date_picker.py` & `ex4nicegui-0.6.7/ex4nicegui/bi/elements/ui_date_picker.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_echarts.py` & `ex4nicegui-0.6.7/ex4nicegui/bi/elements/ui_echarts.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_radio.py` & `ex4nicegui-0.6.7/ex4nicegui/bi/elements/ui_radio.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_range.py` & `ex4nicegui-0.6.7/ex4nicegui/bi/elements/ui_range.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_select.py` & `ex4nicegui-0.6.7/ex4nicegui/bi/elements/ui_select.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_slider.py` & `ex4nicegui-0.6.7/ex4nicegui/bi/elements/ui_slider.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/bi/elements/ui_table.py` & `ex4nicegui-0.6.7/ex4nicegui/bi/elements/ui_table.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/bi/index.py` & `ex4nicegui-0.6.7/ex4nicegui/bi/index.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/bi/protocols.py` & `ex4nicegui-0.6.7/ex4nicegui/bi/protocols.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/experimental_/gridLayout/index.py` & `ex4nicegui-0.6.7/ex4nicegui/experimental_/gridLayout/index.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/gsap/gsap.py` & `ex4nicegui-0.6.7/ex4nicegui/gsap/gsap.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/gsap/timeline.js` & `ex4nicegui-0.6.7/ex4nicegui/gsap/timeline.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/gsap/timeline.py` & `ex4nicegui-0.6.7/ex4nicegui/gsap/timeline.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/gsap/wrapGsap.js` & `ex4nicegui-0.6.7/ex4nicegui/gsap/wrapGsap.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/layout/gridFlex/GridFlex.js` & `ex4nicegui-0.6.7/ex4nicegui/layout/gridFlex/GridFlex.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/layout/gridFlex/gridFlex.py` & `ex4nicegui-0.6.7/ex4nicegui/layout/gridFlex/gridFlex.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/layout/gridFlex/utils.py` & `ex4nicegui-0.6.7/ex4nicegui/layout/gridFlex/utils.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/layout/rxFlex/index.py` & `ex4nicegui-0.6.7/ex4nicegui/layout/rxFlex/index.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/layout/rxFlex/types.py` & `ex4nicegui-0.6.7/ex4nicegui/layout/rxFlex/types.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-color.ems.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/d3/d3-color.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-dispatch.ems.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/d3/d3-dispatch.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-drag.ems.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/d3/d3-drag.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-ease.ems.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/d3/d3-ease.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-interpolate.ems.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/d3/d3-interpolate.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-selection.ems.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/d3/d3-selection.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-timer.ems.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/d3/d3-timer.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-transition.ems.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/d3/d3-transition.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/d3/d3-zoom.ems.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/d3/d3-zoom.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/CSSPlugin.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/gsap/CSSPlugin.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/CSSRulePlugin.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/gsap/CSSRulePlugin.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/CustomEase.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/gsap/CustomEase.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/Draggable.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/gsap/Draggable.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/EasePack.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/gsap/EasePack.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/EaselPlugin.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/gsap/EaselPlugin.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/Flip.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/gsap/Flip.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/MotionPathPlugin.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/gsap/MotionPathPlugin.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/Observer.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/gsap/Observer.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/PixiPlugin.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/gsap/PixiPlugin.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/ScrollToPlugin.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/gsap/ScrollToPlugin.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/ScrollTrigger.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/gsap/ScrollTrigger.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/TextPlugin.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/gsap/TextPlugin.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/all.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/gsap/all.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/gsap-core.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/gsap/gsap-core.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/utils/matrix.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/gsap/utils/matrix.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/utils/paths.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/gsap/utils/paths.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/libs/gsap/utils/strings.js` & `ex4nicegui-0.6.7/ex4nicegui/libs/gsap/utils/strings.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/EChartsComponent/ECharts.js` & `ex4nicegui-0.6.7/ex4nicegui/reactive/EChartsComponent/ECharts.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -3,21 +3,37 @@
 } from "../../static/utils/dynamic_properties.js";
 
 function collectMapRegisterTask() {
     const tasks = new Map();
 
     if (typeof window.ex4ngEchartsMapTasks !== "undefined") {
 
-        for (const [mapName, src] of window.ex4ngEchartsMapTasks.entries()) {
-
+        for (const [mapName, opt] of window.ex4ngEchartsMapTasks.entries()) {
+            const {
+                src,
+                type: mapDataType,
+                specialAreas
+            } = opt;
             const registerPromise = new Promise((resolve, reject) => {
                 fetch(src)
-                    .then((response) => response.json())
+                    .then((response) => {
+                        if (mapDataType === "genJSON") {
+                            return response.json();
+                        }
+
+                        return response.text();
+                    })
                     .then((data) => {
-                        echarts.registerMap(mapName, data);
+                        if (mapDataType === "svg") {
+                            data = {
+                                svg: data
+                            }
+                        }
+
+                        echarts.registerMap(mapName, data, specialAreas);
                         resolve();
                     });
 
             });
 
             tasks.set(mapName, registerPromise);
         }
@@ -44,35 +60,35 @@
 const mapRegisterTasks = collectMapRegisterTask();
 
 export default {
     template: "<div></div>",
     async mounted() {
         await this.$nextTick(); // wait for Tailwind classes to be applied
 
-        if (hasMapOrGeo(this.options)) {
-            await Promise.all(Array.from(mapRegisterTasks.values()));
-        }
-
         this.chart = echarts.init(this.$el, this.theme);
 
         this.resizeObs = new ResizeObserver(this.chart.resize)
 
         // Prevent interruption of chart animations due to resize operations.
         // It is recommended to register the callbacks for such an event before setOption.
         const createResizeObserver = () => {
             this.resizeObs.observe(this.$el);
             this.chart.off("finished", createResizeObserver);
         };
         this.chart.on("finished", createResizeObserver);
 
         if (this.options) {
+            if (hasMapOrGeo(this.options)) {
+                await Promise.all(Array.from(mapRegisterTasks.values()));
+            }
             this.update_chart();
         } else {
             const fn = new Function('return ' + this.code)()
-            fn(this.chart)
+            await Promise.all(Array.from(mapRegisterTasks.values()));
+            fn(this.chart, echarts)
             this.$emit("__update_options_from_client", this.chart.getOption())
         }
         this.chart.getZr().on("click", (e) => {
             if (!e.target) {
                 this.$emit("clickBlank")
             }
         });
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/EChartsComponent/ECharts.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/EChartsComponent/ECharts.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/EChartsComponent/events.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/EChartsComponent/events.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/EChartsComponent/types.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/EChartsComponent/types.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/EChartsComponent/utils.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/EChartsComponent/utils.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/UseDraggable/UseDraggable.js` & `ex4nicegui-0.6.7/ex4nicegui/reactive/UseDraggable/UseDraggable.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/UseDraggable/UseDraggable.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/UseDraggable/UseDraggable.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/__init__.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/__init__.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/deferredTask.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/deferredTask.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/dropZone/dropZone.js` & `ex4nicegui-0.6.7/ex4nicegui/reactive/dropZone/dropZone.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/dropZone/dropZone.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/dropZone/dropZone.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/fileWatcher.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/fileWatcher.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/local_file_picker.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/local_file_picker.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/mermaid/mermaid.js` & `ex4nicegui-0.6.7/ex4nicegui/reactive/mermaid/mermaid.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/mermaid/mermaid.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/mermaid/mermaid.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/aggrid.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/aggrid.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
     Any,
     Callable,
     List,
     Dict,
     Optional,
 )
 from ex4nicegui.utils.signals import (
-    ReadonlyRef,
     is_ref,
     ref_computed,
     to_value,
     _TMaybeRef as TMaybeRef,
+    TGetterOrReadonlyRef,
 )
 from ex4nicegui.utils.apiEffect import ui_effect
 from nicegui import ui
 from .base import BindableUi
 from ex4nicegui.reactive.utils import ParameterClassifier, dataframe2col_str
 
 
@@ -74,21 +74,21 @@
         columnDefs = AggridBindableUi._get_columnDefs_from_dataframe(
             copy_df, columns_define_fn
         )
         rowData = copy_df.to_dict("records")  # type: ignore
         options = {"columnDefs": columnDefs, "rowData": rowData}
         return cls(options, **org_kws)
 
-    def bind_prop(self, prop: str, ref_ui: ReadonlyRef[Any]):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef[Any]):
         if prop == "options":
             return self.bind_options(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_options(self, ref_ui: ReadonlyRef[List[Dict]]):
+    def bind_options(self, ref_ui: TGetterOrReadonlyRef[List[Dict]]):
         @ui_effect
         def _():
             ele = self.element
             data = to_value(ref_ui)
             ele._props["options"].update(data)
             ele.update()
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/base.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,24 @@
         """Remove a child element.
 
         :param element: either the element instance or its ID
         """
         return self.element.remove(element)
 
     def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef[Any]):
+        """data binding is manipulating an element's property
+
+        @see - https://github.com/CrystalWindSnake/ex4nicegui/blob/main/README.en.md#bind_prop
+        @中文文档 - https://gitee.com/carson_add/ex4nicegui/tree/main/#bind_prop
+
+        Args:
+            prop (str): property name
+            ref_ui (TGetterOrReadonlyRef[Any]): a reference to the value to bind to
+
+        """
         if prop == "visible":
             return self.bind_visible(ref_ui)
 
         if prop == "text" and isinstance(self.element, TextElement):
 
             @self._ui_effect
             def _():
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/button.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/button.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import (
     Any,
     Callable,
     Optional,
 )
 from ex4nicegui.reactive.utils import ParameterClassifier
 from ex4nicegui.utils.signals import (
-    ReadonlyRef,
+    TGetterOrReadonlyRef,
     _TMaybeRef as TMaybeRef,
     to_value,
 )
 from nicegui import ui
 from .base import BindableUi, DisableableMixin
 
 
@@ -29,32 +29,32 @@
         element = ui.button(**pc.get_values_kws())
 
         super().__init__(element)
 
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
-    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "text":
             return self.bind_text(ref_ui)
         if prop == "icon":
             return self.bind_icon(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_text(self, ref_ui: ReadonlyRef):
+    def bind_text(self, ref_ui: TGetterOrReadonlyRef):
         @self._ui_effect
         def _():
             ele = self.element
             ele._props["label"] = to_value(ref_ui)
             ele.update()
 
         return self
 
-    def bind_icon(self, ref_ui: ReadonlyRef):
+    def bind_icon(self, ref_ui: TGetterOrReadonlyRef[str]):
         @self._ui_effect
         def _():
             ele = self.element
             ele._props["icon"] = to_value(ref_ui)
             ele.update()
 
         return self
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/card.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/card.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/checkbox.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/checkbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     Callable,
     Optional,
     TypeVar,
 )
 from ex4nicegui.reactive.utils import ParameterClassifier
 from ex4nicegui.utils.apiEffect import ui_effect
 from ex4nicegui.utils.signals import (
-    ReadonlyRef,
+    TGetterOrReadonlyRef,
     _TMaybeRef as TMaybeRef,
     to_value,
 )
 from nicegui import ui
 from .base import BindableUi, DisableableMixin
 
 T = TypeVar("T")
@@ -40,20 +40,20 @@
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
     @property
     def value(self):
         return self.element.value
 
-    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "value":
             return self.bind_value(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_value(self, ref_ui: ReadonlyRef[bool]):
+    def bind_value(self, ref_ui: TGetterOrReadonlyRef[bool]):
         @ui_effect
         def _():
             self.element.set_value(to_value(ref_ui))
             self.element.update()
 
         return self
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/circular_progress.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/circular_progress.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import (
     Optional,
 )
 from ex4nicegui.reactive.utils import ParameterClassifier
 from ex4nicegui.utils.apiEffect import ui_effect
 
 from ex4nicegui.utils.signals import (
-    ReadonlyRef,
+    TGetterOrReadonlyRef,
     _TMaybeRef as TMaybeRef,
     to_value,
 )
 from nicegui import ui
 from .base import BindableUi, DisableableMixin
 
 
@@ -46,19 +46,19 @@
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
     @property
     def value(self):
         return self.element.value
 
-    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "value":
             return self.bind_value(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_value(self, ref_ui: ReadonlyRef[float]):
+    def bind_value(self, ref_ui: TGetterOrReadonlyRef[float]):
         @ui_effect
         def _():
             self.element.set_value(to_value(ref_ui))
 
         return self
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/color_picker.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/color_picker.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     Optional,
     cast,
 )
 from ex4nicegui.reactive.utils import ParameterClassifier
 from ex4nicegui.utils.apiEffect import ui_effect
 
 from ex4nicegui.utils.signals import (
-    ReadonlyRef,
+    TGetterOrReadonlyRef,
     Ref,
     _TMaybeRef as TMaybeRef,
     is_setter_ref,
     to_value,
 )
 from nicegui import ui
 from nicegui.events import handle_event
@@ -65,28 +65,28 @@
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
     @property
     def value(self):
         return self.element.value
 
-    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "value":
             return self.bind_value(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_color(self, ref_ui: ReadonlyRef[str]):
+    def bind_color(self, ref_ui: TGetterOrReadonlyRef[str]):
         @ui_effect
         def _():
             self.element.set_color(to_value(ref_ui))
 
         return self
 
-    def bind_value(self, ref_ui: ReadonlyRef[bool]):
+    def bind_value(self, ref_ui: TGetterOrReadonlyRef[bool]):
         @ui_effect
         def _():
             self.element.set_value(to_value(ref_ui))
 
         return self
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/column.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/row.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 from ex4nicegui.utils.signals import (
     _TMaybeRef as TMaybeRef,
 )
 from nicegui import ui
 from .base import BindableUi
 
 
-class ColumnBindableUi(BindableUi[ui.column]):
+class RowBindableUi(BindableUi[ui.row]):
     def __init__(self, *, wrap: TMaybeRef[bool] = True) -> None:
         pc = ParameterClassifier(locals(), maybeRefs=["wrap"], events=[])
-        element = ui.column(**pc.get_values_kws())
+        element = ui.row(**pc.get_values_kws())
 
         super().__init__(element)
-
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
     def bind_prop(self, prop: str, ref_ui: TMaybeRef):
         if prop == "wrap":
             return self.bind_wrap(ref_ui)
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/date.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/date.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Callable, List, Optional, TypeVar
 from typing_extensions import TypedDict
 from ex4nicegui.reactive.utils import ParameterClassifier
 from ex4nicegui.utils.apiEffect import ui_effect
 
 from ex4nicegui.utils.signals import (
-    ReadonlyRef,
+    TGetterOrReadonlyRef,
     _TMaybeRef as TMaybeRef,
     to_value,
 )
 from nicegui import ui
 from .base import BindableUi
 
 
@@ -41,21 +41,16 @@
         :param value: the initial date
         :param mask: the format of the date string (default: 'YYYY-MM-DD')
         :param on_change: callback to execute when changing the date
         """
         pc = ParameterClassifier(
             locals(),
             maybeRefs=[
-                "label",
                 "value",
-                "placeholder",
-                "password",
-                "password_toggle_button",
-                "autocomplete",
-                "validation",
+                "mask",
             ],
             v_model=("value", "on_change"),
             events=["on_change"],
         )
 
         value_kws = pc.get_values_kws()
         element = ui.date(**value_kws)
@@ -64,19 +59,19 @@
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
     @property
     def value(self):
         return self.element.value
 
-    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "value":
             return self.bind_value(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_value(self, ref_ui: ReadonlyRef[bool]):
+    def bind_value(self, ref_ui: TGetterOrReadonlyRef[bool]):
         @ui_effect
         def _():
             self.element.set_value(to_value(ref_ui))
 
         return self
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/drawer.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/drawer.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/echarts.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/echarts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Union, cast, Optional
+from typing import Any, Callable, Dict, List, Union, cast, Optional, Literal
 from ex4nicegui.reactive.utils import ParameterClassifier
 from ex4nicegui.utils.signals import (
-    ReadonlyRef,
+    TGetterOrReadonlyRef,
     is_ref,
     ref_computed,
     _TMaybeRef as TMaybeRef,
     to_value,
     to_raw,
     on,
 )
 from .base import BindableUi
 from ex4nicegui.reactive.EChartsComponent.ECharts import echarts
 from ex4nicegui.reactive.EChartsComponent.types import _T_event_name
 from ex4nicegui.reactive.EChartsComponent.events import EChartsMouseEventArguments
 
 from nicegui.awaitable_response import AwaitableResponse
 from nicegui import ui, app
+import orjson as json
 
 
 class EChartsBindableUi(BindableUi[echarts]):
     EChartsMouseEventArguments = EChartsMouseEventArguments
 
     def __init__(
         self,
@@ -42,38 +43,55 @@
         if not_merge is not None:
             self.__update_setting = {"notMerge": not_merge}
 
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
     @classmethod
-    def register_map(cls, map_name: str, src: Union[str, Path]):
+    def register_map(
+        cls,
+        map_name: str,
+        src: Union[str, Path],
+        *,
+        type: Literal["geoJSON", "svg"] = "geoJSON",
+        special_areas: Optional[Dict[str, Any]] = None,
+    ):
         """Registers available maps. This can only be used after including geo component or chart series of map.
 
         @see - https://github.com/CrystalWindSnake/ex4nicegui/blob/main/README.en.md#rxuiechartsregister_map
         @中文文档 - https://gitee.com/carson_add/ex4nicegui/tree/main/#rxuiechartsregister_map
 
         Args:
             map_name (str): Map name, referring to map value set in geo component or map.
             src (Union[str, Path]): Map data. If str, it should be a network address. If path, it should be a valid file.
+            type (Literal["geoJSON", "svg"], optional): Map data type. Defaults to "geoJSON".
+            special_areas (Optional[Dict[str, Any]], optional): Special areas. Defaults to None.
         """
         if isinstance(src, Path):
             src = app.add_static_file(local_file=src)
 
         assert isinstance(src, str)
 
         ui.add_body_html(
             rf"""
-            <script>
-                if (typeof window.ex4ngEchartsMapTasks === "undefined") {{ 
-                    window.ex4ngEchartsMapTasks = new Map();
-                }}
-
-                window.ex4ngEchartsMapTasks.set('{map_name}', '{src}');
-            </script>
+<script>
+    (function () {{
+        if (typeof window.ex4ngEchartsMapTasks === "undefined") {{
+            window.ex4ngEchartsMapTasks = new Map();
+        }}
+
+        const value = {{
+            src: '{src}',
+            type: '{type}',
+            specialAreas: {json.dumps(special_areas).decode('utf-8')}
+        }}
+
+        window.ex4ngEchartsMapTasks.set('{map_name}', value);
+    }})()
+</script>
         """
         )
 
         return cls
 
     @classmethod
     def from_pyecharts(cls, chart: TMaybeRef):
@@ -112,21 +130,21 @@
         ```
 
         """
         if isinstance(code, Path):
             code = code.read_text("utf8")
         return cls(code=code)
 
-    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "options":
             return self.bind_options(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_options(self, ref_ui: ReadonlyRef[Dict]):
+    def bind_options(self, ref_ui: TGetterOrReadonlyRef[Dict]):
         @on(ref_ui)
         def _():
             ele = self.element
             ele.update_options(to_raw(to_value(ref_ui)), self.__update_setting)
             ele.update()
 
         return self
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/expansion.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/expansion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Optional, Callable
 from nicegui import ui
 from ex4nicegui.reactive.utils import ParameterClassifier
 from ex4nicegui.utils.apiEffect import ui_effect
 from ex4nicegui.utils.signals import (
+    TGetterOrReadonlyRef,
     _TMaybeRef as TMaybeRef,
     to_value,
 )
 from .base import BindableUi
 
 
 class ExpansionBindableUi(BindableUi[ui.expansion]):
@@ -41,21 +42,21 @@
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
     @property
     def value(self):
         return self.element.value
 
-    def bind_prop(self, prop: str, ref_ui: TMaybeRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "value":
             return self.bind_value(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_value(self, ref_ui: TMaybeRef):
+    def bind_value(self, ref_ui: TGetterOrReadonlyRef):
         @ui_effect
         def _():
             self.element.set_value(to_value(ref_ui))
 
         return self
 
     def __enter__(self):
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/grid.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/grid.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/html.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/html.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/icon.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/icon.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     Optional,
     cast,
 )
 from ex4nicegui.reactive.utils import ParameterClassifier
 from ex4nicegui.utils.apiEffect import ui_effect
 
 from ex4nicegui.utils.signals import (
-    ReadonlyRef,
+    TGetterOrReadonlyRef,
     _TMaybeRef as TMaybeRef,
     to_value,
 )
 from nicegui import ui
 from nicegui.elements.mixins.color_elements import (
     TextColorElement,
 )
@@ -31,27 +31,27 @@
 
         element = ui.icon(**pc.get_values_kws())
         super().__init__(element)
 
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
-    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "name":
             return self.bind_name(ref_ui)
 
         if prop == "color":
             return self.bind_color(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_color(self, ref_ui: ReadonlyRef):
+    def bind_color(self, ref_ui: TGetterOrReadonlyRef):
         return _bind_color(self, ref_ui)
 
-    def bind_name(self, ref_ui: ReadonlyRef):
+    def bind_name(self, ref_ui: TGetterOrReadonlyRef):
         @ui_effect
         def _():
             ele = cast(TextColorElement, self.element)
             ele._props["name"] = to_value(ref_ui)
             ele.update()
 
         return self
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/image.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import (
     Union,
 )
 from ex4nicegui.reactive.utils import ParameterClassifier
 from ex4nicegui.utils.apiEffect import ui_effect
 
 from ex4nicegui.utils.signals import (
-    ReadonlyRef,
+    TGetterOrReadonlyRef,
     _TMaybeRef as TMaybeRef,
     to_value,
 )
 from nicegui import ui
 from .base import BindableUi
 
 
@@ -23,17 +23,17 @@
 
         element = ui.image(**pc.get_values_kws())
         super().__init__(element)
 
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
-    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "source":
             return self.bind_source(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_source(self, ref_ui: ReadonlyRef[Union[str, Path]]):
+    def bind_source(self, ref_ui: TGetterOrReadonlyRef[Union[str, Path]]):
         @ui_effect
         def _():
             self.element.set_source(to_value(ref_ui))
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/input.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Callable, List, Optional, Dict, cast
 from ex4nicegui.utils.apiEffect import ui_effect
 
 
 from ex4nicegui.utils.signals import (
-    ReadonlyRef,
+    TGetterOrReadonlyRef,
     Ref,
     _TMaybeRef as TMaybeRef,
     effect,
     is_setter_ref,
     to_value,
 )
 
@@ -49,31 +49,31 @@
 
         element = ui.input(**value_kws)
         super().__init__(element)  # type: ignore
 
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
-    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "value":
             return self.bind_value(ref_ui)
         if prop == "password":
             return self.bind_password(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_value(self, ref_ui: ReadonlyRef[str]):
+    def bind_value(self, ref_ui: TGetterOrReadonlyRef[str]):
         @ui_effect
         def _():
             self.element.set_value(to_value(ref_ui))
             self.element.update()
 
         return self
 
-    def bind_password(self, ref_ui: ReadonlyRef[bool]):
+    def bind_password(self, ref_ui: TGetterOrReadonlyRef[bool]):
         @ui_effect
         def _():
             self.element._props["type"] = "password" if to_value(ref_ui) else "text"
             self.element.update()
 
         return self
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/knob.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/knob.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,17 @@
     Callable,
     Optional,
 )
 from ex4nicegui.reactive.utils import ParameterClassifier
 from ex4nicegui.utils.apiEffect import ui_effect
 
 from ex4nicegui.utils.signals import (
-    ReadonlyRef,
     _TMaybeRef as TMaybeRef,
     to_value,
+    TGetterOrReadonlyRef,
 )
 from nicegui import ui
 from .base import BindableUi, DisableableMixin
 
 
 class KnobBindableUi(
     BindableUi[ui.knob],
@@ -57,19 +57,19 @@
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
     @property
     def value(self):
         return self.element.value
 
-    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "value":
             return self.bind_value(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_value(self, ref_ui: ReadonlyRef[float]):
+    def bind_value(self, ref_ui: TGetterOrReadonlyRef[float]):
         @ui_effect
         def _():
             self.element.set_value(to_value(ref_ui))
 
         return self
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/label.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/label.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any
 from ex4nicegui.reactive.utils import ParameterClassifier
 from ex4nicegui.utils.signals import (
+    TGetterOrReadonlyRef,
     to_value,
     _TMaybeRef as TMaybeRef,
 )
 from nicegui import ui
 from .base import BindableUi
 
 
@@ -21,31 +22,31 @@
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
     @property
     def text(self):
         return self.element.text
 
-    def bind_prop(self, prop: str, ref_ui: TMaybeRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "text":
             return self.bind_text(ref_ui)
 
         if prop == "color":
             return self.bind_color(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_color(self, ref_ui: TMaybeRef):
+    def bind_color(self, ref_ui: TGetterOrReadonlyRef):
         @self._ui_effect
         def _():
             ele = self.element
             color = to_value(ref_ui)
             ele._style["color"] = color
             ele.update()
 
-    def bind_text(self, ref_ui: TMaybeRef):
+    def bind_text(self, ref_ui: TGetterOrReadonlyRef):
         @self._ui_effect
         def _():
             self.element.set_text(str(to_value(ref_ui)))
             self.element.update()
 
         return self
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/linear_progress.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/linear_progress.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import (
     Optional,
 )
 from ex4nicegui.reactive.utils import ParameterClassifier
 from ex4nicegui.utils.apiEffect import ui_effect
 
 from ex4nicegui.utils.signals import (
-    ReadonlyRef,
+    TGetterOrReadonlyRef,
     _TMaybeRef as TMaybeRef,
     to_value,
 )
 from nicegui import ui
 
 from .base import BindableUi, _bind_color
 
@@ -43,25 +43,25 @@
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
     @property
     def value(self):
         return self.element.value
 
-    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "value":
             return self.bind_value(ref_ui)
 
         if prop == "color":
             return self.bind_color(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_color(self, ref_ui: ReadonlyRef):
+    def bind_color(self, ref_ui: TGetterOrReadonlyRef):
         return _bind_color(self, ref_ui)
 
-    def bind_value(self, ref_ui: ReadonlyRef):
+    def bind_value(self, ref_ui: TGetterOrReadonlyRef):
         @ui_effect
         def _():
             self.element.set_value(to_value(ref_ui))
 
         return self
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/number.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/number.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,33 +6,39 @@
     Dict,
     Union,
 )
 from ex4nicegui.reactive.utils import ParameterClassifier
 from ex4nicegui.utils.apiEffect import ui_effect
 
 from ex4nicegui.utils.signals import (
-    ReadonlyRef,
+    TGetterOrReadonlyRef,
     _TMaybeRef as TMaybeRef,
     to_value,
+    on,
 )
 from nicegui import ui
 from .base import BindableUi
 
 T = TypeVar("T")
 
 
+def _default_vmodel_args_getter(e):
+    return e.sender.value
+
+
 class NumberBindableUi(BindableUi[ui.number]):
     def __init__(
         self,
         label: Optional[TMaybeRef[str]] = None,
         *,
         placeholder: Optional[TMaybeRef[str]] = None,
         value: Optional[Union[TMaybeRef[float], TMaybeRef[int]]] = None,
         min: Optional[TMaybeRef[float]] = None,
         max: Optional[TMaybeRef[float]] = None,
+        precision: Optional[TMaybeRef[int]] = None,
         step: Optional[TMaybeRef[float]] = None,
         prefix: Optional[TMaybeRef[str]] = None,
         suffix: Optional[TMaybeRef[str]] = None,
         format: Optional[TMaybeRef[str]] = None,
         on_change: Optional[Callable[..., Any]] = None,
         validation: Dict[str, Callable[..., bool]] = {},
     ) -> None:
@@ -40,41 +46,53 @@
             locals(),
             maybeRefs=[
                 "label",
                 "placeholder",
                 "value",
                 "min",
                 "max",
+                "precision",
                 "step",
                 "prefix",
                 "suffix",
                 "format",
                 "validation",
             ],
             v_model=("value", "on_change"),
             events=["on_change"],
+            v_model_arg_getter=_default_vmodel_args_getter,
         )
 
         value_kws = pc.get_values_kws()
-
         element = ui.number(**value_kws)
         super().__init__(element)  # type: ignore
 
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
     @property
     def value(self):
         return self.element.value
 
-    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "value":
             return self.bind_value(ref_ui)
 
+        if prop == "precision":
+            return self._bind_precision(ref_ui)
+
         return super().bind_prop(prop, ref_ui)
 
-    def bind_value(self, ref_ui: ReadonlyRef[float]):
+    def bind_value(self, ref_ui: TGetterOrReadonlyRef[float]):
         @ui_effect
         def _():
             self.element.set_value(to_value(ref_ui))
 
         return self
+
+    def _bind_precision(self, ref_ui: TGetterOrReadonlyRef[int]):
+        @on(ref_ui, onchanges=True)
+        def _():
+            self.element.precision = to_value(ref_ui)
+            self.element.sanitize()
+
+        return self
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/radio.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/radio.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Dict,
     Union,
 )
 from ex4nicegui.reactive.utils import ParameterClassifier
 from ex4nicegui.utils.apiEffect import ui_effect
 
 from ex4nicegui.utils.signals import (
-    ReadonlyRef,
+    TGetterOrReadonlyRef,
     _TMaybeRef as TMaybeRef,
     to_value,
 )
 from nicegui import ui
 from nicegui.elements.mixins.value_element import ValueElement
 from .base import BindableUi
 
@@ -49,29 +49,29 @@
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
     @property
     def value(self):
         return self.element.value
 
-    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "value":
             return self.bind_value(ref_ui)
 
         if prop == "options":
             return self.bind_options(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_options(self, ref_ui: ReadonlyRef):
+    def bind_options(self, ref_ui: TGetterOrReadonlyRef):
         @ui_effect
         def _():
             self.element.set_options(to_value(ref_ui))
 
         return self
 
-    def bind_value(self, ref_ui: ReadonlyRef):
+    def bind_value(self, ref_ui: TGetterOrReadonlyRef):
         @ui_effect
         def _():
             cast(ValueElement, self.element).set_value(to_value(ref_ui))
 
         return self
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/row.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/column.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from typing import (
     Any,
 )
 from ex4nicegui.reactive.utils import ParameterClassifier
 from ex4nicegui.utils.signals import (
+    TGetterOrReadonlyRef,
     _TMaybeRef as TMaybeRef,
 )
 from nicegui import ui
 from .base import BindableUi
 
 
-class RowBindableUi(BindableUi[ui.row]):
+class ColumnBindableUi(BindableUi[ui.column]):
     def __init__(self, *, wrap: TMaybeRef[bool] = True) -> None:
         pc = ParameterClassifier(locals(), maybeRefs=["wrap"], events=[])
-        element = ui.row(**pc.get_values_kws())
+        element = ui.column(**pc.get_values_kws())
 
         super().__init__(element)
+
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
-    def bind_prop(self, prop: str, ref_ui: TMaybeRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "wrap":
             return self.bind_wrap(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_wrap(self, ref_ui: TMaybeRef):
+    def bind_wrap(self, ref_ui: TGetterOrReadonlyRef):
         self.bind_classes({"wrap": ref_ui})
 
     def __enter__(self):
         self.element.__enter__()
         return self
 
     def __exit__(self, *_: Any):
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/select.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/select.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Dict,
     Union,
 )
 from ex4nicegui.reactive.utils import ParameterClassifier
 from ex4nicegui.utils.apiEffect import ui_effect
 
 from ex4nicegui.utils.signals import (
-    ReadonlyRef,
+    TGetterOrReadonlyRef,
     _TMaybeRef as TMaybeRef,
     to_value,
 )
 from nicegui import ui
 from nicegui.elements.mixins.value_element import ValueElement
 from .base import BindableUi
 
@@ -71,29 +71,29 @@
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
     @property
     def value(self):
         return self.element.value
 
-    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "value":
             return self.bind_value(ref_ui)
 
         if prop == "options":
             return self.bind_options(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_options(self, ref_ui: ReadonlyRef):
+    def bind_options(self, ref_ui: TGetterOrReadonlyRef):
         @ui_effect()
         def _():
             self.element.set_options(to_value(ref_ui))
 
         return self
 
-    def bind_value(self, ref_ui: ReadonlyRef):
+    def bind_value(self, ref_ui: TGetterOrReadonlyRef):
         @ui_effect()
         def _():
             cast(ValueElement, self.element).set_value(to_value(ref_ui) or None)
 
         return self
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/slider.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/slider.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     TypeVar,
     cast,
 )
 from ex4nicegui.reactive.utils import ParameterClassifier
 from ex4nicegui.utils.apiEffect import ui_effect
 
 from ex4nicegui.utils.signals import (
-    ReadonlyRef,
+    TGetterOrReadonlyRef,
     Ref,
     _TMaybeRef as TMaybeRef,
     is_setter_ref,
     to_value,
 )
 from nicegui import ui
 from nicegui.events import handle_event
@@ -56,21 +56,21 @@
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
     @property
     def value(self):
         return self.element.value
 
-    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "value":
             return self.bind_value(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_value(self, ref_ui: ReadonlyRef[float]):
+    def bind_value(self, ref_ui: TGetterOrReadonlyRef[float]):
         @ui_effect
         def _():
             self.element.set_value(to_value(ref_ui))
             self.element.update()
 
         return self
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/switch.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/switch.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     Optional,
     TypeVar,
 )
 from ex4nicegui.reactive.utils import ParameterClassifier
 from ex4nicegui.utils.apiEffect import ui_effect
 
 from ex4nicegui.utils.signals import (
-    ReadonlyRef,
+    TGetterOrReadonlyRef,
     _TMaybeRef as TMaybeRef,
     to_value,
 )
 from nicegui import ui
 from .base import BindableUi
 
 T = TypeVar("T")
@@ -45,19 +45,19 @@
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
     @property
     def value(self):
         return self.element.value
 
-    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "value":
             return self.bind_value(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_value(self, ref_ui: ReadonlyRef[bool]):
+    def bind_value(self, ref_ui: TGetterOrReadonlyRef[bool]):
         @ui_effect
         def _():
             self.element.set_value(to_value(ref_ui))
 
         return self
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/tab.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/tab.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/tab_panel.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/tab_panel.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/tab_panels.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/q_pagination.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,50 @@
-from typing import Any, Callable, Optional
+from typing import Any, Optional, Callable
 from ex4nicegui.reactive.utils import ParameterClassifier
 from ex4nicegui.utils.signals import (
+    TGetterOrReadonlyRef,
     to_value,
     _TMaybeRef as TMaybeRef,
 )
 from nicegui import ui
-from .base import BindableUi
+from ex4nicegui.reactive.officials.base import BindableUi
 
 
-class TabPanelsBindableUi(BindableUi[ui.tab_panels]):
+class PaginationBindableUi(BindableUi[ui.pagination]):
     def __init__(
         self,
-        value: Optional[TMaybeRef[str]] = None,
-        *,
+        min: TMaybeRef[int],
+        max: TMaybeRef[int],
+        *,  # pylint: disable=redefined-builtin
+        direction_links: TMaybeRef[bool] = False,
+        value: TMaybeRef[int] = ...,  # type: ignore
         on_change: Optional[Callable[..., Any]] = None,
-        animated: TMaybeRef[bool] = True,
-        keep_alive: TMaybeRef[bool] = True,
     ) -> None:
         pc = ParameterClassifier(
             locals(),
-            maybeRefs=["value", "animated", "keep_alive"],
+            maybeRefs=["min", "max", "direction_links", "value"],
             v_model=("value", "on_change"),
             events=["on_change"],
         )
 
-        element = ui.tab_panels(**pc.get_values_kws())
+        element = ui.pagination(**pc.get_values_kws())
         super().__init__(element)
 
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
     @property
     def value(self):
         return self.element.value
 
-    def bind_prop(self, prop: str, ref_ui: TMaybeRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "value":
             return self.bind_value(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_value(self, ref_ui: TMaybeRef):
+    def bind_value(self, ref_ui: TGetterOrReadonlyRef[int]):
         @self._ui_effect
         def _():
             self.element.set_value(to_value(ref_ui))
+
+        return self
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/table.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     Optional,
     Dict,
 )
 from typing_extensions import Literal
 from ex4nicegui.reactive.utils import ParameterClassifier, dataframe2col_str
 import ex4nicegui.utils.common as utils_common
 from ex4nicegui.utils.signals import (
+    TGetterOrReadonlyRef,
     ReadonlyRef,
     is_ref,
     ref_computed,
     to_ref,
     _TMaybeRef as TMaybeRef,
     to_value,
     to_raw,
@@ -139,27 +140,27 @@
                 },
                 **columns_define_fn(col),
             }
             for col in df.columns  # type: ignore
         ]
         return cls(cols, rows, **other_kws)
 
-    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "dataframe":
             return self.bind_dataframe(ref_ui)
 
         if prop == "rows":
             return self.bind_rows(ref_ui)
 
         if prop == "columns":
             return self.bind_columns(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_dataframe(self, ref_df: ReadonlyRef):
+    def bind_dataframe(self, ref_df: TGetterOrReadonlyRef):
         @ref_computed
         def cp_converted_df():
             df = ref_df.value
             return utils_common.convert_dataframe(df)
 
         @ref_computed
         def cp_rows():
@@ -176,24 +177,24 @@
                 for col in cp_converted_df.value.columns
             ]
 
         self.bind_rows(cp_rows).bind_columns(cp_cols)  # type: ignore
 
         return self
 
-    def bind_rows(self, ref_ui: ReadonlyRef[List[Dict]]):
+    def bind_rows(self, ref_ui: TGetterOrReadonlyRef[List[Dict]]):
         @on(ref_ui, deep=True)
         def _():
             ele = self.element
             ele._props["rows"] = list(to_raw(to_value(ref_ui)))
             ele.update()
 
         return self
 
-    def bind_columns(self, ref_ui: ReadonlyRef[List[Dict]]):
+    def bind_columns(self, ref_ui: TGetterOrReadonlyRef[List[Dict]]):
         @on(ref_ui, deep=True)
         def _():
             ele = self.element
             ele._props["columns"] = list(to_raw(to_value(ref_ui)))
             ele.update()
 
         return self
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/textarea.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/textarea.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     Optional,
     Dict,
     cast,
 )
 from ex4nicegui.reactive.utils import ParameterClassifier
 from ex4nicegui.utils.apiEffect import ui_effect
 from ex4nicegui.utils.signals import (
-    ReadonlyRef,
+    TGetterOrReadonlyRef,
     Ref,
     _TMaybeRef as TMaybeRef,
     effect,
     is_setter_ref,
     to_value,
 )
 from nicegui import ui
@@ -50,21 +50,21 @@
         for key, value in pc.get_bindings().items():
             self.bind_prop(key, value)  # type: ignore
 
     @property
     def value(self):
         return self.element.value
 
-    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+    def bind_prop(self, prop: str, ref_ui: TGetterOrReadonlyRef):
         if prop == "value":
             return self.bind_value(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    def bind_value(self, ref_ui: ReadonlyRef[str]):
+    def bind_value(self, ref_ui: TGetterOrReadonlyRef[str]):
         @ui_effect
         def _():
             self.element.set_value(to_value(ref_ui))
 
         return self
```

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/officials/upload.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/officials/upload.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/transitionGroup.js` & `ex4nicegui-0.6.7/ex4nicegui/reactive/transitionGroup.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/transitionGroup.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/transitionGroup.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/useMouse/UseMouse.js` & `ex4nicegui-0.6.7/ex4nicegui/reactive/useMouse/UseMouse.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/useMouse/UseMouse.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/useMouse/UseMouse.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/usePagination.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/usePagination.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/utils.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/utils.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/vfor.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/vfor.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/reactive/vmodel.py` & `ex4nicegui-0.6.7/ex4nicegui/reactive/vmodel.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/tools/debug.py` & `ex4nicegui-0.6.7/ex4nicegui/tools/debug.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/utils/apiEffect.py` & `ex4nicegui-0.6.7/ex4nicegui/utils/apiEffect.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/utils/asyncComputed.py` & `ex4nicegui-0.6.7/ex4nicegui/utils/asyncComputed.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/utils/clientScope.py` & `ex4nicegui-0.6.7/ex4nicegui/utils/clientScope.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/utils/common.py` & `ex4nicegui-0.6.7/ex4nicegui/utils/common.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/utils/effect.py` & `ex4nicegui-0.6.7/ex4nicegui/utils/effect.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/utils/scheduler.py` & `ex4nicegui-0.6.7/ex4nicegui/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.6/ex4nicegui/utils/signals.py` & `ex4nicegui-0.6.7/ex4nicegui/utils/signals.py`

 * *Files identical despite different names*


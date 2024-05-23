# Comparing `tmp/glotlib-0.9.6.tar.gz` & `tmp/glotlib-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glotlib-0.9.6.tar", last modified: Tue Feb  6 23:19:34 2024, max compression
+gzip compressed data, was "glotlib-0.9.7.tar", last modified: Thu May 23 22:47:19 2024, max compression
```

## Comparing `glotlib-0.9.6.tar` & `glotlib-0.9.7.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-02-06 23:19:34.869221 glotlib-0.9.6/
--rw-r--r--   0 greent7    (502) staff       (20)    26526 2023-07-11 00:37:56.000000 glotlib-0.9.6/LICENSE
--rw-r--r--   0 greent7    (502) staff       (20)      653 2024-02-06 23:19:34.869129 glotlib-0.9.6/PKG-INFO
--rw-r--r--   0 greent7    (502) staff       (20)       66 2023-07-11 00:59:47.000000 glotlib-0.9.6/README.txt
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-02-06 23:19:34.862450 glotlib-0.9.6/glotlib/
--rw-r--r--   0 greent7    (502) staff       (20)      609 2023-07-20 00:12:44.000000 glotlib-0.9.6/glotlib/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     1274 2023-07-20 00:12:44.000000 glotlib-0.9.6/glotlib/colors.py
--rw-r--r--   0 greent7    (502) staff       (20)      162 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/constants.py
--rw-r--r--   0 greent7    (502) staff       (20)     6924 2023-08-10 23:59:21.000000 glotlib-0.9.6/glotlib/font.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-02-06 23:19:34.863367 glotlib-0.9.6/glotlib/font_files/
--rw-r--r--   0 greent7    (502) staff       (20)        0 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/font_files/__init__.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-02-06 23:19:34.865912 glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/
--rw-r--r--   0 greent7    (502) staff       (20)     5954 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/COPYRIGHT.TXT
--rw-r--r--   0 greent7    (502) staff       (20)      320 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/README.TXT
--rw-r--r--   0 greent7    (502) staff       (20)     8112 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/RELEASENOTES.TXT
--rw-r--r--   0 greent7    (502) staff       (20)    65932 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/Vera.ttf
--rw-r--r--   0 greent7    (502) staff       (20)    63208 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/VeraBI.ttf
--rw-r--r--   0 greent7    (502) staff       (20)    58716 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/VeraBd.ttf
--rw-r--r--   0 greent7    (502) staff       (20)    63684 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/VeraIt.ttf
--rw-r--r--   0 greent7    (502) staff       (20)    55032 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/VeraMoBI.ttf
--rw-r--r--   0 greent7    (502) staff       (20)    49052 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/VeraMoBd.ttf
--rw-r--r--   0 greent7    (502) staff       (20)    54508 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/VeraMoIt.ttf
--rw-r--r--   0 greent7    (502) staff       (20)    49224 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/VeraMono.ttf
--rw-r--r--   0 greent7    (502) staff       (20)    60280 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/VeraSe.ttf
--rw-r--r--   0 greent7    (502) staff       (20)    58736 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/VeraSeBd.ttf
--rw-r--r--   0 greent7    (502) staff       (20)     1012 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/local.conf
--rw-r--r--   0 greent7    (502) staff       (20)      123 2023-08-10 23:59:24.000000 glotlib-0.9.6/glotlib/fonts.py
--rw-r--r--   0 greent7    (502) staff       (20)     1773 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/hline.py
--rw-r--r--   0 greent7    (502) staff       (20)     4399 2024-02-05 08:15:40.000000 glotlib-0.9.6/glotlib/label.py
--rw-r--r--   0 greent7    (502) staff       (20)     2876 2024-01-13 00:45:26.000000 glotlib-0.9.6/glotlib/main.py
--rw-r--r--   0 greent7    (502) staff       (20)     1935 2024-02-06 23:08:54.000000 glotlib-0.9.6/glotlib/matrix.py
--rw-r--r--   0 greent7    (502) staff       (20)     2740 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/miter_lines.py
--rw-r--r--   0 greent7    (502) staff       (20)    16714 2024-02-05 08:15:01.000000 glotlib-0.9.6/glotlib/plot.py
--rw-r--r--   0 greent7    (502) staff       (20)     2430 2023-08-10 23:57:14.000000 glotlib-0.9.6/glotlib/program.py
--rw-r--r--   0 greent7    (502) staff       (20)     2534 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/programs.py
--rw-r--r--   0 greent7    (502) staff       (20)     5115 2024-02-06 00:50:48.000000 glotlib-0.9.6/glotlib/series.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-02-06 23:19:34.867103 glotlib-0.9.6/glotlib/shaders/
--rw-r--r--   0 greent7    (502) staff       (20)        0 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/shaders/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)       99 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/shaders/frag.frag
--rw-r--r--   0 greent7    (502) staff       (20)     1311 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/shaders/miter_line.vert
--rw-r--r--   0 greent7    (502) staff       (20)      161 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/shaders/mvp_z.vert
--rw-r--r--   0 greent7    (502) staff       (20)      195 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/shaders/points.frag
--rw-r--r--   0 greent7    (502) staff       (20)     1548 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/shaders/square_instanced_line.vert
--rw-r--r--   0 greent7    (502) staff       (20)      260 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/shaders/text.frag
--rw-r--r--   0 greent7    (502) staff       (20)      251 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/shaders/text.vert
--rw-r--r--   0 greent7    (502) staff       (20)     1793 2024-02-05 08:15:36.000000 glotlib-0.9.6/glotlib/step_series.py
--rw-r--r--   0 greent7    (502) staff       (20)     2090 2023-08-10 23:24:49.000000 glotlib-0.9.6/glotlib/ticker.py
--rw-r--r--   0 greent7    (502) staff       (20)     5289 2024-02-06 00:50:58.000000 glotlib-0.9.6/glotlib/vbo.py
--rw-r--r--   0 greent7    (502) staff       (20)     1849 2023-07-11 00:37:56.000000 glotlib-0.9.6/glotlib/vline.py
--rw-r--r--   0 greent7    (502) staff       (20)    12787 2024-02-06 23:11:01.000000 glotlib-0.9.6/glotlib/window.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-02-06 23:19:34.868905 glotlib-0.9.6/glotlib.egg-info/
--rw-r--r--   0 greent7    (502) staff       (20)      653 2024-02-06 23:19:34.000000 glotlib-0.9.6/glotlib.egg-info/PKG-INFO
--rw-r--r--   0 greent7    (502) staff       (20)     1745 2024-02-06 23:19:34.000000 glotlib-0.9.6/glotlib.egg-info/SOURCES.txt
--rw-r--r--   0 greent7    (502) staff       (20)        1 2024-02-06 23:19:34.000000 glotlib-0.9.6/glotlib.egg-info/dependency_links.txt
--rw-r--r--   0 greent7    (502) staff       (20)       46 2024-02-06 23:19:34.000000 glotlib-0.9.6/glotlib.egg-info/requires.txt
--rw-r--r--   0 greent7    (502) staff       (20)        8 2024-02-06 23:19:34.000000 glotlib-0.9.6/glotlib.egg-info/top_level.txt
--rw-r--r--   0 greent7    (502) staff       (20)      838 2024-02-06 23:19:34.869553 glotlib-0.9.6/setup.cfg
--rw-r--r--   0 greent7    (502) staff       (20)       38 2023-07-11 00:37:56.000000 glotlib-0.9.6/setup.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-02-06 23:19:34.868658 glotlib-0.9.6/tests/
--rw-r--r--   0 greent7    (502) staff       (20)      251 2023-07-11 00:37:56.000000 glotlib-0.9.6/tests/test1.py
--rw-r--r--   0 greent7    (502) staff       (20)     1379 2024-02-06 23:08:54.000000 glotlib-0.9.6/tests/test10.py
--rw-r--r--   0 greent7    (502) staff       (20)      260 2024-02-06 23:08:54.000000 glotlib-0.9.6/tests/test11.py
--rw-r--r--   0 greent7    (502) staff       (20)     1046 2023-07-11 00:37:56.000000 glotlib-0.9.6/tests/test2.py
--rw-r--r--   0 greent7    (502) staff       (20)     1064 2023-07-11 00:37:56.000000 glotlib-0.9.6/tests/test3.py
--rw-r--r--   0 greent7    (502) staff       (20)     1020 2024-02-05 07:19:05.000000 glotlib-0.9.6/tests/test4.py
--rw-r--r--   0 greent7    (502) staff       (20)      727 2023-07-11 00:37:56.000000 glotlib-0.9.6/tests/test5.py
--rw-r--r--   0 greent7    (502) staff       (20)      179 2023-07-11 00:37:56.000000 glotlib-0.9.6/tests/test6.py
--rw-r--r--   0 greent7    (502) staff       (20)     2250 2023-07-20 00:12:44.000000 glotlib-0.9.6/tests/test7.py
--rw-r--r--   0 greent7    (502) staff       (20)      584 2024-02-05 08:15:40.000000 glotlib-0.9.6/tests/test8.py
--rw-r--r--   0 greent7    (502) staff       (20)     1156 2024-02-05 08:15:32.000000 glotlib-0.9.6/tests/test9.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 22:47:19.122642 glotlib-0.9.7/
+-rw-r--r--   0 greent7    (502) staff       (20)    26526 2023-07-11 00:37:56.000000 glotlib-0.9.7/LICENSE
+-rw-r--r--   0 greent7    (502) staff       (20)      653 2024-05-23 22:47:19.122567 glotlib-0.9.7/PKG-INFO
+-rw-r--r--   0 greent7    (502) staff       (20)       66 2023-07-11 00:59:47.000000 glotlib-0.9.7/README.txt
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 22:47:19.116393 glotlib-0.9.7/glotlib/
+-rw-r--r--   0 greent7    (502) staff       (20)      609 2023-07-20 00:12:44.000000 glotlib-0.9.7/glotlib/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1255 2024-05-23 21:49:41.000000 glotlib-0.9.7/glotlib/colors.py
+-rw-r--r--   0 greent7    (502) staff       (20)      162 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/constants.py
+-rw-r--r--   0 greent7    (502) staff       (20)     6924 2023-08-10 23:59:21.000000 glotlib-0.9.7/glotlib/font.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 22:47:19.117093 glotlib-0.9.7/glotlib/font_files/
+-rw-r--r--   0 greent7    (502) staff       (20)        0 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/font_files/__init__.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 22:47:19.119449 glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/
+-rw-r--r--   0 greent7    (502) staff       (20)     5954 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/COPYRIGHT.TXT
+-rw-r--r--   0 greent7    (502) staff       (20)      320 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/README.TXT
+-rw-r--r--   0 greent7    (502) staff       (20)     8112 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/RELEASENOTES.TXT
+-rw-r--r--   0 greent7    (502) staff       (20)    65932 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/Vera.ttf
+-rw-r--r--   0 greent7    (502) staff       (20)    63208 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/VeraBI.ttf
+-rw-r--r--   0 greent7    (502) staff       (20)    58716 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/VeraBd.ttf
+-rw-r--r--   0 greent7    (502) staff       (20)    63684 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/VeraIt.ttf
+-rw-r--r--   0 greent7    (502) staff       (20)    55032 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/VeraMoBI.ttf
+-rw-r--r--   0 greent7    (502) staff       (20)    49052 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/VeraMoBd.ttf
+-rw-r--r--   0 greent7    (502) staff       (20)    54508 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/VeraMoIt.ttf
+-rw-r--r--   0 greent7    (502) staff       (20)    49224 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/VeraMono.ttf
+-rw-r--r--   0 greent7    (502) staff       (20)    60280 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/VeraSe.ttf
+-rw-r--r--   0 greent7    (502) staff       (20)    58736 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/VeraSeBd.ttf
+-rw-r--r--   0 greent7    (502) staff       (20)     1012 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/local.conf
+-rw-r--r--   0 greent7    (502) staff       (20)      123 2023-08-10 23:59:24.000000 glotlib-0.9.7/glotlib/fonts.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1773 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/hline.py
+-rw-r--r--   0 greent7    (502) staff       (20)     4436 2024-05-23 22:27:25.000000 glotlib-0.9.7/glotlib/label.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2876 2024-01-13 00:45:26.000000 glotlib-0.9.7/glotlib/main.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1935 2024-02-06 23:40:38.000000 glotlib-0.9.7/glotlib/matrix.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2740 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/miter_lines.py
+-rw-r--r--   0 greent7    (502) staff       (20)    18407 2024-05-23 22:45:28.000000 glotlib-0.9.7/glotlib/plot.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2430 2023-08-10 23:57:14.000000 glotlib-0.9.7/glotlib/program.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2534 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/programs.py
+-rw-r--r--   0 greent7    (502) staff       (20)     5115 2024-02-06 00:50:48.000000 glotlib-0.9.7/glotlib/series.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 22:47:19.120797 glotlib-0.9.7/glotlib/shaders/
+-rw-r--r--   0 greent7    (502) staff       (20)        0 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/shaders/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)       99 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/shaders/frag.frag
+-rw-r--r--   0 greent7    (502) staff       (20)     1311 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/shaders/miter_line.vert
+-rw-r--r--   0 greent7    (502) staff       (20)      161 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/shaders/mvp_z.vert
+-rw-r--r--   0 greent7    (502) staff       (20)      195 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/shaders/points.frag
+-rw-r--r--   0 greent7    (502) staff       (20)     1548 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/shaders/square_instanced_line.vert
+-rw-r--r--   0 greent7    (502) staff       (20)      260 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/shaders/text.frag
+-rw-r--r--   0 greent7    (502) staff       (20)      251 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/shaders/text.vert
+-rw-r--r--   0 greent7    (502) staff       (20)     1793 2024-02-05 08:15:36.000000 glotlib-0.9.7/glotlib/step_series.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2090 2023-08-10 23:24:49.000000 glotlib-0.9.7/glotlib/ticker.py
+-rw-r--r--   0 greent7    (502) staff       (20)     5289 2024-05-21 20:14:20.000000 glotlib-0.9.7/glotlib/vbo.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1849 2023-07-11 00:37:56.000000 glotlib-0.9.7/glotlib/vline.py
+-rw-r--r--   0 greent7    (502) staff       (20)    12787 2024-02-06 23:40:38.000000 glotlib-0.9.7/glotlib/window.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 22:47:19.122332 glotlib-0.9.7/glotlib.egg-info/
+-rw-r--r--   0 greent7    (502) staff       (20)      653 2024-05-23 22:47:19.000000 glotlib-0.9.7/glotlib.egg-info/PKG-INFO
+-rw-r--r--   0 greent7    (502) staff       (20)     1745 2024-05-23 22:47:19.000000 glotlib-0.9.7/glotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 greent7    (502) staff       (20)        1 2024-05-23 22:47:19.000000 glotlib-0.9.7/glotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 greent7    (502) staff       (20)       46 2024-05-23 22:47:19.000000 glotlib-0.9.7/glotlib.egg-info/requires.txt
+-rw-r--r--   0 greent7    (502) staff       (20)        8 2024-05-23 22:47:19.000000 glotlib-0.9.7/glotlib.egg-info/top_level.txt
+-rw-r--r--   0 greent7    (502) staff       (20)      838 2024-05-23 22:47:19.122887 glotlib-0.9.7/setup.cfg
+-rw-r--r--   0 greent7    (502) staff       (20)       38 2023-07-11 00:37:56.000000 glotlib-0.9.7/setup.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 22:47:19.122157 glotlib-0.9.7/tests/
+-rw-r--r--   0 greent7    (502) staff       (20)      321 2024-05-23 22:45:28.000000 glotlib-0.9.7/tests/test1.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1415 2024-05-23 21:48:07.000000 glotlib-0.9.7/tests/test10.py
+-rw-r--r--   0 greent7    (502) staff       (20)      247 2024-05-23 21:48:13.000000 glotlib-0.9.7/tests/test11.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1046 2023-07-11 00:37:56.000000 glotlib-0.9.7/tests/test2.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1064 2023-07-11 00:37:56.000000 glotlib-0.9.7/tests/test3.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1020 2024-02-05 07:19:05.000000 glotlib-0.9.7/tests/test4.py
+-rw-r--r--   0 greent7    (502) staff       (20)      727 2023-07-11 00:37:56.000000 glotlib-0.9.7/tests/test5.py
+-rw-r--r--   0 greent7    (502) staff       (20)      179 2023-07-11 00:37:56.000000 glotlib-0.9.7/tests/test6.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2250 2023-07-20 00:12:44.000000 glotlib-0.9.7/tests/test7.py
+-rw-r--r--   0 greent7    (502) staff       (20)      584 2024-02-05 08:15:40.000000 glotlib-0.9.7/tests/test8.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1156 2024-02-05 08:15:32.000000 glotlib-0.9.7/tests/test9.py
```

### Comparing `glotlib-0.9.6/LICENSE` & `glotlib-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/PKG-INFO` & `glotlib-0.9.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glotlib
-Version: 0.9.6
+Version: 0.9.7
 Summary: Library for creating plots using OpenGL.
 Home-page: https://github.com/tgree/glotlib
 Author: Terry Greeniaus
 Author-email: terry.greeniaus@gmail.com
 License: LGPLv2
 Keywords: glotlib
 Classifier: Operating System :: OS Independent
```

### Comparing `glotlib-0.9.6/glotlib/__init__.py` & `glotlib-0.9.7/glotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/colors.py` & `glotlib-0.9.7/glotlib/colors.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,15 @@
     'black'     : (0, 0, 0, 1),
     'white'     : (1, 1, 1, 1),
 }
 
 
 def cycle(iterable):
     while iterable:
-        for e in iterable:
-            yield e
+        yield from iterable
 
 
 def make(v, none_iter):
     if v is None:
         return next(none_iter)
     if isinstance(v, tuple):
         if len(v) == 4:
```

### Comparing `glotlib-0.9.6/glotlib/font.py` & `glotlib-0.9.7/glotlib/font.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/COPYRIGHT.TXT` & `glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/COPYRIGHT.TXT`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/RELEASENOTES.TXT` & `glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/RELEASENOTES.TXT`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/Vera.ttf` & `glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/Vera.ttf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/VeraBI.ttf` & `glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/VeraBI.ttf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/VeraBd.ttf` & `glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/VeraBd.ttf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/VeraIt.ttf` & `glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/VeraIt.ttf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/VeraMoBI.ttf` & `glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/VeraMoBI.ttf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/VeraMoBd.ttf` & `glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/VeraMoBd.ttf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/VeraMoIt.ttf` & `glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/VeraMoIt.ttf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/VeraMono.ttf` & `glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/VeraMono.ttf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/VeraSe.ttf` & `glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/VeraSe.ttf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/VeraSeBd.ttf` & `glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/VeraSeBd.ttf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/font_files/ttf_bitstream_vera_1_10/local.conf` & `glotlib-0.9.7/glotlib/font_files/ttf_bitstream_vera_1_10/local.conf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/hline.py` & `glotlib-0.9.7/glotlib/hline.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/label.py` & `glotlib-0.9.7/glotlib/label.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,19 @@
     'W'     : (HAlign.LEFT,     VAlign.MIDDLE),
     'NW'    : (HAlign.LEFT,     VAlign.TOP),
     'C'     : (HAlign.MIDDLE,   VAlign.MIDDLE),
 }
 
 
 class Label:
-    def __init__(self, pos, text, font=None, theta=0, anchor='SW',
+    def __init__(self, window, pos, text, font=None, theta=0, anchor='SW',
                  visible=True):
         assert font
 
+        self.window    = window
         self.font      = font
         self.pos       = (round(pos[0]), round(pos[1]))
         self.theta     = theta
         self.visible   = visible
         self.text      = None
         self.mvp       = None
         alignment      = ALIGNMENTS[anchor]
@@ -110,41 +111,40 @@
         self.font.bind(0)
         programs.text.use(0, mvp, self.font, color=color)
         GL.glEnable(GL.GL_BLEND)
         GL.glDrawArrays(GL.GL_TRIANGLES, 0, self.nvertices)
         GL.glDisable(GL.GL_BLEND)
 
     def draw_batched(self, mvp):
-        if not self.nvertices:
+        if not self.nvertices or not self.visible:
             return
 
         mvp = mvp @ self.mvp
         programs.text.uniformMatrix4fv('u_mvp', mvp)
         GL.glBindVertexArray(self.vao)
         GL.glDrawArrays(GL.GL_TRIANGLES, 0, self.nvertices)
 
+    def show(self):
+        self.visible = True
+        self.window.mark_dirty()
+
+    def hide(self):
+        self.visible = False
+        self.window.mark_dirty()
+
 
 class FlexLabel(Label):
     def __init__(self, window, pos, *args, **kwargs):
-        self.window   = window
         self.flex_pos = pos
         pos           = (pos[0] * window.w_w, pos[1] * window.w_h)
-        super().__init__(pos, *args, **kwargs)
+        super().__init__(window, pos, *args, **kwargs)
 
     def _handle_resize(self):
         pos = (self.flex_pos[0] * self.window.w_w,
                self.flex_pos[1] * self.window.w_h)
         super().set_pos(pos)
 
     def set_pos(self, pos):
         self.flex_pos = pos
         pos           = (pos[0] * self.window.w_w,
                          pos[1] * self.window.w_h)
         super().set_pos(pos)
-
-    def show(self):
-        self.visible = True
-        self.window.mark_dirty()
-
-    def hide(self):
-        self.visible = False
-        self.window.mark_dirty()
```

### Comparing `glotlib-0.9.6/glotlib/main.py` & `glotlib-0.9.7/glotlib/main.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/matrix.py` & `glotlib-0.9.7/glotlib/matrix.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/miter_lines.py` & `glotlib-0.9.7/glotlib/miter_lines.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/plot.py` & `glotlib-0.9.7/glotlib/plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -121,20 +121,27 @@
         self.h_ticks        = []
         self.v_ticks        = []
 
         self.sharex.add(self)
         self.sharey.add(self)
 
         for _ in range(max_h_ticks):
-            self.h_ticks.append(Label((0, 0), '', fonts.vera(12, 0),
+            self.h_ticks.append(Label(window, (0, 0), '', fonts.vera(12, 0),
                                       anchor='N'))
         for _ in range(max_v_ticks):
-            self.v_ticks.append(Label((0, 0), '', fonts.vera(12, 0),
+            self.v_ticks.append(Label(window, (0, 0), '', fonts.vera(12, 0),
                                       anchor='E'))
 
+        self.x_label = Label(window, (0, 0), '', fonts.vera(12, 0), anchor='N',
+                             visible=False)
+        self.x_label_side = 'bottom'
+        self.y_label = Label(window, (0, 0), '', fonts.vera(12, 0), anchor='S',
+                             visible=False, theta=math.pi / 2)
+        self.y_label_side = 'left'
+
         self._gen_bounds()
         l, r, b, t = self._adjust_lrbt(l, r, b, t)
         self._renormalize(l, r, b, t)
         self._gen_ticks()
         self._update_shared_axes()
 
     def _get_data_bounds(self):
@@ -239,14 +246,31 @@
                 y = int((ticks[i] - b) * self.h / (t - b))
                 v_t.set_pos((self.x - 2, self.y + y + 2))
                 v_t.set_text(texts[i])
             else:
                 v_t.pos = (0, 0)
                 v_t.set_text('')
 
+        self._gen_labels()
+
+    def _gen_labels(self):
+        if self.x_label_side == 'bottom':
+            x_ticks_height = max(h_t.height for h_t in self.h_ticks)
+            self.x_label.set_pos((self.x + self.w / 2,
+                                  self.y - x_ticks_height - 6))
+        else:
+            self.x_label.set_pos((self.x + self.w / 2, self.y + self.h + 18))
+
+        if self.y_label_side == 'left':
+            y_ticks_width = max(v_t.width for v_t in self.v_ticks)
+            self.y_label.set_pos((self.x - y_ticks_width - 16,
+                                  self.y + self.h / 2))
+        else:
+            self.y_label.set_pos((self.x + self.w + 16, self.y + self.h / 2))
+
     def _gen_mvp_from_limits(self, l, r, b, t):
         '''
         Generates mvp and mvpi such that we will be viewing the specified
         rectangle of data dimensions.  This is a simple orthographic
         projection.
         '''
         ml, mb, _, _ = self.rmatrix @ (l, b, 0, 1)
@@ -451,14 +475,34 @@
         l, r, _, _ = self._get_data_bounds()
         w, _ = self.aspect.adjust_horiz((r - l, t - b), (self.w, self.h))
         l    = (l + r - w) / 2
         r    = (l + r + w) / 2
         self._gen_mvp_from_limits(l, r, b, t)
         self._gen_ticks()
 
+    def set_x_label(self, t, side='bottom'):
+        self.x_label.set_text(t)
+        if t != '':
+            self.x_label.show()
+        else:
+            self.x_label.hide()
+        self.x_label_side = side
+        self._gen_labels()
+        self.window.mark_dirty()
+
+    def set_y_label(self, t, side='left'):
+        self.y_label.set_text(t)
+        if t != '':
+            self.y_label.show()
+        else:
+            self.y_label.hide()
+        self.y_label_side = side
+        self._gen_labels()
+        self.window.mark_dirty()
+
     def show(self):
         self.visible = True
         self.window.mark_dirty()
 
     def hide(self):
         self.visible = False
         self.window.mark_dirty()
@@ -479,13 +523,15 @@
         programs.text.uniform4f('u_color', 0, 0, 0, 1)
         programs.text.uniform1i('u_sampler', 0)
         GL.glEnable(GL.GL_BLEND)
         for h_t in self.h_ticks:
             h_t.draw_batched(self.window.mvp)
         for v_t in self.v_ticks:
             v_t.draw_batched(self.window.mvp)
+        self.x_label.draw_batched(self.window.mvp)
+        self.y_label.draw_batched(self.window.mvp)
         GL.glDisable(GL.GL_BLEND)
 
         GL.glViewport(self.fb_x, self.fb_y, self.fb_w, self.fb_h)
         for ga in self.graph_artists:
             # TODO: I feel like this is where self.mvp32 goes.
             ga.draw(t, 0, self.mvp, (self.w, self.h))
```

### Comparing `glotlib-0.9.6/glotlib/program.py` & `glotlib-0.9.7/glotlib/program.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/programs.py` & `glotlib-0.9.7/glotlib/programs.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/series.py` & `glotlib-0.9.7/glotlib/series.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/shaders/miter_line.vert` & `glotlib-0.9.7/glotlib/shaders/miter_line.vert`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/shaders/square_instanced_line.vert` & `glotlib-0.9.7/glotlib/shaders/square_instanced_line.vert`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/step_series.py` & `glotlib-0.9.7/glotlib/step_series.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/ticker.py` & `glotlib-0.9.7/glotlib/ticker.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/vbo.py` & `glotlib-0.9.7/glotlib/vbo.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         vertices list.
         '''
         self.set_component_data(1, Y)
 
     def set_x_y_data(self, X, Y):
         '''
         Replaces the first and second components of all vertices with the
-        specifeid X and Y values, which must both be the same length and match
+        specified X and Y values, which must both be the same length and match
         the number of entries in the current vertices list, unless the current
         vertices list is only comprised of (x, y) vertices in which case it can
         simply replace them all.
         '''
         if self.ncomponents == 2:
             self.set_data(np.column_stack((X, Y)).astype(np.float32,
                                                          copy=False))
```

### Comparing `glotlib-0.9.6/glotlib/vline.py` & `glotlib-0.9.7/glotlib/vline.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib/window.py` & `glotlib-0.9.7/glotlib/window.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/glotlib.egg-info/PKG-INFO` & `glotlib-0.9.7/glotlib.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glotlib
-Version: 0.9.6
+Version: 0.9.7
 Summary: Library for creating plots using OpenGL.
 Home-page: https://github.com/tgree/glotlib
 Author: Terry Greeniaus
 Author-email: terry.greeniaus@gmail.com
 License: LGPLv2
 Keywords: glotlib
 Classifier: Operating System :: OS Independent
```

### Comparing `glotlib-0.9.6/glotlib.egg-info/SOURCES.txt` & `glotlib-0.9.7/glotlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/setup.cfg` & `glotlib-0.9.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = glotlib
-version = 0.9.6
+version = 0.9.7
 author = Terry Greeniaus
 author_email = terry.greeniaus@gmail.com
 description = Library for creating plots using OpenGL.
 long_description = Library for creating plots using OpenGL.
 long_description_content_type = text/x-rst
 keywords = glotlib
 url = https://github.com/tgree/glotlib
```

### Comparing `glotlib-0.9.6/tests/test10.py` & `glotlib-0.9.7/tests/test10.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,16 @@
         self.plot = self.add_plot(limits=(0, DY - 1, 2 * math.pi, DY + 1))
 
         self.series  = [self.plot.add_lines(X=[], Y=[], width=1, point_width=1)
                         for _ in AMP_RATES[:-1]]
         self.series += [self.plot.add_steps(X=[], Y=[], width=1, point_width=1)
                         for _ in AMP_RATES[-1:]]
         self.index = 0
-        self.label = self.add_label((0, 1), '', font=fonts.vera(20, 1), anchor='NW')
+        self.label = self.add_label((0, 1), '', font=fonts.vera(20, 1),
+                                    anchor='NW')
 
     def update_geometry(self, t):
         if self.index >= 10000000:
             return False
 
         for s, ar, tr in zip(self.series, AMP_RATES, THICK_RATES):
             X = dX * (self.index + np.arange(100))
```

### Comparing `glotlib-0.9.6/tests/test2.py` & `glotlib-0.9.7/tests/test2.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/tests/test3.py` & `glotlib-0.9.7/tests/test3.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/tests/test4.py` & `glotlib-0.9.7/tests/test4.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/tests/test5.py` & `glotlib-0.9.7/tests/test5.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/tests/test7.py` & `glotlib-0.9.7/tests/test7.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/tests/test8.py` & `glotlib-0.9.7/tests/test8.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.6/tests/test9.py` & `glotlib-0.9.7/tests/test9.py`

 * *Files identical despite different names*


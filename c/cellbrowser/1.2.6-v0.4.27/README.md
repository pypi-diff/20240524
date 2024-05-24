# Comparing `tmp/cellbrowser-1.2.6.tar.gz` & `tmp/cellbrowser-v0.4.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellbrowser-1.2.6.tar", last modified: Fri May 24 18:53:14 2024, max compression
+gzip compressed data, was "dist/cellbrowser-v0.4.27.tar", last modified: Mon Dec 17 16:26:39 2018, max compression
```

## Comparing `cellbrowser-1.2.6.tar` & `cellbrowser-v0.4.27.tar`

### file list

```diff
@@ -1,202 +1,124 @@
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/
--rwxrwxr-x   0 chmalee  (30024) genecats  (1305)    44506 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/hubmaker.py
--rwxrwxr-x   0 chmalee  (30024) genecats  (1305)    23637 2024-05-24 18:53:09.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/genes.py
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    14389 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/geneinfo.py
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/R/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    21294 2024-05-24 18:53:09.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/R/cellbrowser.R
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    25016 2024-01-26 18:30:04.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/seurat.py
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      917 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/tiny-queue.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     4595 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/slick.grid.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    60211 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/palette.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    16713 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/papaparse.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    16032 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/lz-string.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3365 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/FileSaver.1.1.20151003.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     6416 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jsurl2.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     7038 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/tablesort.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     8545 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/hamster.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    41928 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/spectrum.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    17797 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.event.drag-2.3.0.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     5057 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-submenu.min.css
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      160 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/browser.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      110 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/viridis.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     2673 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/README.md
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/example/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    32231 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/example/example.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      480 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/example/d3-random-matrix.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      350 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/example/package.json
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      717 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/example/gradients.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     2741 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/package.json
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      110 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/inferno.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      757 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/LICENSE
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      108 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/magma.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      226 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/build.js
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/utils/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      438 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/utils/rgb2hex.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      998 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/utils/interpolate.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      232 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/utils/hex2rgb.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)       13 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/.npmignore
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/rgb/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     8707 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/rgb/plasma.json
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     8709 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/rgb/magma.json
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     8707 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/rgb/viridis.json
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     8707 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/rgb/inferno.json
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/hex/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     2561 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/hex/plasma.json
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     2561 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/hex/viridis.json
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     2561 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/hex/inferno.json
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     2561 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/hex/magma.json
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      109 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/plasma.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      182 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/Makefile
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3823 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-dropmenu.min.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     9960 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/introjs.2.4.0.min.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    43247 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.sparkline.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    19452 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/OverlayScrollbars.min.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    23408 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/intro.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    10395 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/normalizeWheel.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     5791 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/slick.cellselectionmodel.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    10058 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/chosen.1.8.2.min.css
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/images/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3274 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_555555_256x240.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3262 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_777620_256x240.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3264 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_ffffff_256x240.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3266 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_777777_256x240.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)       86 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-bg_flat_0_aaaaaa_40x100.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3266 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_444444_256x240.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3262 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_cc0000_256x240.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   107817 2024-01-26 18:30:04.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.tablesorter.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    15196 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/select2.4.0.4.min.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     4772 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-submenu.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     1784 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/slick.cellrangedecorator.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3329 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/slick.examples.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     6668 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.contextMenu.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    30319 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/chartjs-chart-box-and-violin-plot.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    20835 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/split.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   106428 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/selectize.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     6516 2024-01-26 18:30:04.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/theme.bootstrap_3.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    45130 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/science.v1.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     4862 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/mousetrap.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   253668 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery-ui.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    14199 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/FastBitSet.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   121200 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.3.3.7.min.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   172843 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/slick.grid.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    29004 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/chosen.jquery.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    90609 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.contextMenu.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    66604 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/select2.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     5050 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/slick.cellrangeselector.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      538 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/chosen-sprite.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    11595 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/spectrum-1.8.0.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    27231 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/font-awesome.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    37045 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      541 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/tablesort.number.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     1802 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/slick.formatters.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)  1320211 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/minified.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    10947 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/selectize.bootstrap3.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   121155 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.min.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   211133 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/Chart.bundle.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    16723 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/slick.editors.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    14269 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/scaleColorPerceptual.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      777 2022-05-13 20:50:10.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/chosen-sprite@2x.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    64000 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/materialIcons.woff
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     1440 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.tipsy.1.0.3.min.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      494 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/googleMaterialIcons.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    41643 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.overlayScrollbars.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3447 2023-01-23 21:01:33.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/drawImage-clipper.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    23234 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/pako_inflate.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    86709 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.3.1.1.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   127111 2024-01-26 18:30:04.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.tablesorter.widgets.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     5855 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.ui.position.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     6845 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.tipsy.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    76717 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/reorder.v1.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    17618 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/slick.core.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    35973 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery-ui-1.12.1.css
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/js/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   110135 2024-05-24 18:53:09.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/js/maxPlot.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    19327 2024-01-26 18:30:04.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/js/maxHeat.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    66347 2024-05-24 18:53:09.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/js/cbData.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   356543 2024-05-24 18:53:09.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/js/cellBrowser.js
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      754 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/zoom.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      140 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/marker.png
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      386 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-gravity-west-24.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      455 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-rect-select-16.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     1612 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/README.txt
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      565 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-scale-16.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      443 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-rect-select-22.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     1047 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-info-24.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      615 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-merge-down-16.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      682 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-info-16.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      583 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/gtk-save.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      776 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-move-22.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      594 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-zoom-16.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      586 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-free-select-16.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      284 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/gtk-justify-left.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      561 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-controller-16.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      825 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-controller-24.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      646 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-center-16.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      598 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-move-16.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     1065 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-center-24.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      754 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-zoom-22.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      814 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-free-select-22.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)       27 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/log.txt
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      523 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-edit-16.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      776 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/move.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      814 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/lasso.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)       41 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/README.md
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      222 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/info.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      443 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/select.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      598 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/icons8-help-32.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     1065 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/center.png
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/css/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    68255 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/css/MaterialIcons-Regular.ttf
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    65874 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/css/MaterialIcons-Regular.woff2
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    16310 2024-05-24 18:53:09.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/css/cellBrowser.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    57620 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/css/MaterialIcons-Regular.woff
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    68260 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/css/MaterialIcons-Regular.eot
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/genes/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     2259 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/genes/makeGenes.py
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   691255 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/genes/hg38.json.gz
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      372 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/genes/files.json
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)  5012383 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/genes/hg19.gc34.tsv
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)  3666259 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/genes/mm10.vm25.tsv
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   592310 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/genes/mm10.json.gz
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)  5290936 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/genes/hg38.gc34.tsv
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      310 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/genes/log.txt
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   636974 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/genes/hg19.json.gz
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      126 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/__init__.py
--rwxrwxr-x   0 chmalee  (30024) genecats  (1305)   285505 2024-05-24 18:53:09.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cellbrowser.py
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/sampleConfig/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3112 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/sampleConfig/scanpy.conf
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     2166 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/sampleConfig/hub.conf
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     8524 2024-05-24 18:53:09.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/sampleConfig/cellbrowser.conf
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     2616 2024-05-24 18:53:09.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/sampleConfig/desc.conf
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      456 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/sampleConfig/summary.html
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      978 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/sampleConfig/seurat.conf
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    18221 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/download.py
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    31816 2024-05-24 18:53:09.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/convert.py
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      498 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser/_version.py
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/RangeHTTPServer/
--rwxrwxr-x   0 chmalee  (30024) genecats  (1305)      594 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/RangeHTTPServer/__main__.py
--rwxrwxr-x   0 chmalee  (30024) genecats  (1305)     3663 2022-05-13 19:19:20.000000 cellbrowser-1.2.6/src/cbPyLib/RangeHTTPServer/__init__.py
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser.egg-info/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)       28 2024-05-24 18:53:13.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser.egg-info/top_level.txt
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)        1 2022-05-13 21:01:59.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser.egg-info/not-zip-safe
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     1523 2024-05-24 18:53:13.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser.egg-info/PKG-INFO
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)        1 2024-05-24 18:53:13.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser.egg-info/dependency_links.txt
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      602 2024-05-24 18:53:13.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser.egg-info/entry_points.txt
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    10209 2024-05-24 18:53:13.000000 cellbrowser-1.2.6/src/cbPyLib/cellbrowser.egg-info/SOURCES.txt
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      614 2022-05-13 19:19:19.000000 cellbrowser-1.2.6/MANIFEST.in
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     7087 2024-05-24 18:53:09.000000 cellbrowser-1.2.6/README.rst
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    35147 2022-05-13 19:19:19.000000 cellbrowser-1.2.6/LICENSE
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      221 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/setup.cfg
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     1523 2024-05-24 18:53:14.000000 cellbrowser-1.2.6/PKG-INFO
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3207 2023-01-23 21:01:33.000000 cellbrowser-1.2.6/setup.py
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    68611 2022-05-13 19:19:21.000000 cellbrowser-1.2.6/versioneer.py
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/
+-rw-rw-r--   0 max       (1501) protein   (1304)     2234 2018-12-17 15:44:55.000000 cellbrowser-v0.4.27/setup.py
+-rw-rw-r--   0 max       (1501) protein   (1304)     1102 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/PKG-INFO
+-rw-rw-r--   0 max       (1501) protein   (1304)      994 2018-12-17 16:16:51.000000 cellbrowser-v0.4.27/README.rst
+-rw-rw-r--   0 max       (1501) protein   (1304)    68611 2018-12-07 13:51:58.000000 cellbrowser-v0.4.27/versioneer.py
+-rw-rw-r--   0 max       (1501) protein   (1304)      217 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/setup.cfg
+-rw-rw-r--   0 max       (1501) protein   (1304)      566 2018-12-07 13:51:59.000000 cellbrowser-v0.4.27/MANIFEST.in
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/
+-rwxrwxr-x   0 max       (1501) protein   (1304)      341 2018-11-21 10:54:55.000000 cellbrowser-v0.4.27/src/cbScanpy
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/RangeHTTPServer/
+-rwxrwxr-x   0 max       (1501) protein   (1304)     3663 2018-08-17 12:09:51.000000 cellbrowser-v0.4.27/src/cbPyLib/RangeHTTPServer/__init__.py
+-rwxrwxr-x   0 max       (1501) protein   (1304)      594 2018-08-17 12:09:51.000000 cellbrowser-v0.4.27/src/cbPyLib/RangeHTTPServer/__main__.py
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser.egg-info/
+-rw-rw-r--   0 max       (1501) protein   (1304)     5590 2018-12-17 16:26:38.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser.egg-info/SOURCES.txt
+-rw-rw-r--   0 max       (1501) protein   (1304)     1101 2018-12-17 16:26:38.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser.egg-info/PKG-INFO
+-rw-rw-r--   0 max       (1501) protein   (1304)        1 2018-12-17 16:26:38.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser.egg-info/dependency_links.txt
+-rw-rw-r--   0 max       (1501) protein   (1304)       28 2018-12-17 16:26:38.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser.egg-info/top_level.txt
+-rw-rw-r--   0 max       (1501) protein   (1304)      525 2018-12-17 16:26:38.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser.egg-info/entry_points.txt
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/html/
+-rw-rw-r--   0 max       (1501) protein   (1304)     2573 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/html/index.html
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/
+-rw-rw-r--   0 max       (1501) protein   (1304)     5855 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.ui.position.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)     9481 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/selectize.0.12.4.min.css
+-rw-rw-r--   0 max       (1501) protein   (1304)    15196 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/select2.4.0.4.min.css
+-rw-rw-r--   0 max       (1501) protein   (1304)   121155 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.min.css
+-rw-rw-r--   0 max       (1501) protein   (1304)    20835 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/split.js
+-rw-rw-r--   0 max       (1501) protein   (1304)      538 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/chosen-sprite.png
+-rw-rw-r--   0 max       (1501) protein   (1304)    29004 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/chosen.jquery.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    90609 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.contextMenu.js
+-rw-rw-r--   0 max       (1501) protein   (1304)      494 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/googleMaterialIcons.css
+-rw-rw-r--   0 max       (1501) protein   (1304)     3365 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/FileSaver.1.1.20151003.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    23408 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/intro.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)     6668 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.contextMenu.css
+-rw-rw-r--   0 max       (1501) protein   (1304)    23234 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/pako_inflate.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)     4862 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/mousetrap.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)     3823 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-dropmenu.min.css
+-rw-rw-r--   0 max       (1501) protein   (1304)     8545 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/hamster.js
+-rw-rw-r--   0 max       (1501) protein   (1304)   211133 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/Chart.bundle.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)     1440 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.tipsy.1.0.3.min.css
+-rw-rw-r--   0 max       (1501) protein   (1304)    35973 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery-ui-1.12.1.css
+-rw-rw-r--   0 max       (1501) protein   (1304)    10395 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/normalizeWheel.js
+-rw-rw-r--   0 max       (1501) protein   (1304)      541 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/tablesort.number.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)   253668 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery-ui.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)     4772 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-submenu.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    64000 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/materialIcons.woff
+-rw-rw-r--   0 max       (1501) protein   (1304)    16713 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/papaparse.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)     7038 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/tablesort.js
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/
+-rw-rw-r--   0 max       (1501) protein   (1304)     3262 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_cc0000_256x240.png
+-rw-rw-r--   0 max       (1501) protein   (1304)       86 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rw-rw-r--   0 max       (1501) protein   (1304)     3266 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_777777_256x240.png
+-rw-rw-r--   0 max       (1501) protein   (1304)     3262 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_777620_256x240.png
+-rw-rw-r--   0 max       (1501) protein   (1304)     3274 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_555555_256x240.png
+-rw-rw-r--   0 max       (1501) protein   (1304)     3264 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_ffffff_256x240.png
+-rw-rw-r--   0 max       (1501) protein   (1304)     3266 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_444444_256x240.png
+-rw-rw-r--   0 max       (1501) protein   (1304)    30319 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/chartjs-chart-box-and-violin-plot.js
+-rw-rw-r--   0 max       (1501) protein   (1304)     5057 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-submenu.min.css
+-rw-rw-r--   0 max       (1501) protein   (1304)    45139 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/selectize.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    41928 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/spectrum.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    11595 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/spectrum-1.8.0.css
+-rw-rw-r--   0 max       (1501) protein   (1304)    60211 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/palette.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    66604 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/select2.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    43247 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.sparkline.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    86709 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.3.1.1.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)     9960 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/introjs.2.4.0.min.css
+-rw-rw-r--   0 max       (1501) protein   (1304)   121200 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.3.3.7.min.css
+-rw-rw-r--   0 max       (1501) protein   (1304)    10058 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/chosen.1.8.2.min.css
+-rw-rw-r--   0 max       (1501) protein   (1304)    14199 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/FastBitSet.js
+-rw-rw-r--   0 max       (1501) protein   (1304)     6845 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.tipsy.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    27231 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/font-awesome.css
+-rw-rw-r--   0 max       (1501) protein   (1304)    37045 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.min.js
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/
+-rw-rw-r--   0 max       (1501) protein   (1304)      443 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/select.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      140 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/marker.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      814 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/lasso.png
+-rw-rw-r--   0 max       (1501) protein   (1304)     1065 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/center.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      776 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/move.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      754 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/zoom.png
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/
+-rw-rw-r--   0 max       (1501) protein   (1304)     1612 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/README.txt
+-rw-rw-r--   0 max       (1501) protein   (1304)      615 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-merge-down-16.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      565 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-scale-16.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      586 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-free-select-16.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      561 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-controller-16.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      583 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/gtk-save.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      825 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-controller-24.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      594 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-zoom-16.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      284 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/gtk-justify-left.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      754 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-zoom-22.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      443 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-rect-select-22.png
+-rw-rw-r--   0 max       (1501) protein   (1304)     1047 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-info-24.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      646 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-center-16.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      523 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-edit-16.png
+-rw-rw-r--   0 max       (1501) protein   (1304)       27 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/log.txt
+-rw-rw-r--   0 max       (1501) protein   (1304)      682 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-info-16.png
+-rw-rw-r--   0 max       (1501) protein   (1304)     1065 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-center-24.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      386 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-gravity-west-24.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      455 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-rect-select-16.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      598 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-move-16.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      776 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-move-22.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      814 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-free-select-22.png
+-rw-rw-r--   0 max       (1501) protein   (1304)       41 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/README.md
+-rw-rw-r--   0 max       (1501) protein   (1304)      222 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/info.png
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/css/
+-rw-rw-r--   0 max       (1501) protein   (1304)     9258 2018-12-06 15:18:38.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/css/cellBrowser.css
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/js/
+-rw-rw-r--   0 max       (1501) protein   (1304)   160782 2018-12-12 16:03:21.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/js/cellBrowser.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    24701 2018-10-28 23:47:29.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/js/cbData.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    64150 2018-10-29 00:23:00.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/js/maxPlot.js
+-rwxrwxr-x   0 max       (1501) protein   (1304)    36845 2018-11-28 12:06:04.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/hubmaker.py
+-rwxrwxr-x   0 max       (1501) protein   (1304)     3597 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/guessgenes.py
+-rw-rw-r--   0 max       (1501) protein   (1304)      126 2018-12-07 13:51:59.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/__init__.py
+-rw-rw-r--   0 max       (1501) protein   (1304)    16960 2018-12-17 15:08:51.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/seurat.py
+-rw-rw-r--   0 max       (1501) protein   (1304)    17914 2018-12-17 13:09:30.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/convert.py
+-rw-rw-r--   0 max       (1501) protein   (1304)      499 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/_version.py
+-rwxrwxr-x   0 max       (1501) protein   (1304)   128622 2018-12-07 16:05:22.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cellbrowser.py
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/sampleConfig/
+-rw-rw-r--   0 max       (1501) protein   (1304)      697 2018-11-15 11:23:14.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/sampleConfig/seurat.conf
+-rw-rw-r--   0 max       (1501) protein   (1304)     3641 2018-11-23 18:46:31.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/sampleConfig/cellbrowser.conf
+-rw-rw-r--   0 max       (1501) protein   (1304)     2129 2018-12-06 16:01:46.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/sampleConfig/scanpy.conf
+-rw-rw-r--   0 max       (1501) protein   (1304)    15089 2018-11-29 15:25:30.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/geneinfo.py
```

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/hubmaker.py` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/hubmaker.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,136 +1,102 @@
 # create a track hub from an expression matrix
 
-import subprocess, colorsys, hashlib
+import subprocess, colorsys
 import logging, sys, optparse, re, unicodedata, string, glob, distutils.spawn, gzip
 from collections import defaultdict, namedtuple
-from os.path import join, basename, dirname, isfile, isdir, splitext, abspath
+from os.path import join, basename, dirname, isfile, isdir, splitext
 import os
 
 import sys
-from .cellbrowser import setDebug, lineFileNextRow, getSizesFname, readGeneSymbols, parseGeneLocs
-from .cellbrowser import MatrixTsvReader, runCommand, copyPkgFile, loadConfig, iterItems, getStaticFile
-from .cellbrowser import errAbort, getConfig, getAliasFname, makeDir
-
-CBEMAIL = os.getenv("CBEMAIL", None)
-
-# We do not require numpy but numpy is around 30-40% faster in processing arrays
-# So use it if it's present
-numpyLoaded = True
-try:
-    import numpy as np
-except:
-    numpyLoaded = False
-    logging.debug("Numpy could not be loaded. This is fine but matrix conversion may be 2/3 slower.")
-#numpyLoaded = False
+import cellbrowser
+
+CBEMAIL = os.getenv("CBEMAIL", "unknown")
 
 # ==== functions =====
     
 def cbHub_parseArgs():
     " setup logging, parse command line arguments and options. -h shows auto-generated help page "
     parser = optparse.OptionParser("""usage: %prog [options] - create a UCSC track hub for a single cell dataset
 
-    Run the program with "--init" to write a sample hub.conf into the current directory.
-    Adapt this file to your needs.
+    Run the program with "--init" to write a sample cellbrowser.conf into the current directory.
+    Adapt this file to your needs. For %prog, only the parts under "hub" are relevant.
 
-    Call the program like this if there is hub.conf in the current dir:
-    %prog -o hub
-    It will read hub.conf, create hub/hub.txt and write the job scripts.
+    Call the program without any arguments if there is cellbrowser.conf in the current dir:
+    %prog
+    It will read cellbrowser.conf, create hub.txt and write the job scripts.
     You can then run the job scripts as described below.
 
+    This will create one shell script per cell cluster, with names like 'job-xxx.sh',
+    in the current directory. To run these scripts in parallel on a big server,
+    e.g. with 10 processes use the Unix command "parallel":
+      ls *.sh | parallel -j 10 bash
+
+    Each job will write a log of stdout/stderr to files named e.g. job-1.log
+
+    Requirements that have to be installed on this machine with binaries in PATH:
+    - samtools https://github.com/samtools/samtools
+    - wiggletools https://github.com/Ensembl/WiggleTools
+    - intronProspector https://github.com/diekhans/intronProspector
+    - UCSC tools wigToBigWig, bedToBigBed from http://hgdownload.soe.ucsc.edu/admin/exe/
+
     Run the UCSC tool hubCheck on the resulting hub.txt to make sure that all jobs
     have successfully completed.
 
-    You can override some settings from cellbrowser.conf with command line options:
-    %prog -m meta.tsv -c Cluster -m exprMatrix.tsv.gz -o hub
-
-    ONLY if 'bamDir' has been specified in cellbrowser.conf:
-      | %prog will create one shell script per cell cluster, with names like 'job-xxx.sh',
-      | in the current directory. To run these scripts in parallel on a big server,
-      | e.g. with 10 processes use the Unix command "parallel":
-      |   ls *.sh | parallel -j 10 bash
-      | Each job will write a log of stdout/stderr to files named e.g. job-1.log
-      | Requirements that have to be installed on this machine with binaries in PATH:
-      | - samtools https://github.com/samtools/samtools
-      | - wiggletools https://github.com/Ensembl/WiggleTools
-      | - intronProspector https://github.com/diekhans/intronProspector
-      | - UCSC tools wigToBigWig, bedToBigBed, chromToUcsc from http://hgdownload.soe.ucsc.edu/admin/exe/
-      |
-      | To link meta.tsv with bamDir files:
-      | The cellId from meta.tsv will be used to try to find the BAM file in bamDir,
-      | by stripping off .bam and/or using just the file name before the first dot.
-    Otherwise:
-      - %prog requires bedToBigBed in the current PATH, see http://hgdownload.soe.ucsc.edu/admin/exe/
+    You can override some settings in cellbrowser.conf with the command line options:
+    %prog -m metaFname -c clusterField -m exprMatrix -o hubDir
     """)
 
     parser.add_option("", "--init", dest="init", action="store_true", \
-            help="write a sample hub.conf to the current directory")
+            help="write a sample cellbrowser.conf to the current directory")
 
     parser.add_option("-i", "--inConf", dest="inConf", action="store", \
-            help="a hub.conf input file to read all options from. (settings can also be specified via cellbrowser.conf in the current directory.) default %default", \
-            default = "hub.conf")
+            help="a cellbrowser.conf input file to read all options from, default %default", \
+            default = "cellbrowser.conf")
 
     #parser.add_option("-g", "--genome", dest="genome", action="store", \
             #help="a ucsc assembly identifier, like hg19, hg38 or mm10")
 
     parser.add_option("-m", "--metaFname", dest="meta", action="store", \
             help="a csv or tsv matrix, one row per cell")
 
     parser.add_option("-e", "--exprMatrix", dest="exprMatrix", action="store", \
             help="exprMatrix is a tsv or csv expression matrix, one line per cell")
 
     parser.add_option("-c", "--clusterField", dest="clusterField", action="store", \
             help="field in expr matrix that contains the cluster name")
 
-    parser.add_option("-o", "--outDir", dest="outDir", action="store", \
+    parser.add_option("-o", "--hubDir", dest="hubDir", action="store", \
             help="the output directory for the hub, default is %default")
 
-    parser.add_option("", "--stat", dest="stat", action="store", \
-            help="how to summarize data values of a cluster, one of: median, mean, percentile, nonzero. default is %default", default="median")
-
-    parser.add_option("", "--perc", dest="percentile", action="store", \
-            help="if stat is 'percentile', which percentile to use. a number 0-100. default is %default", default=90,
-            type='int')
-
     parser.add_option("-d", "--debug", dest="debug", action="store_true", help="show debug messages")
     #parser.add_option("", "--fixDot", dest="fixDot", action="store_true", help="replace dots in cell meta IDs with dashes (for R)")
     #parser.add_option("-t", "--geneType", dest="geneType", help="type of gene IDs in expression matrix. values like 'symbols', or 'gencode22', 'gencode28' or 'gencode-m13'.")
     #parser.add_option("", "--bamDir", dest="bamDir", help="directory with BAM files, one per cell. Merges small BAM files into one per cell cluster.")
-    #parser.add_option("", "--clusterOrder", dest="clusterOrder", help="file with cluster names in the order that they should appear in the track. default is alphabetical order.")
+    parser.add_option("", "--clusterOrder", dest="clusterOrder", help="file with cluster names in the order that they should appear in the track. default is alphabetical order.")
     parser.add_option("-s", "--skipBarchart", dest="skipBarchart", help="do not create the bar chart graph", action="store_true")
     #parser.add_option("", "--name", dest="name", help="name of track hub.")
     #parser.add_option("", "--email", dest="email", help="contact email for track hub. Default is %default, taken from the env. variable CBEMAIL", default=CBEMAIL)
     #parser.add_option("-f", "--file", dest="file", action="store", help="run on file") 
     #parser.add_option("", "--test", dest="test", action="store_true", help="do something") 
     (options, args) = parser.parse_args()
 
-    #if not options.exprMatrix and not isfile(options.inConf) and not options.init :
-    if not options.outDir and not options.init:
+    if not options.exprMatrix and not isfile(options.inConf) and not options.init:
         parser.print_help()
         exit(1)
 
-    setDebug(options.debug)
+    cellbrowser.setDebug(options.debug)
     return args, options
 
 def parseClustersFromMeta(metaFname, clusterFieldName, fixDot):
     " parse cluster -> cellId assignment from meta file, return as dict clusterName -> list of cellIds "
     logging.info("Parsing and using first field as the cell ID in file %s" % metaFname)
-
-    # in some scripts, meta.tsv has only two columns and no headers. Use stupid heuristics to detect this
-    noHeader = False
-    for row in lineFileNextRow(metaFname):
-        if len(row)==2 and not row[0]=="" and not "ell" in row[0] and not "rcode" in row[0]:
-            noHeader = True
-        break
-
     clusterToCells = defaultdict(list)
     metaCellIds = set()
     skipCount = 0
-
-    for row in lineFileNextRow(metaFname, noHeaders=noHeader):
+    for row in cellbrowser.lineFileNextRow(metaFname):
         clusterName = row._asdict()[clusterFieldName]
         cellId = row[0]
         if fixDot:
             cellId = cellId.replace(".", "-")
 
         # skip all cells assigned to the "" cluster
         if clusterName=="":
@@ -159,55 +125,18 @@
 email %s
 descriptionUrl hub.txt
 
 genome %s
 
 """ % (hubName, hubName, email, db))
 
-def writeBarChartDesc(hubDir, hubName, hubUrl, refHtmlFname):
-    " write the desc. html pages for the barchart track "
-    htmFname = join(hubDir, "barChart.html")
-    ofh = open(htmFname, "w")
-
-    hubBase = hubUrl.rsplit("/")[0]
-    refHtml = ""
-    if refHtmlFname is not None:
-        refHtml = open(refHtmlFname).read()
-
-    ofh.write("""
-<h2>Description</h2>
-<p>This track shows the median value of expression, for all cells from each cell cluster.
-
-<h2>Display Conventions and Configuration</h2>
-<p>This track is a <a href='https://genome.ucsc.edu/goldenPath/help/barChart.html'>barChart Graph</a> track.
-
-<h2>Methods</h2>
-<p>The annotation files that associate cells to cluster names were parsed. Then the expression matrix was read.
-For each gene, the expresssion values for all cells from a cluster were read and sorted.
-The median of this sorted list was written to a bigBed file.</p>
-
-<h2>Data Access</h2>
-<p>The bigBed file can be downloaded from the <a href='{hubBase}'>track hub directory</a>.</p>
-
-<h2>Credits</h2>
-<p>Thanks for the authors of the dataset for making their data available.</p>
-
-<h2>References</h2>
-<p>
-{refHtml}
-</p>""".format(**locals()))
-
-    ofh.close()
-
-def writeBamDescPages(hubDir, hubName, hubUrl, refHtmlFname):
-    " write the desc. html pages for the bam-related tracks "
+def writeDescPages(hubDir, hubName, hubUrl, refHtmlFname):
     saneHubName = sanitizeName(hubName)
     readDesc = join(hubDir, saneHubName+".html")
     readFh = open(readDesc, "w")
-
     hubBase = hubUrl.rsplit("/")[0]
     refHtml = ""
     if refHtmlFname is not None:
         refHtml = open(refHtmlFname).read()
 
     readFh.write("""
 <h2>Description</h2>
@@ -338,15 +267,15 @@
     if progPath==None:
         errAbort("Cannot find program '%s' in PATH." % name)
     return progPath
 
 def writeJobScript(jobFn, cmds):
     " write commands to a shell script with file name "
     jobFh = open(jobFn, "w")
-    logFname = splitext(basename(jobFn))[0]+'.log'
+    logFname = splitext(jobFn)[0]+'.log'
 
     jobFh.write("#!/bin/bash\n")
     jobFh.write("set -e # = abort on error\n")
     jobFh.write("set -o pipefail # = even in pipes\n")
     jobFh.write("echo Job %s start, stdout/stderr go to %s\n" % (jobFn, logFname))
     jobFh.write("exec 1> %s\n" % logFname)
     jobFh.write("exec 2>&1\n");
@@ -416,15 +345,15 @@
     yield cellId4.replace("_R1", "").replace("_R2", "")
 
 def findBams(bamDir, clusterToCells):
     """
     create dict with cluster -> (cellIds, bamFnames)
     """
     metaCellIds = set()
-    for cluster, cellIds in iterItems(clusterToCells):
+    for cluster, cellIds in clusterToCells.iteritems():
         for cellId in cellIds:
             metaCellIds.add(cellId)
 
     bamMask =join(bamDir, "*.bam")
     logging.info("Getting list of BAM files matching %s" % bamMask)
     bamPaths = glob.glob(bamMask)
     bamPaths.sort()
@@ -454,15 +383,15 @@
             cellIdToBamFnames[cellId].append(bamPath)
 
     clusterBams = dict()
 
     #logging.info("Got %s BAM files and %s cell ids in the meta data" % (len(metaCellIds), len(cellIdToBamFnames)))
 
     emptyClusterCount = 0
-    for clusterName, cellIds in iterItems(clusterToCells):
+    for clusterName, cellIds in clusterToCells.iteritems():
 
         bamFnames = []
         for cellId in cellIds:
             cellBams = cellIdToBamFnames[cellId]
             bamFnames.extend(cellBams)
 
         if len(bamFnames)==0:
@@ -495,15 +424,15 @@
     ofh.write("#cellId\thasMeta\tcluster\tbamFname1\tbamFname2OrMore\n")
 
     allMetaCellIds = set(allMetaCellIds)
 
     allCellIds = set(allMetaCellIds).union(cellIdToBams)
 
     cellToCluster = {}
-    for clusterName, (cellIds, bamFnames) in iterItems(clusterBams):
+    for clusterName, (cellIds, bamFnames) in clusterBams.iteritems():
         for cellId in cellIds:
             cellToCluster[cellId] = clusterName
 
     for cellId in allCellIds:
         ofh.write(cellId+"\t")
 
         if cellId in allMetaCellIds:
@@ -537,34 +466,30 @@
     logging.info("*** Merging and analyzing BAM files")
 
     clusterBams, allMetaCellIds, cellIdToBams = findBams(bamDir, clusterToCells)
 
     idReportFname = join(outDir, "metaBamMatch.txt")
     cellCount = writeDebugReport(allMetaCellIds, cellIdToBams, clusterBams, idReportFname)
 
-    jobsDir = join(outDir, "jobs")
-    outDir = abspath(outDir)
+    jlFh = open("jobList", "w")
 
-    makeDir(join(jobsDir, "jobs"))
-    jlFh = open(join(jobsDir, "jobList"), "w")
-
-    for clusterName, (cellIds, bamFnames) in iterItems(clusterBams):
+    #cellCount = 0
+    for clusterName, (cellIds, bamFnames) in clusterBams.iteritems():
         uniqueCellIds = set(cellIds)
         #cellCount += len(uniqueCellIds)
 
     logging.info("Merging BAM files and writing hub")
     saneHubName = sanitizeName(hubName)
     writeParentStanzas(tfh, saneHubName, hubName, cellCount)
 
-    chromSizes = getSizesFname(db)
-    aliasTable = getAliasFname(db)
+    chromSizes = cellbrowser.getSizesFname(db)
 
     jobNo = 0
     emptyClusterCount = 0
-    for clusterName, (cellIds, bamFnames) in iterItems(clusterBams):
+    for clusterName, (cellIds, bamFnames) in clusterBams.iteritems():
         saneClusterName = sanitizeName(clusterName)
         logging.info("Processing cluster %s, %d cellIds/BAM files, examples: %s" % (clusterName, len(cellIds), cellIds[0]))
         cmds = []
 
         outBam = join(outDir, saneClusterName+".bam")
         outStat = join(outDir, saneClusterName+".stats.txt")
         outCalls = join(outDir, saneClusterName+".calls.tsv")
@@ -578,16 +503,14 @@
         intronBb = intronBed.replace(".bed", ".bb")
 
         cmd = "echo merging %d bam files for %d cell IDs" % (len(bamFnames), len(set(cellIds)))
         cmds.append(cmd)
 
         intronProspector = findProgram("intronProspector")
         samtools = findProgram("samtools")
-        bamFnames = [join("..", "..", fn) for fn in bamFnames]
-
         if len(bamFnames)==1:
             # samtools merge aborts if only one input BAM file
             cmd = "cat %s " % (bamFnames[0])
         else:
             # -r construct read groups
             # -f overwrite output files if needed
             cmd = samtools+" merge -f -r - %s " % (" ".join(bamFnames))
@@ -602,18 +525,18 @@
 
         # XX could be part of the samtools merge command, in a pipe
         #cmds.append(cmd)
 
         cmd = "samtools index %s" % outBam
         cmds.append(cmd)
 
-        cmd = """export LC_COLLATE=C; cat %s | awk '($5>1000) {$5=1000;} { OFS="\\t"; print}' | chromToUcsc -a %s | sort -k1,1 -k2,2n > %s""" % (junctionBed, aliasTable, junctionBedSorted)
+        cmd = """export LC_COLLATE=C; cat %s | awk '($5>1000) {$5=1000;} { OFS="\\t"; print}'  | sort -k1,1 -k2,2n > %s""" % (junctionBed, junctionBedSorted)
         cmds.append(cmd)
 
-        cmd = """export LC_COLLATE=C; cat %s | awk '($5>1000) {$5=1000;} { OFS="\\t"; print}' | chromToUcsc -a %s | sort -k1,1 -k2,2n > %s""" % (intronBed, aliasTable, intronBedSorted)
+        cmd = """export LC_COLLATE=C; cat %s | awk '($5>1000) {$5=1000;} { OFS="\\t"; print}' | sort -k1,1 -k2,2n > %s""" % (intronBed, intronBedSorted)
         cmds.append(cmd)
 
         bigBed = findProgram("bedToBigBed")
         cmd = bigBed+" %s %s %s -type=bed6 -tab" % (intronBedSorted, chromSizes, intronBb)
         cmds.append(cmd)
 
         cmd = bigBed+" %s %s %s -type=bed12 -tab" % (junctionBedSorted, chromSizes, junctionBb)
@@ -625,32 +548,33 @@
         cmds.append(cmd)
 
         wiggletools = findProgram("wiggletools")
         outWig = join(outDir, saneClusterName+".wig")
         outBw = join(outDir, saneClusterName+".bw")
         # fix up the chrom field and the chrom=xxx stepSize fields
         # For wiggle files with Ensembl chrom names, we need UCSC chrom names
-        cmd = wiggletools+ """ coverage %s | chromToUcsc -a %s > %s""" % (outBam, aliasTable, outWig)
+        cmd = wiggletools+ """ coverage %s | awk '($1 ~ /^[0-9XYM]/ && (NF==4)) { if ($1=="MT") {$1="M"}; $1="chr"$1 } ($2 ~ /^chrom=[0-9XYM]/) {split($2,a, "="); if (a[2]=="MT") {a[2]="M"}; $2="chrom=chr"a[2]} // {OFS=" "; print}' > %s""" % (outBam, outWig)
         cmds.append(cmd)
 
         wigToBigWig = findProgram("wigToBigWig")
         # -clip also means to not check the sequence names against chrom.sizes anymore
         # clip is needed so GL and KI seqs in hg38 don't mess up the conversion
         cmd = wigToBigWig+ " %s %s %s -clip" % (outWig, chromSizes, outBw)
         cmds.append(cmd)
 
         cmd = "rm -f %s %s %s" % (outWig, intronBedSorted, junctionBedSorted)
         cmds.append(cmd)
 
+        #if False:
         if isfile(outBw):
             logging.info("Not running anything for %s, file %s already exists" % (saneClusterName, outBw))
         else:
-            jobFn = join(jobsDir, "job-%d.sh" % jobNo)
+            jobFn = "job-%d.sh" % jobNo
             writeJobScript(jobFn, cmds)
-            jlFh.write("/bin/bash %s {check out exists %s}\n" % (basename(jobFn), outBw))
+            jlFh.write("/bin/bash %s {check out exists %s}\n" % (jobFn, outBw))
         jobNo+=1
 
         writeTdbStanzas(tfh, clusterName, saneHubName, len(cellIds))
 
     if emptyClusterCount==len(clusterToCells):
         logging.error("No single BAM file could be linked to the meta data. Please check the identifiers in the meta data table against the file names in %s." % (bamDir))
         sys.exit(1)
@@ -665,45 +589,41 @@
 
 def toHex(rgb):
     r = rgb[0]
     g = rgb[1]
     b = rgb[2]
     return "#{0:02x}{1:02x}{2:02x}".format(clamp(r*255), clamp(g*255), clamp(b*255))
 
-def writeBarChartTdb(tfh, bbFname, clusterNames, unitName, stat, percentile):
+def writeBarChartTdb(tfh, bbFname, clusterNames, unitName):
     " write the barChart tdb stanza "
     stepSize = 1.0 / len(clusterNames)
     colorCodes = []
     x = 0
     while x < 1.0:
         colorCodes.append(colorsys.hsv_to_rgb(x, 1.0, 1.0))
         x+=stepSize
 
     hexCodes = [toHex(x) for x in colorCodes]
 
     tfh.write('track barChart\n')
     tfh.write('type bigBarChart\n')
     tfh.write('visibility full\n')
     tfh.write('shortLabel Cluster expression\n')
-    if stat=="percentile":
-        metric = "%dth percentile" % percentile
-    else:
-        metric = stat.capitalize()
-    tfh.write('longLabel %s Cluster expression\n' % metric)
+    tfh.write('longLabel Median Cluster expression\n')
 
     # only remove spaces, this is more readable than sanitizeName
     saneClusterNames = []
     for cn in clusterNames:
         cn = cn.replace(" ", "_")
         #cn = ''.join(ch for ch in newName if (ch.isalnum() or ch=="_"))
         saneClusterNames.append(cn)
 
     tfh.write('barChartBars %s\n' % " ".join(saneClusterNames))
     tfh.write('barChartColors %s\n' % " ".join(hexCodes))
-    tfh.write('barChartMetric %s\n' % metric)
+    tfh.write('barChartMetric median\n')
     tfh.write('barChartUnit %s\n' % unitName)
     tfh.write('barChartMatrixUrl exprMatrix.tsv\n')
     tfh.write('barChartSampleUrl clusters.tsv\n')
     tfh.write('defaultLabelFields name2\n')
     tfh.write('labelFields name2,name\n')
     tfh.write('bigDataUrl barChart.bb\n\n')
 
@@ -713,231 +633,178 @@
     # with the 'title' method and join them together.
     return components[0] + ''.join(x.title() for x in components[1:])
 
 def sanitizeName(name):
     " remove all nonalpha chars and camel case name "
     newName = to_camel_case(name.replace(" ", "_"))
     newName = ''.join(ch for ch in newName if (ch.isalnum() or ch=="_"))
-    if len(newName)>80: # genome browser is limited to 128 chars
-        md5 = hashlib.md5(newName.encode('utf-8')).hexdigest()[:10]
-        newName = newName[:30]+"_"+newName[-30:]+"_"+md5
-
     return newName
 
 def writeCatFile(clusterToCells, catFname):
     " write file with cellId<tab>clusterName "
     logging.info("Writing %s" % catFname)
     ofh = open(catFname, "w")
-    for clusterName, cellIds in iterItems(clusterToCells):
+    for clusterName, cellIds in clusterToCells.iteritems():
         for cellId in cellIds:
             ofh.write("%s\t%s\n" % (cellId, clusterName))
     ofh.close()
 
-def makeClusterCellIdxArray(clusterOrder, clusterToCells, cellNames, clusterFname):
-    """
-    make a list of lists of cellIds, one per cluster, in the right order.
-    Result is an array (one element per cluster), with each inside array the list of cell indices of this cluster.
-    also write the cluster names to clusterFname
+def makeBarGraphBigBed(genome, inMatrixFname, outMatrixFname, geneType, clusterToCells, \
+        clusterOrder, clusterFname, bbFname):
+    """ create a barGraph bigBed file for an expression matrix
+    clusterToCells is a dict clusterName -> list of cellIDs
+    clusterOrder is a list of the clusterNames in the right order
     """
+    logging.info("*** Creating barChartGraph bigbed file")
+    if geneType.startswith("symbol"):
+        # create a mapping from symbol -> gene locations
+        if "/" in geneType:
+            defGenes = geneType.split("/")[1]
+        elif genome=="hg38":
+            defGenes = "gencode24"
+        elif genome=="hg19":
+            defGenes = "gencode19"
+        elif genome=="mm10":
+            defGenes = "gencode-m13"
+        else:
+            errAbort("Unclear how to map symbols to genome for db %s. Please adapt cellbrowser.py" % genome)
+
+        logging.info("Using %s to map symbols to genome" % defGenes)
+
+        geneToSym = cellbrowser.readGeneSymbols({'geneIdType':defGenes})
+        geneLocsId = cellbrowser.parseGeneLocs(defGenes)
+        geneLocs = {}
+        for geneId, locs in iterItems(geneLocsId):
+            sym = geneToSym[geneId]
+            geneLocs[sym] = locs
+    else:
+        geneToSym = cellbrowser.readGeneSymbols({'geneIdType':geneType})
+        geneLocs = cellbrowser.parseGeneLocs(geneType)
+
+    matOfh = open(outMatrixFname, "w")
     clustOfh = open(clusterFname, "w")
-    allCellIds = range(0, len(cellNames))
-    cellNameToId = dict(zip(cellNames, allCellIds))
 
+    mr = cellbrowser.MatrixTsvReader()
+    mr.open(inMatrixFname)
+    matType, cellNames = mr.matType, mr.sampleNames
+
+    cellIds = range(0, len(cellNames))
+    cellNameToId = dict(zip(cellNames, cellIds))
+
+    # make a list of lists of cellIds, one per cluster, in the right order
     clusterCellIds = [] # list of tuples with cell-indexes, one per cluster
     allCellNames = [] # list for cellIds, with a matrix, meta and with bam file
     allCellIndices = [] # position of all cellIds in allCellNames
-    notInMat = []
     for clusterName in clusterOrder:
         cellIdxList = []
         for cellName in clusterToCells[clusterName]:
             if cellName not in cellNameToId:
-                #logging.warn("%s is in meta but not in expression matrix." % cellName)
-                notInMat.append(cellName)
+                logging.warn("%s is in meta but not in expression matrix." % cellName)
                 continue
             idx = cellNameToId[cellName]
             cellIdxList.append(idx)
             allCellNames.append(cellName)
             allCellIndices.append(idx)
             sanClusterName = clusterName.replace(" ", "_")
             clustOfh.write("%s\t%s\n" % (cellName, sanClusterName))
 
         if len(cellIdxList)==0:
             logging.warn("No cells assigned to cluster %s" % clusterName)
 
-        if numpyLoaded:
-            cellIds = np.array(cellIdxList)
-        else:
-            cellIds = tuple(cellIdxList)
-
-        clusterCellIds.append(cellIdxList)
-
+        clusterCellIds.append(tuple(cellIdxList))
     clustOfh.close()
 
-    if len(notInMat)!=0:
-        logging.warn("%d identifiers from the meta file are not in the expression matrix. Examples: %s" % (len(notInMat), notInMat[:10]))
-
-    return clusterCellIds, allCellNames, allCellIndices
-
-def makeBarGraphBigBed(genome, inMatrixFname, outMatrixFname, geneType, geneModel, clusterToCells, \
-        clusterOrder, stat, percentile, clusterFname, bbFname):
-    """ create a barGraph bigBed file for an expression matrix
-    clusterToCells is a dict clusterName -> list of cellIDs
-    clusterOrder is a list of the clusterNames in the right order
-    """
-    logging.info("Creating barChartGraph bigbed file: genome %s, geneType %s, geneModel %s" % (genome, geneType, geneModel))
-    geneToSym = readGeneSymbols(geneType, inMatrixFname)
-    if geneToSym is None:
-        geneToSym = readGeneSymbols("gencode-human", inMatrixFname)
-        symToGene = {v: k for k, v in geneToSym.items()} # invert the dictionary key->value to value->key
-        geneToSym = None
-
-    geneLocs = parseGeneLocs(genome, geneModel)
-
-    matOfh = open(outMatrixFname, "w")
-
-    mr = MatrixTsvReader(geneToSym)
-    mr.open(inMatrixFname)
-    matType, cellNames = mr.matType, mr.sampleNames
-
-    clusterCellIds, allCellNames, allCellIndices = \
-            makeClusterCellIdxArray(clusterOrder, clusterToCells, cellNames, clusterFname)
-
     # write header line
     matOfh.write("#gene\t")
     matOfh.write("\t".join(allCellNames))
     matOfh.write("\n")
 
     # make the barchart bed file. format:
     # chr14 95086227 95158010 ENSG00000100697.10 999 - DICER1 5 10.94,11.60,8.00,6.69,4.89 93153 26789
     #bedFname = join(outDir, "barchart.bed")
     bedFname = bbFname.replace(".bb", ".bed")
     assert(bedFname!=bbFname)
 
     bedFh = open(bedFname, "w")
 
-    geneCount = 0
     skipCount = 0
     for geneId, sym, exprArr in mr.iterRows():
-        logging.debug("Writing BED and matrix line for %s, symbol %s, %d expr values" % (geneId, sym, len(exprArr)))
+        logging.debug("Writing BED and matrix line for %s" % geneId)
 
-        if geneType.startswith("symbol"):
-            # input has symbols
-            if symToGene and geneId not in symToGene:
-                logging.warn("Cannot resolve symbol %s to a gene accession" % geneId)
-                continue
-            else:
-                geneId = symToGene[geneId]
-                bedRows = geneLocs[geneId]
-        else:
-            # input has accessions
-            if geneId not in geneLocs:
-                geneId2 = geneId.replace(".", "-", 1) # does this make sense? (for R)
-                if geneId2 not in geneLocs:
-                    logging.warn("Cannot place gene '%s' onto genome, dropping it" % geneId)
-                    skipCount += 1
-                    continue
-                else:
-                    geneId = geneId2
-            bedRows = geneLocs[geneId]
-
-        # write the new matrix row first field
+        # write the new matrix row
         offset = matOfh.tell()
-        rowHeader = "%s\t" % (sym)
+        rowHeader = "%s\t" % (geneId)
         matOfh.write(rowHeader)
 
-        # write the new matrix row values
         newRow = []
         for idx in allCellIndices:
             newRow.append(str(exprArr[idx]))
-
         newLine = "\t".join(newRow)
         matOfh.write(newLine)
         matOfh.write("\n")
         lineLen = len(geneId)+len(newLine)+2 # include tab and newline
 
-        bedScore = 0
-
         medianList = []
+
         for cellIds in clusterCellIds:
-            if not numpyLoaded:
-                assert(False) # XXX at the moment, I require numpy
-                exprList = []
-                for cellId in cellIds:
-                    exprList.append(exprArr[cellId])
-                n = len(cellIds)
-
-                if stat=="median":
-                    if len(exprList)==0:
-                        summVal = 0
-                    else:
-                        summVal = sorted(exprList)[n//2] # approx OK, no special case for even n's
-                elif stat=="mean":
-                    summVal = float(sum(exprList))/len(exprList)
-                elif stat=="percentile":
-                    summVal = sorted(exprList)[int(percentile/100.0*len(exprList))] # did not check this against numpy
-                elif stat=="nonzero":
-                    summVal = float(len([x for x in exprList if x!=0])) / len(exprList)
+            exprList = []
+            for cellId in cellIds:
+                exprList.append(exprArr[cellId])
+            n = len(cellIds)
+            if len(exprList)==0:
+                median = 0
             else:
-                clusterExprs = np.take(exprArr, cellIds)
-                if stat=="median":
-                    summVal = np.median(clusterExprs)
-                elif stat=="mean":
-                    summVal = np.mean(clusterExprs)
-                elif stat=="percentile":
-                    summVal = np.percentile(clusterExprs, percentile)
-                elif stat=="nonzero":
-                    summVal = np.count_nonzero(clusterExprs) / float(clusterExprs.size)
-
-            medianList.append(str(summVal))
-
+                median = sorted(exprList)[n//2] # approx OK, no special case for even n's
+            medianList.append(str(median))
+            bedScore = len([x for x in exprList if x!=0]) # score = non-zero medians
+            bedScore = min(1000, bedScore)
+
+        if geneId not in geneLocs:
+            geneId2 = geneId.replace(".", "-", 1) # does this make sense? (for R)
+            if geneId2 not in geneLocs:
+                logging.warn("Cannot place gene '%s' onto genome, dropping it" % geneId)
+                skipCount += 1
+                continue
+            else:
+                geneId = geneId2
 
-        geneCount += 1
+        bedRows = geneLocs[geneId]
 
         # one geneId may have multiple placements, e.g. Ensembl's rule for duplicate genes
         for bedRow in bedRows:
-            #if geneToSym!=None:
-                #sym = geneToSym.get(geneId, geneId)
-            #else:
-                #sym = geneId
+            sym = geneToSym.get(geneId, geneId)
             bedRow[4] = str(bedScore) # 4 = score field
-            bedRow[3] = sym
-            bedRow.append(geneId)
+            bedRow.append(sym)
             bedRow.append(str(len(medianList)))
             bedRow.append(",".join(medianList))
             bedRow.append(str(offset))
             bedRow.append(str(lineLen))
 
             bedFh.write("\t".join(bedRow))
             bedFh.write("\n")
-            bedFh.flush()
 
     bedFh.close()
 
     if skipCount != 0:
         logging.info("Could not place %d genes, these were skipped" % skipCount)
 
-    if geneCount==0:
-        errAbort("Could not resolve a single gene to a genome location. You will need to change the gene identifier options in hub.conf and check the expression matrix.")
-
-    logging.info("Processed %d genes" % geneCount)
     bedFname2 = bedFname.replace(".bed", ".sorted.bed")
     cmd = "LC_COLLATE=C sort -k1,1 -k2,2n %s > %s" % (bedFname, bedFname2)
-    runCommand(cmd)
+    cellbrowser.runCommand(cmd)
 
     # convert to .bb using .as file
     # from https://genome.ucsc.edu/goldenpath/help/examples/barChart/barChartBed.as
-    asFname = getStaticFile(join("genomes", "barChartBed.as"))
-    sizesFname = getSizesFname(genome)
+    #asFname = join(dataDir, )
+    asFname = cellbrowser.getStaticFile(["genomes", "barChartBed.as"])
+    sizesFname = cellbrowser.getSizesFname(genome)
 
     cmd = "bedToBigBed -as=%s -type=bed6+5 -tab %s %s %s" % (asFname, bedFname2, sizesFname, bbFname)
-    runCommand(cmd)
+    cellbrowser.runCommand(cmd)
 
-def buildTrackHub(db, inMatrixFname, metaFname, clusterFieldName, clusterOrderFile, hubName, bamDir, fixDot, \
-        geneType, geneModel, unitName, email, refHtmlFname, hubUrl, skipBarchart, stat, percentile, outDir):
-    " main function: make bigBarChart, trackDb and possibly bigWig and bigBed files "
+def buildTrackHub(db, inMatrixFname, metaFname, clusterFieldName, clusterOrderFile, hubName, bamDir, fixDot, geneType, unitName, email, refHtmlFname, hubUrl, skipBarchart, outDir):
 
     clusterToCells = parseClustersFromMeta(metaFname, clusterFieldName, fixDot)
 
     if clusterOrderFile is None:
         clusterOrder = list(sorted(clusterToCells.keys()))
         logging.info("No cluster order specified, using clusters in alphabetical order")
     else:
@@ -952,114 +819,72 @@
 
     writeHubStanza(tfh, hubName, db, email)
 
     matrixFname = join(outDir, "exprMatrix.tsv")
 
     bbFname = join(outDir, 'barChart.bb')
     catFname = join(outDir, 'clusters.tsv')
-    if skipBarchart or geneModel is None:
-        logging.info("Not creating barChart file, got command line option or geneModel is None")
+    if skipBarchart:
+        logging.info("Not creating barChart file, got command line option")
     else:
-        writeBarChartTdb(tfh, bbFname, clusterOrder, unitName, stat, percentile)
-        #if isfile(bbFname):
-            #logging.info("Not creating barChart file, %s already exists" % bbFname)
-        makeBarGraphBigBed(db, inMatrixFname, matrixFname, geneType, geneModel, clusterToCells, clusterOrder, stat, percentile, \
-                catFname, bbFname)
-        writeBarChartDesc(outDir, hubName, hubUrl, refHtmlFname)
+        writeBarChartTdb(tfh, bbFname, clusterOrder, unitName)
+        if isfile(bbFname):
+            logging.info("Not creating barChart file, %s already exists" % bbFname)
+        else:
+            makeBarGraphBigBed(db, inMatrixFname, matrixFname, geneType, clusterToCells, clusterOrder, catFname, bbFname)
 
     if bamDir:
         mergeBams(hubName, db, tfh, bamDir, clusterToCells, outDir)
-        writeBamDescPages(outDir, hubName, hubUrl, refHtmlFname)
 
     tfh.close()
 
+    writeDescPages(outDir, hubName, hubUrl, refHtmlFname)
 
 def cbTrackHub(options):
     " make track hub given meta file and directory with bam files "
     if options.init:
-        copyPkgFile("sampleConfig/hub.conf")
+        cellbrowser.copyPkgFile("sampleConfig/cellbrowser.conf")
         sys.exit(0)
 
-    global CBEMAIL
-    if CBEMAIL is None:
-        CBEMAIL = getConfig("email")
-
-    db, geneModel, email = None, None, None
-
-    cbConfFname = join(dirname(options.inConf), "cellbrowser.conf")
-    if isfile(cbConfFname):
-        logging.info("Initializing configuration from %s" % cbConfFname)
-        conf = loadConfig(cbConfFname)
-    else:
-        conf = {}
-
-    if not isfile(options.inConf):
-        logging.warn("Could not find a file %s. You can create one with the --init option." % options.inConf)
-    else:
-        conf = loadConfig(options.inConf, addTo=conf)
+    if isfile(options.inConf):
+        conf = cellbrowser.loadConfig(options.inConf)
 
-        geneModel = conf.get("geneModel")
-        db = conf.get("ucscDb")
-        email = conf.get("email", CBEMAIL)
-
-        inMatrixFname = conf.get("exprMatrix", None)
+        db = conf["ucscDb"]
+        inMatrixFname = conf["exprMatrix"]
         metaFname = conf["meta"]
         clusterFieldName = conf["clusterField"]
         clusterOrderFile = conf.get("clusterOrder")
-        bamDir = conf.get("bamDir")
-
+        bamDir = conf.get("bamDir", "bam")
         fixDot = conf.get("fixDot", False)
-
-        geneType = conf.get("geneIdType")
-
-        if not "unit" in conf:
-            errAbort("For track hubs, the unit of the values in the matrix is important. "
-            "Please specify a value for the 'unit' setting in cellbrowser.conf or hub.conf.")
-
-        unitName = conf.get("unit")
-        hubUrl = conf.get("hubUrl")
-        if not hubUrl:
-            errAbort("For track hubs, the URL to the final hub is important. "
-            "Please specify a value for the 'hubUrl' setting in cellbrowser.conf or hub.conf. "
-            "If you're unsure, set it to a non-existing URL now and update it later, when you know the URL")
-
-        refHtmlFname = conf.get("refHtmlFile", None)
+        email = conf.get("hubEmail", CBEMAIL)
+        geneType = conf["geneIdType"]
+        outDir = conf["hubDir"]
+        unitName = conf.get("unit", "TPM")
+        hubUrl = conf.get("hubUrl", "")
+        refHtmlFname = conf.get("refHtml", None)
 
         # use name, shortLabel or hubName from conf
-        hubName = conf.get("shortLabel", "UCSC single cell track hub, generated by cbHub")
-
-    if not db:
-        errAbort("You need to specify the ucscDb setting in your hub.conf."
-            "A track hub requires at least the name of the UCSC assembly, e.g. 'hg19' or 'mm10'.")
-    if not geneModel:
-        logging.warn("You did not specify the geneModel setting in your hub.conf. Example values are 'gencode28' for hg38."
-            "Because no gene -> genome mapping is known, the barchart graph has been deactivated. ")
-    if email is None:
-        errAbort("A UCSC track hub should include an email address. "
-            "Please specify one in hub.conf with the 'email=' setting or via the CBEMAIL environment variable or with the 'email=' setting in in ~/.cellbrowser.conf")
-
-    outDir = options.outDir
+        hubName = conf.get("hubName", conf.get("shortLabel", conf["name"]))
 
+    if options.hubDir:
+        outDir = options.hubDir
     if options.exprMatrix:
         inMatrixFname = options.exprMatrix
     if options.meta:
         metaFname = options.meta
     if options.clusterField:
         clusterFieldName = options.clusterField
-    #if options.clusterOrder:
-        #clusterOrderFile = options.clusterOrder
-    if options.outDir:
-        outDir = options.outDir
+    if options.clusterOrder:
+        clusterOrderFile = options.clusterOrder
+    if options.hubDir:
+        outDir = options.hubDir
     skipBarchart = options.skipBarchart
 
     if not isdir(outDir):
         logging.info("Making %s" % outDir)
         os.makedirs(outDir)
 
-    stat = options.stat
-    percentile = options.percentile
-
-    buildTrackHub(db, inMatrixFname, metaFname, clusterFieldName, clusterOrderFile, hubName, bamDir, fixDot, geneType, geneModel, unitName, email, refHtmlFname, hubUrl, skipBarchart, stat, percentile, outDir)
+    buildTrackHub(db, inMatrixFname, metaFname, clusterFieldName, clusterOrderFile, hubName, bamDir, fixDot, geneType, unitName, email, refHtmlFname, hubUrl, skipBarchart, outDir)
 
 def cbHubCli():
     args, options = cbHub_parseArgs()
     cbTrackHub(options, *args)
```

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/geneinfo.py` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/geneinfo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 # annotate a list of gene IDs with links to various external databases
 
 import logging, sys, optparse, re, unicodedata, string, csv
 from collections import defaultdict, namedtuple
 from os.path import join, basename, dirname, isfile
 
-from .cellbrowser import openStaticFile, staticFileNextRow, openFile, splitOnce, iterItems, lineFileNextRow, setDebug
-from .cellbrowser import readGeneSymbols
-
 dataDir = "geneAnnot"
 
-# no spaces/special chars in filenames - otherwise the URL will be rejected as invalid by urllib2
 HPRD = join(dataDir, "HPRD_molecular_class_081914.txt")
 HGNC = join(dataDir, "hgnc_complete_set_05Dec17.txt")
 SFARI = join(dataDir, "SFARI-Gene_genes_export06-12-2017.csv")
 OMIM = join(dataDir, "mim2gene.txt")
-COSMIC = join(dataDir, "Census_allWed_Dec__6_18_35_54_2017.tsv")
+COSMIC = join(dataDir, "Census_allWed Dec  6 18_35_54 2017.tsv")
 HPO = join(dataDir, "hpo_frequent_7Dec17.txt")
 BRAINSPANLMD = join(dataDir, "brainspan_genes.csv")
 BRAINSPANMOUSEDEV = join(dataDir, "brainspanMouse_9Dec17.txt")
 MGIORTHO = join(dataDir, "mgi_HGNC_homologene_8Dec17.txt")
 EUREXPRESS = join(dataDir, "eurexpress_7Dec17.txt")
 DDD = join(dataDir, "DDG2P_18_10_2018.csv.gz")
 
+from cellbrowser import openStaticFile, staticFileNextRow, openFile
 
 # ==== functions =====
     
 def parseArgs():
     " setup logging, parse command line arguments and options. -h shows auto-generated help page "
     parser = optparse.OptionParser("""usage: %prog [options] inFname outFname - annotate a tab-sep gene list file with information from other databases
             
-    A minimal input file has a header line with at one field called "gene" (=symbol or ENS/Entrez geneID) and
+    A minimal input file has a header line with at one field called "gene" (=symbol) and
     one field called "cluster".
     
     In the cellbrowser, the cluster name should match the cluster name in the meta data file.""")
 
     parser.add_option("-d", "--debug", dest="debug", action="store_true", help="show debug messages")
     parser.add_option("", "--hprd", dest="hprd", action="store", help="location of HPRD file, default %default", default=HPRD)
     parser.add_option("", "--hgnc", dest="hgnc", action="store", help="location of HGNC file, default %default", default=HGNC)
@@ -49,21 +46,72 @@
     #parser.add_option("", "--test", dest="test", action="store_true", help="do something") 
     (options, args) = parser.parse_args()
 
     if args==[]:
         parser.print_help()
         exit(1)
 
-    setDebug(options.debug)
+    if options.debug:
+        logging.basicConfig(level=logging.DEBUG)
+    else:
+        logging.basicConfig(level=logging.INFO)
     return args, options
 
+def lineFileNextRow(inFile):
+    """
+    parses tab-sep file with headers in first line
+    yields collection.namedtuples
+    strips "#"-prefix from header line
+    """
+
+    if isinstance(inFile, str):
+        fh = openFile(inFile)
+    else:
+        fh = inFile
+
+    line1 = fh.readline()
+    line1 = line1.strip("\n").lstrip("#")
+    headers = line1.split("\t")
+    headers = [re.sub("[^a-zA-Z0-9_]","_", h) for h in headers]
+    headers = [re.sub("^_","", h) for h in headers] # remove _ prefix
+    headers = [x if x!="" else "noName" for x in headers]
+
+    filtHeads = []
+    for h in headers:
+        if h[0].isdigit():
+            filtHeads.append("x"+h)
+        else:
+            filtHeads.append(h)
+    headers = filtHeads
+
+
+    Record = namedtuple('tsvRec', headers)
+    for line in fh:
+        if line.startswith("#"):
+            continue
+        line = line.decode("latin1")
+        # skip special chars in meta data and keep only ASCII
+        line = unicodedata.normalize('NFKD', line).encode('ascii','ignore')
+        line = line.rstrip("\n").rstrip("\r")
+        fields = string.split(line, "\t", maxsplit=len(headers)-1)
+        try:
+            rec = Record(*fields)
+        except Exception as e:
+            logging.error("Exception occured while parsing line, %s" % e)
+            logging.error("Filename %s" % fh.name)
+            logging.error("Line was: %s" % line)
+            logging.error("Does number of fields match headers?")
+            logging.error("Headers are: %s" % headers)
+            raise Exception("header count: %d != field count: %d wrong field count in line %s" % (len(headers), len(fields), line))
+        yield rec
+
 # ----------- main --------------
 def parseBrainspanLmd(inFname):
     " return entrez -> brainspanGeneId with all entrez IDs that are in the brainspan LMD set "
-    with openStaticFile(inFname, 'r') as csvfile:
+    with openStaticFile(inFname, 'rb') as csvfile:
         ret = {}
         cr = csv.reader(csvfile)
         headers = None
         for row in cr:
             if headers == None:
                 assert(row==['row_num','gene_id','ensembl_gene_id','gene_symbol','entrez_id'])
                 headers = row
@@ -83,15 +131,15 @@
             "4" : "Autism, 4 - Minimal evidence",
             "5" : "Autism, 5 - Hypothesized but untested",
             "6" : "Autism, 6 - Evidence does not support role",
     }
     # ['status', 'gene-symbol', 'gene-name', 'chromosome', 'genetic-category', 'gene-score', 'syndromic', 'number-of-reports']
     headers = None
     ret = {}
-    with openStaticFile(inFname, 'r') as csvfile:
+    with openStaticFile(inFname, 'rb') as csvfile:
         spamreader = csv.reader(csvfile)
         for row in spamreader:
             if headers == None:
                 headers = row
                 assert(headers[5]=="gene-score")
                 continue
             score = row[5]
@@ -155,15 +203,15 @@
             continue
         row = line.rstrip("\n").split("\t")
         entrez = row[2]
         hpoName = row[4]
         geneToNames[entrez].add(hpoName)
 
     ret = {}
-    for entrez, names in iterItems(geneToNames):
+    for entrez, names in geneToNames.iteritems():
         names = list(names)
         names.sort()
         ret[entrez] = ", ".join(names)
     return ret
 
 def parseMgiOrtho(hgncIdToEntrez, inFname):
     " return dict with mouse entrezId -> human entrez "
@@ -197,71 +245,54 @@
         if row.EMAP_Term!="":
             entrezToTerms[humanEntrez].add(row.EMAP_Term)
         entrezToEuroexpress[humanEntrez] = row.Assay_ID
 
     logging.info("Eurexpress mouse entrez IDs: %d mappable, %d not-mappable to human " % (len(entrezToEuroexpress),len(skippedMouseIds)))
     logging.debug("Eurexpress mouse: mouse entrez IDs not mappable to human: %s" % ",".join(skippedMouseIds))
     ret = {}
-    for entrezId, terms in iterItems(entrezToTerms):
+    for entrezId, terms in entrezToTerms.iteritems():
         eurexpId = entrezToEuroexpress[entrezId]
         ret[entrezId] = (eurexpId, ", ".join(sorted(list(terms))))
 
     return ret
 
 def parseDDD(fname):
     " parse DDD phenotype file "
     ret = {}
-    #for row in staticFileNextRow(inFname):
-        #print row
+    for row in staticFileNextRow(inFname):
+        print row
     return ret
     
 def parseSimpleMap(inFname):
     " parse simple tab-sep key-value file and return as dict "
     ret = {}
     for line in openStaticFile(inFname):
         row = line.rstrip("\n").split("\t")
         ret[row[0]] = row[1]
     return ret
 
 def tabGeneAnnotate(inFname, symToEntrez, symToSfari, entrezToClass, entrezToOmim, entrezToCosmic, entrezToHpo, entrezToLmd, entrezToEuroexpress, humanToMouseEntrezList, mouseEntrezToBrainspanMouseDev):
     " "
     headers = None
-    geneToSym = -1
     for row in lineFileNextRow(inFname):
         if headers is None:
             headers = list(row._fields)
             headers.append("_hprdClass")
             headers.append("_expr")
             headers.append("_geneLists")
             yield headers
-        sym = row[1]
-        if "|" in sym: # marker gene lists can carry geneId|symbol, strip the symbol in this case and re-convert below
-            sym = sym.split("|")[0]
-        if "." in sym: # remove Ensembl version identifier
-            sym = sym.split(".")[0]
-
-        # convert gene IDs to symbols
-        if geneToSym is -1:
-            geneToSym = readGeneSymbols(None, [sym])
-        if geneToSym is not None:
-            geneId = geneToSym.get(sym)
-            if geneId is None:
-                logging.debug("Cannot find NCBI Gene ID for symbol: %s" % sym)
-                geneId = sym
-            sym = geneId
-
+        sym = row.gene
         hprdClass = ""
         entrezId = symToEntrez.get(sym)
-
-        if entrezId == None:
-            logging.debug("Cannot find entrezId for symbol %s" % sym)
+        omimId = entrezToOmim.get(entrezId, "")
+        if entrezId != None:
+            hprdClass = entrezToClass.get(entrezId, "")
 
         # now summarize the presence/absence of this gene in various specialized gene lists:
         # OMIM, COSMIC, SFARI
-        hprdClass = entrezToClass.get(entrezId, "")
         geneLists = []
         if sym!="":
             # SFARI
             sfariInfo = symToSfari.get(sym)
             if sfariInfo is not None:
                 sfariInfo = "SFARI||"+sfariInfo
                 geneLists.append(sfariInfo)
@@ -298,15 +329,14 @@
 
             mouseEntrezList = humanToMouseEntrezList[entrezId]
             for mouseEntrez in mouseEntrezList:
                 if mouseEntrez in mouseEntrezToBrainspanMouseDev:
                     exprParts.append("BrainSpMouseDev|"+mouseEntrezToBrainspanMouseDev[mouseEntrez])
 
         row = list(row)
-        row[1] = sym # in case the original ID was a geneID, not a symbol
 
         row.append(hprdClass)
         row.append(";".join(exprParts))
         row.append(";".join(geneLists))
 
         yield row
 
@@ -325,18 +355,14 @@
     symToSfari = parseSfari(options.sfari)
     entrezToClass = parseHprd(options.hprd)
     #symToDdd = parseDdd(DDD)
 
     filename = args[0]
     outFname = args[1]
 
-    rowCount = 0
     ofh = open(outFname, "w")
     for row in tabGeneAnnotate(filename, symToEntrez, symToSfari, entrezToClass, entrezToOmim, entrezToCosmic, entrezToHpo, entrezToLmd, entrezToEuroexpress, humanToMouseEntrezList, entrezToBrainspanMouseDev):
         ofh.write("\t".join(row))
         ofh.write("\n")
-        rowCount +=1
     ofh.close()
 
-    logging.info("Annotated %d marker gene rows, output written to %s" % (rowCount, outFname))
-
```

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/palette.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/palette.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/papaparse.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/papaparse.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/FileSaver.1.1.20151003.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/FileSaver.1.1.20151003.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/tablesort.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/tablesort.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/hamster.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/hamster.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/spectrum.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/spectrum.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-submenu.min.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-submenu.min.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-dropmenu.min.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-dropmenu.min.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/introjs.2.4.0.min.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/introjs.2.4.0.min.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.sparkline.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.sparkline.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/intro.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/intro.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/normalizeWheel.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/normalizeWheel.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/chosen.1.8.2.min.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/chosen.1.8.2.min.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_555555_256x240.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_777620_256x240.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_ffffff_256x240.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_777777_256x240.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_444444_256x240.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_cc0000_256x240.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/select2.4.0.4.min.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/select2.4.0.4.min.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-submenu.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-submenu.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.contextMenu.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.contextMenu.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/chartjs-chart-box-and-violin-plot.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/chartjs-chart-box-and-violin-plot.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/split.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/split.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/mousetrap.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/mousetrap.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery-ui.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/FastBitSet.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/FastBitSet.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.3.3.7.min.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.3.3.7.min.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/chosen.jquery.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/chosen.jquery.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.contextMenu.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.contextMenu.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/select2.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/select2.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/chosen-sprite.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/chosen-sprite.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/spectrum-1.8.0.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/spectrum-1.8.0.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/font-awesome.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/font-awesome.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/tablesort.number.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/tablesort.number.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.min.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/Chart.bundle.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/Chart.bundle.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/materialIcons.woff` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/materialIcons.woff`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.tipsy.1.0.3.min.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.tipsy.1.0.3.min.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/pako_inflate.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/pako_inflate.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.3.1.1.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.3.1.1.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.ui.position.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.ui.position.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.tipsy.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.tipsy.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/ext/jquery-ui-1.12.1.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery-ui-1.12.1.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/js/maxPlot.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/js/maxPlot.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,261 +1,168 @@
 'use strict';
 // maxPlot: a fast scatter plot class
 /*jshint globalstrict: true*/
-/*jshint -W069 */
-/*jshint -W104 */
-/*jshint -W117 */
 
 // TODO:
+// remove onNoHover
 // fix mouseout into body -> marquee stays
+// fix the aspect ratio of the zoom marquee
 
 function getAttr(obj, attrName, def) {
     var val = obj[attrName];
     if (val === undefined)
         return def;
     else
         return val;
 }
 
 function cloneObj(d) {
-    /* returns a deep copy of an object, wasteful and destroys old references */
+    /* returns a copy of an object, wasteful */
     // see http://stackoverflow.com/questions/122102/what-is-the-most-efficient-way-to-deep-clone-an-object-in-javascript
     return JSON.parse(JSON.stringify(d));
 }
 
-function isValid(x) {
-    /* x is not null nor undefined */
-    return (x !== null && x !== undefined)
-}
-
-function cloneArray(a) {
-    /* returns a copy of an array */
-    return a.slice();
-}
-
-function copyObj(src, trg) {
-    /* object copying: copies all values from src to trg */
-    var key;
-    for (key in src) {
-        trg[key] = src[key]; // copies each property to the objCopy object
-    }
-}
-
-function debug(msg) {
-    if (window.doDebug)
-        console.log(msg);
-}
 
 function MaxPlot(div, top, left, width, height, args) {
     // a class that draws circles onto a canvas, like a scatter plot
     // div is a div DOM element under which the canvas will be created
     // top, left: position in pixels, integers
     // width and height: integers, in pixels, includes the status line
 
-    const HIDCOORD = 12345; // magic value for missing coordinates
-    // In rare instances, coordinates are saved but should not be shown. This way of implementing hiding
-    // may look hacky, but it simplifies the logic and improves performance.
-
-    // export this special value so other part of the code can use it
-    this.hiddenCoord = HIDCOORD;
-
-    var self = this; // 'this' has two conflicting meanings in javascript.
+    var self = this; // 'this' has two conflicting meanings in javascript. 
     // I use 'self' to refer to object variables, so I can use 'this' to refer to the caller context
 
     const gTextSize = 16; // size of cluster labels
     const gTitleSize = 18; // size of title text
-    const gStatusHeight = 14; // height of status bar
+    const gStatusHeight = 12; // height of status bar
     const gZoomButtonSize = 30; // size of zoom buttons
-    const gZoomFromLeft = 10; // position of zoom buttons from left
-    const gZoomFromBottom = 140; // position of zoom buttons from bottom
-    const gButtonBackground = "rgb(230, 230, 230, 0.85)" // grey level of buttons
+    const gZoomFromRight = 60; // position of zoom buttons from right
+    const gZoomFromBottom = 120; // position of zoom buttons from bottom
+    const gButtonBackground = "rgb(230, 230, 230, 0.6)" // grey level of buttons
     const gButtonBackgroundClicked = "rgb(180, 180, 180, 0.6)"; // grey of buttons when clicked
-    const gCloseButtonFromRight = 60; // distance of "close" button from right edge
-
-    const nonFatColor = "F9F9F9"; // color used in fattening mode for all non-fat cells
-    const nonFatColorCircles = "BBBBBB"; // color used in fattening mode for all non-fat cells
 
     // the rest of the initialization is done at the end of this file,
     // because the init involves many functions that are not defined yet here
 
-    this.initCanvas = function(div, top, left, width, height, args) {
+    this.initCanvas = function(div, top, left, width, height) {
         /* initialize a new Canvas */
 
-        div.style.top = top + "px";
-        div.style.left = left + "px";
-        div.style.position = "absolute";
-        div.style.display = "block";
         self.div = div;
-
         self.gSampleDescription = "cell";
         self.ctx = null; // the canvas context
         self.canvas = addCanvasToDiv(div, top, left, width, height - gStatusHeight);
 
-        self.interact = false;
-
-        if (args && args.showClose === true) {
-            self.closeButton = addChildControls(10, width - gCloseButtonFromRight);
-        }
-
-        if (args === undefined || (args["interact"] !== false)) {
-            self.interact = true;
-
-            addZoomButtons(height - gZoomFromBottom, gZoomFromLeft, self);
-            addModeButtons(10, 10, self);
-            addStatusLine(height - gStatusHeight, left, width, gStatusHeight);
-            addTitleDiv(height - gTitleSize - gStatusHeight - 4, 8);
-
-            console.log(self.parentPlot, self.childPlot);
-            /* add the div used for the mouse selection/zoom rectangle to the DOM */
-            var selectDiv = document.createElement('div');
-            selectDiv.id = "mpSelectBox";
-            selectDiv.style.border = "1px dotted black";
-            selectDiv.style.position = "absolute";
-            selectDiv.style.display = "none";
-            selectDiv.style.pointerEvents = "none";
-            self.div.appendChild(selectDiv);
-
-            // callbacks when user clicks or hovers over label or cell
-            self.onLabelClick = null; // called on label click, args: text of label and event
-            self.onCellClick = null; // called on cell click, args: array of cellIds and event
-            self.onCellHover = null; // called on cell hover, arg: array of cellIds
-            self.onNoCellHover = null; // called on hover over empty background
-            self.onSelChange = null; // called when the selection has been changed, arg: array of cell Ids
-            self.onLabelHover = null; // called when mouse hovers over a label
-            self.onNoLabelHover = null; // called when mouse does not hover over a label
-            self.onLineHover = null; // called when mouse over a trajectory line
-            self.onRadiusAlphaChange = null; // called when user changes radius or alpha
-            // self.onZoom100Click: called when user clicks the zoom100 button. Implemented below.
-            self.selectBox = selectDiv; // we need this later
-            self.setupMouse();
-
-            // connected plots
-            self.childPlot = null; // plot that is syncing from us, see split()
-            self.parentPlot = null; // plot that syncs to us, see split()
-
-        }
-
+        addZoomButtons(top + height - gZoomFromBottom, left + width - gZoomFromRight, self);
+        addModeButtons(top + 10, left + 10, self);
+        addStatusLine(top + height - gStatusHeight, left, width, gStatusHeight);
         addProgressBars(top + Math.round(height * 0.3), left + 30);
-        if (!args || args.showSliders === undefined || args.showSliders === true)
-            addSliders(height - gStatusHeight - 30, width);
+        addTitleDiv(top + height - gTitleSize - gStatusHeight, left + 5);
+
+        /* add the div used for the mouse selection/zoom rectangle to the DOM */
+        var selectDiv = document.createElement('div');
+        selectDiv.id = "mpSelectBox";
+        selectDiv.style.border = "1px dotted black";
+        selectDiv.style.position = "absolute";
+        selectDiv.style.display = "none";
+        selectDiv.pointerEvents = "none";
+        self.div.appendChild(selectDiv);
+        self.selectBox = selectDiv; // we need this later
+
+        self.setupMouse();
+
+        // callbacks when user clicks or hovers over label or cell 
+        self.onLabelClick = null; // called on label click, args: text of label and event
+        self.onCellClick = null; // called on cell click, args: array of cellIds and event
+        self.onCellHover = null; // called on cell hover, arg: array of cellIds
+        self.onNoCellHover = null; // called on hover over empty background
+        self.onSelChange = null; // called when the selection has been changed, arg: array of cell Ids
+        // self.onZoom100Click: called when user clicks the zoom100 button. Implemented below.
 
         // timer that is reset on every mouse move
         self.timer = null;
-    }
-
-    function isHidden(x, y) {
-        /* special coords are used for circles that are off-screen or otherwise not visible */
-        return ((x === HIDCOORD && y === HIDCOORD)) // not shown (e.g. no coordinate or off-screen)
-    }
 
-    this.initPort = function(args) {
-        /* init all viewport related state (zoom, radius, alpha) */
-        self.port = {};
-        self.port.zoomRange = {}; // object with keys minX, , maxX, minY, maxY, in data units
-        self.port.radius = getAttr(args, "radius", null); // current radius of the circles, 0=one pixel dots
+        // all other object variables are added by the "initPlot(args)" function below
 
-        // we keep a copy of the 'initial' arguments at 100% zoom
-        self.port.initZoom = {};
-        self.port.initRadius = self.port.radius; // circle radius at full zoom
-        self.port.initAlpha = getAttr(args, "alpha", 0.3);
-    };
+        // when the user starts to select but lifts the mouse button outside
+        // the canvas, the current selection must be reset
+        //self.canvas.addEventListener("mouseleave", function() {self.resetMarquee();});
+
+        //document.body.addEventListener("mouseup", function(evt) {
+        //var targetId = evt.target.id;
+        //console.log("mouseup on body");
+        //if(targetId !== "mpCanvas" && targetId!=="mpSelectBox") {  // do nothing on the canvas
+        //console.log("mouseup outside of canvas, resetting marquee");
+        //self.resetMarquee();
+        //evt.stopPropagation();
+        //}
+        //});
+        // for this to work, the body has to really cover the whole page
+        //document.body.style.height = "100vh";
+    }
 
     this.initPlot = function(args) {
         /* create a new scatter plot on the canvas */
         if (args === undefined)
             args = {};
 
-        self.scalingDone = false;
-
-        self.globalOpts = args;
-
         self.mode = 1; // drawing mode
 
-        // everything related to circle coordinates
-        self.coords = {};
-        self.coords.orig = null; // coordinates of cells in original coordinates
-        self.coords.labels = null; // cluster label positions in pixels, array of [x,y,text]
+        self.zoomRange = null; // object with keys minX, , maxX, minY, maxY
+        self.coords = null;
+        self.clusterLabels = null; // cluster labels, array of [x,y,text]
+
+        self.pxCoords = null; // coordinates of cells as screen pixels or 0,0 if not shown
+        self.pxLabels = null; // cluster labels in pixels, array of [x,y,text] 
+        self.pxLabelBbox = null; // cluster label bounding boxes, array of [x1,x2,x2,y2]
 
-        self.coords.px = null; // coordinates of cells and labels as screen pixels or (HIDCOORD,HIDCOORD) if not shown
-        self.coords.labelBbox = null; // cluster label bounding boxes, array of [x1,x2,x2,y2]
-
-        self.col = {};
-        self.col.pal = null; // list of six-digit hex codes
-        self.col.arr = null; // length is coords.px/2, one byte per cell = index into self.col.pal
-
-        self.selCells = new Set(); // IDs of cells that are selected (drawn in black)
+        self.doDrawLabels = true; // should cluster labels be drawn?
 
-        self.fatIdx = null; // Index of value that is in "fat mode" (=cells bigger, all other cells in light-grey)
+        self.colors = null; // list of six-digit hex codes
+        self.colorArr = null; // length is pxCoords/2, one byte per cell = index into self.colors
+        self.radius = getAttr(args, "radius", null); // current radius of the circles, 0=one pixel dots
+        self.alpha = getAttr(args, "alpha", 0.3);
+        self.selCells = null; // IDs of cells that are "selected" and as such highlighted in some way
 
-        self.doDrawLabels = true; // should cluster labels be drawn?
-        self.initPort(args);
+        // we keep a copy of the 'initial' arguments at 100% zoom
+        self.initZoom = cloneObj(self.zoomRange);
+        self.initRadius = self.radius; // circle radius at full zoom
 
-        // mouse drag mode: can be "select", "move" or "zoom"
+        // mouse drag is modal: can be "select", "move" or "zoom"
         self.dragMode = "select";
 
         // for zooming and panning
         self.mouseDownX = null;
         self.mouseDownY = null;
         self.panCopy = null;
 
         // to detect if user just clicked on a dot
         self.dotClickX = null;
         self.dotClickY = null;
 
-        // the background image for spatial mode
-        self.background = null;
-
         self.activateMode(getAttr(args, "mode", "move"));
-
     };
 
+    // call the constructor
+    //self.newObject(div, top, left, width, height, args);
+
     this.clear = function() {
-        clearCanvas(self.ctx, self.canvas.width, self.canvas.height);
+        clearCanvas(self.ctx, self.width, self.height);
+    };
+
+    this.setPos = function(left, top) {
+        /* position the canvas on the page */
+        self.canvas.style.left = left + "px";
+        self.canvas.style.top = top + "px";
     };
 
     this.setTitle = function(text) {
         self.title = text;
         self.titleDiv.innerHTML = text;
     };
 
-    this.activateSliders = function() {
-        $(self.alphaSlider).slider({
-            "value": 4,
-            "min": 1,
-            "max": 7,
-            "step": 1,
-            "slide": onChangeAlpha
-        });
-        $(self.radiusSlider).slider({
-            "value": 4,
-            "min": 1,
-            "max": 7,
-            "step": 1,
-            "slide": onChangeRadius
-        });
-
-    }
-
-    this.setWatermark = function(text) {
-        if (text === "" && self.watermark) {
-            self.watermark.parentNode.removeChild(self.watermark);
-            self.watermark = undefined;
-            return;
-        }
-
-        if (self.watermark)
-            self.watermark.parentNode.removeChild(self.watermark);
-
-        var elem = document.createElement('div');
-        elem.id = "tpWatermark";
-        elem.style.cssText = 'pointer-events: none;position: absolute; width: 1000px; opacity: 0.5; top: 10px; left: 45px; text-align: left; vertical-align: top; color: black; font-size: 20px; font-weight:bold; font-style:oblique';
-        elem.textContent = text;
-        self.div.appendChild(elem);
-        self.watermark = elem;
-    }
 
     // -- (private) helper functions
     // -- these are normal functions, not methods, they do not access "self"
 
     function gebi(idStr) {
         return document.getElementById(idStr);
     }
@@ -264,15 +171,15 @@
         var el = gebi(idStr);
         if (el !== null) {
             el.parentNode.removeChild(el);
         }
     }
 
     function activateTooltip(selector) {
-        /* uses bootstrap tooltip. Use noconflict in html, I had to rename BS's tooltip to avoid overwrite by jquery
+        /* uses bootstrap tooltip. Use noconflict in html, I had to rename BS's tooltip to avoid overwrite by jquery 
          */
         if (window.jQuery && $.fn.bsTooltip !== undefined) {
             var ttOpt = {
                 "html": true,
                 "animation": false,
                 "delay": {
                     "show": 400,
@@ -292,70 +199,47 @@
             return 2;
         else if (coordCount > 4000)
             return 4;
         else
             return 5;
     }
 
-    function createSliderSpan(id, width, height, left) {
-        /* create div with given width and height */
-        var div = document.createElement('span');
-        div.id = id;
-        div.style.position = "relative";
-        div.style.width = width + "px";
-        div.style.height = height + "px";
-        div.style.left = left + "px";
-        return div;
-    }
-
-    function createButton(width, height, id, title, text, imgFname, paddingTop, paddingBottom, addSep, addThickSep, fontSize) {
-        /* make a light-grey div that behaves like a button, with text and/or an image on it
+    function createButton(width, height, id, title, text, imgFname, paddingTop, addSep) {
+        /* make a light-grey div that behaves like a button, with text and/or an image on it 
          * Images are hard to vertically center, so padding top can be specified.
          * */
         var div = document.createElement('div');
         div.id = id;
-        div.className = "mpButton";
         div.style.backgroundColor = gButtonBackground;
         div.style.width = width + "px";
         div.style.height = height + "px";
-        div.style["z-index"] = "10";
         div.style["text-align"] = "center";
         div.style["vertical-align"] = "middle";
         div.style["line-height"] = height + "px";
-        if (fontSize === undefined || fontSize === null) {
-            if (text !== null)
-                if (text.length > 3)
-                    div.style["font-size"] = "11px";
-                else
-                    div.style["font-size"] = "14px";
-        } else {
-            div.style["font-size"] = fontSize + "px";
-        }
+        if (text !== null)
+            if (text.length > 3)
+                div.style["font-size"] = "11px";
+            else
+                div.style["font-size"] = "14px";
         div.style["font-weight"] = "bold";
         div.style["font-family"] = "sans-serif";
 
         if (title !== null)
             div.title = title;
         if (text !== null)
-            div.innerHTML = text;
-        if (imgFname !== null && imgFname !== undefined) {
+            div.textContent = text;
+        if (imgFname !== null && imgFname != undefined) {
             var img = document.createElement('img');
             img.src = imgFname;
-            if (paddingTop !== null && paddingTop !== undefined) {
+            if (paddingTop !== null && paddingTop != undefined)
                 img.style.paddingTop = paddingTop + "px";
-                if (paddingBottom)
-                    img.style.paddingBottom = paddingBottom + "px";
-            }
             div.appendChild(img);
         }
         if (addSep === true)
             div.style["border-bottom"] = "1px solid #D7D7D7";
-        if (addThickSep === true)
-            div.style["border-bottom"] = "2px solid #C7C7C7";
-
 
         // make color dark grey when mouse is pressed
         div.addEventListener("mousedown", function() {
             this.style.backgroundColor = gButtonBackgroundClicked;
         });
 
         div.addEventListener("mouseup", function() {
@@ -381,27 +265,26 @@
     }
 
     function addZoomButtons(top, left, self) {
         /* add the plus/minus buttons to the DOM and place at position x,y on the screen */
         var width = gZoomButtonSize;
         var height = gZoomButtonSize;
 
-        var plusDiv = createButton(width, height, "mpCtrlZoomPlus", "Zoom in. Keyboard: +", "+", null, null, null, true);
+        var plusDiv = createButton(width, height, "mpCtrlZoomPlus", "Zoom in", "+", null, null, true);
         //plusDiv.style["border-bottom"] = "1px solid #D7D7D7";
 
-        var fullDiv = createButton(width, height, "mpCtrlZoom100", "Zoom in. Keyboard: space", "100%", null, null, null, true);
+        var fullDiv = createButton(width, height, "mpCtrlZoom100", "Zoom in", "100%", null, null, true);
         //full.style["border-bottom"] = "1px solid #D7D7D7";
 
-        var minusDiv = createButton(width, height, "mpCtrlZoomMinus", "Zoom out. Keyboard: -", "-");
+        var minusDiv = createButton(width, height, "mpCtrlZoomMinus", "Zoom out", "-");
 
         var ctrlDiv = makeCtrlContainer(top, left);
         ctrlDiv.appendChild(plusDiv);
         ctrlDiv.appendChild(fullDiv);
         ctrlDiv.appendChild(minusDiv);
-        self.zoomDiv = ctrlDiv;
 
         self.div.appendChild(ctrlDiv);
 
         minusDiv.addEventListener('click', function() {
             self.zoomBy(0.75);
             self.drawDots();
         });
@@ -412,200 +295,70 @@
         plusDiv.addEventListener('click', function() {
             self.zoomBy(1.333);
             self.drawDots();
         });
     }
 
     function addTitleDiv(top, left) {
-        var div = document.createElement('div');
-        div.className = "tpTitle";
-        div.style.top = top + "px";
-        div.style.left = left + "px";
-        div.style.fontSize = gTitleSize;
-        div.id = 'mpTitle';
-        self.div.appendChild(div);
-        self.titleDiv = div;
-    }
-
-    function onChangeAlpha(ev, ui) {
-        console.log("alpha: " + ui.value);
-        var sliderVal = ui.value; // 1-7
-        var multMap = {
-            7: 0.15,
-            6: 0.4,
-            5: 0.8,
-            4: 1.0,
-            3: 1.2,
-            2: 1.5,
-            1: 1.8
-        }
-        self.port.alphaMult = multMap[sliderVal];
-        console.log("alphaMult: " + self.port.alphaMult);
-        self.calcRadius();
-        self.drawDots();
-    }
-
-    function onChangeRadius(ev, ui) {
-        //console.log("radius: "+ui.value);
-        var sliderVal = ui.value; // 1-7
-        var multMap = {
-            1: 1 / 3,
-            2: 1 / 2,
-            3: 1 / 1.5,
-            4: 1.0,
-            5: 1.5,
-            6: 2.0,
-            7: 3.0
-        }
-        self.port.radiusMult = multMap[sliderVal];
-        self.calcRadius();
-        self.drawDots();
-    }
-
-    function addSliders(fromTop, canvWidth) {
-        /* add sliders for transparency and radius */
-        // alpha reset slider: a label, a slider + a reset button
-        var sliderWidth = 90;
-        var fromLeft = canvWidth - sliderWidth - 2 * 45 - 50;
-
-        var alphaSlider = createSliderSpan("mpAlphaSlider", sliderWidth, 10, 35);
-        self.alphaSlider = alphaSlider; // see activateSliders() for the jquery UI part of the code, executed later
-        alphaSlider.style.float = "left";
-        //alphaSlider.style.top = "3px";
-
-        // container for label + control elements
-        var alphaCont = document.createElement('div');
-        alphaCont.id = "mpAlphaCont";
-        //alphaCont.style.left = "150px"; // cellbrowser.css defines grid widths: 45
-        alphaCont.className = "sliderContainer";
-        alphaCont.style.top = "15px"; // (fromTop-14)+"px";
-        alphaCont.style.left = "0px";
-
-        var alphaLabel = document.createElement('div'); // contains the slider and the reset button, floats right
-        alphaLabel.id = "alphaSliderLabel";
-        alphaLabel.textContent = "Transparency";
-        alphaLabel.className = "sliderLabel";
-
-        // reset button
-        var undoSvg = '<svg xmlns="http://www.w3.org/2000/svg" height="1em" viewBox="0 0 512 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><path d="M212.333 224.333H12c-6.627 0-12-5.373-12-12V12C0 5.373 5.373 0 12 0h48c6.627 0 12 5.373 12 12v78.112C117.773 39.279 184.26 7.47 258.175 8.007c136.906.994 246.448 111.623 246.157 248.532C504.041 393.258 393.12 504 256.333 504c-64.089 0-122.496-24.313-166.51-64.215-5.099-4.622-5.334-12.554-.467-17.42l33.967-33.967c4.474-4.474 11.662-4.717 16.401-.525C170.76 415.336 211.58 432 256.333 432c97.268 0 176-78.716 176-176 0-97.267-78.716-176-176-176-58.496 0-110.28 28.476-142.274 72.333h98.274c6.627 0 12 5.373 12 12v48c0 6.627-5.373 12-12 12z"/></svg>';
-
-        //var alphaReset = createButton(15, 15, "mpAlphaReset", "Reset transparency", undoSvg, null, null, null, false, false, 10);
-        //alphaReset.style.float = "right";
-        //alphaReset.style.marginLeft = "2px";
-        //alphaReset.addEventListener ('click',  function() { self.resetAlpha(); self.drawDots();}, false);
-
-        var sliderReset = createButton(15, 15, "mpSliderReset", "Reset transparency and circle size", undoSvg, null, null, null, false, false, 10);
-        sliderReset.style.backgroundColor = "transparent";
-        sliderReset.style.float = "right";
-        //sliderReset.style.lineHeight = "16px";
-        sliderReset.style.marginLeft = "10px";
-        sliderReset.style.top = "0px";
-        sliderReset.style.top = "0px";
-        sliderReset.style.position = "relative";
-        sliderReset["z-index"] = "10"; // ? why ?
-        sliderReset.addEventListener('click', function() {
-            self.resetAlpha();
-            self.resetRadius();
-            self.drawDots()
-        }, false);
-
-        alphaCont.appendChild(alphaLabel);
-        alphaCont.appendChild(alphaSlider);
-        //alphaCont.appendChild(alphaReset);
-        alphaCont.appendChild(sliderReset);
-
-        // Radius reset slider: label, slider and reset button
-        var radiusSlider = createSliderSpan("mpRadiusSlider", sliderWidth, 10, 35);
-        radiusSlider.style.float = "left";
-        self.radiusSlider = radiusSlider; // see activateSliders() for the jquery UI part of the code, executed later
-
-        // container for label + slider and reset button
-
-        var radiusCont = document.createElement('span');
-        radiusCont.className = "sliderContainer";
-        radiusCont.id = "mpRadiusDiv";
-        radiusCont.style.left = "0px"; //fromLeft+"px";
-        radiusCont.style.top = "0px"; //fromTop+"px";
-        radiusCont.appendChild(radiusSlider)
-
-
-        var radiusLabel = document.createElement('span'); // contains the slider and the reset button, floats right
-        radiusLabel.id = "radiusSliderLabel";
-        radiusLabel.textContent = "Circle Size";
-        radiusLabel.style.width = "80px";
-        radiusLabel.className = "sliderLabel";
-
-        radiusCont.appendChild(radiusLabel);
-        radiusCont.appendChild(radiusSlider);
-        //radiusCont.appendChild(sliderReset);
-        var brEl = document.createElement('br');
-        radiusCont.appendChild(brEl);
-
-        // add both to the big container div that holds all three slider elements
-        var sliderDiv = document.createElement('span');
-        sliderDiv.style.top = fromTop + "px";
-        sliderDiv.style.left = fromLeft + "px";
-        sliderDiv.style.position = "relative";
-        sliderDiv.style.zIndex = "10";
-        sliderDiv.id = "mpSliderDiv";
-        sliderDiv.appendChild(radiusCont);
-        sliderDiv.appendChild(alphaCont);
-        self.div.appendChild(sliderDiv);
-        self.sliderDiv = sliderDiv; // for quickResize()
-    }
-
-    function addCloseButton(top, left) {
-        /* add close button and sync checkbox */
+        //var ctx = self.ctx;
+        //ctx.save();
+        //ctx.font = "bold "+gTextSize+"px Sans-serif"
+        //ctx.fillStyle = "rgba(220, 220, 220)";
+        //ctx.textBaseline = "top";
+        //ctx.fillText(self.title,5,self.height - gTextSize - 3); 
+        //ctx.restore();
         var div = document.createElement('div');
         div.style.cursor = "default";
         div.style.left = left + "px";
         div.style.top = top + "px";
         div.style.display = "block";
         div.style.position = "absolute";
         div.style.fontSize = gTitleSize;
-        div.style.padding = "3px";
-        div.style.borderRadius = "3px";
-        div.style.border = "1px solid #c5c5c5";
-        div.style.backgroundColor = "#f6f6f6";
-        div.style.color = "#454545";
-        div.id = 'mpCloseButton';
-        div.textContent = "Close";
+        div.id = 'mpTitle';
+        //div.innerHTML = title;
+        div.style['color'] = "lightgrey";
         self.div.appendChild(div);
-        return div;
-    }
-
-    function addChildControls(top, left) {
-        addCloseButton(top, left);
+        self.titleDiv = div;
     }
 
     function appendButton(parentDiv, id, title, imgName) {
         /* add a div styled like a button under div */
         var div = document.createElement('div');
         div.title = title;
         div.id = id;
 
     }
 
     function addModeButtons(top, left, self) {
         /* add the zoom/move/select control buttons to the DOM */
+        //var htmls = [];
+        //htmls.push('<div id="mpIcons" style="display:inline-block">');
+        //htmls.push('<div style="vertical-align:top">');
+        //htmls.push('<div title="Select mode.<br>Keyboard: shift or s" id="mpIconModeSelect"><img src="img/select.png"></button>');
+        //htmls.push('<div title="Zoom-to-rectangle mode. Keyboard: Windows/Command or z" id="mpIconModeZoom" style="display: block; margin-right:0"><img src="img/zoom.png"></button>');
+        //htmls.push('<div data-placement="bottom" title="Move mode. Keyboard: Alt or m" id="mpIconModeMove" data-toggle="tooltip" class="ui-button tpIconButton" class="mpModeButton" style="margin-right:0"><img src="img/move.png"></button>');
+        //htmls.push('</div>');
+        //htmls.push('<button title="Zoom to 100%, showing all data, keyboard: space" data-placement="bottom" data-toggle="tooltip" id="mpZoom100Button" class="ui-button tpIconButton" style="font-size:10px; font-weight: bold; margin-top: 4px; margin-right:0; display:block; padding:0">100%</button>');
+        //<img style="width:22px; height:22px" src="img/center.png">
+
         var ctrlDiv = makeCtrlContainer(top, left);
 
         var bSize = gZoomButtonSize;
 
-        var selectButton = createButton(bSize, bSize, "mpIconModeSelect", "Select mode. Keyboard: shift or s", null, "img/select.png", 0, 4, true, true);
+        var selectButton = createButton(bSize, bSize, "mpIconModeSelect", "Select mode. Keyboard: shift or s", null, "img/select.png", 4, true);
         selectButton.addEventListener('click', function() {
             self.activateMode("select")
         }, false);
 
-        var zoomButton = createButton(bSize, bSize, "mpIconModeZoom", "Zoom-to-rectangle mode. Keyboard: Windows/Command or z", null, "img/zoom.png", 4, 4, true);
+        var zoomButton = createButton(bSize, bSize, "mpIconModeZoom", "Zoom-to-rectangle mode. Keyboard: Windows/Command or z", null, "img/zoom.png", 4, true);
         zoomButton.addEventListener('click', function() {
             self.activateMode("zoom")
         }, false);
 
-        var moveButton = createButton(bSize, bSize, "mpIconModeMove", "Move mode. Keyboard: Alt or m", null, "img/move.png", 4, 4);
+        var moveButton = createButton(bSize, bSize, "mpIconModeMove", "Move mode. Keyboard: Alt or m", null, "img/move.png", 4);
         moveButton.addEventListener('click', function() {
             self.activateMode("move");
         }, false);
 
         self.icons = {};
         self.icons["move"] = moveButton;
         self.icons["select"] = selectButton;
@@ -613,37 +366,43 @@
 
         //ctrlDiv.innerHTML = htmls.join("");
         ctrlDiv.appendChild(moveButton);
         ctrlDiv.appendChild(selectButton);
         ctrlDiv.appendChild(zoomButton);
 
         self.div.appendChild(ctrlDiv);
-        self.toolDiv = ctrlDiv;
 
         activateTooltip('.mpIconButton');
+
+        //gebi('mpZoom100Button').addEventListener ('click', function(ev) { return self.onZoom100Click(ev) } );
     }
 
     function setStatus(text) {
         self.statusLine.innerHTML = text;
     }
 
     function addStatusLine(top, left, width, height) {
         /* add a status line div */
         var div = document.createElement('div');
         div.id = "mpStatus";
         div.style.backgroundColor = "rgb(240, 240, 240)";
         div.style.position = "absolute";
         div.style.top = top + "px";
-        //div.style.left = left+"px";
+        div.style.left = left + "px";
         div.style.width = width + "px";
         div.style.height = height + "px";
         div.style["border-left"] = "1px solid #DDD";
         div.style["border-right"] = "1px solid #DDD";
         div.style["border-top"] = "1px solid #DDD";
+        //div.style["border-bottom"]="1px solid #DDD";
         div.style["font-size"] = (gStatusHeight - 1) + "px";
+        //div.style["vertical-align"]="middle";
+        //div.style["line-height"]=(height-2)+"px";
+        //div.style["box-shadow"]="0px 2px 4px rgba(0,0,0,0.3)";
+        //div.style["border-radius"]="2px";
         div.style["cursor"] = "pointer";
         div.style["font-family"] = "sans-serif";
         self.div.appendChild(div);
         self.statusLine = div;
     }
 
     function addProgressBars(top, left) {
@@ -654,15 +413,15 @@
         div.style.left = left + "px";
         div.style.position = "absolute";
 
         var htmls = [];
         for (var i = 0; i < 3; i++) {
             htmls.push('<div id="mpProgressDiv' + i + '" style="display:none; height:17px; width:300px; background-color: rgba(180, 180, 180, 0.3)" style="">');
             htmls.push('<div id="mpProgress' + i + '" style="background-color:#666; height:17px; width:10%"></div>');
-            htmls.push('<div id="mpProgressLabel' + i + '" style="color:black; line-height:17px; position:absolute; top:' + (i * 17) + 'px;left:100px">Loading...</div>');
+            htmls.push('<div id="mpProgressLabel' + i + '" style="color:white; line-height:17px; position:absolute; top:' + (i * 17) + 'px;left:100px">Loading...</div>');
             htmls.push('</div>');
         }
 
         div.innerHTML = htmls.join("");
         self.div.appendChild(div);
     }
 
@@ -672,16 +431,16 @@
         canv.id = 'mpCanvas';
         //canv.style.border = "1px solid #AAAAAA";
         canv.style.backgroundColor = "white";
         canv.style.position = "absolute";
         canv.style.display = "block";
         canv.style.width = width + "px";
         canv.style.height = height + "px";
-        //canv.style.top = top+"px";
-        //canv.style.left = left+"px";
+        canv.style.top = top + "px";
+        canv.style.left = left + "px";
         // No scaling = one unit on screen is one pixel. Essential for speed.
         canv.width = width;
         canv.height = height;
 
         // need to keep these as ints, need them all the time
         self.width = width;
         self.height = height;
@@ -720,89 +479,33 @@
         var pxLabels = [];
         for (var i = 0; i < labels.length; i++) {
             var annot = labels[i];
             var x = annot[0];
             var y = annot[1];
             var text = annot[2];
             // XX ignore anything outside of current zoom range. Performance?
-            if (isHidden(x, y) || (x < minX) || (x > maxX) || (y < minY) || (y > maxY)) {
+            if ((x < minX) || (x > maxX) || (y < minY) || (y > maxY)) {
                 pxLabels.push(null);
-            } else {
-                var xPx = Math.round((x - minX) * xMult) + borderSize;
-                var yPx = winHeight - Math.round((y - minY) * yMult) + borderSize;
-                pxLabels.push([xPx, yPx, text]);
+                continue;
             }
+            var xPx = Math.round((x - minX) * xMult) + borderSize;
+            var yPx = winHeight - Math.round((y - minY) * yMult) + borderSize;
+            pxLabels.push([xPx, yPx, text]);
         }
         return pxLabels;
     }
 
-    function constrainVal(x, min, max) {
-        /* if x is not in range min, max, limit to min or max */
-        if (x < min)
-            return min;
-        if (x > max)
-            return max;
-        return x;
-    }
-
-    function scaleLines(lines, zoomRange, winWidth, winHeight) {
-        /* scale an array of (x1, y1, x2, y2), cutting lines at the screen edges */
-        var minX = zoomRange.minX;
-        var maxX = zoomRange.maxX;
-        var minY = zoomRange.minY;
-        var maxY = zoomRange.maxY;
-
-        var spanX = maxX - minX;
-        var spanY = maxY - minY;
-        var xMult = winWidth / spanX;
-        var yMult = winHeight / spanY;
-
-        // transform from data floats to screen pixel coordinates
-        var pxLines = [];
-        for (var lineIdx = 0; lineIdx < lines.length; lineIdx++) {
-            var line = lines[lineIdx];
-            var x1 = line[0];
-            var y1 = line[1];
-            var x2 = line[2];
-            var y2 = line[3];
-
-            var startInvis = ((x1 < minX) || (x1 > maxX) || (y1 < minY) || (y1 > maxY));
-            var endInvis = ((x2 < minX) || (x2 > maxX) || (y2 < minY) || (y2 > maxY));
-
-            // line is entirely hidden
-            if (startInvis && endInvis)
-                continue
-            if (startInvis) {
-                x1 = constrainVal(x1, minX, maxX);
-                y1 = constrainVal(y1, minY, maxY);
-            }
-            if (endInvis) {
-                x2 = constrainVal(x2, minX, maxX);
-                y2 = constrainVal(y2, minY, maxY);
-            }
-
-            var x1Px = Math.round((x1 - minX) * xMult);
-            var y1Px = winHeight - Math.round((y1 - minY) * yMult);
-            var x2Px = Math.round((x2 - minX) * xMult);
-            var y2Px = winHeight - Math.round((y2 - minY) * yMult);
-            pxLines.push([x1Px, y1Px, x2Px, y2Px]);
-        }
-        return pxLines;
-    }
-
     function scaleCoords(coords, borderSize, zoomRange, winWidth, winHeight, annots) {
         /* scale list of [x (float),y (float)] to integer pixels on screen and
          * annots is an array with on-screen annotations in the format (x, y,
          * otherInfo) that is also scaled.  return [array of (x (int), y (int)),
          * scaled annots array]. Take into account the current zoom range.      *
          * Canvas origin is top-left, but usually plotting origin is bottom-left,
-         * so also flip the Y axis. sets invisible coords to HIDCOORD
+         * so also flip the Y axis.
          * */
-        if (coords === null)
-            return;
         console.time("scale");
         var minX = zoomRange.minX;
         var maxX = zoomRange.maxX;
         var minY = zoomRange.minY;
         var maxY = zoomRange.maxY;
 
         winWidth = winWidth - (2 * borderSize);
@@ -814,239 +517,85 @@
         var yMult = winHeight / spanY;
 
         // transform from data floats to screen pixel coordinates
         var pixelCoords = new Uint16Array(coords.length);
         for (var i = 0; i < coords.length / 2; i++) {
             var x = coords[i * 2];
             var y = coords[i * 2 + 1];
-            // set everything outside of current zoom range to hidden
-            if ((x < minX) || (x > maxX) || (y < minY) || (y > maxY)) {
-                pixelCoords[2 * i] = HIDCOORD; // see isHidden()
-                pixelCoords[2 * i + 1] = HIDCOORD;
-            } else {
-                var xPx = Math.round((x - minX) * xMult) + borderSize;
-                // our y-axis is flipped compared to matplotlib/R, so we do winHeight - pixel value
-                // to make sure that our plot looks like the figures in the papers
-                var yPx = winHeight - Math.round((y - minY) * yMult) + borderSize;
-                pixelCoords[2 * i] = xPx;
-                pixelCoords[2 * i + 1] = yPx;
-            }
+            // simply ignore anything outside of current zoom range.
+            if ((x < minX) || (x > maxX) || (y < minY) || (y > maxY))
+                continue;
+            var xPx = Math.round((x - minX) * xMult) + borderSize;
+            // flipY: y-axis is flipped, so we do winHeight - pixel value
+            var yPx = winHeight - Math.round((y - minY) * yMult) + borderSize;
+            pixelCoords[2 * i] = xPx;
+            pixelCoords[2 * i + 1] = yPx;
         }
 
         console.timeEnd("scale");
         return pixelCoords;
     }
 
-    function drawRect(ctx, pxCoords, coordColors, colors, radius, alpha, selCells, fatIdx) {
-        /* draw not circles but tiny rectangles. Maybe good enough for 2pixels sizes */
-        debug("Drawing " + coordColors.length + " rectangles, with fillRect");
+    function drawRect(ctx, pxCoords, coordColors, colors, radius, alpha, selCells) {
+        console.log("Drawing " + coordColors.length + " rectangles, with fillRect");
         ctx.save();
         ctx.globalAlpha = alpha;
         var dblSize = 2 * radius;
         var count = 0;
         for (var i = 0; i < pxCoords.length / 2; i++) {
             var pxX = pxCoords[2 * i];
             var pxY = pxCoords[2 * i + 1];
-            if (isHidden(pxX, pxY))
+            if (pxX === 0 && pxY === 0)
                 continue;
-
-            var valIdx = coordColors[i];
-            var col = colors[valIdx];
-            if (fatIdx !== null)
-                if (valIdx === fatIdx)
-                    col = "000000";
-                else
-                    col = "DDDDDD";
-
+            var col = colors[coordColors[i]];
             ctx.fillStyle = "#" + col;
             ctx.fillRect(pxX - radius, pxY - radius, dblSize, dblSize);
             count++;
         }
 
         // draw the selection as black rectangles
-        if (fatIdx === null) {
-            ctx.globalAlpha = 0.7;
-            ctx.fillStyle = "black";
-            selCells.forEach(function(cellId) {
-                let pxX = pxCoords[2 * cellId];
-                let pxY = pxCoords[2 * cellId + 1];
+        ctx.globalAlpha = 0.7;
+        ctx.fillStyle = "black";
+        if (selCells !== null)
+            for (i = 0; i < selCells.length; i++) {
+                var cellId = selCells[i];
+                var pxX = pxCoords[2 * cellId];
+                var pxY = pxCoords[2 * cellId + 1];
                 ctx.fillRect(pxX - radius, pxY - radius, dblSize, dblSize);
                 count += 1;
-            })
-        }
-        debug(count + " rectangles drawn (including selection)");
+            }
+        console.log(count + " rectangles drawn (including selection)");
         ctx.restore();
-        return count;
     }
 
-    function drawCirclesStupid(ctx, pxCoords, coordColors, colors, radius, alpha, selCells, fatIdx) {
-        /* TOO SLOW - Only used in testing/for demos. Not used anywhere else. Draw circles onto canvas with very slow functions.. */
-        debug("Drawing " + coordColors.length + " circles with stupid renderer");
+    function drawCirclesStupid(ctx, pxCoords, coordColors, colors, radius, alpha, selCells) {
+        /* draw little circles onto canvas. pxCoords are the centers.  */
+        console.log("Drawing " + coordColors.length + " circles with stupid renderer");
         ctx.globalAlpha = alpha;
         var dblSize = 2 * radius;
-        var count = 0;
         for (var i = 0; i < pxCoords.length / 2; i++) {
             var pxX = pxCoords[2 * i];
             var pxY = pxCoords[2 * i + 1];
-            if (isHidden(pxX, pxY))
-                continue;
-            var valIdx = coordColors[i];
-            var col = colors[valIdx];
-            if (fatIdx !== null && valIdx !== fatIdx)
-                col = nonFatColor;
-
+            var col = colors[coordColors[i]];
             ctx.fillStyle = "#" + col;
+            //ctx.fillRect(pxX-size, pxY-size, dblSize, dblSize);
             ctx.beginPath();
             ctx.arc(pxX, pxY, radius, 0, 2 * Math.PI);
             ctx.closePath();
             ctx.fill();
-            count++;
         }
-        return count;
     }
 
     function intersectRect(r1left, r1right, r1top, r1bottom, r2left, r2right, r2top, r2bottom) {
-        /* return true if two rectangles overlap,
+        /* return true if two rectangles overlap, 
        https://stackoverflow.com/questions/2752349/fast-rectangle-to-rectangle-intersection
 	*/
         return !(r2left > r1right || r2right < r1left || r2top > r1bottom || r2bottom < r1top);
     }
 
-    function drawLines(ctx, pxLines, width, height, attrs) {
-        /* draw lines defined by array with (x1, y1, x2, y2) arrays.
-         * color is a CSS name, so usually prefixed by # if a hexcode
-         * width is the width in pixels.
-         * */
-        ctx.save();
-        //ctx.globalAlpha = 1.0;
-
-        ctx.strokeStyle = attrs.lineColor || "#888888";
-        ctx.lineWidth = attrs.lineWidth || 3;
-        ctx.globalAlpha = attrs.lineAlpha || 0.5;
-        //ctx.miterLimit =2;
-        //ctx.strokeStyle = "rgba(200, 200, 200, 0.3)";
-
-        for (var i = 0; i < pxLines.length; i++) {
-            var line = pxLines[i];
-            var x1 = line[0];
-            var y1 = line[1];
-            var x2 = line[2];
-            var y2 = line[3];
-
-            ctx.beginPath();
-            ctx.moveTo(x1, y1);
-            ctx.lineTo(x2, y2);
-            ctx.stroke();
-        }
-        ctx.restore();
-    }
-
-    function drawLabelsSvg(svgLines, labelCoords, winWidth, winHeight, zoomFact) {
-        /* given an array of [x, y, text], draw the text. returns bounding
-         * boxes as array of [x1, y1, x2, y2]  */
-
-        for (var i = 0; i < labelCoords.length; i++) {
-            var coord = labelCoords[i];
-            if (coord === null) { // outside of view range, push a null to avoid messing up the order of bboxArr
-                continue;
-            }
-
-            var x = coord[0];
-            var y = coord[1];
-            var text = coord[2];
-
-            // don't draw labels where the midpoint is off-screen
-            if (x < 0 || y < 0 || x > winWidth || y > winHeight) {
-                continue;
-            }
-
-            svgLines.push("<text font-family='sans-serif' font-size='" + (gTextSize + 2) + "' fill='black' text-anchor='middle' x='" + x + "' y='" + y + "'>" + text + "</text>");
-        }
-
-    }
-
-    self.drawLegendSvg = function(legend) {
-        /* draw a legend onto the SVG given a legend object. */
-        var legWidth = self.svgLabelWidth;
-        var svgLines = self.svgLines;
-
-        var rows = legend.rows;
-
-        var legTitle = legend.title;
-        var subTitle = legend.subTitle;
-
-        var left = self.canvas.width; // x position where legend starts
-
-        var lineHeight = gTextSize;
-
-        var x = left + 11;
-        var y = lineHeight;
-        svgLines.push("<text font-family='sans-serif' font-size='" + gTextSize + "' fill='black' x='" + x + "' y='" + y + "'>" + legTitle + "</text>");
-        y += lineHeight;
-
-        if (subTitle) {
-            svgLines.push("<text font-family='sans-serif' font-size='" + gTextSize + "' fill='black' text-anchor='middle' x='" + x + "' y='" + y + "'>" + subTitle + "</text>");
-            y += lineHeight;
-        }
-
-        y += lineHeight;
-
-        // get the sum of all rows, to calculate frequency
-        // this code was copied from buildLegend -> refactor one day
-        var sum = 0;
-        for (var i = 0; i < rows.length; i++) {
-            let count = rows[i].count;
-            sum += count;
-        }
-
-        for (i = 0; i < rows.length; i++) {
-            // a lot was copied from cellBrowser:buildLegend(), could use some refactoring to reduce duplication
-            var row = rows[i];
-            var colorHex = row.color; // manual color
-            if (colorHex === null)
-                colorHex = row.defColor; // default color
-
-            var label = row.label;
-            var longLabel = row.longLabel;
-
-            let count = row.count;
-            var valueIndex = row.intKey;
-            var freq = 100 * count / sum;
-
-            if (count === 0) // never output categories with 0 count.
-                continue;
-
-            // this was copied from cellbrowser:buildLegend - refactor soon
-            label = label.replace(/_/g, " ").replace(/'/g, "&#39;").trim();
-            if (label === "") {
-                label = "(empty)";
-            }
-            label = label.replace("&ndash;", "-");
-
-            // draw colored rectangle first
-
-            var textSize = gTextSize - 3;
-
-            svgLines.push("<rect width='15' height='15' fill='#" + colorHex + "' x='" + x + "' y='" + y + "'></rect>");
-
-            var prec = 1;
-            if (freq < 1)
-                prec = 2;
-
-            //var lineCount = 0;
-            //svgLines.push("<text font-family='sans-serif' font-size='"+textSize+"' fill='black' text-anchor='start' x='"+(x+18)+"' y='"+((y-4)+lineCount*textSize)+"'>"+label+"</text>");
-            svgLines.push("<text font-family='sans-serif' font-size='" + textSize + "' fill='black' text-anchor='start' x='" + (x + 18) + "' y='" + (y + 8) + "'>" + label + "</text>");
-            //}
-            svgLines.push("<text font-family='sans-serif' font-size='" + textSize + "' fill='black' text-anchor='end' x='" + (left + legWidth - 3) + "' y='" + (y + 15) + "'>" + freq.toFixed(prec) + "%</text>");
-            y += textSize;
-
-        }
-        // cannot draw violin plots in SVG - no library for it
-    };
-
     function drawLabels(ctx, labelCoords, winWidth, winHeight, zoomFact) {
         /* given an array of [x, y, text], draw the text. returns bounding
          * boxes as array of [x1, y1, x2, y2]  */
 
         console.time("labels");
         ctx.save();
         ctx.font = "bold " + gTextSize + "px Sans-serif"
@@ -1064,109 +613,140 @@
         ctx.textAlign = "left";
 
         var addMargin = 1; // how many pixels to extend the bbox around the text, make clicking easier
         var bboxArr = []; // array of click hit boxes
 
         for (var i = 0; i < labelCoords.length; i++) {
             var coord = labelCoords[i];
-            if (coord === null) { // outside of view range, push a null to avoid messing up the order of bboxArr
+            if (coord === null) { // outside of view range
                 bboxArr.push(null);
-                continue;
+                continue
             }
 
             var x = coord[0];
             var y = coord[1];
             var text = coord[2];
 
             var textWidth = Math.round(ctx.measureText(text).width);
             // move x to the left, so text is centered on x
             x = x - Math.round(textWidth * 0.5);
 
+            // don't draw labels where the midpoint is off-screen
+            if (x < 0 || y < 0 || x > winWidth || y > winWidth) {
+                bboxArr.push(null);
+                continue;
+            }
+
             var textX1 = x;
             var textY1 = y;
             var textX2 = Math.round(x + textWidth);
             var textY2 = y + gTextSize;
 
-            // don't draw labels where the midpoint is off-screen
-            if (x < 0 || y < 0 || x > winWidth || y > winHeight) {
-                bboxArr.push(null);
-                continue;
+            if (zoomFact === 1.0) {
+                // at 100% zoom, make some minimal effort to keep labels on screen
+                if (x < 0)
+                    x = 0;
+                if ((x + textWidth) > winWidth)
+                    x = winWidth - textWidth;
+                if (y + gTextSize > winHeight)
+                    y = winHeight - gTextSize;
+
+                // also only at 100% zoom, make a minimal effort to avoid label overlaps
+                // a perfect solution would take much more time
+                for (var j = 0; j < bboxArr.length; j++) {
+                    var bbox = bboxArr[j];
+                    if (bbox === null) // = outside of screen
+                        continue;
+                    var bx1 = bbox[0];
+                    var by1 = bbox[1];
+                    var bx2 = bbox[2];
+                    var by2 = bbox[3];
+                    if (intersectRect(textX1, textX2, textY1, textY2, bx1, bx2, by1, by2)) {
+                        // push the overlapping label away a little
+                        var diff = Math.round(0.75 * gTextSize);
+                        if (textY1 < by1)
+                            y -= diff;
+                        else
+                            y += diff;
+                    }
+                }
             }
 
-
             ctx.strokeText(text, x, y);
             ctx.fillText(text, x, y);
 
             bboxArr.push([textX1 - addMargin, textY1 - addMargin, textX2 + addMargin, textY2 + addMargin]);
         }
         ctx.restore();
         console.timeEnd("labels");
         return bboxArr;
     }
 
-    // function drawLabels_dom(ctx, labelCoords, isFull) {
-    //     /* given an array of [x, y, text], draw the text. returns bounding boxes as array of [x1, y1, x2, y2]  */
-    //     for (var i=0; i < labelCoords.length; i++) {
-    //         var coord = labelCoords[i];
-    //         var x = coord[0];
-    //         var y = coord[1];
-    //         var text = coord[2];
-
-    //         var div = document.createElement('div');
-    //         div.id = id;
-    //         //div.style.border = "1px solid #DDDDDD";
-    //         div.style.backgroundColor = "rgb(230, 230, 230, 0.6)";
-    //         div.style.width = width+"px";
-    //         div.style.height = height+"px";
-    //         div.style["text-align"]="center";
-    //         div.style["vertical-align"]="middle";
-    //         div.style["line-height"]=height+"px";
-    //     }
-    //     ctx.restore();
-    //     return bboxArr;
-    // }
+    function drawLabels_dom(ctx, labelCoords, isFull) {
+        /* given an array of [x, y, text], draw the text. returns bounding boxes as array of [x1, y1, x2, y2]  */
+        for (var i = 0; i < labelCoords.length; i++) {
+            var coord = labelCoords[i];
+            var x = coord[0];
+            var y = coord[1];
+            var text = coord[2];
+
+            var div = document.createElement('div');
+            div.id = id;
+            //div.style.border = "1px solid #DDDDDD";
+            div.style.backgroundColor = "rgb(230, 230, 230, 0.6)";
+            div.style.width = width + "px";
+            div.style.height = height + "px";
+            div.style["text-align"] = "center";
+            div.style["vertical-align"] = "middle";
+            div.style["line-height"] = height + "px";
+        }
+        ctx.restore();
+        return bboxArr;
+    }
 
     // https://stackoverflow.com/questions/5560248/programmatically-lighten-or-darken-a-hex-color-or-rgb-and-blend-colors
     function shadeColor(color, percent) {
         var f = parseInt(color, 16),
             t = percent < 0 ? 0 : 255,
             p = percent < 0 ? percent * -1 : percent,
             R = f >> 16,
             G = f >> 8 & 0x00FF,
             B = f & 0x0000FF;
         return (0x1000000 + (Math.round((t - R) * p) + R) * 0x10000 + (Math.round((t - G) * p) + G) * 0x100 + (Math.round((t - B) * p) + B)).toString(16).slice(1);
     }
 
-    function makeTemplates(radius, tileWidth, tileHeight, colors, fatIdx) {
-        /* create an off-screen-canvas with the circle-templates that will be stamped later onto the bigger canvas 
-         * Add one final circle at the end with the outline, for the selection. */
-        var colCount = colors.length;
-        var off = document.createElement('canvas'); // not added to DOM, will be gc'ed
-
-        if (fatIdx !== null) {
-            colCount = 2;
-            colors = [colors[fatIdx], nonFatColorCircles];
-        }
+    function drawCirclesDrawImage(ctx, pxCoords, coordColors, colors, radius, alpha, selCells) {
+        /* predraw and copy circles into canvas. pxCoords are the centers.  */
+        // almost copied from by https://stackoverflow.com/questions/13916066/speed-up-the-drawing-of-many-points-on-a-html5-canvas-element
+        // around 2x faster than drawing full circles
+        // create an off-screen canvas
 
-        off.width = (colCount + 1) * tileWidth;
+        ctx.save();
+        console.log("Drawing " + coordColors.length + " coords with drawImg renderer, radius=" + radius);
+        var off = document.createElement('canvas'); // not added to DOM, will be gc'ed
+        var diam = Math.round(2 * radius);
+        var tileWidth = diam + 2; // must add one pixel on each side, space for antialising
+        var tileHeight = tileWidth; // otherwise circles look cut off
+        off.width = (colors.length + 1) * tileWidth;
         off.height = tileHeight;
         var ctxOff = off.getContext('2d');
 
         //pre-render circles into the off-screen canvas.
         for (var i = 0; i < colors.length; ++i) {
+            //ctxOff.lineWidth=1;
             ctxOff.fillStyle = "#" + colors[i];
             ctxOff.beginPath();
             // arc(x, y, r, 0, 2*pi)
             ctxOff.arc(i * tileWidth + radius + 1, radius + 1, radius, 0, 2 * Math.PI);
             ctxOff.closePath();
             ctxOff.fill();
 
             // only draw outline for big circles
-            if (radius > 5) {
-                ctxOff.lineWidth = 1.0;
+            ctxOff.lineWidth = 1.0;
+            if (radius > 6) {
                 var strokeCol = "#" + shadeColor(colors[i], 0.9);
                 ctxOff.strokeStyle = strokeCol;
 
                 ctxOff.beginPath();
                 ctxOff.arc(i * tileWidth + radius + 1, radius + 1, radius, 0, 2 * Math.PI);
                 ctxOff.closePath();
                 ctxOff.stroke();
@@ -1179,97 +759,49 @@
         ctxOff.lineWidth = 2;
         ctxOff.strokeStyle = "black";
         ctxOff.beginPath();
         // args: arc(x, y, r, 0, 2*pi)
         ctxOff.arc((selImgId * tileWidth) + radius + 1, radius + 1, radius - 1, 0, 2 * Math.PI);
         ctxOff.stroke();
 
-        return off;
-    }
-
-    function blitTwo(ctx, off, pxCoords, coordColors, tileWidth, tileHeight, radius, fatIdx, selImgId) {
-        /* blit only the fatIdx circle in color, and all the rest in grey. Also draw selection circles. */
-        var count = 0;
-        for (let i = 0; i < pxCoords.length / 2; i++) {
-            var pxX = pxCoords[2 * i];
-            var pxY = pxCoords[2 * i + 1];
-            if (isHidden(pxX, pxY))
-                continue;
-            var col = coordColors[i];
-            if (col === fatIdx)
-                col = 0;
-            else
-                col = 1;
-            count++;
-            ctx.drawImage(off, col * tileWidth, 0, tileWidth, tileHeight, pxX - radius - 1, pxY - radius - 1, tileWidth, tileHeight);
-
-            if (radius >= 5)
-                ctx.drawImage(off, selImgId * tileWidth, 0, tileWidth, tileHeight, pxX - radius - 1, pxY - radius - 1, tileWidth, tileHeight);
-        }
-        return count;
-    }
+        if (alpha !== undefined)
+            ctx.globalAlpha = alpha;
 
-    function blitAll(ctx, off, pxCoords, coordColors, tileWidth, tileHeight, radius) {
-        /* blit the circles onto the main canvas, using all colors */
+        // blit the circles onto the main canvas
         var count = 0;
-        for (let i = 0; i < pxCoords.length / 2; i++) {
+        for (var i = 0; i < pxCoords.length / 2; i++) {
             var pxX = pxCoords[2 * i];
             var pxY = pxCoords[2 * i + 1];
-            if (isHidden(pxX, pxY))
+            if (pxX === 0 && pxY === 0)
                 continue;
             var col = coordColors[i];
             count++;
             // drawImage(img,sx,sy,swidth,sheight,x,y,width,height);
             ctx.drawImage(off, col * tileWidth, 0, tileWidth, tileHeight, pxX - radius - 1, pxY - radius - 1, tileWidth, tileHeight);
         }
-        //debug(count +" circles drawn");
-        return count;
-    }
-
-
-    function drawCirclesDrawImage(ctx, pxCoords, coordColors, colors, radius, alpha, selCells, fatIdx) {
-        /* predraw and copy circles into canvas. pxCoords are the centers.  */
-        // almost copied from by https://stackoverflow.com/questions/13916066/speed-up-the-drawing-of-many-points-on-a-html5-canvas-element
-        // around 2x faster than drawing full circles by using an off-screen canvas
-
-        debug("Drawing " + coordColors.length + " coords with drawImg renderer, radius=" + radius);
-
-        var diam = Math.round(2 * radius);
-        var tileWidth = diam + 2; // must add one pixel on each side, space for antialising
-        var tileHeight = tileWidth; // otherwise circles look cut off
-
-        let off = makeTemplates(radius, tileWidth, tileHeight, colors, fatIdx);
-
-        ctx.save();
-        if (alpha !== undefined)
-            ctx.globalAlpha = alpha;
-
-        let count = 0;
-        if (fatIdx !== null)
-            count = blitTwo(ctx, off, pxCoords, coordColors, tileWidth, tileHeight, radius, fatIdx, selImgId);
-        else
-            count = blitAll(ctx, off, pxCoords, coordColors, tileWidth, tileHeight, radius);
 
         // overdraw the selection as solid black circle outlines
         ctx.globalAlpha = 0.7;
-        var selImgId = colors.length;
-        selCells.forEach(function(cellId) {
-            let pxX = pxCoords[2 * cellId];
-            let pxY = pxCoords[2 * cellId + 1];
-            if (isHidden(pxX, pxY))
-                return;
-            // make sure that old leftover overlapping black circles don't shine through and redraw the circle
-            // slow, but not sure what else I can do...
-            let col = coordColors[cellId];
-            ctx.drawImage(off, col * tileWidth, 0, tileWidth, tileHeight, pxX - radius - 1, pxY - radius - 1, tileWidth, tileHeight);
-            ctx.drawImage(off, selImgId * tileWidth, 0, tileWidth, tileHeight, pxX - radius - 1, pxY - radius - 1, tileWidth, tileHeight);
-        })
+        if (selCells !== null) {
+            for (i = 0; i < selCells.length; i++) {
+                var cellId = selCells[i];
+                var pxX = pxCoords[2 * cellId];
+                var pxY = pxCoords[2 * cellId + 1];
+                if (pxX === 0 && pxY === 0)
+                    continue;
+                // make sure that old leftover overlapping black circles don't shine through
+                var col = coordColors[cellId];
+                ctx.drawImage(off, col * tileWidth, 0, tileWidth, tileHeight, pxX - radius - 1, pxY - radius - 1, tileWidth, tileHeight);
 
+                ctx.drawImage(off, selImgId * tileWidth, 0, tileWidth, tileHeight, pxX - radius - 1, pxY - radius - 1, tileWidth, tileHeight);
+            }
+        }
+
+        console.log(count + " circles drawn");
         ctx.restore();
-        return count;
     }
 
     function hexToInt(colors) {
         /* convert a list of hex values to ints */
         var intList = [];
         for (var i = 0; i < colors.length; i++) {
             var colHex = colors[i];
@@ -1291,15 +823,15 @@
         var rgbColors = hexToInt(colors);
         var invAlpha = 1.0 - alpha;
 
         // alpha-blend pixels into array
         for (var i = 0; i < pxCoords.length / 2; i++) {
             var pxX = pxCoords[2 * i];
             var pxY = pxCoords[2 * i + 1];
-            if (isHidden(pxX, pxY))
+            if (pxX === 0 && pxY === 0)
                 continue;
             var p = 4 * (pxY * width + pxX); // pointer to red value of pixel at x,y
 
             var oldR = cData[p];
             var oldG = cData[p + 1];
             var oldB = cData[p + 2];
 
@@ -1315,113 +847,68 @@
             cData[p] = mixR;
             cData[p + 1] = mixG;
             cData[p + 2] = mixB;
             cData[p + 3] = 255; // no transparency... ever?
         }
     }
 
-    function drawBackground(ctx, back) {
-        /* draw the background image onto the canvas ctx */
-        if (!back)
-            return;
-        console.time("image");
-        //var ctxWidth = ctx.canvas.width; // size of the canvas on the screen in pixels
-        //var ctxHeight = ctx.canvas.height;
-
-        //var clipWidth = backuwidth;
-        //var clipHeight = back.height;
-
-        // arguments are: (imgObject, x/y coord on image for clipping, width / height of clipped image, where to place the image, width/height of image)
-        //var a = getSafeRect(back.image.width, back.image.height, back.clipX, back.clipY, back.image.width, back.image.height, 0, 0, ctxWidth, ctxHeight);
-        //console.log("drawing fixed coords", a.sx, a.sy, a.sw, a.sh, a.dx, a.dy, a.dw, a.dh);
-        //self.ctx.drawImage(back.image, a.sx, a.sy, a.sw, a.sh, a.dx, a.dy, a.dw, a.dh);
-        //self.ctx.drawImage(back.image, a.sx, a.sy, back.width, back.height, a.dx, a.dy, a.dw, a.dh);
-        console.log("drawImage sx, sy, sw, sh, dx, dy, dw, dh", back.sx, back.sy, back.sw, back.sh, back.dx, back.dy, back.dw, back.dh);
-        //self.ctx.drawImage(back.image, back.sx, back.sy, back.width, back.height, 0, 0, ctxWidth, ctxHeight);
-        self.ctx.drawImage(back.image, back.sx, back.sy, back.sw, back.sh, back.dx, back.dy, back.dw, back.dh);
-
-        console.timeEnd("image");
-    }
-
-
-    function drawPixels(ctx, width, height, pxCoords, coordColors, colors, alpha, selCells, fatIdx) {
+    function drawPixels(ctx, width, height, pxCoords, colorArr, colors, alpha, selCells) {
         /* draw single pixels into a pixel buffer and copy the buffer into a canvas */
 
         // by default the canvas has black pixels
         // so not doing: var canvasData = ctx.createImageData(width, height);
         // XX is this really faster than manually zero'ing the array?
         var canvasData = ctx.getImageData(0, 0, width, height);
         var cData = canvasData.data;
 
         var rgbColors = hexToInt(colors);
         var invAlpha = 1.0 - alpha;
 
-        var count = 0;
-
         // alpha-blend pixels into array
         for (var i = 0; i < pxCoords.length / 2; i++) {
             var pxX = pxCoords[2 * i];
             var pxY = pxCoords[2 * i + 1];
-            if (isHidden(pxX, pxY))
+            if (pxX === 0 && pxY === 0)
                 continue;
             var p = 4 * (pxY * width + pxX); // pointer to red value of pixel at x,y
 
-            var valIdx = coordColors[i];
+            var oldR = cData[p];
+            var oldG = cData[p + 1];
+            var oldB = cData[p + 2];
+
+            var newRgb = rgbColors[colorArr[i]];
+            var newR = (newRgb >>> 16) & 0xff;
+            var newG = (newRgb >>> 8) & 0xff;
+            var newB = (newRgb) & 0xff;
 
-            if (fatIdx !== null) {
-                // fattening mode: fat cluster is black, all the rest is grey
-                let grey;
-                if (valIdx !== fatIdx)
-                    grey = 0xDD;
-                else
-                    grey = 0;
-
-                cData[p] = grey;
-                cData[p + 1] = grey;
-                cData[p + 2] = grey;
-                cData[p + 3] = 255; // no transparency... ever?
-            } else {
-                // normal colors
-                var oldR = cData[p];
-                var oldG = cData[p + 1];
-                var oldB = cData[p + 2];
-
-                var newRgb = rgbColors[valIdx];
-                var newR = (newRgb >>> 16) & 0xff;
-                var newG = (newRgb >>> 8) & 0xff;
-                var newB = (newRgb) & 0xff;
-
-                var mixR = ~~(oldR * invAlpha + newR * alpha);
-                var mixG = ~~(oldG * invAlpha + newG * alpha);
-                var mixB = ~~(oldB * invAlpha + newB * alpha);
-
-                cData[p] = mixR;
-                cData[p + 1] = mixG;
-                cData[p + 2] = mixB;
-                cData[p + 3] = 255; // no transparency... ever?
-            }
-            count++;
+            var mixR = ~~(oldR * invAlpha + newR * alpha);
+            var mixG = ~~(oldG * invAlpha + newG * alpha);
+            var mixB = ~~(oldB * invAlpha + newB * alpha);
+
+            cData[p] = mixR;
+            cData[p + 1] = mixG;
+            cData[p + 2] = mixB;
+            cData[p + 3] = 255; // no transparency... ever?
         }
 
         // overdraw the selection as black pixels
-        if (fatIdx === null) {
-            selCells.forEach(function(cellId) {
-                let pxX = pxCoords[2 * cellId];
-                let pxY = pxCoords[2 * cellId + 1];
-                if (isHidden(pxX, pxY))
-                    return;
-                let p = 4 * (pxY * width + pxX); // pointer to red value of pixel at x,y
+        if (selCells !== null)
+            for (i = 0; i < selCells.length; i++) {
+                var cellId = selCells[i];
+                var pxX = pxCoords[2 * cellId];
+                var pxY = pxCoords[2 * cellId + 1];
+                if (pxX === 0 && pxY === 0)
+                    continue;
+                var p = 4 * (pxY * width + pxX); // pointer to red value of pixel at x,y
                 cData[p] = 0;
                 cData[p + 1] = 0;
                 cData[p + 2] = 0;
-            })
-        }
+            }
 
         self.ctx.putImageData(canvasData, 0, 0);
-        return count;
     }
 
     function findRange(coords) {
         /* find range of pairs-array and return obj with attributes minX/maxX/minY/maxY */
         var minX = 9999999;
         var maxX = -9999999;
         var minY = 9999999;
@@ -1445,581 +932,276 @@
         obj.maxY = maxY;
         return obj; // not needed, but more explicit
     }
 
     function clearCanvas(ctx, width, height) {
         /* clear with a white background */
         // jsperf says this is fastest on Chrome, and still OK-ish in FF
-        //console.time("clear");
+        console.time("clear");
         ctx.save();
         ctx.globalAlpha = 1.0;
         ctx.fillStyle = "rgb(255,255,255)";
         ctx.fillRect(0, 0, width, height);
         ctx.restore();
-        //console.timeEnd("clear");
+        console.timeEnd("clear");
     }
 
     // -- object methods (=access the self object)
 
     this.onZoom100Click = function(ev) {
         self.zoom100();
         self.drawDots();
     };
 
-    this.setBackground = function(img) {
-        /* */
-        if (self.background === undefined || self.background === null)
-            self.background = {};
-        self.background.image = img;
-        self.scaleBackground(self.background, self.port.initZoom, self.port.zoomRange);
-        if (self.childPlot)
-            self.childPlot.setBackground(img);
-    };
-
-    function getSafeRect(width, height, sx, sy, sw, sh, dx, dy, dw, dh) {
-        if (sw < 0) {
-            sx += sw;
-            sw = Math.abs(sw);
-        }
-        if (sh < 0) {
-            sy += sh;
-            sh = Math.abs(sh);
-        }
-        if (dw < 0) {
-            dx += dw;
-            dw = Math.abs(dw);
-        }
-        if (dh < 0) {
-            dy += dh;
-            dh = Math.abs(dh);
-        }
-        const x1 = Math.max(sx, 0);
-        const x2 = Math.min(sx + sw, width);
-        const y1 = Math.max(sy, 0);
-        const y2 = Math.min(sy + sh, height);
-        const w_ratio = dw / sw;
-        const h_ratio = dh / sh;
-
-    }
-
-    this.scaleBackground = function(background, dataRange, zoomRange) {
-        /* determine the (x,y,width,height) in pixels of the current rectangle of the background bitmap on the canvas */
-        if (!background)
-            return;
-
-        var width = background.image.width; // source image width
-        var height = background.image.height; // source image height
-
-        var ctxWidth = self.canvas.width;
-        var ctxHeight = self.canvas.height;
-
-        var coordHeight = dataRange.maxY - dataRange.minY;
-        var coordWidth = dataRange.maxX - dataRange.minX;
-
-        var scaleX = width / coordWidth; // this is px/dataUnit to convert background image pixels to canvas pixels
-        var scaleY = height / coordHeight;
-
-        var sx1 = zoomRange.minX * scaleX; // sx = x position on source image
-        var sx2 = zoomRange.maxX * scaleX;
-
-        var sy1 = (coordHeight - zoomRange.maxY) * scaleY; // Y-positions must be subtracted from coordHeight - y axis is flipped!
-        var sy2 = (coordHeight - zoomRange.minY) * scaleY; // Our y-axis is always flipped!
-
-        var sw = sx2 - sx1; // size of slice of background image that is currently shown, in source pixels
-        var sh = sy2 - sy1;
-
-        var ctxWidth = self.canvas.width;
-        var ctxHeight = self.canvas.height;
-
-        // lame: since I wasn't able to figure out how to transform negative sx, sy to corrected dx, dy, coords - safari doesn't understand negative sx/sy - I simply use the scaleData function
-        // somehow https://gist.github.com/Kaiido/ca9c837382d89b9d0061e96181d1d862 didn't work for me
-        //var coords = [0.0, 0.0, dataRange.maxX, dataRange.maxY];
-        //var newCoords = scaleCoords(coords, 0, zoomRange, ctxWidth, ctxHeight, [])
-
-        var dx = 0;
-        var dy = 0;
-        var dw = ctxWidth;
-        var dh = ctxHeight;
-
-        //if (sx1 < 0) {
-        //sx1 = 0;
-        //sw = width;
-        //dx = newCoords[0];
-        //dw = newCoords[2] - dx;
-        //}
-
-        //if (sy1 < 0) {
-        //sy1 = 0;
-        //sh = height;
-        //dy = newCoords[1];
-        //dh = newCoords[3] - dy;
-        //}
-
-        background.sx = sx1;
-        background.sy = sy1;
-        background.sw = sw;
-        background.sh = sh;
-
-        background.dx = dx;
-        background.dy = dy;
-        background.dw = dw;
-        background.dh = dh;
-    }
-
     this.scaleData = function() {
         /* scale coords and labels to current zoom range, write results to pxCoords and pxLabels */
-        if (!self.coords) // window resize can call this before coordinates are loaded.
-            return;
-
-        var borderMargin = self.port.radius;
-        self.calcRadius();
-
-        self.coords.px = scaleCoords(self.coords.orig, borderMargin, self.port.zoomRange, self.canvas.width, self.canvas.height);
-        if (self.coords.lines)
-            self.coords.pxLines = scaleLines(self.coords.lines, self.port.zoomRange, self.canvas.width, self.canvas.height);
-        self.scaleBackground(self.background, self.port.initZoom, self.port.zoomRange);
-        self.scalingDone = true;
-    }
-
-    this.readyToDraw = function() {
-        return (self.scalingDone)
-    }
+        var borderMargin = self.radius;
+        self.pxCoords = scaleCoords(self.coords, borderMargin, self.zoomRange, self.canvas.width, self.canvas.height);
 
-    this.setTopLeft = function(top, left) {
-        /* set top and left position in pixels of the canvas */
-        self.top = top;
-        self.left = left; // keep an integer version of these numbers
-        self.div.style.top = top + "px";
-        self.div.style.left = left + "px";
-
-        self.setSize(self.width, self.height, false); // resize the various buttons
+        self.pxLabels = null;
+        if (self.clusterLabels !== undefined && self.clusterLabels !== null)
+            self.pxLabels = scaleLabels(self.clusterLabels, self.zoomRange, borderMargin, self.canvas.width, self.canvas.height);
     }
 
-    this.quickResize = function(width, height) {
-        /* resize the canvas and move the status line, don't rescale or draw  */
-        self.div.style.width = width + "px";
-        self.div.style.height = height + "px";
-
-        // if in split screen mode, pass on the message to the second window
-        if (self.childPlot) {
-            width = width / 2;
-            //self.childPlot.left = self.left+width;
-            //self.childPlot.canvas.style.left = self.childPlot.left+"px";
-            self.childPlot.setPos(null, self.left + width);
-            self.childPlot.setSize(width, height, true);
-        }
+    this.setSize = function(width, height) {
+        /* resize canvas on the page re-scale the data and re-draw */
 
-        if (self.closeButton) {
-            self.closeButton.style.left = width - gCloseButtonFromRight;
-        }
+        // css and canvas sizes: these must be identical, otherwise canvas gets super slow
+        var canvWidth = width;
+        var canvHeight = height - gStatusHeight;
+        self.canvas.style.width = canvWidth + "px";
+        self.canvas.style.height = canvHeight + "px";
+        self.canvas.width = canvWidth;
+        self.canvas.height = canvHeight;
 
-        // css and actual canvas sizes: these must be identical, otherwise canvas gets super slow
-        self.canvas.style.width = width + "px";
         self.width = width;
         self.height = height;
-        //let canvHeight = height - gStatusHeight;
 
-        let canvHeight = height - gStatusHeight;
-        self.canvas.height = canvHeight;
-        self.canvas.width = width;
-        self.canvas.style.height = canvHeight + "px";
-        self.zoomDiv.style.top = (height - gZoomFromBottom) + "px";
-        self.zoomDiv.style.left = (gZoomFromLeft) + "px";
+        var zoomDiv = gebi('mpCtrls');
+        zoomDiv.style.top = (self.top + height - gZoomFromBottom) + "px";
+        zoomDiv.style.left = (self.left + width - gZoomFromRight) + "px";
 
-        // move status line, dataset name and radius/transparency sliders
         var statusDiv = self.statusLine;
-        statusDiv.style.top = (height - gStatusHeight) + "px";
+        statusDiv.style.top = (self.top + height - gStatusHeight) + "px";
         statusDiv.style.width = width + "px";
 
-        self.titleDiv.style.top = (height - gStatusHeight - gTitleSize) + "px";
-        if (self.sliderDiv)
-            self.sliderDiv.style.top = (height - gStatusHeight - gTitleSize) + "px";
+        self.titleDiv.style.top = (self.top + height - gStatusHeight - gTitleSize) + "px";
 
-    }
-
-    this.setPos = function(top, left) {
-        /* position canvas. Does not affect child  */
-        if (top) {
-            self.top = top;
-            self.div.style.top = top + "px";
-        }
-        if (left) {
-            self.left = left;
-            self.div.style.left = left + "px";
-        }
-    }
-
-    this.setSize = function(width, height, doRedraw) {
-        /* resize canvas on the page re-scale the data and re-draw, unless doRedraw is false */
-        if (width === null)
-            width = self.div.getBoundingClientRect().width;
-
-        self.quickResize(width, height);
-
-        if (self.coords)
-            self.scaleData();
-
-        if (doRedraw === undefined || doRedraw === true)
-            self.drawDots();
+        self.scaleData();
+        //clearCanvas(self.ctx, width, height);
+        self.drawDots();
     };
 
-    this.setCoords = function(coords, clusterLabels, coordInfo, opts) {
+    this.setCoords = function(coords, clusterLabels, minX, maxX, minY, maxY) {
         /* specify new coordinates of circles to draw, an array of (x,y) coordinates */
         /* Scale data to current screen dimensions */
         /* clusterLabels is optional: array of [x, y, labelString]*/
-        /* minX, maxX, etc are optional
-         * opts are optional arguments like radius, alpha etc, see initPlot/args */
-        self.scalingDone = false;
+        /* minX, maxX, etc are optional */
+        // "==null" checks for both undefined and null
         if (coords.length === 0)
             alert("cbDraw-setCoords called with no coordinates");
 
-        var minX = coordInfo.minX;
-        var maxX = coordInfo.maxX;
-        var minY = coordInfo.minY;
-        var maxY = coordInfo.maxY;
-        var useRaw = coordInfo.useRaw;
-
-        var coordOpts = cloneObj(self.globalOpts);
-        copyObj(opts, coordOpts);
-
-        var oldRadius = self.port.initRadius;
-        var oldAlpha = self.port.initAlpha;
-        var oldLabels = self.coords.pxLabels;
-        self.port = {};
-        self.initPort(coordOpts);
-        if (oldRadius)
-            self.port.initRadius = oldRadius;
-        if (oldAlpha)
-            self.port.initAlpha = oldAlpha;
-        self.coords = {};
-
-        self.coords.origAll = undefined;
-
-        var newZr = {};
         if (minX === undefined || maxX === undefined || minY === undefined || maxY === undefined)
-            newZr = findRange(coords);
-        else {
-            newZr = {
+            self.initZoom = findRange(coords);
+        else
+            self.initZoom = {
                 minX: minX,
                 maxX: maxX,
                 minY: minY,
                 maxY: maxY
-            };
-        }
-
-        // switch off any moving of the spots to the minimum position
-        if (useRaw) {
-            newZr.minX = 0.0;
-            newZr.minY = 0.0;
-        }
-
-        // we need the maximal min-max ranges of the original coordinates for later
-        copyObj(newZr, self.port.initZoom);
-        // the current min-max ranges of the values are the maximal values, so copy them = zoom 100%
-        copyObj(newZr, self.port.zoomRange);
-
-        self.coords.orig = coords;
-        self.coords.labels = clusterLabels;
-
-        var count = 0;
-        for (var i = 0; i < coords.length / 2; i++) {
-            var cellX = coords[i * 2];
-            var cellY = coords[i * 2 + 1];
-            if (!(isHidden(cellX, cellY)))
-                count++;
-        }
+            }
+        self.zoomRange = cloneObj(self.initZoom);
 
-        setStatus(count + " visible " + self.gSampleDescription + "s loaded");
+        self.coords = coords;
+        self.clusterLabels = clusterLabels;
+        setStatus((coords.length / 2) + " " + self.gSampleDescription + "s loaded");
 
-        if (opts.lines)
-            self._setLines(opts["lines"], opts);
         self.scaleData();
-    };
-
-    this.setLabelCoords = function(labelCoords) {
-        /* set the label coords and return true if there were any labels before */
-        var hadLabelsBefore = self.coords.labels.length > 0;
-        self.coords.labels = labelCoords;
-        return hadLabelsBefore;
+        if (self.radius === null || self.radius == undefined) {
+            self.radius = guessRadius(coords.length);
+            self.initRadius = self.radius;
+        }
     };
 
     this.setColorArr = function(colorArr) {
         /* set the color array, one array with one index per coordinate */
-        self.col.arr = colorArr;
+        self.colorArr = colorArr;
     };
 
     this.setColors = function(colors) {
         /* set the colors, one for each value of a in setColorArr(a). colors is an
          * array of six-digit hex strings. Not #-prefixed! */
-        self.col.pal = colors;
+        self.colors = colors;
     };
 
-    this.calcRadius = function() {
-        /* calculate the radius from current zoom factor and set radius, alpha and zoomFact in self.port */
-        // make the circles a bit smaller than expected
-        var zr = self.port.zoomRange;
-        var iz = self.port.initZoom;
-        var initAlpha = self.port.initAlpha;
-        var initSpan = iz.maxX - iz.minX;
-        var currentSpan = zr.maxX - zr.minX;
-        var zoomFact = initSpan / currentSpan;
-
-        // both radius and alpha can be change by a 'multiplier'
-        var alphaMult = self.port.alphaMult || 1.0;
-        var radiusMult = self.port.radiusMult || 1.0;
-
-        var baseRadius = self.port.initRadius;
-        if (baseRadius === 0)
-            baseRadius = 0.7;
-        var radius = Math.floor(baseRadius * Math.sqrt(zoomFact) * radiusMult);
-
-        // the higher the zoom factor, the higher the alpha value
-        var zoomFrac = Math.min(1.0, zoomFact / 100.0); // zoom as fraction, max is 1.0
-        var alpha = initAlpha + 3.0 * zoomFrac * (1.0 - initAlpha);
-        alpha = Math.min(0.8, alpha) * alphaMult;
-        debug("Zoom factor: ", zoomFact, ", Radius: " + radius + ", alpha: " + alpha);
-
-        if (self.onRadiusAlphaChange)
-            self.onRadiusAlphaChange(radiusMult, alphaMult);
-
-        self.port.zoomFact = zoomFact;
-        self.port.alpha = alpha;
-        self.port.alphaMult = alphaMult;
-        self.port.radius = radius;
-        self.port.radiusMult = radiusMult;
-    }
-
-    this.drawSvg = function(alpha, radius, coords, colArr, pal) {
-        self.svgLines = [];
-        var plotHeight = self.canvas.height;
-        var plotWidth = self.canvas.width;
-        var width = plotWidth + self.svgLabelWidth;
-        var height = 1500; // enough space for 100 lines in the legend
-        self.svgLines.push("<svg  xmlns='http://www.w3.org/2000/svg' height='" + height + "' width='" + width + "'>\n");
-        drawCirclesSvg(self.svgLines, coords, colArr, pal, radius, alpha, self.selCells);
-        if (self.doDrawLabels === true && self.coords.labels !== null && self.coords.labels !== undefined)
-            drawLabelsSvg(self.svgLines, self.coords.pxLabels, plotWidth, plotHeight, self.port.zoomFact);
-        // axis lines
-        self.svgLines.push('<line x1="2" y1="2" x2="2" y2="' + plotHeight + '" stroke="black" stroke-width="2"/>');
-        self.svgLines.push('<line x1="2" y1="2" x2="' + plotWidth + '" y2="2" stroke="black" stroke-width="2"/>');
-
-        // draw axis labels
-        var initZoom = self.port.initZoom;
-        // x axis
-        self.svgLines.push("<text font-family='sans-serif' font-size='" + (gTextSize) + "' fill='black' text-anchor='left' x='" + 10 + "' y='" + (gTextSize + 20) + "'>" + initZoom.minY + "</text>");
-        self.svgLines.push("<text font-family='sans-serif' font-size='" + (gTextSize) + "' fill='black' text-anchor='left' x='" + 10 + "' y='" + (plotHeight - gTextSize - 2) + "'>" + initZoom.maxY + "</text>");
-        // y axis
-        self.svgLines.push("<text font-family='sans-serif' font-size='" + (gTextSize) + "' fill='black' text-anchor='left' x='" + 10 + "' y='" + (gTextSize + 3) + "'>" + initZoom.minX + "</text>");
-        self.svgLines.push("<text font-family='sans-serif' font-size='" + (gTextSize) + "' fill='black' text-anchor='left' x='" + (plotWidth - 40) + "' y='" + (gTextSize + 3) + "'>" + initZoom.maxX + "</text>");
-        return;
-    }
+    //this.drawTitle = function() {
+    //var ctx = self.ctx;
+    //ctx.save();
+    //ctx.font = "bold "+gTextSize+"px Sans-serif"
+    //ctx.fillStyle = "rgba(220, 220, 220)";
+    //ctx.textBaseline = "top";
+    //ctx.fillText(self.title,5,self.height - gTextSize - 3); 
+    //ctx.restore();
+    //};
 
-    this.drawDots = function(doSvg) {
+    this.drawDots = function() {
         /* draw coordinates to canvas with current colors */
         console.time("draw");
 
         self.clear();
 
-        var radius = self.port.radius;
-        var alpha = self.port.alpha;
-        var zoomFact = self.port.zoomFact;
-        var coords = self.coords.px;
-        var pal = self.col.pal;
-        var colArr = self.col.arr;
-        var count = 0;
+        //if (self.title!==undefined)
+        //self.drawTitle();
 
-        if (alpha === undefined)
+        if (self.alpha === undefined)
             alert("internal error: alpha is not defined");
-        if (coords === null)
+        if (self.pxCoords === null)
             alert("internal error: cannot draw if coordinates are not set yet");
-        if (colArr.length !== (coords.length >> 1))
-            alert("internal error: cbDraw.drawDots - colorArr is not 1/2 of coords array. Got " + pal.length + " color values but coordinates for " + (coords.length / 2) + " cells.");
+        if (self.colorArr.length !== (self.pxCoords.length >> 1))
+            alert("internal error: cbDraw.drawDots - colorArr is not 1/2 of coords array. Got " + self.colors.length + " color values but coordinates for " + (self.pxCoords.length / 2) + " cells.");
 
-        if (doSvg !== undefined) {
-            self.drawSvg(alpha, radius, coords, colArr, pal);
-            return;
-        }
+        self.zoomFact = ((self.initZoom.maxX - self.initZoom.minX) / (self.zoomRange.maxX - self.zoomRange.minX));
 
-        drawBackground(self.ctx, self.background)
+        console.log("Zoom factor: " + self.zoomFact);
+        // make the circles a bit smaller than expected
+        var baseRadius = self.initRadius;
+        if (baseRadius === 0)
+            baseRadius = 0.7;
+        self.radius = Math.floor(baseRadius * Math.sqrt(self.zoomFact));
 
-        // if the labels are not shown, fattening should not be active
-        if (self.fatIdx && !self.doDrawLabels)
-            self.fatIdx = null;
-
-        if (radius === 0) {
-            count = drawPixels(self.ctx, self.canvas.width, self.canvas.height, coords,
-                colArr, pal, alpha, self.selCells, self.fatIdx);
-        } else if (radius === 1 || radius === 2) {
-            count = drawRect(self.ctx, coords, colArr, pal, radius, alpha, self.selCells, self.fatIdx);
+        // the higher the zoom factor, the higher the alpha value
+        var zoomFrac = Math.min(1.0, self.zoomFact / 100.0); // zoom as fraction, max is 1.0
+        var alpha = self.alpha + 3.0 * zoomFrac * (1.0 - self.alpha);
+        alpha = Math.min(0.8, alpha);
+        console.log("Radius: " + self.radius + ", alpha: " + alpha);
+
+        if (self.radius === 0) {
+            drawPixels(self.ctx, self.canvas.width, self.canvas.height, self.pxCoords,
+                self.colorArr, self.colors, alpha, self.selCells);
+        } else if (self.radius === 1 || self.radius === 2) {
+            drawRect(self.ctx, self.pxCoords, self.colorArr, self.colors, self.radius, alpha, self.selCells);
         } else {
+
             switch (self.mode) {
                 case 0:
-                    count = drawCirclesStupid(self.ctx, coords, colArr, pal, radius, alpha, self.selCells, self.fatIdx);
+                    drawCirclesStupid(self.ctx, self.pxCoords, self.colorArr, self.colors, self.radius, alpha, self.selCells);
                     break;
                 case 1:
-                    count = drawCirclesDrawImage(self.ctx, coords, colArr, pal, radius, alpha, self.selCells, self.fatIdx);
+                    drawCirclesDrawImage(self.ctx, self.pxCoords, self.colorArr, self.colors, self.radius, alpha, self.selCells);
                     break;
                 case 2:
                     break;
             }
         }
 
-        self.count = count;
-
         console.timeEnd("draw");
 
-        if (self.coords.pxLines) {
-            console.time("draw lines");
-            drawLines(self.ctx, self.coords.pxLines, self.canvas.width, self.canvas.height, self.coords.lineAttrs);
-            console.timeEnd("draw lines");
-        }
-
-        if (self.doDrawLabels === true && self.coords.labels !== null && self.coords.labels !== undefined) {
-            self.redrawLabels();
-        }
-
-        if (self.childPlot)
-            self.childPlot.drawDots();
-    };
-
-    this.getSvgText = function() {
-        /* close and return the accumulated svg lines and clear the svg line buffer */
-        var svgLines = self.svgLines;
-        svgLines.push("</svg>\n");
-        self.svgLines = null;
-        return svgLines;
-    }
-
-    this.redrawLabels = function() {
-        /* draw only the labels */
-        self.coords.pxLabels = scaleLabels(
-            self.coords.labels,
-            self.port.zoomRange,
-            self.port.radius,
-            self.canvas.width,
-            self.canvas.height
-        );
-        self.coords.labelBbox = drawLabels(
-            self.ctx,
-            self.coords.pxLabels,
-            self.canvas.width,
-            self.canvas.height,
-            self.port.zoomFact
-        );
+        if (self.doDrawLabels === true && self.pxLabels !== null) {
+            self.pxLabelBbox = drawLabels(self.ctx, self.pxLabels, self.canvas.width, self.canvas.height, self.zoomFact);
+        }
     };
 
     this.cellsAtPixel = function(x, y) {
         /* return the Ids of all cells at a particular pixel */
         var res = [];
-        var pxCoords = self.coords.px;
-        for (var i = 0; i < pxCoords.length / 2; i++) {
+        var pxCoords = self.pxCoords;
+        for (var i = 0; i < self.pxCoords.length / 2; i++) {
             var cellX = pxCoords[i * 2];
             var cellY = pxCoords[i * 2 + 1];
             if (cellX === x || cellY === y)
                 res.push(i);
         }
         return res;
     };
 
     this.cellsInRect = function(x1, y1, x2, y2) {
         /* return the Ids of all cells within certain pixel boundaries */
         var res = [];
-        var pxCoords = self.coords.px;
-        for (var i = 0; i < pxCoords.length / 2; i++) {
+        var pxCoords = self.pxCoords;
+        for (var i = 0; i < self.pxCoords.length / 2; i++) {
             var cellX = pxCoords[i * 2];
             var cellY = pxCoords[i * 2 + 1];
             if ((cellX >= x1) && (cellX <= x2) && (cellY >= y1) && (cellY <= y2))
                 res.push(i);
         }
         return res;
     };
 
-    this.resetAlpha = function() {
-        self.port.alphaMult = 1.0;
-        $('#mpAlphaSlider').slider({
-            value: 4
-        });
-        self.calcRadius();
-    };
-
-    this.resetRadius = function() {
-        self.port.radiusMult = 1.0;
-        $('#mpRadiusSlider').slider({
-            value: 4
-        });
-        self.calcRadius();
-    };
-
-    this.setRadiusAlpha = function(radius, alpha) {
-        self.port.radiusMult = radius;
-        self.port.alphaMult = alpha;
-        self.calcRadius();
-    };
+    //this.setSelection = function (idList) {
+    /* select some dots. idList is a list of integers. Specify null to clear. */
+    //self.selCells = new FastBitSet(idList);
+    //};
 
     this.zoom100 = function() {
         /* zoom to 100% and redraw */
-        copyObj(self.port.initZoom, self.port.zoomRange);
-        self.resetAlpha();
-        self.resetRadius();
+        self.zoomRange = cloneObj(self.initZoom);
         self.scaleData();
-        //self.drawDots();
+        self.radius = self.initRadius;
+        self.drawDots();
     };
 
     this.zoomTo = function(x1, y1, x2, y2) {
         /* zoom to rectangle defined by two points */
         // make sure that x1<x2 and y1<y2 - can happen if mouse movement was upwards
-        debug("Zooming to pixels: ", x1, y1, x2, y2);
         var pxMinX = Math.min(x1, x2);
         var pxMaxX = Math.max(x1, x2);
 
         var pxMinY = Math.min(y1, y2);
         var pxMaxY = Math.max(y1, y2);
 
-        var zoomRange = self.port.zoomRange;
+        // force the zoom rectangle to have the same aspect ratio as our canvas
+        // by adapting the height. This is what Microsoft software does
+        // It may be better to fix the aspect ratio of the zoom rectangle while zooming?
+        // We probably do not want to distort the ratio.
+        var aspectRatio = self.width / self.height;
+        var rectWidth = (pxMaxX - pxMinX);
+        var newHeight = rectWidth / aspectRatio;
+        pxMaxY = pxMinY + newHeight;
+
+        var zoomRange = self.zoomRange;
         // window size in data coordinates
         var spanX = zoomRange.maxX - zoomRange.minX;
         var spanY = zoomRange.maxY - zoomRange.minY;
 
         // multiplier to convert from pixels to data coordinates
-        var xMult = spanX / self.canvas.width; // multiplier dataRange/pixel
-        var yMult = spanY / self.canvas.height;
+        var xMult = spanX / self.width; // multiplier dataRange/pixel
+        var yMult = spanY / self.height;
 
         var oldMinX = zoomRange.minX;
         var oldMinY = zoomRange.minY;
 
         zoomRange.minX = oldMinX + (pxMinX * xMult);
         zoomRange.minY = oldMinY + (pxMinY * yMult);
 
         zoomRange.maxX = oldMinX + (pxMaxX * xMult);
         zoomRange.maxY = oldMinY + (pxMaxY * yMult);
 
-        self.port.zoomRange = zoomRange;
-        debug("Marquee zoom window: " + JSON.stringify(self.port.zoomRange));
+        self.zoomRange = zoomRange;
 
         self.scaleData();
     };
 
     this.zoomBy = function(zoomFact, xPx, yPx) {
-        /* zoom centered around xPx,yPx by a given factor. Returns new zoom range.
+        /* zoom centered around xPx,yPx by a given factor. Returns new zoom range. 
          * zoomFact = 1.2 means zoom +20%
          * zoomFact = 0.8 means zoom -20%
          * */
-        var zr = self.port.zoomRange;
-        var iz = self.port.initZoom;
+        var zr = self.zoomRange;
+        var iz = self.initZoom;
 
-        debug("old zoomfact " + self.port.zoomFact);
+        console.log("zoomfact " + self.zoomFact);
 
         var xRange = Math.abs(zr.maxX - zr.minX);
         var yRange = Math.abs(zr.maxY - zr.minY);
 
         var minWeightX = 0.5; // how zooming should be distributed between min/max
         var minWeightY = 0.5;
         if (xPx !== undefined) {
             minWeightX = (xPx / self.width);
-            minWeightY = (yPx / self.canvas.height);
+            minWeightY = (yPx / self.height);
         }
         var scale = (1.0 - zoomFact);
 
         var newRange = {};
         newRange.minX = zr.minX - (xRange * scale * minWeightX);
         newRange.maxX = zr.maxX + (xRange * scale * (1 - minWeightX));
 
@@ -2029,62 +1211,36 @@
 
         // extreme zoom factors don't make sense, at some point we reach
         // the limit of the floating point numbers
         var newZoom = ((iz.maxX - iz.minX) / (newRange.maxX - newRange.minX));
         if (newZoom < 0.01 || newZoom > 1500)
             return zr;
 
-        debug("x min max " + zr.minX + " " + zr.maxX);
-        debug("y min max " + zr.minY + " " + zr.maxY);
-
-        self.port.zoomRange = newRange;
+        console.log("x min max " + zr.minX + " " + zr.maxX);
+        console.log("y min max " + zr.minY + " " + zr.maxY);
 
+        self.zoomRange = newRange;
         self.scaleData();
-
-        // a special case for connected plots that are not sharing our pixel coordinates
-        if (self.childPlot && self.coords !== self.childPlot.coords) {
-            self.childPlot.zoomBy(zoomFact, xPx, yPx);
-        }
-
         return newRange;
     };
 
-    this.movePerc = function(xDiffFrac, yDiffFrac) {
-        /* move a certain percentage of current view. xDiff/yDiff are floats, e.g. 0.1 is 10% up */
-        var zr = self.port.zoomRange;
-        var xRange = Math.abs(zr.maxX - zr.minX);
-        var yRange = Math.abs(zr.maxY - zr.minY);
-
-        var xDiffAbs = xRange * xDiffFrac;
-        var yDiffAbs = yRange * yDiffFrac;
-
-        var newRange = {};
-        newRange.minX = zr.minX + xDiffAbs;
-        newRange.maxX = zr.maxX + xDiffAbs;
-        newRange.minY = zr.minY + yDiffAbs;
-        newRange.maxY = zr.maxY + yDiffAbs;
-
-        copyObj(newRange, self.port.zoomRange);
-        self.scaleData();
-    };
-
     this.panStart = function() {
         /* called when starting a panning sequence, makes a snapshop of the current image */
         self.panCopy = document.createElement('canvas'); // not added to DOM, will be gc'ed
         self.panCopy.width = self.canvas.width;
         self.panCopy.height = self.canvas.height;
         var destCtx = self.panCopy.getContext("2d", {
             alpha: false
         });
         destCtx.drawImage(self.canvas, 0, 0);
     }
 
     this.panBy = function(xDiff, yDiff) {
         /* pan current image by x/y pixels */
-        debug('panning by ' + xDiff + ' ' + yDiff);
+        console.log('panning by ' + xDiff + ' ' + yDiff);
 
         //var srcCtx = self.panCopy.getContext("2d", { alpha: false });
         clearCanvas(self.ctx, self.canvas.width, self.canvas.height);
         self.ctx.drawImage(self.panCopy, -xDiff, -yDiff);
         // keep these for panEnd
         self.panDiffX = xDiff;
         self.panDiffY = yDiff;
@@ -2094,685 +1250,395 @@
         /* end a sequence of panBy calls, called when the mouse is released */
         self.moveBy(self.panDiffX, -self.panDiffY); // -1 because of flipY
         self.panCopy = null;
         self.panDiffX = null;
         self.panDiffY = null;
     }
 
-    // BEGIN SELECTION METHODS (could be an object?)
-
-    this.selectClear = function(skipNotify) {
+    this.selectClear = function() {
         /* clear selection */
-        self.selCells.clear();
+        self.selCells = null;
         setStatus("");
-        if (self.onSelChange !== null && skipNotify !== true)
-            self.onSelChange(self.selCells);
+        if (self.onSelChange !== null)
+            self.onSelChange([]);
     };
 
     this.selectSet = function(cellIds) {
         /* set selection to an array of integer cellIds */
-        self.selCells.clear();
-        //self.selCells.push(...cellIds); // "extend" = array spread syntax, https://davidwalsh.name/spread-operator
-        let selCells = self.selCells;
-        for (let i = 0; i < cellIds.length; i++)
-            selCells.add(cellIds[i]);
+        self.selCells = cellIds;
         self._selUpdate();
     };
 
     this.selectAdd = function(cellIdx) {
         /* add a single cell to the selection. If it already exists, remove it. */
+        if (self.selCells === null) {
+            self.selCells = [cellIdx];
+            self._selUpdate();
+            return;
+        }
+
         console.time("selectAdd");
-        if (self.selCells.has(cellIdx))
-            self.selCells.delete(cellIdx);
+        var foundIdx = self.selCells.indexOf(cellIdx);
+        if (foundIdx === -1)
+            self.selCells.push(cellIdx);
         else
-            self.selCells.add(cellIdx);
+            self.selCells.splice(foundIdx, 1);
         console.time("selectAdd");
         self._selUpdate();
     };
 
-    this.selectAll = function(cellIdx) {
-        /* add all cells to selection */
-        var selCells = self.selCells;
-        var pxCoords = self.coords.px;
-        for (var i = 0, I = pxCoords.length / 2; i < I; i++) {
-            selCells.add(i);
-        }
-        self.selCells = selCells;
-        self._selUpdate();
-    };
-
     this.selectVisible = function() {
         /* add all visible cells to selection */
+        if (self.selCells === null)
+            self.selCells = [];
+
         var selCells = self.selCells;
-        var pxCoords = self.coords.px;
+        var pxCoords = self.pxCoords;
         for (var i = 0; i < pxCoords.length / 2; i++) {
             var pxX = pxCoords[2 * i];
             var pxY = pxCoords[2 * i + 1];
-            if (isHidden(pxX, pxY))
+            if (pxX === 0 && pxY === 0)
                 continue;
-            selCells.add(i);
+            selCells.push(i);
         }
         self.selCells = selCells;
         self._selUpdate();
     }
 
     this.selectByColor = function(colIdx) {
         /* add all cells with a given color to the selection */
-        var colArr = self.col.arr;
-        var selCells = self.selCells;
-        var cnt = 0;
-        for (var i = 0; i < colArr.length; i++) {
-            if (colArr[i] === colIdx) {
-                selCells.add(i);
-                cnt++;
-            }
-        }
-        self.selCells = selCells;
-        debug(cnt + " cells appended to selection, by color");
-        self._selUpdate();
-    };
-
-    this.unselectByColor = function(colIdx) {
-        /* remove all cells with a given color from the selection */
-        var colArr = self.col.arr;
+        var colArr = self.colorArr;
         var selCells = self.selCells;
-        var cnt = 0;
+        if (selCells === null)
+            selCells = [];
         for (var i = 0; i < colArr.length; i++) {
-            if (colArr[i] === colIdx) {
-                selCells.delete(i);
-                cnt++;
-            }
+            if (colArr[i] === colIdx)
+                selCells.push(i);
         }
-
         self.selCells = selCells;
-        debug(cnt + " cells removed from selection, by color");
+        console.log(self.selCells.length + " cells selected, by color");
         self._selUpdate();
     };
 
     this.selectInRect = function(x1, y1, x2, y2) {
         /* find all cells within a rectangle and add them to the selection. */
         var minX = Math.min(x1, x2);
         var maxX = Math.max(x1, x2);
 
         var minY = Math.min(y1, y2);
         var maxY = Math.max(y1, y2);
 
         console.time("select");
-        var pxCoords = self.coords.px;
+        if (self.selCells === null)
+            self.selCells = [];
+
+        var pxCoords = self.pxCoords;
         for (var i = 0; i < pxCoords.length / 2; i++) {
             var pxX = pxCoords[2 * i];
             var pxY = pxCoords[2 * i + 1];
-            if (isHidden(pxX, pxY))
+            if (pxX === 0 && pxY === 0)
                 continue;
             if ((minX <= pxX) && (pxX <= maxX) && (minY <= pxY) && (pxY <= maxY)) {
-                self.selCells.add(i);
+                self.selCells.push(i);
             }
 
         }
         console.timeEnd("select");
         self._selUpdate();
     };
 
-    this.hasSelected = function() {
-        return (self.selCells.size !== 0)
-    }
-
-    this.hasAllSelected = function() {
-        return (self.selCells.length === self.getCount());
-    }
-
-    this.getSelection = function() {
-        /* return selected cells as a list of ints */
-        var cellIds = [];
-        self.selCells.forEach(function(x) {
-            cellIds.push(x)
-        });
-        return cellIds;
-    };
-
-    this.selectInvert = function() {
-        /* invert selection */
-        var selCells = self.selCells;
-        var cellCount = self.getCount();
-        for (let i = 0; i < cellCount; i++) {
-            if (selCells.has(i)) {
-                selCells.delete(i);
-            } else {
-                selCells.add(i);
-            }
-        }
-        self.selCells = selCells;
-        self._selUpdate();
-    };
-
-    this.selectOnlyShow = function() {
-        /* the opposite of selectHide() = remove all coords that are not selected */
-        var selCells = self.selCells;
-        if (selCells.size === 0)
-            return;
-
-        if (self.coords.origAll === undefined)
-            self.coords.origAll = cloneArray(self.coords.orig);
-        var coords = self.coords.orig;
-        for (var i = 0; i < coords.length / 2; i++) {
-            if (!selCells.has(i)) {
-                coords[2 * i] = HIDCOORD;
-                coords[2 * i + 1] = HIDCOORD;
-            }
-        }
-        self.scaleData();
-        self.selCells.clear();
-        self._selUpdate();
-    }
-
-
-    this.selectHide = function() {
-        /* remove all coords that are selected */
-        if (self.coords.origAll === undefined)
-            self.coords.origAll = cloneArray(self.coords.orig);
-
-        var selCells = self.selCells;
-        var coords = self.coords.orig;
-
-        for (var i = 0; i < coords.length / 2; i++) {
-            if (selCells.has(i)) {
-                coords[2 * i] = HIDCOORD;
-                coords[2 * i + 1] = HIDCOORD;
-            }
-        }
-
-        self.scaleData();
-        self.selectSet([]);
-        self._selUpdate();
-    }
-
-    this.unhideAll = function() {
-        /* undo the hide operation */
-        if (self.coords.origAll !== undefined) {
-            self.coords.orig = self.coords.origAll;
-            self.coords.origAll = undefined;
-        }
-        self.scaleData();
-    }
-
-    this.getCount = function() {
-        /* return maximum number of cells in dataset, may include hidden cells, see isHidden() */
-        return self.coords.orig.length / 2;
-    };
-
-    this.getVisibleCount = function() {
-        /* return number of cells that are visible */
-        let count = 0;
-        let coords = self.coords.orig;
-        for (var i = 0; i < coords.length / 2; i++) {
-            if (!isHidden(coords[2 * i], coords[2 * i + 1]))
-                count++;
-        }
-        return count;
-    };
-
-    // END SELECTION METHODS (could be an object?)
-
     this._selUpdate = function() {
         /* called after the selection has been updated, calls the onSelChange callback */
-        setStatus(self.selCells.size + " " + self.gSampleDescription + "s selected");
+        setStatus(self.selCells.length + " " + self.gSampleDescription + "s selected");
         if (self.onSelChange !== null)
             self.onSelChange(self.selCells);
     }
 
     this.moveBy = function(xDiff, yDiff) {
         /* update the pxCoords by a certain x/y distance and redraw */
 
         // convert pixel range to data scale range
-        var zr = self.port.zoomRange;
+        var zr = self.zoomRange;
         var xDiffData = xDiff * ((zr.maxX - zr.minX) / self.canvas.width);
         var yDiffData = yDiff * ((zr.maxY - zr.minY) / self.canvas.height);
 
-        // move zoom range
+        // move zoom range 
         zr.minX = zr.minX + xDiffData;
         zr.maxX = zr.maxX + xDiffData;
         zr.minY = zr.minY + yDiffData;
         zr.maxY = zr.maxY + yDiffData;
 
         self.scaleData();
-
-        // a special case for connected plots that are not sharing our pixel coordinates
-        if (self.childPlot && self.coords !== self.childPlot.coords) {
-            self.childPlot.moveBy(xDiff, yDiff);
-        }
     };
 
     this.labelAt = function(x, y) {
-        /* return the index and the text of the label at position x,y or null if nothing there */
+        /* return the text of the label at position x,y or null if nothing there */
         //console.time("labelCheck");
-        var clusterLabels = self.coords.labels;
+        var clusterLabels = self.clusterLabels;
         if (clusterLabels === null || clusterLabels === undefined)
             return null;
-        var labelCoords = self.coords.labels;
-        var boxes = self.coords.labelBbox;
-
-        if (boxes == null) // no cluster labels
-            return null;
+        var labelCoords = self.pxLabels;
+        var boxes = self.pxLabelBbox;
 
         if (labelCoords.length !== clusterLabels.length)
             alert("internal error maxPLot.js: coordinates of labels are different from clusterLabels");
 
         for (var i = 0; i < labelCoords.length; i++) {
             var box = boxes[i];
             if (box === null) // = outside of the screen
                 continue;
+            var labelText = clusterLabels[i][2];
             var x1 = box[0];
             var y1 = box[1];
             var x2 = box[2];
             var y2 = box[3];
             if ((x >= x1) && (x <= x2) && (y >= y1) && (y <= y2)) {
                 //console.timeEnd("labelCheck");
-                var labelText = clusterLabels[i][2];
-                return [labelText, i];
+                return labelText;
             }
         }
         //console.timeEnd("labelCheck");
         return null;
-    };
-
-    this.lineAt = function(x, y) {
-        /* check if there is a line at x,y and return its label if so or null if not */
-        var pxLines = self.coords.pxLines;
-        for (var i = 0; i < pxLines.length; i++) {
-            var line = pxLines[i];
-            var x1 = line[0];
-            var y1 = line[1];
-            var x2 = line[2];
-            var y2 = line[3];
-            if (pDistance(x, y, x1, y1, x2, y2) <= 2) {
-                var lineLabel = self.coords.lineLabels[i];
-                return lineLabel;
-            }
-        }
-        return null;
-    };
+    }
 
     this.cellsAt = function(x, y) {
         /* check which cell's bounding boxes contain (x, y), return a list of the cell IDs, sorted by distance */
-        //console.time("cellSearch");
-        var pxCoords = self.coords.px;
+        console.time("cellSearch");
+        var pxCoords = self.pxCoords;
         if (pxCoords === null)
             return null;
         var possIds = [];
-        var radius = self.port.radius;
         for (var i = 0; i < pxCoords.length / 2; i++) {
             var pxX = pxCoords[2 * i];
             var pxY = pxCoords[2 * i + 1];
-            if (isHidden(pxX, pxY))
+            if (pxX === 0 && pxY === 0)
                 continue;
-            var x1 = pxX - radius;
-            var y1 = pxY - radius;
-            var x2 = pxX + radius;
-            var y2 = pxY + radius;
+            var x1 = pxX - self.radius;
+            var y1 = pxY - self.radius;
+            var x2 = pxX + self.radius;
+            var y2 = pxY + self.radius;
             if ((x >= x1) && (x <= x2) && (y >= y1) && (y <= y2)) {
                 var dist = Math.sqrt(Math.pow(x - pxX, 2) + Math.pow(y - pxY, 2));
                 possIds.push([dist, i]);
             }
         }
 
-        //console.timeEnd("cellSearch");
+        console.timeEnd("cellSearch");
         if (possIds.length === 0)
             return null;
         else {
             possIds.sort(function(a, b) {
                 return a[0] - b[0]
             }); // sort by distance
 
             // strip the distance information
             var ret = [];
-            for (let i = 0; i < possIds.length; i++) {
+            for (var i = 0; i < possIds.length; i++) {
                 ret.push(possIds[i][1]);
             }
             return ret;
         }
     };
 
+    this.getSelection = function() {
+        /* return selected cells as a list of ints */
+        return self.selCells;
+    };
+
     this.resetMarquee = function() {
         /* make the marquee disappear and reset its internal status */
-        if (!self.interact)
-            return;
-
         self.mouseDownX = null;
         self.mouseDownY = null;
         self.lastPanX = null;
         self.lastPanY = null;
         self.selectBox.style.display = "none";
         self.selectBox.style.width = 0;
         self.selectBox.style.height = 0;
     };
 
-    this.drawMarquee = function(x1, y1, x2, y2, forceAspect) {
+    this.drawMarquee = function(x1, y1, x2, y2) {
         /* draw the selection or zooming marquee using the DIVs created by setupMouse */
         var selectWidth = Math.abs(x1 - x2);
-        var selectHeight = 0;
-        if (forceAspect) {
-            var aspectRatio = self.width / self.canvas.height;
-            selectHeight = selectWidth / aspectRatio;
-        } else
-            selectHeight = Math.abs(y1 - y2);
-
+        var selectHeight = Math.abs(y1 - y2);
         var minX = Math.min(x1, x2);
         var minY = Math.min(y1, y2);
         var div = self.selectBox;
-        div.style.left = (minX - self.left) + "px";
-        div.style.top = (minY - self.top) + "px";
+        div.style.left = minX + "px";
+        div.style.top = minY + "px";
         div.style.width = selectWidth + "px";
         div.style.height = selectHeight + "px";
         div.style.display = "block";
     };
 
-    this.activatePlot = function() {
-        /* draw black border around plot, remove black border from all connected plots, call onActive */
-        if (self.parentPlot === null)
-            return false;
-
-        // only need to do something if we're not already the active plot
-        self.canvas.style["border"] = "2px solid black";
-        self.parentPlot.canvas.style["border"] = "2px solid white";
-
-        // flip the parent/child relationship
-        self.childPlot = self.parentPlot;
-        self.childPlot.parentPlot = self;
-        self.parentPlot = null;
-        self.childPlot.childPlot = null;
-
-        // hide/show the tool and zoom buttons
-        self.childPlot.zoomDiv.style.display = "none";
-        self.childPlot.toolDiv.style.display = "none";
-        self.zoomDiv.style.display = "block";
-        self.toolDiv.style.display = "block";
-
-        // notify the UI
-        self.onActiveChange(self);
-        return true;
-    }
-
-    this.isSplit = function() {
-        /* return true if this renderer has either a parent or a child plot = is in split screen mode */
-        return (isValid(self.parentPlot) || isValid(self.childPlot))
-    }
-
-    // https://stackoverflow.com/questions/73187456/canvas-determine-if-point-is-on-line
-    //function distancePointFromLine(x0, y0, x1, y1, x2, y2) {
-    //return Math.abs((x2 - x1) * (y1 - y0) - (x1 - x0) * (y2 - y1)) / Math.sqrt((x2 - x1) ** 2 + (y2 - y1) ** 2)
-    //}
-    function pDistance(x, y, x1, y1, x2, y2) {
-        /* distance of point from line segment, copied from https://stackoverflow.com/questions/849211/shortest-distance-between-a-point-and-a-line-segment */
-        var A = x - x1;
-        var B = y - y1;
-        var C = x2 - x1;
-        var D = y2 - y1;
-
-        var dot = A * C + B * D;
-        var len_sq = C * C + D * D;
-        var param = -1;
-        if (len_sq != 0) //in case of 0 length line
-            param = dot / len_sq;
-
-        var xx, yy;
-
-        if (param < 0) {
-            xx = x1;
-            yy = y1;
-        } else if (param > 1) {
-            xx = x2;
-            yy = y2;
-        } else {
-            xx = x1 + param * C;
-            yy = y1 + param * D;
-        }
-
-        var dx = x - xx;
-        var dy = y - yy;
-        return Math.sqrt(dx * dx + dy * dy);
-    }
+    //this.onHamster = function(ev, delta, deltaX, deltaY) {
+    //console.log(delta, deltaX, deltaY);
+    //console.log(ev);
+    //var pxX = ev.originalEvent.clientX - self.left;
+    //var pxY = ev.originalEvent.clientY - self.top;
+    //self.zoomBy(1+(0.01*delta), pxX, pxY);
+    //self.drawDots();
+    //ev.preventDefault();
+    //};
 
     this.onMouseMove = function(ev) {
         /* called when the mouse is moved over the Canvas */
 
         // set a timer so we can get "hover" functionality without too much CPU
-        if (self.timer !== null)
+        if (self.timer != null)
             clearTimeout(self.timer);
-        self.timer = setTimeout(self.onNoMouseMove, 130);
+        self.timer = setTimeout(self.onNoMouseMove, 170);
         // save mouse pos for onNoMouseMove timer handler
         self.lastMouseX = ev.clientX;
         self.lastMouseY = ev.clientY;
 
         // label hit check requires canvas coordinates x/y
         var clientX = ev.clientX;
         var clientY = ev.clientY;
         var canvasTop = self.top;
         var canvasLeft = self.left;
         var xCanvas = clientX - canvasLeft;
         var yCanvas = clientY - canvasTop;
 
-        // is there just white space under the mouse, do nothing,
-        // from https://stackoverflow.com/questions/15325283/how-to-detect-if-a-mouse-pointer-hits-a-line-already-drawn-on-an-html-5-canvas
-        //var imageData = self.ctx.getImageData(0, 0, self.width, self.height);
-        //var inputData = imageData.data;
-        //var pData = (~~xCanvas + (~~yCanvas * self.width)) * 4;
-
-        //if (!inputData[pData + 3]) {
-        //console.log("just white space under mouse");
-        //return;
-        //}
-
-        // when the cursor is over a label, change it to a hand, but only when there is no marquee
-        if (self.coords.labelBbox !== null && self.mouseDownX === null) {
+        // when the cursor is over a label, change it to a hand
+        if (self.pxLabelBbox !== null && self.pxLabels !== null) {
             var labelInfo = self.labelAt(xCanvas, yCanvas);
-            if (labelInfo === null) {
+            if (labelInfo === null)
                 self.canvas.style.cursor = self.canvasCursor;
-                self.onNoLabelHover(ev);
-            } else {
+            else {
                 self.canvas.style.cursor = 'pointer'; // not 'hand' anymore ! and not 'grab' yet!
                 if (self.onLabelHover !== null)
-                    self.onLabelHover(labelInfo[0], labelInfo[1], ev);
+                    self.onLabelHover(labelInfo, ev);
             }
         }
 
-        // when the cursor is over a line, trigger callback
-        if (self.onLineHover && self.coords.lineLabels) {
-            var lineLabel = self.lineAt(xCanvas, yCanvas);
-            self.onLineHover(lineLabel, ev);
-        }
-
         if (self.mouseDownX !== null) {
-            // we're panning
-            if (((ev.altKey || self.dragMode === "move")) && self.panCopy !== null) {
+            if ((ev.altKey || self.dragMode === "move") && self.panCopy !== null) {
                 var xDiff = self.mouseDownX - clientX;
                 var yDiff = self.mouseDownY - clientY;
                 self.panBy(xDiff, yDiff);
-            } else {
-                // zooming or selecting
-                var forceAspect = false;
-                var anyKey = (ev.metaKey || ev.altKey || ev.shiftKey);
-                if ((self.dragMode === "zoom" && !anyKey) || ev.metaKey)
-                    forceAspect = true;
-                self.drawMarquee(self.mouseDownX, self.mouseDownY, clientX, clientY, forceAspect);
-            }
+            } else
+                self.drawMarquee(self.mouseDownX, self.mouseDownY, clientX, clientY);
         }
     };
 
     this.onNoMouseMove = function() {
         /* called after some time has elapsed and the mouse has not been moved */
-        if (self.coords.px === null)
-            return;
         var x = self.lastMouseX - self.left; // need canvas, not screen coordinates
         var y = self.lastMouseY - self.top;
         var cellIds = self.cellsAt(x, y);
         // only call onNoCellHover if callback exists and there is nothing selected
         if (cellIds === null && self.onNoCellHover !== null && self.selCells === null)
             self.onNoCellHover();
         else if (self.onCellHover !== null)
             self.onCellHover(cellIds);
     };
 
-
     this.onMouseDown = function(ev) {
         /* user clicks onto canvas */
-        if (self.activatePlot())
-            return; // ignore the first click into the plot, if it was the activating click
-        debug("background mouse down");
+        console.log("background mouse down");
         var clientX = ev.clientX;
         var clientY = ev.clientY;
-        if ((ev.altKey || self.dragMode === "move") && !ev.shiftKey && !ev.metaKey) {
-            debug("alt key or move mode: starting panning");
+        if (ev.altKey || self.dragMode === "move") {
+            console.log("alt key or move mode: starting panning");
             self.panStart();
         }
         self.mouseDownX = clientX;
         self.mouseDownY = clientY;
     };
 
     this.onMouseUp = function(ev) {
-        debug("background mouse up");
+        console.log("background mouse up");
         // these are screen coordinates
         var clientX = ev.clientX;
         var clientY = ev.clientY;
         var mouseDidNotMove = (self.mouseDownX === clientX && self.mouseDownY === clientY);
 
         if (self.panCopy !== null && !mouseDidNotMove) {
-            debug("ending panning operation");
+            console.log("ending panning operation");
             self.panEnd();
             self.mouseDownX = null;
             self.mouseDownY = null;
             self.drawDots();
             return;
-        } else {
-            // abort panning
-            self.panCopy = null;
         }
 
         if (self.mouseDownX === null && self.lastPanX === null) {
             // user started the click outside of the canvas: do nothing
-            debug("first click must have been outside of canvas");
+            console.log("first click must have been outside of canvas");
             return;
         }
 
         // the subsequent operations require canvas coordinates x/y
         var canvasTop = self.top;
         var canvasLeft = self.left;
         var x1 = self.mouseDownX - canvasLeft;
         var y1 = self.mouseDownY - canvasTop;
         var x2 = clientX - canvasLeft;
         var y2 = clientY - canvasTop;
 
         // user did not move the mouse, so this is a click
         if (mouseDidNotMove) {
-            // recognize a double click -> zoom
-            if (self.lastClick !== undefined && x2 === self.lastClick[0] && y2 === self.lastClick[1]) {
-                self.zoomBy(1.33);
-                self.lastClick = [-1, -1];
-            } else {
-                self.lastClick = [x2, y2];
-            }
-
-            var labelInfo = self.labelAt(x2, y2);
-            if (labelInfo !== null && self.doDrawLabels)
-                self.onLabelClick(labelInfo[0], labelInfo[1], ev);
+            var clickedLabel = self.labelAt(x2, y2);
+            if (clickedLabel !== null)
+                self.onLabelClick(clickedLabel, ev);
             else {
                 var clickedCellIds = self.cellsAt(x2, y2);
-                // click on a cell -> update selection and redraw
                 if (clickedCellIds !== null && self.onCellClick !== null) {
-                    self.selectClear(true);
-                    for (var i = 0; i < clickedCellIds.length; i++) {
-                        self.selCells.add(clickedCellIds[i]);
-                    }
-                    self.drawDots();
+                    self.selCells = clickedCellIds;
                     self.onCellClick(clickedCellIds, ev);
-
+                    self.drawDots();
                 } else {
                     // user clicked onto background:
                     // reset selection and redraw
-                    debug("not moved at all: reset " + clientX + " " + self.mouseDownX + " " + self.mouseDownY + " " + clientY);
+                    console.log("not moved at all: reset " + clientX + " " + self.mouseDownX + " " + self.mouseDownY + " " + clientY);
                     self.selectClear();
-
                     self.drawDots();
                 }
 
                 self.lastPanX = null;
                 self.lastPanY = null;
             }
             self.mouseDownX = null;
             self.mouseDownY = null;
             return;
         }
-        //debug("moved: reset "+x+" "+mouseDownX+" "+mouseDownY+" "+y);
+        //console.log("moved: reset "+x+" "+mouseDownX+" "+mouseDownY+" "+y);
 
         // it wasn't a click, so it was a drag
         var anyKey = (ev.metaKey || ev.altKey || ev.shiftKey);
 
         // zooming
-        if ((self.dragMode === "zoom" && !anyKey) || ev.metaKey) {
-            // get current coords of the marquee in canvas pixels
-            var div = self.selectBox;
-            let zoomX1 = parseInt(div.style.left.replace("px", ""));
-            let zoomY1 = parseInt(div.style.top.replace("px", ""));
-            let zoomX2 = zoomX1 + parseInt(div.style.width.replace("px", ""));
-            let zoomY2 = zoomY1 + parseInt(div.style.height.replace("px", ""));
-            zoomY1 = self.canvas.height - zoomY1;
-            zoomY2 = self.canvas.height - zoomY2;
-            self.zoomTo(zoomX1, zoomY1, zoomX2, zoomY2);
-            // switch back to the mode before zoom was clicked
-            if (self.prevMode) {
-                self.activateMode(self.prevMode);
-                self.prevMode = null;
-            }
-
-
-        }
-        // marquee select
+        if ((self.dragMode === "zoom" && !anyKey) || ev.metaKey)
+            self.zoomTo(x1, y1, x2, y2);
+        // marquee select 
         else if ((self.dragMode === "select" && !anyKey) || ev.shiftKey) {
             if (!ev.shiftKey)
-                self.selectClear(true);
+                self.selectClear();
             self.selectInRect(x1, y1, x2, y2);
         } else {
-            debug("Internal error: no mode?");
+            console.log("Internal error: no mode?");
         }
 
         self.resetMarquee();
 
         self.drawDots();
     };
 
-    function drawCirclesSvg(svgLines, pxCoords, coordColors, colors, radius, alpha, selCells) {
-        /* add SVG text to the array svgLines */
-        debug("Drawing " + coordColors.length + " circles with SVG renderer");
-        var count = 0;
-        for (var i = 0; i < pxCoords.length / 2; i++) {
-            var pxX = pxCoords[2 * i];
-            var pxY = pxCoords[2 * i + 1];
-            if (isHidden(pxX, pxY))
-                continue;
-            var col = colors[coordColors[i]];
-
-            svgLines.push("<circle cx='" + pxX + "' cy='" + pxY + "' r='" + radius + "' fill-opacity='" + alpha + "' fill='#" + col + "' />");
-            count++;
-        }
-        return count;
-    }
-
     this.onWheel = function(ev) {
         /* called when the user moves the mouse wheel */
-        if (self.parentPlot !== null)
-            return;
-        debug(ev);
+        console.log(ev);
         var normWheel = normalizeWheel(ev);
-        debug(normWheel);
+        console.log(normWheel);
         var pxX = ev.clientX - self.left;
         var pxY = ev.clientY - self.top;
         var spinFact = 0.1;
-        if (ev.ctrlKey) // = OSX pinch and zoom gesture (and no other OS/mouse combination?)
-            spinFact = 0.08; // is too fast, so slow it down a little
+        if (ev.ctrlKey) // = OSX pinch and zoom gesture
+            spinFact = 0.02; // is too fast, so slow it down a little
         var zoomFact = 1 - (spinFact * normWheel.spinY);
-        debug("Wheel Zoom by " + zoomFact);
+        console.log("Wheel Zoom by " + zoomFact);
         self.zoomBy(zoomFact, pxX, pxY);
         self.drawDots();
         ev.preventDefault();
         ev.stopPropagation();
     };
 
     this.setupMouse = function() {
@@ -2787,236 +1653,64 @@
         self.canvas.addEventListener("wheel", self.onWheel);
     };
 
     this.setShowLabels = function(doShow) {
         self.doDrawLabels = doShow;
     };
 
-    this.getLabels = function() {
-        /* get current labels */
-        var ret = [];
-        var labels = self.coords.labels;
-        for (var i = 0; i < labels.length; i++)
-            ret.push(labels[i][2]);
-        return ret;
-    }
-
-    this.setLabels = function(newLabels) {
-        /* set new label text */
-        if (newLabels.length !== self.coords.labels.length) {
-            debug("maxPlot:setLabels error: new labels have wrong length.");
-            return;
-        }
-
-        for (var i = 0; i < newLabels.length; i++)
-            self.coords.labels[i][2] = newLabels[i];
-
-        self.coords.pxLabels = scaleLabels(self.coords.labels, self.port.zoomRange, self.port.radius,
-            self.canvas.width, self.canvas.height);
-
-        // a special case for connected plots that are not sharing our pixel coordinates
-        if (self.childPlot && self.coords !== self.childPlot.coords) {
-            self.childPlot.setLabels(newLabels);
-        }
-    };
-
-    this._setLines = function(lines, attrs) {
-        /* set the line attributes */
-        if (lines === undefined)
-            return;
-        self.coords.lines = lines;
-
-        if (!attrs)
-            self.coords.lineAttrs = {};
-        else
-            self.coords.lineAttrs = attrs;
-
-        // save the labels elsewhere. Labels are optional.
-        if (lines[0].length > 4) {
-            var lineLabels = []
-            for (var i = 0; i < lines.length; i++) {
-                lineLabels.push(lines[i][4]);
-            }
-            self.coords.lineLabels = lineLabels;
-        }
-    }
-
     this.activateMode = function(modeName) {
         /* switch to one of the mouse drag modes: zoom, select or move */
-        if (modeName === "zoom")
-            self.prevMode = self.dragMode;
-        else
-            self.prevMode = null;
-
         self.dragMode = modeName;
 
         var cursor = null;
 
         if (modeName === "move")
             cursor = 'all-scroll';
         else if (modeName === "zoom")
-            cursor = "zoom-in"
-        else if (modeName == "select")
             cursor = 'crosshair';
-        //else
-        //cursor= 'default';
+        else
+            cursor = 'default';
 
         self.canvas.style.cursor = cursor;
         self.canvasCursor = cursor;
 
         self.resetMarquee();
 
-        if (self.interact) {
-            self.icons["move"].style.backgroundColor = gButtonBackground;
-            self.icons["zoom"].style.backgroundColor = gButtonBackground;
-            self.icons["select"].style.backgroundColor = gButtonBackground;
-            self.icons[modeName].style.backgroundColor = gButtonBackgroundClicked;
-        }
-        if (self.childPlot)
-            self.childPlot.activateMode(modeName);
+        self.icons["move"].style.backgroundColor = gButtonBackground;
+        self.icons["zoom"].style.backgroundColor = gButtonBackground;
+        self.icons["select"].style.backgroundColor = gButtonBackground;
+        self.icons[modeName].style.backgroundColor = gButtonBackgroundClicked;
+
+        //var upModeName = modeName[0].toUpperCase() + modeName.slice(1);
+        //var buttonId = "mpIconMode"+upModeName;
     }
 
     this.randomDots = function(n, radius, mode) {
         /* draw x random dots with x random colors*/
-        function randomArray(ArrType, length, max) {
+        function randomArray(arrType, length, max) {
             /* make Array and fill it with random numbers up to max */
-            var arr = new ArrType(length);
+            var arr = new arrType(length);
             for (var i = 0; i < length; i++) {
                 arr[i] = Math.round(Math.random() * max);
             }
             return arr;
         }
 
         if (mode !== undefined)
             self.mode = mode;
-        self.port.radius = radius;
+        self.radius = radius;
         self.setCoords(randomArray(Uint16Array, 2 * n, 65535));
         self.setColors(["FF0000", "00FF00", "0000FF", "CC00CC", "008800"]);
         self.setColorArr(randomArray(Uint8Array, n, 4));
 
         console.time("draw");
         self.drawDots();
         console.timeEnd("draw");
         return self;
-    };
-
-    this.split = function() {
-        /* reduce width of renderer, create new renderer and place both side-by-side.
-         * They initially share the .coords but setCoords() can break that relationship.
-         * */
-        var canvHeight = self.canvas.height;
-        var canvLeft = self.left;
-        var newWidth = self.width / 2;
-        var newTop = self.top;
-        var newLeft = self.left + newWidth;
-        var newHeight = canvHeight + gStatusHeight;
-
-        var newDiv = document.createElement('div');
-        newDiv.id = "mpPlot2";
-        document.body.appendChild(newDiv);
-
-        var opts = cloneObj(self.globalOpts);
-        opts.showClose = true;
-
-        var plot2 = new MaxPlot(newDiv, newTop, newLeft, newWidth, newHeight, {
-            "showClose": true,
-            "showSliders": false
-        });
-
-        plot2.statusLine.style.display = "none";
-
-        plot2.port = self.port;
-        plot2.selCells = self.selCells;
 
-        plot2.coords = self.coords;
-
-        plot2.col = {};
-        plot2.col.pal = self.col.pal;
-        plot2.col.arr = self.col.arr;
-
-        if (self.background)
-            plot2.setBackground(self.background.img);
-
-        self.setSize(newWidth, newHeight, false); // will call scaleData(), but not redraw.
-
-        plot2.onLabelClick = self.onLabelClick;
-        plot2.onCellClick = self.onCellClick;
-        plot2.onCellHover = self.onCellHover;
-        plot2.onNoCellHover = self.onNoCellHover;
-        plot2.onSelChange = self.onSelChange;
-        plot2.onLabelHover = self.onLabelHover;
-        plot2.onNoLabelHover = self.onNoLabelHover;
-        plot2.onActiveChange = self.onActiveChange;
-
-        plot2.drawDots();
-
-        self.childPlot = plot2;
-        plot2.parentPlot = self;
-
-        // add a thick border and hide the menus in the child
-        self.canvas.style["border"] = "2px solid black";
-        self.childPlot.zoomDiv.style.display = "none";
-        self.childPlot.toolDiv.style.display = "none";
-
-        return plot2;
     };
 
-    this.unsplit = function() {
-        /* remove the connected non-active renderer */
-        //var canvWidth = window.innerWidth - canvLeft - legendBarWidth;
-        var otherRend = self.childPlot;
-        self.childPlot = undefined;
-        if (!otherRend) {
-            otherRend = self.parentPlot;
-            self.parentPlot = undefined;
-        }
-        self.setSize(self.width * 2, self.height, false);
-
-        otherRend.div.remove();
-        self.canvas.style["border"] = "none";
-        return;
-    }
-
-    this.getWidth = function() {
-        /* return total size of renderer, including any split child renderers */
-        if (self.childPlot)
-            return self.width + self.childPlot.width;
-        else
-            return self.width;
-    }
-
-    this.calcMedian = function(coords, values, names, numNames) {
-        /* given an array of coordinates (x at even positions, y at odd positions) and an array of names for each of them
-         * return the median for each name as an object name -> array of [x, y, count]
-         * if names is undefined, will use numNames and convert to two decimals 
-         * */
-        var calc = {};
-        for (var i = 0, I = values.length; i < I; i++) {
-            var label = null;
-            if (names) {
-                label = names[values[i]];
-            } else {
-                label = numNames[i].toFixed(2);
-            }
-            if (calc[label] === undefined) {
-                calc[label] = [
-                    [],
-                    [], 0
-                ]; // all X, all Y, count
-            }
-            var x = coords[i * 2];
-            var y = coords[i * 2 + 1];
-
-            if (isHidden(x, y))
-                continue;
-
-            calc[label][0].push(x);
-            calc[label][1].push(y);
-            calc[label][2] += 1;
-        }
-        return calc;
-    }
-
     // object constructor code
-    self.initCanvas(div, top, left, width, height, args);
+    self.initCanvas(div, top, left, width, height);
     self.initPlot(args);
+
 }
```

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/zoom.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/zoom.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/README.txt` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/README.txt`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-scale-16.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-scale-16.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-info-24.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-info-24.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-merge-down-16.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-merge-down-16.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-info-16.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-info-16.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/gtk-save.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/gtk-save.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-move-22.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/move.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-zoom-16.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-zoom-16.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-free-select-16.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-free-select-16.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-controller-16.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-controller-16.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-controller-24.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-controller-24.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-center-16.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-center-16.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-move-16.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-move-16.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-center-24.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/center.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-zoom-22.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-zoom-22.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-free-select-22.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/lasso.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-edit-16.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-edit-16.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/move.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-move-22.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/lasso.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-free-select-22.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/cbWeb/img/center.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-center-24.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser/download.py` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/convert.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,480 +1,457 @@
-# download data from single cell repos
+# various format converters for single cell data:
+# - cellranger, mtx to tsv, matConcat, etc
 
-import logging, optparse, io, sys, os, shutil, operator
-from collections import defaultdict, OrderedDict, Counter
+import logging, optparse, io, sys, os, shutil, operator, glob, re
+from collections import defaultdict
 
 from .cellbrowser import runGzip, openFile, errAbort, setDebug, moveOrGzip, makeDir, iterItems
-from .cellbrowser import mtxToTsvGz, writeCellbrowserConf, parseIntoColumns, readMatrixAnndata, splitOnce
-from .cellbrowser import generateHtmls, writePyConf
+from .cellbrowser import mtxToTsvGz, writeCellbrowserConf, getAllFields, readMatrixAnndata
+from .cellbrowser import anndataToTsv, loadConfig, sanitizeName, lineFileNextRow, scanpyToCellbrowser, build
 
 from os.path import join, basename, dirname, isfile, isdir, relpath, abspath, getsize, getmtime, expanduser
 
-def cbGet_parseArgs(showHelp=False):
+def cbToolCli_parseArgs(showHelp=False):
     " setup logging, parse command line arguments and options. -h shows auto-generated help page "
-    parser = optparse.OptionParser("""usage: %prog [options] <repo> <accession> - import single cell data from repositories
+    parser = optparse.OptionParser("""usage: %prog [options] mtx2tsv|matCat|metaCat - convert various single-cell related files
 
-    The only valid repo right now is: ebi
+    mtx2tsv   - convert matrix market to .tsv.gz
+    matCat - merge expression matrices with one line per gene into a big matrix.
+        Matrices must have identical genes in the same order and the same number of
+        lines. Handles .csv files, otherwise defaults to tab-sep input. gzip OK.
+    metaCat - concat meta tables
 
     Examples:
-    - %prog ebi -a E-GEOD-100058 -o myEbiDataset - import E-GEOD-10058 to myEbiDataset/
-    - %prog ebi -i E-GEOD-100058-mirror/ -o myEbiDataset - convert E-GEOD-10058 FTP mirror to myEbiDataset/
+    - %prog mtx2tsv matrix.mtx genes.tsv barcodes.tsv exprMatrix.tsv.gz - convert .mtx to .tsv.gz file
+    - %prog matCat mat1.tsv.gz mat2.tsv.gz exprMatrix.tsv.gz - concatenate expression matrices
+    - %prog metaCat meta.tsv seurat/meta.tsv scanpy/meta.tsv newMeta.tsv - merge meta matrices
     """)
 
     parser.add_option("-d", "--debug", dest="debug", action="store_true",
         help="show debug messages")
-    parser.add_option("-a", "--accession", dest="acc", action="store",
-        help="Accession in source database")
-    parser.add_option("-i", "--inDir", dest="inDir", action="store",
-        help="Input directory")
-    parser.add_option("-o", "--outDir", dest="outDir", action="store",
-        help="Output directory")
+    parser.add_option("", "--fixDots", dest="fixDots", action="store_true",
+        help="try to fix R's mangling of various special chars to '.' in the cell IDs")
+
 
     (options, args) = parser.parse_args()
 
     if showHelp:
         parser.print_help()
         exit(1)
 
     setDebug(options.debug)
     return args, options
 
-def mirrorFtp(hostName, ftpDir, localDir):
-    " mirror an ftp directory to local disk "
-    makeDir(localDir)
-    from ftplib import FTP
-    logging.info("FTP: connecting to %s, dir %s" % (hostName, ftpDir))
-    ftp = FTP(hostName)
-    ftp.login()
-    ftp.cwd(ftpDir)
-
-    ls = ftp.nlst()
-    count = len(ls)
-    curr = 0
-    logging.info("Found {} files".format(count))
-    for fn in ls:
-        if fn=="complete":
-            continue
-        curr += 1
-        logging.info('Downloading file {} ... {} of {} ...'.format(fn, curr, count))
-        outPath = join(localDir, fn)
-        ftp.retrbinary('RETR ' + fn, open(outPath, 'wb').write)
-
-    ftp.quit()
-
-    complFn = join(localDir, "complete")
-    open(complFn, "w").close() # = create 0-size file
-    logging.info("FTP download complete.")
-
-#def downloadFromEbi(acc, outDir):
-    #" download files to outDir/orig and then create cell browser files in outDir/ "
-    #for fExt in [".clusters.tsv"]:
-        #fname = acc+fExt
-        #fileUrl = baseUrl+"/"+fname
-        #localPath = join(outDir, fname)
-
-def parseClusters(fname):
-    """ find the optimal K number in the clusters file and the cluster assignment
-    return a the value of K and a dictionary with sampleName -> clusterNumber
-    """
-    logging.info("Parsing %s" % fname)
-    bestK = None
-    for line in open(fname):
-        row = line.rstrip("\n\r").split("\t")
-        if row[0]=="sel.K":
-            sampleNames = row[2:]
-            continue
-        selK = row[0]
-        lastRow = row
-        if selK=="TRUE":
-            bestK = row[1]
-            clusters = row[2:]
-            break
-
-    if bestK is None:
-        logging.warn("No best K found, using last K")
-        bestK = lastRow[1]
-        clusters = lastK[2:]
-
-    return bestK, dict(zip(sampleNames, clusters))
-
-def parseCondSdrf(cellIds, fname):
-    """ parse the condensed sdrf into cellId -> dict of key-val """
-    cellIds = set(cellIds)
-    cellMeta = defaultdict(dict)
-    for line in open(fname):
-        #E-MTAB-7303             ERR2847884      characteristic  organism        Homo sapiens    http://purl.obolibrary.org/obo/NCBITaxon_9606
-        #E-MTAB-4850		SAMEA50486668	characteristic	age	42 year
-        row = line.rstrip("\n\r").split("\t")
-        dsId, _, cellId, _, fieldName, val = row[:6]
-        if cellId not in cellIds:
-            continue
-        cellMeta[cellId][fieldName] = val
-    return cellMeta
+def cbToolCli():
+    " run various tools from the command line "
+    args, options = cbToolCli_parseArgs()
 
-def parseSdrfFieldNames(sdrfFname):
-    " return list of field names in sdrf file "
-    ifh = open(sdrfFname)
-
-    #Source Name	Comment[ENA_SAMPLE]	Comment[BioSD_SAMPLE]	Characteristics[organism]	Characteristics[disease]	Characteristics[disease staging]	Characteristics[age]	Unit[time unit]	Characteristics[sex]	Characteristics[organism part]	Characteristics[cell type]	Characteristics[cell line]	Characteristics[single cell well quality]	Comment[single cell quality]	Material Type	Protocol REF	Protocol REF	Extract Name	Comment[LIBRARY_LAYOUT]	Comment[LIBRARY_SELECTION]	Comment[LIBRARY_SOURCE]	Comment[LIBRARY_STRAND]	Comment[LIBRARY_STRATEGY]	Comment[NOMINAL_LENGTH]	Comment[NOMINAL_SDEV]	Comment[ORIENTATION]	Comment[single cell isolation]	Comment[library construction]	Comment[input molecule]	Comment[primer]	Comment[end bias]	Protocol REF	Performer	Assay Name	Comment[technical replicate group]	Technology Type	Comment[ENA_EXPERIMENT]	Scan Name	Comment[SUBMITTED_FILE_NAME]	Comment[ENA_RUN]	Comment[FASTQ_URI]	Comment[SPOT_LENGTH]	Comment[READ_INDEX_1_BASE_COORD]	Factor value[cell line]	Factor Value[stimulus]	Factor Value[single cell identifier]
-
-    fieldNames = ifh.readline().strip("\n\r").split("\t")
-
-    newNames = []
-    for fieldName in fieldNames:
-        if "[" in fieldName:
-            fieldName = fieldName.split("[")[1].rstrip("]")
-        newNames.append(fieldName)
-    return newNames
-
-#def parseSdrf(srdfFname):
-    #""" parse EBI srdf file to list of fieldNames. Remove fields with only a single value.
-    #return a dict with the fields and values where all lines contain the same value.
-    #Also remove filename and URI fields.
-    #"""
-    #logging.debug("Parsing %s" % srdfFname)
-    #columns = parseIntoColumns(srdfFname)
-    ##cleanList = []
-    #fieldList = []
-    #genInfo = {}
-    #for fieldName, values in columns:
-        #if "[" in fieldName:
-            #fieldName = fieldName.split("[")[1].rstrip("]")
-
-        #valSet = set(values)
-
-        #logging.debug(fieldName)
-        #logging.debug(valSet)
-        #if len(valSet)==1:
-            #logging.debug("Field has only a single value, adding to info dict: %s=%s" % (fieldName, values[0]))
-            #genInfo[fieldName] = values[0]
-        #else:
-            #cleanList.append( (fieldName, values) )
-            #fieldList.append(fieldName)
-
-    #return fieldList, genInfo
-
-def parseIdf(fname):
-    " parse idf and return as dict key = value "
-    logging.debug("Parsing %s" % fname)
-    data = OrderedDict()
-    for line in open(fname, "Ut"):
-        if line.startswith("\n"):
-            continue
-        line = line.rstrip("\n")
-        key, val = splitOnce(line, "\t")
-        data[key] = val
-    return data
-
-def toStr(s):
-    " prettify raw IDF tab-sep list to a normal string "
-    return s.strip("\t").replace("\t", ", ")
-
-def translateIdf(idf):
-    " convert dict read from IDF to a simple key-value format for the cell browser desc.conf "
-    desc = OrderedDict()
-    desc["title"] = toStr(idf["Investigation Title"])
-    desc["abstract"] = toStr(idf["Experiment Description"])
-    desc["design"] = toStr(idf["Experimental Design"])
-    desc["expType"] = toStr(idf["Comment[EAExperimentType]"])
-    desc["methods"] = toStr(idf["Protocol Description"])
-    desc["curator"] = toStr(idf["Comment[EACurator]"])+", EBI Single Cell Expression Atlas"
-    desc["submitter"] = toStr(idf["Person First Name"])+" "+toStr(idf["Person Last Name"])+" <"+toStr(idf["Person Email"])+">"
-    desc["submission_date"] = toStr(idf["Public Release Date"])
-    if "PubMed ID" in idf:
-        desc["pmid"] = toStr(idf["PubMed ID"])
-    if "Publication DOI" in idf:
-        desc["doi"] = toStr(idf["Publication DOI"])
-
-    if "Comment[ArrayExpressAccession]" in idf:
-        desc["arrayexpress"] = toStr(idf["Comment[ArrayExpressAccession]"])
-
-    if "Comment [SecondaryAccession]" in idf:
-        desc["ena_project"] = toStr(idf["Comment [SecondaryAccession]"])
-
-    return desc
-
-def convertCoords(coordFname, newCoordFname):
-    " simply reorder columns"
-    ofh = open(newCoordFname, "w")
-    for line in open(coordFname):
-        row = line.rstrip("\n\r").split("\t")
-        newRow = (row[2], row[0], row[1])
-        ofh.write("\t".join(newRow))
-        ofh.write("\n")
-    ofh.close()
-    logging.info("Wrote %s" % newCoordFname)
+    if len(args)<=1:
+        cbToolCli_parseArgs(showHelp=True)
+        sys.exit(1)
 
-def convertMarkers(inFname, outFname):
-    " reorder columns and reheader and return list of one top marker per cluster "
-    #names	groups	scores	logfc	pvals	pvals_adj
-    #ENSG00000112096	0	9.120421	1.4149776	3.5174541399729827e-15	5.52275474517158e-11
-    ofh = open(outFname, "w")
-    clusterToMarkers = defaultdict(list)
-    for line in open(inFname):
-        row = line.rstrip("\n\r").split("\t")
-        #cluster, pval, auroc, gene = row
-        geneId, cluster, score, logfc, pval, pvalAdj = row
-        if row[0]=="names":
-            newRow = ["Cluster", "Gene", "p-Value Adj.", "p-Value", "logFC", "score"]
-        else:
-            newRow = (row[1], row[0], row[5], row[4], row[3], row[2])
-            clusterToMarkers[cluster].append( (float(pvalAdj), geneId) )
+    cmd = args[0]
 
-        ofh.write("\t".join(newRow))
-        ofh.write("\n")
+    cmds = ["mtx2tsv", "matCat", "metaCat"]
 
-    ofh.close()
-    logging.info("Wrote %s" % outFname)
+    if cmd=="mtx2tsv":
+        mtxFname = args[1]
+        geneFname = args[2]
+        barcodeFname = args[3]
+        outFname = args[4]
+        mtxToTsvGz(mtxFname, geneFname, barcodeFname, outFname)
+    elif cmd=="matCat":
+        inFnames = args[1:-1]
+        outFname = args[-1]
+        matCat(inFnames, outFname)
+    elif cmd=="metaCat":
+        inFnames = args[1:-1]
+        outFname = args[-1]
+        metaCat(inFnames, outFname, options)
+    else:
+        errAbort("Command %s is not a valid command. Valid commands are: %s" % (cmd, ", ".join(cmds)))
 
-    topMarkers = {}
-    for cluster, pValGenes in iterItems(clusterToMarkers):
-        pValGenes.sort()
-        topGene = pValGenes[0][1]
-        topMarkers[cluster] = topGene
-
-    return topMarkers
-
-def writeQuickGenes(topGenes, outFname):
-    " given cluster -> gene, create a quickGenes file "
-    ofh = open(outFname, "w")
-    for cluster, gene in iterItems(topGenes):
-        ofh.write("%s\tCluster %s\n"% (gene, cluster))
-    ofh.close()
-    logging.info("Wrote %s" % outFname)
+def matCat(inFnames, outFname):
+    tmpFname = outFname+".tmp"
+    ofh = openFile(tmpFname, "w")
 
-def makeBasicCbConf(name, shortLabel, hasInferred, matrixFname="exprMatrix.tsv.gz"):
-    " just fill a basic conf dict and return it "
-    c = OrderedDict()
-    c["name"] = name
-    c["shortLabel"] = shortLabel
-    c["exprMatrix"] = matrixFname
-    c["meta"] = "meta.tsv"
-    c["#priority"] = "10"
-    c["tags"] = ["ebi"]
-    c["enumFields"] = "cluster"
-
-    if hasInferred:
-        clusterField = "inferred cell type"
-        c["acroFname"] = "acronyms.tsv"
-    else:
-        clusterField = "cluster"
+    ifhs = []
+
+    sep = "\t"
+    if ".csv" in inFnames[0]:
+        sep = ","
+
+    for fn in inFnames:
+        ifhs.append( openFile(fn) )
+
+    headers, colCounts = getAllFields(ifhs, sep)
+    ofh.write("\t".join(headers))
+    ofh.write("\n")
+
+    for i, ifh in enumerate(ifhs):
+        logging.info("File %s: %d columns with values" % (ifhs[i].name, colCounts[i]-1)) 
 
-    c["clusterField"] = clusterField
-    c["labelField"] = clusterField
+    fileCount = len(inFnames)
+    progressStep = 1000
 
-    c["#unit"] = "TPM"
-    c["coords"] = [{"file":"tsne_perp25.coords.tsv", "shortLabel" : "t-SNE Perp=25"}]
-    c["markers"] = [{"file":"markers.tsv", "shortLabel":"Cluster-specific genes"}]
-    c["quickGenesFile"] = "quickGenes.tsv"
-    return c
-
-def writeMeta(clusters, cellIds, sdrfFields, boringFields, cellMeta, metaFname):
-    " write a meta.tsv file, add in the clusters "
-    #idIdx = None
-    #fieldNames = []
-    #for fieldIdx, (fieldName, vals) in enumerate(metaColumns):
-        #if fieldName=="ENA_RUN":
-            #idIdx = fieldIdx
-            #break
-        #fieldNames.append(fieldName)
-
-    #if idIdx is None:
-        #errAbort("Couldn't find the main ID field in the sdrf file. Possible field names: %s" % ",".join(fieldNames))
-
-    # basic check of the ID field
-    #idName = metaColumns[idIdx][0]
-    #idList = metaColumns[idIdx][1]
-    #if len(idList)!=len(set(idList)):
-        #idCounts = Counter(idList)
-        #errAbort("field %s was identified as the ID field, but it is not unique" % idCounts)
-
-    # put the id field first
-    #newOrder = []
-    #newOrder.append(metaColumns[idIdx])
-    #for i in range(0, idList):
-        #if i==idIdx or i==0: # remove the first source name field
-            #continue
-        #newOrder.append(metaColumns[i])
-
-    # add the cluster field
-    #clustVals = []
-    #for cellId in newOrder[0][1]:
-        #clustId = clusters[cellId]
-        #clustVals.append(clustId)
-
-    #newOrder.insert(1, ("Cluster", clustVals))
-
-    #headers = [f[0] for f in newOrder]
-
-    #fieldValues = [x[1] for x in newOrder]
-    #for i in range(0, len(idList)):
-        #row = []
-        #for field in fieldValues:
-            #row.append(field[i])
-        #ofh.write("\t".join(row))
-        #ofh.write("\n")
-    #ofh.close()
-    #logging.info("Wrote %s" % newCoordFname)
-
-    logging.debug("Fields in the SDRF: %s" % sdrfFields)
-    logging.debug("Boring fields: %s" % boringFields.keys())
-
-    allFields = set()
-    for cellId in cellIds:
-        meta = cellMeta[cellId]
-        allFields.update(meta.keys())
-    logging.debug("All fields from the condensed: %s" % allFields)
-
-    fieldOrder = []
-    doneFields = set()
-    for fn in sdrfFields:
-        if fn not in boringFields and fn in allFields and fn not in doneFields:
-            fieldOrder.append(fn)
-            doneFields.add(fn)
-
-    logging.debug("final field order: %s" % fieldOrder)
-    assert(len(set(fieldOrder))==len(fieldOrder)) # fields must not appear twice
-
-    ofh = open(metaFname, "w")
-    ofh.write("cell ID\tcluster\t")
-    ofh.write("\t".join(fieldOrder))
+    doProcess = True
+    lineCount = 0
+
+    while doProcess:
+        geneId = None
+
+        lineCount += 1
+        if lineCount % progressStep == 0:
+            logging.info("Processed %d rows" % (lineCount))
+
+        for i, ifh in enumerate(ifhs):
+            lineStr = ifh.readline()
+            # check if we're at EOF
+            if lineStr=='':
+                doProcess = False
+                break
+
+            fields = lineStr.rstrip('\r\n').split(sep)
+            fields = [x.strip('"') for x in fields]
+            if (len(fields)!=colCounts[i]): # check number of columns against header count
+                raise Exception("Illegal number of fields: file %s, line %d, field count: %d, expected %d" % 
+                    (ifh.name, lineCount, len(fields), colCounts[i]))
+
+            # check the gene ID
+            if i==0: # get the gene ID from the first file
+                geneId = fields[0]
+                allVals = [geneId]
+            else:
+                #assert(geneId == fields[0]) # if this fails, then the rows are not in the same order
+                if geneId != fields[0]:
+                    print("Error: File %s has gene IDs that is out of order." % ifh.name)
+                    print("Expected geneID: %s, got geneID: %s" % (geneId, fields[0]))
+                    sys.exit(1)
+
+            allVals.extend(fields[1:])
+
+        ofh.write("\t".join(allVals))
+        ofh.write("\n")
+
+    # make sure that we've read through all files
+    for ifh in ifhs:
+        assert(ifh.readline()=='') # a file has still lines left to read?
+
+    ofh.close()
+    moveOrGzip(tmpFname, outFname)
+    logging.info("Wrote %d lines (not counting header)" % lineCount)
+
+def metaCat(inFnames, outFname, options):
+    " merge all tsv/csv columns in inFnames into a new file, outFname. Column 1 is ID to join on. "
+    allHeaders = ["cellId"]
+    allRows = defaultdict(dict) # cellId -> fileIdx -> list of non-ID fields
+    fieldCounts = {} # fileIdx -> number of non-ID fields
+    allIds = set() # set with all cellIds
+
+    for fileIdx, fname in enumerate(inFnames):
+        headers = None
+        for row in lineFileNextRow(fname):
+            if headers is None:
+                headers = row._fields[1:]
+                logging.info("Reading %s, %d columns:  %s" % (fname, len(headers), repr(headers)))
+                allHeaders.extend(headers)
+                fieldCounts[fileIdx] = len(headers)
+
+            cellId = row[0]
+            allIds.add(cellId)
+            allRows[cellId][fileIdx] = row[1:]
+
+    nonCharRe = re.compile(r'[^a-zA-Z0-9]')
+
+    if options.fixDots:
+        # first create a map realId -> rId
+        rToReal = {}
+        for cellId, rowData in iterItems(allRows):
+            rId = nonCharRe.sub(".", cellId)
+            if rId!=cellId and rId in allRows:
+                assert(rId not in rToReal) # Uh-oh! Mapping R <-> realId is not simple. May need some manual work.
+                rToReal[rId]=cellId
+        logging.info("Found %d cell IDs that look like they've been mangled by R" % (len(rToReal)))
+
+        # now merge the R-id entries into the real ID entries
+        newRows = {}
+        for rId, readlId in iterItems(rToReal):
+            allRows[cellId].update(allRows[rId])
+        for rId in rToReal.keys():
+            del allRows[rId]
+        logging.info("Merged back rIds into normal data")
+
+    tmpFname = outFname+".tmp"
+    ofh = openFile(tmpFname, "w")
+    ofh.write("\t".join(allHeaders))
     ofh.write("\n")
 
-    for cellId, meta in iterItems(cellMeta):
-        row = [cellId]
-        clustId = clusters.get(cellId, "Unknown")
-        row.append(clustId)
-        for fieldName in fieldOrder:
-            val = meta.get(fieldName, "")
-            row.append(val)
+    for cellId, rowData in iterItems(allRows):
+        row = []
+        for fileIdx in range(0, len(inFnames)):
+            if fileIdx in rowData:
+                row.extend(rowData[fileIdx])
+            else:
+                row.extend([""]*fieldCounts[fileIdx])
+
+        ofh.write(cellId)
+        ofh.write("\t")
         ofh.write("\t".join(row))
         ofh.write("\n")
+
+    ofh.close()
+    os.rename(tmpFname, outFname)
+    logging.info("Wrote %d lines (not counting header)" % len(allRows))
+
+def crangerToCellbrowser(datasetName, inDir, outDir):
+    " convert cellranger output to a cellbrowser directory "
+    makeDir(outDir)
+    # copy over the clusters
+    clustFname = join(inDir, "analysis/clustering/graphclust/clusters.csv")
+    if not isfile(clustFname):
+        logging.warn("Cannot find %s" % clustFname)
+        clustFname = join(inDir, "analysis/kmeans/10_clusters/clusters.csv")
+        logging.warn("Using%s instead" % clustFname)
+    metaFname = join(outDir, "meta.csv")
+    shutil.copy(clustFname, metaFname)
+
+    # copy over the t-SNE coords
+    tsneFname = join(inDir, "analysis/tsne/2_components/projection.csv")
+    if not isfile(tsneFname):
+        tsneFname = join(inDir, "analysis/tsne/projection.csv")
+    coordFname = join(outDir, "tsne.coords.csv")
+    shutil.copy(tsneFname, coordFname)
+
+    # copy over the markers
+    dgeFname = join(inDir, "analysis/diffexp/graphclust/differential_expression.csv")
+    if not isfile(dgeFname):
+        logging.warn("Not found: %s" % dgeFname)
+        dgeFname = join(inDir, "analysis/kmeans/10_clusters/differential_expression.csv")
+        logging.warn("Using instead: %s" % dgeFname)
+
+    markerFname = join(outDir, "markers.tsv")
+    geneFname = join(outDir, "gene2sym.tsv")
+    crangerSignMarkers(dgeFname, markerFname, geneFname, 0.01, 100)
+
+    # convert the matrix
+    outExprFname = join(outDir, "exprMatrix.tsv.gz")
+    mask1 = join(inDir, "filtered_gene_bc_matrices/*/matrix.mtx")
+    logging.info("Looking for %s" % mask1)
+    matFnames = glob.glob(mask1)
+    if len(matFnames)!=0:
+        assert(len(matFnames)==1)
+        matFname = matFnames[0]
+        barcodeFname = matFname.replace("matrix.mtx", "barcodes.tsv")
+        geneFname = matFname.replace("matrix.mtx", "genes.tsv")
+        mtxToTsvGz(matFname, geneFname, barcodeFname, outExprFname)
+    else:
+        mask2 = join(inDir, "*_filtered_gene_bc_matrices_h5.h5")
+        logging.info("Looking for %s" % mask2)
+        matFnames = glob.glob(mask2)
+        if len(matFnames)==0:
+            errAbort("Could not find matrix, neither as %s nor as %s" % (mask1, mask2))
+        import scanpy.api as sc
+        logging.info("Reading matrix %s" % matFname)
+        adata = readMatrixAnndata(matFname)
+        anndataToTsv(adata, outExprFname)
+
+    confName = join(outDir, "cellbrowser.conf")
+    coordDescs = [{"file":"tsne.coords.csv", "shortLabel":"CellRanger t-SNE"}]
+    confArgs =  {"meta" : "meta.csv", "clusterField" : "Cluster", "tags" : ["10x"]}
+    writeCellbrowserConf(datasetName, coordDescs, confName, confArgs)
+
+    crangerWriteMethods(inDir, outDir, matFname)
+    generateDownloads(datasetName, outDir)
+
+def crangerWriteMethods(inDir, outDir, matFname):
+    htmlFname = join(outDir, "methods.html")
+    if isfile(htmlFname):
+        logging.info("%s exists, not overwriting" % htmlFname)
+        return
+
+    import csv
+    csvMask = join(inDir, "*_metrics_summary.csv")
+    csvFnames = glob.glob(csvMask)
+    if len(csvFnames)==0:
+        logging.warn("Cannot find %s, not writing %s" % (csvMask, htmlFname))
+        return
+
+    qcVals = list(csv.DictReader(open(csvFnames[0])))[0]
+
+    ofh = open(htmlFname, "w")
+    ofh.write("This dataset was imported from a CellRanger analysis directory with cbCellranger.<p><p>")
+    ofh.write("<p><b>QC metrics reported by CellRanger:</b></p>\n")
+
+    for key, value in iterItems(qcVals):
+        ofh.write("%s: %s<br>\n" % (key, value))
     ofh.close()
     logging.info("Wrote %s" % ofh.name)
 
-def findBoringFields(cellMetaDict):
-    """ return a dict of all fieldNames that have only a single value. The keys of this dict are the field names, 
-    the values of this dict are the single values."""
-    fieldValues = defaultdict(set)
-    for cellId, cellMeta in iterItems(cellMetaDict):
-        for fieldName, val in iterItems(cellMeta):
-            fieldValues[fieldName].add(val)
-
-    boringFields = {}
-    for fieldName, vals in iterItems(fieldValues):
-        if fieldName.endswith("_FILE_NAME") or fieldName.endswith("_URI") or fieldName=="single cell identifier":
-            logging.debug("Skipping field %s" % fieldName)
-            boringFields[fieldName] = None
+def generateDownloads(datasetName, outDir):
+    htmlFname = join(outDir, "downloads.html")
+    if isfile(htmlFname):
+        logging.info("%s exists, not overwriting" % htmlFname)
+        return
+
+    ofh = open(htmlFname, "w")
+    ofh.write("<b>Expression matrix:</b> <a href='%s/exprMatrix.tsv.gz'>exprMatrix.tsv.gz</a><p>\n" % datasetName)
+
+    cFname = join(outDir, "cellbrowser.conf")
+    if isfile(cFname):
+        conf = loadConfig(cFname)
+        if "unit" in conf:
+            ofh.write("Unit of expression matrix: %s<p>\n" % conf["unit"])
+
+    ofh.write("<b>Cell meta annotations:</b> <a href='%s/meta.tsv'>meta.tsv</a><p>" % datasetName)
+
+    coordDescs = conf["coords"]
+    for coordDesc in coordDescs:
+        coordLabel = coordDesc["shortLabel"]
+        cleanName = sanitizeName(coordLabel.replace(" ", "_"))
+        coordFname = cleanName+".coords.tsv.gz"
+        ofh.write("<b>%s coordinates:</b> <a href='%s/%s'>%s</a><br>" % (coordLabel, datasetName, coordFname, coordFname))
+
+    rdsFname = join(datasetName, "seurat.rds")
+    if isfile(rdsFname):
+        ofh.write("<b>Seurat R data file:</b> <a href='%s'>seurat.rds</a><p>" % rdsFname)
+
+    scriptFname = join(datasetName, "runSeurat.R")
+    if isfile(scriptFname):
+        ofh.write("<b>Seurat R analysis script:</b> <a href='%s'>runSeurat.R</a><p>" % scriptFname)
+
+    logFname = join(datasetName, "analysisLog.txt")
+    if isfile(logFname):
+        ofh.write("<b>Analysis Log File:</b> <a href='%s'>analysisLog.txt</a><p>" % logFname)
+
+def crangerSignMarkers(dgeFname, markerFname, geneFname, maxPval, maxGenes):
+    " convert cellranger diff exp file to markers.tsv file "
+    # Old Cellranger 1 format:
+    # Gene ID,Gene Name,Cluster 1 Weight,Cluster 1 UMI counts/cell,Cluster 2 Weight,Cluster 2 UMI counts/cell,Cluster 3 Weight,Cluster 3 UMI counts/cell,Cluster 4 Weight,Cluster 4 UMI counts/cell,Cluster 5 Weight,Cluster 5 UMI counts/cell,Cluster 6 Weight,Cluster 6 UMI counts/cell,Cluster 7 Weight,Cluster 7 UMI counts/cell,Cluster 8 Weight,Cluster 8 UMI counts/cell,Cluster 9 Weight,Cluster 9 UMI counts/cell,Cluster 10 Weight,Cluster 10 UMI counts/cell
+
+    ofh = open(markerFname, "w")
+    ofh.write("cluster\tgene\tAdj. P-Value\tLog2 fold change\tMean UMI Counts\n")
+
+    clusterToGenes = defaultdict(list)
+
+    # read the significant markers and their p-Values
+    for line in open(dgeFname):
+        if line.startswith("Gene ID"):
+            if "Cluster 1 Weight" in line:
+                fieldsProCluster = 2
+                fileVersion = 1
+            else:
+                fieldsProCluster = 3
+                fileVersion = 2
             continue
-        if len(vals)==1:
-            boringFields[fieldName] = list(vals)[0]
-    return boringFields
-
-def writeAcronyms(cellMeta, acroFname):
-    " extract acronyms from inferred cell name field "
-    ofh = open(acroFname, "w")
-    for cellId, metaDict in iterItems(cellMeta):
-        cellName = metaDict.get("inferred cell type")
-        if cellName and "(" in cellName:
-            longName, shortName = cellName.split("(")
-            longName = longName.strip()
-            shortName = shortName.strip(")")
-            metaDict["inferred cell type"] = shortName
-            ofh.write(shortName+"\t"+longName+"\n")
+        row = line.rstrip("\n\r").split(",")
+        geneId = row[0]
+        sym = row[1]
+        clusterCount = int((len(row)-2) / fieldsProCluster)
+        for clusterIdx in range(0, clusterCount):
+            startField = (clusterIdx*fieldsProCluster)+2
+            if fileVersion==2:
+                mean = float(row[startField])
+                fc = float(row[startField+1])
+                pVal = float(row[startField+2])
+            else:
+                fc = float(row[startField])
+                mean = float(row[startField+1])
+                pVal = 0.0001
+
+            if pVal < maxPval:
+                clusterToGenes[clusterIdx+1].append((fc, mean, pVal, sym))
+
+    # write out the markers
+    for clusterId, clusterGenes in iterItems(clusterToGenes):
+        clusterGenes.sort(key=operator.itemgetter(2)) # sort by fold change
+        maxIdx = min(maxGenes, len(clusterGenes))
+        for i in range(0, maxIdx):
+            fc, mean, pVal, sym = clusterGenes[i]
+            ofh.write("%d\t%s\t%g\t%f\t%f\n" % (clusterId, sym, pVal, fc, mean))
+
     ofh.close()
     logging.info("Wrote %s" % ofh.name)
-    return cellMeta
 
-def convertFromEbi(origDir, acc, outDir):
-    " convert single cell expression files to cell browser format "
-    # cluster is a special meta data attribute, parse it into a dict
-    clusterFname = join(origDir, acc+".clusters.tsv")
-    bestK, clusters = parseClusters(clusterFname)
-
-    # best K determines marker file name
-    markerFname = join(origDir, acc+".marker_genes_%s.tsv" % bestK)
-    newMarkerFname = join(outDir, "markers.tsv")
-    topGenes = convertMarkers(markerFname, newMarkerFname)
-
-    quickGeneFname = join(outDir, "quickGenes.tsv")
-    writeQuickGenes(topGenes, quickGeneFname)
-
-    # make sure we use the same cellID order in meta and matrix
-    sampleNameFname = join(origDir, acc+".aggregated_filtered_counts.mtx_cols")
-    sampleNames = open(sampleNameFname).read().splitlines()
-
-    # meta data
-    sdrfFname = join(origDir, acc+".sdrf.txt")
-    #fieldNames, sdrfInfo = parseSdrf(sdrfFname)
-    fieldNames = parseSdrfFieldNames(sdrfFname) # we're doing this to get them in the proper order
-    condSdrfFname = join(origDir, acc+".condensed-sdrf.tsv")
-    cellMeta = parseCondSdrf(sampleNames, condSdrfFname)
-    boringFields = findBoringFields(cellMeta)
-
-    # default perp is 25
-    coordFname = join(origDir, acc+".tsne_perp_25.tsv")
-    newCoordFname = join(outDir, "tsne_perp25.coords.tsv")
-    convertCoords(coordFname, newCoordFname)
-
-    # dataset descriptor
-    idfFname = join(origDir, acc+".idf.txt")
-    idfInfo = parseIdf(idfFname)
-    datasetDesc = translateIdf(idfInfo)
-    datasetDesc["custom"] = boringFields
-    descFname = join(outDir, "desc.conf")
-    writePyConf(datasetDesc, descFname)
-
-    # write acronyms and add the short names to the meta data
-    hasInferred = ("inferred cell type" in fieldNames)
-    if hasInferred:
-        acroFname = join(outDir, "acronyms.tsv")
-        cellMeta = writeAcronyms(cellMeta, acroFname)
-
-    # write the meta 
-    metaFname = join(outDir, "meta.tsv")
-    writeMeta(clusters, sampleNames, fieldNames, boringFields, cellMeta, metaFname)
-
-    # cellbrowser.conf file
-    confFname = join(outDir, "cellbrowser.conf")
-    conf = makeBasicCbConf(acc, datasetDesc["title"], hasInferred)
-    writePyConf(conf, confFname)
-
-    mtxName = join(origDir, acc+".aggregated_filtered_counts.mtx.gz")
-    sampleNamesFname = join(origDir, acc+".aggregated_filtered_counts.mtx_cols")
-    geneNamesFname = join(origDir, acc+".aggregated_filtered_counts.decorated.mtx_rows")
-    outMatName = join(outDir, "exprMatrix.tsv.gz")
-    #runGzip(inMatName, outMatName)
-    if not isfile(outMatName):
-        mtxToTsvGz(mtxName, geneNamesFname, sampleNamesFname, outMatName)
-
-def cbGetCli():
-    " run downloaders "
-    args, options = cbGet_parseArgs()
+def cbCellrangerCli():
+    args, options = cbCellrangerCli_parseArgs()
+
+    if options.outDir is None or options.inDir is None or options.datasetName is None:
+        logging.error("You have to specify at least an input and an output directory and a dataset name.")
+        cbCellrangerCli_parseArgs(showHelp=True)
+
+    crangerToCellbrowser(options.datasetName, options.inDir, options.outDir)
+
+def cbCellrangerCli_parseArgs(showHelp=False):
+    " setup logging, parse command line arguments and options. -h shows auto-generated help page "
+    parser = optparse.OptionParser("""usage: %prog [options] -i cellRangerDir -o outputDir - convert the cellranger output to cellbrowser format and create a cellranger.conf file
 
-    if len(args)<1:
-        cbGet_parseArgs(showHelp=True)
+    """)
+
+    parser.add_option("-d", "--debug", dest="debug", action="store_true",
+        help="show debug messages")
+
+    parser.add_option("-i", "--inDir", dest="inDir", action="store", help="input folder with the cellranger analysis output. This is the directory with the two directories 'analysis' and 'filtered_gene_bc_matrices'")
+    parser.add_option("-o", "--outDir", dest="outDir", action="store", help="output directory")
+    #parser.add_option("-g", "--geneSet", dest="geneSet", action="store", help="geneset, e.g. gencode28 or gencode-m13 or similar. Default: %default", default="gencode24")
+    parser.add_option("-n", "--name", dest="datasetName", action="store", help="name of the dataset")
+
+    (options, args) = parser.parse_args()
+
+    if showHelp:
+        parser.print_help()
+        exit(1)
+
+    setDebug(options.debug)
+
+    return args, options
+
+def cbImportScanpy_parseArgs(showHelp=False):
+    " setup logging, parse command line arguments and options. -h shows auto-generated help page "
+    parser = optparse.OptionParser("""usage: %prog [options] input.h5ad outDir datasetName - convert Scanpy AnnData object to cellbrowser
+
+    Example:
+    - %prog pbmc3k.h5ad pbmc3kScanpy pbmc3kScanpy - convert pbmc3k to directory with tab-separated files
+    """)
+
+    parser.add_option("-d", "--debug", dest="debug", action="store_true",
+        help="show debug messages")
+
+    parser.add_option("", "--htmlDir", dest="htmlDir", action="store",
+        help="do not only convert to tab-sep files but also run cbBuild to"
+            "convert the data and add the dataset under htmlDir")
+
+    parser.add_option("-p", "--port", dest="port", action="store", type="int",
+            help="only with --htmlDir: start webserver on port to serve htmlDir")
+
+    parser.add_option("-m", "--skipMatrix", dest="skipMatrix", action="store_true",
+        help="do not convert the matrix, saves time if the same one has been exported before to the "
+        "same directory")
+
+    (options, args) = parser.parse_args()
+
+    if showHelp:
+        parser.print_help()
+        exit(1)
+
+    setDebug(options.debug)
+    return args, options
+
+def cbImportScanpyCli():
+    " convert h5ad to directory "
+    args, options = cbImportScanpy_parseArgs()
+
+    if len(args)<3:
+        cbImportScanpy_parseArgs(showHelp=True)
         sys.exit(1)
 
-    outDir = options.outDir
-    if outDir is None:
-        outDir = acc
+    inFname, outDir, datasetName = args
 
-    cmd = args[0]
+    import anndata
+    ad = anndata.read_h5ad(inFname)
+    scanpyToCellbrowser(ad, outDir, datasetName, skipMatrix=options.skipMatrix)
 
-    cmds = ["ebi"]
+    if options.port and not options.htmlDir:
+        errAbort("--port requires --htmlDir")
+
+    if options.htmlDir:
+        build(outDir, options.htmlDir, port=options.port)
 
-    if cmd=="ebi":
-        acc = options.acc
-        if options.inDir:
-            origDir = options.inDir
-        else:
-            origDir = join(outDir, "orig")
-            flagFname = join(origDir, "complete")
-            logging.debug("Checking %s" % flagFname)
-            if not isfile(flagFname):
-                hostName = "ftp.ebi.ac.uk"
-                ftpDir = "/pub/databases/microarray/data/atlas/sc_experiments/%s" % acc
-                mirrorFtp(hostName, ftpDir, origDir)
-        convertFromEbi(origDir, acc, outDir)
-    else:
-        errAbort("Repository %s is not valid. Valid repos are: %s" % (cmd, ", ".join(cmds)))
```

### Comparing `cellbrowser-1.2.6/src/cbPyLib/RangeHTTPServer/__main__.py` & `cellbrowser-v0.4.27/src/cbPyLib/RangeHTTPServer/__main__.py`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/RangeHTTPServer/__init__.py` & `cellbrowser-v0.4.27/src/cbPyLib/RangeHTTPServer/__init__.py`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.6/src/cbPyLib/cellbrowser.egg-info/entry_points.txt` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser.egg-info/entry_points.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 [console_scripts]
 cbBuild = cellbrowser.cellbrowser:cbBuildCli
-cbGenes = cellbrowser.genes:cbGenesCli
 cbGuessGencode = cellbrowser.guessgenes:cbGuessGencodeCli
-cbHub = cellbrowser.hubmaker:cbHubCli
 cbImportCellranger = cellbrowser.convert:cbCellrangerCli
 cbImportScanpy = cellbrowser.convert:cbImportScanpyCli
-cbImportSeurat = cellbrowser.seurat:cbImportSeuratCli
+cbImportSeurat2 = cellbrowser.seurat:cbImportSeurat2Cli
 cbMarkerAnnotate = cellbrowser.geneinfo:cbMarkerAnnotateCli
 cbScanpy = cellbrowser.cellbrowser:cbScanpyCli
 cbSeurat = cellbrowser.seurat:cbSeuratCli
 cbTool = cellbrowser.convert:cbToolCli
-cbUpgrade = cellbrowser.cellbrowser:cbUpgradeCli
+cbUpgrade = cellbrowser.cellbrowser:cbMake_cli
```

### Comparing `cellbrowser-1.2.6/MANIFEST.in` & `cellbrowser-v0.4.27/MANIFEST.in`

 * *Files 8% similar despite different names*

```diff
@@ -6,10 +6,8 @@
 #include ../src/cbPyLib/cellbrowser/sampleConfig/cellbrowser.conf
 #include ../src/cbPyLib/cellbrowser/sampleConfig/scanpy.conf
 #include ../src/cbPyLib/cellbrowser/sampleConfig/seurat.conf
 #include cellbrowser/sampleConfig/cellbrowser.conf
 #include cellbrowser/sampleConfig/scanpy.conf
 ##include cellbrowser/sampleConfig/seurat.conf
 include versioneer.py
-include LICENSE
 include src/cbPyLib/cellbrowser/_version.py
-graft src/cbPyLib/cellbrowser/R
```

### Comparing `cellbrowser-1.2.6/versioneer.py` & `cellbrowser-v0.4.27/versioneer.py`

 * *Files identical despite different names*


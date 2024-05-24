# Comparing `tmp/gdstk-0.9.51.tar.gz` & `tmp/gdstk-0.9.52-cp39-cp39-musllinux_1_1_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdstk-0.9.51.tar", last modified: Wed Apr 17 12:48:28 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


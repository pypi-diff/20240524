# Comparing `tmp/mlconcepts-0.0.1a1.tar.gz` & `tmp/mlconcepts-0.0.1a2-cp36-cp36m-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlconcepts-0.0.1a1.tar", last modified: Wed May 15 09:30:47 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


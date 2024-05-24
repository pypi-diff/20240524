# Comparing `tmp/pyjess-0.1.1.tar.gz` & `tmp/pyjess-0.2.0-cp311-cp311-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjess-0.1.1.tar", last modified: Thu Apr 18 16:18:40 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


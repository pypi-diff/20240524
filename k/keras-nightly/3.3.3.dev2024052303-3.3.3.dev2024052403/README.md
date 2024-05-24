# Comparing `tmp/keras_nightly-3.3.3.dev2024052303.tar.gz` & `tmp/keras_nightly-3.3.3.dev2024052403-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras_nightly-3.3.3.dev2024052303.tar", last modified: Thu May 23 03:20:56 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


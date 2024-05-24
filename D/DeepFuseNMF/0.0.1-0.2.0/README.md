# Comparing `tmp/DeepFuseNMF-0.0.1.tar.gz` & `tmp/DeepFuseNMF-0.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepFuseNMF-0.0.1.tar", last modified: Tue Mar 19 15:46:12 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


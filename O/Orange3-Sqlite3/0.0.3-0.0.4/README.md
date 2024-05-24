# Comparing `tmp/orange3_sqlite3-0.0.3.tar.gz` & `tmp/Orange3_Sqlite3-0.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orange3_sqlite3-0.0.3.tar", last modified: Tue May  7 19:34:06 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


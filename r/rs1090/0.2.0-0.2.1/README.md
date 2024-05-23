# Comparing `tmp/rs1090-0.2.0.tar.gz` & `tmp/rs1090-0.2.1-pp39-pypy39_pp73-manylinux_2_12_i686.manylinux2010_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


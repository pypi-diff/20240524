# Comparing `tmp/coherent_test-0.3.0.tar.gz` & `tmp/coherent_test-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coherent_test-0.3.0.tar", last modified: Mon May 20 18:57:47 2024, max compression
+gzip compressed data, was "coherent_test-0.3.1.tar", last modified: Fri May 24 16:39:33 2024, max compression
```

## Comparing `coherent_test-0.3.0.tar` & `coherent_test-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-20 18:57:46.208529 coherent_test-0.3.0/
--rw-r--r--   0 jaraco     (501) staff       (20)      162 2024-05-19 19:18:00.123702 coherent_test-0.3.0/README.md
--rw-r--r--   0 jaraco     (501) staff       (20)       76 2024-05-20 18:56:33.571034 coherent_test-0.3.0/__init__.py
--rw-r--r--   0 jaraco     (501) staff       (20)      448 2024-05-20 18:56:07.499951 coherent_test-0.3.0/__main__.py
--rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-20 18:57:46.208601 coherent_test-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      528 2024-05-20 18:57:47.472283 coherent_test-0.3.0/PKG-INFO
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-24 16:39:32.193159 coherent_test-0.3.1/
+-rw-r--r--   0 jaraco     (501) staff       (20)      162 2024-05-19 19:18:00.123702 coherent_test-0.3.1/README.md
+-rw-r--r--   0 jaraco     (501) staff       (20)       76 2024-05-20 18:56:33.571034 coherent_test-0.3.1/__init__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)      384 2024-05-24 16:38:38.901578 coherent_test-0.3.1/__main__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-24 16:39:32.193230 coherent_test-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      770 2024-05-24 16:39:33.542003 coherent_test-0.3.1/PKG-INFO
```


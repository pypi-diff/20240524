# Comparing `tmp/unprint-0.0.5.tar.gz` & `tmp/unprint-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unprint-0.0.5.tar", last modified: Fri May 24 15:13:48 2024, max compression
+gzip compressed data, was "unprint-0.0.6.tar", last modified: Fri May 24 15:31:48 2024, max compression
```

## Comparing `unprint-0.0.5.tar` & `unprint-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 lzl        (501) staff       (20)        0 2024-05-24 15:13:48.102619 unprint-0.0.5/
--rw-r--r--   0 lzl        (501) staff       (20)        0 2024-05-24 11:43:40.000000 unprint-0.0.5/LICENSE
--rw-r--r--   0 lzl        (501) staff       (20)      560 2024-05-24 15:13:48.102302 unprint-0.0.5/PKG-INFO
--rw-r--r--   0 lzl        (501) staff       (20)       45 2024-05-24 11:23:44.000000 unprint-0.0.5/README.md
--rw-r--r--   0 lzl        (501) staff       (20)       84 2024-05-24 11:24:20.000000 unprint-0.0.5/pyproject.toml
--rw-r--r--   0 lzl        (501) staff       (20)       38 2024-05-24 15:13:48.102666 unprint-0.0.5/setup.cfg
--rw-r--r--   0 lzl        (501) staff       (20)      844 2024-05-24 15:13:47.000000 unprint-0.0.5/setup.py
-drwxr-xr-x   0 lzl        (501) staff       (20)        0 2024-05-24 15:13:48.101026 unprint-0.0.5/unprint/
-drwxr-xr-x   0 lzl        (501) staff       (20)        0 2024-05-24 15:13:48.102115 unprint-0.0.5/unprint/unprint.egg-info/
--rw-r--r--   0 lzl        (501) staff       (20)      560 2024-05-24 15:13:48.000000 unprint-0.0.5/unprint/unprint.egg-info/PKG-INFO
--rw-r--r--   0 lzl        (501) staff       (20)      197 2024-05-24 15:13:48.000000 unprint-0.0.5/unprint/unprint.egg-info/SOURCES.txt
--rw-r--r--   0 lzl        (501) staff       (20)        1 2024-05-24 15:13:48.000000 unprint-0.0.5/unprint/unprint.egg-info/dependency_links.txt
--rw-r--r--   0 lzl        (501) staff       (20)        1 2024-05-24 15:13:48.000000 unprint-0.0.5/unprint/unprint.egg-info/top_level.txt
+drwxr-xr-x   0 lzl        (501) staff       (20)        0 2024-05-24 15:31:48.234459 unprint-0.0.6/
+-rw-r--r--   0 lzl        (501) staff       (20)     1073 2024-05-24 15:30:50.000000 unprint-0.0.6/LICENSE
+-rw-r--r--   0 lzl        (501) staff       (20)      576 2024-05-24 15:31:48.234264 unprint-0.0.6/PKG-INFO
+-rw-r--r--   0 lzl        (501) staff       (20)      170 2024-05-24 15:30:39.000000 unprint-0.0.6/README.md
+-rw-r--r--   0 lzl        (501) staff       (20)      458 2024-05-24 15:30:28.000000 unprint-0.0.6/pyproject.toml
+-rw-r--r--   0 lzl        (501) staff       (20)       38 2024-05-24 15:31:48.234503 unprint-0.0.6/setup.cfg
+-rw-r--r--   0 lzl        (501) staff       (20)      675 2024-05-24 15:26:08.000000 unprint-0.0.6/setup.py
+drwxr-xr-x   0 lzl        (501) staff       (20)        0 2024-05-24 15:31:48.234088 unprint-0.0.6/unprint.egg-info/
+-rw-r--r--   0 lzl        (501) staff       (20)      576 2024-05-24 15:31:48.000000 unprint-0.0.6/unprint.egg-info/PKG-INFO
+-rw-r--r--   0 lzl        (501) staff       (20)      165 2024-05-24 15:31:48.000000 unprint-0.0.6/unprint.egg-info/SOURCES.txt
+-rw-r--r--   0 lzl        (501) staff       (20)        1 2024-05-24 15:31:48.000000 unprint-0.0.6/unprint.egg-info/dependency_links.txt
+-rw-r--r--   0 lzl        (501) staff       (20)        1 2024-05-24 15:31:48.000000 unprint-0.0.6/unprint.egg-info/top_level.txt
```

### Comparing `unprint-0.0.5/setup.py` & `unprint-0.0.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,26 +2,22 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="unprint",
-    version="0.0.5",
+    version="0.0.6",
     author="Liu Zuo Lin",
     author_email="zlliu246@gmail.com",
     description="A simple package to unprint lines in the terminal",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/pypa/sampleproject",
-    project_urls={
-        "Bug Tracker": "https://github.com/pypa/sampleproject/issues",
-    },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    package_dir={"": "unprint"},
-    packages=setuptools.find_packages(where="unprint"),
+    install_requires=[],
+    packages=setuptools.find_packages(),
     python_requires=">=3.7",
 )
```


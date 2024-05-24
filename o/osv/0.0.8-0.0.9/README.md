# Comparing `tmp/osv-0.0.8.tar.gz` & `tmp/osv-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/osv/osv/lib/dist/tmpujqwie3a/osv-0.0.8.tar", last modified: Mon Nov 29 03:31:09 2021, max compression
+gzip compressed data, was "/home/runner/work/osv/osv/lib/dist/tmphos668qw/osv-0.0.9.tar", last modified: Mon Nov 29 04:19:02 2021, max compression
```

## Comparing `osv-0.0.8.tar` & `osv-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 03:31:09.000000 osv-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      783 2021-11-29 03:31:09.000000 osv-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      328 2021-11-29 03:30:56.000000 osv-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 03:31:09.000000 osv-0.0.8/osv/
--rw-r--r--   0 runner    (1001) docker     (121)      711 2021-11-29 03:30:56.000000 osv-0.0.8/osv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 03:31:09.000000 osv-0.0.8/osv/analyze_tool/
--rw-r--r--   0 runner    (1001) docker     (121)     3218 2021-11-29 03:30:56.000000 osv-0.0.8/osv/analyze_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      656 2021-11-29 03:30:56.000000 osv-0.0.8/osv/analyze_tool/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2021-11-29 03:30:56.000000 osv-0.0.8/osv/bug.py
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2021-11-29 03:30:56.000000 osv-0.0.8/osv/bug_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5108 2021-11-29 03:30:56.000000 osv-0.0.8/osv/ecosystems.py
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2021-11-29 03:30:56.000000 osv-0.0.8/osv/ecosystems_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    22159 2021-11-29 03:30:56.000000 osv-0.0.8/osv/impact.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 03:31:09.000000 osv-0.0.8/osv/maven/
--rw-r--r--   0 runner    (1001) docker     (121)      628 2021-11-29 03:30:56.000000 osv-0.0.8/osv/maven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7752 2021-11-29 03:30:56.000000 osv-0.0.8/osv/maven/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     9171 2021-11-29 03:30:56.000000 osv-0.0.8/osv/maven/version_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    24988 2021-11-29 03:30:56.000000 osv-0.0.8/osv/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     5390 2021-11-29 03:30:56.000000 osv-0.0.8/osv/repos.py
--rw-r--r--   0 runner    (1001) docker     (121)     3918 2021-11-29 03:30:56.000000 osv-0.0.8/osv/semver_index.py
--rw-r--r--   0 runner    (1001) docker     (121)     3825 2021-11-29 03:30:56.000000 osv-0.0.8/osv/semver_index_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7848 2021-11-29 03:30:56.000000 osv-0.0.8/osv/sources.py
--rw-r--r--   0 runner    (1001) docker     (121)     5413 2021-11-29 03:30:56.000000 osv-0.0.8/osv/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)    34733 2021-11-29 03:30:56.000000 osv-0.0.8/osv/vulnerability_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 03:31:09.000000 osv-0.0.8/osv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      783 2021-11-29 03:31:09.000000 osv-0.0.8/osv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      564 2021-11-29 03:31:09.000000 osv-0.0.8/osv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-29 03:31:09.000000 osv-0.0.8/osv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-29 03:31:08.000000 osv-0.0.8/osv.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-29 03:31:09.000000 osv-0.0.8/osv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-11-29 03:31:09.000000 osv-0.0.8/osv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-29 03:31:09.000000 osv-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1427 2021-11-29 03:30:56.000000 osv-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 04:19:02.000000 osv-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      783 2021-11-29 04:19:02.000000 osv-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      328 2021-11-29 04:18:48.000000 osv-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 04:19:02.000000 osv-0.0.9/osv/
+-rw-r--r--   0 runner    (1001) docker     (121)      711 2021-11-29 04:18:48.000000 osv-0.0.9/osv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 04:19:02.000000 osv-0.0.9/osv/analyze_tool/
+-rw-r--r--   0 runner    (1001) docker     (121)     3218 2021-11-29 04:18:48.000000 osv-0.0.9/osv/analyze_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2021-11-29 04:18:48.000000 osv-0.0.9/osv/analyze_tool/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1658 2021-11-29 04:18:48.000000 osv-0.0.9/osv/bug.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1460 2021-11-29 04:18:48.000000 osv-0.0.9/osv/bug_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5133 2021-11-29 04:18:48.000000 osv-0.0.9/osv/ecosystems.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1522 2021-11-29 04:18:48.000000 osv-0.0.9/osv/ecosystems_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22159 2021-11-29 04:18:48.000000 osv-0.0.9/osv/impact.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 04:19:02.000000 osv-0.0.9/osv/maven/
+-rw-r--r--   0 runner    (1001) docker     (121)      628 2021-11-29 04:18:48.000000 osv-0.0.9/osv/maven/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7752 2021-11-29 04:18:48.000000 osv-0.0.9/osv/maven/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9171 2021-11-29 04:18:48.000000 osv-0.0.9/osv/maven/version_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24988 2021-11-29 04:18:48.000000 osv-0.0.9/osv/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5390 2021-11-29 04:18:48.000000 osv-0.0.9/osv/repos.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3918 2021-11-29 04:18:48.000000 osv-0.0.9/osv/semver_index.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3825 2021-11-29 04:18:48.000000 osv-0.0.9/osv/semver_index_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7848 2021-11-29 04:18:48.000000 osv-0.0.9/osv/sources.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5413 2021-11-29 04:18:48.000000 osv-0.0.9/osv/tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34733 2021-11-29 04:18:48.000000 osv-0.0.9/osv/vulnerability_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 04:19:02.000000 osv-0.0.9/osv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      783 2021-11-29 04:19:02.000000 osv-0.0.9/osv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      564 2021-11-29 04:19:02.000000 osv-0.0.9/osv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-29 04:19:02.000000 osv-0.0.9/osv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-29 04:19:01.000000 osv-0.0.9/osv.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-29 04:19:02.000000 osv-0.0.9/osv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2021-11-29 04:19:02.000000 osv-0.0.9/osv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-29 04:19:02.000000 osv-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1427 2021-11-29 04:18:48.000000 osv-0.0.9/setup.py
```

### Comparing `osv-0.0.8/PKG-INFO` & `osv-0.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osv
-Version: 0.0.8
+Version: 0.0.9
 Summary: Open Source Vulnerabilities library
 Home-page: https://github.com/google/osv
 Author: OSV authors
 Author-email: osv-discuss@googlegroups.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `osv-0.0.8/osv/__init__.py` & `osv-0.0.9/osv/__init__.py`

 * *Files identical despite different names*

### Comparing `osv-0.0.8/osv/analyze_tool/__init__.py` & `osv-0.0.9/osv/analyze_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `osv-0.0.8/osv/analyze_tool/__main__.py` & `osv-0.0.9/osv/analyze_tool/__main__.py`

 * *Files identical despite different names*

### Comparing `osv-0.0.8/osv/bug.py` & `osv-0.0.9/osv/bug.py`

 * *Files identical despite different names*

### Comparing `osv-0.0.8/osv/bug_test.py` & `osv-0.0.9/osv/bug_test.py`

 * *Files identical despite different names*

### Comparing `osv-0.0.8/osv/ecosystems.py` & `osv-0.0.9/osv/ecosystems.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
   def next_version(self, package, version):
     """Get the next version after the given version."""
     del package  # Unused.
     parsed_version = semver_index.parse(version)
     if parsed_version.prerelease:
       return version + '.0'
 
-    return version + '-0'
+    return str(parsed_version.bump_patch()) + '-0'
 
   @property
   def is_semver(self):
     return True
 
 
 Crates = SemverEcosystem
```

### Comparing `osv-0.0.8/osv/ecosystems_test.py` & `osv-0.0.9/osv/ecosystems_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,13 +31,13 @@
     ecosystem = ecosystems.get('Maven')
     self.assertEqual('1.36.0',
                      ecosystem.next_version('io.grpc:grpc-core', '1.35.1'))
     self.assertEqual('0.7.0', ecosystem.next_version('io.grpc:grpc-core', '0'))
 
   def test_semver(self):
     ecosystem = ecosystems.get('Go')
-    self.assertEqual('1.0.0-0', ecosystem.next_version('blah', '1.0.0'))
+    self.assertEqual('1.0.1-0', ecosystem.next_version('blah', '1.0.0'))
     self.assertEqual('1.0.0-pre.0', ecosystem.next_version('blah', '1.0.0-pre'))
 
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `osv-0.0.8/osv/impact.py` & `osv-0.0.9/osv/impact.py`

 * *Files identical despite different names*

### Comparing `osv-0.0.8/osv/maven/__init__.py` & `osv-0.0.9/osv/maven/__init__.py`

 * *Files identical despite different names*

### Comparing `osv-0.0.8/osv/maven/version.py` & `osv-0.0.9/osv/maven/version.py`

 * *Files identical despite different names*

### Comparing `osv-0.0.8/osv/maven/version_test.py` & `osv-0.0.9/osv/maven/version_test.py`

 * *Files identical despite different names*

### Comparing `osv-0.0.8/osv/models.py` & `osv-0.0.9/osv/models.py`

 * *Files identical despite different names*

### Comparing `osv-0.0.8/osv/repos.py` & `osv-0.0.9/osv/repos.py`

 * *Files identical despite different names*

### Comparing `osv-0.0.8/osv/semver_index.py` & `osv-0.0.9/osv/semver_index.py`

 * *Files identical despite different names*

### Comparing `osv-0.0.8/osv/semver_index_test.py` & `osv-0.0.9/osv/semver_index_test.py`

 * *Files identical despite different names*

### Comparing `osv-0.0.8/osv/sources.py` & `osv-0.0.9/osv/sources.py`

 * *Files identical despite different names*

### Comparing `osv-0.0.8/osv/tests.py` & `osv-0.0.9/osv/tests.py`

 * *Files identical despite different names*

### Comparing `osv-0.0.8/osv/vulnerability_pb2.py` & `osv-0.0.9/osv/vulnerability_pb2.py`

 * *Files identical despite different names*

### Comparing `osv-0.0.8/osv.egg-info/PKG-INFO` & `osv-0.0.9/osv.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osv
-Version: 0.0.8
+Version: 0.0.9
 Summary: Open Source Vulnerabilities library
 Home-page: https://github.com/google/osv
 Author: OSV authors
 Author-email: osv-discuss@googlegroups.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `osv-0.0.8/osv.egg-info/SOURCES.txt` & `osv-0.0.9/osv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osv-0.0.8/setup.py` & `osv-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
   long_description = fh.read()
 
 setuptools.setup(
     name='osv',
-    version='0.0.8',
+    version='0.0.9',
     author='OSV authors',
     author_email='osv-discuss@googlegroups.com',
     description='Open Source Vulnerabilities library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/google/osv',
     packages=setuptools.find_packages(),
```


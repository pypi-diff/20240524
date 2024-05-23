# Comparing `tmp/heaserver_organizations-1.4.1.tar.gz` & `tmp/heaserver_organizations-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver_organizations-1.4.1.tar", last modified: Wed May 22 19:19:24 2024, max compression
+gzip compressed data, was "heaserver_organizations-1.4.2.tar", last modified: Thu May 23 22:34:27 2024, max compression
```

## Comparing `heaserver_organizations-1.4.1.tar` & `heaserver_organizations-1.4.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 19:19:24.178798 heaserver_organizations-1.4.1/
--rw-rw-rw-   0        0        0      261 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.1/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.1/.gitignore
--rw-rw-rw-   0        0        0     1663 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.1/Dockerfile
--rw-rw-rw-   0        0        0    11625 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.1/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5552 2024-05-22 19:19:24.177774 heaserver_organizations-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     4162 2024-05-22 19:18:02.000000 heaserver_organizations-1.4.1/README.md
--rw-rw-rw-   0        0        0     1749 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.1/RELEASING.md
--rw-rw-rw-   0        0        0      594 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.1/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-05-22 19:19:24.039204 heaserver_organizations-1.4.1/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-05-22 19:19:24.039715 heaserver_organizations-1.4.1/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-22 19:19:24.112173 heaserver_organizations-1.4.1/integrationtests/heaserver/organizationintegrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.1/integrationtests/heaserver/organizationintegrationtest/__init__.py
--rw-rw-rw-   0        0        0    10980 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.1/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py
--rw-rw-rw-   0        0        0      835 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.1/integrationtests/heaserver/organizationintegrationtest/test_all.py
--rw-rw-rw-   0        0        0    15050 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.1/integrationtests/heaserver/organizationintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.1/pytest.ini
--rw-rw-rw-   0        0        0      362 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.1/requirements_dev.txt
--rw-rw-rw-   0        0        0     6574 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.1/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-05-22 19:19:24.179326 heaserver_organizations-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1911 2024-05-22 19:18:43.000000 heaserver_organizations-1.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 19:19:24.041506 heaserver_organizations-1.4.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-22 19:19:24.040767 heaserver_organizations-1.4.1/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-22 19:19:24.114234 heaserver_organizations-1.4.1/src/heaserver/organization/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.1/src/heaserver/organization/__init__.py
--rw-rw-rw-   0        0        0    52582 2024-05-22 19:00:26.000000 heaserver_organizations-1.4.1/src/heaserver/organization/service.py
-drwxrwxrwx   0        0        0        0 2024-05-22 19:19:24.128606 heaserver_organizations-1.4.1/src/heaserver/organization/wstl/
--rw-rw-rw-   0        0        0    24887 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.1/src/heaserver/organization/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-05-22 19:19:24.176749 heaserver_organizations-1.4.1/src/heaserver_organizations.egg-info/
--rw-rw-rw-   0        0        0     5552 2024-05-22 19:19:24.000000 heaserver_organizations-1.4.1/src/heaserver_organizations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      997 2024-05-22 19:19:24.000000 heaserver_organizations-1.4.1/src/heaserver_organizations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 19:19:24.000000 heaserver_organizations-1.4.1/src/heaserver_organizations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-22 19:19:24.000000 heaserver_organizations-1.4.1/src/heaserver_organizations.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-05-22 19:19:24.000000 heaserver_organizations-1.4.1/src/heaserver_organizations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-22 19:19:24.000000 heaserver_organizations-1.4.1/src/heaserver_organizations.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-22 19:19:24.042545 heaserver_organizations-1.4.1/tests/
-drwxrwxrwx   0        0        0        0 2024-05-22 19:19:24.042545 heaserver_organizations-1.4.1/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-22 19:19:24.174752 heaserver_organizations-1.4.1/tests/heaserver/organizationtest/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.1/tests/heaserver/organizationtest/__init__.py
--rw-rw-rw-   0        0        0     2214 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.1/tests/heaserver/organizationtest/test_all.py
--rw-rw-rw-   0        0        0     7050 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.1/tests/heaserver/organizationtest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.898150 heaserver_organizations-1.4.2/
+-rw-rw-rw-   0        0        0      261 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.2/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.2/.gitignore
+-rw-rw-rw-   0        0        0     1663 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.2/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.2/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5667 2024-05-23 22:34:27.896500 heaserver_organizations-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4244 2024-05-23 22:33:21.000000 heaserver_organizations-1.4.2/README.md
+-rw-rw-rw-   0        0        0     1749 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.2/RELEASING.md
+-rw-rw-rw-   0        0        0      594 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.2/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.733137 heaserver_organizations-1.4.2/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.733137 heaserver_organizations-1.4.2/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.831032 heaserver_organizations-1.4.2/integrationtests/heaserver/organizationintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.2/integrationtests/heaserver/organizationintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0    10980 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.2/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      835 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.2/integrationtests/heaserver/organizationintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0    15050 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.2/integrationtests/heaserver/organizationintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.2/pytest.ini
+-rw-rw-rw-   0        0        0      362 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.2/requirements_dev.txt
+-rw-rw-rw-   0        0        0     6574 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.2/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 22:34:27.898675 heaserver_organizations-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1931 2024-05-23 22:33:35.000000 heaserver_organizations-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.735136 heaserver_organizations-1.4.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.734137 heaserver_organizations-1.4.2/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.833387 heaserver_organizations-1.4.2/src/heaserver/organization/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.2/src/heaserver/organization/__init__.py
+-rw-rw-rw-   0        0        0    52582 2024-05-22 19:00:26.000000 heaserver_organizations-1.4.2/src/heaserver/organization/service.py
+drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.843820 heaserver_organizations-1.4.2/src/heaserver/organization/wstl/
+-rw-rw-rw-   0        0        0    24887 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.2/src/heaserver/organization/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.895444 heaserver_organizations-1.4.2/src/heaserver_organizations.egg-info/
+-rw-rw-rw-   0        0        0     5667 2024-05-23 22:34:27.000000 heaserver_organizations-1.4.2/src/heaserver_organizations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      997 2024-05-23 22:34:27.000000 heaserver_organizations-1.4.2/src/heaserver_organizations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 22:34:27.000000 heaserver_organizations-1.4.2/src/heaserver_organizations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-23 22:34:27.000000 heaserver_organizations-1.4.2/src/heaserver_organizations.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2024-05-23 22:34:27.000000 heaserver_organizations-1.4.2/src/heaserver_organizations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 22:34:27.000000 heaserver_organizations-1.4.2/src/heaserver_organizations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.736137 heaserver_organizations-1.4.2/tests/
+drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.737137 heaserver_organizations-1.4.2/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-23 22:34:27.892443 heaserver_organizations-1.4.2/tests/heaserver/organizationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.2/tests/heaserver/organizationtest/__init__.py
+-rw-rw-rw-   0        0        0     2214 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.2/tests/heaserver/organizationtest/test_all.py
+-rw-rw-rw-   0        0        0     7050 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.2/tests/heaserver/organizationtest/testcase.py
```

### Comparing `heaserver_organizations-1.4.1/Dockerfile` & `heaserver_organizations-1.4.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.1/LICENSE` & `heaserver_organizations-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.1/PKG-INFO` & `heaserver_organizations-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-organizations
-Version: 1.4.1
+Version: 1.4.2
 Summary: a service for managing organization information for research laboratories and other research groups
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-organizations,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -22,21 +22,25 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: heaserver~=1.6.0
+Requires-Dist: heaobject~=1.6.1
 
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.4.2
+* Corrected heaobject.organization.Organization permissions.
+
 ## Version 1.4.1
 * Generate the correct name attribute for heaobject.keychain.AWSCredentials objects.
 
 ## Version 1.4.0
 * Changing organization members, managers, admins, and PI now changes the users' volumes and credentials objects to
 match.
 * The admin, manager, and member lists now omit system users.
```

### Comparing `heaserver_organizations-1.4.1/README.md` & `heaserver_organizations-1.4.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.4.2
+* Corrected heaobject.organization.Organization permissions.
+
 ## Version 1.4.1
 * Generate the correct name attribute for heaobject.keychain.AWSCredentials objects.
 
 ## Version 1.4.0
 * Changing organization members, managers, admins, and PI now changes the users' volumes and credentials objects to
 match.
 * The admin, manager, and member lists now omit system users.
```

### Comparing `heaserver_organizations-1.4.1/RELEASING.md` & `heaserver_organizations-1.4.2/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.1/docker-entrypoint.sh` & `heaserver_organizations-1.4.2/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.1/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py` & `heaserver_organizations-1.4.2/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.1/integrationtests/heaserver/organizationintegrationtest/test_all.py` & `heaserver_organizations-1.4.2/integrationtests/heaserver/organizationintegrationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.1/integrationtests/heaserver/organizationintegrationtest/testcase.py` & `heaserver_organizations-1.4.2/integrationtests/heaserver/organizationintegrationtest/testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.1/run-swaggerui.py` & `heaserver_organizations-1.4.2/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.1/setup.py` & `heaserver_organizations-1.4.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-organizations',
-    version='1.4.1',
+    version='1.4.2',
     description="a service for managing organization information for research laboratories and other research groups",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.organization'],
     package_data={'heaserver.organization': ['wstl/*.json']},
-    install_requires=['heaserver~=1.6.0'],
+    install_requires=['heaserver~=1.6.0', 'heaobject~=1.6.1'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver_organizations-1.4.1/src/heaserver/organization/service.py` & `heaserver_organizations-1.4.2/src/heaserver/organization/service.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.1/src/heaserver/organization/wstl/all.json` & `heaserver_organizations-1.4.2/src/heaserver/organization/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.1/src/heaserver_organizations.egg-info/PKG-INFO` & `heaserver_organizations-1.4.2/src/heaserver_organizations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-organizations
-Version: 1.4.1
+Version: 1.4.2
 Summary: a service for managing organization information for research laboratories and other research groups
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-organizations,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -22,21 +22,25 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: heaserver~=1.6.0
+Requires-Dist: heaobject~=1.6.1
 
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.4.2
+* Corrected heaobject.organization.Organization permissions.
+
 ## Version 1.4.1
 * Generate the correct name attribute for heaobject.keychain.AWSCredentials objects.
 
 ## Version 1.4.0
 * Changing organization members, managers, admins, and PI now changes the users' volumes and credentials objects to
 match.
 * The admin, manager, and member lists now omit system users.
```

### Comparing `heaserver_organizations-1.4.1/src/heaserver_organizations.egg-info/SOURCES.txt` & `heaserver_organizations-1.4.2/src/heaserver_organizations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.1/tests/heaserver/organizationtest/test_all.py` & `heaserver_organizations-1.4.2/tests/heaserver/organizationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.1/tests/heaserver/organizationtest/testcase.py` & `heaserver_organizations-1.4.2/tests/heaserver/organizationtest/testcase.py`

 * *Files identical despite different names*


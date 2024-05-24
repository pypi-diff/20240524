# Comparing `tmp/espy_contact-2.0.0.tar.gz` & `tmp/espy_contact-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espy_contact-2.0.0.tar", last modified: Fri May 24 06:42:12 2024, max compression
+gzip compressed data, was "espy_contact-2.0.1.tar", last modified: Fri May 24 06:49:19 2024, max compression
```

## Comparing `espy_contact-2.0.0.tar` & `espy_contact-2.0.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:42:12.124818 espy_contact-2.0.0/
--rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-04-26 01:29:16.000000 espy_contact-2.0.0/LICENSE
--rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-24 06:42:12.124540 espy_contact-2.0.0/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      109 2024-05-05 21:34:51.000000 espy_contact-2.0.0/README.md
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:42:12.115104 espy_contact-2.0.0/espy_contact/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.0/espy_contact/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:42:12.117613 espy_contact-2.0.0/espy_contact/model/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:34:03.000000 espy_contact-2.0.0/espy_contact/model/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      558 2024-04-28 03:38:46.000000 espy_contact-2.0.0/espy_contact/model/messaging.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2692 2024-05-24 06:00:52.000000 espy_contact-2.0.0/espy_contact/model/models.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3622 2024-05-07 01:04:59.000000 espy_contact-2.0.0/espy_contact/model/reach.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1821 2024-04-28 03:38:03.000000 espy_contact-2.0.0/espy_contact/model/tranx.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:42:12.120658 espy_contact-2.0.0/espy_contact/schema/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-27 05:18:23.000000 espy_contact-2.0.0/espy_contact/schema/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1170 2024-05-18 16:51:45.000000 espy_contact-2.0.0/espy_contact/schema/blog.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2967 2024-05-24 06:12:34.000000 espy_contact-2.0.0/espy_contact/schema/campus.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      295 2024-04-28 00:12:40.000000 espy_contact-2.0.0/espy_contact/schema/messaging.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     5759 2024-04-28 03:39:29.000000 espy_contact-2.0.0/espy_contact/schema/mgcampus.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1741 2024-05-09 02:58:06.000000 espy_contact-2.0.0/espy_contact/schema/reach.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3395 2024-05-24 05:51:09.000000 espy_contact-2.0.0/espy_contact/schema/schema.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      932 2024-04-28 03:35:00.000000 espy_contact-2.0.0/espy_contact/schema/tranx.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:42:12.121123 espy_contact-2.0.0/espy_contact/service/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-28 00:08:44.000000 espy_contact-2.0.0/espy_contact/service/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1574 2024-04-27 02:59:30.000000 espy_contact-2.0.0/espy_contact/service/service.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:42:12.123290 espy_contact-2.0.0/espy_contact/util/
--rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-04-26 03:59:10.000000 espy_contact-2.0.0/espy_contact/util/CONSTANTS.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:33:54.000000 espy_contact-2.0.0/espy_contact/util/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1055 2024-05-12 03:28:55.000000 espy_contact-2.0.0/espy_contact/util/db.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3989 2024-05-23 21:32:05.000000 espy_contact-2.0.0/espy_contact/util/enums.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      113 2024-05-20 14:38:12.000000 espy_contact-2.0.0/espy_contact/util/esread.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     4353 2024-05-24 05:29:17.000000 espy_contact-2.0.0/espy_contact/util/pg.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:42:12.115742 espy_contact-2.0.0/espy_contact.egg-info/
--rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-24 06:42:12.000000 espy_contact-2.0.0/espy_contact.egg-info/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      914 2024-05-24 06:42:12.000000 espy_contact-2.0.0/espy_contact.egg-info/SOURCES.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-05-24 06:42:12.000000 espy_contact-2.0.0/espy_contact.egg-info/dependency_links.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       77 2024-05-24 06:42:12.000000 espy_contact-2.0.0/espy_contact.egg-info/requires.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       19 2024-05-24 06:42:12.000000 espy_contact-2.0.0/espy_contact.egg-info/top_level.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-05-24 06:42:12.124929 espy_contact-2.0.0/setup.cfg
--rw-r--r--   0 philipadigun   (501) staff       (20)      659 2024-05-24 06:40:00.000000 espy_contact-2.0.0/setup.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:42:12.124258 espy_contact-2.0.0/tests/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.0/tests/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1621 2024-04-26 01:31:37.000000 espy_contact-2.0.0/tests/test_copyright.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.0/tests/test_service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:49:19.660006 espy_contact-2.0.1/
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-04-26 01:29:16.000000 espy_contact-2.0.1/LICENSE
+-rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-24 06:49:19.659864 espy_contact-2.0.1/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      109 2024-05-05 21:34:51.000000 espy_contact-2.0.1/README.md
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:49:19.651995 espy_contact-2.0.1/espy_contact/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.1/espy_contact/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:49:19.653900 espy_contact-2.0.1/espy_contact/model/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:34:03.000000 espy_contact-2.0.1/espy_contact/model/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      558 2024-04-28 03:38:46.000000 espy_contact-2.0.1/espy_contact/model/messaging.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2692 2024-05-24 06:00:52.000000 espy_contact-2.0.1/espy_contact/model/models.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3622 2024-05-07 01:04:59.000000 espy_contact-2.0.1/espy_contact/model/reach.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1821 2024-04-28 03:38:03.000000 espy_contact-2.0.1/espy_contact/model/tranx.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:49:19.656785 espy_contact-2.0.1/espy_contact/schema/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-27 05:18:23.000000 espy_contact-2.0.1/espy_contact/schema/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1170 2024-05-18 16:51:45.000000 espy_contact-2.0.1/espy_contact/schema/blog.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2918 2024-05-24 06:48:35.000000 espy_contact-2.0.1/espy_contact/schema/campus.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      295 2024-04-28 00:12:40.000000 espy_contact-2.0.1/espy_contact/schema/messaging.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     5759 2024-04-28 03:39:29.000000 espy_contact-2.0.1/espy_contact/schema/mgcampus.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1741 2024-05-09 02:58:06.000000 espy_contact-2.0.1/espy_contact/schema/reach.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3395 2024-05-24 05:51:09.000000 espy_contact-2.0.1/espy_contact/schema/schema.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      932 2024-04-28 03:35:00.000000 espy_contact-2.0.1/espy_contact/schema/tranx.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:49:19.657517 espy_contact-2.0.1/espy_contact/service/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-28 00:08:44.000000 espy_contact-2.0.1/espy_contact/service/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1574 2024-04-27 02:59:30.000000 espy_contact-2.0.1/espy_contact/service/service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:49:19.659036 espy_contact-2.0.1/espy_contact/util/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-04-26 03:59:10.000000 espy_contact-2.0.1/espy_contact/util/CONSTANTS.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:33:54.000000 espy_contact-2.0.1/espy_contact/util/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1055 2024-05-12 03:28:55.000000 espy_contact-2.0.1/espy_contact/util/db.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3989 2024-05-23 21:32:05.000000 espy_contact-2.0.1/espy_contact/util/enums.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      113 2024-05-20 14:38:12.000000 espy_contact-2.0.1/espy_contact/util/esread.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     4353 2024-05-24 05:29:17.000000 espy_contact-2.0.1/espy_contact/util/pg.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:49:19.652608 espy_contact-2.0.1/espy_contact.egg-info/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-24 06:49:19.000000 espy_contact-2.0.1/espy_contact.egg-info/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      914 2024-05-24 06:49:19.000000 espy_contact-2.0.1/espy_contact.egg-info/SOURCES.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-05-24 06:49:19.000000 espy_contact-2.0.1/espy_contact.egg-info/dependency_links.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       77 2024-05-24 06:49:19.000000 espy_contact-2.0.1/espy_contact.egg-info/requires.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       19 2024-05-24 06:49:19.000000 espy_contact-2.0.1/espy_contact.egg-info/top_level.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-05-24 06:49:19.660068 espy_contact-2.0.1/setup.cfg
+-rw-r--r--   0 philipadigun   (501) staff       (20)      659 2024-05-24 06:49:12.000000 espy_contact-2.0.1/setup.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:49:19.659676 espy_contact-2.0.1/tests/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.1/tests/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1621 2024-04-26 01:31:37.000000 espy_contact-2.0.1/tests/test_copyright.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.1/tests/test_service.py
```

### Comparing `espy_contact-2.0.0/LICENSE` & `espy_contact-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.0/espy_contact/model/messaging.py` & `espy_contact-2.0.1/espy_contact/model/messaging.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.0/espy_contact/model/models.py` & `espy_contact-2.0.1/espy_contact/model/models.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.0/espy_contact/model/reach.py` & `espy_contact-2.0.1/espy_contact/model/reach.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.0/espy_contact/model/tranx.py` & `espy_contact-2.0.1/espy_contact/model/tranx.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.0/espy_contact/schema/blog.py` & `espy_contact-2.0.1/espy_contact/schema/blog.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.0/espy_contact/schema/campus.py` & `espy_contact-2.0.1/espy_contact/schema/campus.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 """
 from pydantic import BaseModel
 from typing import List, Optional
 from datetime import datetime
-from espy_contact.util.enums import ResourceEnum, GradeLevel
-from espy_contact.model.campus import Term
-import uuid
+from espy_contact.util.enums import ResourceEnum, GradeLevel, Term
 
 
 class Resource(BaseModel):
     """Type of resource can be Poll, Form Builder, Questionnaire, RichText, Video, Audio, File, Hyperlink."""
 
     id: Optional[int] = None
     title: str
```

### Comparing `espy_contact-2.0.0/espy_contact/schema/mgcampus.py` & `espy_contact-2.0.1/espy_contact/schema/mgcampus.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.0/espy_contact/schema/reach.py` & `espy_contact-2.0.1/espy_contact/schema/reach.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.0/espy_contact/schema/schema.py` & `espy_contact-2.0.1/espy_contact/schema/schema.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.0/espy_contact/schema/tranx.py` & `espy_contact-2.0.1/espy_contact/schema/tranx.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.0/espy_contact/service/service.py` & `espy_contact-2.0.1/espy_contact/service/service.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.0/espy_contact/util/CONSTANTS.py` & `espy_contact-2.0.1/espy_contact/util/CONSTANTS.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.0/espy_contact/util/db.py` & `espy_contact-2.0.1/espy_contact/util/db.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.0/espy_contact/util/enums.py` & `espy_contact-2.0.1/espy_contact/util/enums.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.0/espy_contact/util/pg.py` & `espy_contact-2.0.1/espy_contact/util/pg.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.0/espy_contact.egg-info/SOURCES.txt` & `espy_contact-2.0.1/espy_contact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.0/setup.py` & `espy_contact-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 VERSION = '0.0.4'
 DESCRIPTION = 'ESSL users management'
 LONG_DESCRIPTION = 'Internal helper package for ESSL users management'
 setup(
     name='espy_contact',
-    version='2.0.0',
+    version='2.0.1',
     packages=find_packages(),
     install_requires=[
         'bcrypt==4.1.2',
         'pytest==8.1.1',
         'pydantic==2.7.1',
         'sqlalchemy==2.0.29',
         'PyYAML ==6.0.1'
```

### Comparing `espy_contact-2.0.0/tests/test_copyright.py` & `espy_contact-2.0.1/tests/test_copyright.py`

 * *Files identical despite different names*


# Comparing `tmp/PT3S-90.14.8.0.dev1.tar.gz` & `tmp/PT3S-90.14.9.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PT3S-90.14.8.0.dev1.tar", last modified: Mon Feb 26 11:12:20 2024, max compression
+gzip compressed data, was "PT3S-90.14.9.0.dev1.tar", last modified: Mon Feb 26 12:55:12 2024, max compression
```

## Comparing `PT3S-90.14.8.0.dev1.tar` & `PT3S-90.14.9.0.dev1.tar`

### file list

```diff
@@ -1,32 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 11:12:20.455770 PT3S-90.14.8.0.dev1/
--rw-rw-rw-   0        0        0    48762 2024-02-13 12:36:04.000000 PT3S-90.14.8.0.dev1/Am.py
--rw-rw-rw-   0        0        0    16320 2024-02-13 12:36:04.000000 PT3S-90.14.8.0.dev1/Dm.py
--rw-rw-rw-   0        0        0    85008 2024-02-14 09:29:49.000000 PT3S-90.14.8.0.dev1/Dx.py
--rw-rw-rw-   0        0        0   122518 2024-02-13 12:36:04.000000 PT3S-90.14.8.0.dev1/Lx.py
--rw-rw-rw-   0        0        0   264794 2024-02-13 15:47:22.000000 PT3S-90.14.8.0.dev1/Mx.py
--rw-rw-rw-   0        0        0     7185 2024-02-13 12:36:04.000000 PT3S-90.14.8.0.dev1/NFD.py
--rw-rw-rw-   0        0        0      724 2024-02-26 11:12:20.446759 PT3S-90.14.8.0.dev1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-02-26 11:12:20.446759 PT3S-90.14.8.0.dev1/PT3S.egg-info/
--rw-rw-rw-   0        0        0      724 2024-02-26 11:12:19.000000 PT3S-90.14.8.0.dev1/PT3S.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2024-02-26 11:12:19.000000 PT3S-90.14.8.0.dev1/PT3S.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 11:12:19.000000 PT3S-90.14.8.0.dev1/PT3S.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2024-02-26 11:12:19.000000 PT3S-90.14.8.0.dev1/PT3S.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-02-26 11:12:19.000000 PT3S-90.14.8.0.dev1/PT3S.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    43812 2024-02-26 11:10:26.000000 PT3S-90.14.8.0.dev1/PT3S.ipynb
--rw-rw-rw-   0        0        0      183 2024-02-13 12:36:04.000000 PT3S-90.14.8.0.dev1/README.rst
--rw-rw-rw-   0        0        0   529732 2024-02-13 12:36:04.000000 PT3S-90.14.8.0.dev1/Rm.py
-drwxrwxrwx   0        0        0        0 2024-02-26 11:12:20.415854 PT3S-90.14.8.0.dev1/UTILS/
--rw-rw-rw-   0        0        0    39929 2024-02-13 12:36:04.000000 PT3S-90.14.8.0.dev1/UTILS/Db.py
--rw-rw-rw-   0        0        0    26818 2024-02-13 12:36:04.000000 PT3S-90.14.8.0.dev1/UTILS/Xml.py
--rw-rw-rw-   0        0        0        2 2024-02-13 12:36:04.000000 PT3S-90.14.8.0.dev1/UTILS/__init__.py
--rw-rw-rw-   0        0        0   654882 2024-02-13 12:36:04.000000 PT3S-90.14.8.0.dev1/Xm.py
--rw-rw-rw-   0        0        0     1507 2024-02-13 12:36:04.000000 PT3S-90.14.8.0.dev1/__init__.py
--rw-rw-rw-   0        0        0    10332 2024-02-26 11:11:48.000000 PT3S-90.14.8.0.dev1/conf.py
--rw-rw-rw-   0        0        0     9129 2024-02-14 18:22:42.000000 PT3S-90.14.8.0.dev1/dxAndMxHelperFcts.py
--rw-rw-rw-   0        0        0    10021 2024-02-13 12:36:04.000000 PT3S-90.14.8.0.dev1/dxDecodeObjsData.py
-drwxrwxrwx   0        0        0        0 2024-02-26 11:12:20.440094 PT3S-90.14.8.0.dev1/lds/
--rw-rw-rw-   0        0        0        2 2024-02-13 12:36:04.000000 PT3S-90.14.8.0.dev1/lds/__init__.py
--rw-rw-rw-   0        0        0    25505 2024-02-13 12:36:04.000000 PT3S-90.14.8.0.dev1/lds/rpts.py
--rw-rw-rw-   0        0        0    37497 2024-02-13 12:36:04.000000 PT3S-90.14.8.0.dev1/pNFD.py
--rw-rw-rw-   0        0        0       42 2024-02-26 11:12:20.456776 PT3S-90.14.8.0.dev1/setup.cfg
--rw-rw-rw-   0        0        0     9484 2024-02-26 11:11:09.000000 PT3S-90.14.8.0.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-26 12:55:12.492024 PT3S-90.14.9.0.dev1/
+-rw-rw-rw-   0        0        0    48762 2024-02-13 12:36:04.000000 PT3S-90.14.9.0.dev1/Am.py
+-rw-rw-rw-   0        0        0    16320 2024-02-13 12:36:04.000000 PT3S-90.14.9.0.dev1/Dm.py
+-rw-rw-rw-   0        0        0    85008 2024-02-14 09:29:49.000000 PT3S-90.14.9.0.dev1/Dx.py
+drwxrwxrwx   0        0        0        0 2024-02-26 12:55:12.410244 PT3S-90.14.9.0.dev1/Examples/
+-rw-rw-rw-   0        0        0  7426048 2024-02-26 11:52:49.000000 PT3S-90.14.9.0.dev1/Examples/DistrictHeating.db3
+drwxrwxrwx   0        0        0        0 2024-02-26 12:55:12.266962 PT3S-90.14.9.0.dev1/Examples/WDDistrictHeating/
+drwxrwxrwx   0        0        0        0 2024-02-26 12:55:12.266962 PT3S-90.14.9.0.dev1/Examples/WDDistrictHeating/B1/
+drwxrwxrwx   0        0        0        0 2024-02-26 12:55:12.266962 PT3S-90.14.9.0.dev1/Examples/WDDistrictHeating/B1/V0/
+drwxrwxrwx   0        0        0        0 2024-02-26 12:55:12.430442 PT3S-90.14.9.0.dev1/Examples/WDDistrictHeating/B1/V0/BZ1/
+-rw-rw-rw-   0        0        0   179964 2024-02-26 11:40:43.000000 PT3S-90.14.9.0.dev1/Examples/WDDistrictHeating/B1/V0/BZ1/M-1-0-1.1.MX1
+-rw-rw-rw-   0        0        0   155140 2024-02-26 11:40:49.000000 PT3S-90.14.9.0.dev1/Examples/WDDistrictHeating/B1/V0/BZ1/M-1-0-1.1.MX3
+-rw-rw-rw-   0        0        0  4343920 2024-02-26 11:40:49.000000 PT3S-90.14.9.0.dev1/Examples/WDDistrictHeating/B1/V0/BZ1/M-1-0-1.1.MXS
+-rw-rw-rw-   0        0        0   122518 2024-02-13 12:36:04.000000 PT3S-90.14.9.0.dev1/Lx.py
+-rw-rw-rw-   0        0        0   264794 2024-02-13 15:47:22.000000 PT3S-90.14.9.0.dev1/Mx.py
+-rw-rw-rw-   0        0        0     7185 2024-02-13 12:36:04.000000 PT3S-90.14.9.0.dev1/NFD.py
+-rw-rw-rw-   0        0        0      724 2024-02-26 12:55:12.492024 PT3S-90.14.9.0.dev1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-02-26 12:55:12.483745 PT3S-90.14.9.0.dev1/PT3S.egg-info/
+-rw-rw-rw-   0        0        0      724 2024-02-26 12:55:11.000000 PT3S-90.14.9.0.dev1/PT3S.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      887 2024-02-26 12:55:11.000000 PT3S-90.14.9.0.dev1/PT3S.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-26 12:55:11.000000 PT3S-90.14.9.0.dev1/PT3S.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2024-02-26 12:55:11.000000 PT3S-90.14.9.0.dev1/PT3S.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-02-26 12:55:11.000000 PT3S-90.14.9.0.dev1/PT3S.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   407604 2024-02-26 12:55:02.000000 PT3S-90.14.9.0.dev1/PT3S.ipynb
+-rw-rw-rw-   0        0        0      183 2024-02-13 12:36:04.000000 PT3S-90.14.9.0.dev1/README.rst
+-rw-rw-rw-   0        0        0   529732 2024-02-13 12:36:04.000000 PT3S-90.14.9.0.dev1/Rm.py
+drwxrwxrwx   0        0        0        0 2024-02-26 12:55:12.471504 PT3S-90.14.9.0.dev1/UTILS/
+-rw-rw-rw-   0        0        0    39929 2024-02-13 12:36:04.000000 PT3S-90.14.9.0.dev1/UTILS/Db.py
+-rw-rw-rw-   0        0        0    26818 2024-02-13 12:36:04.000000 PT3S-90.14.9.0.dev1/UTILS/Xml.py
+-rw-rw-rw-   0        0        0        2 2024-02-13 12:36:04.000000 PT3S-90.14.9.0.dev1/UTILS/__init__.py
+-rw-rw-rw-   0        0        0   654882 2024-02-13 12:36:04.000000 PT3S-90.14.9.0.dev1/Xm.py
+-rw-rw-rw-   0        0        0     1507 2024-02-13 12:36:04.000000 PT3S-90.14.9.0.dev1/__init__.py
+-rw-rw-rw-   0        0        0    10332 2024-02-26 12:52:21.000000 PT3S-90.14.9.0.dev1/conf.py
+-rw-rw-rw-   0        0        0     9129 2024-02-14 18:22:42.000000 PT3S-90.14.9.0.dev1/dxAndMxHelperFcts.py
+-rw-rw-rw-   0        0        0    10021 2024-02-13 12:36:04.000000 PT3S-90.14.9.0.dev1/dxDecodeObjsData.py
+drwxrwxrwx   0        0        0        0 2024-02-26 12:55:12.483745 PT3S-90.14.9.0.dev1/lds/
+-rw-rw-rw-   0        0        0        2 2024-02-13 12:36:04.000000 PT3S-90.14.9.0.dev1/lds/__init__.py
+-rw-rw-rw-   0        0        0    25505 2024-02-13 12:36:04.000000 PT3S-90.14.9.0.dev1/lds/rpts.py
+-rw-rw-rw-   0        0        0    37497 2024-02-13 12:36:04.000000 PT3S-90.14.9.0.dev1/pNFD.py
+-rw-rw-rw-   0        0        0       42 2024-02-26 12:55:12.492024 PT3S-90.14.9.0.dev1/setup.cfg
+-rw-rw-rw-   0        0        0     9973 2024-02-26 12:52:18.000000 PT3S-90.14.9.0.dev1/setup.py
```

### Comparing `PT3S-90.14.8.0.dev1/Am.py` & `PT3S-90.14.9.0.dev1/Am.py`

 * *Files identical despite different names*

### Comparing `PT3S-90.14.8.0.dev1/Dm.py` & `PT3S-90.14.9.0.dev1/Dm.py`

 * *Files identical despite different names*

### Comparing `PT3S-90.14.8.0.dev1/Dx.py` & `PT3S-90.14.9.0.dev1/Dx.py`

 * *Files identical despite different names*

### Comparing `PT3S-90.14.8.0.dev1/Lx.py` & `PT3S-90.14.9.0.dev1/Lx.py`

 * *Files identical despite different names*

### Comparing `PT3S-90.14.8.0.dev1/Mx.py` & `PT3S-90.14.9.0.dev1/Mx.py`

 * *Files identical despite different names*

### Comparing `PT3S-90.14.8.0.dev1/NFD.py` & `PT3S-90.14.9.0.dev1/NFD.py`

 * *Files identical despite different names*

### Comparing `PT3S-90.14.8.0.dev1/PKG-INFO` & `PT3S-90.14.9.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PT3S
-Version: 90.14.8.0.dev1
+Version: 90.14.9.0.dev1
 Summary: Python Tools 3S
 Home-page: https://github.com/aw3s/PT3S
 Author: PT3S
 Author-email: andreashwolters@gmail.com
 License: MIT
 Keywords: Python Tools 3S
 Requires-Python: >=3
```

### Comparing `PT3S-90.14.8.0.dev1/PT3S.egg-info/PKG-INFO` & `PT3S-90.14.9.0.dev1/PT3S.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PT3S
-Version: 90.14.8.0.dev1
+Version: 90.14.9.0.dev1
 Summary: Python Tools 3S
 Home-page: https://github.com/aw3s/PT3S
 Author: PT3S
 Author-email: andreashwolters@gmail.com
 License: MIT
 Keywords: Python Tools 3S
 Requires-Python: >=3
```

### Comparing `PT3S-90.14.8.0.dev1/Rm.py` & `PT3S-90.14.9.0.dev1/Rm.py`

 * *Files identical despite different names*

### Comparing `PT3S-90.14.8.0.dev1/UTILS/Db.py` & `PT3S-90.14.9.0.dev1/UTILS/Db.py`

 * *Files identical despite different names*

### Comparing `PT3S-90.14.8.0.dev1/UTILS/Xml.py` & `PT3S-90.14.9.0.dev1/UTILS/Xml.py`

 * *Files identical despite different names*

### Comparing `PT3S-90.14.8.0.dev1/Xm.py` & `PT3S-90.14.9.0.dev1/Xm.py`

 * *Files identical despite different names*

### Comparing `PT3S-90.14.8.0.dev1/__init__.py` & `PT3S-90.14.9.0.dev1/__init__.py`

 * *Files identical despite different names*

### Comparing `PT3S-90.14.8.0.dev1/conf.py` & `PT3S-90.14.9.0.dev1/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '90.14'
 # The full version, including alpha/beta/rc tags.
-release = '90.14.8.0.dev1'
+release = '90.14.9.0.dev1'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `PT3S-90.14.8.0.dev1/dxAndMxHelperFcts.py` & `PT3S-90.14.9.0.dev1/dxAndMxHelperFcts.py`

 * *Files identical despite different names*

### Comparing `PT3S-90.14.8.0.dev1/dxDecodeObjsData.py` & `PT3S-90.14.9.0.dev1/dxDecodeObjsData.py`

 * *Files identical despite different names*

### Comparing `PT3S-90.14.8.0.dev1/lds/rpts.py` & `PT3S-90.14.9.0.dev1/lds/rpts.py`

 * *Files identical despite different names*

### Comparing `PT3S-90.14.8.0.dev1/pNFD.py` & `PT3S-90.14.9.0.dev1/pNFD.py`

 * *Files identical despite different names*

### Comparing `PT3S-90.14.8.0.dev1/setup.py` & `PT3S-90.14.9.0.dev1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 setup(
     name='PT3S',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='90.14.8.0.dev1',
+    version='90.14.9.0.dev1',
 
     description='Python Tools 3S',
     long_description=long_description,
 
     # The project's main homepage.
     url='https://github.com/aw3s/PT3S',
 
@@ -91,129 +91,136 @@
 
     # If there are data files included in your packages that need to be
     # installed, specify them here.  If using Python 2.6 or less, then these
     # have to be included in MANIFEST.in as well.
     package_data={
         'PT3S': [           
             'PT3S.ipynb'          
-           ,'PT3S.html'
-           ,'PT3S.pdf'  
+        #   ,'PT3S.html'
+        #   ,'PT3S.pdf' 
+        
+            ,'Examples\DistrictHeating.db3'
+            ,'Examples\WDDistrictHeating\B1\V0\BZ1\M-1-0-1.1.MX1'       
+            ,'Examples\WDDistrictHeating\B1\V0\BZ1\M-1-0-1.1.MX2'               
+            ,'Examples\WDDistrictHeating\B1\V0\BZ1\M-1-0-1.1.MX3'               
+            ,'Examples\WDDistrictHeating\B1\V0\BZ1\M-1-0-1.1.MXS'               
+        
            #,'Lx.ipynb'
-           ,'NFD Module Test.ipynb'
-           ,'NFD Module Test.html'
-           ,'fPngFromPdf Module Test.ipynb'
-           ,'fPngFromPdf Module Test.html'
-           ,'GraphDecomp Module Test.ipynb'
-           ,'GraphDecomp Module Test.html'
+        #   ,'NFD Module Test.ipynb'
+        #   ,'NFD Module Test.html'
+        #   ,'fPngFromPdf Module Test.ipynb'
+        #   ,'fPngFromPdf Module Test.html'
+        #   ,'GraphDecomp Module Test.ipynb'
+        #   ,'GraphDecomp Module Test.html'
            #,'testdata\Lx\20201113_151238a - 6 Logs.7z'
-           ,'testdata\OneLPipe.XML'
+        #   ,'testdata\OneLPipe.XML'
            #,'testdata\OneLPipe.mdb'
-           ,'testdata\WDOneLPipe\B1\V0\BZ1\M-1-0-1.1.MX1'
-           ,'testdata\WDOneLPipe\B1\V0\BZ1\M-1-0-1.MX2'
-           ,'testdata\WDOneLPipe\B1\V0\BZ1\M-1-0-1.1.MXS'
-           ,'testdata\LocalHeatingNetwork.XML'
+        #   ,'testdata\WDOneLPipe\B1\V0\BZ1\M-1-0-1.1.MX1'
+        #   ,'testdata\WDOneLPipe\B1\V0\BZ1\M-1-0-1.MX2'
+        #   ,'testdata\WDOneLPipe\B1\V0\BZ1\M-1-0-1.1.MXS'
+        #   ,'testdata\LocalHeatingNetwork.XML'
            #,'testdata\LocalHeatingNetwork.mdb'
-           ,'testdata\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.1.MX1'
-           ,'testdata\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.MX2'
-           ,'testdata\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.1.MXS'
-           ,'testdata\TinyWDN.XML'
+        #   ,'testdata\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.1.MX1'
+        #   ,'testdata\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.MX2'
+        #   ,'testdata\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.1.MXS'
+        #   ,'testdata\TinyWDN.XML'
            #,'testdata\TinyWDN.mdb'
-           ,'testdata\WDTinyWDN\B1\V0\BZ1\M-1-0-1.1.MX1'
-           ,'testdata\WDTinyWDN\B1\V0\BZ1\M-1-0-1.MX2'
-           ,'testdata\WDTinyWDN\B1\V0\BZ1\M-1-0-1.1.MXS'
-           ,'testdata\GPipes.XML'
-           ,'testdata\WDGPipes\B1\V0\BZ1\M-1-0-1.1.MX1'
-           ,'testdata\WDGPipes\B1\V0\BZ1\M-1-0-1.MX2'
-           ,'testdata\WDGPipes\B1\V0\BZ1\M-1-0-1.1.MXS'
-           ,'testdata\GPipe.XML'
+        #   ,'testdata\WDTinyWDN\B1\V0\BZ1\M-1-0-1.1.MX1'
+        #   ,'testdata\WDTinyWDN\B1\V0\BZ1\M-1-0-1.MX2'
+        #   ,'testdata\WDTinyWDN\B1\V0\BZ1\M-1-0-1.1.MXS'
+        #   ,'testdata\GPipes.XML'
+        #   ,'testdata\WDGPipes\B1\V0\BZ1\M-1-0-1.1.MX1'
+        #   ,'testdata\WDGPipes\B1\V0\BZ1\M-1-0-1.MX2'
+        #   ,'testdata\WDGPipes\B1\V0\BZ1\M-1-0-1.1.MXS'
+        #   ,'testdata\GPipe.XML'
            #,'testdata\GPipe.mdb'
-           ,'testdata\WDGPipe\B1\V0\BZ1\M-1-0-1.1.MX1'
-           ,'testdata\WDGPipe\B1\V0\BZ1\M-1-0-1.MX2'
-           ,'testdata\WDGPipe\B1\V0\BZ1\M-1-0-1.1.MXS'
-           ,'testdata\DHNetwork.XML'
-           ,'testdata\DHNetwork.mdb'
-           ,'testdata\DHNetwork_LINKS.dbf'
-           ,'testdata\DHNetwork_LINKS.shp'
-           ,'testdata\DHNetwork_LINKS.shx'
-           ,'testdata\DHNetwork-ZK.pdf'
-           ,'testdata\WDDHNetwork\B1\V0\BZ1\M-1-0-1.1.MX1'
-           ,'testdata\WDDHNetwork\B1\V0\BZ1\M-1-0-1.MX2'
-           ,'testdata\WDDHNetwork\B1\V0\BZ1\M-1-0-1.1.MXS'
-           ,'testdata\WDDHNetwork\B1\V0\BZ1\GraphDecomp.log'
-           ,'testdata11\OneLPipe.XML'
-           ,'testdata11\OneLPipe.mdb'
-           ,'testdata11\WDOneLPipe\B1\V0\BZ1\M-1-0-1.1.MX1'
-           ,'testdata11\WDOneLPipe\B1\V0\BZ1\M-1-0-1.MX2'
-           ,'testdata11\WDOneLPipe\B1\V0\BZ1\M-1-0-1.1.MXS'
-           ,'testdata11\LocalHeatingNetwork.XML'
-           ,'testdata11\LocalHeatingNetwork.mdb'
-           ,'testdata11\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.1.MX1'
-           ,'testdata11\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.MX2'
-           ,'testdata11\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.1.MXS'
-           ,'testdata11\TinyWDN.XML'
-           ,'testdata11\TinyWDN.mdb'
-           ,'testdata11\WDTinyWDN\B1\V0\BZ1\M-1-0-1.1.MX1'
-           ,'testdata11\WDTinyWDN\B1\V0\BZ1\M-1-0-1.MX2'
-           ,'testdata11\WDTinyWDN\B1\V0\BZ1\M-1-0-1.1.MXS'
-           ,'testdata11\GPipes.XML'
-           ,'testdata11\WDGPipes\B1\V0\BZ1\M-1-0-1.1.MX1'
-           ,'testdata11\WDGPipes\B1\V0\BZ1\M-1-0-1.MX2'
-           ,'testdata11\WDGPipes\B1\V0\BZ1\M-1-0-1.1.MXS'
-           ,'testdata11\GPipe.XML'
-           ,'testdata11\GPipe.mdb'
-           ,'testdata11\WDGPipe\B1\V0\BZ1\M-1-0-1.1.MX1'
-           ,'testdata11\WDGPipe\B1\V0\BZ1\M-1-0-1.MX2'
-           ,'testdata11\WDGPipe\B1\V0\BZ1\M-1-0-1.1.MXS'
-           ,'testdata11\DHNetwork.XML'
-           ,'testdata11\DHNetwork.mdb'
-           ,'testdata11\WDDHNetwork\B1\V0\BZ1\M-1-0-1.1.MX1'
-           ,'testdata11\WDDHNetwork\B1\V0\BZ1\M-1-0-1.MX2'
+        #   ,'testdata\WDGPipe\B1\V0\BZ1\M-1-0-1.1.MX1'
+        #   ,'testdata\WDGPipe\B1\V0\BZ1\M-1-0-1.MX2'
+        #   ,'testdata\WDGPipe\B1\V0\BZ1\M-1-0-1.1.MXS'
+        #   ,'testdata\DHNetwork.XML'
+        #   ,'testdata\DHNetwork.mdb'
+        #   ,'testdata\DHNetwork_LINKS.dbf'
+        #   ,'testdata\DHNetwork_LINKS.shp'
+        #   ,'testdata\DHNetwork_LINKS.shx'
+        #   ,'testdata\DHNetwork-ZK.pdf'
+        #   ,'testdata\WDDHNetwork\B1\V0\BZ1\M-1-0-1.1.MX1'
+        #   ,'testdata\WDDHNetwork\B1\V0\BZ1\M-1-0-1.MX2'
+        #   ,'testdata\WDDHNetwork\B1\V0\BZ1\M-1-0-1.1.MXS'
+        #   ,'testdata\WDDHNetwork\B1\V0\BZ1\GraphDecomp.log'
+        #   ,'testdata11\OneLPipe.XML'
+        #   ,'testdata11\OneLPipe.mdb'
+        #   ,'testdata11\WDOneLPipe\B1\V0\BZ1\M-1-0-1.1.MX1'
+        #   ,'testdata11\WDOneLPipe\B1\V0\BZ1\M-1-0-1.MX2'
+        #   ,'testdata11\WDOneLPipe\B1\V0\BZ1\M-1-0-1.1.MXS'
+        #   ,'testdata11\LocalHeatingNetwork.XML'
+        #   ,'testdata11\LocalHeatingNetwork.mdb'
+        #   ,'testdata11\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.1.MX1'
+        #   ,'testdata11\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.MX2'
+        #   ,'testdata11\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.1.MXS'
+        #   ,'testdata11\TinyWDN.XML'
+        #   ,'testdata11\TinyWDN.mdb'
+        #   ,'testdata11\WDTinyWDN\B1\V0\BZ1\M-1-0-1.1.MX1'
+        #   ,'testdata11\WDTinyWDN\B1\V0\BZ1\M-1-0-1.MX2'
+        #   ,'testdata11\WDTinyWDN\B1\V0\BZ1\M-1-0-1.1.MXS'
+        #   ,'testdata11\GPipes.XML'
+        #   ,'testdata11\WDGPipes\B1\V0\BZ1\M-1-0-1.1.MX1'
+        #   ,'testdata11\WDGPipes\B1\V0\BZ1\M-1-0-1.MX2'
+        #   ,'testdata11\WDGPipes\B1\V0\BZ1\M-1-0-1.1.MXS'
+        #   ,'testdata11\GPipe.XML'
+        #   ,'testdata11\GPipe.mdb'
+        #   ,'testdata11\WDGPipe\B1\V0\BZ1\M-1-0-1.1.MX1'
+        #   ,'testdata11\WDGPipe\B1\V0\BZ1\M-1-0-1.MX2'
+        #   ,'testdata11\WDGPipe\B1\V0\BZ1\M-1-0-1.1.MXS'
+        #   ,'testdata11\DHNetwork.XML'
+        #   ,'testdata11\DHNetwork.mdb'
+        #   ,'testdata11\WDDHNetwork\B1\V0\BZ1\M-1-0-1.1.MX1'
+        #   ,'testdata11\WDDHNetwork\B1\V0\BZ1\M-1-0-1.MX2'
            #,'testdata\WDDHNetwork\B1\V0\BZ1\M-1-0-1.1.MXS'
 
-           ,'testdata10\OneLPipe.XML'
-           ,'testdata10\OneLPipe.mdb'
-           ,'testdata10\WDOneLPipe\B1\V0\BZ1\M-1-0-1.1.MX1'
-           ,'testdata10\WDOneLPipe\B1\V0\BZ1\M-1-0-1.MX2'
-           ,'testdata10\WDOneLPipe\B1\V0\BZ1\M-1-0-1.1.MXS'
-           ,'testdata10\LocalHeatingNetwork.XML'
-           ,'testdata10\LocalHeatingNetwork.mdb'
-           ,'testdata10\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.1.MX1'
-           ,'testdata10\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.MX2'
-           ,'testdata10\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.1.MXS'
-           ,'testdata10\TinyWDN.XML'
-           ,'testdata10\TinyWDN.mdb'
-           ,'testdata10\WDTinyWDN\B1\V0\BZ1\M-1-0-1.1.MX1'
-           ,'testdata10\WDTinyWDN\B1\V0\BZ1\M-1-0-1.MX2'
-           ,'testdata10\WDTinyWDN\B1\V0\BZ1\M-1-0-1.1.MXS'
-           ,'testdata10\GPipe.XML'
-           ,'testdata10\GPipe.mdb'
-           ,'testdata10\WDGPipe\B1\V0\BZ1\M-1-0-1.1.MX1'
-           ,'testdata10\WDGPipe\B1\V0\BZ1\M-1-0-1.MX2'
-           ,'testdata10\WDGPipe\B1\V0\BZ1\M-1-0-1.1.MXS'
-
-           ,'testdata09\OneLPipe.XML'
-           ,'testdata09\OneLPipe.mdb'
-           ,'testdata09\WDOneLPipe\B1\V0\BZ1\M-1-0-1.MX1'
-           ,'testdata09\WDOneLPipe\B1\V0\BZ1\M-1-0-1.MX2'
-           ,'testdata09\WDOneLPipe\B1\V0\BZ1\M-1-0-1.MXS'
-           ,'testdata09\LocalHeatingNetwork.XML'
-           ,'testdata09\LocalHeatingNetwork.mdb'
-           ,'testdata09\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.MX1'
-           ,'testdata09\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.MX2'
-           ,'testdata09\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.MXS'
-           ,'testdata09\TinyWDN.XML'
-           ,'testdata09\TinyWDN.mdb'
-           ,'testdata09\WDTinyWDN\B1\V0\BZ1\M-1-0-1.MX1'
-           ,'testdata09\WDTinyWDN\B1\V0\BZ1\M-1-0-1.MX2'
-           ,'testdata09\WDTinyWDN\B1\V0\BZ1\M-1-0-1.MXS'
-           ,'testdata09\GPipe.XML'
-           ,'testdata09\GPipe.mdb'
-           ,'testdata09\WDGPipe\B1\V0\BZ1\M-1-0-1.MX1'
-           ,'testdata09\WDGPipe\B1\V0\BZ1\M-1-0-1.MX2'
-           ,'testdata09\WDGPipe\B1\V0\BZ1\M-1-0-1.MXS'
+        #   ,'testdata10\OneLPipe.XML'
+        #   ,'testdata10\OneLPipe.mdb'
+        #   ,'testdata10\WDOneLPipe\B1\V0\BZ1\M-1-0-1.1.MX1'
+        #   ,'testdata10\WDOneLPipe\B1\V0\BZ1\M-1-0-1.MX2'
+        #   ,'testdata10\WDOneLPipe\B1\V0\BZ1\M-1-0-1.1.MXS'
+        #  ,'testdata10\LocalHeatingNetwork.XML'
+        #   ,'testdata10\LocalHeatingNetwork.mdb'
+        #   ,'testdata10\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.1.MX1'
+        #   ,'testdata10\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.MX2'
+        #   ,'testdata10\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.1.MXS'
+        #   ,'testdata10\TinyWDN.XML'
+        #   ,'testdata10\TinyWDN.mdb'
+        #   ,'testdata10\WDTinyWDN\B1\V0\BZ1\M-1-0-1.1.MX1'
+        #   ,'testdata10\WDTinyWDN\B1\V0\BZ1\M-1-0-1.MX2'
+        #   ,'testdata10\WDTinyWDN\B1\V0\BZ1\M-1-0-1.1.MXS'
+        #   ,'testdata10\GPipe.XML'
+        #   ,'testdata10\GPipe.mdb'
+        #   ,'testdata10\WDGPipe\B1\V0\BZ1\M-1-0-1.1.MX1'
+        #   ,'testdata10\WDGPipe\B1\V0\BZ1\M-1-0-1.MX2'
+        #   ,'testdata10\WDGPipe\B1\V0\BZ1\M-1-0-1.1.MXS'
+
+        #   ,'testdata09\OneLPipe.XML'
+        #   ,'testdata09\OneLPipe.mdb'
+        #   ,'testdata09\WDOneLPipe\B1\V0\BZ1\M-1-0-1.MX1'
+        #   ,'testdata09\WDOneLPipe\B1\V0\BZ1\M-1-0-1.MX2'
+        #   ,'testdata09\WDOneLPipe\B1\V0\BZ1\M-1-0-1.MXS'
+        #   ,'testdata09\LocalHeatingNetwork.XML'
+        #   ,'testdata09\LocalHeatingNetwork.mdb'
+        #   ,'testdata09\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.MX1'
+        #   ,'testdata09\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.MX2'
+        #   ,'testdata09\WDLocalHeatingNetwork\B1\V0\BZ1\M-1-0-1.MXS'
+        #   ,'testdata09\TinyWDN.XML'
+        #   ,'testdata09\TinyWDN.mdb'
+        #   ,'testdata09\WDTinyWDN\B1\V0\BZ1\M-1-0-1.MX1'
+        #   ,'testdata09\WDTinyWDN\B1\V0\BZ1\M-1-0-1.MX2'
+        #   ,'testdata09\WDTinyWDN\B1\V0\BZ1\M-1-0-1.MXS'
+        #   ,'testdata09\GPipe.XML'
+        #   ,'testdata09\GPipe.mdb'
+        #   ,'testdata09\WDGPipe\B1\V0\BZ1\M-1-0-1.MX1'
+        #   ,'testdata09\WDGPipe\B1\V0\BZ1\M-1-0-1.MX2'
+        #   ,'testdata09\WDGPipe\B1\V0\BZ1\M-1-0-1.MXS'
             ],
     },
 
     # Although 'package_data' is the preferred approach, in some case you may
     # need to place data files outside of your packages. See:
     # http://docs.python.org/3.4/distutils/setupscript.html#installing-additional-files # noqa
     # In this case, 'data_file' will be installed into '<sys.prefix>/my_data'
```


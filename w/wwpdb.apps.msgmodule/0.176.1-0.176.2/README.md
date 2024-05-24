# Comparing `tmp/wwpdb.apps.msgmodule-0.176.1.tar.gz` & `tmp/wwpdb_apps_msgmodule-0.176.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.msgmodule-0.176.1.tar", last modified: Sat Apr 13 10:10:32 2024, max compression
+gzip compressed data, was "wwpdb_apps_msgmodule-0.176.2.tar", last modified: Fri May 24 11:14:58 2024, max compression
```

## Comparing `wwpdb.apps.msgmodule-0.176.1.tar` & `wwpdb_apps_msgmodule-0.176.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:10:32.930486 wwpdb.apps.msgmodule-0.176.1/
--rw-r--r--   0 vsts      (1001) docker     (127)     1131 2024-04-13 10:10:32.930486 wwpdb.apps.msgmodule-0.176.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      301 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-13 10:10:32.934486 wwpdb.apps.msgmodule-0.176.1/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2326 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:10:32.926486 wwpdb.apps.msgmodule-0.176.1/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:10:32.926486 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:10:32.926486 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/
--rwxr-xr-x   0 vsts      (1001) docker     (127)      153 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:10:32.930486 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/depict/
--rw-r--r--   0 vsts      (1001) docker     (127)    38649 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/depict/MessagingDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26771 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/depict/MessagingTemplates.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:10:32.930486 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/
--rw-r--r--   0 vsts      (1001) docker     (127)     1491 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/DateUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4420 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/EmHeaderUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7771 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/MessagingDataExport.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7384 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/MessagingDataImport.py
--rw-r--r--   0 vsts      (1001) docker     (127)   269531 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/MessagingIo.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:10:32.930486 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/models/
--rw-r--r--   0 vsts      (1001) docker     (127)    17412 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/models/Message.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/models/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:10:32.930486 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/util/
--rw-r--r--   0 vsts      (1001) docker     (127)     5613 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/util/AutoMessage.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27417 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/util/ExtractMessage.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/util/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:10:32.930486 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/webapp/
--rw-r--r--   0 vsts      (1001) docker     (127)    83116 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/webapp/MessagingWebApp.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/webapp/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4918 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/webapp/wsgi.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:10:32.930486 wwpdb.apps.msgmodule-0.176.1/wwpdb.apps.msgmodule.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1131 2024-04-13 10:10:32.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb.apps.msgmodule.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1072 2024-04-13 10:10:32.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb.apps.msgmodule.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-13 10:10:32.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb.apps.msgmodule.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-13 10:10:19.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb.apps.msgmodule.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      206 2024-04-13 10:10:32.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb.apps.msgmodule.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-13 10:10:32.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb.apps.msgmodule.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 11:14:58.864301 wwpdb_apps_msgmodule-0.176.2/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1131 2024-05-24 11:14:58.864301 wwpdb_apps_msgmodule-0.176.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      301 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-05-24 11:14:58.864301 wwpdb_apps_msgmodule-0.176.2/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2326 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 11:14:58.860301 wwpdb_apps_msgmodule-0.176.2/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 11:14:58.860301 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 11:14:58.860301 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      153 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 11:14:58.860301 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/depict/
+-rw-r--r--   0 vsts      (1001) docker     (127)    38649 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/depict/MessagingDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26771 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/depict/MessagingTemplates.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 11:14:58.864301 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/io/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1491 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/io/DateUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4420 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/io/EmHeaderUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7771 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/io/MessagingDataExport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7384 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/io/MessagingDataImport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   269981 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/io/MessagingIo.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 11:14:58.864301 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/models/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17412 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/models/Message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/models/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 11:14:58.864301 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/util/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5613 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/util/AutoMessage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27417 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/util/ExtractMessage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/util/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 11:14:58.864301 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (127)    83255 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/webapp/MessagingWebApp.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/webapp/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4918 2024-05-24 11:13:22.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/webapp/wsgi.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 11:14:58.864301 wwpdb_apps_msgmodule-0.176.2/wwpdb.apps.msgmodule.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1131 2024-05-24 11:14:58.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb.apps.msgmodule.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1072 2024-05-24 11:14:58.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb.apps.msgmodule.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-24 11:14:58.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb.apps.msgmodule.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-24 11:14:45.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb.apps.msgmodule.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      206 2024-05-24 11:14:58.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb.apps.msgmodule.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-24 11:14:58.000000 wwpdb_apps_msgmodule-0.176.2/wwpdb.apps.msgmodule.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.msgmodule-0.176.1/PKG-INFO` & `wwpdb_apps_msgmodule-0.176.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.msgmodule
-Version: 0.176.1
+Version: 0.176.2
 Summary: wwPDB messaging module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_ann_tasks_v2
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.msgmodule-0.176.1/setup.py` & `wwpdb_apps_msgmodule-0.176.2/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/depict/MessagingDepict.py` & `wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/depict/MessagingDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/depict/MessagingTemplates.py` & `wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/depict/MessagingTemplates.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/DateUtil.py` & `wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/io/DateUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/EmHeaderUtils.py` & `wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/io/EmHeaderUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/MessagingDataExport.py` & `wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/io/MessagingDataExport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/MessagingDataImport.py` & `wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/io/MessagingDataImport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/MessagingIo.py` & `wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/io/MessagingIo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1404,14 +1404,17 @@
             elif p_tmpltType == "reminder":  # CS 2024-04-04 change type from remind-feedback to reminder to match frontend drop-down
                 msgTmplt = MessagingTemplates.msgTmplt_reminder_em if p_isEmdbEntry else MessagingTemplates.msgTmplt_reminder
                 attachFiles = False
                 isNote = True
                 # Need all ids
                 accstr = templateDict["accession_ids"]
                 subject = "ARCHIVED: Still awaiting feedback for " + accstr
+            else:
+                logger.error("Unknown message template %s", p_tmpltType)
+                msgTmplt = "This is an unknown message template."
 
             # Assemble message with templates
             msg = msgTmplt % templateDict
             #
             messageDict = {
                 "deposition_data_set_id": depId,
                 "sender": p_sender,
@@ -4254,14 +4257,17 @@
 
         if p_IdType == "PDB":
             ctgryNm = "audit_author"
             itemNm = "name"
         elif p_IdType == "EMDB":
             ctgryNm = "em_author_list"
             itemNm = "author"
+        else:
+            logger.error("p_IdType unknown %s", p_IdType)
+            return
 
         try:
             if self.__verbose:
                 logger.info("-- Category name sought from [%s] is: '%s'", self.__dbFilePath, ctgryNm)
             #
             catObj = self.__getCatObj(ctgryNm)
             if catObj:
@@ -4403,14 +4409,17 @@
 
         if p_IdType == "PDB":
             ctgryNm = "struct"
             itemNm = "title"
         elif p_IdType == "EMDB":
             ctgryNm = "em_admin"
             itemNm = "title"
+        else:
+            logger.error("p_IdType unknown %s", p_IdType)
+            return
 
         try:
             if self.__verbose:
                 logger.info("Category name sought from [%s] is: '%s'", self.__dbFilePath, ctgryNm)
             #
             catObj = self.__getCatObj(ctgryNm)
             if catObj:
@@ -4957,14 +4966,17 @@
 
         if p_IdType == "PDB":
             cType = "validation-report-full-annotate"
             frmt = "pdf"
         elif p_IdType == "EMDB":
             cType = "correspondence-to-depositor"
             frmt = "txt"
+        else:
+            logger.error("lastOutboundRpttDate: unknown IdType %s", p_IdType)
+            return
 
         msgDI = MessagingDataImport(self.__reqObj, verbose=self.__verbose, log=self.__lfh)
         pathDict = msgDI.getMileStoneFilePaths(contentType=cType, format=frmt)
         archiveFilePth = pathDict["annotPth"]
 
         if archiveFilePth is not None:
             du = DateUtil()
```

### Comparing `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/models/Message.py` & `wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/models/Message.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/util/AutoMessage.py` & `wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/util/AutoMessage.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/util/ExtractMessage.py` & `wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/util/ExtractMessage.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/webapp/MessagingWebApp.py` & `wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/webapp/MessagingWebApp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1699,14 +1699,17 @@
             logger.info("--------------------------------------------")
             logger.info("+MessagingWebAppWorker.__exitMessagingMod() - starting")
         #
         if mode == "completed":
             state = "closed(0)"
         elif mode == "unfinished":
             state = "waiting"
+        else:
+            state = "unknown"
+            logger.error("+MessagingWebAppWorker.__exitMessagingMod() unknown mode: %s", mode)
         #
         bIsWorkflow = self.__isWorkflow()
         #
         self.__getSession()
         sessionId = self.__sessionId
         depId = self.__reqObj.getValue("identifier")
         instId = self.__reqObj.getValue("instance")
```

### Comparing `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/webapp/wsgi.py` & `wwpdb_apps_msgmodule-0.176.2/wwpdb/apps/msgmodule/webapp/wsgi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176.1/wwpdb.apps.msgmodule.egg-info/PKG-INFO` & `wwpdb_apps_msgmodule-0.176.2/wwpdb.apps.msgmodule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.msgmodule
-Version: 0.176.1
+Version: 0.176.2
 Summary: wwPDB messaging module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_ann_tasks_v2
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.msgmodule-0.176.1/wwpdb.apps.msgmodule.egg-info/SOURCES.txt` & `wwpdb_apps_msgmodule-0.176.2/wwpdb.apps.msgmodule.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/pyocient-3.3.0-py3-none-any.whl.zip` & `tmp/pyocient-3.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 50902 bytes, number of entries: 11
+Zip file size: 50953 bytes, number of entries: 11
 ?rwxrwxrwx  2.0 unx     2871 b- defN 80-Jan-01 00:00 pyocient/__init__.py
-?rwxrwxrwx  2.0 unx   117819 b- defN 80-Jan-01 00:00 pyocient/api.py
+?rwxrwxrwx  2.0 unx   118029 b- defN 80-Jan-01 00:00 pyocient/api.py
 ?rwxrwxrwx  2.0 unx    24540 b- defN 80-Jan-01 00:00 pyocient/cli.py
 ?rwxrwxrwx  2.0 unx    38403 b- defN 80-Jan-01 00:00 pyocient/ocient_protocol_pb2.py
 ?rwxrwxrwx  2.0 unx       43 b- defN 80-Jan-01 00:00 pyocient/pkg_version.py
 ?rwxrwxrwx  2.0 unx    11922 b- defN 80-Jan-01 00:00 pyocient/sso.py
 ?rwxrwxrwx  2.0 unx    11098 b- defN 80-Jan-01 00:00 pyocient/text2sql.py
-?rwxrwxrwx  2.0 unx       91 b- defN 80-Jan-01 00:00 pyocient-3.3.0.dist-info/WHEEL
-?rwxrwxrwx  2.0 unx     2188 b- defN 80-Jan-01 00:00 pyocient-3.3.0.dist-info/METADATA
-?rwxrwxrwx  2.0 unx       44 b- defN 80-Jan-01 00:00 pyocient-3.3.0.dist-info/entry_points.txt
-?rwxrwxrwx  2.0 unx      847 b- defN 80-Jan-01 00:00 pyocient-3.3.0.dist-info/RECORD
-11 files, 209866 bytes uncompressed, 49496 bytes compressed:  76.4%
+?rwxrwxrwx  2.0 unx       91 b- defN 80-Jan-01 00:00 pyocient-3.3.2.dist-info/WHEEL
+?rwxrwxrwx  2.0 unx     2188 b- defN 80-Jan-01 00:00 pyocient-3.3.2.dist-info/METADATA
+?rwxrwxrwx  2.0 unx       44 b- defN 80-Jan-01 00:00 pyocient-3.3.2.dist-info/entry_points.txt
+?rwxrwxrwx  2.0 unx      847 b- defN 80-Jan-01 00:00 pyocient-3.3.2.dist-info/RECORD
+11 files, 210076 bytes uncompressed, 49547 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: pyocient/sso.py
 Comment: 
 
 Filename: pyocient/text2sql.py
 Comment: 
 
-Filename: pyocient-3.3.0.dist-info/WHEEL
+Filename: pyocient-3.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: pyocient-3.3.0.dist-info/METADATA
+Filename: pyocient-3.3.2.dist-info/METADATA
 Comment: 
 
-Filename: pyocient-3.3.0.dist-info/entry_points.txt
+Filename: pyocient-3.3.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: pyocient-3.3.0.dist-info/RECORD
+Filename: pyocient-3.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyocient/api.py

```diff
@@ -1441,15 +1441,15 @@
         if not self.sock:
             raise Error("No connection")
 
         try:
             # Send end session message
             req = proto.Request()
             req.type = req.CLOSE_CONNECTION
-            req.close_connection.endSession = True
+            req.close_connection.endSession = False
             _send_msg(self, req)
         except IOError:
             # Ignore end session errors
             pass
         finally:
             logger.debug("Closing connection on socket %s", self.sock)
             # Do this little dance so that even if the close() call
@@ -1697,14 +1697,16 @@
 
         Parameters may be provided as a mapping and will be bound to variables
         in the operation. Variables are specified in Python extended format codes,
         e.g. ...WHERE name=%(name)s
         """
         self._reinitialize()
 
+        # parameterlist should not be None, but some applications set it so.
+        # Guard against that
         if parameterlist is None:
             parameterlist = {}
 
         # we can't just execute all the queries at once....ocient only allows
         # one query at a time on a connection.  So queue up all the queries and
         # we'll call them later
         for param in parameterlist:
@@ -1720,14 +1722,16 @@
 
         Parameters may be provided as a mapping and will be bound to variables
         in the operation. Variables are specified in Python extended format codes,
         e.g. ...WHERE name=%(name)s
         """
         self._reinitialize()
 
+        # parameters should not be None, but some applications set it so.
+        # Guard against that
         if parameters is None:
             parameters = {}
 
         self._execute_internal(operation, parameters)
 
         return self
```

## pyocient/pkg_version.py

```diff
@@ -1,3 +1,3 @@
 # pyocient version
 #
-__version__ = '3.3.0'
+__version__ = '3.3.2'
```

## Comparing `pyocient-3.3.0.dist-info/METADATA` & `pyocient-3.3.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 Requires-Dist: tabulate
 Requires-Dist: cryptography<42.0.0
 Requires-Dist: protobuf>=3.20.0,<=4.22.0
 Provides-Extra: anthropic
 Requires-Dist: anthropic>=0.3.10; extra == 'anthropic'
 Provides-Extra: openai
 Requires-Dist: openai>=0.27.0; extra == 'openai'
-Version: 3.3.0
+Version: 3.3.2
 
 # Ocient Hyperscale Data Warehouse DBAPI Driver
 
 This python database API conforms to the Python Database API
 Specification 2.0 and can be used to access the Ocient database.
 
 This module can also be called as a main function, in which case
```

## Comparing `pyocient-3.3.0.dist-info/RECORD` & `pyocient-3.3.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 pyocient/__init__.py,sha256=NiBZT9ACjmautgXjk-fILb_s4wIfcAIubLtRTZHCFlw,2871
-pyocient/api.py,sha256=IohqmRDMjb7NRCrT6sSsRde1JFtKd7MoqRx9nZvYnzQ,117819
+pyocient/api.py,sha256=Hw66bOKgh1zFCcuWFX5czqTdqQ5ISHYTYr1AspiyQBk,118029
 pyocient/cli.py,sha256=PG7lXecIKr82pgN6ZpCbuxYo6rj8NlOyVHREM2-Ckk8,24540
 pyocient/ocient_protocol_pb2.py,sha256=bHdj-bdtXO9NWrrTP0A3bgGLVaoaXGEDjZDMeKShHdw,38403
-pyocient/pkg_version.py,sha256=fVgwkY_qMMbI1aB3WAOwYc9VFNdgz-w3SaQ280ORvSg,43
+pyocient/pkg_version.py,sha256=4usXEZeVaLkxcPWTRZnZghicLba8_lBj8KyvDAPQfqs,43
 pyocient/sso.py,sha256=F8f3Ro8ps39no7wbWfjG-EgXokqu3o-RXoAvtFFLUkw,11922
 pyocient/text2sql.py,sha256=mYcDdjCsYzsOlaKXHeXRPeJs_jL6b1fgZISgOY8RL8M,11098
-pyocient-3.3.0.dist-info/WHEEL,sha256=sobxWSyDDkdg_rinUth-jxhXHqoNqlmNMJY3aTZn2Us,91
-pyocient-3.3.0.dist-info/METADATA,sha256=S4xbkou8sez7NxySfGdPLQJ11cVo_S7-s0UroQkWCsY,2188
-pyocient-3.3.0.dist-info/entry_points.txt,sha256=GK3p7eqGAjsA9wcwOihIjA6x-acF5qBI2nAMlDT9txQ,44
-pyocient-3.3.0.dist-info/RECORD,,
+pyocient-3.3.2.dist-info/WHEEL,sha256=sobxWSyDDkdg_rinUth-jxhXHqoNqlmNMJY3aTZn2Us,91
+pyocient-3.3.2.dist-info/METADATA,sha256=iGKaknzExE_t3ZtAuea-sZQVal9Snlv2MT9A94OMrr0,2188
+pyocient-3.3.2.dist-info/entry_points.txt,sha256=GK3p7eqGAjsA9wcwOihIjA6x-acF5qBI2nAMlDT9txQ,44
+pyocient-3.3.2.dist-info/RECORD,,
```


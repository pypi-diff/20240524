# Comparing `tmp/speakeasy-client-sdk-python-5.9.2.tar.gz` & `tmp/speakeasy-client-sdk-python-5.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speakeasy-client-sdk-python-5.9.2.tar", last modified: Tue May 21 00:12:54 2024, max compression
+gzip compressed data, was "speakeasy-client-sdk-python-5.9.3.tar", last modified: Thu May 23 00:18:30 2024, max compression
```

## Comparing `speakeasy-client-sdk-python-5.9.2.tar` & `speakeasy-client-sdk-python-5.9.3.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:12:54.374686 speakeasy-client-sdk-python-5.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)    23387 2024-05-21 00:12:54.374686 speakeasy-client-sdk-python-5.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15131 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 00:12:54.374686 speakeasy-client-sdk-python-5.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:12:54.350686 speakeasy-client-sdk-python-5.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:12:54.354686 speakeasy-client-sdk-python-5.9.2/src/speakeasy/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:12:54.354686 speakeasy-client-sdk-python-5.9.2/src/speakeasy/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    29402 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/apiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    22156 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    24848 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    14216 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/embeds.py
--rw-r--r--   0 runner    (1001) docker     (127)    16846 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/github.py
--rw-r--r--   0 runner    (1001) docker     (127)    10843 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:12:54.354686 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:12:54.358686 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/errors/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:12:54.358686 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:12:54.366686 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/deleteapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/deleteapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/deleteschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/deleteversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/downloadschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/downloadschemarevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/findapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/generateopenapispec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/generatepostmancollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/generaterequestpostmancollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getallapiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getallapiversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getallforversionapiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getapis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getblob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getchangesreportsignedurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getembedaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getlintingreportsignedurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getnamespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getorganizations.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getorganizationusage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getrequestfromeventlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getrevisions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getschemadiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getschemarevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getschemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/gettags.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getvalidembedaccesstokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getworkspaceaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getworkspaceeventsbytarget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getworkspacetargets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/githubcheckaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/githubconfiguretarget.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/githubtriggeraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/insertversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/posttags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/postworkspaceevents.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/preflight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/queryeventlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/registerschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/revokeembedaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/searchworkspaceevents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/uploadreport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/upsertapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/upsertapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/validateapikey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:12:54.374686 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/accessdetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/accesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/addtags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/api_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/apiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/apiendpoint_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/apikeydetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/boundedrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    20537 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/clievent.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/embedaccesstokenresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/embedtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/featureflag.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/filter_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/generateopenapispecdiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/getnamespacesresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/getrevisionsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/gettagsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/githubconfiguretargetrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/githubtriggeractionrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/interactiontype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/organizationusage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/organizationusageresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/preflightrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/preflighttoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/report.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/requestmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/revision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/schemadiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     8823 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/targetsdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/unboundedrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/v2descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/versionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/versionmetadata_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    11614 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    28973 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:12:54.374686 speakeasy-client-sdk-python-5.9.2/src/speakeasy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32647 2024-05-21 00:12:46.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:12:54.374686 speakeasy-client-sdk-python-5.9.2/src/speakeasy_client_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23387 2024-05-21 00:12:54.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy_client_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-21 00:12:54.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 00:12:54.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy_client_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-21 00:12:54.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy_client_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 00:12:54.000000 speakeasy-client-sdk-python-5.9.2/src/speakeasy_client_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:18:30.980498 speakeasy-client-sdk-python-5.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    23459 2024-05-23 00:18:30.980498 speakeasy-client-sdk-python-5.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15139 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 00:18:30.980498 speakeasy-client-sdk-python-5.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:18:30.964498 speakeasy-client-sdk-python-5.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:18:30.964498 speakeasy-client-sdk-python-5.9.3/src/speakeasy/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:18:30.964498 speakeasy-client-sdk-python-5.9.3/src/speakeasy/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29402 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/apiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22156 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24848 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14216 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/embeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16846 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10843 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:18:30.964498 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:18:30.968498 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/errors/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:18:30.968498 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:18:30.972498 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/deleteapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/deleteapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/deleteschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/deleteversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/downloadschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/downloadschemarevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/findapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/generateopenapispec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/generatepostmancollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/generaterequestpostmancollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getallapiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getallapiversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getallforversionapiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getapis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getblob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getchangesreportsignedurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getembedaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getlintingreportsignedurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getnamespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getorganizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getorganizationusage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getrequestfromeventlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getrevisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getschemadiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getschemarevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getschemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/gettags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getvalidembedaccesstokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getworkspaceaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getworkspaceeventsbytarget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getworkspacetargets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/githubcheckaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/githubconfiguretarget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/githubtriggeraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/insertversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/posttags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/postworkspaceevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/preflight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/queryeventlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/registerschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/revokeembedaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/searchworkspaceevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/uploadreport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/upsertapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/upsertapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/validateapikey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:18:30.980498 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/accessdetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/accesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/addtags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/api_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/apiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/apiendpoint_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/apikeydetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/boundedrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20537 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/clievent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/embedaccesstokenresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/embedtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/featureflag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/filter_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/generateopenapispecdiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/getnamespacesresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/getrevisionsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/gettagsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/githubconfiguretargetrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/githubtriggeractionrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/interactiontype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/organizationusage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/organizationusageresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/preflightrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/preflighttoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/requestmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/schemadiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8823 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/targetsdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/unboundedrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/v2descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/versionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/versionmetadata_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11614 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28973 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:18:30.980498 speakeasy-client-sdk-python-5.9.3/src/speakeasy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32697 2024-05-23 00:18:21.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:18:30.980498 speakeasy-client-sdk-python-5.9.3/src/speakeasy_client_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23459 2024-05-23 00:18:30.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy_client_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-23 00:18:30.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 00:18:30.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy_client_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-23 00:18:30.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy_client_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 00:18:30.000000 speakeasy-client-sdk-python-5.9.3/src/speakeasy_client_sdk_python.egg-info/top_level.txt
```

### Comparing `speakeasy-client-sdk-python-5.9.2/PKG-INFO` & `speakeasy-client-sdk-python-5.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakeasy-client-sdk-python
-Version: 5.9.2
+Version: 5.9.3
 Summary: Speakeasy API Client SDK for Python
 Home-page: https://github.com/speakeasy-api/speakeasy-client-sdk-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # speakeasy-client-sdk-python
         
         <!-- Start SDK Installation [installation] -->
@@ -26,14 +26,15 @@
         
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
         )
         
+        
         res = s.apis.get_apis(request=operations.GetApisRequest())
         
         if res.apis is not None:
             # handle response
             pass
         
         ```
@@ -162,14 +163,15 @@
         )
         
         res = None
         try:
             res = s.events.get_workspace_events_by_target(request=operations.GetWorkspaceEventsByTargetRequest(
             target_id='<value>',
         ))
+        
         except errors.Error as e:
             # handle exception
             raise(e)
         except errors.SDKError as e:
             # handle exception
             raise(e)
         
@@ -202,14 +204,15 @@
         s = speakeasy.Speakeasy(
             server="prod",
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
         )
         
+        
         res = s.apis.delete_api(request=operations.DeleteAPIRequest(
             api_id='<value>',
             version_id='<value>',
         ))
         
         if res is not None:
             # handle response
@@ -228,14 +231,15 @@
         s = speakeasy.Speakeasy(
             server_url="https://api.prod.speakeasyapi.dev",
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
         )
         
+        
         res = s.apis.delete_api(request=operations.DeleteAPIRequest(
             api_id='<value>',
             version_id='<value>',
         ))
         
         if res is not None:
             # handle response
@@ -283,14 +287,15 @@
         
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
         )
         
+        
         res = s.apis.delete_api(request=operations.DeleteAPIRequest(
             api_id='<value>',
             version_id='<value>',
         ))
         
         if res is not None:
             # handle response
@@ -324,14 +329,15 @@
         
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
         )
         
+        
         res = s.events.get_workspace_events_by_target(request=operations.GetWorkspaceEventsByTargetRequest(
             target_id='<value>',
         ))
         
         if res.cli_event_batch is not None:
             # handle response
             pass
@@ -352,14 +358,15 @@
         
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
         )
         
+        
         res = s.auth.get_workspace_access(request=operations.GetWorkspaceAccessRequest(),
             RetryConfig('backoff', BackoffStrategy(1, 50, 1.1, 100), False))
         
         if res.access_details is not None:
             # handle response
             pass
         
@@ -374,14 +381,15 @@
         s = speakeasy.Speakeasy(
             retry_config=RetryConfig('backoff', BackoffStrategy(1, 50, 1.1, 100), False),
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
         )
         
+        
         res = s.auth.get_workspace_access(request=operations.GetWorkspaceAccessRequest())
         
         if res.access_details is not None:
             # handle response
             pass
         
         ```
```

### Comparing `speakeasy-client-sdk-python-5.9.2/README.md` & `speakeasy-client-sdk-python-5.9.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 s = speakeasy.Speakeasy(
     security=shared.Security(
         api_key="<YOUR_API_KEY_HERE>",
     ),
 )
 
+
 res = s.apis.get_apis(request=operations.GetApisRequest())
 
 if res.apis is not None:
     # handle response
     pass
 
 ```
@@ -155,14 +156,15 @@
 )
 
 res = None
 try:
     res = s.events.get_workspace_events_by_target(request=operations.GetWorkspaceEventsByTargetRequest(
     target_id='<value>',
 ))
+
 except errors.Error as e:
     # handle exception
     raise(e)
 except errors.SDKError as e:
     # handle exception
     raise(e)
 
@@ -195,14 +197,15 @@
 s = speakeasy.Speakeasy(
     server="prod",
     security=shared.Security(
         api_key="<YOUR_API_KEY_HERE>",
     ),
 )
 
+
 res = s.apis.delete_api(request=operations.DeleteAPIRequest(
     api_id='<value>',
     version_id='<value>',
 ))
 
 if res is not None:
     # handle response
@@ -221,14 +224,15 @@
 s = speakeasy.Speakeasy(
     server_url="https://api.prod.speakeasyapi.dev",
     security=shared.Security(
         api_key="<YOUR_API_KEY_HERE>",
     ),
 )
 
+
 res = s.apis.delete_api(request=operations.DeleteAPIRequest(
     api_id='<value>',
     version_id='<value>',
 ))
 
 if res is not None:
     # handle response
@@ -276,14 +280,15 @@
 
 s = speakeasy.Speakeasy(
     security=shared.Security(
         api_key="<YOUR_API_KEY_HERE>",
     ),
 )
 
+
 res = s.apis.delete_api(request=operations.DeleteAPIRequest(
     api_id='<value>',
     version_id='<value>',
 ))
 
 if res is not None:
     # handle response
@@ -317,14 +322,15 @@
 
 s = speakeasy.Speakeasy(
     security=shared.Security(
         api_key="<YOUR_API_KEY_HERE>",
     ),
 )
 
+
 res = s.events.get_workspace_events_by_target(request=operations.GetWorkspaceEventsByTargetRequest(
     target_id='<value>',
 ))
 
 if res.cli_event_batch is not None:
     # handle response
     pass
@@ -345,14 +351,15 @@
 
 s = speakeasy.Speakeasy(
     security=shared.Security(
         api_key="<YOUR_API_KEY_HERE>",
     ),
 )
 
+
 res = s.auth.get_workspace_access(request=operations.GetWorkspaceAccessRequest(),
     RetryConfig('backoff', BackoffStrategy(1, 50, 1.1, 100), False))
 
 if res.access_details is not None:
     # handle response
     pass
 
@@ -367,14 +374,15 @@
 s = speakeasy.Speakeasy(
     retry_config=RetryConfig('backoff', BackoffStrategy(1, 50, 1.1, 100), False),
     security=shared.Security(
         api_key="<YOUR_API_KEY_HERE>",
     ),
 )
 
+
 res = s.auth.get_workspace_access(request=operations.GetWorkspaceAccessRequest())
 
 if res.access_details is not None:
     # handle response
     pass
 
 ```
```

### Comparing `speakeasy-client-sdk-python-5.9.2/setup.py` & `speakeasy-client-sdk-python-5.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='speakeasy-client-sdk-python',
-    version='5.9.2',
+    version='5.9.3',
     author='Speakeasy',
     description='Speakeasy API Client SDK for Python',
     url='https://github.com/speakeasy-api/speakeasy-client-sdk-python.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/_hooks/registration.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/_hooks/sdkhooks.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/_hooks/types.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/apiendpoints.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/apiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/apis.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/apis.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/artifacts.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/artifacts.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/auth.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/auth.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/embeds.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/embeds.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/events.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/events.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/github.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/github.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/metadata.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/metadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/errors/error.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/errors/error.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/errors/sdkerror.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/__init__.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/deleteapi.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/deleteapi.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/deleteapiendpoint.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/deleteapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/deleteschema.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/deleteschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/deleteversionmetadata.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/deleteversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/downloadschema.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/downloadschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/downloadschemarevision.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/downloadschemarevision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/findapiendpoint.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/findapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/generateopenapispec.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/generateopenapispec.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/generatepostmancollection.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/generatepostmancollection.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/generaterequestpostmancollection.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/generaterequestpostmancollection.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getaccesstoken.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getallapiendpoints.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getallapiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getallapiversions.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getallapiversions.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getallforversionapiendpoints.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getallforversionapiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getapiendpoint.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getapis.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getapis.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getblob.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getblob.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getchangesreportsignedurl.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getchangesreportsignedurl.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getembedaccesstoken.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getembedaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getlintingreportsignedurl.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getlintingreportsignedurl.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getmanifest.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getmanifest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getnamespaces.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getnamespaces.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getorganizations.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getorganizations.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getorganizationusage.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getorganizationusage.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getrequestfromeventlog.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getrequestfromeventlog.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getrevisions.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getrevisions.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getschema.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getschemadiff.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getschemadiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getschemarevision.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getschemarevision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getschemas.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getschemas.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/gettags.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/gettags.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getuser.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getuser.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getvalidembedaccesstokens.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getvalidembedaccesstokens.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getversionmetadata.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getworkspaceaccess.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getworkspaceaccess.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getworkspaceeventsbytarget.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getworkspaceeventsbytarget.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/getworkspacetargets.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/getworkspacetargets.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/githubcheckaccess.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/githubcheckaccess.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/githubconfiguretarget.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/githubconfiguretarget.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/githubtriggeraction.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/githubtriggeraction.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/insertversionmetadata.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/insertversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/posttags.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/posttags.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/postworkspaceevents.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/postworkspaceevents.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/preflight.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/preflight.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/queryeventlog.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/queryeventlog.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/registerschema.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/registerschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/revokeembedaccesstoken.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/revokeembedaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/searchworkspaceevents.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/searchworkspaceevents.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/uploadreport.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/uploadreport.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/upsertapi.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/upsertapi.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/upsertapiendpoint.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/upsertapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/operations/validateapikey.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/operations/validateapikey.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/__init__.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/accessdetails.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/accessdetails.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/accesstoken.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/accesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/addtags.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/addtags.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/annotations.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/annotations.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/api.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/api.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/api_input.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/api_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/apiendpoint.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/apiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/apiendpoint_input.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/apiendpoint_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/apikeydetails.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/apikeydetails.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/boundedrequest.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/boundedrequest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/clievent.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/clievent.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/embedaccesstokenresponse.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/embedaccesstokenresponse.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/embedtoken.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/embedtoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/featureflag.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/featureflag.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/filter_.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/filter_.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/filters.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/filters.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/generateopenapispecdiff.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/generateopenapispecdiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/getrevisionsresponse.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/getrevisionsresponse.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/githubconfiguretargetrequest.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/githubconfiguretargetrequest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/githubtriggeractionrequest.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/githubtriggeractionrequest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/manifest.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/manifest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/namespace.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/namespace.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/organization.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/organization.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/organizationusage.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/organizationusage.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/organizationusageresponse.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/organizationusageresponse.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/preflighttoken.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/preflighttoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/report.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/report.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/requestmetadata.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/requestmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/revision.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/revision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/schema.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/schema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/schemadiff.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/schemadiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/security.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/security.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/tag.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/tag.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/targetsdk.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/targetsdk.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/unboundedrequest.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/unboundedrequest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/user.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/user.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/v2descriptor.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/v2descriptor.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/versionmetadata.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/versionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/models/shared/versionmetadata_input.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/models/shared/versionmetadata_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/organizations.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/organizations.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/reports.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/reports.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/requests.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/requests.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/schemas.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/schemas.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/sdk.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/sdk.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/sdkconfiguration.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/sdkconfiguration.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     client: requests_http.Session
     globals: internal.Globals
     security: Union[shared.Security,Callable[[], shared.Security]] = None
     server_url: Optional[str] = ''
     server: Optional[str] = ''
     language: str = 'python'
     openapi_doc_version: str = '0.4.0 .'
-    sdk_version: str = '5.9.2'
-    gen_version: str = '2.333.3'
-    user_agent: str = 'speakeasy-sdk/python 5.9.2 2.333.3 0.4.0 . speakeasy-client-sdk-python'
+    sdk_version: str = '5.9.3'
+    gen_version: str = '2.335.5'
+    user_agent: str = 'speakeasy-sdk/python 5.9.3 2.335.5 0.4.0 . speakeasy-client-sdk-python'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/utils/retries.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/utils/retries.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy/utils/utils.py` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -814,19 +814,19 @@
             return ",".join(items)
     else:
         return f"{_val_to_string(obj)}"
 
     return ""
 
 
-def unmarshal_json(data, typ, decoder=None):
+def unmarshal_json(data, typ, decoder=None, infer_missing=False):
     unmarshal = make_dataclass("Unmarshal", [("res", typ)], bases=(DataClassJsonMixin,))
     json_dict = json.loads(data)
     try:
-        out = unmarshal.from_dict({"res": json_dict})
+        out = unmarshal.from_dict({"res": json_dict}, infer_missing=infer_missing)
     except AttributeError as attr_err:
         raise AttributeError(
             f"unable to unmarshal {data} as {typ} - {attr_err}"
         ) from attr_err
 
     return out.res if decoder is None else decoder(out.res)
```

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy_client_sdk_python.egg-info/PKG-INFO` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy_client_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakeasy-client-sdk-python
-Version: 5.9.2
+Version: 5.9.3
 Summary: Speakeasy API Client SDK for Python
 Home-page: https://github.com/speakeasy-api/speakeasy-client-sdk-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # speakeasy-client-sdk-python
         
         <!-- Start SDK Installation [installation] -->
@@ -26,14 +26,15 @@
         
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
         )
         
+        
         res = s.apis.get_apis(request=operations.GetApisRequest())
         
         if res.apis is not None:
             # handle response
             pass
         
         ```
@@ -162,14 +163,15 @@
         )
         
         res = None
         try:
             res = s.events.get_workspace_events_by_target(request=operations.GetWorkspaceEventsByTargetRequest(
             target_id='<value>',
         ))
+        
         except errors.Error as e:
             # handle exception
             raise(e)
         except errors.SDKError as e:
             # handle exception
             raise(e)
         
@@ -202,14 +204,15 @@
         s = speakeasy.Speakeasy(
             server="prod",
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
         )
         
+        
         res = s.apis.delete_api(request=operations.DeleteAPIRequest(
             api_id='<value>',
             version_id='<value>',
         ))
         
         if res is not None:
             # handle response
@@ -228,14 +231,15 @@
         s = speakeasy.Speakeasy(
             server_url="https://api.prod.speakeasyapi.dev",
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
         )
         
+        
         res = s.apis.delete_api(request=operations.DeleteAPIRequest(
             api_id='<value>',
             version_id='<value>',
         ))
         
         if res is not None:
             # handle response
@@ -283,14 +287,15 @@
         
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
         )
         
+        
         res = s.apis.delete_api(request=operations.DeleteAPIRequest(
             api_id='<value>',
             version_id='<value>',
         ))
         
         if res is not None:
             # handle response
@@ -324,14 +329,15 @@
         
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
         )
         
+        
         res = s.events.get_workspace_events_by_target(request=operations.GetWorkspaceEventsByTargetRequest(
             target_id='<value>',
         ))
         
         if res.cli_event_batch is not None:
             # handle response
             pass
@@ -352,14 +358,15 @@
         
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
         )
         
+        
         res = s.auth.get_workspace_access(request=operations.GetWorkspaceAccessRequest(),
             RetryConfig('backoff', BackoffStrategy(1, 50, 1.1, 100), False))
         
         if res.access_details is not None:
             # handle response
             pass
         
@@ -374,14 +381,15 @@
         s = speakeasy.Speakeasy(
             retry_config=RetryConfig('backoff', BackoffStrategy(1, 50, 1.1, 100), False),
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
         )
         
+        
         res = s.auth.get_workspace_access(request=operations.GetWorkspaceAccessRequest())
         
         if res.access_details is not None:
             # handle response
             pass
         
         ```
```

### Comparing `speakeasy-client-sdk-python-5.9.2/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt` & `speakeasy-client-sdk-python-5.9.3/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*


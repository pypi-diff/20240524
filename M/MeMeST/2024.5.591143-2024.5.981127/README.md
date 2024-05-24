# Comparing `tmp/MeMeST-2024.5.591143-py3-none-any.whl.zip` & `tmp/MeMeST-2024.5.981127-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 34048 bytes, number of entries: 16
--rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-10 04:45 MeMeST-2024.5.591143.data/data/LICENSE
+Zip file size: 34053 bytes, number of entries: 16
+-rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-10 04:45 MeMeST-2024.5.981127.data/data/LICENSE
 -rw-rw-r--  2.0 unx       76 b- defN 24-Apr-10 04:45 git_tools/__init__.py
 -rw-rw-r--  2.0 unx     1139 b- defN 24-Apr-18 09:30 git_tools/base_dtypes.py
--rw-rw-r--  2.0 unx     9287 b- defN 24-May-05 13:38 git_tools/git_api.py
+-rw-rw-r--  2.0 unx     9299 b- defN 24-May-24 14:54 git_tools/git_api.py
 -rw-rw-r--  2.0 unx      143 b- defN 24-Apr-10 04:45 git_tools/rep_task.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-Apr-10 04:45 mest/__init__.py
 -rw-rw-r--  2.0 unx     4518 b- defN 24-Apr-29 10:15 mest/config.py
 -rw-rw-r--  2.0 unx     4135 b- defN 24-May-08 09:06 mest/main.py
 -rw-rw-r--  2.0 unx     2717 b- defN 24-Apr-29 13:50 mest/rep_mana.py
 -rw-rw-r--  2.0 unx      569 b- defN 24-Apr-10 04:45 mest/test_git.py
--rwxrwxr-x  2.0 unx    35149 b- defN 24-May-08 09:07 MeMeST-2024.5.591143.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1797 b- defN 24-May-08 09:07 MeMeST-2024.5.591143.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-08 09:07 MeMeST-2024.5.591143.dist-info/WHEEL
--rw-rw-r--  2.0 unx       42 b- defN 24-May-08 09:07 MeMeST-2024.5.591143.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       15 b- defN 24-May-08 09:07 MeMeST-2024.5.591143.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1286 b- defN 24-May-08 09:07 MeMeST-2024.5.591143.dist-info/RECORD
-16 files, 96114 bytes uncompressed, 31932 bytes compressed:  66.8%
+-rwxrwxr-x  2.0 unx    35149 b- defN 24-May-24 14:55 MeMeST-2024.5.981127.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1797 b- defN 24-May-24 14:55 MeMeST-2024.5.981127.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-24 14:55 MeMeST-2024.5.981127.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       42 b- defN 24-May-24 14:55 MeMeST-2024.5.981127.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       15 b- defN 24-May-24 14:55 MeMeST-2024.5.981127.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1286 b- defN 24-May-24 14:55 MeMeST-2024.5.981127.dist-info/RECORD
+16 files, 96126 bytes uncompressed, 31937 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -1,8 +1,8 @@
-Filename: MeMeST-2024.5.591143.data/data/LICENSE
+Filename: MeMeST-2024.5.981127.data/data/LICENSE
 Comment: 
 
 Filename: git_tools/__init__.py
 Comment: 
 
 Filename: git_tools/base_dtypes.py
 Comment: 
@@ -24,26 +24,26 @@
 
 Filename: mest/rep_mana.py
 Comment: 
 
 Filename: mest/test_git.py
 Comment: 
 
-Filename: MeMeST-2024.5.591143.dist-info/LICENSE
+Filename: MeMeST-2024.5.981127.dist-info/LICENSE
 Comment: 
 
-Filename: MeMeST-2024.5.591143.dist-info/METADATA
+Filename: MeMeST-2024.5.981127.dist-info/METADATA
 Comment: 
 
-Filename: MeMeST-2024.5.591143.dist-info/WHEEL
+Filename: MeMeST-2024.5.981127.dist-info/WHEEL
 Comment: 
 
-Filename: MeMeST-2024.5.591143.dist-info/entry_points.txt
+Filename: MeMeST-2024.5.981127.dist-info/entry_points.txt
 Comment: 
 
-Filename: MeMeST-2024.5.591143.dist-info/top_level.txt
+Filename: MeMeST-2024.5.981127.dist-info/top_level.txt
 Comment: 
 
-Filename: MeMeST-2024.5.591143.dist-info/RECORD
+Filename: MeMeST-2024.5.981127.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## git_tools/git_api.py

```diff
@@ -163,15 +163,15 @@
 def push(rep_data: RepData):
     if not good_rep_data(rep_data):
         return
     local_branch_list = get_local_branch_list(rep_data.work_dir)
     logger.info("push to {}", rep_data.address)
     work_dir = rep_data.work_dir
     for branch in local_branch_list:
-        checkout_command = ["git", "checkout", branch]
+        checkout_command = ["git", "checkout", branch, "--"]
         logger.info("run {}", checkout_command)
         result = subprocess.run(
             checkout_command,
             cwd=work_dir,
             stdout=subprocess.DEVNULL,
             stderr=subprocess.PIPE,
             check=False,
@@ -229,15 +229,15 @@
 def merge_remote_branches(rep_data):
     if not good_rep_data(rep_data):
         return
     work_dir = rep_data.work_dir
     branch_list = rep_data.branch_list
     alias = rep_data.alias
     for branch in branch_list:
-        checkout_command = ["git", "checkout", branch]
+        checkout_command = ["git", "checkout", branch, "--"]
         subprocess.run(
             checkout_command,
             cwd=work_dir,
             env=ENV,
             stdout=subprocess.DEVNULL,
             stderr=subprocess.PIPE,
             check=False,
```

## Comparing `MeMeST-2024.5.591143.data/data/LICENSE` & `MeMeST-2024.5.981127.data/data/LICENSE`

 * *Files identical despite different names*

## Comparing `MeMeST-2024.5.591143.dist-info/LICENSE` & `MeMeST-2024.5.981127.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `MeMeST-2024.5.591143.dist-info/METADATA` & `MeMeST-2024.5.981127.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeMeST
-Version: 2024.5.591143
+Version: 2024.5.981127
 Summary: Multi-Repository Sync Tool
 Author: Xin-Xin Ma
 License: GPL
 Project-URL: Source, https://github.com/xxmawhu/memest.git
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: termcolor
```

## Comparing `MeMeST-2024.5.591143.dist-info/RECORD` & `MeMeST-2024.5.981127.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-MeMeST-2024.5.591143.data/data/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+MeMeST-2024.5.981127.data/data/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
 git_tools/__init__.py,sha256=-M_wTgmk-Pe-gzayRUsldMI8maSAQpgrCrKbiUQFV2o,76
 git_tools/base_dtypes.py,sha256=Y7F6fUoZvETZVV4EKpPnrfS3Qfeudb-Oojh-B93mSPQ,1139
-git_tools/git_api.py,sha256=D9w3gaNY04_Nf7KBBiFgjsVlxRO2SEbTnjSAkjZBUq4,9287
+git_tools/git_api.py,sha256=p1mwQ5XZYWVXflKBD3DW_zwD8NXjbA2t12V3qbImhqo,9299
 git_tools/rep_task.py,sha256=vFPW1Z8mTIF0ZGJgaGF8AZM91A4Ogf_Sdo-bKtdo8-c,143
 mest/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mest/config.py,sha256=YS4NJNE1fIAz0K3l7SreoqdtpM3nAJCe_oJc4LwREo0,4518
 mest/main.py,sha256=WLrMP2GO4yyCJB0OutmquQA1_A2IrP5xZ1k07JnleBk,4135
 mest/rep_mana.py,sha256=ZEhbeopuFBYIr4Eg64GUEQQ7M9bZZn0IFhmf3HJ2Mso,2717
 mest/test_git.py,sha256=BgD4moVzqnxfnhZzoM-EgHklAVFYPbtYu5Ke6qqFHhI,569
-MeMeST-2024.5.591143.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-MeMeST-2024.5.591143.dist-info/METADATA,sha256=OhTih6yjIkqxmfJmONZutZwN-CAylW7lkkCtOY95Elo,1797
-MeMeST-2024.5.591143.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-MeMeST-2024.5.591143.dist-info/entry_points.txt,sha256=OYg2gMfzGJOXcQc_TTGdfCSPRPqlQylNW3LSReX_ta8,42
-MeMeST-2024.5.591143.dist-info/top_level.txt,sha256=iFxJRSyvq4K2f9Wl2wqP84mPUD7Ta4IoyDy9bDHkiYE,15
-MeMeST-2024.5.591143.dist-info/RECORD,,
+MeMeST-2024.5.981127.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+MeMeST-2024.5.981127.dist-info/METADATA,sha256=evkYWihIKX2a7FZ1KQD1o1w1myBSR94hKNnkLlvdpO0,1797
+MeMeST-2024.5.981127.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+MeMeST-2024.5.981127.dist-info/entry_points.txt,sha256=OYg2gMfzGJOXcQc_TTGdfCSPRPqlQylNW3LSReX_ta8,42
+MeMeST-2024.5.981127.dist-info/top_level.txt,sha256=iFxJRSyvq4K2f9Wl2wqP84mPUD7Ta4IoyDy9bDHkiYE,15
+MeMeST-2024.5.981127.dist-info/RECORD,,
```


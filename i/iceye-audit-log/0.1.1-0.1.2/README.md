# Comparing `tmp/iceye_audit_log-0.1.1.tar.gz` & `tmp/iceye_audit_log-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iceye_audit_log-0.1.1.tar", last modified: Wed May 22 06:15:44 2024, max compression
+gzip compressed data, was "iceye_audit_log-0.1.2.tar", last modified: Fri May 24 10:58:42 2024, max compression
```

## Comparing `iceye_audit_log-0.1.1.tar` & `iceye_audit_log-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:15:44.782797 iceye_audit_log-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:15:44.782797 iceye_audit_log-0.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:15:44.782797 iceye_audit_log-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-22 06:15:44.782797 iceye_audit_log-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:15:44.782797 iceye_audit_log-0.1.1/audit_log/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/audit_log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/audit_log/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/audit_log/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/audit_log/log.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/audit_log/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/audit_log/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:15:44.782797 iceye_audit_log-0.1.1/iceye_audit_log.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-22 06:15:44.000000 iceye_audit_log-0.1.1/iceye_audit_log.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-22 06:15:44.000000 iceye_audit_log-0.1.1/iceye_audit_log.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 06:15:44.000000 iceye_audit_log-0.1.1/iceye_audit_log.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 06:15:44.000000 iceye_audit_log-0.1.1/iceye_audit_log.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 06:15:44.782797 iceye_audit_log-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:15:44.782797 iceye_audit_log-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/tests/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-22 06:15:33.000000 iceye_audit_log-0.1.1/tests/test_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:58:42.704715 iceye_audit_log-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:58:42.700715 iceye_audit_log-0.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-24 10:58:31.000000 iceye_audit_log-0.1.2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-24 10:58:31.000000 iceye_audit_log-0.1.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:58:42.700715 iceye_audit_log-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-24 10:58:31.000000 iceye_audit_log-0.1.2/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-24 10:58:31.000000 iceye_audit_log-0.1.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-24 10:58:31.000000 iceye_audit_log-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-24 10:58:31.000000 iceye_audit_log-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-24 10:58:31.000000 iceye_audit_log-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-24 10:58:31.000000 iceye_audit_log-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-24 10:58:31.000000 iceye_audit_log-0.1.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-24 10:58:42.704715 iceye_audit_log-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-24 10:58:31.000000 iceye_audit_log-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-24 10:58:31.000000 iceye_audit_log-0.1.2/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:58:42.704715 iceye_audit_log-0.1.2/audit_log/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 10:58:31.000000 iceye_audit_log-0.1.2/audit_log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-24 10:58:31.000000 iceye_audit_log-0.1.2/audit_log/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-24 10:58:31.000000 iceye_audit_log-0.1.2/audit_log/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-24 10:58:31.000000 iceye_audit_log-0.1.2/audit_log/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 10:58:31.000000 iceye_audit_log-0.1.2/audit_log/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-24 10:58:31.000000 iceye_audit_log-0.1.2/audit_log/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:58:42.704715 iceye_audit_log-0.1.2/iceye_audit_log.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-24 10:58:42.000000 iceye_audit_log-0.1.2/iceye_audit_log.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-24 10:58:42.000000 iceye_audit_log-0.1.2/iceye_audit_log.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 10:58:42.000000 iceye_audit_log-0.1.2/iceye_audit_log.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 10:58:42.000000 iceye_audit_log-0.1.2/iceye_audit_log.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-24 10:58:31.000000 iceye_audit_log-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-24 10:58:31.000000 iceye_audit_log-0.1.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 10:58:42.704715 iceye_audit_log-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:58:42.704715 iceye_audit_log-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-24 10:58:31.000000 iceye_audit_log-0.1.2/tests/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-24 10:58:31.000000 iceye_audit_log-0.1.2/tests/test_log.py
```

### Comparing `iceye_audit_log-0.1.1/.github/workflows/release.yml` & `iceye_audit_log-0.1.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `iceye_audit_log-0.1.1/.github/workflows/test.yml` & `iceye_audit_log-0.1.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `iceye_audit_log-0.1.1/.gitignore` & `iceye_audit_log-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `iceye_audit_log-0.1.1/.pre-commit-config.yaml` & `iceye_audit_log-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `iceye_audit_log-0.1.1/LICENSE` & `iceye_audit_log-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iceye_audit_log-0.1.1/PKG-INFO` & `iceye_audit_log-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceye-audit-log
-Version: 0.1.1
+Version: 0.1.2
 Summary: Audit logging library for Python
 License: MIT License
         
         Copyright (c) 2024 Iceye Oy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `iceye_audit_log-0.1.1/SECURITY.md` & `iceye_audit_log-0.1.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `iceye_audit_log-0.1.1/audit_log/headers.py` & `iceye_audit_log-0.1.2/audit_log/headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,9 +93,9 @@
 
     try:
         spiffe = parse_spiffe(headers[MTLS_CERT_HEADER])
     except Exception as e:
         raise AuditPrincipalError("Invalid SPIFFE header") from e
     else:
         return Principal(
-            type=PrincipalType.SERVICE, authority=spiffe.domain, id=spiffe.spiffe_id
+            type=PrincipalType.SYSTEM, authority=spiffe.domain, id=spiffe.spiffe_id
         )
```

### Comparing `iceye_audit_log-0.1.1/audit_log/log.py` & `iceye_audit_log-0.1.2/audit_log/log.py`

 * *Files identical despite different names*

### Comparing `iceye_audit_log-0.1.1/iceye_audit_log.egg-info/PKG-INFO` & `iceye_audit_log-0.1.2/iceye_audit_log.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceye-audit-log
-Version: 0.1.1
+Version: 0.1.2
 Summary: Audit logging library for Python
 License: MIT License
         
         Copyright (c) 2024 Iceye Oy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `iceye_audit_log-0.1.1/iceye_audit_log.egg-info/SOURCES.txt` & `iceye_audit_log-0.1.2/iceye_audit_log.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iceye_audit_log-0.1.1/pyproject.toml` & `iceye_audit_log-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iceye_audit_log-0.1.1/tests/test_headers.py` & `iceye_audit_log-0.1.2/tests/test_headers.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     with pytest.raises(ValueError, match="Invalid SPIFFE header"):
         parse_spiffe(VALID_SPIFFE_HEADER_INVALID_PATH)
 
 
 def test_get_principal_from_headers_valid():
     principal = get_principal_from_headers(VALID_HEADERS)
     assert isinstance(principal, Principal)
-    assert principal.type == PrincipalType.SERVICE
+    assert principal.type == PrincipalType.SYSTEM
     assert principal.authority == "example.com"
     assert principal.id == "spiffe://example.com/ns/namespace/sa/service-account"
 
 
 def test_get_principal_from_headers_invalid():
     with pytest.raises(AuditPrincipalError, match="Invalid SPIFFE header"):
         get_principal_from_headers(INVALID_HEADERS)
@@ -94,10 +94,10 @@
 
 def test_parse_principal_spiffe_insensitive():
     headers = {
         "X-fOrWaRdEd-ClIeNt-CeRt": VALID_SPIFFE_HEADER,
     }
     principal = get_principal_from_headers(headers)
     assert isinstance(principal, Principal)
-    assert principal.type == PrincipalType.SERVICE
+    assert principal.type == PrincipalType.SYSTEM
     assert principal.authority == "example.com"
     assert principal.id == "spiffe://example.com/ns/namespace/sa/service-account"
```

### Comparing `iceye_audit_log-0.1.1/tests/test_log.py` & `iceye_audit_log-0.1.2/tests/test_log.py`

 * *Files identical despite different names*


# Comparing `tmp/cert-schema-3.6.3.tar.gz` & `tmp/cert-schema-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cert-schema-3.6.3.tar", last modified: Tue Mar 19 17:33:25 2024, max compression
+gzip compressed data, was "cert-schema-3.6.4.tar", last modified: Fri May 24 08:00:20 2024, max compression
```

## Comparing `cert-schema-3.6.3.tar` & `cert-schema-3.6.4.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-19 17:33:25.006569 cert-schema-3.6.3/
--rw-rw-r--   0 travis    (2000) travis    (2000)    31107 2024-03-19 17:32:38.000000 cert-schema-3.6.3/CHANGELOG.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1096 2024-03-19 17:32:38.000000 cert-schema-3.6.3/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       47 2024-03-19 17:32:38.000000 cert-schema-3.6.3/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     3531 2024-03-19 17:33:25.006569 cert-schema-3.6.3/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3283 2024-03-19 17:32:38.000000 cert-schema-3.6.3/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-19 17:33:24.978567 cert-schema-3.6.3/cert_schema/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-19 17:33:24.982567 cert-schema-3.6.3/cert_schema/1.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8207 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/1.1/certificate-schema-v1-1.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1558 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/1.1/issuer-schema-v1-1.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-19 17:33:24.986568 cert-schema-3.6.3/cert_schema/1.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4174 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/1.2/assertion-1.2.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2406 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/1.2/blockchain-certificate-1.2.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2912 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/1.2/blockchain-receipt-1.2.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3607 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/1.2/certificate-1.2.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     5557 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/1.2/certificate-document-1.2.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     5343 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/1.2/context.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3321 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/1.2/issuer-1.2.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3240 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/1.2/issuer-id-1.2.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-19 17:33:24.986568 cert-schema-3.6.3/cert_schema/2.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1888 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/2.0/context.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     6472 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/2.0/issuerSchema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1521 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/2.0/merkleProof2017Schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     4494 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/2.0/obi.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1085 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/2.0/recipientSchema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    11948 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/2.0/schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1237 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/2.0/signatureLineSchema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-19 17:33:24.990568 cert-schema-3.6.3/cert_schema/2.0-alpha/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1951 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/2.0-alpha/context.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7035 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/2.0-alpha/issuerSchema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1430 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/2.0-alpha/merkleProof2017Schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1085 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/2.0-alpha/recipientSchema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    14584 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/2.0-alpha/schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1237 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/2.0-alpha/signatureLineSchema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-19 17:33:24.990568 cert-schema-3.6.3/cert_schema/2.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1888 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/2.1/context.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     6472 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/2.1/issuerSchema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1521 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/2.1/merkleProof2017Schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     4494 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/2.1/obi.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1085 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/2.1/recipientSchema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    11948 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/2.1/schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1237 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/2.1/signatureLineSchema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-19 17:33:24.994568 cert-schema-3.6.3/cert_schema/3.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)      703 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0/claimSchema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1800 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0/context.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7308 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0/credential.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1499 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0/credentialSubjectSchema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      796 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0/displaySchema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      929 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0/merkleProof2019Context.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2823 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0/merkleProof2019Schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     5078 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0/schema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-19 17:33:24.994568 cert-schema-3.6.3/cert_schema/3.0-alpha/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1142 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0-alpha/context.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7308 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0-alpha/credential.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1767 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0-alpha/exampleCredential.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7477 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0-alpha/issuerSchema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      934 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0-alpha/merkleProof2019Context.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2829 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0-alpha/merkleProof2019Schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3883 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0-alpha/schema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-19 17:33:24.998568 cert-schema-3.6.3/cert_schema/3.0-beta/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1810 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0-beta/context.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7308 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0-beta/credential.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      755 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0-beta/displaySchema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1767 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0-beta/exampleCredential.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      934 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0-beta/merkleProof2019Context.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2829 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0-beta/merkleProof2019Schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     4432 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.0-beta/schema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-19 17:33:25.002569 cert-schema-3.6.3/cert_schema/3.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2575 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.1/chainedProof2021Context.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      703 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.1/claimSchema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1753 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.1/context.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7308 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.1/credential.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1499 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.1/credentialSubjectSchema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      796 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.1/displaySchema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2321 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.1/merkleProof2019Context.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2823 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.1/merkleProof2019Schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     5078 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.1/schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1274 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.1/statusList2021Context.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-19 17:33:25.002569 cert-schema-3.6.3/cert_schema/3.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)      703 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.2/claimSchema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1753 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.2/context.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1499 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.2/credentialSubjectSchema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     9750 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.2/credential_v2.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2609 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.2/dataIntegrityProof.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      796 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.2/displaySchema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     5078 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.2/schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1274 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/3.2/statusList2021Context.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      814 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2024-03-19 17:33:24.000000 cert-schema-3.6.3/cert_schema/__version__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1597 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/context_urls.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2863 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/context_urls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       97 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11660 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/jsonld_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4263 2024-03-19 17:32:38.000000 cert-schema-3.6.3/cert_schema/schema_validator.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-19 17:33:24.982567 cert-schema-3.6.3/cert_schema.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3531 2024-03-19 17:33:24.000000 cert-schema-3.6.3/cert_schema.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3208 2024-03-19 17:33:24.000000 cert-schema-3.6.3/cert_schema.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-03-19 17:33:24.000000 cert-schema-3.6.3/cert_schema.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       60 2024-03-19 17:33:24.000000 cert-schema-3.6.3/cert_schema.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2024-03-19 17:33:24.000000 cert-schema-3.6.3/cert_schema.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1533 2024-03-19 17:32:38.000000 cert-schema-3.6.3/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)       60 2024-03-19 17:32:38.000000 cert-schema-3.6.3/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      137 2024-03-19 17:33:25.006569 cert-schema-3.6.3/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1531 2024-03-19 17:32:38.000000 cert-schema-3.6.3/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-19 17:33:25.006569 cert-schema-3.6.3/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-03-19 17:32:38.000000 cert-schema-3.6.3/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4839 2024-03-19 17:32:38.000000 cert-schema-3.6.3/tests/test_context_urls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2973 2024-03-19 17:32:38.000000 cert-schema-3.6.3/tests/test_jsonld_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3218 2024-03-19 17:32:38.000000 cert-schema-3.6.3/tests/test_schema_validator.py
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2024-05-24 08:00:20.735876 cert-schema-3.6.4/
+-rw-r--r--   0 julien     (503) staff       (20)    30581 2024-05-21 13:53:07.000000 cert-schema-3.6.4/CHANGELOG.md
+-rw-r--r--   0 julien     (503) staff       (20)     1096 2021-04-08 16:27:50.000000 cert-schema-3.6.4/LICENSE
+-rw-r--r--   0 julien     (503) staff       (20)       47 2021-04-08 16:27:50.000000 cert-schema-3.6.4/MANIFEST.in
+-rw-r--r--   0 julien     (503) staff       (20)     4156 2024-05-24 08:00:20.736231 cert-schema-3.6.4/PKG-INFO
+-rw-r--r--   0 julien     (503) staff       (20)     3283 2021-04-08 16:27:50.000000 cert-schema-3.6.4/README.md
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2024-05-24 08:00:20.621056 cert-schema-3.6.4/cert_schema/
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2024-05-24 08:00:20.628997 cert-schema-3.6.4/cert_schema/1.1/
+-rw-r--r--   0 julien     (503) staff       (20)     8207 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/1.1/certificate-schema-v1-1.json
+-rw-r--r--   0 julien     (503) staff       (20)     1558 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/1.1/issuer-schema-v1-1.json
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2024-05-24 08:00:20.637689 cert-schema-3.6.4/cert_schema/1.2/
+-rw-r--r--   0 julien     (503) staff       (20)     4174 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/1.2/assertion-1.2.json
+-rw-r--r--   0 julien     (503) staff       (20)     2406 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/1.2/blockchain-certificate-1.2.json
+-rw-r--r--   0 julien     (503) staff       (20)     2912 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/1.2/blockchain-receipt-1.2.json
+-rw-r--r--   0 julien     (503) staff       (20)     3607 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/1.2/certificate-1.2.json
+-rw-r--r--   0 julien     (503) staff       (20)     5557 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/1.2/certificate-document-1.2.json
+-rw-r--r--   0 julien     (503) staff       (20)     5343 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/1.2/context.json
+-rw-r--r--   0 julien     (503) staff       (20)     3321 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/1.2/issuer-1.2.json
+-rw-r--r--   0 julien     (503) staff       (20)     3240 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/1.2/issuer-id-1.2.json
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2024-05-24 08:00:20.647982 cert-schema-3.6.4/cert_schema/2.0/
+-rw-r--r--   0 julien     (503) staff       (20)     1888 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/2.0/context.json
+-rw-r--r--   0 julien     (503) staff       (20)     6472 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/2.0/issuerSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1521 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/2.0/merkleProof2017Schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     4494 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/2.0/obi.json
+-rw-r--r--   0 julien     (503) staff       (20)     1085 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/2.0/recipientSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)    11948 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/2.0/schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1237 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/2.0/signatureLineSchema.json
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2024-05-24 08:00:20.657442 cert-schema-3.6.4/cert_schema/2.0-alpha/
+-rw-r--r--   0 julien     (503) staff       (20)     1951 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/2.0-alpha/context.json
+-rw-r--r--   0 julien     (503) staff       (20)     7035 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/2.0-alpha/issuerSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1430 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/2.0-alpha/merkleProof2017Schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1085 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/2.0-alpha/recipientSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)    14584 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/2.0-alpha/schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1237 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/2.0-alpha/signatureLineSchema.json
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2024-05-24 08:00:20.666274 cert-schema-3.6.4/cert_schema/2.1/
+-rw-r--r--   0 julien     (503) staff       (20)     1888 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/2.1/context.json
+-rw-r--r--   0 julien     (503) staff       (20)     6472 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/2.1/issuerSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1521 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/2.1/merkleProof2017Schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     4494 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/2.1/obi.json
+-rw-r--r--   0 julien     (503) staff       (20)     1085 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/2.1/recipientSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)    11948 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/2.1/schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1237 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/2.1/signatureLineSchema.json
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2024-05-24 08:00:20.678612 cert-schema-3.6.4/cert_schema/3.0/
+-rw-r--r--   0 julien     (503) staff       (20)      703 2021-12-03 14:49:12.000000 cert-schema-3.6.4/cert_schema/3.0/claimSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1800 2022-06-16 15:34:06.000000 cert-schema-3.6.4/cert_schema/3.0/context.json
+-rw-r--r--   0 julien     (503) staff       (20)     7308 2021-10-05 15:30:06.000000 cert-schema-3.6.4/cert_schema/3.0/credential.json
+-rw-r--r--   0 julien     (503) staff       (20)     1499 2022-03-08 17:50:38.000000 cert-schema-3.6.4/cert_schema/3.0/credentialSubjectSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)      796 2021-12-03 13:09:37.000000 cert-schema-3.6.4/cert_schema/3.0/displaySchema.json
+-rw-r--r--   0 julien     (503) staff       (20)      929 2022-06-16 15:34:40.000000 cert-schema-3.6.4/cert_schema/3.0/merkleProof2019Context.json
+-rw-r--r--   0 julien     (503) staff       (20)     2823 2021-12-03 14:53:56.000000 cert-schema-3.6.4/cert_schema/3.0/merkleProof2019Schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     5078 2021-12-08 14:45:05.000000 cert-schema-3.6.4/cert_schema/3.0/schema.json
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2024-05-24 08:00:20.696496 cert-schema-3.6.4/cert_schema/3.0-alpha/
+-rw-r--r--   0 julien     (503) staff       (20)     1142 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/3.0-alpha/context.json
+-rw-r--r--   0 julien     (503) staff       (20)     7308 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/3.0-alpha/credential.json
+-rw-r--r--   0 julien     (503) staff       (20)     1767 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/3.0-alpha/exampleCredential.json
+-rw-r--r--   0 julien     (503) staff       (20)     7477 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/3.0-alpha/issuerSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)      934 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/3.0-alpha/merkleProof2019Context.json
+-rw-r--r--   0 julien     (503) staff       (20)     2829 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/3.0-alpha/merkleProof2019Schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     3883 2021-10-05 15:30:06.000000 cert-schema-3.6.4/cert_schema/3.0-alpha/schema.json
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2024-05-24 08:00:20.707543 cert-schema-3.6.4/cert_schema/3.0-beta/
+-rw-r--r--   0 julien     (503) staff       (20)     1810 2021-10-05 15:30:06.000000 cert-schema-3.6.4/cert_schema/3.0-beta/context.json
+-rw-r--r--   0 julien     (503) staff       (20)     7308 2021-10-05 15:30:06.000000 cert-schema-3.6.4/cert_schema/3.0-beta/credential.json
+-rw-r--r--   0 julien     (503) staff       (20)      755 2021-10-05 15:30:06.000000 cert-schema-3.6.4/cert_schema/3.0-beta/displaySchema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1767 2021-10-05 15:30:06.000000 cert-schema-3.6.4/cert_schema/3.0-beta/exampleCredential.json
+-rw-r--r--   0 julien     (503) staff       (20)      934 2021-10-05 15:30:06.000000 cert-schema-3.6.4/cert_schema/3.0-beta/merkleProof2019Context.json
+-rw-r--r--   0 julien     (503) staff       (20)     2829 2021-10-05 15:30:06.000000 cert-schema-3.6.4/cert_schema/3.0-beta/merkleProof2019Schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     4432 2021-12-08 14:45:05.000000 cert-schema-3.6.4/cert_schema/3.0-beta/schema.json
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2024-05-24 08:00:20.719778 cert-schema-3.6.4/cert_schema/3.1/
+-rw-r--r--   0 julien     (503) staff       (20)     2575 2022-06-20 17:53:03.000000 cert-schema-3.6.4/cert_schema/3.1/chainedProof2021Context.json
+-rw-r--r--   0 julien     (503) staff       (20)      703 2021-12-03 14:49:12.000000 cert-schema-3.6.4/cert_schema/3.1/claimSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1753 2022-05-10 14:38:30.000000 cert-schema-3.6.4/cert_schema/3.1/context.json
+-rw-r--r--   0 julien     (503) staff       (20)     7308 2021-10-05 15:30:06.000000 cert-schema-3.6.4/cert_schema/3.1/credential.json
+-rw-r--r--   0 julien     (503) staff       (20)     1499 2022-03-08 17:50:38.000000 cert-schema-3.6.4/cert_schema/3.1/credentialSubjectSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)      796 2021-12-03 13:09:37.000000 cert-schema-3.6.4/cert_schema/3.1/displaySchema.json
+-rw-r--r--   0 julien     (503) staff       (20)     2321 2022-06-20 17:53:03.000000 cert-schema-3.6.4/cert_schema/3.1/merkleProof2019Context.json
+-rw-r--r--   0 julien     (503) staff       (20)     2823 2021-12-03 14:53:56.000000 cert-schema-3.6.4/cert_schema/3.1/merkleProof2019Schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     5078 2021-12-08 14:45:05.000000 cert-schema-3.6.4/cert_schema/3.1/schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1274 2023-03-30 13:05:28.000000 cert-schema-3.6.4/cert_schema/3.1/statusList2021Context.json
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2024-05-24 08:00:20.731248 cert-schema-3.6.4/cert_schema/3.2/
+-rw-r--r--   0 julien     (503) staff       (20)      703 2024-03-07 14:45:55.000000 cert-schema-3.6.4/cert_schema/3.2/claimSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1753 2024-03-07 14:45:55.000000 cert-schema-3.6.4/cert_schema/3.2/context.json
+-rw-r--r--   0 julien     (503) staff       (20)     1499 2024-03-07 14:45:55.000000 cert-schema-3.6.4/cert_schema/3.2/credentialSubjectSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)     9923 2024-05-22 09:42:44.000000 cert-schema-3.6.4/cert_schema/3.2/credential_v2.json
+-rw-r--r--   0 julien     (503) staff       (20)     2609 2024-03-07 14:45:55.000000 cert-schema-3.6.4/cert_schema/3.2/dataIntegrityProof.json
+-rw-r--r--   0 julien     (503) staff       (20)      796 2024-03-07 14:45:55.000000 cert-schema-3.6.4/cert_schema/3.2/displaySchema.json
+-rw-r--r--   0 julien     (503) staff       (20)     5078 2024-03-07 14:45:55.000000 cert-schema-3.6.4/cert_schema/3.2/schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1274 2024-03-07 14:45:55.000000 cert-schema-3.6.4/cert_schema/3.2/statusList2021Context.json
+-rw-r--r--   0 julien     (503) staff       (20)      814 2024-03-08 14:44:45.000000 cert-schema-3.6.4/cert_schema/__init__.py
+-rw-r--r--   0 julien     (503) staff       (20)       22 2024-05-24 07:59:53.000000 cert-schema-3.6.4/cert_schema/__version__.py
+-rw-r--r--   0 julien     (503) staff       (20)     1597 2024-03-07 14:45:55.000000 cert-schema-3.6.4/cert_schema/context_urls.json
+-rw-r--r--   0 julien     (503) staff       (20)     2863 2024-03-07 14:45:55.000000 cert-schema-3.6.4/cert_schema/context_urls.py
+-rw-r--r--   0 julien     (503) staff       (20)       97 2021-04-08 16:27:50.000000 cert-schema-3.6.4/cert_schema/errors.py
+-rw-r--r--   0 julien     (503) staff       (20)    11660 2024-03-08 15:40:45.000000 cert-schema-3.6.4/cert_schema/jsonld_helpers.py
+-rw-r--r--   0 julien     (503) staff       (20)     4263 2021-12-08 14:45:05.000000 cert-schema-3.6.4/cert_schema/schema_validator.py
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2024-05-24 08:00:20.626307 cert-schema-3.6.4/cert_schema.egg-info/
+-rw-r--r--   0 julien     (503) staff       (20)     4156 2024-05-24 08:00:20.000000 cert-schema-3.6.4/cert_schema.egg-info/PKG-INFO
+-rw-r--r--   0 julien     (503) staff       (20)     3208 2024-05-24 08:00:20.000000 cert-schema-3.6.4/cert_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 julien     (503) staff       (20)        1 2024-05-24 08:00:20.000000 cert-schema-3.6.4/cert_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 julien     (503) staff       (20)       60 2024-05-24 08:00:20.000000 cert-schema-3.6.4/cert_schema.egg-info/requires.txt
+-rw-r--r--   0 julien     (503) staff       (20)       18 2024-05-24 08:00:20.000000 cert-schema-3.6.4/cert_schema.egg-info/top_level.txt
+-rw-r--r--   0 julien     (503) staff       (20)     1533 2024-05-21 13:53:07.000000 cert-schema-3.6.4/pyproject.toml
+-rw-r--r--   0 julien     (503) staff       (20)       60 2024-03-08 15:40:45.000000 cert-schema-3.6.4/requirements.txt
+-rw-r--r--   0 julien     (503) staff       (20)      137 2024-05-24 08:00:20.737108 cert-schema-3.6.4/setup.cfg
+-rw-r--r--   0 julien     (503) staff       (20)     1531 2024-03-08 15:40:45.000000 cert-schema-3.6.4/setup.py
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2024-05-24 08:00:20.734555 cert-schema-3.6.4/tests/
+-rw-r--r--   0 julien     (503) staff       (20)        0 2021-04-08 16:27:50.000000 cert-schema-3.6.4/tests/__init__.py
+-rw-r--r--   0 julien     (503) staff       (20)     4839 2024-03-07 14:45:55.000000 cert-schema-3.6.4/tests/test_context_urls.py
+-rw-r--r--   0 julien     (503) staff       (20)     2973 2023-05-17 15:00:18.000000 cert-schema-3.6.4/tests/test_jsonld_helpers.py
+-rw-r--r--   0 julien     (503) staff       (20)     3218 2021-12-08 14:45:05.000000 cert-schema-3.6.4/tests/test_schema_validator.py
```

### Comparing `cert-schema-3.6.3/CHANGELOG.md` & `cert-schema-3.6.4/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,42 @@
 # CHANGELOG
 
 
 
+## v3.6.3 (2024-03-19)
+
+### Chore
+
+* chore(SemanticRelease): simplify .travis.yml ([`f646418`](https://github.com/blockchain-certificates/cert-schema/commit/f6464189cb6b4b669d0fdeeeb30fc00fee5bb4ed))
+
+* chore(SemanticRelease): correctly set authToken ([`92ea4ca`](https://github.com/blockchain-certificates/cert-schema/commit/92ea4ca3395f16c0691a8d5a9b1307c86592d817))
+
+* chore(SemanticRelease): cleanup code and set npmAuth ([`2b00b21`](https://github.com/blockchain-certificates/cert-schema/commit/2b00b21c0427dfd2cd77bd96e91563612ba792a9))
+
+### Fix
+
+* fix(Context): update VC v2 context ([`2adab90`](https://github.com/blockchain-certificates/cert-schema/commit/2adab902d60345bc96c6ac13b13e2f201571e739))
+
+### Unknown
+
+* Merge pull request #64 from blockchain-certificates/fix/update-credential-v2-context
+
+Fix/update credential v2 context ([`56ee99f`](https://github.com/blockchain-certificates/cert-schema/commit/56ee99ff18258509c91c40cc246e01302c966073))
+
+* Merge branch &#39;master&#39; into fix/update-credential-v2-context ([`371156e`](https://github.com/blockchain-certificates/cert-schema/commit/371156ed7ce856438e9d02857e4d970f9228d7f4))
+
+* Merge pull request #63 from blockchain-certificates/chore/fix-semantic-release
+
+chore(SemanticRelease): correctly set authToken ([`a868084`](https://github.com/blockchain-certificates/cert-schema/commit/a86808437b4281dcb98bdf8113259e6d728eea7a))
+
+* Merge pull request #62 from blockchain-certificates/chore/fix-semantic-release
+
+chore(SemanticRelease): cleanup code and set npmAuth ([`d76b0e3`](https://github.com/blockchain-certificates/cert-schema/commit/d76b0e31ddef45ace924a9addf60302d1e91588c))
+
+
 ## v3.6.2 (2024-03-08)
 
 ### Chore
 
 * chore(SemanticRelease): decommission semantic-release js - move responsibility to python-semantic-release and manually publish ([`a4bec8c`](https://github.com/blockchain-certificates/cert-schema/commit/a4bec8c3d289efd84df82ebefa315806c1071497))
 
 * chore(Tox): prevent failure due to accessing cert_schema files before installing deps ([`5091bf5`](https://github.com/blockchain-certificates/cert-schema/commit/5091bf5fca67ab1d7f218e94c83592328b40eced))
@@ -28,14 +59,16 @@
 
 ### Unknown
 
 * Merge pull request #61 from blockchain-certificates/chore/fix-semantic-release
 
 chore(SemanticRelease): decommission semantic-release js - move respo… ([`79b20ec`](https://github.com/blockchain-certificates/cert-schema/commit/79b20ecdd63dea1289abdf0dfd20456438777414))
 
+* Merge branch &#39;master&#39; of https://github.com/blockchain-certificates/cert-schema ([`110e2db`](https://github.com/blockchain-certificates/cert-schema/commit/110e2dbf6b4166892df42bb370bbdf0037a258b4))
+
 * Merge pull request #60 from blockchain-certificates/chore/fix-semantic-release
 
 chore(SemanticRelease): configure python-semantic-release for &gt; v7 ([`d62cc64`](https://github.com/blockchain-certificates/cert-schema/commit/d62cc6410e5c8ef2f86a760fb79e04ef0d7048ef))
 
 * Merge pull request #59 from blockchain-certificates/feat/expose-data-integrity-proof-ctx
 
 fix(DataIntegrityProof): correct name for data integrity proof property ([`6588c07`](https://github.com/blockchain-certificates/cert-schema/commit/6588c07b19f7337ae08755ac6da86bf280db21d2))
@@ -353,15 +386,15 @@
 ### Unknown
 
 * Merge pull request #36 from blockchain-certificates/chore/npm-package
 
 Chore/npm package ([`ffd9f51`](https://github.com/blockchain-certificates/cert-schema/commit/ffd9f51bb343410d716e44413ba1d6bdf02cc672))
 
 
-## v3.0.4 (2022-04-05)
+## v3.0.4 (2022-04-04)
 
 ### Chore
 
 * chore(Release): update release steps ([`67a4e11`](https://github.com/blockchain-certificates/cert-schema/commit/67a4e1180dfa6fa70d7c8e2a48300576f70f6332))
 
 * chore(Version): bump version ([`df5082f`](https://github.com/blockchain-certificates/cert-schema/commit/df5082f3cc4cf900fadb8e0eae4b60ccc84c278f))
 
@@ -393,32 +426,28 @@
 
 * feat(v3b): list VC contexts ([`7fc11b2`](https://github.com/blockchain-certificates/cert-schema/commit/7fc11b2c27308135ab98a1c6ecd127fb7f65fa28))
 
 * feat(V3Beta): normalize display property ([`c4e5f18`](https://github.com/blockchain-certificates/cert-schema/commit/c4e5f18f378d5470e9ccee590c62d9bb1fa023b8))
 
 * feat(Metadata): define metadata object ([`05e5976`](https://github.com/blockchain-certificates/cert-schema/commit/05e59762baa3fc2591e6c976d2e00f27e34016cd))
 
-* feat(3.0-beta): added attempt for metadata ([`b59b65e`](https://github.com/blockchain-certificates/cert-schema/commit/b59b65e81802ca244ab4be1f805b2df018afa69c))
-
 ### Fix
 
 * fix(JsonLd): fix preloading URL for blockcert.org ([`af3cc64`](https://github.com/blockchain-certificates/cert-schema/commit/af3cc6404fd8a781bd51094fbb5647352ef67524))
 
 * fix(V3): ensure display value is being hashed ([`dc5f2eb`](https://github.com/blockchain-certificates/cert-schema/commit/dc5f2eb5e93bdf398eaa6acf737b69977924f8ba))
 
 * fix(v3): remove copy paste item ([`51f72d1`](https://github.com/blockchain-certificates/cert-schema/commit/51f72d15062b756809c62e60da1c50ae43f068dc))
 
 * fix(v3): correct w3id path to schema ([`ba9c4f1`](https://github.com/blockchain-certificates/cert-schema/commit/ba9c4f164c21f45c1eb55d9b32837f6746bce8e2))
 
 * fix(v3): properly expose items ([`30d8601`](https://github.com/blockchain-certificates/cert-schema/commit/30d8601ed6f1c6e98fbf26d87b03cf2bfbcba747))
 
 * fix(Context): change copy paste error ([`9d37aad`](https://github.com/blockchain-certificates/cert-schema/commit/9d37aad9bd666d5bcc1fc61f1b22fdd675290af2))
 
-* fix(ld): leverage w3id syntax ([`72b0710`](https://github.com/blockchain-certificates/cert-schema/commit/72b0710390c9dab8e4c7d4ed33f68a8147e210a7))
-
 ### Test
 
 * test(v3): define id as non-relative value ([`3531682`](https://github.com/blockchain-certificates/cert-schema/commit/3531682d768c72bd833b7dc8e9263a5ac33c344d))
 
 * test(All): ensure all tests are run ([`fd87426`](https://github.com/blockchain-certificates/cert-schema/commit/fd87426bd6393e98b98f9421589b93aa6486cc9b))
 
 * test(V3): add custom contexts tests ([`968368f`](https://github.com/blockchain-certificates/cert-schema/commit/968368f017be5b8b0cd0b64ea53cb92fe22b77da))
@@ -483,20 +512,14 @@
 
 add import validater ([`f735f24`](https://github.com/blockchain-certificates/cert-schema/commit/f735f241585bdb2dcbc76eee5f6c7243edbe63c4))
 
 * import validater ([`926bfff`](https://github.com/blockchain-certificates/cert-schema/commit/926bfffa45d0ce033e9708dcfa64592c4af73929))
 
 * doc(3.0-beta): added doc ([`b154dd5`](https://github.com/blockchain-certificates/cert-schema/commit/b154dd5b902c4ca3341e99277a9ccade519f7a83))
 
-* doc(30Beta): missing ssl protocols ([`f45d3fa`](https://github.com/blockchain-certificates/cert-schema/commit/f45d3fae55972592c5db5ee1e512b249247d2d87))
-
-* Merge branch &#39;feat/v3-beta&#39; of https://github.com/blockchain-certificates/cert-schema into feat/v3-beta ([`d0a29f8`](https://github.com/blockchain-certificates/cert-schema/commit/d0a29f8fdb75ff0834325e7b4f5a87214075705d))
-
-* doc(3.0-beta): removed false description ([`aafd7da`](https://github.com/blockchain-certificates/cert-schema/commit/aafd7dadb1838233061116158ec3c242869982fc))
-
 * Merge pull request #22 from blockchain-certificates/update-merkleproof2019-link
 
 update link ([`96c3e42`](https://github.com/blockchain-certificates/cert-schema/commit/96c3e423ce0dec046c7d080fe384dacd51316efa))
 
 * update link ([`1d4dac8`](https://github.com/blockchain-certificates/cert-schema/commit/1d4dac8f44af90c241080a71f4eec44492865fe4))
 
 * Revving version to republish PyPI package. ([`fc2652a`](https://github.com/blockchain-certificates/cert-schema/commit/fc2652a9426061edfd605aaf487fc098dbcb8528))
@@ -537,32 +560,8 @@
 
 * Merge pull request #12 from blockchain-certificates/v3
 
 Fixing v3-alpha schema ([`b3d9f93`](https://github.com/blockchain-certificates/cert-schema/commit/b3d9f937313ba9eba6c4bb2eb59d6206d80aacc4))
 
 * Bump v3-alpha version ([`9d58742`](https://github.com/blockchain-certificates/cert-schema/commit/9d5874238283b80e8e5278febf1b04211d7e2fa7))
 
-* Remove old/conflicting schema references in v3 ([`3d6f681`](https://github.com/blockchain-certificates/cert-schema/commit/3d6f681f9028b71c87127c9207ea4ae3d376f1cc))
-
-* Fix v3 reference link ([`4374b7d`](https://github.com/blockchain-certificates/cert-schema/commit/4374b7d87218bd842b9c27c0d79da2700377318f))
-
 * Update bbba8553-8ec1-445f-82c9-a57251dd731c.json ([`f608739`](https://github.com/blockchain-certificates/cert-schema/commit/f60873943f1d975346ff40519bacd2473ec3dac0))
-
-* Update README.md ([`6cf90f2`](https://github.com/blockchain-certificates/cert-schema/commit/6cf90f277e4655b260c572977c2cc32e7fca8cf2))
-
-* Merge pull request #10 from blockchain-certificates/v3
-
-PyPI Updates V3 ([`bce6b9b`](https://github.com/blockchain-certificates/cert-schema/commit/bce6b9bc28634d64dea192513a0455741f1b8521))
-
-* Merge remote-tracking branch &#39;origin/v3&#39; into v3 ([`53df114`](https://github.com/blockchain-certificates/cert-schema/commit/53df11406489e508e07eb4074baeb3dd381304aa))
-
-* Updating v3 for publishing to pypi ([`7a6af7c`](https://github.com/blockchain-certificates/cert-schema/commit/7a6af7c3c36080c1bdf59eac2067dd45f8048a25))
-
-* Merge pull request #9 from blockchain-certificates/v3
-
-V3 ([`d3aabc1`](https://github.com/blockchain-certificates/cert-schema/commit/d3aabc105e6f54ba75306ac769f293ef1e042a1c))
-
-* Update README.md ([`30da460`](https://github.com/blockchain-certificates/cert-schema/commit/30da460c714845e0bce99ab283e422f130ecee3a))
-
-* Merge pull request #7 from davidlj95/unknown-eth-testnet
-
-Remove ambiguous ethereumTestnet from anchor chains ([`67b5467`](https://github.com/blockchain-certificates/cert-schema/commit/67b5467b88bc4cbd5fcd59af516dcc429c5917d6))
```

### Comparing `cert-schema-3.6.3/LICENSE` & `cert-schema-3.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/PKG-INFO` & `cert-schema-3.6.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,88 +1,88 @@
 Metadata-Version: 2.1
 Name: cert-schema
-Version: 3.6.3
+Version: 3.6.4
 Summary: Blockchain certificates JSON-LD context and JSON schemas
 Home-page: https://github.com/blockchain-certificates/cert-schema
 Author: info@blockcerts.org
 Author-email: info@blockcerts.org
 License: MIT
+Description: [![Build Status](https://travis-ci.org/blockchain-certificates/cert-schema.svg?branch=master)](https://travis-ci.org/blockchain-certificates/cert-schema)
+        [![PyPI version](https://badge.fury.io/py/cert-schema.svg)](https://badge.fury.io/py/cert-schema)
+        
+        # cert-schema
+        
+        Blockchain Certificate schemas implement those of [Verifiable Credentials](https://www.w3.org/TR/vc-data-model/). As with Verifiable Credentials, we've provided both a JSON-LD context and JSON schema. The purpose of the JSON-LD context is to map types to Internationalized Resource Identifiers (IRIs), providing semantic context for data. The JSON Schema is used for syntactic validation.
+        
+        This python package allows verification of a Blockchain Certificate against the JSON
+        schemas as a convenience. This is not the same as verifying the contents of a certificate against what is stored
+        on the blockchain. See the [cert-verifier-js](https://github.com/blockchain-certificates/cert-verifier-js) project.
+        
+        *   [Blockcerts JSON Schema](docs/schema-3.0-alpha.md)
+        
+        ## Example
+        
+        TODO update for V3 once cert-issuer issues one
+        
+        The following is a Blockchain Certificate issued on the testnet Bitcoin network.
+        
+        ```json
+        {
+          "@context": [
+            "https://www.w3.org/2018/credentials/v1",
+            "https://www.blockcerts.org/schema/3.0-alpha/context.json",
+            "https://www.w3.org/2018/credentials/examples/v1"
+          ],
+          "id": "urn:uuid:bbba8553-8ec1-445f-82c9-a57251dd731c",
+          "type": [
+            "VerifiableCredential"
+          ],
+          "issuer": "did:example:23adb1f712ebc6f1c276eba4dfa",
+          "issuanceDate": "2010-01-01T19:73:24Z",
+          "credentialSubject": {
+            "id": "did:example:ebfeb1f712ebc6f1c276e12ec21",
+            "alumniOf": {
+              "id": "did:example:c276e12ec21ebfeb1f712ebc6f1"
+            }
+          },
+          "signature": {
+            "type": "MerkleProof2019",
+            "created": "2020-01-21T12:32:11.693759",
+            "proofValue": "z2LuLBVSfnVzaQtvzuA7EaPQsGEgYWeaMTH1p3uqAG3ESx9HYyFzFFrYsyPkZSbn1Ji5LN76jw6HBr3oiaa8KsQenCPqKk7dJvxEXsDnYvhuDHtsrSRbzHdJKd66jAowkzPxPFi3ivyAv7WRK1WV2VhegYVQEnCBTrGJWFUMFFXunTcus7ZyedQvS4sr61X2y8QuJ57ycB5JMEHvUgAVq3qh2g3ucehg2ERKLo98jmqTcsh9HThkECG3BTNYRD3QL7AHWPjxRbQNSA83QNYXcCNA7NaZnCWyjC17ZBj3xszp76XvqFRrLjQbRSbzjVTPtBSV8QjhxThT3KTfgwjRn5JeeXhYvebsTT9YGL3W4ufzFRDpH79n5KPiaj1BPbEUfUq7vf2dg26QWeZBi7ME56",
+            "proofPurpose": "assertionMethod",
+            "verificationMethod": "ecdsa-koblitz-pubkey:0x7e30a37763e6Ba1fFeDE1750bBeFB4c60b17a1B3"
+          }
+        }
+        ```
+        
+        ## Publishing package to pypi
+        
+        - [First time info](https://web.archive.org/web/20180501071551/http://peterdowns.com/posts/first-time-with-pypi.html)
+        - Publish script: `./release_package.sh`
+        
+        
+        ## Unit tests
+        
+        This project uses tox to validate against several python environments.
+        
+        1. Ensure you have an python environment. [Recommendations](https://github.com/blockchain-certificates/cert-issuer/blob/master/docs/virtualenv.md)
+        
+        2. Run tests
+            ```
+            ./run_tests.sh
+            ```
+        
+        
+        ## Compile markdown from schema
+        
+        Note that json-schema-to-markdown doesn't handle ref schemas well, so you will 
+        need to manually update any 'undefined' references.
+        
+        `scripts/generate_markdown.js` builds the markdown-formatted schemas from json
+        
+        ## Contact
+        
+        Contact us at [the Blockcerts community forum](http://community.blockcerts.org/).
+        
+        
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Build Status](https://travis-ci.org/blockchain-certificates/cert-schema.svg?branch=master)](https://travis-ci.org/blockchain-certificates/cert-schema)
-[![PyPI version](https://badge.fury.io/py/cert-schema.svg)](https://badge.fury.io/py/cert-schema)
-
-# cert-schema
-
-Blockchain Certificate schemas implement those of [Verifiable Credentials](https://www.w3.org/TR/vc-data-model/). As with Verifiable Credentials, we've provided both a JSON-LD context and JSON schema. The purpose of the JSON-LD context is to map types to Internationalized Resource Identifiers (IRIs), providing semantic context for data. The JSON Schema is used for syntactic validation.
-
-This python package allows verification of a Blockchain Certificate against the JSON
-schemas as a convenience. This is not the same as verifying the contents of a certificate against what is stored
-on the blockchain. See the [cert-verifier-js](https://github.com/blockchain-certificates/cert-verifier-js) project.
-
-*   [Blockcerts JSON Schema](docs/schema-3.0-alpha.md)
-
-## Example
-
-TODO update for V3 once cert-issuer issues one
-
-The following is a Blockchain Certificate issued on the testnet Bitcoin network.
-
-```json
-{
-  "@context": [
-    "https://www.w3.org/2018/credentials/v1",
-    "https://www.blockcerts.org/schema/3.0-alpha/context.json",
-    "https://www.w3.org/2018/credentials/examples/v1"
-  ],
-  "id": "urn:uuid:bbba8553-8ec1-445f-82c9-a57251dd731c",
-  "type": [
-    "VerifiableCredential"
-  ],
-  "issuer": "did:example:23adb1f712ebc6f1c276eba4dfa",
-  "issuanceDate": "2010-01-01T19:73:24Z",
-  "credentialSubject": {
-    "id": "did:example:ebfeb1f712ebc6f1c276e12ec21",
-    "alumniOf": {
-      "id": "did:example:c276e12ec21ebfeb1f712ebc6f1"
-    }
-  },
-  "signature": {
-    "type": "MerkleProof2019",
-    "created": "2020-01-21T12:32:11.693759",
-    "proofValue": "z2LuLBVSfnVzaQtvzuA7EaPQsGEgYWeaMTH1p3uqAG3ESx9HYyFzFFrYsyPkZSbn1Ji5LN76jw6HBr3oiaa8KsQenCPqKk7dJvxEXsDnYvhuDHtsrSRbzHdJKd66jAowkzPxPFi3ivyAv7WRK1WV2VhegYVQEnCBTrGJWFUMFFXunTcus7ZyedQvS4sr61X2y8QuJ57ycB5JMEHvUgAVq3qh2g3ucehg2ERKLo98jmqTcsh9HThkECG3BTNYRD3QL7AHWPjxRbQNSA83QNYXcCNA7NaZnCWyjC17ZBj3xszp76XvqFRrLjQbRSbzjVTPtBSV8QjhxThT3KTfgwjRn5JeeXhYvebsTT9YGL3W4ufzFRDpH79n5KPiaj1BPbEUfUq7vf2dg26QWeZBi7ME56",
-    "proofPurpose": "assertionMethod",
-    "verificationMethod": "ecdsa-koblitz-pubkey:0x7e30a37763e6Ba1fFeDE1750bBeFB4c60b17a1B3"
-  }
-}
-```
-
-## Publishing package to pypi
-
-- [First time info](https://web.archive.org/web/20180501071551/http://peterdowns.com/posts/first-time-with-pypi.html)
-- Publish script: `./release_package.sh`
-
-
-## Unit tests
-
-This project uses tox to validate against several python environments.
-
-1. Ensure you have an python environment. [Recommendations](https://github.com/blockchain-certificates/cert-issuer/blob/master/docs/virtualenv.md)
-
-2. Run tests
-    ```
-    ./run_tests.sh
-    ```
-
-
-## Compile markdown from schema
-
-Note that json-schema-to-markdown doesn't handle ref schemas well, so you will 
-need to manually update any 'undefined' references.
-
-`scripts/generate_markdown.js` builds the markdown-formatted schemas from json
-
-## Contact
-
-Contact us at [the Blockcerts community forum](http://community.blockcerts.org/).
-
```

### Comparing `cert-schema-3.6.3/README.md` & `cert-schema-3.6.4/README.md`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/1.1/certificate-schema-v1-1.json` & `cert-schema-3.6.4/cert_schema/1.1/certificate-schema-v1-1.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/1.1/issuer-schema-v1-1.json` & `cert-schema-3.6.4/cert_schema/1.1/issuer-schema-v1-1.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/1.2/assertion-1.2.json` & `cert-schema-3.6.4/cert_schema/1.2/assertion-1.2.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/1.2/blockchain-certificate-1.2.json` & `cert-schema-3.6.4/cert_schema/1.2/blockchain-certificate-1.2.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/1.2/blockchain-receipt-1.2.json` & `cert-schema-3.6.4/cert_schema/1.2/blockchain-receipt-1.2.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/1.2/certificate-1.2.json` & `cert-schema-3.6.4/cert_schema/1.2/certificate-1.2.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/1.2/certificate-document-1.2.json` & `cert-schema-3.6.4/cert_schema/1.2/certificate-document-1.2.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/1.2/context.json` & `cert-schema-3.6.4/cert_schema/1.2/context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/1.2/issuer-1.2.json` & `cert-schema-3.6.4/cert_schema/1.2/issuer-1.2.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/1.2/issuer-id-1.2.json` & `cert-schema-3.6.4/cert_schema/1.2/issuer-id-1.2.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/2.0/context.json` & `cert-schema-3.6.4/cert_schema/2.0/context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/2.0/issuerSchema.json` & `cert-schema-3.6.4/cert_schema/2.0/issuerSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/2.0/merkleProof2017Schema.json` & `cert-schema-3.6.4/cert_schema/2.0/merkleProof2017Schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/2.0/obi.json` & `cert-schema-3.6.4/cert_schema/2.0/obi.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/2.0/recipientSchema.json` & `cert-schema-3.6.4/cert_schema/2.0/recipientSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/2.0/schema.json` & `cert-schema-3.6.4/cert_schema/2.0/schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/2.0/signatureLineSchema.json` & `cert-schema-3.6.4/cert_schema/2.0/signatureLineSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/2.0-alpha/context.json` & `cert-schema-3.6.4/cert_schema/2.0-alpha/context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/2.0-alpha/issuerSchema.json` & `cert-schema-3.6.4/cert_schema/2.0-alpha/issuerSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/2.0-alpha/merkleProof2017Schema.json` & `cert-schema-3.6.4/cert_schema/2.0-alpha/merkleProof2017Schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/2.0-alpha/recipientSchema.json` & `cert-schema-3.6.4/cert_schema/2.0-alpha/recipientSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/2.0-alpha/schema.json` & `cert-schema-3.6.4/cert_schema/2.0-alpha/schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/2.0-alpha/signatureLineSchema.json` & `cert-schema-3.6.4/cert_schema/2.0-alpha/signatureLineSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/2.1/context.json` & `cert-schema-3.6.4/cert_schema/2.1/context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/2.1/issuerSchema.json` & `cert-schema-3.6.4/cert_schema/2.1/issuerSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/2.1/merkleProof2017Schema.json` & `cert-schema-3.6.4/cert_schema/2.1/merkleProof2017Schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/2.1/obi.json` & `cert-schema-3.6.4/cert_schema/2.1/obi.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/2.1/recipientSchema.json` & `cert-schema-3.6.4/cert_schema/2.1/recipientSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/2.1/schema.json` & `cert-schema-3.6.4/cert_schema/2.1/schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/2.1/signatureLineSchema.json` & `cert-schema-3.6.4/cert_schema/2.1/signatureLineSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0/claimSchema.json` & `cert-schema-3.6.4/cert_schema/3.0/claimSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0/context.json` & `cert-schema-3.6.4/cert_schema/3.0/context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0/credential.json` & `cert-schema-3.6.4/cert_schema/3.0/credential.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0/credentialSubjectSchema.json` & `cert-schema-3.6.4/cert_schema/3.0/credentialSubjectSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0/displaySchema.json` & `cert-schema-3.6.4/cert_schema/3.0/displaySchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0/merkleProof2019Context.json` & `cert-schema-3.6.4/cert_schema/3.0/merkleProof2019Context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0/merkleProof2019Schema.json` & `cert-schema-3.6.4/cert_schema/3.0/merkleProof2019Schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0/schema.json` & `cert-schema-3.6.4/cert_schema/3.0/schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0-alpha/context.json` & `cert-schema-3.6.4/cert_schema/3.0-alpha/context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0-alpha/credential.json` & `cert-schema-3.6.4/cert_schema/3.0-alpha/credential.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0-alpha/exampleCredential.json` & `cert-schema-3.6.4/cert_schema/3.0-alpha/exampleCredential.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0-alpha/issuerSchema.json` & `cert-schema-3.6.4/cert_schema/3.0-alpha/issuerSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0-alpha/merkleProof2019Context.json` & `cert-schema-3.6.4/cert_schema/3.0-alpha/merkleProof2019Context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0-alpha/merkleProof2019Schema.json` & `cert-schema-3.6.4/cert_schema/3.0-alpha/merkleProof2019Schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0-alpha/schema.json` & `cert-schema-3.6.4/cert_schema/3.0-alpha/schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0-beta/context.json` & `cert-schema-3.6.4/cert_schema/3.0-beta/context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0-beta/credential.json` & `cert-schema-3.6.4/cert_schema/3.0-beta/credential.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0-beta/displaySchema.json` & `cert-schema-3.6.4/cert_schema/3.0-beta/displaySchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0-beta/exampleCredential.json` & `cert-schema-3.6.4/cert_schema/3.0-beta/exampleCredential.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0-beta/merkleProof2019Context.json` & `cert-schema-3.6.4/cert_schema/3.0-beta/merkleProof2019Context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0-beta/merkleProof2019Schema.json` & `cert-schema-3.6.4/cert_schema/3.0-beta/merkleProof2019Schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.0-beta/schema.json` & `cert-schema-3.6.4/cert_schema/3.0-beta/schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.1/chainedProof2021Context.json` & `cert-schema-3.6.4/cert_schema/3.1/chainedProof2021Context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.1/claimSchema.json` & `cert-schema-3.6.4/cert_schema/3.1/claimSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.1/context.json` & `cert-schema-3.6.4/cert_schema/3.1/context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.1/credential.json` & `cert-schema-3.6.4/cert_schema/3.1/credential.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.1/credentialSubjectSchema.json` & `cert-schema-3.6.4/cert_schema/3.1/credentialSubjectSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.1/displaySchema.json` & `cert-schema-3.6.4/cert_schema/3.1/displaySchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.1/merkleProof2019Context.json` & `cert-schema-3.6.4/cert_schema/3.1/merkleProof2019Context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.1/merkleProof2019Schema.json` & `cert-schema-3.6.4/cert_schema/3.1/merkleProof2019Schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.1/schema.json` & `cert-schema-3.6.4/cert_schema/3.1/schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.1/statusList2021Context.json` & `cert-schema-3.6.4/cert_schema/3.1/statusList2021Context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.2/claimSchema.json` & `cert-schema-3.6.4/cert_schema/3.2/claimSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.2/context.json` & `cert-schema-3.6.4/cert_schema/3.2/context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.2/credentialSubjectSchema.json` & `cert-schema-3.6.4/cert_schema/3.2/credentialSubjectSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.2/credential_v2.json` & `cert-schema-3.6.4/cert_schema/3.2/credential_v2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997759856630825%*

 * *Differences: {"'@context'": "{'BitstringStatusList': {'@context': {'statusReference': {replace: "*

 * *               "OrderedDict([('@id', 'https://www.w3.org/ns/credentials/status#statusReference'), "*

 * *               "('@type', '@id')])}, 'statusSize': {replace: OrderedDict([('@id', "*

 * *               "'https://www.w3.org/ns/credentials/status#statusSize'), ('@type', "*

 * *               "'https://www.w3.org/2001/XMLSchema#positiveInteger')])}}}}"}*

```diff
@@ -20,16 +20,22 @@
                         "message": "https://www.w3.org/ns/credentials/status#message",
                         "status": "https://www.w3.org/ns/credentials/status#status",
                         "type": "@type"
                     },
                     "@id": "https://www.w3.org/ns/credentials/status#statusMessage"
                 },
                 "statusPurpose": "https://www.w3.org/ns/credentials/status#statusPurpose",
-                "statusReference": "https://www.w3.org/ns/credentials/status#statusReference",
-                "statusSize": "https://www.w3.org/ns/credentials/status#statusSize",
+                "statusReference": {
+                    "@id": "https://www.w3.org/ns/credentials/status#statusReference",
+                    "@type": "@id"
+                },
+                "statusSize": {
+                    "@id": "https://www.w3.org/ns/credentials/status#statusSize",
+                    "@type": "https://www.w3.org/2001/XMLSchema#positiveInteger"
+                },
                 "ttl": "https://www.w3.org/ns/credentials/status#ttl",
                 "type": "@type"
             },
             "@id": "https://www.w3.org/ns/credentials/status#BitstringStatusList"
         },
         "BitstringStatusListCredential": "https://www.w3.org/ns/credentials/status#BitstringStatusListCredential",
         "BitstringStatusListEntry": {
```

### Comparing `cert-schema-3.6.3/cert_schema/3.2/dataIntegrityProof.json` & `cert-schema-3.6.4/cert_schema/3.2/dataIntegrityProof.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.2/displaySchema.json` & `cert-schema-3.6.4/cert_schema/3.2/displaySchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.2/schema.json` & `cert-schema-3.6.4/cert_schema/3.2/schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/3.2/statusList2021Context.json` & `cert-schema-3.6.4/cert_schema/3.2/statusList2021Context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/__init__.py` & `cert-schema-3.6.4/cert_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/context_urls.json` & `cert-schema-3.6.4/cert_schema/context_urls.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/context_urls.py` & `cert-schema-3.6.4/cert_schema/context_urls.py`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/jsonld_helpers.py` & `cert-schema-3.6.4/cert_schema/jsonld_helpers.py`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema/schema_validator.py` & `cert-schema-3.6.4/cert_schema/schema_validator.py`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/cert_schema.egg-info/PKG-INFO` & `cert-schema-3.6.4/cert_schema.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,88 +1,88 @@
 Metadata-Version: 2.1
 Name: cert-schema
-Version: 3.6.3
+Version: 3.6.4
 Summary: Blockchain certificates JSON-LD context and JSON schemas
 Home-page: https://github.com/blockchain-certificates/cert-schema
 Author: info@blockcerts.org
 Author-email: info@blockcerts.org
 License: MIT
+Description: [![Build Status](https://travis-ci.org/blockchain-certificates/cert-schema.svg?branch=master)](https://travis-ci.org/blockchain-certificates/cert-schema)
+        [![PyPI version](https://badge.fury.io/py/cert-schema.svg)](https://badge.fury.io/py/cert-schema)
+        
+        # cert-schema
+        
+        Blockchain Certificate schemas implement those of [Verifiable Credentials](https://www.w3.org/TR/vc-data-model/). As with Verifiable Credentials, we've provided both a JSON-LD context and JSON schema. The purpose of the JSON-LD context is to map types to Internationalized Resource Identifiers (IRIs), providing semantic context for data. The JSON Schema is used for syntactic validation.
+        
+        This python package allows verification of a Blockchain Certificate against the JSON
+        schemas as a convenience. This is not the same as verifying the contents of a certificate against what is stored
+        on the blockchain. See the [cert-verifier-js](https://github.com/blockchain-certificates/cert-verifier-js) project.
+        
+        *   [Blockcerts JSON Schema](docs/schema-3.0-alpha.md)
+        
+        ## Example
+        
+        TODO update for V3 once cert-issuer issues one
+        
+        The following is a Blockchain Certificate issued on the testnet Bitcoin network.
+        
+        ```json
+        {
+          "@context": [
+            "https://www.w3.org/2018/credentials/v1",
+            "https://www.blockcerts.org/schema/3.0-alpha/context.json",
+            "https://www.w3.org/2018/credentials/examples/v1"
+          ],
+          "id": "urn:uuid:bbba8553-8ec1-445f-82c9-a57251dd731c",
+          "type": [
+            "VerifiableCredential"
+          ],
+          "issuer": "did:example:23adb1f712ebc6f1c276eba4dfa",
+          "issuanceDate": "2010-01-01T19:73:24Z",
+          "credentialSubject": {
+            "id": "did:example:ebfeb1f712ebc6f1c276e12ec21",
+            "alumniOf": {
+              "id": "did:example:c276e12ec21ebfeb1f712ebc6f1"
+            }
+          },
+          "signature": {
+            "type": "MerkleProof2019",
+            "created": "2020-01-21T12:32:11.693759",
+            "proofValue": "z2LuLBVSfnVzaQtvzuA7EaPQsGEgYWeaMTH1p3uqAG3ESx9HYyFzFFrYsyPkZSbn1Ji5LN76jw6HBr3oiaa8KsQenCPqKk7dJvxEXsDnYvhuDHtsrSRbzHdJKd66jAowkzPxPFi3ivyAv7WRK1WV2VhegYVQEnCBTrGJWFUMFFXunTcus7ZyedQvS4sr61X2y8QuJ57ycB5JMEHvUgAVq3qh2g3ucehg2ERKLo98jmqTcsh9HThkECG3BTNYRD3QL7AHWPjxRbQNSA83QNYXcCNA7NaZnCWyjC17ZBj3xszp76XvqFRrLjQbRSbzjVTPtBSV8QjhxThT3KTfgwjRn5JeeXhYvebsTT9YGL3W4ufzFRDpH79n5KPiaj1BPbEUfUq7vf2dg26QWeZBi7ME56",
+            "proofPurpose": "assertionMethod",
+            "verificationMethod": "ecdsa-koblitz-pubkey:0x7e30a37763e6Ba1fFeDE1750bBeFB4c60b17a1B3"
+          }
+        }
+        ```
+        
+        ## Publishing package to pypi
+        
+        - [First time info](https://web.archive.org/web/20180501071551/http://peterdowns.com/posts/first-time-with-pypi.html)
+        - Publish script: `./release_package.sh`
+        
+        
+        ## Unit tests
+        
+        This project uses tox to validate against several python environments.
+        
+        1. Ensure you have an python environment. [Recommendations](https://github.com/blockchain-certificates/cert-issuer/blob/master/docs/virtualenv.md)
+        
+        2. Run tests
+            ```
+            ./run_tests.sh
+            ```
+        
+        
+        ## Compile markdown from schema
+        
+        Note that json-schema-to-markdown doesn't handle ref schemas well, so you will 
+        need to manually update any 'undefined' references.
+        
+        `scripts/generate_markdown.js` builds the markdown-formatted schemas from json
+        
+        ## Contact
+        
+        Contact us at [the Blockcerts community forum](http://community.blockcerts.org/).
+        
+        
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Build Status](https://travis-ci.org/blockchain-certificates/cert-schema.svg?branch=master)](https://travis-ci.org/blockchain-certificates/cert-schema)
-[![PyPI version](https://badge.fury.io/py/cert-schema.svg)](https://badge.fury.io/py/cert-schema)
-
-# cert-schema
-
-Blockchain Certificate schemas implement those of [Verifiable Credentials](https://www.w3.org/TR/vc-data-model/). As with Verifiable Credentials, we've provided both a JSON-LD context and JSON schema. The purpose of the JSON-LD context is to map types to Internationalized Resource Identifiers (IRIs), providing semantic context for data. The JSON Schema is used for syntactic validation.
-
-This python package allows verification of a Blockchain Certificate against the JSON
-schemas as a convenience. This is not the same as verifying the contents of a certificate against what is stored
-on the blockchain. See the [cert-verifier-js](https://github.com/blockchain-certificates/cert-verifier-js) project.
-
-*   [Blockcerts JSON Schema](docs/schema-3.0-alpha.md)
-
-## Example
-
-TODO update for V3 once cert-issuer issues one
-
-The following is a Blockchain Certificate issued on the testnet Bitcoin network.
-
-```json
-{
-  "@context": [
-    "https://www.w3.org/2018/credentials/v1",
-    "https://www.blockcerts.org/schema/3.0-alpha/context.json",
-    "https://www.w3.org/2018/credentials/examples/v1"
-  ],
-  "id": "urn:uuid:bbba8553-8ec1-445f-82c9-a57251dd731c",
-  "type": [
-    "VerifiableCredential"
-  ],
-  "issuer": "did:example:23adb1f712ebc6f1c276eba4dfa",
-  "issuanceDate": "2010-01-01T19:73:24Z",
-  "credentialSubject": {
-    "id": "did:example:ebfeb1f712ebc6f1c276e12ec21",
-    "alumniOf": {
-      "id": "did:example:c276e12ec21ebfeb1f712ebc6f1"
-    }
-  },
-  "signature": {
-    "type": "MerkleProof2019",
-    "created": "2020-01-21T12:32:11.693759",
-    "proofValue": "z2LuLBVSfnVzaQtvzuA7EaPQsGEgYWeaMTH1p3uqAG3ESx9HYyFzFFrYsyPkZSbn1Ji5LN76jw6HBr3oiaa8KsQenCPqKk7dJvxEXsDnYvhuDHtsrSRbzHdJKd66jAowkzPxPFi3ivyAv7WRK1WV2VhegYVQEnCBTrGJWFUMFFXunTcus7ZyedQvS4sr61X2y8QuJ57ycB5JMEHvUgAVq3qh2g3ucehg2ERKLo98jmqTcsh9HThkECG3BTNYRD3QL7AHWPjxRbQNSA83QNYXcCNA7NaZnCWyjC17ZBj3xszp76XvqFRrLjQbRSbzjVTPtBSV8QjhxThT3KTfgwjRn5JeeXhYvebsTT9YGL3W4ufzFRDpH79n5KPiaj1BPbEUfUq7vf2dg26QWeZBi7ME56",
-    "proofPurpose": "assertionMethod",
-    "verificationMethod": "ecdsa-koblitz-pubkey:0x7e30a37763e6Ba1fFeDE1750bBeFB4c60b17a1B3"
-  }
-}
-```
-
-## Publishing package to pypi
-
-- [First time info](https://web.archive.org/web/20180501071551/http://peterdowns.com/posts/first-time-with-pypi.html)
-- Publish script: `./release_package.sh`
-
-
-## Unit tests
-
-This project uses tox to validate against several python environments.
-
-1. Ensure you have an python environment. [Recommendations](https://github.com/blockchain-certificates/cert-issuer/blob/master/docs/virtualenv.md)
-
-2. Run tests
-    ```
-    ./run_tests.sh
-    ```
-
-
-## Compile markdown from schema
-
-Note that json-schema-to-markdown doesn't handle ref schemas well, so you will 
-need to manually update any 'undefined' references.
-
-`scripts/generate_markdown.js` builds the markdown-formatted schemas from json
-
-## Contact
-
-Contact us at [the Blockcerts community forum](http://community.blockcerts.org/).
-
```

### Comparing `cert-schema-3.6.3/cert_schema.egg-info/SOURCES.txt` & `cert-schema-3.6.4/cert_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/pyproject.toml` & `cert-schema-3.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/setup.py` & `cert-schema-3.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/tests/test_context_urls.py` & `cert-schema-3.6.4/tests/test_context_urls.py`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/tests/test_jsonld_helpers.py` & `cert-schema-3.6.4/tests/test_jsonld_helpers.py`

 * *Files identical despite different names*

### Comparing `cert-schema-3.6.3/tests/test_schema_validator.py` & `cert-schema-3.6.4/tests/test_schema_validator.py`

 * *Files identical despite different names*


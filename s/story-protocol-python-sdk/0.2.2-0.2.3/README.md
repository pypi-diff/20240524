# Comparing `tmp/story_protocol_python_sdk-0.2.2.tar.gz` & `tmp/story_protocol_python_sdk-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "story_protocol_python_sdk-0.2.2.tar", last modified: Fri May 24 01:31:28 2024, max compression
+gzip compressed data, was "story_protocol_python_sdk-0.2.3.tar", last modified: Fri May 24 18:31:24 2024, max compression
```

## Comparing `story_protocol_python_sdk-0.2.2.tar` & `story_protocol_python_sdk-0.2.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.401136 story_protocol_python_sdk-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-24 01:31:28.401136 story_protocol_python_sdk-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 01:31:28.401136 story_protocol_python_sdk-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.393136 story_protocol_python_sdk-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.397136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.397136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.397136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/
--rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.397136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/
--rw-r--r--   0 runner    (1001) docker     (127)    15302 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.397136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseRegistry/
--rw-r--r--   0 runner    (1001) docker     (127)    25612 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseRegistry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.397136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseToken/
--rw-r--r--   0 runner    (1001) docker     (127)    21851 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseToken/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.397136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicensingModule/
--rw-r--r--   0 runner    (1001) docker     (127)    18746 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicensingModule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.401136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/
--rw-r--r--   0 runner    (1001) docker     (127)    25040 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.401136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyModule/
--rw-r--r--   0 runner    (1001) docker     (127)    15228 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyModule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.401136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/
--rw-r--r--   0 runner    (1001) docker     (127)    13327 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.401136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/resources/IPAsset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/resources/License.py
--rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/resources/Royalty.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.401136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/scripts/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/scripts/config_impl.json
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/scripts/generate_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/scripts/generate_client_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/story_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.401136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/utils/license_terms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/utils/transaction_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.397136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-24 01:31:28.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-24 01:31:28.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 01:31:28.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-24 01:31:28.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-24 01:31:28.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:24.858859 story_protocol_python_sdk-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-24 18:31:24.858859 story_protocol_python_sdk-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 18:31:24.858859 story_protocol_python_sdk-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-24 18:31:24.000000 story_protocol_python_sdk-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:24.846859 story_protocol_python_sdk-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:24.850859 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:24.850859 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:24.850859 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/IPAssetRegistry/
+-rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/IPAssetRegistry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:24.850859 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/
+-rw-r--r--   0 runner    (1001) docker     (127)    15302 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:24.850859 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/LicenseRegistry/
+-rw-r--r--   0 runner    (1001) docker     (127)    25612 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/LicenseRegistry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:24.850859 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/LicenseToken/
+-rw-r--r--   0 runner    (1001) docker     (127)    21851 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/LicenseToken/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:24.854859 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/LicensingModule/
+-rw-r--r--   0 runner    (1001) docker     (127)    18746 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/LicensingModule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:24.854859 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/PILicenseTemplate/
+-rw-r--r--   0 runner    (1001) docker     (127)    25040 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/PILicenseTemplate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:24.854859 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/RoyaltyModule/
+-rw-r--r--   0 runner    (1001) docker     (127)    15228 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/RoyaltyModule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:24.854859 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/
+-rw-r--r--   0 runner    (1001) docker     (127)    13327 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:24.854859 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/resources/IPAsset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/resources/License.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/resources/Royalty.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:24.854859 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/scripts/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/scripts/config_impl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/scripts/generate_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/scripts/generate_client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/story_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:24.858859 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/utils/license_terms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-24 18:31:21.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/utils/transaction_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:31:24.858859 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-24 18:31:24.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-24 18:31:24.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 18:31:24.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-24 18:31:24.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-24 18:31:24.000000 story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk.egg-info/top_level.txt
```

### Comparing `story_protocol_python_sdk-0.2.2/LICENSE` & `story_protocol_python_sdk-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/PKG-INFO` & `story_protocol_python_sdk-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: story_protocol_python_sdk
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python SDK for interacting with the Story Protocol.
 Home-page: https://github.com/storyprotocol/python-sdk
 Author: Andrew Chung
 Author-email: andrew@storyprotocol.xyz
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: web3>=5.0.0
+Requires-Dist: pytest
+Requires-Dist: python-dotenv
 
 # Story Protocol SDK
 
 Welcome to the documents for Story Protocol Python SDK. The Python SDK provides the APIs for developers to build applications with Story Protocol. By using the SDK, developers can create the resources like IP assets and perform actions to interact with the resource.
 
 ## How to use Story Protocol SDK in Your Project
 
@@ -86,9 +88,7 @@
 to discuss what you would like to change. Details see: [CONTRIBUTING](/CONTRIBUTING.md)
 
 Please make sure to update tests as appropriate.
 
 ## License
 
 [MIT License](/LICENSE.md)
-
-
```

### Comparing `story_protocol_python_sdk-0.2.2/README.md` & `story_protocol_python_sdk-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/setup.py` & `story_protocol_python_sdk-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='story_protocol_python_sdk',
-    version='0.2.2',
+    version='0.2.3',
     packages=find_packages(where='src', exclude=["tests"]),
     package_dir={'': 'src'},
     install_requires=[
         'web3>=5.0.0',
         'pytest',
         'python-dotenv'
     ],
```

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/resources/IPAsset.py` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/resources/IPAsset.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/resources/License.py` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/resources/License.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/resources/Royalty.py` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/resources/Royalty.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/scripts/config.json` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/scripts/config.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/scripts/generate_client.py` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/scripts/generate_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/scripts/generate_client_impl.py` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/scripts/generate_client_impl.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/story_client.py` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/story_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/utils/license_terms.py` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/utils/license_terms.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/utils/transaction_utils.py` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk/utils/transaction_utils.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk.egg-info/PKG-INFO` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
-Name: story-protocol-python-sdk
-Version: 0.2.2
+Name: story_protocol_python_sdk
+Version: 0.2.3
 Summary: A Python SDK for interacting with the Story Protocol.
 Home-page: https://github.com/storyprotocol/python-sdk
 Author: Andrew Chung
 Author-email: andrew@storyprotocol.xyz
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: web3>=5.0.0
+Requires-Dist: pytest
+Requires-Dist: python-dotenv
 
 # Story Protocol SDK
 
 Welcome to the documents for Story Protocol Python SDK. The Python SDK provides the APIs for developers to build applications with Story Protocol. By using the SDK, developers can create the resources like IP assets and perform actions to interact with the resource.
 
 ## How to use Story Protocol SDK in Your Project
 
@@ -86,9 +88,7 @@
 to discuss what you would like to change. Details see: [CONTRIBUTING](/CONTRIBUTING.md)
 
 Please make sure to update tests as appropriate.
 
 ## License
 
 [MIT License](/LICENSE.md)
-
-
```

### Comparing `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk.egg-info/SOURCES.txt` & `story_protocol_python_sdk-0.2.3/src/story_protocol_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


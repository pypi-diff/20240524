# Comparing `tmp/story_protocol_python_sdk-0.2.1.tar.gz` & `tmp/story_protocol_python_sdk-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "story_protocol_python_sdk-0.2.1.tar", last modified: Thu May 23 20:54:28 2024, max compression
+gzip compressed data, was "story_protocol_python_sdk-0.2.2.tar", last modified: Fri May 24 01:31:28 2024, max compression
```

## Comparing `story_protocol_python_sdk-0.2.1.tar` & `story_protocol_python_sdk-0.2.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 20:54:28.046492 story_protocol_python_sdk-0.2.1/
--rw-rw-rw-   0        0        0     1092 2024-05-14 01:32:03.000000 story_protocol_python_sdk-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      219 2024-05-23 01:32:43.000000 story_protocol_python_sdk-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3430 2024-05-23 20:54:28.045492 story_protocol_python_sdk-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2841 2024-05-23 02:26:36.000000 story_protocol_python_sdk-0.2.1/README.md
--rw-rw-rw-   0        0        0        0 2024-05-15 18:58:37.000000 story_protocol_python_sdk-0.2.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 20:54:28.046492 story_protocol_python_sdk-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      905 2024-05-23 20:54:25.000000 story_protocol_python_sdk-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:54:27.963493 story_protocol_python_sdk-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 20:54:27.976494 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/
--rw-rw-rw-   0        0        0      221 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:54:27.999493 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/
-drwxrwxrwx   0        0        0        0 2024-05-23 20:54:28.002493 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/IPAssetRegistry/
--rw-rw-rw-   0        0        0    13409 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json
--rw-rw-rw-   0        0        0     4546 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/IPAssetRegistry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:54:28.006493 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/
--rw-rw-rw-   0        0        0    16117 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
--rw-rw-rw-   0        0        0     1761 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:54:28.009493 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/LicenseRegistry/
--rw-rw-rw-   0        0        0    26905 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json
--rw-rw-rw-   0        0        0     4230 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/LicenseRegistry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:54:28.013494 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/LicenseToken/
--rw-rw-rw-   0        0        0    23007 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json
--rw-rw-rw-   0        0        0     1159 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/LicenseToken/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:54:28.017494 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/LicensingModule/
--rw-rw-rw-   0        0        0    19697 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json
--rw-rw-rw-   0        0        0     5246 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/LicensingModule/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:54:28.021493 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/PILicenseTemplate/
--rw-rw-rw-   0        0        0    26246 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json
--rw-rw-rw-   0        0        0     4625 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/PILicenseTemplate/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:54:28.025492 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/RoyaltyModule/
--rw-rw-rw-   0        0        0    16029 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json
--rw-rw-rw-   0        0        0     1489 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/RoyaltyModule/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:54:28.028494 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/
--rw-rw-rw-   0        0        0    14037 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
--rw-rw-rw-   0        0        0     1183 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:54:28.034492 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/resources/
--rw-rw-rw-   0        0        0     5472 2024-05-23 18:37:04.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/resources/IPAsset.py
--rw-rw-rw-   0        0        0    10540 2024-05-23 20:53:55.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/resources/License.py
--rw-rw-rw-   0        0        0     8542 2024-05-23 20:29:32.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/resources/Royalty.py
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:54:28.040493 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/scripts/
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/scripts/__init__.py
--rw-rw-rw-   0        0        0     3539 2024-05-23 01:34:07.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/scripts/config.json
--rw-rw-rw-   0        0        0      426 2024-05-23 01:34:07.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/scripts/config_impl.json
--rw-rw-rw-   0        0        0     7361 2024-05-23 01:34:07.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/scripts/generate_client.py
--rw-rw-rw-   0        0        0     5288 2024-05-23 01:34:07.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/scripts/generate_client_impl.py
--rw-rw-rw-   0        0        0     1426 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/story_client.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:54:28.043492 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/utils/
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0     2444 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/utils/license_terms.py
--rw-rw-rw-   0        0        0     1449 2024-05-23 18:37:10.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/utils/transaction_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:54:27.998492 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk.egg-info/
--rw-rw-rw-   0        0        0     3430 2024-05-23 20:54:27.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2767 2024-05-23 20:54:27.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 20:54:27.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-23 20:54:27.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-23 20:54:27.000000 story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.401136 story_protocol_python_sdk-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-24 01:31:28.401136 story_protocol_python_sdk-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 01:31:28.401136 story_protocol_python_sdk-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.393136 story_protocol_python_sdk-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.397136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.397136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.397136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/
+-rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.397136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/
+-rw-r--r--   0 runner    (1001) docker     (127)    15302 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.397136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseRegistry/
+-rw-r--r--   0 runner    (1001) docker     (127)    25612 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseRegistry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.397136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseToken/
+-rw-r--r--   0 runner    (1001) docker     (127)    21851 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseToken/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.397136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicensingModule/
+-rw-r--r--   0 runner    (1001) docker     (127)    18746 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicensingModule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.401136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/
+-rw-r--r--   0 runner    (1001) docker     (127)    25040 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.401136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyModule/
+-rw-r--r--   0 runner    (1001) docker     (127)    15228 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyModule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.401136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/
+-rw-r--r--   0 runner    (1001) docker     (127)    13327 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.401136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/resources/IPAsset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/resources/License.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/resources/Royalty.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.401136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/scripts/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/scripts/config_impl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/scripts/generate_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/scripts/generate_client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/story_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.401136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/utils/license_terms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-24 01:31:25.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/utils/transaction_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:31:28.397136 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-24 01:31:28.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-24 01:31:28.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 01:31:28.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-24 01:31:28.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-24 01:31:28.000000 story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk.egg-info/top_level.txt
```

### Comparing `story_protocol_python_sdk-0.2.1/LICENSE` & `story_protocol_python_sdk-0.2.2/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Story Protocol
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Story Protocol
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `story_protocol_python_sdk-0.2.1/PKG-INFO` & `story_protocol_python_sdk-0.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-Metadata-Version: 2.1
-Name: story_protocol_python_sdk
-Version: 0.2.1
-Summary: A Python SDK for interacting with the Story Protocol.
-Home-page: https://github.com/storyprotocol/python-sdk
-Author: Andrew Chung
-Author-email: andrew@storyprotocol.xyz
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: web3>=5.0.0
-Requires-Dist: pytest
-Requires-Dist: python-dotenv
-
-# Story Protocol SDK
-
-Welcome to the documents for Story Protocol Python SDK. The Python SDK provides the APIs for developers to build applications with Story Protocol. By using the SDK, developers can create the resources like IP assets and perform actions to interact with the resource.
-
-## How to use Story Protocol SDK in Your Project
-
-### Install Story Protocol core SDK
-
-Suppose you already have a node project or created a new node project. First, you need to install `story_protocol_python_sdk` in your project. You can use one of the following command to install the package:
-
-Use `pip`:
-
-```
-pip install story_protocol_python_sdk web3
-```
-
-Besides the Story Protocol SDK package `story_protocol_python_sdk`, we also require the package `web3` (https://pypi.org/project/web3/) to access the DeFi wallet accounts.
-
-# Initiate SDK Client
-
-Next we can initiate the SDK Client by first setting up our wallet and then the client itself.
-
-## Set up your wallet
-
-The SDK supports using `web3` for initiating SDK client. Create a Python file and write the following code to initiate the client with a private key:
-
-> :information-source: Make sure to have WALLET_PRIVATE_KEY set up in your .env file.
-
-```Python main.py
-import os
-from dotenv import load_dotenv
-from web3 import Web3
-
-load_dotenv()
-private_key = os.getenv('WALLET_PRIVATE_KEY')
-rpc_url = os.getenv('RPC_PROVIDER_URL')
-
-# Initialize Web3
-web3 = Web3(Web3.HTTPProvider(rpc_url))
-
-# Set up the account with the private key
-account = web3.eth.account.from_key(private_key)
-```
-
-The preceding code created the `account` object for creating the SDK client.
-
-## Set up SDK client
-
-To set up the SDK client, import `StoryClient` from `story_protocol_python_sdk`. Write the following code, utilizing the `account` we created previously.
-
-> :information-source: Make sure to have RPC_PROVIDER_URL for your desired chain set up in your .env file. We recommend using the Sepolia network with `RPC_PROVIDER_URL=https://rpc.ankr.com/eth_sepolia`.
-
-```Python main.py
-from story_protocol_python_sdk import StoryClient
-
-# Create StoryClient instance
-sepolia_chain_id = 11155111
-story_client = StoryClient(web3, account, sepolia_chain_id)
-```
-
-## Release
-
-| Package                         | Description                                    |
-| :------------------------------ | :--------------------------------------------- |
-| [story_protocol_python_sdk](./src/story_protocol_python_sdk) | A Python SDK for interacting with the Story Protocol. |
-
-## Contributing
-
-Pull requests are welcome. For major changes, please open an issue first
-to discuss what you would like to change. Details see: [CONTRIBUTING](/CONTRIBUTING.md)
-
-Please make sure to update tests as appropriate.
-
-## License
-
-[MIT License](/LICENSE.md)
+Metadata-Version: 2.1
+Name: story_protocol_python_sdk
+Version: 0.2.2
+Summary: A Python SDK for interacting with the Story Protocol.
+Home-page: https://github.com/storyprotocol/python-sdk
+Author: Andrew Chung
+Author-email: andrew@storyprotocol.xyz
+License: MIT
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Story Protocol SDK
+
+Welcome to the documents for Story Protocol Python SDK. The Python SDK provides the APIs for developers to build applications with Story Protocol. By using the SDK, developers can create the resources like IP assets and perform actions to interact with the resource.
+
+## How to use Story Protocol SDK in Your Project
+
+### Install Story Protocol core SDK
+
+Suppose you already have a node project or created a new node project. First, you need to install `story_protocol_python_sdk` in your project. You can use one of the following command to install the package:
+
+Use `pip`:
+
+```
+pip install story_protocol_python_sdk web3
+```
+
+Besides the Story Protocol SDK package `story_protocol_python_sdk`, we also require the package `web3` (https://pypi.org/project/web3/) to access the DeFi wallet accounts.
+
+# Initiate SDK Client
+
+Next we can initiate the SDK Client by first setting up our wallet and then the client itself.
+
+## Set up your wallet
+
+The SDK supports using `web3` for initiating SDK client. Create a Python file and write the following code to initiate the client with a private key:
+
+> :information-source: Make sure to have WALLET_PRIVATE_KEY set up in your .env file.
+
+```Python main.py
+import os
+from dotenv import load_dotenv
+from web3 import Web3
+
+load_dotenv()
+private_key = os.getenv('WALLET_PRIVATE_KEY')
+rpc_url = os.getenv('RPC_PROVIDER_URL')
+
+# Initialize Web3
+web3 = Web3(Web3.HTTPProvider(rpc_url))
+
+# Set up the account with the private key
+account = web3.eth.account.from_key(private_key)
+```
+
+The preceding code created the `account` object for creating the SDK client.
+
+## Set up SDK client
+
+To set up the SDK client, import `StoryClient` from `story_protocol_python_sdk`. Write the following code, utilizing the `account` we created previously.
+
+> :information-source: Make sure to have RPC_PROVIDER_URL for your desired chain set up in your .env file. We recommend using the Sepolia network with `RPC_PROVIDER_URL=https://rpc.ankr.com/eth_sepolia`.
+
+```Python main.py
+from story_protocol_python_sdk import StoryClient
+
+# Create StoryClient instance
+sepolia_chain_id = 11155111
+story_client = StoryClient(web3, account, sepolia_chain_id)
+```
+
+## Release
+
+| Package                         | Description                                    |
+| :------------------------------ | :--------------------------------------------- |
+| [story_protocol_python_sdk](./src/story_protocol_python_sdk) | A Python SDK for interacting with the Story Protocol. |
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first
+to discuss what you would like to change. Details see: [CONTRIBUTING](/CONTRIBUTING.md)
+
+Please make sure to update tests as appropriate.
+
+## License
+
+[MIT License](/LICENSE.md)
+
+
```

### Comparing `story_protocol_python_sdk-0.2.1/README.md` & `story_protocol_python_sdk-0.2.2/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-# Story Protocol SDK
-
-Welcome to the documents for Story Protocol Python SDK. The Python SDK provides the APIs for developers to build applications with Story Protocol. By using the SDK, developers can create the resources like IP assets and perform actions to interact with the resource.
-
-## How to use Story Protocol SDK in Your Project
-
-### Install Story Protocol core SDK
-
-Suppose you already have a node project or created a new node project. First, you need to install `story_protocol_python_sdk` in your project. You can use one of the following command to install the package:
-
-Use `pip`:
-
-```
-pip install story_protocol_python_sdk web3
-```
-
-Besides the Story Protocol SDK package `story_protocol_python_sdk`, we also require the package `web3` (https://pypi.org/project/web3/) to access the DeFi wallet accounts.
-
-# Initiate SDK Client
-
-Next we can initiate the SDK Client by first setting up our wallet and then the client itself.
-
-## Set up your wallet
-
-The SDK supports using `web3` for initiating SDK client. Create a Python file and write the following code to initiate the client with a private key:
-
-> :information-source: Make sure to have WALLET_PRIVATE_KEY set up in your .env file.
-
-```Python main.py
-import os
-from dotenv import load_dotenv
-from web3 import Web3
-
-load_dotenv()
-private_key = os.getenv('WALLET_PRIVATE_KEY')
-rpc_url = os.getenv('RPC_PROVIDER_URL')
-
-# Initialize Web3
-web3 = Web3(Web3.HTTPProvider(rpc_url))
-
-# Set up the account with the private key
-account = web3.eth.account.from_key(private_key)
-```
-
-The preceding code created the `account` object for creating the SDK client.
-
-## Set up SDK client
-
-To set up the SDK client, import `StoryClient` from `story_protocol_python_sdk`. Write the following code, utilizing the `account` we created previously.
-
-> :information-source: Make sure to have RPC_PROVIDER_URL for your desired chain set up in your .env file. We recommend using the Sepolia network with `RPC_PROVIDER_URL=https://rpc.ankr.com/eth_sepolia`.
-
-```Python main.py
-from story_protocol_python_sdk import StoryClient
-
-# Create StoryClient instance
-sepolia_chain_id = 11155111
-story_client = StoryClient(web3, account, sepolia_chain_id)
-```
-
-## Release
-
-| Package                         | Description                                    |
-| :------------------------------ | :--------------------------------------------- |
-| [story_protocol_python_sdk](./src/story_protocol_python_sdk) | A Python SDK for interacting with the Story Protocol. |
-
-## Contributing
-
-Pull requests are welcome. For major changes, please open an issue first
-to discuss what you would like to change. Details see: [CONTRIBUTING](/CONTRIBUTING.md)
-
-Please make sure to update tests as appropriate.
-
-## License
-
-[MIT License](/LICENSE.md)
+# Story Protocol SDK
+
+Welcome to the documents for Story Protocol Python SDK. The Python SDK provides the APIs for developers to build applications with Story Protocol. By using the SDK, developers can create the resources like IP assets and perform actions to interact with the resource.
+
+## How to use Story Protocol SDK in Your Project
+
+### Install Story Protocol core SDK
+
+Suppose you already have a node project or created a new node project. First, you need to install `story_protocol_python_sdk` in your project. You can use one of the following command to install the package:
+
+Use `pip`:
+
+```
+pip install story_protocol_python_sdk web3
+```
+
+Besides the Story Protocol SDK package `story_protocol_python_sdk`, we also require the package `web3` (https://pypi.org/project/web3/) to access the DeFi wallet accounts.
+
+# Initiate SDK Client
+
+Next we can initiate the SDK Client by first setting up our wallet and then the client itself.
+
+## Set up your wallet
+
+The SDK supports using `web3` for initiating SDK client. Create a Python file and write the following code to initiate the client with a private key:
+
+> :information-source: Make sure to have WALLET_PRIVATE_KEY set up in your .env file.
+
+```Python main.py
+import os
+from dotenv import load_dotenv
+from web3 import Web3
+
+load_dotenv()
+private_key = os.getenv('WALLET_PRIVATE_KEY')
+rpc_url = os.getenv('RPC_PROVIDER_URL')
+
+# Initialize Web3
+web3 = Web3(Web3.HTTPProvider(rpc_url))
+
+# Set up the account with the private key
+account = web3.eth.account.from_key(private_key)
+```
+
+The preceding code created the `account` object for creating the SDK client.
+
+## Set up SDK client
+
+To set up the SDK client, import `StoryClient` from `story_protocol_python_sdk`. Write the following code, utilizing the `account` we created previously.
+
+> :information-source: Make sure to have RPC_PROVIDER_URL for your desired chain set up in your .env file. We recommend using the Sepolia network with `RPC_PROVIDER_URL=https://rpc.ankr.com/eth_sepolia`.
+
+```Python main.py
+from story_protocol_python_sdk import StoryClient
+
+# Create StoryClient instance
+sepolia_chain_id = 11155111
+story_client = StoryClient(web3, account, sepolia_chain_id)
+```
+
+## Release
+
+| Package                         | Description                                    |
+| :------------------------------ | :--------------------------------------------- |
+| [story_protocol_python_sdk](./src/story_protocol_python_sdk) | A Python SDK for interacting with the Story Protocol. |
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first
+to discuss what you would like to change. Details see: [CONTRIBUTING](/CONTRIBUTING.md)
+
+Please make sure to update tests as appropriate.
+
+## License
+
+[MIT License](/LICENSE.md)
```

### Comparing `story_protocol_python_sdk-0.2.1/setup.py` & `story_protocol_python_sdk-0.2.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from setuptools import setup, find_packages
-
-setup(
-    name='story_protocol_python_sdk',
-    version='0.2.1',
-    packages=find_packages(where='src', exclude=["tests"]),
-    package_dir={'': 'src'},
-    install_requires=[
-        'web3>=5.0.0',
-        'pytest',
-        'python-dotenv'
-    ],
-    include_package_data=True,  # Ensure package data is included
-    url='https://github.com/storyprotocol/python-sdk',
-    license='MIT',
-    author='Andrew Chung',
-    author_email='andrew@storyprotocol.xyz',
-    description='A Python SDK for interacting with the Story Protocol.',
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
-    classifiers=[
-        'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-    ],
-    python_requires='>=3.10',
-)
+from setuptools import setup, find_packages
+
+setup(
+    name='story_protocol_python_sdk',
+    version='0.2.2',
+    packages=find_packages(where='src', exclude=["tests"]),
+    package_dir={'': 'src'},
+    install_requires=[
+        'web3>=5.0.0',
+        'pytest',
+        'python-dotenv'
+    ],
+    include_package_data=True,  # Ensure package data is included
+    url='https://github.com/storyprotocol/python-sdk',
+    license='MIT',
+    author='Andrew Chung',
+    author_email='andrew@storyprotocol.xyz',
+    description='A Python SDK for interacting with the Story Protocol.',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
+    classifiers=[
+        'Programming Language :: Python :: 3',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+    ],
+    python_requires='>=3.10',
+)
```

### Comparing `story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py` & `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-
-import json
-import os
-from web3 import Web3
-
-class IpRoyaltyVaultImplClient:
-    def __init__(self, web3: Web3, contract_address=None):
-        self.web3 = web3
-        abi_path = os.path.join(os.path.dirname(__file__), 'IpRoyaltyVaultImpl.json')
-        with open(abi_path, 'r') as abi_file:
-            abi = json.load(abi_file)
-        self.contract = self.web3.eth.contract(address=contract_address, abi=abi)
-    
-    def claimRevenueBySnapshotBatch(self, snapshotIds, token):
-        
-        return self.contract.functions.claimRevenueBySnapshotBatch(snapshotIds, token).transact()
-        
-    def build_claimRevenueBySnapshotBatch_transaction(self, snapshotIds, token, tx_params):
-        return self.contract.functions.claimRevenueBySnapshotBatch(snapshotIds, token).build_transaction(tx_params)
-    
-    
-    def collectRoyaltyTokens(self, ancestorIpId):
-        
-        return self.contract.functions.collectRoyaltyTokens(ancestorIpId).transact()
-        
-    def build_collectRoyaltyTokens_transaction(self, ancestorIpId, tx_params):
-        return self.contract.functions.collectRoyaltyTokens(ancestorIpId).build_transaction(tx_params)
-    
-    
-    def snapshot(self, ):
-        
-        return self.contract.functions.snapshot().transact()
-        
-    def build_snapshot_transaction(self, tx_params):
-        return self.contract.functions.snapshot().build_transaction(tx_params)
-    
-    
-    def claimableRevenue(self, account, snapshotId, token):
-        
-        return self.contract.functions.claimableRevenue(account, snapshotId, token).call()
-        
-    
-    def unclaimedRoyaltyTokens(self, ):
-        
-        return self.contract.functions.unclaimedRoyaltyTokens().call()
-        
+
+import json
+import os
+from web3 import Web3
+
+class IpRoyaltyVaultImplClient:
+    def __init__(self, web3: Web3, contract_address=None):
+        self.web3 = web3
+        abi_path = os.path.join(os.path.dirname(__file__), 'IpRoyaltyVaultImpl.json')
+        with open(abi_path, 'r') as abi_file:
+            abi = json.load(abi_file)
+        self.contract = self.web3.eth.contract(address=contract_address, abi=abi)
+    
+    def claimRevenueBySnapshotBatch(self, snapshotIds, token):
+        
+        return self.contract.functions.claimRevenueBySnapshotBatch(snapshotIds, token).transact()
+        
+    def build_claimRevenueBySnapshotBatch_transaction(self, snapshotIds, token, tx_params):
+        return self.contract.functions.claimRevenueBySnapshotBatch(snapshotIds, token).build_transaction(tx_params)
+    
+    
+    def collectRoyaltyTokens(self, ancestorIpId):
+        
+        return self.contract.functions.collectRoyaltyTokens(ancestorIpId).transact()
+        
+    def build_collectRoyaltyTokens_transaction(self, ancestorIpId, tx_params):
+        return self.contract.functions.collectRoyaltyTokens(ancestorIpId).build_transaction(tx_params)
+    
+    
+    def snapshot(self, ):
+        
+        return self.contract.functions.snapshot().transact()
+        
+    def build_snapshot_transaction(self, tx_params):
+        return self.contract.functions.snapshot().build_transaction(tx_params)
+    
+    
+    def claimableRevenue(self, account, snapshotId, token):
+        
+        return self.contract.functions.claimableRevenue(account, snapshotId, token).call()
+        
+    
+    def unclaimedRoyaltyTokens(self, ):
+        
+        return self.contract.functions.unclaimedRoyaltyTokens().call()
+
```

### Comparing `story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py` & `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-
-import json
-import os
-from web3 import Web3
-
-class LicenseRegistryClient:
-    def __init__(self, web3: Web3):
-        self.web3 = web3
-        # Assuming config.json is located at the root of the project
-        config_path = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', '..', 'scripts', 'config.json'))
-        with open(config_path, 'r') as config_file:
-            config = json.load(config_file)
-        contract_address = None
-        for contract in config['contracts']:
-            if contract['contract_name'] == 'LicenseRegistry':
-                contract_address = contract['contract_address']
-                break
-        if not contract_address:
-            raise ValueError(f"Contract address for LicenseRegistry not found in config.json")
-        abi_path = os.path.join(os.path.dirname(__file__), 'LicenseRegistry.json')
-        with open(abi_path, 'r') as abi_file:
-            abi = json.load(abi_file)
-        self.contract = self.web3.eth.contract(address=contract_address, abi=abi)
-    
-    def authority(self, ):
-        
-        return self.contract.functions.authority().call()
-        
-    
-    def exists(self, licenseTemplate, licenseTermsId):
-        
-        return self.contract.functions.exists(licenseTemplate, licenseTermsId).call()
-        
-    
-    def getAttachedLicenseTerms(self, ipId, index):
-        
-        return self.contract.functions.getAttachedLicenseTerms(ipId, index).call()
-        
-    
-    def getAttachedLicenseTermsCount(self, ipId):
-        
-        return self.contract.functions.getAttachedLicenseTermsCount(ipId).call()
-        
-    
-    def getDefaultLicenseTerms(self, ):
-        
-        return self.contract.functions.getDefaultLicenseTerms().call()
-        
-    
-    def getDerivativeIp(self, parentIpId, index):
-        
-        return self.contract.functions.getDerivativeIp(parentIpId, index).call()
-        
-    
-    def getDerivativeIpCount(self, parentIpId):
-        
-        return self.contract.functions.getDerivativeIpCount(parentIpId).call()
-        
-    
-    def getExpireTime(self, ipId):
-        
-        return self.contract.functions.getExpireTime(ipId).call()
-        
-    
-    def getLicensingConfig(self, ipId, licenseTemplate, licenseTermsId):
-        
-        return self.contract.functions.getLicensingConfig(ipId, licenseTemplate, licenseTermsId).call()
-        
-    
-    def getParentIp(self, childIpId, index):
-        
-        return self.contract.functions.getParentIp(childIpId, index).call()
-        
-    
-    def getParentIpCount(self, childIpId):
-        
-        return self.contract.functions.getParentIpCount(childIpId).call()
-        
-    
-    def hasDerivativeIps(self, parentIpId):
-        
-        return self.contract.functions.hasDerivativeIps(parentIpId).call()
-        
-    
-    def hasIpAttachedLicenseTerms(self, ipId, licenseTemplate, licenseTermsId):
-        
-        return self.contract.functions.hasIpAttachedLicenseTerms(ipId, licenseTemplate, licenseTermsId).call()
-        
-    
-    def isConsumingScheduledOp(self, ):
-        
-        return self.contract.functions.isConsumingScheduledOp().call()
-        
-    
-    def isDerivativeIp(self, childIpId):
-        
-        return self.contract.functions.isDerivativeIp(childIpId).call()
-        
-    
-    def isExpiredNow(self, ipId):
-        
-        return self.contract.functions.isExpiredNow(ipId).call()
-        
-    
-    def isParentIp(self, parentIpId, childIpId):
-        
-        return self.contract.functions.isParentIp(parentIpId, childIpId).call()
-        
-    
-    def isRegisteredLicenseTemplate(self, licenseTemplate):
-        
-        return self.contract.functions.isRegisteredLicenseTemplate(licenseTemplate).call()
-        
-    
-    def proxiableUUID(self, ):
-        
-        return self.contract.functions.proxiableUUID().call()
-        
-    
-    def verifyMintLicenseToken(self, licensorIpId, licenseTemplate, licenseTermsId, isMintedByIpOwner):
-        
-        return self.contract.functions.verifyMintLicenseToken(licensorIpId, licenseTemplate, licenseTermsId, isMintedByIpOwner).call()
-        
+
+import json
+import os
+from web3 import Web3
+
+class LicenseRegistryClient:
+    def __init__(self, web3: Web3):
+        self.web3 = web3
+        # Assuming config.json is located at the root of the project
+        config_path = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', '..', 'scripts', 'config.json'))
+        with open(config_path, 'r') as config_file:
+            config = json.load(config_file)
+        contract_address = None
+        for contract in config['contracts']:
+            if contract['contract_name'] == 'LicenseRegistry':
+                contract_address = contract['contract_address']
+                break
+        if not contract_address:
+            raise ValueError(f"Contract address for LicenseRegistry not found in config.json")
+        abi_path = os.path.join(os.path.dirname(__file__), 'LicenseRegistry.json')
+        with open(abi_path, 'r') as abi_file:
+            abi = json.load(abi_file)
+        self.contract = self.web3.eth.contract(address=contract_address, abi=abi)
+    
+    def authority(self, ):
+        
+        return self.contract.functions.authority().call()
+        
+    
+    def exists(self, licenseTemplate, licenseTermsId):
+        
+        return self.contract.functions.exists(licenseTemplate, licenseTermsId).call()
+        
+    
+    def getAttachedLicenseTerms(self, ipId, index):
+        
+        return self.contract.functions.getAttachedLicenseTerms(ipId, index).call()
+        
+    
+    def getAttachedLicenseTermsCount(self, ipId):
+        
+        return self.contract.functions.getAttachedLicenseTermsCount(ipId).call()
+        
+    
+    def getDefaultLicenseTerms(self, ):
+        
+        return self.contract.functions.getDefaultLicenseTerms().call()
+        
+    
+    def getDerivativeIp(self, parentIpId, index):
+        
+        return self.contract.functions.getDerivativeIp(parentIpId, index).call()
+        
+    
+    def getDerivativeIpCount(self, parentIpId):
+        
+        return self.contract.functions.getDerivativeIpCount(parentIpId).call()
+        
+    
+    def getExpireTime(self, ipId):
+        
+        return self.contract.functions.getExpireTime(ipId).call()
+        
+    
+    def getLicensingConfig(self, ipId, licenseTemplate, licenseTermsId):
+        
+        return self.contract.functions.getLicensingConfig(ipId, licenseTemplate, licenseTermsId).call()
+        
+    
+    def getParentIp(self, childIpId, index):
+        
+        return self.contract.functions.getParentIp(childIpId, index).call()
+        
+    
+    def getParentIpCount(self, childIpId):
+        
+        return self.contract.functions.getParentIpCount(childIpId).call()
+        
+    
+    def hasDerivativeIps(self, parentIpId):
+        
+        return self.contract.functions.hasDerivativeIps(parentIpId).call()
+        
+    
+    def hasIpAttachedLicenseTerms(self, ipId, licenseTemplate, licenseTermsId):
+        
+        return self.contract.functions.hasIpAttachedLicenseTerms(ipId, licenseTemplate, licenseTermsId).call()
+        
+    
+    def isConsumingScheduledOp(self, ):
+        
+        return self.contract.functions.isConsumingScheduledOp().call()
+        
+    
+    def isDerivativeIp(self, childIpId):
+        
+        return self.contract.functions.isDerivativeIp(childIpId).call()
+        
+    
+    def isExpiredNow(self, ipId):
+        
+        return self.contract.functions.isExpiredNow(ipId).call()
+        
+    
+    def isParentIp(self, parentIpId, childIpId):
+        
+        return self.contract.functions.isParentIp(parentIpId, childIpId).call()
+        
+    
+    def isRegisteredLicenseTemplate(self, licenseTemplate):
+        
+        return self.contract.functions.isRegisteredLicenseTemplate(licenseTemplate).call()
+        
+    
+    def proxiableUUID(self, ):
+        
+        return self.contract.functions.proxiableUUID().call()
+        
+    
+    def verifyMintLicenseToken(self, licensorIpId, licenseTemplate, licenseTermsId, isMintedByIpOwner):
+        
+        return self.contract.functions.verifyMintLicenseToken(licensorIpId, licenseTemplate, licenseTermsId, isMintedByIpOwner).call()
+
```

### Comparing `story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py` & `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-
-import json
-import os
-from web3 import Web3
-
-class LicenseTokenClient:
-    def __init__(self, web3: Web3):
-        self.web3 = web3
-        # Assuming config.json is located at the root of the project
-        config_path = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', '..', 'scripts', 'config.json'))
-        with open(config_path, 'r') as config_file:
-            config = json.load(config_file)
-        contract_address = None
-        for contract in config['contracts']:
-            if contract['contract_name'] == 'LicenseToken':
-                contract_address = contract['contract_address']
-                break
-        if not contract_address:
-            raise ValueError(f"Contract address for LicenseToken not found in config.json")
-        abi_path = os.path.join(os.path.dirname(__file__), 'LicenseToken.json')
-        with open(abi_path, 'r') as abi_file:
-            abi = json.load(abi_file)
-        self.contract = self.web3.eth.contract(address=contract_address, abi=abi)
-    
-    def ownerOf(self, tokenId):
-        
-        return self.contract.functions.ownerOf(tokenId).call()
-        
+
+import json
+import os
+from web3 import Web3
+
+class LicenseTokenClient:
+    def __init__(self, web3: Web3):
+        self.web3 = web3
+        # Assuming config.json is located at the root of the project
+        config_path = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', '..', 'scripts', 'config.json'))
+        with open(config_path, 'r') as config_file:
+            config = json.load(config_file)
+        contract_address = None
+        for contract in config['contracts']:
+            if contract['contract_name'] == 'LicenseToken':
+                contract_address = contract['contract_address']
+                break
+        if not contract_address:
+            raise ValueError(f"Contract address for LicenseToken not found in config.json")
+        abi_path = os.path.join(os.path.dirname(__file__), 'LicenseToken.json')
+        with open(abi_path, 'r') as abi_file:
+            abi = json.load(abi_file)
+        self.contract = self.web3.eth.contract(address=contract_address, abi=abi)
+    
+    def ownerOf(self, tokenId):
+        
+        return self.contract.functions.ownerOf(tokenId).call()
+
```

### Comparing `story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py` & `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-
-import json
-import os
-from web3 import Web3
-
-class LicensingModuleClient:
-    def __init__(self, web3: Web3):
-        self.web3 = web3
-        # Assuming config.json is located at the root of the project
-        config_path = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', '..', 'scripts', 'config.json'))
-        with open(config_path, 'r') as config_file:
-            config = json.load(config_file)
-        contract_address = None
-        for contract in config['contracts']:
-            if contract['contract_name'] == 'LicensingModule':
-                contract_address = contract['contract_address']
-                break
-        if not contract_address:
-            raise ValueError(f"Contract address for LicensingModule not found in config.json")
-        abi_path = os.path.join(os.path.dirname(__file__), 'LicensingModule.json')
-        with open(abi_path, 'r') as abi_file:
-            abi = json.load(abi_file)
-        self.contract = self.web3.eth.contract(address=contract_address, abi=abi)
-    
-    def attachLicenseTerms(self, ipId, licenseTemplate, licenseTermsId):
-        
-        return self.contract.functions.attachLicenseTerms(ipId, licenseTemplate, licenseTermsId).transact()
-        
-    def build_attachLicenseTerms_transaction(self, ipId, licenseTemplate, licenseTermsId, tx_params):
-        return self.contract.functions.attachLicenseTerms(ipId, licenseTemplate, licenseTermsId).build_transaction(tx_params)
-    
-    
-    def initialize(self, accessManager):
-        
-        return self.contract.functions.initialize(accessManager).transact()
-        
-    def build_initialize_transaction(self, accessManager, tx_params):
-        return self.contract.functions.initialize(accessManager).build_transaction(tx_params)
-    
-    
-    def mintLicenseTokens(self, licensorIpId, licenseTemplate, licenseTermsId, amount, receiver, royaltyContext):
-        
-        return self.contract.functions.mintLicenseTokens(licensorIpId, licenseTemplate, licenseTermsId, amount, receiver, royaltyContext).transact()
-        
-    def build_mintLicenseTokens_transaction(self, licensorIpId, licenseTemplate, licenseTermsId, amount, receiver, royaltyContext, tx_params):
-        return self.contract.functions.mintLicenseTokens(licensorIpId, licenseTemplate, licenseTermsId, amount, receiver, royaltyContext).build_transaction(tx_params)
-    
-    
-    def pause(self, ):
-        
-        return self.contract.functions.pause().transact()
-        
-    def build_pause_transaction(self, tx_params):
-        return self.contract.functions.pause().build_transaction(tx_params)
-    
-    
-    def registerDerivative(self, childIpId, parentIpIds, licenseTermsIds, licenseTemplate, royaltyContext):
-        
-        return self.contract.functions.registerDerivative(childIpId, parentIpIds, licenseTermsIds, licenseTemplate, royaltyContext).transact()
-        
-    def build_registerDerivative_transaction(self, childIpId, parentIpIds, licenseTermsIds, licenseTemplate, royaltyContext, tx_params):
-        return self.contract.functions.registerDerivative(childIpId, parentIpIds, licenseTermsIds, licenseTemplate, royaltyContext).build_transaction(tx_params)
-    
-    
-    def registerDerivativeWithLicenseTokens(self, childIpId, licenseTokenIds, royaltyContext):
-        
-        return self.contract.functions.registerDerivativeWithLicenseTokens(childIpId, licenseTokenIds, royaltyContext).transact()
-        
-    def build_registerDerivativeWithLicenseTokens_transaction(self, childIpId, licenseTokenIds, royaltyContext, tx_params):
-        return self.contract.functions.registerDerivativeWithLicenseTokens(childIpId, licenseTokenIds, royaltyContext).build_transaction(tx_params)
-    
-    
-    def setAuthority(self, newAuthority):
-        
-        return self.contract.functions.setAuthority(newAuthority).transact()
-        
-    def build_setAuthority_transaction(self, newAuthority, tx_params):
-        return self.contract.functions.setAuthority(newAuthority).build_transaction(tx_params)
-    
-    
-    def setLicensingConfig(self, ipId, licenseTemplate, licenseTermsId, licensingConfig):
-        
-        return self.contract.functions.setLicensingConfig(ipId, licenseTemplate, licenseTermsId, licensingConfig).transact()
-        
-    def build_setLicensingConfig_transaction(self, ipId, licenseTemplate, licenseTermsId, licensingConfig, tx_params):
-        return self.contract.functions.setLicensingConfig(ipId, licenseTemplate, licenseTermsId, licensingConfig).build_transaction(tx_params)
-    
-    
-    def unpause(self, ):
-        
-        return self.contract.functions.unpause().transact()
-        
-    def build_unpause_transaction(self, tx_params):
-        return self.contract.functions.unpause().build_transaction(tx_params)
-    
-    
-    def upgradeToAndCall(self, newImplementation, data):
-        
-        return self.contract.functions.upgradeToAndCall(newImplementation, data).transact()
-        
-    def build_upgradeToAndCall_transaction(self, newImplementation, data, tx_params):
-        return self.contract.functions.upgradeToAndCall(newImplementation, data).build_transaction(tx_params)
-    
+
+import json
+import os
+from web3 import Web3
+
+class LicensingModuleClient:
+    def __init__(self, web3: Web3):
+        self.web3 = web3
+        # Assuming config.json is located at the root of the project
+        config_path = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', '..', 'scripts', 'config.json'))
+        with open(config_path, 'r') as config_file:
+            config = json.load(config_file)
+        contract_address = None
+        for contract in config['contracts']:
+            if contract['contract_name'] == 'LicensingModule':
+                contract_address = contract['contract_address']
+                break
+        if not contract_address:
+            raise ValueError(f"Contract address for LicensingModule not found in config.json")
+        abi_path = os.path.join(os.path.dirname(__file__), 'LicensingModule.json')
+        with open(abi_path, 'r') as abi_file:
+            abi = json.load(abi_file)
+        self.contract = self.web3.eth.contract(address=contract_address, abi=abi)
+    
+    def attachLicenseTerms(self, ipId, licenseTemplate, licenseTermsId):
+        
+        return self.contract.functions.attachLicenseTerms(ipId, licenseTemplate, licenseTermsId).transact()
+        
+    def build_attachLicenseTerms_transaction(self, ipId, licenseTemplate, licenseTermsId, tx_params):
+        return self.contract.functions.attachLicenseTerms(ipId, licenseTemplate, licenseTermsId).build_transaction(tx_params)
+    
+    
+    def initialize(self, accessManager):
+        
+        return self.contract.functions.initialize(accessManager).transact()
+        
+    def build_initialize_transaction(self, accessManager, tx_params):
+        return self.contract.functions.initialize(accessManager).build_transaction(tx_params)
+    
+    
+    def mintLicenseTokens(self, licensorIpId, licenseTemplate, licenseTermsId, amount, receiver, royaltyContext):
+        
+        return self.contract.functions.mintLicenseTokens(licensorIpId, licenseTemplate, licenseTermsId, amount, receiver, royaltyContext).transact()
+        
+    def build_mintLicenseTokens_transaction(self, licensorIpId, licenseTemplate, licenseTermsId, amount, receiver, royaltyContext, tx_params):
+        return self.contract.functions.mintLicenseTokens(licensorIpId, licenseTemplate, licenseTermsId, amount, receiver, royaltyContext).build_transaction(tx_params)
+    
+    
+    def pause(self, ):
+        
+        return self.contract.functions.pause().transact()
+        
+    def build_pause_transaction(self, tx_params):
+        return self.contract.functions.pause().build_transaction(tx_params)
+    
+    
+    def registerDerivative(self, childIpId, parentIpIds, licenseTermsIds, licenseTemplate, royaltyContext):
+        
+        return self.contract.functions.registerDerivative(childIpId, parentIpIds, licenseTermsIds, licenseTemplate, royaltyContext).transact()
+        
+    def build_registerDerivative_transaction(self, childIpId, parentIpIds, licenseTermsIds, licenseTemplate, royaltyContext, tx_params):
+        return self.contract.functions.registerDerivative(childIpId, parentIpIds, licenseTermsIds, licenseTemplate, royaltyContext).build_transaction(tx_params)
+    
+    
+    def registerDerivativeWithLicenseTokens(self, childIpId, licenseTokenIds, royaltyContext):
+        
+        return self.contract.functions.registerDerivativeWithLicenseTokens(childIpId, licenseTokenIds, royaltyContext).transact()
+        
+    def build_registerDerivativeWithLicenseTokens_transaction(self, childIpId, licenseTokenIds, royaltyContext, tx_params):
+        return self.contract.functions.registerDerivativeWithLicenseTokens(childIpId, licenseTokenIds, royaltyContext).build_transaction(tx_params)
+    
+    
+    def setAuthority(self, newAuthority):
+        
+        return self.contract.functions.setAuthority(newAuthority).transact()
+        
+    def build_setAuthority_transaction(self, newAuthority, tx_params):
+        return self.contract.functions.setAuthority(newAuthority).build_transaction(tx_params)
+    
+    
+    def setLicensingConfig(self, ipId, licenseTemplate, licenseTermsId, licensingConfig):
+        
+        return self.contract.functions.setLicensingConfig(ipId, licenseTemplate, licenseTermsId, licensingConfig).transact()
+        
+    def build_setLicensingConfig_transaction(self, ipId, licenseTemplate, licenseTermsId, licensingConfig, tx_params):
+        return self.contract.functions.setLicensingConfig(ipId, licenseTemplate, licenseTermsId, licensingConfig).build_transaction(tx_params)
+    
+    
+    def unpause(self, ):
+        
+        return self.contract.functions.unpause().transact()
+        
+    def build_unpause_transaction(self, tx_params):
+        return self.contract.functions.unpause().build_transaction(tx_params)
+    
+    
+    def upgradeToAndCall(self, newImplementation, data):
+        
+        return self.contract.functions.upgradeToAndCall(newImplementation, data).transact()
+        
+    def build_upgradeToAndCall_transaction(self, newImplementation, data, tx_params):
+        return self.contract.functions.upgradeToAndCall(newImplementation, data).build_transaction(tx_params)
+
```

### Comparing `story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py` & `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-
-import json
-import os
-from web3 import Web3
-
-class PILicenseTemplateClient:
-    def __init__(self, web3: Web3):
-        self.web3 = web3
-        # Assuming config.json is located at the root of the project
-        config_path = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', '..', 'scripts', 'config.json'))
-        with open(config_path, 'r') as config_file:
-            config = json.load(config_file)
-        contract_address = None
-        for contract in config['contracts']:
-            if contract['contract_name'] == 'PILicenseTemplate':
-                contract_address = contract['contract_address']
-                break
-        if not contract_address:
-            raise ValueError(f"Contract address for PILicenseTemplate not found in config.json")
-        abi_path = os.path.join(os.path.dirname(__file__), 'PILicenseTemplate.json')
-        with open(abi_path, 'r') as abi_file:
-            abi = json.load(abi_file)
-        self.contract = self.web3.eth.contract(address=contract_address, abi=abi)
-    
-    def initialize(self, accessManager, name, metadataURI):
-        
-        return self.contract.functions.initialize(accessManager, name, metadataURI).transact()
-        
-    def build_initialize_transaction(self, accessManager, name, metadataURI, tx_params):
-        return self.contract.functions.initialize(accessManager, name, metadataURI).build_transaction(tx_params)
-    
-    
-    def registerLicenseTerms(self, terms):
-        
-        return self.contract.functions.registerLicenseTerms(terms).transact()
-        
-    def build_registerLicenseTerms_transaction(self, terms, tx_params):
-        return self.contract.functions.registerLicenseTerms(terms).build_transaction(tx_params)
-    
-    
-    def setApproval(self, parentIpId, licenseTermsId, childIpId, approved):
-        
-        return self.contract.functions.setApproval(parentIpId, licenseTermsId, childIpId, approved).transact()
-        
-    def build_setApproval_transaction(self, parentIpId, licenseTermsId, childIpId, approved, tx_params):
-        return self.contract.functions.setApproval(parentIpId, licenseTermsId, childIpId, approved).build_transaction(tx_params)
-    
-    
-    def setAuthority(self, newAuthority):
-        
-        return self.contract.functions.setAuthority(newAuthority).transact()
-        
-    def build_setAuthority_transaction(self, newAuthority, tx_params):
-        return self.contract.functions.setAuthority(newAuthority).build_transaction(tx_params)
-    
-    
-    def upgradeToAndCall(self, newImplementation, data):
-        
-        return self.contract.functions.upgradeToAndCall(newImplementation, data).transact()
-        
-    def build_upgradeToAndCall_transaction(self, newImplementation, data, tx_params):
-        return self.contract.functions.upgradeToAndCall(newImplementation, data).build_transaction(tx_params)
-    
-    
-    def verifyRegisterDerivative(self, childIpId, parentIpId, licenseTermsId, licensee):
-        
-        return self.contract.functions.verifyRegisterDerivative(childIpId, parentIpId, licenseTermsId, licensee).transact()
-        
-    def build_verifyRegisterDerivative_transaction(self, childIpId, parentIpId, licenseTermsId, licensee, tx_params):
-        return self.contract.functions.verifyRegisterDerivative(childIpId, parentIpId, licenseTermsId, licensee).build_transaction(tx_params)
-    
-    
-    def verifyRegisterDerivativeForAllParents(self, childIpId, parentIpIds, licenseTermsIds, childIpOwner):
-        
-        return self.contract.functions.verifyRegisterDerivativeForAllParents(childIpId, parentIpIds, licenseTermsIds, childIpOwner).transact()
-        
-    def build_verifyRegisterDerivativeForAllParents_transaction(self, childIpId, parentIpIds, licenseTermsIds, childIpOwner, tx_params):
-        return self.contract.functions.verifyRegisterDerivativeForAllParents(childIpId, parentIpIds, licenseTermsIds, childIpOwner).build_transaction(tx_params)
-    
-    
-    def exists(self, licenseTermsId):
-        
-        return self.contract.functions.exists(licenseTermsId).call()
-        
-    
-    def getLicenseTerms(self, selectedLicenseTermsId):
-        
-        return self.contract.functions.getLicenseTerms(selectedLicenseTermsId).call()
-        
-    
-    def getLicenseTermsId(self, terms):
-        
-        return self.contract.functions.getLicenseTermsId(terms).call()
-        
-    
-    def getRoyaltyPolicy(self, licenseTermsId):
-        
-        return self.contract.functions.getRoyaltyPolicy(licenseTermsId).call()
-        
+
+import json
+import os
+from web3 import Web3
+
+class PILicenseTemplateClient:
+    def __init__(self, web3: Web3):
+        self.web3 = web3
+        # Assuming config.json is located at the root of the project
+        config_path = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', '..', 'scripts', 'config.json'))
+        with open(config_path, 'r') as config_file:
+            config = json.load(config_file)
+        contract_address = None
+        for contract in config['contracts']:
+            if contract['contract_name'] == 'PILicenseTemplate':
+                contract_address = contract['contract_address']
+                break
+        if not contract_address:
+            raise ValueError(f"Contract address for PILicenseTemplate not found in config.json")
+        abi_path = os.path.join(os.path.dirname(__file__), 'PILicenseTemplate.json')
+        with open(abi_path, 'r') as abi_file:
+            abi = json.load(abi_file)
+        self.contract = self.web3.eth.contract(address=contract_address, abi=abi)
+    
+    def initialize(self, accessManager, name, metadataURI):
+        
+        return self.contract.functions.initialize(accessManager, name, metadataURI).transact()
+        
+    def build_initialize_transaction(self, accessManager, name, metadataURI, tx_params):
+        return self.contract.functions.initialize(accessManager, name, metadataURI).build_transaction(tx_params)
+    
+    
+    def registerLicenseTerms(self, terms):
+        
+        return self.contract.functions.registerLicenseTerms(terms).transact()
+        
+    def build_registerLicenseTerms_transaction(self, terms, tx_params):
+        return self.contract.functions.registerLicenseTerms(terms).build_transaction(tx_params)
+    
+    
+    def setApproval(self, parentIpId, licenseTermsId, childIpId, approved):
+        
+        return self.contract.functions.setApproval(parentIpId, licenseTermsId, childIpId, approved).transact()
+        
+    def build_setApproval_transaction(self, parentIpId, licenseTermsId, childIpId, approved, tx_params):
+        return self.contract.functions.setApproval(parentIpId, licenseTermsId, childIpId, approved).build_transaction(tx_params)
+    
+    
+    def setAuthority(self, newAuthority):
+        
+        return self.contract.functions.setAuthority(newAuthority).transact()
+        
+    def build_setAuthority_transaction(self, newAuthority, tx_params):
+        return self.contract.functions.setAuthority(newAuthority).build_transaction(tx_params)
+    
+    
+    def upgradeToAndCall(self, newImplementation, data):
+        
+        return self.contract.functions.upgradeToAndCall(newImplementation, data).transact()
+        
+    def build_upgradeToAndCall_transaction(self, newImplementation, data, tx_params):
+        return self.contract.functions.upgradeToAndCall(newImplementation, data).build_transaction(tx_params)
+    
+    
+    def verifyRegisterDerivative(self, childIpId, parentIpId, licenseTermsId, licensee):
+        
+        return self.contract.functions.verifyRegisterDerivative(childIpId, parentIpId, licenseTermsId, licensee).transact()
+        
+    def build_verifyRegisterDerivative_transaction(self, childIpId, parentIpId, licenseTermsId, licensee, tx_params):
+        return self.contract.functions.verifyRegisterDerivative(childIpId, parentIpId, licenseTermsId, licensee).build_transaction(tx_params)
+    
+    
+    def verifyRegisterDerivativeForAllParents(self, childIpId, parentIpIds, licenseTermsIds, childIpOwner):
+        
+        return self.contract.functions.verifyRegisterDerivativeForAllParents(childIpId, parentIpIds, licenseTermsIds, childIpOwner).transact()
+        
+    def build_verifyRegisterDerivativeForAllParents_transaction(self, childIpId, parentIpIds, licenseTermsIds, childIpOwner, tx_params):
+        return self.contract.functions.verifyRegisterDerivativeForAllParents(childIpId, parentIpIds, licenseTermsIds, childIpOwner).build_transaction(tx_params)
+    
+    
+    def exists(self, licenseTermsId):
+        
+        return self.contract.functions.exists(licenseTermsId).call()
+        
+    
+    def getLicenseTerms(self, selectedLicenseTermsId):
+        
+        return self.contract.functions.getLicenseTerms(selectedLicenseTermsId).call()
+        
+    
+    def getLicenseTermsId(self, terms):
+        
+        return self.contract.functions.getLicenseTermsId(terms).call()
+        
+    
+    def getRoyaltyPolicy(self, licenseTermsId):
+        
+        return self.contract.functions.getRoyaltyPolicy(licenseTermsId).call()
+
```

### Comparing `story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py` & `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-
-import json
-import os
-from web3 import Web3
-
-class RoyaltyModuleClient:
-    def __init__(self, web3: Web3):
-        self.web3 = web3
-        # Assuming config.json is located at the root of the project
-        config_path = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', '..', 'scripts', 'config.json'))
-        with open(config_path, 'r') as config_file:
-            config = json.load(config_file)
-        contract_address = None
-        for contract in config['contracts']:
-            if contract['contract_name'] == 'RoyaltyModule':
-                contract_address = contract['contract_address']
-                break
-        if not contract_address:
-            raise ValueError(f"Contract address for RoyaltyModule not found in config.json")
-        abi_path = os.path.join(os.path.dirname(__file__), 'RoyaltyModule.json')
-        with open(abi_path, 'r') as abi_file:
-            abi = json.load(abi_file)
-        self.contract = self.web3.eth.contract(address=contract_address, abi=abi)
-    
-    def payRoyaltyOnBehalf(self, receiverIpId, payerIpId, token, amount):
-        
-        return self.contract.functions.payRoyaltyOnBehalf(receiverIpId, payerIpId, token, amount).transact()
-        
-    def build_payRoyaltyOnBehalf_transaction(self, receiverIpId, payerIpId, token, amount, tx_params):
-        return self.contract.functions.payRoyaltyOnBehalf(receiverIpId, payerIpId, token, amount).build_transaction(tx_params)
-    
+
+import json
+import os
+from web3 import Web3
+
+class RoyaltyModuleClient:
+    def __init__(self, web3: Web3):
+        self.web3 = web3
+        # Assuming config.json is located at the root of the project
+        config_path = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', '..', 'scripts', 'config.json'))
+        with open(config_path, 'r') as config_file:
+            config = json.load(config_file)
+        contract_address = None
+        for contract in config['contracts']:
+            if contract['contract_name'] == 'RoyaltyModule':
+                contract_address = contract['contract_address']
+                break
+        if not contract_address:
+            raise ValueError(f"Contract address for RoyaltyModule not found in config.json")
+        abi_path = os.path.join(os.path.dirname(__file__), 'RoyaltyModule.json')
+        with open(abi_path, 'r') as abi_file:
+            abi = json.load(abi_file)
+        self.contract = self.web3.eth.contract(address=contract_address, abi=abi)
+    
+    def payRoyaltyOnBehalf(self, receiverIpId, payerIpId, token, amount):
+        
+        return self.contract.functions.payRoyaltyOnBehalf(receiverIpId, payerIpId, token, amount).transact()
+        
+    def build_payRoyaltyOnBehalf_transaction(self, receiverIpId, payerIpId, token, amount, tx_params):
+        return self.contract.functions.payRoyaltyOnBehalf(receiverIpId, payerIpId, token, amount).build_transaction(tx_params)
+
```

### Comparing `story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json` & `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4842615049751244%*

 * *Differences: {'0': "{'inputs': {0: {'name': 'royaltyPolicyLAP'}, 1: {'name': 'disputeModule'}}}",*

 * * '1': "{'name': 'IpRoyaltyVault__AlreadyClaimed'}",*

 * * '10': "{'inputs': {0: {'internalType': 'uint8', 'type': 'uint8'}}}",*

 * * '11': "{'inputs': {1: {'name': 'token'}, insert: [(0, OrderedDict([('indexed', False), "*

 * *       "('internalType', 'address'), ('name', 'claimer'), ('type', 'address')])), (2, "*

 * *       "OrderedDict([('indexed', False), ('internalType', 'uint256'), ('name', 'amount'), ('type', "*

 * *       "'uint256')]))]}, ' […]*

```diff
@@ -1,711 +1,816 @@
 [
     {
         "inputs": [
             {
                 "internalType": "address",
-                "name": "royaltyModule",
+                "name": "royaltyPolicyLAP",
                 "type": "address"
             },
             {
                 "internalType": "address",
-                "name": "licensingModule",
+                "name": "disputeModule",
                 "type": "address"
             }
         ],
         "stateMutability": "nonpayable",
         "type": "constructor"
     },
     {
-        "inputs": [
-            {
-                "internalType": "address",
-                "name": "authority",
-                "type": "address"
-            }
-        ],
-        "name": "AccessManagedInvalidAuthority",
-        "type": "error"
-    },
-    {
-        "inputs": [
-            {
-                "internalType": "address",
-                "name": "caller",
-                "type": "address"
-            },
-            {
-                "internalType": "uint32",
-                "name": "delay",
-                "type": "uint32"
-            }
-        ],
-        "name": "AccessManagedRequiredDelay",
-        "type": "error"
-    },
-    {
-        "inputs": [
-            {
-                "internalType": "address",
-                "name": "caller",
-                "type": "address"
-            }
-        ],
-        "name": "AccessManagedUnauthorized",
-        "type": "error"
-    },
-    {
-        "inputs": [
-            {
-                "internalType": "address",
-                "name": "target",
-                "type": "address"
-            }
-        ],
-        "name": "AddressEmptyCode",
-        "type": "error"
-    },
-    {
-        "inputs": [
-            {
-                "internalType": "address",
-                "name": "account",
-                "type": "address"
-            }
-        ],
-        "name": "AddressInsufficientBalance",
-        "type": "error"
-    },
-    {
-        "inputs": [
-            {
-                "internalType": "address",
-                "name": "implementation",
-                "type": "address"
-            }
-        ],
-        "name": "ERC1967InvalidImplementation",
-        "type": "error"
-    },
-    {
         "inputs": [],
-        "name": "ERC1967NonPayable",
+        "name": "IpRoyaltyVault__AlreadyClaimed",
         "type": "error"
     },
     {
         "inputs": [],
-        "name": "EnforcedPause",
+        "name": "IpRoyaltyVault__ClaimerNotAnAncestor",
         "type": "error"
     },
     {
         "inputs": [],
-        "name": "ExpectedPause",
+        "name": "IpRoyaltyVault__EnforcedPause",
         "type": "error"
     },
     {
         "inputs": [],
-        "name": "FailedInnerCall",
+        "name": "IpRoyaltyVault__IpTagged",
         "type": "error"
     },
     {
         "inputs": [],
-        "name": "InvalidInitialization",
+        "name": "IpRoyaltyVault__NotRoyaltyPolicyLAP",
         "type": "error"
     },
     {
         "inputs": [],
-        "name": "NotInitializing",
+        "name": "IpRoyaltyVault__SnapshotIntervalTooShort",
         "type": "error"
     },
     {
         "inputs": [],
-        "name": "ReentrancyGuardReentrantCall",
+        "name": "IpRoyaltyVault__ZeroDisputeModule",
         "type": "error"
     },
     {
         "inputs": [],
-        "name": "RoyaltyPolicyLAP__AboveAncestorsLimit",
-        "type": "error"
-    },
-    {
-        "inputs": [],
-        "name": "RoyaltyPolicyLAP__AboveParentLimit",
-        "type": "error"
-    },
-    {
-        "inputs": [],
-        "name": "RoyaltyPolicyLAP__AboveRoyaltyStackLimit",
-        "type": "error"
-    },
-    {
-        "inputs": [],
-        "name": "RoyaltyPolicyLAP__InvalidParentRoyaltiesLength",
-        "type": "error"
-    },
-    {
-        "inputs": [],
-        "name": "RoyaltyPolicyLAP__LastPositionNotAbleToMintLicense",
-        "type": "error"
-    },
-    {
-        "inputs": [],
-        "name": "RoyaltyPolicyLAP__NotRoyaltyModule",
-        "type": "error"
-    },
-    {
-        "inputs": [],
-        "name": "RoyaltyPolicyLAP__UnlinkableToParents",
-        "type": "error"
-    },
-    {
-        "inputs": [],
-        "name": "RoyaltyPolicyLAP__ZeroAccessManager",
-        "type": "error"
-    },
-    {
-        "inputs": [],
-        "name": "RoyaltyPolicyLAP__ZeroIpRoyaltyVaultBeacon",
-        "type": "error"
-    },
-    {
-        "inputs": [],
-        "name": "RoyaltyPolicyLAP__ZeroLicensingModule",
-        "type": "error"
-    },
-    {
-        "inputs": [],
-        "name": "RoyaltyPolicyLAP__ZeroRoyaltyModule",
+        "name": "IpRoyaltyVault__ZeroRoyaltyPolicyLAP",
         "type": "error"
     },
     {
+        "anonymous": false,
         "inputs": [
             {
+                "indexed": true,
                 "internalType": "address",
-                "name": "token",
+                "name": "owner",
                 "type": "address"
+            },
+            {
+                "indexed": true,
+                "internalType": "address",
+                "name": "spender",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "value",
+                "type": "uint256"
             }
         ],
-        "name": "SafeERC20FailedOperation",
-        "type": "error"
-    },
-    {
-        "inputs": [],
-        "name": "UUPSUnauthorizedCallContext",
-        "type": "error"
+        "name": "Approval",
+        "type": "event"
     },
     {
+        "anonymous": false,
         "inputs": [
             {
-                "internalType": "bytes32",
-                "name": "slot",
-                "type": "bytes32"
+                "indexed": false,
+                "internalType": "uint8",
+                "name": "version",
+                "type": "uint8"
             }
         ],
-        "name": "UUPSUnsupportedProxiableUUID",
-        "type": "error"
+        "name": "Initialized",
+        "type": "event"
     },
     {
         "anonymous": false,
         "inputs": [
             {
                 "indexed": false,
                 "internalType": "address",
-                "name": "authority",
+                "name": "claimer",
                 "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
             }
         ],
-        "name": "AuthorityUpdated",
+        "name": "RevenueTokenClaimed",
         "type": "event"
     },
     {
         "anonymous": false,
         "inputs": [
             {
                 "indexed": false,
-                "internalType": "uint64",
-                "name": "version",
-                "type": "uint64"
+                "internalType": "address",
+                "name": "ancestorIpId",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "royaltyTokensCollected",
+                "type": "uint256"
             }
         ],
-        "name": "Initialized",
+        "name": "RoyaltyTokensCollected",
         "type": "event"
     },
     {
         "anonymous": false,
         "inputs": [
             {
                 "indexed": false,
-                "internalType": "address",
-                "name": "account",
-                "type": "address"
+                "internalType": "uint256",
+                "name": "id",
+                "type": "uint256"
             }
         ],
-        "name": "Paused",
+        "name": "Snapshot",
         "type": "event"
     },
     {
         "anonymous": false,
         "inputs": [
             {
                 "indexed": false,
-                "internalType": "address",
-                "name": "ipId",
-                "type": "address"
+                "internalType": "uint256",
+                "name": "snapshotId",
+                "type": "uint256"
             },
             {
                 "indexed": false,
-                "internalType": "address",
-                "name": "ipRoyaltyVault",
-                "type": "address"
+                "internalType": "uint256",
+                "name": "snapshotTimestamp",
+                "type": "uint256"
             },
             {
                 "indexed": false,
                 "internalType": "uint32",
-                "name": "royaltyStack",
+                "name": "unclaimedTokens",
                 "type": "uint32"
-            },
-            {
-                "indexed": false,
-                "internalType": "address[]",
-                "name": "targetAncestors",
-                "type": "address[]"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint32[]",
-                "name": "targetRoyaltyAmount",
-                "type": "uint32[]"
             }
         ],
-        "name": "PolicyInitialized",
+        "name": "SnapshotCompleted",
         "type": "event"
     },
     {
         "anonymous": false,
         "inputs": [
             {
-                "indexed": false,
+                "indexed": true,
                 "internalType": "address",
-                "name": "token",
+                "name": "from",
                 "type": "address"
             },
             {
-                "indexed": false,
+                "indexed": true,
                 "internalType": "address",
-                "name": "vault",
+                "name": "to",
                 "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "value",
+                "type": "uint256"
             }
         ],
-        "name": "RevenueTokenAddedToVault",
+        "name": "Transfer",
         "type": "event"
     },
     {
-        "anonymous": false,
-        "inputs": [
+        "inputs": [],
+        "name": "DISPUTE_MODULE",
+        "outputs": [
             {
-                "indexed": false,
-                "internalType": "address",
-                "name": "account",
+                "internalType": "contract IDisputeModule",
+                "name": "",
                 "type": "address"
             }
         ],
-        "name": "Unpaused",
-        "type": "event"
+        "stateMutability": "view",
+        "type": "function"
     },
     {
-        "anonymous": false,
-        "inputs": [
+        "inputs": [],
+        "name": "ROYALTY_POLICY_LAP",
+        "outputs": [
             {
-                "indexed": true,
-                "internalType": "address",
-                "name": "implementation",
+                "internalType": "contract IRoyaltyPolicyLAP",
+                "name": "",
                 "type": "address"
             }
         ],
-        "name": "Upgraded",
-        "type": "event"
+        "stateMutability": "view",
+        "type": "function"
     },
     {
-        "inputs": [],
-        "name": "LICENSING_MODULE",
-        "outputs": [
+        "inputs": [
             {
                 "internalType": "address",
-                "name": "",
+                "name": "token",
                 "type": "address"
             }
         ],
-        "stateMutability": "view",
+        "name": "addIpRoyaltyVaultTokens",
+        "outputs": [
+            {
+                "internalType": "bool",
+                "name": "",
+                "type": "bool"
+            }
+        ],
+        "stateMutability": "nonpayable",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "MAX_ANCESTORS",
+        "inputs": [
+            {
+                "internalType": "address",
+                "name": "owner",
+                "type": "address"
+            },
+            {
+                "internalType": "address",
+                "name": "spender",
+                "type": "address"
+            }
+        ],
+        "name": "allowance",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "",
                 "type": "uint256"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "MAX_PARENTS",
+        "inputs": [
+            {
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            }
+        ],
+        "name": "ancestorsVaultAmount",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "",
                 "type": "uint256"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "ROYALTY_MODULE",
-        "outputs": [
+        "inputs": [
             {
                 "internalType": "address",
-                "name": "",
+                "name": "spender",
                 "type": "address"
+            },
+            {
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
             }
         ],
-        "stateMutability": "view",
+        "name": "approve",
+        "outputs": [
+            {
+                "internalType": "bool",
+                "name": "",
+                "type": "bool"
+            }
+        ],
+        "stateMutability": "nonpayable",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "TOTAL_RT_SUPPLY",
+        "inputs": [
+            {
+                "internalType": "address",
+                "name": "account",
+                "type": "address"
+            }
+        ],
+        "name": "balanceOf",
         "outputs": [
             {
-                "internalType": "uint32",
+                "internalType": "uint256",
                 "name": "",
-                "type": "uint32"
+                "type": "uint256"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "UPGRADE_INTERFACE_VERSION",
+        "inputs": [
+            {
+                "internalType": "address",
+                "name": "account",
+                "type": "address"
+            },
+            {
+                "internalType": "uint256",
+                "name": "snapshotId",
+                "type": "uint256"
+            }
+        ],
+        "name": "balanceOfAt",
         "outputs": [
             {
-                "internalType": "string",
+                "internalType": "uint256",
                 "name": "",
-                "type": "string"
+                "type": "uint256"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "internalType": "uint256[]",
+                "name": "snapshotIds",
+                "type": "uint256[]"
+            },
+            {
                 "internalType": "address",
-                "name": "accessManager",
+                "name": "token",
                 "type": "address"
             }
         ],
-        "name": "__ProtocolPausable_init",
+        "name": "claimRevenueBySnapshotBatch",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "authority",
-        "outputs": [
+        "inputs": [
             {
-                "internalType": "address",
-                "name": "",
-                "type": "address"
+                "internalType": "uint256",
+                "name": "snapshotId",
+                "type": "uint256"
+            },
+            {
+                "internalType": "address[]",
+                "name": "tokenList",
+                "type": "address[]"
             }
         ],
-        "stateMutability": "view",
+        "name": "claimRevenueByTokenBatch",
+        "outputs": [],
+        "stateMutability": "nonpayable",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "getIpRoyaltyVaultBeacon",
-        "outputs": [
+        "inputs": [
             {
                 "internalType": "address",
-                "name": "",
+                "name": "token",
                 "type": "address"
             }
         ],
+        "name": "claimVaultAmount",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "internalType": "uint256",
+                "name": "snapshotId",
+                "type": "uint256"
+            },
+            {
                 "internalType": "address",
-                "name": "ipId",
+                "name": "token",
                 "type": "address"
             }
         ],
-        "name": "getRoyaltyData",
+        "name": "claimableAtSnapshot",
         "outputs": [
             {
-                "internalType": "bool",
+                "internalType": "uint256",
                 "name": "",
-                "type": "bool"
-            },
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
             {
                 "internalType": "address",
-                "name": "",
+                "name": "account",
                 "type": "address"
             },
             {
-                "internalType": "uint32",
-                "name": "",
-                "type": "uint32"
-            },
-            {
-                "internalType": "address[]",
-                "name": "",
-                "type": "address[]"
+                "internalType": "uint256",
+                "name": "snapshotId",
+                "type": "uint256"
             },
             {
-                "internalType": "uint32[]",
-                "name": "",
-                "type": "uint32[]"
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
             }
         ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "getSnapshotInterval",
+        "name": "claimableRevenue",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "",
                 "type": "uint256"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
                 "internalType": "address",
-                "name": "accessManager",
+                "name": "ancestorIpId",
                 "type": "address"
             }
         ],
-        "name": "initialize",
+        "name": "collectRoyaltyTokens",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "isConsumingScheduledOp",
+        "name": "decimals",
         "outputs": [
             {
-                "internalType": "bytes4",
+                "internalType": "uint8",
                 "name": "",
-                "type": "bytes4"
+                "type": "uint8"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
                 "internalType": "address",
-                "name": "ipId",
+                "name": "spender",
                 "type": "address"
             },
             {
-                "internalType": "bytes",
-                "name": "licenseData",
-                "type": "bytes"
-            },
+                "internalType": "uint256",
+                "name": "subtractedValue",
+                "type": "uint256"
+            }
+        ],
+        "name": "decreaseAllowance",
+        "outputs": [
             {
-                "internalType": "bytes",
-                "name": "externalData",
-                "type": "bytes"
+                "internalType": "bool",
+                "name": "",
+                "type": "bool"
             }
         ],
-        "name": "onLicenseMinting",
-        "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
             {
                 "internalType": "address",
-                "name": "ipId",
+                "name": "spender",
                 "type": "address"
             },
             {
-                "internalType": "address[]",
-                "name": "parentIpIds",
-                "type": "address[]"
+                "internalType": "uint256",
+                "name": "addedValue",
+                "type": "uint256"
+            }
+        ],
+        "name": "increaseAllowance",
+        "outputs": [
+            {
+                "internalType": "bool",
+                "name": "",
+                "type": "bool"
+            }
+        ],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "string",
+                "name": "name",
+                "type": "string"
             },
             {
-                "internalType": "bytes[]",
-                "name": "licenseData",
-                "type": "bytes[]"
+                "internalType": "string",
+                "name": "symbol",
+                "type": "string"
             },
             {
-                "internalType": "bytes",
-                "name": "externalData",
-                "type": "bytes"
+                "internalType": "uint32",
+                "name": "supply",
+                "type": "uint32"
+            },
+            {
+                "internalType": "uint32",
+                "name": "unclaimedTokens",
+                "type": "uint32"
+            },
+            {
+                "internalType": "address",
+                "name": "ipIdAddress",
+                "type": "address"
             }
         ],
-        "name": "onLinkToParents",
+        "name": "initialize",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
-        "inputs": [
+        "inputs": [],
+        "name": "ipId",
+        "outputs": [
             {
                 "internalType": "address",
-                "name": "caller",
+                "name": "",
                 "type": "address"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "uint256",
+                "name": "snapshotId",
+                "type": "uint256"
             },
             {
                 "internalType": "address",
-                "name": "ipId",
+                "name": "claimer",
                 "type": "address"
             },
             {
                 "internalType": "address",
                 "name": "token",
                 "type": "address"
-            },
+            }
+        ],
+        "name": "isClaimedAtSnapshot",
+        "outputs": [
             {
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
+                "internalType": "bool",
+                "name": "",
+                "type": "bool"
             }
         ],
-        "name": "onRoyaltyPayment",
-        "outputs": [],
-        "stateMutability": "nonpayable",
+        "stateMutability": "view",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "pause",
-        "outputs": [],
-        "stateMutability": "nonpayable",
+        "inputs": [
+            {
+                "internalType": "address",
+                "name": "ancestorIpId",
+                "type": "address"
+            }
+        ],
+        "name": "isCollectedByAncestor",
+        "outputs": [
+            {
+                "internalType": "bool",
+                "name": "",
+                "type": "bool"
+            }
+        ],
+        "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "paused",
+        "name": "lastSnapshotTimestamp",
         "outputs": [
             {
-                "internalType": "bool",
+                "internalType": "uint256",
                 "name": "",
-                "type": "bool"
+                "type": "uint256"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "proxiableUUID",
+        "name": "name",
         "outputs": [
             {
-                "internalType": "bytes32",
+                "internalType": "string",
                 "name": "",
-                "type": "bytes32"
+                "type": "string"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
-        "inputs": [
+        "inputs": [],
+        "name": "snapshot",
+        "outputs": [
             {
-                "internalType": "address",
-                "name": "newAuthority",
-                "type": "address"
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
             }
         ],
-        "name": "setAuthority",
-        "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
-        "inputs": [
+        "inputs": [],
+        "name": "symbol",
+        "outputs": [
             {
-                "internalType": "address",
-                "name": "beacon",
-                "type": "address"
+                "internalType": "string",
+                "name": "",
+                "type": "string"
             }
         ],
-        "name": "setIpRoyaltyVaultBeacon",
-        "outputs": [],
-        "stateMutability": "nonpayable",
+        "stateMutability": "view",
         "type": "function"
     },
     {
-        "inputs": [
+        "inputs": [],
+        "name": "tokens",
+        "outputs": [
+            {
+                "internalType": "address[]",
+                "name": "",
+                "type": "address[]"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [],
+        "name": "totalSupply",
+        "outputs": [
             {
                 "internalType": "uint256",
-                "name": "timestampInterval",
+                "name": "",
                 "type": "uint256"
             }
         ],
-        "name": "setSnapshotInterval",
-        "outputs": [],
-        "stateMutability": "nonpayable",
+        "stateMutability": "view",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "unpause",
-        "outputs": [],
-        "stateMutability": "nonpayable",
+        "inputs": [
+            {
+                "internalType": "uint256",
+                "name": "snapshotId",
+                "type": "uint256"
+            }
+        ],
+        "name": "totalSupplyAt",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
                 "internalType": "address",
-                "name": "newImplementation",
+                "name": "to",
                 "type": "address"
             },
             {
-                "internalType": "bytes",
-                "name": "data",
-                "type": "bytes"
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
             }
         ],
-        "name": "upgradeToAndCall",
-        "outputs": [],
-        "stateMutability": "payable",
+        "name": "transfer",
+        "outputs": [
+            {
+                "internalType": "bool",
+                "name": "",
+                "type": "bool"
+            }
+        ],
+        "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
             {
                 "internalType": "address",
-                "name": "newVault",
+                "name": "from",
+                "type": "address"
+            },
+            {
+                "internalType": "address",
+                "name": "to",
                 "type": "address"
+            },
+            {
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            }
+        ],
+        "name": "transferFrom",
+        "outputs": [
+            {
+                "internalType": "bool",
+                "name": "",
+                "type": "bool"
             }
         ],
-        "name": "upgradeVaults",
-        "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "uint256",
+                "name": "snapshotId",
+                "type": "uint256"
+            }
+        ],
+        "name": "unclaimedAtSnapshot",
+        "outputs": [
+            {
+                "internalType": "uint32",
+                "name": "",
+                "type": "uint32"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [],
+        "name": "unclaimedRoyaltyTokens",
+        "outputs": [
+            {
+                "internalType": "uint32",
+                "name": "",
+                "type": "uint32"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
     }
 ]
```

### Comparing `story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py` & `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-
-import json
-import os
-from web3 import Web3
-
-class RoyaltyPolicyLAPClient:
-    def __init__(self, web3: Web3):
-        self.web3 = web3
-        # Assuming config.json is located at the root of the project
-        config_path = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', '..', 'scripts', 'config.json'))
-        with open(config_path, 'r') as config_file:
-            config = json.load(config_file)
-        contract_address = None
-        for contract in config['contracts']:
-            if contract['contract_name'] == 'RoyaltyPolicyLAP':
-                contract_address = contract['contract_address']
-                break
-        if not contract_address:
-            raise ValueError(f"Contract address for RoyaltyPolicyLAP not found in config.json")
-        abi_path = os.path.join(os.path.dirname(__file__), 'RoyaltyPolicyLAP.json')
-        with open(abi_path, 'r') as abi_file:
-            abi = json.load(abi_file)
-        self.contract = self.web3.eth.contract(address=contract_address, abi=abi)
-    
-    def getRoyaltyData(self, ipId):
-        
-        return self.contract.functions.getRoyaltyData(ipId).call()
-        
+
+import json
+import os
+from web3 import Web3
+
+class RoyaltyPolicyLAPClient:
+    def __init__(self, web3: Web3):
+        self.web3 = web3
+        # Assuming config.json is located at the root of the project
+        config_path = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', '..', 'scripts', 'config.json'))
+        with open(config_path, 'r') as config_file:
+            config = json.load(config_file)
+        contract_address = None
+        for contract in config['contracts']:
+            if contract['contract_name'] == 'RoyaltyPolicyLAP':
+                contract_address = contract['contract_address']
+                break
+        if not contract_address:
+            raise ValueError(f"Contract address for RoyaltyPolicyLAP not found in config.json")
+        abi_path = os.path.join(os.path.dirname(__file__), 'RoyaltyPolicyLAP.json')
+        with open(abi_path, 'r') as abi_file:
+            abi = json.load(abi_file)
+        self.contract = self.web3.eth.contract(address=contract_address, abi=abi)
+    
+    def getRoyaltyData(self, ipId):
+        
+        return self.contract.functions.getRoyaltyData(ipId).call()
+
```

### Comparing `story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/resources/License.py` & `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/resources/License.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,239 +1,239 @@
-#src/story_protcol_python_sdk/resources/License.py
-
-from web3 import Web3
-
-from story_protocol_python_sdk.abi.PILicenseTemplate.PILicenseTemplate_client import PILicenseTemplateClient
-from story_protocol_python_sdk.abi.LicenseRegistry.LicenseRegistry_client import LicenseRegistryClient
-from story_protocol_python_sdk.abi.LicensingModule.LicensingModule_client import LicensingModuleClient
-from story_protocol_python_sdk.abi.IPAssetRegistry.IPAssetRegistry_client import IPAssetRegistryClient
-
-from story_protocol_python_sdk.utils.license_terms import get_license_term_by_type, PIL_TYPE
-from story_protocol_python_sdk.utils.transaction_utils import build_and_send_transaction
-
-class License:
-    def __init__(self, web3: Web3, account, chain_id):
-        self.web3 = web3
-        self.account = account
-        self.chain_id = chain_id
-
-        self.license_template_client = PILicenseTemplateClient(web3)
-        self.license_registry_client = LicenseRegistryClient(web3)
-        self.licensing_module_client  = LicensingModuleClient(web3)
-        self.ip_asset_registry_client = IPAssetRegistryClient(web3)
-
-    def _get_license_terms_id(self, license_terms):
-        return self.license_template_client.getLicenseTermsId(license_terms)
-
-    def registerNonComSocialRemixingPIL(self, tx_options=None):
-        try:
-            # Get the license terms for non-commercial social remixing PIL
-            license_terms = get_license_term_by_type(PIL_TYPE['NON_COMMERCIAL_REMIX'])
-
-            # Check if the license terms are already registered
-            license_terms_id = self._get_license_terms_id(license_terms)
-            if (license_terms_id is not None) and (license_terms_id != 0):
-                return {'licenseTermsId': license_terms_id}
-
-            # Build and send the transaction
-            response = build_and_send_transaction(
-                self.web3,
-                self.account,
-                self.license_template_client.build_registerLicenseTerms_transaction,
-                license_terms,
-                tx_options=tx_options
-            )
-
-            # Parse the event logs for LicenseTermsRegistered
-            target_logs = self._parse_tx_license_terms_registered_event(response['txReceipt'])
-            return {
-                'txHash': response['txHash'],
-                'licenseTermsId': target_logs
-            }
-
-        except Exception as e:
-            raise e
-        
-    def registerCommercialUsePIL(self, minting_fee, currency, royalty_policy, tx_options=None):
-        try:
-            # Construct complete license terms
-            complete_license_terms = get_license_term_by_type(PIL_TYPE['COMMERCIAL_USE'], {
-                'mintingFee': minting_fee,
-                'currency': currency,
-                'royaltyPolicy': royalty_policy,
-            })
-
-            # Check if the license terms are already registered
-            license_terms_id = self._get_license_terms_id(complete_license_terms)
-            if (license_terms_id is not None) and (license_terms_id != 0):
-                return {'licenseTermsId': license_terms_id}
-
-            # Build and send the transaction
-            response = build_and_send_transaction(
-                self.web3,
-                self.account,
-                self.license_template_client.build_registerLicenseTerms_transaction,
-                complete_license_terms,
-                tx_options=tx_options
-            )
-
-            # Parse the event logs for LicenseTermsRegistered
-            if not response['txReceipt'].logs:
-                return None
-
-            target_logs = self._parse_tx_license_terms_registered_event(response['txReceipt'])
-            return {
-                'txHash': response['txHash'],
-                'licenseTermsId': target_logs
-            }
-
-        except Exception as e:
-            raise e
-
-    def registerCommercialRemixPIL(self, minting_fee, currency, commercial_rev_share, royalty_policy, tx_options=None):
-        try:
-            # Construct complete license terms
-            complete_license_terms = get_license_term_by_type(PIL_TYPE['COMMERCIAL_REMIX'], {
-                'mintingFee': minting_fee,
-                'currency': currency,
-                'commercialRevShare': commercial_rev_share,
-                'royaltyPolicy': royalty_policy,
-            })
-            # Check if the license terms are already registered
-            license_terms_id = self._get_license_terms_id(complete_license_terms)
-            if license_terms_id and license_terms_id != 0:
-                return {'licenseTermsId': license_terms_id}
-
-            # Build and send the transaction
-            response = build_and_send_transaction(
-                self.web3,
-                self.account,
-                self.license_template_client.build_registerLicenseTerms_transaction,
-                complete_license_terms,
-                tx_options=tx_options
-            )
-
-            # Parse the event logs for LicenseTermsRegistered
-            if not response['txReceipt'].logs:
-                return None
-
-            target_logs = self._parse_tx_license_terms_registered_event(response['txReceipt'])
-            return {
-                'txHash': response['txHash'],
-                'licenseTermsId': target_logs
-            }
-
-        except Exception as e:
-            raise e
-
-    def _parse_tx_license_terms_registered_event(self, tx_receipt):
-        event_signature = self.web3.keccak(text="LicenseTermsRegistered(uint256,address,bytes)").hex()
-
-        for log in tx_receipt['logs']:
-            if log['topics'][0].hex() == event_signature:
-                return int(log['topics'][1].hex(), 16)
-
-        return None
-    
-    def attachLicenseTerms(self, ip_id, license_template, license_terms_id, tx_options=None):
-        try:
-            # Validate the license template address
-            if not Web3.is_address(license_template):
-                raise ValueError(f'Address "{license_template}" is invalid.')
-
-            # Check if the IP is registered
-            is_registered = self.ip_asset_registry_client.isRegistered(ip_id)
-            if not is_registered:
-                raise ValueError(f"The IP with id {ip_id} is not registered.")
-
-            # Check if the license terms exist
-            is_existed = self.license_registry_client.exists(license_template, license_terms_id)
-            if not is_existed:
-                raise ValueError(f"License terms id {license_terms_id} do not exist.")
-
-            # Check if the license terms are already attached to the IP
-            is_attached_license_terms = self.license_registry_client.hasIpAttachedLicenseTerms(ip_id, license_template, license_terms_id)
-            if is_attached_license_terms:
-                raise ValueError(f"License terms id {license_terms_id} is already attached to the IP with id {ip_id}.")
-
-            # Build and send the transaction
-            response = build_and_send_transaction(
-                self.web3,
-                self.account,
-                self.licensing_module_client.build_attachLicenseTerms_transaction,
-                ip_id,
-                license_template,
-                license_terms_id,
-                tx_options=tx_options
-            )
-
-            return {'txHash': response['txHash']}
-        
-        except Exception as e:
-            raise e
-        
-    def mintLicenseTokens(self, licensor_ip_id, license_template, license_terms_id, amount, receiver, tx_options=None):
-        try:
-            # Validate the license template address
-            if not Web3.is_address(license_template):
-                raise ValueError(f'Address "{license_template}" is invalid.')
-            
-            # Validate the license template address
-            if not Web3.is_address(receiver):
-                raise ValueError(f'Address "{receiver}" is invalid.')
-
-            # Check if the licensor IP is registered
-            is_registered = self.ip_asset_registry_client.isRegistered(licensor_ip_id)
-            if not is_registered:
-                raise ValueError(f"The licensor IP with id {licensor_ip_id} is not registered.")
-
-            # Check if the license terms exist
-            is_existed = self.license_template_client.exists(license_terms_id)
-            if not is_existed:
-                raise ValueError(f"License terms id {license_terms_id} do not exist.")
-
-            # Check if the license terms are attached to the IP
-            is_attached_license_terms = self.license_registry_client.hasIpAttachedLicenseTerms(licensor_ip_id, license_template, license_terms_id)
-            if not is_attached_license_terms:
-                raise ValueError(f"License terms id {license_terms_id} is not attached to the IP with id {licensor_ip_id}.")
-
-            # Build and send the transaction
-            response = build_and_send_transaction(
-                self.web3,
-                self.account,
-                self.licensing_module_client.build_mintLicenseTokens_transaction,
-                licensor_ip_id,
-                license_template,
-                license_terms_id,
-                amount,
-                receiver,
-                '0x0000000000000000000000000000000000000000',
-                tx_options=tx_options
-            )
-
-            # Parse the event logs for LicenseTokensMinted
-            target_logs = self._parse_tx_license_tokens_minted_event(response['txReceipt'])
-
-            return {
-                'txHash': response['txHash'],
-                'licenseTokenIds': target_logs
-            }
-
-        except Exception as e:
-            raise e
-
-    def _parse_tx_license_tokens_minted_event(self, tx_receipt):
-        event_signature = self.web3.keccak(text="LicenseTokenMinted(address,address,uint256)").hex()
-        token_ids = []
-
-        for log in tx_receipt['logs']:
-            if log['topics'][0].hex() == event_signature:
-                start_license_token_id = int(log['topics'][3].hex(), 16)
-                token_ids.append(start_license_token_id)
-
-        return token_ids if token_ids else None
-    
-    def getLicenseTerms(self, selectedLicenseTermsId):
-        try:
-            return self.license_template_client.getLicenseTerms(selectedLicenseTermsId)
-        except Exception as e:
+#src/story_protcol_python_sdk/resources/License.py
+
+from web3 import Web3
+
+from story_protocol_python_sdk.abi.PILicenseTemplate.PILicenseTemplate_client import PILicenseTemplateClient
+from story_protocol_python_sdk.abi.LicenseRegistry.LicenseRegistry_client import LicenseRegistryClient
+from story_protocol_python_sdk.abi.LicensingModule.LicensingModule_client import LicensingModuleClient
+from story_protocol_python_sdk.abi.IPAssetRegistry.IPAssetRegistry_client import IPAssetRegistryClient
+
+from story_protocol_python_sdk.utils.license_terms import get_license_term_by_type, PIL_TYPE
+from story_protocol_python_sdk.utils.transaction_utils import build_and_send_transaction
+
+class License:
+    def __init__(self, web3: Web3, account, chain_id):
+        self.web3 = web3
+        self.account = account
+        self.chain_id = chain_id
+
+        self.license_template_client = PILicenseTemplateClient(web3)
+        self.license_registry_client = LicenseRegistryClient(web3)
+        self.licensing_module_client  = LicensingModuleClient(web3)
+        self.ip_asset_registry_client = IPAssetRegistryClient(web3)
+
+    def _get_license_terms_id(self, license_terms):
+        return self.license_template_client.getLicenseTermsId(license_terms)
+
+    def registerNonComSocialRemixingPIL(self, tx_options=None):
+        try:
+            # Get the license terms for non-commercial social remixing PIL
+            license_terms = get_license_term_by_type(PIL_TYPE['NON_COMMERCIAL_REMIX'])
+
+            # Check if the license terms are already registered
+            license_terms_id = self._get_license_terms_id(license_terms)
+            if (license_terms_id is not None) and (license_terms_id != 0):
+                return {'licenseTermsId': license_terms_id}
+
+            # Build and send the transaction
+            response = build_and_send_transaction(
+                self.web3,
+                self.account,
+                self.license_template_client.build_registerLicenseTerms_transaction,
+                license_terms,
+                tx_options=tx_options
+            )
+
+            # Parse the event logs for LicenseTermsRegistered
+            target_logs = self._parse_tx_license_terms_registered_event(response['txReceipt'])
+            return {
+                'txHash': response['txHash'],
+                'licenseTermsId': target_logs
+            }
+
+        except Exception as e:
+            raise e
+        
+    def registerCommercialUsePIL(self, minting_fee, currency, royalty_policy, tx_options=None):
+        try:
+            # Construct complete license terms
+            complete_license_terms = get_license_term_by_type(PIL_TYPE['COMMERCIAL_USE'], {
+                'mintingFee': minting_fee,
+                'currency': currency,
+                'royaltyPolicy': royalty_policy,
+            })
+
+            # Check if the license terms are already registered
+            license_terms_id = self._get_license_terms_id(complete_license_terms)
+            if (license_terms_id is not None) and (license_terms_id != 0):
+                return {'licenseTermsId': license_terms_id}
+
+            # Build and send the transaction
+            response = build_and_send_transaction(
+                self.web3,
+                self.account,
+                self.license_template_client.build_registerLicenseTerms_transaction,
+                complete_license_terms,
+                tx_options=tx_options
+            )
+
+            # Parse the event logs for LicenseTermsRegistered
+            if not response['txReceipt'].logs:
+                return None
+
+            target_logs = self._parse_tx_license_terms_registered_event(response['txReceipt'])
+            return {
+                'txHash': response['txHash'],
+                'licenseTermsId': target_logs
+            }
+
+        except Exception as e:
+            raise e
+
+    def registerCommercialRemixPIL(self, minting_fee, currency, commercial_rev_share, royalty_policy, tx_options=None):
+        try:
+            # Construct complete license terms
+            complete_license_terms = get_license_term_by_type(PIL_TYPE['COMMERCIAL_REMIX'], {
+                'mintingFee': minting_fee,
+                'currency': currency,
+                'commercialRevShare': commercial_rev_share,
+                'royaltyPolicy': royalty_policy,
+            })
+            # Check if the license terms are already registered
+            license_terms_id = self._get_license_terms_id(complete_license_terms)
+            if license_terms_id and license_terms_id != 0:
+                return {'licenseTermsId': license_terms_id}
+
+            # Build and send the transaction
+            response = build_and_send_transaction(
+                self.web3,
+                self.account,
+                self.license_template_client.build_registerLicenseTerms_transaction,
+                complete_license_terms,
+                tx_options=tx_options
+            )
+
+            # Parse the event logs for LicenseTermsRegistered
+            if not response['txReceipt'].logs:
+                return None
+
+            target_logs = self._parse_tx_license_terms_registered_event(response['txReceipt'])
+            return {
+                'txHash': response['txHash'],
+                'licenseTermsId': target_logs
+            }
+
+        except Exception as e:
+            raise e
+
+    def _parse_tx_license_terms_registered_event(self, tx_receipt):
+        event_signature = self.web3.keccak(text="LicenseTermsRegistered(uint256,address,bytes)").hex()
+
+        for log in tx_receipt['logs']:
+            if log['topics'][0].hex() == event_signature:
+                return int(log['topics'][1].hex(), 16)
+
+        return None
+    
+    def attachLicenseTerms(self, ip_id, license_template, license_terms_id, tx_options=None):
+        try:
+            # Validate the license template address
+            if not Web3.is_address(license_template):
+                raise ValueError(f'Address "{license_template}" is invalid.')
+
+            # Check if the IP is registered
+            is_registered = self.ip_asset_registry_client.isRegistered(ip_id)
+            if not is_registered:
+                raise ValueError(f"The IP with id {ip_id} is not registered.")
+
+            # Check if the license terms exist
+            is_existed = self.license_registry_client.exists(license_template, license_terms_id)
+            if not is_existed:
+                raise ValueError(f"License terms id {license_terms_id} do not exist.")
+
+            # Check if the license terms are already attached to the IP
+            is_attached_license_terms = self.license_registry_client.hasIpAttachedLicenseTerms(ip_id, license_template, license_terms_id)
+            if is_attached_license_terms:
+                raise ValueError(f"License terms id {license_terms_id} is already attached to the IP with id {ip_id}.")
+
+            # Build and send the transaction
+            response = build_and_send_transaction(
+                self.web3,
+                self.account,
+                self.licensing_module_client.build_attachLicenseTerms_transaction,
+                ip_id,
+                license_template,
+                license_terms_id,
+                tx_options=tx_options
+            )
+
+            return {'txHash': response['txHash']}
+        
+        except Exception as e:
+            raise e
+        
+    def mintLicenseTokens(self, licensor_ip_id, license_template, license_terms_id, amount, receiver, tx_options=None):
+        try:
+            # Validate the license template address
+            if not Web3.is_address(license_template):
+                raise ValueError(f'Address "{license_template}" is invalid.')
+            
+            # Validate the license template address
+            if not Web3.is_address(receiver):
+                raise ValueError(f'Address "{receiver}" is invalid.')
+
+            # Check if the licensor IP is registered
+            is_registered = self.ip_asset_registry_client.isRegistered(licensor_ip_id)
+            if not is_registered:
+                raise ValueError(f"The licensor IP with id {licensor_ip_id} is not registered.")
+
+            # Check if the license terms exist
+            is_existed = self.license_template_client.exists(license_terms_id)
+            if not is_existed:
+                raise ValueError(f"License terms id {license_terms_id} do not exist.")
+
+            # Check if the license terms are attached to the IP
+            is_attached_license_terms = self.license_registry_client.hasIpAttachedLicenseTerms(licensor_ip_id, license_template, license_terms_id)
+            if not is_attached_license_terms:
+                raise ValueError(f"License terms id {license_terms_id} is not attached to the IP with id {licensor_ip_id}.")
+
+            # Build and send the transaction
+            response = build_and_send_transaction(
+                self.web3,
+                self.account,
+                self.licensing_module_client.build_mintLicenseTokens_transaction,
+                licensor_ip_id,
+                license_template,
+                license_terms_id,
+                amount,
+                receiver,
+                self.web3.constants.ADDRESS_ZERO,
+                tx_options=tx_options
+            )
+
+            # Parse the event logs for LicenseTokensMinted
+            target_logs = self._parse_tx_license_tokens_minted_event(response['txReceipt'])
+
+            return {
+                'txHash': response['txHash'],
+                'licenseTokenIds': target_logs
+            }
+
+        except Exception as e:
+            raise e
+
+    def _parse_tx_license_tokens_minted_event(self, tx_receipt):
+        event_signature = self.web3.keccak(text="LicenseTokenMinted(address,address,uint256)").hex()
+        token_ids = []
+
+        for log in tx_receipt['logs']:
+            if log['topics'][0].hex() == event_signature:
+                start_license_token_id = int(log['topics'][3].hex(), 16)
+                token_ids.append(start_license_token_id)
+
+        return token_ids if token_ids else None
+    
+    def getLicenseTerms(self, selectedLicenseTermsId):
+        try:
+            return self.license_template_client.getLicenseTerms(selectedLicenseTermsId)
+        except Exception as e:
             raise ValueError(f"Failed to get license terms: {str(e)}")
```

### Comparing `story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/scripts/config.json` & `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/scripts/config.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 24% similar despite different names*

```diff
@@ -1,222 +1,215 @@
-00000000: 7b0d 0a20 2020 2022 636f 6e74 7261 6374  {..    "contract
-00000010: 7322 3a20 5b0d 0a20 2020 2020 2020 207b  s": [..        {
-00000020: 0d0a 2020 2020 2020 2020 2020 2020 2263  ..            "c
-00000030: 6f6e 7472 6163 745f 6e61 6d65 223a 2022  ontract_name": "
-00000040: 4950 4173 7365 7452 6567 6973 7472 7922  IPAssetRegistry"
-00000050: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00000060: 636f 6e74 7261 6374 5f61 6464 7265 7373  contract_address
-00000070: 223a 2022 3078 6434 3366 4530 6438 3635  ": "0xd43fE0d865
-00000080: 6362 3543 3236 6231 3335 3164 3365 4166  cb5C26b1351d3eAf
-00000090: 3245 3330 3634 4245 3332 3736 4636 222c  2E3064BE3276F6",
-000000a0: 0d0a 2020 2020 2020 2020 2020 2020 2266  ..            "f
-000000b0: 756e 6374 696f 6e73 223a 205b 0d0a 2020  unctions": [..  
-000000c0: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-000000d0: 6e69 7469 616c 697a 6522 2c0d 0a20 2020  nitialize",..   
-000000e0: 2020 2020 2020 2020 2020 2020 2022 7061               "pa
-000000f0: 7573 6522 2c0d 0a20 2020 2020 2020 2020  use",..         
-00000100: 2020 2020 2020 2022 7265 6769 7374 6572         "register
-00000110: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000120: 2020 2020 2272 6567 6973 7465 7249 7041      "registerIpA
-00000130: 6363 6f75 6e74 222c 0d0a 2020 2020 2020  ccount",..      
-00000140: 2020 2020 2020 2020 2020 2273 6574 4175            "setAu
-00000150: 7468 6f72 6974 7922 2c0d 0a20 2020 2020  thority",..     
-00000160: 2020 2020 2020 2020 2020 2022 756e 7061             "unpa
-00000170: 7573 6522 2c0d 0a20 2020 2020 2020 2020  use",..         
-00000180: 2020 2020 2020 2022 7570 6772 6164 6554         "upgradeT
-00000190: 6f41 6e64 4361 6c6c 222c 0d0a 2020 2020  oAndCall",..    
-000001a0: 2020 2020 2020 2020 2020 2020 2261 7574              "aut
-000001b0: 686f 7269 7479 222c 0d0a 2020 2020 2020  hority",..      
-000001c0: 2020 2020 2020 2020 2020 2267 6574 4950            "getIP
-000001d0: 4163 636f 756e 7449 6d70 6c22 2c0d 0a20  AccountImpl",.. 
-000001e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000001f0: 6970 4163 636f 756e 7422 2c0d 0a20 2020  ipAccount",..   
-00000200: 2020 2020 2020 2020 2020 2020 2022 6970               "ip
-00000210: 4964 222c 0d0a 2020 2020 2020 2020 2020  Id",..          
-00000220: 2020 2020 2020 2269 7343 6f6e 7375 6d69        "isConsumi
-00000230: 6e67 5363 6865 6475 6c65 644f 7022 2c0d  ngScheduledOp",.
-00000240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000250: 2022 6973 5265 6769 7374 6572 6564 222c   "isRegistered",
-00000260: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000270: 2020 2270 6175 7365 6422 2c0d 0a20 2020    "paused",..   
-00000280: 2020 2020 2020 2020 2020 2020 2022 7072               "pr
-00000290: 6f78 6961 626c 6555 5549 4422 2c0d 0a20  oxiableUUID",.. 
-000002a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000002b0: 746f 7461 6c53 7570 706c 7922 0d0a 2020  totalSupply"..  
-000002c0: 2020 2020 2020 2020 2020 5d0d 0a20 2020            ]..   
-000002d0: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
-000002e0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-000002f0: 2263 6f6e 7472 6163 745f 6e61 6d65 223a  "contract_name":
-00000300: 2022 5049 4c69 6365 6e73 6554 656d 706c   "PILicenseTempl
-00000310: 6174 6522 2c0d 0a20 2020 2020 2020 2020  ate",..         
-00000320: 2020 2022 636f 6e74 7261 6374 5f61 6464     "contract_add
-00000330: 7265 7373 223a 2022 3078 3236 3042 3643  ress": "0x260B6C
-00000340: 4236 3238 3463 3839 6462 4536 3630 6330  B6284c89dbE660c0
-00000350: 3030 3432 3333 6637 6242 3939 4235 6564  004233f7bB99B5ed
-00000360: 4537 222c 0d0a 2020 2020 2020 2020 2020  E7",..          
-00000370: 2020 2266 756e 6374 696f 6e73 223a 205b    "functions": [
-00000380: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000390: 2020 2269 6e69 7469 616c 697a 6522 2c0d    "initialize",.
-000003a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000003b0: 2022 7265 6769 7374 6572 4c69 6365 6e73   "registerLicens
-000003c0: 6554 6572 6d73 222c 0d0a 2020 2020 2020  eTerms",..      
-000003d0: 2020 2020 2020 2020 2020 2273 6574 4170            "setAp
-000003e0: 7072 6f76 616c 222c 0d0a 2020 2020 2020  proval",..      
-000003f0: 2020 2020 2020 2020 2020 2273 6574 4175            "setAu
-00000400: 7468 6f72 6974 7922 2c0d 0a20 2020 2020  thority",..     
-00000410: 2020 2020 2020 2020 2020 2022 7570 6772             "upgr
-00000420: 6164 6554 6f41 6e64 4361 6c6c 222c 0d0a  adeToAndCall",..
-00000430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000440: 2276 6572 6966 7952 6567 6973 7465 7244  "verifyRegisterD
-00000450: 6572 6976 6174 6976 6522 2c0d 0a20 2020  erivative",..   
-00000460: 2020 2020 2020 2020 2020 2020 2022 7665               "ve
-00000470: 7269 6679 5265 6769 7374 6572 4465 7269  rifyRegisterDeri
-00000480: 7661 7469 7665 466f 7241 6c6c 5061 7265  vativeForAllPare
-00000490: 6e74 7322 2c0d 0a20 2020 2020 2020 2020  nts",..         
-000004a0: 2020 2020 2020 2022 6578 6973 7473 222c         "exists",
-000004b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000004c0: 2020 2267 6574 4c69 6365 6e73 6554 6572    "getLicenseTer
-000004d0: 6d73 222c 0d0a 2020 2020 2020 2020 2020  ms",..          
-000004e0: 2020 2020 2020 2267 6574 4c69 6365 6e73        "getLicens
-000004f0: 6554 6572 6d73 4964 222c 0d0a 2020 2020  eTermsId",..    
-00000500: 2020 2020 2020 2020 2020 2020 2267 6574              "get
-00000510: 526f 7961 6c74 7950 6f6c 6963 7922 0d0a  RoyaltyPolicy"..
-00000520: 2020 2020 2020 2020 2020 2020 5d0d 0a20              ].. 
-00000530: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-00000540: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-00000550: 2020 2263 6f6e 7472 6163 745f 6e61 6d65    "contract_name
-00000560: 223a 2022 4c69 6365 6e73 696e 674d 6f64  ": "LicensingMod
-00000570: 756c 6522 2c0d 0a20 2020 2020 2020 2020  ule",..         
-00000580: 2020 2022 636f 6e74 7261 6374 5f61 6464     "contract_add
-00000590: 7265 7373 223a 2022 3078 6538 3962 3045  ress": "0xe89b0E
-000005a0: 6141 3861 3039 3439 3733 3865 6641 3830  aA8a0949738efA80
-000005b0: 6242 3533 3161 3136 3546 4233 3435 3643  bB531a165FB3456C
-000005c0: 4265 222c 0d0a 2020 2020 2020 2020 2020  Be",..          
-000005d0: 2020 2266 756e 6374 696f 6e73 223a 205b    "functions": [
-000005e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000005f0: 2020 2261 7474 6163 684c 6963 656e 7365    "attachLicense
-00000600: 5465 726d 7322 2c0d 0a20 2020 2020 2020  Terms",..       
-00000610: 2020 2020 2020 2020 2022 696e 6974 6961           "initia
-00000620: 6c69 7a65 222c 0d0a 2020 2020 2020 2020  lize",..        
-00000630: 2020 2020 2020 2020 226d 696e 744c 6963          "mintLic
-00000640: 656e 7365 546f 6b65 6e73 222c 0d0a 2020  enseTokens",..  
-00000650: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-00000660: 6175 7365 222c 0d0a 2020 2020 2020 2020  ause",..        
-00000670: 2020 2020 2020 2020 2272 6567 6973 7465          "registe
-00000680: 7244 6572 6976 6174 6976 6522 2c0d 0a20  rDerivative",.. 
-00000690: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000006a0: 7265 6769 7374 6572 4465 7269 7661 7469  registerDerivati
-000006b0: 7665 5769 7468 4c69 6365 6e73 6554 6f6b  veWithLicenseTok
-000006c0: 656e 7322 2c0d 0a20 2020 2020 2020 2020  ens",..         
-000006d0: 2020 2020 2020 2022 7365 7441 7574 686f         "setAutho
-000006e0: 7269 7479 222c 0d0a 2020 2020 2020 2020  rity",..        
-000006f0: 2020 2020 2020 2020 2273 6574 4c69 6365          "setLice
-00000700: 6e73 696e 6743 6f6e 6669 6722 2c0d 0a20  nsingConfig",.. 
-00000710: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000720: 756e 7061 7573 6522 2c0d 0a20 2020 2020  unpause",..     
-00000730: 2020 2020 2020 2020 2020 2022 7570 6772             "upgr
-00000740: 6164 6554 6f41 6e64 4361 6c6c 220d 0a20  adeToAndCall".. 
-00000750: 2020 2020 2020 2020 2020 205d 0d0a 2020             ]..  
-00000760: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
-00000770: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
-00000780: 2022 636f 6e74 7261 6374 5f6e 616d 6522   "contract_name"
-00000790: 3a20 224c 6963 656e 7365 5265 6769 7374  : "LicenseRegist
-000007a0: 7279 222c 0d0a 2020 2020 2020 2020 2020  ry",..          
-000007b0: 2020 2263 6f6e 7472 6163 745f 6164 6472    "contract_addr
-000007c0: 6573 7322 3a20 2230 7834 6634 6231 6266  ess": "0x4f4b1bf
-000007d0: 3731 3335 4337 6666 3134 3632 3832 3643  7135C7ff1462826C
-000007e0: 4341 3831 4230 3438 4564 3139 3536 3265  CA81B048Ed19562e
-000007f0: 6422 2c0d 0a20 2020 2020 2020 2020 2020  d",..           
-00000800: 2022 6675 6e63 7469 6f6e 7322 3a20 5b0d   "functions": [.
-00000810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000820: 2022 6175 7468 6f72 6974 7922 2c0d 0a20   "authority",.. 
-00000830: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000840: 6578 6973 7473 222c 0d0a 2020 2020 2020  exists",..      
-00000850: 2020 2020 2020 2020 2020 2267 6574 4174            "getAt
-00000860: 7461 6368 6564 4c69 6365 6e73 6554 6572  tachedLicenseTer
-00000870: 6d73 222c 0d0a 2020 2020 2020 2020 2020  ms",..          
-00000880: 2020 2020 2020 2267 6574 4174 7461 6368        "getAttach
-00000890: 6564 4c69 6365 6e73 6554 6572 6d73 436f  edLicenseTermsCo
-000008a0: 756e 7422 2c0d 0a20 2020 2020 2020 2020  unt",..         
-000008b0: 2020 2020 2020 2022 6765 7444 6566 6175         "getDefau
-000008c0: 6c74 4c69 6365 6e73 6554 6572 6d73 222c  ltLicenseTerms",
-000008d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000008e0: 2020 2267 6574 4465 7269 7661 7469 7665    "getDerivative
-000008f0: 4970 222c 0d0a 2020 2020 2020 2020 2020  Ip",..          
-00000900: 2020 2020 2020 2267 6574 4465 7269 7661        "getDeriva
-00000910: 7469 7665 4970 436f 756e 7422 2c0d 0a20  tiveIpCount",.. 
-00000920: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000930: 6765 7445 7870 6972 6554 696d 6522 2c0d  getExpireTime",.
+00000000: 7b0a 2020 2020 2263 6f6e 7472 6163 7473  {.    "contracts
+00000010: 223a 205b 0a20 2020 2020 2020 207b 0a20  ": [.        {. 
+00000020: 2020 2020 2020 2020 2020 2022 636f 6e74             "cont
+00000030: 7261 6374 5f6e 616d 6522 3a20 2249 5041  ract_name": "IPA
+00000040: 7373 6574 5265 6769 7374 7279 222c 0a20  ssetRegistry",. 
+00000050: 2020 2020 2020 2020 2020 2022 636f 6e74             "cont
+00000060: 7261 6374 5f61 6464 7265 7373 223a 2022  ract_address": "
+00000070: 3078 6434 3366 4530 6438 3635 6362 3543  0xd43fE0d865cb5C
+00000080: 3236 6231 3335 3164 3365 4166 3245 3330  26b1351d3eAf2E30
+00000090: 3634 4245 3332 3736 4636 222c 0a20 2020  64BE3276F6",.   
+000000a0: 2020 2020 2020 2020 2022 6675 6e63 7469           "functi
+000000b0: 6f6e 7322 3a20 5b0a 2020 2020 2020 2020  ons": [.        
+000000c0: 2020 2020 2020 2020 2269 6e69 7469 616c          "initial
+000000d0: 697a 6522 2c0a 2020 2020 2020 2020 2020  ize",.          
+000000e0: 2020 2020 2020 2270 6175 7365 222c 0a20        "pause",. 
+000000f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000100: 7265 6769 7374 6572 222c 0a20 2020 2020  register",.     
+00000110: 2020 2020 2020 2020 2020 2022 7265 6769             "regi
+00000120: 7374 6572 4970 4163 636f 756e 7422 2c0a  sterIpAccount",.
+00000130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000140: 2273 6574 4175 7468 6f72 6974 7922 2c0a  "setAuthority",.
+00000150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000160: 2275 6e70 6175 7365 222c 0a20 2020 2020  "unpause",.     
+00000170: 2020 2020 2020 2020 2020 2022 7570 6772             "upgr
+00000180: 6164 6554 6f41 6e64 4361 6c6c 222c 0a20  adeToAndCall",. 
+00000190: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000001a0: 6175 7468 6f72 6974 7922 2c0a 2020 2020  authority",.    
+000001b0: 2020 2020 2020 2020 2020 2020 2267 6574              "get
+000001c0: 4950 4163 636f 756e 7449 6d70 6c22 2c0a  IPAccountImpl",.
+000001d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001e0: 2269 7041 6363 6f75 6e74 222c 0a20 2020  "ipAccount",.   
+000001f0: 2020 2020 2020 2020 2020 2020 2022 6970               "ip
+00000200: 4964 222c 0a20 2020 2020 2020 2020 2020  Id",.           
+00000210: 2020 2020 2022 6973 436f 6e73 756d 696e       "isConsumin
+00000220: 6753 6368 6564 756c 6564 4f70 222c 0a20  gScheduledOp",. 
+00000230: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000240: 6973 5265 6769 7374 6572 6564 222c 0a20  isRegistered",. 
+00000250: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000260: 7061 7573 6564 222c 0a20 2020 2020 2020  paused",.       
+00000270: 2020 2020 2020 2020 2022 7072 6f78 6961           "proxia
+00000280: 626c 6555 5549 4422 2c0a 2020 2020 2020  bleUUID",.      
+00000290: 2020 2020 2020 2020 2020 2274 6f74 616c            "total
+000002a0: 5375 7070 6c79 220a 2020 2020 2020 2020  Supply".        
+000002b0: 2020 2020 5d0a 2020 2020 2020 2020 7d2c      ].        },
+000002c0: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
+000002d0: 2020 2020 2020 2022 636f 6e74 7261 6374         "contract
+000002e0: 5f6e 616d 6522 3a20 2250 494c 6963 656e  _name": "PILicen
+000002f0: 7365 5465 6d70 6c61 7465 222c 0a20 2020  seTemplate",.   
+00000300: 2020 2020 2020 2020 2022 636f 6e74 7261           "contra
+00000310: 6374 5f61 6464 7265 7373 223a 2022 3078  ct_address": "0x
+00000320: 3236 3042 3643 4236 3238 3463 3839 6462  260B6CB6284c89db
+00000330: 4536 3630 6330 3030 3432 3333 6637 6242  E660c0004233f7bB
+00000340: 3939 4235 6564 4537 222c 0a20 2020 2020  99B5edE7",.     
+00000350: 2020 2020 2020 2022 6675 6e63 7469 6f6e         "function
+00000360: 7322 3a20 5b0a 2020 2020 2020 2020 2020  s": [.          
+00000370: 2020 2020 2020 2269 6e69 7469 616c 697a        "initializ
+00000380: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00000390: 2020 2020 2272 6567 6973 7465 724c 6963      "registerLic
+000003a0: 656e 7365 5465 726d 7322 2c0a 2020 2020  enseTerms",.    
+000003b0: 2020 2020 2020 2020 2020 2020 2273 6574              "set
+000003c0: 4170 7072 6f76 616c 222c 0a20 2020 2020  Approval",.     
+000003d0: 2020 2020 2020 2020 2020 2022 7365 7441             "setA
+000003e0: 7574 686f 7269 7479 222c 0a20 2020 2020  uthority",.     
+000003f0: 2020 2020 2020 2020 2020 2022 7570 6772             "upgr
+00000400: 6164 6554 6f41 6e64 4361 6c6c 222c 0a20  adeToAndCall",. 
+00000410: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000420: 7665 7269 6679 5265 6769 7374 6572 4465  verifyRegisterDe
+00000430: 7269 7661 7469 7665 222c 0a20 2020 2020  rivative",.     
+00000440: 2020 2020 2020 2020 2020 2022 7665 7269             "veri
+00000450: 6679 5265 6769 7374 6572 4465 7269 7661  fyRegisterDeriva
+00000460: 7469 7665 466f 7241 6c6c 5061 7265 6e74  tiveForAllParent
+00000470: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+00000480: 2020 2020 2265 7869 7374 7322 2c0a 2020      "exists",.  
+00000490: 2020 2020 2020 2020 2020 2020 2020 2267                "g
+000004a0: 6574 4c69 6365 6e73 6554 6572 6d73 222c  etLicenseTerms",
+000004b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000004c0: 2022 6765 744c 6963 656e 7365 5465 726d   "getLicenseTerm
+000004d0: 7349 6422 2c0a 2020 2020 2020 2020 2020  sId",.          
+000004e0: 2020 2020 2020 2267 6574 526f 7961 6c74        "getRoyalt
+000004f0: 7950 6f6c 6963 7922 0a20 2020 2020 2020  yPolicy".       
+00000500: 2020 2020 205d 0a20 2020 2020 2020 207d       ].        }
+00000510: 2c0a 2020 2020 2020 2020 7b0a 2020 2020  ,.        {.    
+00000520: 2020 2020 2020 2020 2263 6f6e 7472 6163          "contrac
+00000530: 745f 6e61 6d65 223a 2022 4c69 6365 6e73  t_name": "Licens
+00000540: 696e 674d 6f64 756c 6522 2c0a 2020 2020  ingModule",.    
+00000550: 2020 2020 2020 2020 2263 6f6e 7472 6163          "contrac
+00000560: 745f 6164 6472 6573 7322 3a20 2230 7865  t_address": "0xe
+00000570: 3839 6230 4561 4138 6130 3934 3937 3338  89b0EaA8a0949738
+00000580: 6566 4138 3062 4235 3331 6131 3635 4642  efA80bB531a165FB
+00000590: 3334 3536 4342 6522 2c0a 2020 2020 2020  3456CBe",.      
+000005a0: 2020 2020 2020 2266 756e 6374 696f 6e73        "functions
+000005b0: 223a 205b 0a20 2020 2020 2020 2020 2020  ": [.           
+000005c0: 2020 2020 2022 6174 7461 6368 4c69 6365       "attachLice
+000005d0: 6e73 6554 6572 6d73 222c 0a20 2020 2020  nseTerms",.     
+000005e0: 2020 2020 2020 2020 2020 2022 696e 6974             "init
+000005f0: 6961 6c69 7a65 222c 0a20 2020 2020 2020  ialize",.       
+00000600: 2020 2020 2020 2020 2022 6d69 6e74 4c69           "mintLi
+00000610: 6365 6e73 6554 6f6b 656e 7322 2c0a 2020  censeTokens",.  
+00000620: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+00000630: 6175 7365 222c 0a20 2020 2020 2020 2020  ause",.         
+00000640: 2020 2020 2020 2022 7265 6769 7374 6572         "register
+00000650: 4465 7269 7661 7469 7665 222c 0a20 2020  Derivative",.   
+00000660: 2020 2020 2020 2020 2020 2020 2022 7265               "re
+00000670: 6769 7374 6572 4465 7269 7661 7469 7665  gisterDerivative
+00000680: 5769 7468 4c69 6365 6e73 6554 6f6b 656e  WithLicenseToken
+00000690: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+000006a0: 2020 2020 2273 6574 4175 7468 6f72 6974      "setAuthorit
+000006b0: 7922 2c0a 2020 2020 2020 2020 2020 2020  y",.            
+000006c0: 2020 2020 2273 6574 4c69 6365 6e73 696e      "setLicensin
+000006d0: 6743 6f6e 6669 6722 2c0a 2020 2020 2020  gConfig",.      
+000006e0: 2020 2020 2020 2020 2020 2275 6e70 6175            "unpau
+000006f0: 7365 222c 0a20 2020 2020 2020 2020 2020  se",.           
+00000700: 2020 2020 2022 7570 6772 6164 6554 6f41       "upgradeToA
+00000710: 6e64 4361 6c6c 220a 2020 2020 2020 2020  ndCall".        
+00000720: 2020 2020 5d0a 2020 2020 2020 2020 7d2c      ].        },
+00000730: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
+00000740: 2020 2020 2020 2022 636f 6e74 7261 6374         "contract
+00000750: 5f6e 616d 6522 3a20 224c 6963 656e 7365  _name": "License
+00000760: 5265 6769 7374 7279 222c 0a20 2020 2020  Registry",.     
+00000770: 2020 2020 2020 2022 636f 6e74 7261 6374         "contract
+00000780: 5f61 6464 7265 7373 223a 2022 3078 3466  _address": "0x4f
+00000790: 3462 3162 6637 3133 3543 3766 6631 3436  4b1bf7135C7ff146
+000007a0: 3238 3236 4343 4138 3142 3034 3845 6431  2826CCA81B048Ed1
+000007b0: 3935 3632 6564 222c 0a20 2020 2020 2020  9562ed",.       
+000007c0: 2020 2020 2022 6675 6e63 7469 6f6e 7322       "functions"
+000007d0: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
+000007e0: 2020 2020 2261 7574 686f 7269 7479 222c      "authority",
+000007f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000800: 2022 6578 6973 7473 222c 0a20 2020 2020   "exists",.     
+00000810: 2020 2020 2020 2020 2020 2022 6765 7441             "getA
+00000820: 7474 6163 6865 644c 6963 656e 7365 5465  ttachedLicenseTe
+00000830: 726d 7322 2c0a 2020 2020 2020 2020 2020  rms",.          
+00000840: 2020 2020 2020 2267 6574 4174 7461 6368        "getAttach
+00000850: 6564 4c69 6365 6e73 6554 6572 6d73 436f  edLicenseTermsCo
+00000860: 756e 7422 2c0a 2020 2020 2020 2020 2020  unt",.          
+00000870: 2020 2020 2020 2267 6574 4465 6661 756c        "getDefaul
+00000880: 744c 6963 656e 7365 5465 726d 7322 2c0a  tLicenseTerms",.
+00000890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008a0: 2267 6574 4465 7269 7661 7469 7665 4970  "getDerivativeIp
+000008b0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000008c0: 2020 2022 6765 7444 6572 6976 6174 6976     "getDerivativ
+000008d0: 6549 7043 6f75 6e74 222c 0a20 2020 2020  eIpCount",.     
+000008e0: 2020 2020 2020 2020 2020 2022 6765 7445             "getE
+000008f0: 7870 6972 6554 696d 6522 2c0a 2020 2020  xpireTime",.    
+00000900: 2020 2020 2020 2020 2020 2020 2267 6574              "get
+00000910: 4c69 6365 6e73 696e 6743 6f6e 6669 6722  LicensingConfig"
+00000920: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000930: 2020 2267 6574 5061 7265 6e74 4970 222c    "getParentIp",
 00000940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000950: 2022 6765 744c 6963 656e 7369 6e67 436f   "getLicensingCo
-00000960: 6e66 6967 222c 0d0a 2020 2020 2020 2020  nfig",..        
-00000970: 2020 2020 2020 2020 2267 6574 5061 7265          "getPare
-00000980: 6e74 4970 222c 0d0a 2020 2020 2020 2020  ntIp",..        
-00000990: 2020 2020 2020 2020 2267 6574 5061 7265          "getPare
-000009a0: 6e74 4970 436f 756e 7422 2c0d 0a20 2020  ntIpCount",..   
-000009b0: 2020 2020 2020 2020 2020 2020 2022 6861               "ha
-000009c0: 7344 6572 6976 6174 6976 6549 7073 222c  sDerivativeIps",
-000009d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000009e0: 2020 2268 6173 4970 4174 7461 6368 6564    "hasIpAttached
-000009f0: 4c69 6365 6e73 6554 6572 6d73 222c 0d0a  LicenseTerms",..
-00000a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a10: 2269 7343 6f6e 7375 6d69 6e67 5363 6865  "isConsumingSche
-00000a20: 6475 6c65 644f 7022 2c0d 0a20 2020 2020  duledOp",..     
-00000a30: 2020 2020 2020 2020 2020 2022 6973 4465             "isDe
-00000a40: 7269 7661 7469 7665 4970 222c 0d0a 2020  rivativeIp",..  
-00000a50: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-00000a60: 7345 7870 6972 6564 4e6f 7722 2c0d 0a20  sExpiredNow",.. 
+00000950: 2022 6765 7450 6172 656e 7449 7043 6f75   "getParentIpCou
+00000960: 6e74 222c 0a20 2020 2020 2020 2020 2020  nt",.           
+00000970: 2020 2020 2022 6861 7344 6572 6976 6174       "hasDerivat
+00000980: 6976 6549 7073 222c 0a20 2020 2020 2020  iveIps",.       
+00000990: 2020 2020 2020 2020 2022 6861 7349 7041           "hasIpA
+000009a0: 7474 6163 6865 644c 6963 656e 7365 5465  ttachedLicenseTe
+000009b0: 726d 7322 2c0a 2020 2020 2020 2020 2020  rms",.          
+000009c0: 2020 2020 2020 2269 7343 6f6e 7375 6d69        "isConsumi
+000009d0: 6e67 5363 6865 6475 6c65 644f 7022 2c0a  ngScheduledOp",.
+000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009f0: 2269 7344 6572 6976 6174 6976 6549 7022  "isDerivativeIp"
+00000a00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000a10: 2020 2269 7345 7870 6972 6564 4e6f 7722    "isExpiredNow"
+00000a20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000a30: 2020 2269 7350 6172 656e 7449 7022 2c0a    "isParentIp",.
+00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a50: 2269 7352 6567 6973 7465 7265 644c 6963  "isRegisteredLic
+00000a60: 656e 7365 5465 6d70 6c61 7465 222c 0a20  enseTemplate",. 
 00000a70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000a80: 6973 5061 7265 6e74 4970 222c 0d0a 2020  isParentIp",..  
-00000a90: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-00000aa0: 7352 6567 6973 7465 7265 644c 6963 656e  sRegisteredLicen
-00000ab0: 7365 5465 6d70 6c61 7465 222c 0d0a 2020  seTemplate",..  
-00000ac0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-00000ad0: 726f 7869 6162 6c65 5555 4944 222c 0d0a  roxiableUUID",..
-00000ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000af0: 2276 6572 6966 794d 696e 744c 6963 656e  "verifyMintLicen
-00000b00: 7365 546f 6b65 6e22 0d0a 2020 2020 2020  seToken"..      
-00000b10: 2020 2020 2020 5d0d 0a20 2020 2020 2020        ]..       
-00000b20: 207d 2c0d 0a20 2020 2020 2020 207b 0d0a   },..        {..
-00000b30: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
-00000b40: 7472 6163 745f 6e61 6d65 223a 2022 4c69  tract_name": "Li
-00000b50: 6365 6e73 6554 6f6b 656e 222c 0d0a 2020  censeToken",..  
-00000b60: 2020 2020 2020 2020 2020 2263 6f6e 7472            "contr
-00000b70: 6163 745f 6164 6472 6573 7322 3a20 2230  act_address": "0
-00000b80: 7831 3333 3363 3738 4138 3231 6339 6135  x1333c78A821c9a5
-00000b90: 3736 3230 3942 3031 6131 3664 4443 4546  76209B01a16dDCEF
-00000ba0: 3838 3163 4162 3666 3222 2c0d 0a20 2020  881cAb6f2",..   
-00000bb0: 2020 2020 2020 2020 2022 6675 6e63 7469           "functi
-00000bc0: 6f6e 7322 3a20 5b0d 0a20 2020 2020 2020  ons": [..       
-00000bd0: 2020 2020 2020 2020 2022 6f77 6e65 724f           "ownerO
-00000be0: 6622 0d0a 2020 2020 2020 2020 2020 2020  f"..            
-00000bf0: 5d0d 0a20 2020 2020 2020 207d 2c0d 0a20  ]..        },.. 
-00000c00: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
-00000c10: 2020 2020 2020 2263 6f6e 7472 6163 745f        "contract_
-00000c20: 6e61 6d65 223a 2022 526f 7961 6c74 7950  name": "RoyaltyP
-00000c30: 6f6c 6963 794c 4150 222c 0d0a 2020 2020  olicyLAP",..    
-00000c40: 2020 2020 2020 2020 2263 6f6e 7472 6163          "contrac
-00000c50: 745f 6164 6472 6573 7322 3a20 2230 7841  t_address": "0xA
-00000c60: 4162 6166 3334 3943 3761 3241 3834 3536  Abaf349C7a2A8456
-00000c70: 3446 3943 4334 4163 3133 3042 3366 3139  4F9CC4Ac130B3f19
-00000c80: 4137 3138 4538 3622 2c0d 0a20 2020 2020  A718E86",..     
-00000c90: 2020 2020 2020 2022 6675 6e63 7469 6f6e         "function
-00000ca0: 7322 3a20 5b0d 0a20 2020 2020 2020 2020  s": [..         
-00000cb0: 2020 2020 2020 2022 6765 7452 6f79 616c         "getRoyal
-00000cc0: 7479 4461 7461 220d 0a20 2020 2020 2020  tyData"..       
-00000cd0: 2020 2020 205d 0d0a 2020 2020 2020 2020       ]..        
-00000ce0: 7d2c 0d0a 2020 2020 2020 2020 7b0d 0a20  },..        {.. 
-00000cf0: 2020 2020 2020 2020 2020 2022 636f 6e74             "cont
-00000d00: 7261 6374 5f6e 616d 6522 3a20 2252 6f79  ract_name": "Roy
-00000d10: 616c 7479 4d6f 6475 6c65 222c 0d0a 2020  altyModule",..  
-00000d20: 2020 2020 2020 2020 2020 2263 6f6e 7472            "contr
-00000d30: 6163 745f 6164 6472 6573 7322 3a20 2230  act_address": "0
-00000d40: 7846 4145 3936 3164 6432 6238 3743 4435  xFAE961dd2b87CD5
-00000d50: 3831 3864 6243 4463 3235 3931 6536 4142  818dbCDc2591e6AB
-00000d60: 3062 3530 4539 3662 3022 2c0d 0a20 2020  0b50E96b0",..   
-00000d70: 2020 2020 2020 2020 2022 6675 6e63 7469           "functi
-00000d80: 6f6e 7322 3a20 5b0d 0a20 2020 2020 2020  ons": [..       
-00000d90: 2020 2020 2020 2020 2022 7061 7952 6f79           "payRoy
-00000da0: 616c 7479 4f6e 4265 6861 6c66 220d 0a20  altyOnBehalf".. 
-00000db0: 2020 2020 2020 2020 2020 205d 0d0a 2020             ]..  
-00000dc0: 2020 2020 2020 7d0d 0a20 2020 205d 0d0a        }..    ]..
-00000dd0: 7d0d 0a                                  }..
+00000a80: 7072 6f78 6961 626c 6555 5549 4422 2c0a  proxiableUUID",.
+00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000aa0: 2276 6572 6966 794d 696e 744c 6963 656e  "verifyMintLicen
+00000ab0: 7365 546f 6b65 6e22 0a20 2020 2020 2020  seToken".       
+00000ac0: 2020 2020 205d 0a20 2020 2020 2020 207d       ].        }
+00000ad0: 2c0a 2020 2020 2020 2020 7b0a 2020 2020  ,.        {.    
+00000ae0: 2020 2020 2020 2020 2263 6f6e 7472 6163          "contrac
+00000af0: 745f 6e61 6d65 223a 2022 4c69 6365 6e73  t_name": "Licens
+00000b00: 6554 6f6b 656e 222c 0a20 2020 2020 2020  eToken",.       
+00000b10: 2020 2020 2022 636f 6e74 7261 6374 5f61       "contract_a
+00000b20: 6464 7265 7373 223a 2022 3078 3133 3333  ddress": "0x1333
+00000b30: 6337 3841 3832 3163 3961 3537 3632 3039  c78A821c9a576209
+00000b40: 4230 3161 3136 6444 4345 4638 3831 6341  B01a16dDCEF881cA
+00000b50: 6236 6632 222c 0a20 2020 2020 2020 2020  b6f2",.         
+00000b60: 2020 2022 6675 6e63 7469 6f6e 7322 3a20     "functions": 
+00000b70: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00000b80: 2020 226f 776e 6572 4f66 220a 2020 2020    "ownerOf".    
+00000b90: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+00000ba0: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
+00000bb0: 2020 2020 2020 2020 2020 2022 636f 6e74             "cont
+00000bc0: 7261 6374 5f6e 616d 6522 3a20 2252 6f79  ract_name": "Roy
+00000bd0: 616c 7479 506f 6c69 6379 4c41 5022 2c0a  altyPolicyLAP",.
+00000be0: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
+00000bf0: 7472 6163 745f 6164 6472 6573 7322 3a20  tract_address": 
+00000c00: 2230 7841 4162 6166 3334 3943 3761 3241  "0xAAbaf349C7a2A
+00000c10: 3834 3536 3446 3943 4334 4163 3133 3042  84564F9CC4Ac130B
+00000c20: 3366 3139 4137 3138 4538 3622 2c0a 2020  3f19A718E86",.  
+00000c30: 2020 2020 2020 2020 2020 2266 756e 6374            "funct
+00000c40: 696f 6e73 223a 205b 0a20 2020 2020 2020  ions": [.       
+00000c50: 2020 2020 2020 2020 2022 6765 7452 6f79           "getRoy
+00000c60: 616c 7479 4461 7461 220a 2020 2020 2020  altyData".      
+00000c70: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+00000c80: 7d2c 0a20 2020 2020 2020 207b 0a20 2020  },.        {.   
+00000c90: 2020 2020 2020 2020 2022 636f 6e74 7261           "contra
+00000ca0: 6374 5f6e 616d 6522 3a20 2252 6f79 616c  ct_name": "Royal
+00000cb0: 7479 4d6f 6475 6c65 222c 0a20 2020 2020  tyModule",.     
+00000cc0: 2020 2020 2020 2022 636f 6e74 7261 6374         "contract
+00000cd0: 5f61 6464 7265 7373 223a 2022 3078 4641  _address": "0xFA
+00000ce0: 4539 3631 6464 3262 3837 4344 3538 3138  E961dd2b87CD5818
+00000cf0: 6462 4344 6332 3539 3165 3641 4230 6235  dbCDc2591e6AB0b5
+00000d00: 3045 3936 6230 222c 0a20 2020 2020 2020  0E96b0",.       
+00000d10: 2020 2020 2022 6675 6e63 7469 6f6e 7322       "functions"
+00000d20: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
+00000d30: 2020 2020 2270 6179 526f 7961 6c74 794f      "payRoyaltyO
+00000d40: 6e42 6568 616c 6622 0a20 2020 2020 2020  nBehalf".       
+00000d50: 2020 2020 205d 0a20 2020 2020 2020 207d       ].        }
+00000d60: 0a20 2020 205d 0a7d 0a                   .    ].}.
```

### Comparing `story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/scripts/generate_client.py` & `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/scripts/generate_client.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,161 +1,161 @@
-#scripts/generate_client.py
-
-import requests
-import json
-import os
-from jinja2 import Template
-from dotenv import load_dotenv
-import time
-
-# Load environment variables from .env file
-load_dotenv(os.path.join(os.path.dirname(__file__), '..', '..', '..', '.env'))
-
-# Get the API key from environment variables
-api_key = os.getenv('ETHERSCAN_API_KEY')
-if not api_key:
-    raise ValueError("Please set ETHERSCAN_API_KEY in the .env file")
-
-def fetch_abi(contract_address, api_key):
-    url = f"https://api-sepolia.etherscan.io/api?module=contract&action=getabi&address={contract_address}&apikey={api_key}"
-    response = requests.get(url)
-    response_json = response.json()
-    if response_json.get('status') == '1':
-        abi = json.loads(response_json['result'])
-        return abi
-    else:
-        raise Exception(f"Error fetching ABI for address {contract_address}: {response_json.get('message')}")
-
-def fetch_proxy_implementation_address(proxy_address, api_key):
-    url = "https://api-sepolia.etherscan.io/api"
-    params = {
-        "module": "proxy",
-        "action": "eth_getStorageAt",
-        "address": proxy_address,
-        "position": "0x360894a13ba1a3210667c828492db98dca3e2076cc3735a920a3ca505d382bbc",
-        "tag": "latest",
-        "apikey": api_key
-    }
-    response = requests.get(url, params=params)
-    response_json = response.json()
-    # print(f"Response JSON for {proxy_address}: {response_json}")  # Debugging output
-    if 'result' in response_json:
-        storage_value = response_json['result']
-        if storage_value and storage_value != '0x':
-            implementation_address = "0x" + storage_value[-40:]
-            return implementation_address
-        else:
-            raise Exception(f"No valid implementation address found in storage for proxy {proxy_address}")
-    else:
-        raise Exception(f"Error fetching implementation address from storage for proxy {proxy_address}: {response_json}")
-
-def fetch_proxy_abi(proxy_address, api_key):
-    try:
-        implementation_address = fetch_proxy_implementation_address(proxy_address, api_key)
-        return fetch_abi(implementation_address, api_key)
-    except Exception as e:
-        print(f"Failed to fetch proxy implementation address for {proxy_address}: {e}")
-        return None
-
-def save_abi(abi, output_path):
-    with open(output_path, 'w') as abi_file:
-        json.dump(abi, abi_file, indent=2)
-
-class_template = Template('''
-import json
-import os
-from web3 import Web3
-
-class {{ class_name }}:
-    def __init__(self, web3: Web3):
-        self.web3 = web3
-        # Assuming config.json is located at the root of the project
-        config_path = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', '..', 'scripts', 'config.json'))
-        with open(config_path, 'r') as config_file:
-            config = json.load(config_file)
-        contract_address = None
-        for contract in config['contracts']:
-            if contract['contract_name'] == '{{ contract_name }}':
-                contract_address = contract['contract_address']
-                break
-        if not contract_address:
-            raise ValueError(f"Contract address for {{ contract_name }} not found in config.json")
-        abi_path = os.path.join(os.path.dirname(__file__), '{{ contract_name }}.json')
-        with open(abi_path, 'r') as abi_file:
-            abi = json.load(abi_file)
-        self.contract = self.web3.eth.contract(address=contract_address, abi=abi)
-    {% for function in functions %}
-    def {{ function.name }}(self, {% if function.inputs %}{{ function.inputs | join(', ') }}{% endif %}):
-        {% if function.stateMutability == 'view' or function.stateMutability == 'pure' %}
-        return self.contract.functions.{{ function.name }}({% if function.inputs %}{{ function.inputs | join(', ') }}{% endif %}).call()
-        {% else %}
-        return self.contract.functions.{{ function.name }}({% if function.inputs %}{{ function.inputs | join(', ') }}{% endif %}).transact()
-        
-    def build_{{ function.name }}_transaction(self, {% if function.inputs %}{{ function.inputs | join(', ') }}, {% endif %}tx_params):
-        return self.contract.functions.{{ function.name }}({% if function.inputs %}{{ function.inputs | join(', ') }}{% endif %}).build_transaction(tx_params)
-    {% endif %}
-    {% endfor %}
-''')
-
-def generate_python_classes_from_abi(abi, contract_name, functions, output_dir):
-    class_name = contract_name + 'Client'  # Use the contract_name directly for proper capitalization
-    
-    selected_functions = []
-    for item in abi:
-        if item['type'] == 'function' and item['name'] in functions:
-            function = {
-                'name': item['name'],
-                'inputs': [input['name'] for input in item['inputs']],
-                'stateMutability': item['stateMutability'] if 'stateMutability' in item else 'nonpayable'
-            }
-            selected_functions.append(function)
-    
-    # Sort functions to have transact functions first and call functions after
-    selected_functions.sort(key=lambda x: x['stateMutability'] in ['view', 'pure'])
-    
-    rendered_class = class_template.render(
-        class_name=class_name,
-        contract_name=contract_name,
-        functions=selected_functions
-    )
-    
-    contract_output_dir = os.path.join(output_dir, contract_name)
-    os.makedirs(contract_output_dir, exist_ok=True)
-
-    output_file_path = os.path.join(contract_output_dir, f"{contract_name}_client.py")
-    with open(output_file_path, 'w') as output_file:
-        output_file.write(rendered_class)
-    
-    print(f"Generated {class_name} class from ABI")
-
-def main(config_path, output_dir):
-    with open(config_path, 'r') as config_file:
-        config = json.load(config_file)
-    
-
-        for contract in config['contracts']:
-            contract_name = contract['contract_name']
-            contract_address = contract['contract_address']
-            functions = contract['functions']
-
-            for attempt in range(3):  # Retry up to 3 times
-                try:
-                    abi = fetch_proxy_abi(contract_address, api_key)
-                    if abi:
-                        contract_output_dir = os.path.join(output_dir, contract_name)
-                        os.makedirs(contract_output_dir, exist_ok=True)
-
-                        save_abi(abi, os.path.join(contract_output_dir, f'{contract_name}.json'))
-                        generate_python_classes_from_abi(abi, contract_name, functions, output_dir)
-                        time.sleep(1)  # Wait for 1 seconds before moving to next contract
-                        break  # If successful, break out of the retry loop
-                    else:
-                        raise Exception("Failed to fetch ABI")
-                except Exception as e:
-                    print(f"Error on attempt {attempt + 1} for {contract_name}: {e}")
-                    time.sleep(2)  # Wait for 2 seconds before retrying
-
-if __name__ == "__main__":
-    config_path = os.path.join(os.path.dirname(__file__), 'config.json')
-    output_dir = os.path.join(os.path.dirname(__file__), '../abi')
-    os.makedirs(output_dir, exist_ok=True)
-    main(config_path, output_dir)
+#scripts/generate_client.py
+
+import requests
+import json
+import os
+from jinja2 import Template
+from dotenv import load_dotenv
+import time
+
+# Load environment variables from .env file
+load_dotenv(os.path.join(os.path.dirname(__file__), '..', '..', '..', '.env'))
+
+# Get the API key from environment variables
+api_key = os.getenv('ETHERSCAN_API_KEY')
+if not api_key:
+    raise ValueError("Please set ETHERSCAN_API_KEY in the .env file")
+
+def fetch_abi(contract_address, api_key):
+    url = f"https://api-sepolia.etherscan.io/api?module=contract&action=getabi&address={contract_address}&apikey={api_key}"
+    response = requests.get(url)
+    response_json = response.json()
+    if response_json.get('status') == '1':
+        abi = json.loads(response_json['result'])
+        return abi
+    else:
+        raise Exception(f"Error fetching ABI for address {contract_address}: {response_json.get('message')}")
+
+def fetch_proxy_implementation_address(proxy_address, api_key):
+    url = "https://api-sepolia.etherscan.io/api"
+    params = {
+        "module": "proxy",
+        "action": "eth_getStorageAt",
+        "address": proxy_address,
+        "position": "0x360894a13ba1a3210667c828492db98dca3e2076cc3735a920a3ca505d382bbc",
+        "tag": "latest",
+        "apikey": api_key
+    }
+    response = requests.get(url, params=params)
+    response_json = response.json()
+    # print(f"Response JSON for {proxy_address}: {response_json}")  # Debugging output
+    if 'result' in response_json:
+        storage_value = response_json['result']
+        if storage_value and storage_value != '0x':
+            implementation_address = "0x" + storage_value[-40:]
+            return implementation_address
+        else:
+            raise Exception(f"No valid implementation address found in storage for proxy {proxy_address}")
+    else:
+        raise Exception(f"Error fetching implementation address from storage for proxy {proxy_address}: {response_json}")
+
+def fetch_proxy_abi(proxy_address, api_key):
+    try:
+        implementation_address = fetch_proxy_implementation_address(proxy_address, api_key)
+        return fetch_abi(implementation_address, api_key)
+    except Exception as e:
+        print(f"Failed to fetch proxy implementation address for {proxy_address}: {e}")
+        return None
+
+def save_abi(abi, output_path):
+    with open(output_path, 'w') as abi_file:
+        json.dump(abi, abi_file, indent=2)
+
+class_template = Template('''
+import json
+import os
+from web3 import Web3
+
+class {{ class_name }}:
+    def __init__(self, web3: Web3):
+        self.web3 = web3
+        # Assuming config.json is located at the root of the project
+        config_path = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', '..', 'scripts', 'config.json'))
+        with open(config_path, 'r') as config_file:
+            config = json.load(config_file)
+        contract_address = None
+        for contract in config['contracts']:
+            if contract['contract_name'] == '{{ contract_name }}':
+                contract_address = contract['contract_address']
+                break
+        if not contract_address:
+            raise ValueError(f"Contract address for {{ contract_name }} not found in config.json")
+        abi_path = os.path.join(os.path.dirname(__file__), '{{ contract_name }}.json')
+        with open(abi_path, 'r') as abi_file:
+            abi = json.load(abi_file)
+        self.contract = self.web3.eth.contract(address=contract_address, abi=abi)
+    {% for function in functions %}
+    def {{ function.name }}(self, {% if function.inputs %}{{ function.inputs | join(', ') }}{% endif %}):
+        {% if function.stateMutability == 'view' or function.stateMutability == 'pure' %}
+        return self.contract.functions.{{ function.name }}({% if function.inputs %}{{ function.inputs | join(', ') }}{% endif %}).call()
+        {% else %}
+        return self.contract.functions.{{ function.name }}({% if function.inputs %}{{ function.inputs | join(', ') }}{% endif %}).transact()
+        
+    def build_{{ function.name }}_transaction(self, {% if function.inputs %}{{ function.inputs | join(', ') }}, {% endif %}tx_params):
+        return self.contract.functions.{{ function.name }}({% if function.inputs %}{{ function.inputs | join(', ') }}{% endif %}).build_transaction(tx_params)
+    {% endif %}
+    {% endfor %}
+''')
+
+def generate_python_classes_from_abi(abi, contract_name, functions, output_dir):
+    class_name = contract_name + 'Client'  # Use the contract_name directly for proper capitalization
+    
+    selected_functions = []
+    for item in abi:
+        if item['type'] == 'function' and item['name'] in functions:
+            function = {
+                'name': item['name'],
+                'inputs': [input['name'] for input in item['inputs']],
+                'stateMutability': item['stateMutability'] if 'stateMutability' in item else 'nonpayable'
+            }
+            selected_functions.append(function)
+    
+    # Sort functions to have transact functions first and call functions after
+    selected_functions.sort(key=lambda x: x['stateMutability'] in ['view', 'pure'])
+    
+    rendered_class = class_template.render(
+        class_name=class_name,
+        contract_name=contract_name,
+        functions=selected_functions
+    )
+    
+    contract_output_dir = os.path.join(output_dir, contract_name)
+    os.makedirs(contract_output_dir, exist_ok=True)
+
+    output_file_path = os.path.join(contract_output_dir, f"{contract_name}_client.py")
+    with open(output_file_path, 'w') as output_file:
+        output_file.write(rendered_class)
+    
+    print(f"Generated {class_name} class from ABI")
+
+def main(config_path, output_dir):
+    with open(config_path, 'r') as config_file:
+        config = json.load(config_file)
+    
+
+        for contract in config['contracts']:
+            contract_name = contract['contract_name']
+            contract_address = contract['contract_address']
+            functions = contract['functions']
+
+            for attempt in range(3):  # Retry up to 3 times
+                try:
+                    abi = fetch_proxy_abi(contract_address, api_key)
+                    if abi:
+                        contract_output_dir = os.path.join(output_dir, contract_name)
+                        os.makedirs(contract_output_dir, exist_ok=True)
+
+                        save_abi(abi, os.path.join(contract_output_dir, f'{contract_name}.json'))
+                        generate_python_classes_from_abi(abi, contract_name, functions, output_dir)
+                        time.sleep(1)  # Wait for 1 seconds before moving to next contract
+                        break  # If successful, break out of the retry loop
+                    else:
+                        raise Exception("Failed to fetch ABI")
+                except Exception as e:
+                    print(f"Error on attempt {attempt + 1} for {contract_name}: {e}")
+                    time.sleep(2)  # Wait for 2 seconds before retrying
+
+if __name__ == "__main__":
+    config_path = os.path.join(os.path.dirname(__file__), 'config.json')
+    output_dir = os.path.join(os.path.dirname(__file__), '../abi')
+    os.makedirs(output_dir, exist_ok=True)
+    main(config_path, output_dir)
```

### Comparing `story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/scripts/generate_client_impl.py` & `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/scripts/generate_client_impl.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-import requests
-import json
-import os
-from jinja2 import Template
-from dotenv import load_dotenv
-import time
-
-# Load environment variables from .env file
-load_dotenv(os.path.join(os.path.dirname(__file__), '..', '..', '..', '.env'))
-
-# Get the API key from environment variables
-api_key = os.getenv('ETHERSCAN_API_KEY')
-if not api_key:
-    raise ValueError("Please set ETHERSCAN_API_KEY in the .env file")
-
-def fetch_abi(contract_address, api_key):
-    url = f"https://api-sepolia.etherscan.io/api?module=contract&action=getabi&address={contract_address}&apikey={api_key}"
-    response = requests.get(url)
-    response_json = response.json()
-    if response_json.get('status') == '1':
-        abi = json.loads(response_json['result'])
-        return abi
-    else:
-        raise Exception(f"Error fetching ABI for address {contract_address}: {response_json.get('message')}")
-
-def save_abi(abi, output_path):
-    with open(output_path, 'w') as abi_file:
-        json.dump(abi, abi_file, indent=2)
-
-class_template = Template('''
-import json
-import os
-from web3 import Web3
-
-class {{ class_name }}:
-    def __init__(self, web3: Web3, contract_address=None):
-        self.web3 = web3
-        abi_path = os.path.join(os.path.dirname(__file__), '{{ contract_name }}.json')
-        with open(abi_path, 'r') as abi_file:
-            abi = json.load(abi_file)
-        self.contract = self.web3.eth.contract(address=contract_address, abi=abi)
-    {% for function in functions %}
-    def {{ function.name }}(self, {% if function.inputs %}{{ function.inputs | join(', ') }}{% endif %}):
-        {% if function.stateMutability == 'view' or function.stateMutability == 'pure' %}
-        return self.contract.functions.{{ function.name }}({% if function.inputs %}{{ function.inputs | join(', ') }}{% endif %}).call()
-        {% else %}
-        return self.contract.functions.{{ function.name }}({% if function.inputs %}{{ function.inputs | join(', ') }}{% endif %}).transact()
-        
-    def build_{{ function.name }}_transaction(self, {% if function.inputs %}{{ function.inputs | join(', ') }}, {% endif %}tx_params):
-        return self.contract.functions.{{ function.name }}({% if function.inputs %}{{ function.inputs | join(', ') }}{% endif %}).build_transaction(tx_params)
-    {% endif %}
-    {% endfor %}
-''')
-
-def generate_python_classes_from_abi(abi, contract_name, functions, output_dir):
-    class_name = contract_name + 'Client'  # Use the contract_name directly for proper capitalization
-    
-    selected_functions = []
-    for item in abi:
-        if item['type'] == 'function' and item['name'] in functions:
-            function = {
-                'name': item['name'],
-                'inputs': [input['name'] for input in item['inputs']],
-                'stateMutability': item['stateMutability'] if 'stateMutability' in item else 'nonpayable'
-            }
-            selected_functions.append(function)
-    
-    # Sort functions to have transact functions first and call functions after
-    selected_functions.sort(key=lambda x: x['stateMutability'] in ['view', 'pure'])
-    
-    rendered_class = class_template.render(
-        class_name=class_name,
-        contract_name=contract_name,
-        functions=selected_functions
-    )
-    
-    contract_output_dir = os.path.join(output_dir, contract_name)
-    os.makedirs(contract_output_dir, exist_ok=True)
-
-    output_file_path = os.path.join(contract_output_dir, f"{contract_name}_client.py")
-    with open(output_file_path, 'w') as output_file:
-        output_file.write(rendered_class)
-    
-    print(f"Generated {class_name} class from ABI")
-
-def main(config_path, output_dir):
-    with open(config_path, 'r') as config_file:
-        config = json.load(config_file)
-    
-        for contract in config['contracts']:
-            contract_name = contract['contract_name']
-            contract_address = contract['contract_address']
-            functions = contract['functions']
-
-            for attempt in range(3):  # Retry up to 3 times
-                try:
-                    abi = fetch_abi(contract_address, api_key)
-                    if abi:
-                        contract_output_dir = os.path.join(output_dir, contract_name)
-                        os.makedirs(contract_output_dir, exist_ok=True)
-
-                        save_abi(abi, os.path.join(contract_output_dir, f'{contract_name}.json'))
-                        generate_python_classes_from_abi(abi, contract_name, functions, output_dir)
-                        time.sleep(1)  # Wait for 1 second before moving to the next contract
-                        break  # If successful, break out of the retry loop
-                    else:
-                        raise Exception("Failed to fetch ABI")
-                except Exception as e:
-                    print(f"Error on attempt {attempt + 1} for {contract_name}: {e}")
-                    time.sleep(2)  # Wait for 2 seconds before retrying
-
-if __name__ == "__main__":
-    config_path = os.path.join(os.path.dirname(__file__), 'config_impl.json')
-    output_dir = os.path.join(os.path.dirname(__file__), '../abi')
-    os.makedirs(output_dir, exist_ok=True)
-    main(config_path, output_dir)
+import requests
+import json
+import os
+from jinja2 import Template
+from dotenv import load_dotenv
+import time
+
+# Load environment variables from .env file
+load_dotenv(os.path.join(os.path.dirname(__file__), '..', '..', '..', '.env'))
+
+# Get the API key from environment variables
+api_key = os.getenv('ETHERSCAN_API_KEY')
+if not api_key:
+    raise ValueError("Please set ETHERSCAN_API_KEY in the .env file")
+
+def fetch_abi(contract_address, api_key):
+    url = f"https://api-sepolia.etherscan.io/api?module=contract&action=getabi&address={contract_address}&apikey={api_key}"
+    response = requests.get(url)
+    response_json = response.json()
+    if response_json.get('status') == '1':
+        abi = json.loads(response_json['result'])
+        return abi
+    else:
+        raise Exception(f"Error fetching ABI for address {contract_address}: {response_json.get('message')}")
+
+def save_abi(abi, output_path):
+    with open(output_path, 'w') as abi_file:
+        json.dump(abi, abi_file, indent=2)
+
+class_template = Template('''
+import json
+import os
+from web3 import Web3
+
+class {{ class_name }}:
+    def __init__(self, web3: Web3, contract_address=None):
+        self.web3 = web3
+        abi_path = os.path.join(os.path.dirname(__file__), '{{ contract_name }}.json')
+        with open(abi_path, 'r') as abi_file:
+            abi = json.load(abi_file)
+        self.contract = self.web3.eth.contract(address=contract_address, abi=abi)
+    {% for function in functions %}
+    def {{ function.name }}(self, {% if function.inputs %}{{ function.inputs | join(', ') }}{% endif %}):
+        {% if function.stateMutability == 'view' or function.stateMutability == 'pure' %}
+        return self.contract.functions.{{ function.name }}({% if function.inputs %}{{ function.inputs | join(', ') }}{% endif %}).call()
+        {% else %}
+        return self.contract.functions.{{ function.name }}({% if function.inputs %}{{ function.inputs | join(', ') }}{% endif %}).transact()
+        
+    def build_{{ function.name }}_transaction(self, {% if function.inputs %}{{ function.inputs | join(', ') }}, {% endif %}tx_params):
+        return self.contract.functions.{{ function.name }}({% if function.inputs %}{{ function.inputs | join(', ') }}{% endif %}).build_transaction(tx_params)
+    {% endif %}
+    {% endfor %}
+''')
+
+def generate_python_classes_from_abi(abi, contract_name, functions, output_dir):
+    class_name = contract_name + 'Client'  # Use the contract_name directly for proper capitalization
+    
+    selected_functions = []
+    for item in abi:
+        if item['type'] == 'function' and item['name'] in functions:
+            function = {
+                'name': item['name'],
+                'inputs': [input['name'] for input in item['inputs']],
+                'stateMutability': item['stateMutability'] if 'stateMutability' in item else 'nonpayable'
+            }
+            selected_functions.append(function)
+    
+    # Sort functions to have transact functions first and call functions after
+    selected_functions.sort(key=lambda x: x['stateMutability'] in ['view', 'pure'])
+    
+    rendered_class = class_template.render(
+        class_name=class_name,
+        contract_name=contract_name,
+        functions=selected_functions
+    )
+    
+    contract_output_dir = os.path.join(output_dir, contract_name)
+    os.makedirs(contract_output_dir, exist_ok=True)
+
+    output_file_path = os.path.join(contract_output_dir, f"{contract_name}_client.py")
+    with open(output_file_path, 'w') as output_file:
+        output_file.write(rendered_class)
+    
+    print(f"Generated {class_name} class from ABI")
+
+def main(config_path, output_dir):
+    with open(config_path, 'r') as config_file:
+        config = json.load(config_file)
+    
+        for contract in config['contracts']:
+            contract_name = contract['contract_name']
+            contract_address = contract['contract_address']
+            functions = contract['functions']
+
+            for attempt in range(3):  # Retry up to 3 times
+                try:
+                    abi = fetch_abi(contract_address, api_key)
+                    if abi:
+                        contract_output_dir = os.path.join(output_dir, contract_name)
+                        os.makedirs(contract_output_dir, exist_ok=True)
+
+                        save_abi(abi, os.path.join(contract_output_dir, f'{contract_name}.json'))
+                        generate_python_classes_from_abi(abi, contract_name, functions, output_dir)
+                        time.sleep(1)  # Wait for 1 second before moving to the next contract
+                        break  # If successful, break out of the retry loop
+                    else:
+                        raise Exception("Failed to fetch ABI")
+                except Exception as e:
+                    print(f"Error on attempt {attempt + 1} for {contract_name}: {e}")
+                    time.sleep(2)  # Wait for 2 seconds before retrying
+
+if __name__ == "__main__":
+    config_path = os.path.join(os.path.dirname(__file__), 'config_impl.json')
+    output_dir = os.path.join(os.path.dirname(__file__), '../abi')
+    os.makedirs(output_dir, exist_ok=True)
+    main(config_path, output_dir)
```

### Comparing `story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/story_client.py` & `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/story_client.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-# src/story_client.py
-
-import os
-import sys
-
-# Ensure the src directory is in the Python path
-current_dir = os.path.dirname(__file__)
-src_path = os.path.abspath(os.path.join(current_dir, '..'))
-if src_path not in sys.path:
-    sys.path.append(src_path)
-
-from story_protocol_python_sdk.resources.IPAsset import IPAsset
-from story_protocol_python_sdk.resources.License import License
-from story_protocol_python_sdk.resources.Royalty import Royalty
-
-class StoryClient:
-    def __init__(self, web3, account, chain_id):
-        if not web3 or not account:
-            raise ValueError("web3 and account must be provided")
-
-        self.web3 = web3
-        self.account = account
-        self.chain_id = chain_id
-
-        # Initialize clients only when accessed
-        self._ip_asset = None
-        self._license = None
-        self._royalty = None
-
-    @property
-    def IPAsset(self):
-        if self._ip_asset is None:
-            self._ip_asset = IPAsset(self.web3, self.account, self.chain_id)
-        return self._ip_asset
-
-    @property
-    def License(self):
-        if self._license is None:
-            self._license = License(self.web3, self.account, self.chain_id)
-        return self._license
-    
-    @property
-    def Royalty(self):
-        if self._royalty is None:
-            self._royalty = Royalty(self.web3, self.account, self.chain_id)
+# src/story_client.py
+
+import os
+import sys
+
+# Ensure the src directory is in the Python path
+current_dir = os.path.dirname(__file__)
+src_path = os.path.abspath(os.path.join(current_dir, '..'))
+if src_path not in sys.path:
+    sys.path.append(src_path)
+
+from story_protocol_python_sdk.resources.IPAsset import IPAsset
+from story_protocol_python_sdk.resources.License import License
+from story_protocol_python_sdk.resources.Royalty import Royalty
+
+class StoryClient:
+    def __init__(self, web3, account, chain_id):
+        if not web3 or not account:
+            raise ValueError("web3 and account must be provided")
+
+        self.web3 = web3
+        self.account = account
+        self.chain_id = chain_id
+
+        # Initialize clients only when accessed
+        self._ip_asset = None
+        self._license = None
+        self._royalty = None
+
+    @property
+    def IPAsset(self):
+        if self._ip_asset is None:
+            self._ip_asset = IPAsset(self.web3, self.account, self.chain_id)
+        return self._ip_asset
+
+    @property
+    def License(self):
+        if self._license is None:
+            self._license = License(self.web3, self.account, self.chain_id)
+        return self._license
+    
+    @property
+    def Royalty(self):
+        if self._royalty is None:
+            self._royalty = Royalty(self.web3, self.account, self.chain_id)
         return self._royalty
```

### Comparing `story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk/utils/transaction_utils.py` & `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk/utils/transaction_utils.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# src/story_protcol_python_sdk/utils/transaction_utils.py
-
-from web3 import Web3
-
-def build_and_send_transaction(web3: Web3, account, client_function, *client_args, tx_options=None):
-    try:
-        # If tx_options is provided, use the values; otherwise, do not include them
-        tx_options = tx_options or {}
-
-        # Build the transaction options
-        transaction_options = {
-            'from': account.address,
-            'nonce': web3.eth.get_transaction_count(account.address),
-        }
-
-        if 'gasPrice' in tx_options:
-            transaction_options['gasPrice'] = web3.to_wei(tx_options['gasPrice'], 'gwei')
-        if 'maxFeePerGas' in tx_options:
-            transaction_options['maxFeePerGas'] = tx_options['maxFeePerGas']
-
-        # Build the transaction using the client function and arguments
-        transaction = client_function(*client_args, transaction_options)
-
-        # Sign the transaction using the account object
-        signed_txn = account.sign_transaction(transaction)
-
-        # Send the transaction
-        tx_hash = web3.eth.send_raw_transaction(signed_txn.rawTransaction)
-
-        # Wait for the transaction receipt
-        tx_receipt = web3.eth.wait_for_transaction_receipt(tx_hash, timeout=300)  # 5 minutes timeout
-
-        return {
-            'txHash': tx_hash.hex(),
-            'txReceipt': tx_receipt
-        }
-
-    except Exception as e:
-        raise e
+# src/story_protcol_python_sdk/utils/transaction_utils.py
+
+from web3 import Web3
+
+def build_and_send_transaction(web3: Web3, account, client_function, *client_args, tx_options=None):
+    try:
+        # If tx_options is provided, use the values; otherwise, do not include them
+        tx_options = tx_options or {}
+
+        # Build the transaction options
+        transaction_options = {
+            'from': account.address,
+            'nonce': web3.eth.get_transaction_count(account.address),
+        }
+
+        if 'gasPrice' in tx_options:
+            transaction_options['gasPrice'] = web3.to_wei(tx_options['gasPrice'], 'gwei')
+        if 'maxFeePerGas' in tx_options:
+            transaction_options['maxFeePerGas'] = tx_options['maxFeePerGas']
+
+        # Build the transaction using the client function and arguments
+        transaction = client_function(*client_args, transaction_options)
+
+        # Sign the transaction using the account object
+        signed_txn = account.sign_transaction(transaction)
+
+        # Send the transaction
+        tx_hash = web3.eth.send_raw_transaction(signed_txn.rawTransaction)
+
+        # Wait for the transaction receipt
+        tx_receipt = web3.eth.wait_for_transaction_receipt(tx_hash, timeout=300)  # 5 minutes timeout
+
+        return {
+            'txHash': tx_hash.hex(),
+            'txReceipt': tx_receipt
+        }
+
+    except Exception as e:
+        raise e
```

### Comparing `story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk.egg-info/PKG-INFO` & `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-Metadata-Version: 2.1
-Name: story-protocol-python-sdk
-Version: 0.2.1
-Summary: A Python SDK for interacting with the Story Protocol.
-Home-page: https://github.com/storyprotocol/python-sdk
-Author: Andrew Chung
-Author-email: andrew@storyprotocol.xyz
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: web3>=5.0.0
-Requires-Dist: pytest
-Requires-Dist: python-dotenv
-
-# Story Protocol SDK
-
-Welcome to the documents for Story Protocol Python SDK. The Python SDK provides the APIs for developers to build applications with Story Protocol. By using the SDK, developers can create the resources like IP assets and perform actions to interact with the resource.
-
-## How to use Story Protocol SDK in Your Project
-
-### Install Story Protocol core SDK
-
-Suppose you already have a node project or created a new node project. First, you need to install `story_protocol_python_sdk` in your project. You can use one of the following command to install the package:
-
-Use `pip`:
-
-```
-pip install story_protocol_python_sdk web3
-```
-
-Besides the Story Protocol SDK package `story_protocol_python_sdk`, we also require the package `web3` (https://pypi.org/project/web3/) to access the DeFi wallet accounts.
-
-# Initiate SDK Client
-
-Next we can initiate the SDK Client by first setting up our wallet and then the client itself.
-
-## Set up your wallet
-
-The SDK supports using `web3` for initiating SDK client. Create a Python file and write the following code to initiate the client with a private key:
-
-> :information-source: Make sure to have WALLET_PRIVATE_KEY set up in your .env file.
-
-```Python main.py
-import os
-from dotenv import load_dotenv
-from web3 import Web3
-
-load_dotenv()
-private_key = os.getenv('WALLET_PRIVATE_KEY')
-rpc_url = os.getenv('RPC_PROVIDER_URL')
-
-# Initialize Web3
-web3 = Web3(Web3.HTTPProvider(rpc_url))
-
-# Set up the account with the private key
-account = web3.eth.account.from_key(private_key)
-```
-
-The preceding code created the `account` object for creating the SDK client.
-
-## Set up SDK client
-
-To set up the SDK client, import `StoryClient` from `story_protocol_python_sdk`. Write the following code, utilizing the `account` we created previously.
-
-> :information-source: Make sure to have RPC_PROVIDER_URL for your desired chain set up in your .env file. We recommend using the Sepolia network with `RPC_PROVIDER_URL=https://rpc.ankr.com/eth_sepolia`.
-
-```Python main.py
-from story_protocol_python_sdk import StoryClient
-
-# Create StoryClient instance
-sepolia_chain_id = 11155111
-story_client = StoryClient(web3, account, sepolia_chain_id)
-```
-
-## Release
-
-| Package                         | Description                                    |
-| :------------------------------ | :--------------------------------------------- |
-| [story_protocol_python_sdk](./src/story_protocol_python_sdk) | A Python SDK for interacting with the Story Protocol. |
-
-## Contributing
-
-Pull requests are welcome. For major changes, please open an issue first
-to discuss what you would like to change. Details see: [CONTRIBUTING](/CONTRIBUTING.md)
-
-Please make sure to update tests as appropriate.
-
-## License
-
-[MIT License](/LICENSE.md)
+Metadata-Version: 2.1
+Name: story-protocol-python-sdk
+Version: 0.2.2
+Summary: A Python SDK for interacting with the Story Protocol.
+Home-page: https://github.com/storyprotocol/python-sdk
+Author: Andrew Chung
+Author-email: andrew@storyprotocol.xyz
+License: MIT
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Story Protocol SDK
+
+Welcome to the documents for Story Protocol Python SDK. The Python SDK provides the APIs for developers to build applications with Story Protocol. By using the SDK, developers can create the resources like IP assets and perform actions to interact with the resource.
+
+## How to use Story Protocol SDK in Your Project
+
+### Install Story Protocol core SDK
+
+Suppose you already have a node project or created a new node project. First, you need to install `story_protocol_python_sdk` in your project. You can use one of the following command to install the package:
+
+Use `pip`:
+
+```
+pip install story_protocol_python_sdk web3
+```
+
+Besides the Story Protocol SDK package `story_protocol_python_sdk`, we also require the package `web3` (https://pypi.org/project/web3/) to access the DeFi wallet accounts.
+
+# Initiate SDK Client
+
+Next we can initiate the SDK Client by first setting up our wallet and then the client itself.
+
+## Set up your wallet
+
+The SDK supports using `web3` for initiating SDK client. Create a Python file and write the following code to initiate the client with a private key:
+
+> :information-source: Make sure to have WALLET_PRIVATE_KEY set up in your .env file.
+
+```Python main.py
+import os
+from dotenv import load_dotenv
+from web3 import Web3
+
+load_dotenv()
+private_key = os.getenv('WALLET_PRIVATE_KEY')
+rpc_url = os.getenv('RPC_PROVIDER_URL')
+
+# Initialize Web3
+web3 = Web3(Web3.HTTPProvider(rpc_url))
+
+# Set up the account with the private key
+account = web3.eth.account.from_key(private_key)
+```
+
+The preceding code created the `account` object for creating the SDK client.
+
+## Set up SDK client
+
+To set up the SDK client, import `StoryClient` from `story_protocol_python_sdk`. Write the following code, utilizing the `account` we created previously.
+
+> :information-source: Make sure to have RPC_PROVIDER_URL for your desired chain set up in your .env file. We recommend using the Sepolia network with `RPC_PROVIDER_URL=https://rpc.ankr.com/eth_sepolia`.
+
+```Python main.py
+from story_protocol_python_sdk import StoryClient
+
+# Create StoryClient instance
+sepolia_chain_id = 11155111
+story_client = StoryClient(web3, account, sepolia_chain_id)
+```
+
+## Release
+
+| Package                         | Description                                    |
+| :------------------------------ | :--------------------------------------------- |
+| [story_protocol_python_sdk](./src/story_protocol_python_sdk) | A Python SDK for interacting with the Story Protocol. |
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first
+to discuss what you would like to change. Details see: [CONTRIBUTING](/CONTRIBUTING.md)
+
+Please make sure to update tests as appropriate.
+
+## License
+
+[MIT License](/LICENSE.md)
+
+
```

### Comparing `story_protocol_python_sdk-0.2.1/src/story_protocol_python_sdk.egg-info/SOURCES.txt` & `story_protocol_python_sdk-0.2.2/src/story_protocol_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


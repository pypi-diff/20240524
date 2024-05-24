# Comparing `tmp/burst2safe-0.3.5.tar.gz` & `tmp/burst2safe-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burst2safe-0.3.5.tar", last modified: Thu May 16 14:26:32 2024, max compression
+gzip compressed data, was "burst2safe-0.4.0.tar", last modified: Fri May 24 13:44:18 2024, max compression
```

## Comparing `burst2safe-0.3.5.tar` & `burst2safe-0.4.0.tar`

### file list

```diff
@@ -1,115 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.805987 burst2safe-0.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.729986 burst2safe-0.3.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.733986 burst2safe-0.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/build-and-deploy-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/build-and-deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/bump-version.yml
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/changelog-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/labeled-pr-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/pytest-golden.yml
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/pytest-integration.yml
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/release-checklist-comment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/static-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-16 14:26:27.000000 burst2safe-0.3.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-16 14:26:27.000000 burst2safe-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-05-16 14:26:32.805987 burst2safe-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-05-16 14:26:27.000000 burst2safe-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-16 14:26:27.000000 burst2safe-0.3.5/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-16 14:26:27.000000 burst2safe-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 14:26:32.805987 burst2safe-0.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.725985 burst2safe-0.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.733986 burst2safe-0.3.5/src/burst2safe/
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    13777 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/burst2safe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.729986 burst2safe-0.3.5/src/burst2safe/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.733986 burst2safe-0.3.5/src/burst2safe/data/support_236/
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_236/s1-level-1-calibration.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_236/s1-level-1-measurement.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_236/s1-level-1-noise.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   147288 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_236/s1-level-1-product.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    62654 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_236/s1-object-types.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.737986 burst2safe-0.3.5/src/burst2safe/data/support_245/
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_245/s1-level-1-calibration.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_245/s1-level-1-measurement.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_245/s1-level-1-noise.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   147222 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_245/s1-level-1-product.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    62654 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_245/s1-object-types.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.737986 burst2safe-0.3.5/src/burst2safe/data/support_260/
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_260/s1-level-1-calibration.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_260/s1-level-1-measurement.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_260/s1-level-1-noise.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   147374 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_260/s1-level-1-product.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    62654 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_260/s1-object-types.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.737986 burst2safe-0.3.5/src/burst2safe/data/support_290/
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_290/s1-level-1-calibration.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_290/s1-level-1-measurement.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_290/s1-level-1-noise.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   147374 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_290/s1-level-1-product.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    60608 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_290/s1-object-types.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.741986 burst2safe-0.3.5/src/burst2safe/data/support_340/
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_340/s1-level-1-calibration.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_340/s1-level-1-measurement.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_340/s1-level-1-noise.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   149999 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_340/s1-level-1-product.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_340/s1-level-1-rfi.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    61552 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_340/s1-object-types.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.741986 burst2safe-0.3.5/src/burst2safe/data/support_371/
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_371/s1-level-1-calibration.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_371/s1-level-1-measurement.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_371/s1-level-1-noise.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   149999 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_371/s1-level-1-product.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_371/s1-level-1-rfi.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    61720 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_371/s1-object-types.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/product.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/rfi.py
--rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/safe.py
--rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/swath.py
--rw-r--r--   0 runner    (1001) docker     (127)     8595 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.805987 burst2safe-0.3.5/src/burst2safe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-05-16 14:26:32.000000 burst2safe-0.3.5/src/burst2safe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-16 14:26:32.000000 burst2safe-0.3.5/src/burst2safe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:26:32.000000 burst2safe-0.3.5/src/burst2safe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-16 14:26:32.000000 burst2safe-0.3.5/src/burst2safe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:26:32.000000 burst2safe-0.3.5/src/burst2safe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-16 14:26:32.000000 burst2safe-0.3.5/src/burst2safe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 14:26:32.000000 burst2safe-0.3.5/src/burst2safe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.741986 burst2safe-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.745986 burst2safe-0.3.5/tests/etc/
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/etc/identify_ipf_differences.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_burst2safe.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.757986 burst2safe-0.3.5/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)  6288473 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_data/S1A_IW_SLC__1SDV_20240408T015045_20240408T015113_053336_06778C_CB5D_VV.xml
--rw-r--r--   0 runner    (1001) docker     (127)  6073763 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_data/S1A_IW_SLC__1SDV_20240408T015111_20240408T015138_053336_06778C_CA9A_VV.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.797987 burst2safe-0.3.5/tests/test_data/ipf/
--rw-r--r--   0 runner    (1001) docker     (127)  5647017 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150117T170523_20150117T170551_004214_0051E7_AE35_VV.xml
--rw-r--r--   0 runner    (1001) docker     (127)  6067536 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150622T170528_20150622T170556_006489_0089B0_EFBC_VV.xml
--rw-r--r--   0 runner    (1001) docker     (127)  6114849 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_data/ipf/S1A_IW_SLC__1SDV_20160124T170510_20160124T170538_009639_00E0BA_7CC5_VV.xml
--rw-r--r--   0 runner    (1001) docker     (127)  6350843 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_data/ipf/S1A_IW_SLC__1SDV_20211223T170557_20211223T170624_041139_04E360_B8E2_VV.xml
--rw-r--r--   0 runner    (1001) docker     (127)  6564579 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_data/ipf/S1A_IW_SLC__1SDV_20240130T170606_20240130T170634_052339_065425_9A35_VV.xml
--rw-r--r--   0 runner    (1001) docker     (127)  6345069 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_data/ipf/S1B_IW_SLC__1SDV_20180507T170449_20180507T170517_010818_013C70_6B12_VV.xml
--rw-r--r--   0 runner    (1001) docker     (127)    36523 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_data/manifest_7C85.safe
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_golden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_ipf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_product.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_rfi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_safe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_swath.py
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:18.507823 burst2safe-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:18.431823 burst2safe-0.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-24 13:44:13.000000 burst2safe-0.4.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-24 13:44:13.000000 burst2safe-0.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:18.431823 burst2safe-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-24 13:44:13.000000 burst2safe-0.4.0/.github/workflows/build-and-deploy-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-24 13:44:13.000000 burst2safe-0.4.0/.github/workflows/build-and-deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-24 13:44:13.000000 burst2safe-0.4.0/.github/workflows/bump-version.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-24 13:44:13.000000 burst2safe-0.4.0/.github/workflows/changelog-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-24 13:44:13.000000 burst2safe-0.4.0/.github/workflows/labeled-pr-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-24 13:44:13.000000 burst2safe-0.4.0/.github/workflows/pytest-golden.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-24 13:44:13.000000 burst2safe-0.4.0/.github/workflows/pytest-integration.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-24 13:44:13.000000 burst2safe-0.4.0/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-24 13:44:13.000000 burst2safe-0.4.0/.github/workflows/release-checklist-comment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-24 13:44:13.000000 burst2safe-0.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-24 13:44:13.000000 burst2safe-0.4.0/.github/workflows/static-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-24 13:44:13.000000 burst2safe-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-24 13:44:13.000000 burst2safe-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-24 13:44:13.000000 burst2safe-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-05-24 13:44:18.507823 burst2safe-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9663 2024-05-24 13:44:13.000000 burst2safe-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-24 13:44:13.000000 burst2safe-0.4.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-24 13:44:13.000000 burst2safe-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 13:44:18.507823 burst2safe-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:18.427823 burst2safe-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:18.435823 burst2safe-0.4.0/src/burst2safe/
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13777 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/burst2safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/burst2stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:18.427823 burst2safe-0.4.0/src/burst2safe/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:18.435823 burst2safe-0.4.0/src/burst2safe/data/support_236/
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_236/s1-level-1-calibration.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_236/s1-level-1-measurement.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_236/s1-level-1-noise.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   147288 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_236/s1-level-1-product.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    62654 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_236/s1-object-types.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:18.439823 burst2safe-0.4.0/src/burst2safe/data/support_245/
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_245/s1-level-1-calibration.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_245/s1-level-1-measurement.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_245/s1-level-1-noise.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   147222 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_245/s1-level-1-product.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    62654 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_245/s1-object-types.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:18.439823 burst2safe-0.4.0/src/burst2safe/data/support_260/
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_260/s1-level-1-calibration.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_260/s1-level-1-measurement.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_260/s1-level-1-noise.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   147374 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_260/s1-level-1-product.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    62654 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_260/s1-object-types.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:18.439823 burst2safe-0.4.0/src/burst2safe/data/support_290/
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_290/s1-level-1-calibration.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_290/s1-level-1-measurement.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_290/s1-level-1-noise.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   147374 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_290/s1-level-1-product.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    60608 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_290/s1-object-types.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:18.443823 burst2safe-0.4.0/src/burst2safe/data/support_340/
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_340/s1-level-1-calibration.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_340/s1-level-1-measurement.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_340/s1-level-1-noise.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   149999 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_340/s1-level-1-product.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_340/s1-level-1-rfi.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    61552 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_340/s1-object-types.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:18.443823 burst2safe-0.4.0/src/burst2safe/data/support_371/
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_371/s1-level-1-calibration.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_371/s1-level-1-measurement.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_371/s1-level-1-noise.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   149999 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_371/s1-level-1-product.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_371/s1-level-1-rfi.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    61720 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/data/support_371/s1-object-types.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/rfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11134 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/swath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-05-24 13:44:13.000000 burst2safe-0.4.0/src/burst2safe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:18.507823 burst2safe-0.4.0/src/burst2safe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-05-24 13:44:18.000000 burst2safe-0.4.0/src/burst2safe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-24 13:44:18.000000 burst2safe-0.4.0/src/burst2safe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 13:44:18.000000 burst2safe-0.4.0/src/burst2safe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-24 13:44:18.000000 burst2safe-0.4.0/src/burst2safe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 13:44:17.000000 burst2safe-0.4.0/src/burst2safe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-24 13:44:18.000000 burst2safe-0.4.0/src/burst2safe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-24 13:44:18.000000 burst2safe-0.4.0/src/burst2safe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:18.447823 burst2safe-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:18.447823 burst2safe-0.4.0/tests/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/etc/identify_ipf_differences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_burst2safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:18.463823 burst2safe-0.4.0/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)  6288473 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_data/S1A_IW_SLC__1SDV_20240408T015045_20240408T015113_053336_06778C_CB5D_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  6073763 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_data/S1A_IW_SLC__1SDV_20240408T015111_20240408T015138_053336_06778C_CA9A_VV.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:18.499823 burst2safe-0.4.0/tests/test_data/ipf/
+-rw-r--r--   0 runner    (1001) docker     (127)  5647017 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150117T170523_20150117T170551_004214_0051E7_AE35_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  6067536 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150622T170528_20150622T170556_006489_0089B0_EFBC_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  6114849 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_data/ipf/S1A_IW_SLC__1SDV_20160124T170510_20160124T170538_009639_00E0BA_7CC5_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  6350843 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_data/ipf/S1A_IW_SLC__1SDV_20211223T170557_20211223T170624_041139_04E360_B8E2_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  6564579 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_data/ipf/S1A_IW_SLC__1SDV_20240130T170606_20240130T170634_052339_065425_9A35_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  6345069 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_data/ipf/S1B_IW_SLC__1SDV_20180507T170449_20180507T170517_010818_013C70_6B12_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    36523 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_data/manifest_7C85.safe
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_golden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_ipf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_rfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_swath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-05-24 13:44:13.000000 burst2safe-0.4.0/tests/test_utils.py
```

### Comparing `burst2safe-0.3.5/.github/workflows/build-and-deploy-test.yml` & `burst2safe-0.4.0/.github/workflows/build-and-deploy-test.yml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/.github/workflows/build-and-deploy.yml` & `burst2safe-0.4.0/.github/workflows/build-and-deploy.yml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/.github/workflows/pytest-golden.yml` & `burst2safe-0.4.0/.github/workflows/pytest-golden.yml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/.github/workflows/pytest-integration.yml` & `burst2safe-0.4.0/.github/workflows/pytest-integration.yml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/.github/workflows/pytest.yml` & `burst2safe-0.4.0/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/.github/workflows/static-analysis.yml` & `burst2safe-0.4.0/.github/workflows/static-analysis.yml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/.gitignore` & `burst2safe-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/CHANGELOG.md` & `burst2safe-0.4.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,28 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [PEP 440](https://www.python.org/dev/peps/pep-0440/)
 and uses [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.4.0]
+
+### Added
+* `burst2stack` tool for creating stacks of SAFEs.
+* The ability to specify swaths and minimum number of bursts when using tool.
+* The ability to specify the SAFE extent by either bounding box or vector file.
+
+### Fixed
+* `Safe.get_name()` so that it correctly parses `Safe` objects with only cross-pol data.
+
+### Changed
+* Moved all search/download functionality to `search.py` module.
+* `--bbox` argument to `--extent`.
+
 ## [0.3.5]
 
 ### Fixed
 * Polarization code now accurately reflects bursts contained in SAFE.
 * Measurement GeoTiff metadata now correctly specifies Sentinel-1 A or B.
 
 ### Added
```

### Comparing `burst2safe-0.3.5/LICENSE` & `burst2safe-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/PKG-INFO` & `burst2safe-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burst2safe
-Version: 0.3.5
+Version: 0.4.0
 Summary: A package for converting ASF-derived Sentinel-1 burst SLC products to the ESA SAFE format
 Author-email: Forrest Williams <ffwilliams2@alaska.edu>
 Project-URL: Homepage, https://github.com/forrestfwilliams/burst2safe
 Project-URL: Bug Tracker, https://github.com/forrestfwilliams/burst2safe/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -25,59 +25,79 @@
 Requires-Dist: pytest; extra == "develop"
 
 # burst2safe
 Utility for converting ASF-derived Sentinel-1 burst SLC products to the ESA SAFE format.
 
 **This is still a work in progress, and we recommend waiting until the release of version 1.0.0 for use in production environments!**
 
-## Credentials
-To use `burst2safe`, you must provide your Earthdata Login credentials via two environment variables 
-(`EARTHDATA_USERNAME` and `EARTHDATA_PASSWORD`), or via your `.netrc` file.
-
-If you do not already have an Earthdata account, you can sign up [here](https://urs.earthdata.nasa.gov/home). 
-
-If you would like to set up Earthdata Login via your `.netrc` file, check out this [guide](https://harmony.earthdata.nasa.gov/docs#getting-started) to get started.
-
-## Usage
+## Setup
+### Installation
 To use the tool, install it via pip:
 
 ```bash
 pip install burst2safe
 ```
 
 Or conda:
 ```bash
 conda install -c conda-forge burst2safe
 ```
 
-Then, run the `burst2safe` command line tool using the following structure:
+### Credentials
+To use `burst2safe`, you must provide your Earthdata Login credentials via two environment variables 
+(`EARTHDATA_USERNAME` and `EARTHDATA_PASSWORD`), or via your `.netrc` file.
+
+If you do not already have an Earthdata account, you can sign up [here](https://urs.earthdata.nasa.gov/home). 
+
+If you would like to set up Earthdata Login via your `.netrc` file, check out this [guide](https://harmony.earthdata.nasa.gov/docs#getting-started) to get started.
+
+## burst2safe usage
+The `burst2safe` command line tool can be run using the following structure:
 ```bash
-burst2safe --orbit 32861 --bbox 53.57 27.54 53.78 27.60 --pols VV VH
+burst2safe --orbit 32861 --extent 53.57 27.54 53.78 27.60 --pols VV VH
 ```
 Where:
 
 * `--orbit` is the absolute orbit number of the Sentinel-1 data.
-* `--bbox` is the bounding box of the area of interest in the format `minlon minlat maxlon maxlat`.
+* `--extent` is the area of interest as a bounding box in the format `minlon minlat maxlon maxlat` or as a path to a GDAL-compatible vector file.
 * `--pols` is the polarization of the Sentinel-1 data. Options are `VV`, `VH`, `HV`, and `HH`.
 
+In addition, the user can specify the swaths they want data for using the `--swaths` argument, and you can specify a minimum number of bursts per polarization/swath combination using the `--min-bursts` argument.
+
+The `--min-bursts` argument is useful for workflows that require a minimum number of bursts, such as Enhanced Spectral Diversity (ESD) processing within InSAR processing chains.
+
 For more control over the burst group, you can also provide specific burst granule IDs to be merged into a SAFE file using the following structure:
 ```bash
 burst2safe S1_136231_IW2_20200604T022312_VV_7C85-BURST S1_136232_IW2_20200604T022315_VV_7C85-BURST S1_136231_IW2_20200604T022312_VH_7C85-BURST S1_136232_IW2_20200604T022315_VH_7C85-BURST
 ```
 This search is equivalent to the previous search.
 To be eligible for processing, all burst granules must:
 
 1. Have the same acquisition mode
 1. Be from the same absolute orbit
 1. Be contiguous in time and space.
 1. Have the same footprint for all polarizations.
 
 The tool should raise an error if any of these conditions are not met.
 
-The output SAFE file will be created in the current directory.
+The output SAFE file will be created in the directory specified using the `--output-dir` argument, which defaults to the current directory.
+
+## burst2stack usage
+For those who want to create stacks of SAFEs (SAFEs covering the same region but from different dates), we have created the `burst2stack` tool. This tool has a similar structure as `burst2safe`, but with small changes to the CLI arguments.
+
+This includes:
+- Exclusion of the granules pathway
+- Specifying the relative instead of absolute orbit number
+- Adding a start date and end date argument
+
+An example command that runs `burst2stack` for the same area as the previous examples, but for a range of dates can be seen below:
+```bash
+burst2stack --rel-orbit 64 --start-date 2020-06-03 --end-date 2020-06-17 --extent 53.57 27.54 53.78 27.60 --pols VV
+```
+The usage of the `--extent`, `--pols`, `--swaths`, and `--min-bursts` arguments is the same as in `burst2safe`.
 
 ## Strategy
 `burst2safe` combines and reformats individual bursts into a SAFE file following the procedure described in the [Sentinel-1 Product Specification Document](https://sentinel.esa.int/web/sentinel/user-guides/sentinel-1-sar/document-library/-/asset_publisher/1dO7RF5fJMbd/content/sentinel-1-product-specification-from-ipf-360?_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_assetEntryId=4846613&_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_redirect=https%3A%2F%2Fsentinel.esa.int%2Fweb%2Fsentinel%2Fuser-guides%2Fsentinel-1-sar%2Fdocument-library%3Fp_p_id%3Dcom_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd%26p_p_lifecycle%3D0%26p_p_state%3Dnormal%26p_p_mode%3Dview%26_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_assetEntryId%3D4846613%26_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_cur%3D0%26p_r_p_resetCur%3Dfalse)
 In this document, ESA describes how to create an Assembled Sentinel-1 Level 1 product from individual Sentinel-1 Level 1 SAFEs. We use this same strategy to combine ASF-extracted burst SLC products into a SAFE file that should be compatible with any SAR processor currently capable of using Sentinel-1 Level SAFEs. For in-depth technical details of the implementation, we refer you to the Sentinel-1 Product Specification document above. However, it is important to know that ESA recommends merging Sentinel-1 data/metadata components using three primary strategies:
 
 ### Include
 A given data/metadata component is the same for all data slices, and any value can be used (i.e., polarization).
```

### Comparing `burst2safe-0.3.5/README.md` & `burst2safe-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,77 @@
 # burst2safe
 Utility for converting ASF-derived Sentinel-1 burst SLC products to the ESA SAFE format.
 
 **This is still a work in progress, and we recommend waiting until the release of version 1.0.0 for use in production environments!**
 
-## Credentials
-To use `burst2safe`, you must provide your Earthdata Login credentials via two environment variables 
-(`EARTHDATA_USERNAME` and `EARTHDATA_PASSWORD`), or via your `.netrc` file.
-
-If you do not already have an Earthdata account, you can sign up [here](https://urs.earthdata.nasa.gov/home). 
-
-If you would like to set up Earthdata Login via your `.netrc` file, check out this [guide](https://harmony.earthdata.nasa.gov/docs#getting-started) to get started.
-
-## Usage
+## Setup
+### Installation
 To use the tool, install it via pip:
 
 ```bash
 pip install burst2safe
 ```
 
 Or conda:
 ```bash
 conda install -c conda-forge burst2safe
 ```
 
-Then, run the `burst2safe` command line tool using the following structure:
+### Credentials
+To use `burst2safe`, you must provide your Earthdata Login credentials via two environment variables 
+(`EARTHDATA_USERNAME` and `EARTHDATA_PASSWORD`), or via your `.netrc` file.
+
+If you do not already have an Earthdata account, you can sign up [here](https://urs.earthdata.nasa.gov/home). 
+
+If you would like to set up Earthdata Login via your `.netrc` file, check out this [guide](https://harmony.earthdata.nasa.gov/docs#getting-started) to get started.
+
+## burst2safe usage
+The `burst2safe` command line tool can be run using the following structure:
 ```bash
-burst2safe --orbit 32861 --bbox 53.57 27.54 53.78 27.60 --pols VV VH
+burst2safe --orbit 32861 --extent 53.57 27.54 53.78 27.60 --pols VV VH
 ```
 Where:
 
 * `--orbit` is the absolute orbit number of the Sentinel-1 data.
-* `--bbox` is the bounding box of the area of interest in the format `minlon minlat maxlon maxlat`.
+* `--extent` is the area of interest as a bounding box in the format `minlon minlat maxlon maxlat` or as a path to a GDAL-compatible vector file.
 * `--pols` is the polarization of the Sentinel-1 data. Options are `VV`, `VH`, `HV`, and `HH`.
 
+In addition, the user can specify the swaths they want data for using the `--swaths` argument, and you can specify a minimum number of bursts per polarization/swath combination using the `--min-bursts` argument.
+
+The `--min-bursts` argument is useful for workflows that require a minimum number of bursts, such as Enhanced Spectral Diversity (ESD) processing within InSAR processing chains.
+
 For more control over the burst group, you can also provide specific burst granule IDs to be merged into a SAFE file using the following structure:
 ```bash
 burst2safe S1_136231_IW2_20200604T022312_VV_7C85-BURST S1_136232_IW2_20200604T022315_VV_7C85-BURST S1_136231_IW2_20200604T022312_VH_7C85-BURST S1_136232_IW2_20200604T022315_VH_7C85-BURST
 ```
 This search is equivalent to the previous search.
 To be eligible for processing, all burst granules must:
 
 1. Have the same acquisition mode
 1. Be from the same absolute orbit
 1. Be contiguous in time and space.
 1. Have the same footprint for all polarizations.
 
 The tool should raise an error if any of these conditions are not met.
 
-The output SAFE file will be created in the current directory.
+The output SAFE file will be created in the directory specified using the `--output-dir` argument, which defaults to the current directory.
+
+## burst2stack usage
+For those who want to create stacks of SAFEs (SAFEs covering the same region but from different dates), we have created the `burst2stack` tool. This tool has a similar structure as `burst2safe`, but with small changes to the CLI arguments.
+
+This includes:
+- Exclusion of the granules pathway
+- Specifying the relative instead of absolute orbit number
+- Adding a start date and end date argument
+
+An example command that runs `burst2stack` for the same area as the previous examples, but for a range of dates can be seen below:
+```bash
+burst2stack --rel-orbit 64 --start-date 2020-06-03 --end-date 2020-06-17 --extent 53.57 27.54 53.78 27.60 --pols VV
+```
+The usage of the `--extent`, `--pols`, `--swaths`, and `--min-bursts` arguments is the same as in `burst2safe`.
 
 ## Strategy
 `burst2safe` combines and reformats individual bursts into a SAFE file following the procedure described in the [Sentinel-1 Product Specification Document](https://sentinel.esa.int/web/sentinel/user-guides/sentinel-1-sar/document-library/-/asset_publisher/1dO7RF5fJMbd/content/sentinel-1-product-specification-from-ipf-360?_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_assetEntryId=4846613&_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_redirect=https%3A%2F%2Fsentinel.esa.int%2Fweb%2Fsentinel%2Fuser-guides%2Fsentinel-1-sar%2Fdocument-library%3Fp_p_id%3Dcom_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd%26p_p_lifecycle%3D0%26p_p_state%3Dnormal%26p_p_mode%3Dview%26_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_assetEntryId%3D4846613%26_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_cur%3D0%26p_r_p_resetCur%3Dfalse)
 In this document, ESA describes how to create an Assembled Sentinel-1 Level 1 product from individual Sentinel-1 Level 1 SAFEs. We use this same strategy to combine ASF-extracted burst SLC products into a SAFE file that should be compatible with any SAR processor currently capable of using Sentinel-1 Level SAFEs. For in-depth technical details of the implementation, we refer you to the Sentinel-1 Product Specification document above. However, it is important to know that ESA recommends merging Sentinel-1 data/metadata components using three primary strategies:
 
 ### Include
 A given data/metadata component is the same for all data slices, and any value can be used (i.e., polarization).
```

### Comparing `burst2safe-0.3.5/pyproject.toml` & `burst2safe-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
 [project.urls]
 Homepage = "https://github.com/forrestfwilliams/burst2safe"
 "Bug Tracker" ="https://github.com/forrestfwilliams/burst2safe/issues"
 
 [project.scripts]
 burst2safe = "burst2safe.burst2safe:main"
+burst2stack = "burst2safe.burst2stack:main"
 
 [project.optional-dependencies]
 develop = [
     "pytest",
 ]
 
 [tool.pytest.ini_options]
```

### Comparing `burst2safe-0.3.5/src/burst2safe/auth.py` & `burst2safe-0.4.0/src/burst2safe/auth.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/base.py` & `burst2safe-0.4.0/src/burst2safe/base.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/calibration.py` & `burst2safe-0.4.0/src/burst2safe/calibration.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_236/s1-level-1-calibration.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_236/s1-level-1-calibration.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_236/s1-level-1-noise.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_236/s1-level-1-noise.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_236/s1-level-1-product.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_236/s1-level-1-product.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_236/s1-object-types.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_236/s1-object-types.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_245/s1-level-1-calibration.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_245/s1-level-1-calibration.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_245/s1-level-1-noise.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_245/s1-level-1-noise.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_245/s1-level-1-product.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_245/s1-level-1-product.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_245/s1-object-types.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_245/s1-object-types.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_260/s1-level-1-calibration.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_260/s1-level-1-calibration.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_260/s1-level-1-noise.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_260/s1-level-1-noise.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_260/s1-level-1-product.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_260/s1-level-1-product.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_260/s1-object-types.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_260/s1-object-types.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_290/s1-level-1-calibration.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_290/s1-level-1-calibration.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_290/s1-level-1-noise.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_290/s1-level-1-noise.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_290/s1-level-1-product.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_290/s1-level-1-product.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_290/s1-object-types.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_290/s1-object-types.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_340/s1-level-1-calibration.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_340/s1-level-1-calibration.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_340/s1-level-1-noise.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_340/s1-level-1-noise.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_340/s1-level-1-product.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_340/s1-level-1-product.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_340/s1-level-1-rfi.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_340/s1-level-1-rfi.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_340/s1-object-types.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_340/s1-object-types.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_371/s1-level-1-calibration.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_371/s1-level-1-calibration.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_371/s1-level-1-noise.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_371/s1-level-1-noise.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_371/s1-level-1-product.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_371/s1-level-1-product.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_371/s1-level-1-rfi.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_371/s1-level-1-rfi.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/data/support_371/s1-object-types.xsd` & `burst2safe-0.4.0/src/burst2safe/data/support_371/s1-object-types.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/manifest.py` & `burst2safe-0.4.0/src/burst2safe/manifest.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/measurement.py` & `burst2safe-0.4.0/src/burst2safe/measurement.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/noise.py` & `burst2safe-0.4.0/src/burst2safe/noise.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/product.py` & `burst2safe-0.4.0/src/burst2safe/product.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/rfi.py` & `burst2safe-0.4.0/src/burst2safe/rfi.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/safe.py` & `burst2safe-0.4.0/src/burst2safe/safe.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
         Returns:
             The name of the SAFE file
         """
 
         platform, beam_mode, product_type = self.burst_infos[0].slc_granule.split('_')[:3]
 
-        pol_codes = {'HH': 'SH', 'VV': 'SV', 'HH_HV': 'DH', 'VH_VV': 'DV'}
+        pol_codes = {'HH': 'SH', 'VV': 'SV', 'VH': 'SV', 'HV': 'SV', 'HH_HV': 'DH', 'VH_VV': 'DV'}
         pols = sorted(list(set([x.polarization for x in self.burst_infos])))
         pol_code = pol_codes['_'.join(pols)]
         product_info = f'1S{pol_code}'
 
         min_date = min([x.date for x in self.burst_infos]).strftime('%Y%m%dT%H%M%S')
         max_date = max([x.date for x in self.burst_infos]).strftime('%Y%m%dT%H%M%S')
         absolute_orbit = f'{self.burst_infos[0].absolute_orbit:06d}'
```

### Comparing `burst2safe-0.3.5/src/burst2safe/swath.py` & `burst2safe-0.4.0/src/burst2safe/swath.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/src/burst2safe/utils.py` & `burst2safe-0.4.0/src/burst2safe/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import json
 import warnings
 from binascii import crc_hqx
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from pathlib import Path
 from typing import Dict, Iterable, List, Optional
 
 import asf_search
 import lxml.etree as ET
 from asf_search.Products.S1BurstProduct import S1BurstProduct
-from osgeo import gdal
+from osgeo import gdal, ogr, osr
+from shapely.geometry import shape
 
 
 gdal.UseExceptions()
 warnings.filterwarnings('ignore')
 
 
 @dataclass
@@ -258,7 +260,37 @@
         element: The element to set the text of.
         text: The text to set the element to.
     """
     if not isinstance(text, str) and not isinstance(text, int):
         raise ValueError('Text must be a string or an integer.')
 
     element.text = str(text)
+
+
+def vector_to_shapely_latlon_polygon(vector_file_path):
+    dataset = ogr.Open(vector_file_path)
+
+    if dataset is None:
+        raise ValueError(f'Could not open file: {vector_file_path}')
+
+    layer = dataset.GetLayer()
+
+    feature_count = layer.GetFeatureCount()
+    if feature_count != 1:
+        raise ValueError(f'File contains {feature_count} features, but exactly one is required.')
+
+    feature = layer.GetFeature(0)
+    geom = feature.GetGeometryRef()
+    if geom.GetGeometryType() != ogr.wkbPolygon:
+        raise ValueError('The feature is not a polygon.')
+
+    source_srs = layer.GetSpatialRef()
+    if int(source_srs.GetAuthorityCode(None)) != 4326:
+        target_srs = osr.SpatialReference()
+        target_srs.ImportFromEPSG(4326)
+        transform = osr.CoordinateTransformation(source_srs, target_srs)
+        geom.Transform(transform)
+
+    polygon = shape(json.loads(geom.ExportToJson()))
+    dataset = None
+
+    return polygon
```

### Comparing `burst2safe-0.3.5/src/burst2safe.egg-info/PKG-INFO` & `burst2safe-0.4.0/src/burst2safe.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burst2safe
-Version: 0.3.5
+Version: 0.4.0
 Summary: A package for converting ASF-derived Sentinel-1 burst SLC products to the ESA SAFE format
 Author-email: Forrest Williams <ffwilliams2@alaska.edu>
 Project-URL: Homepage, https://github.com/forrestfwilliams/burst2safe
 Project-URL: Bug Tracker, https://github.com/forrestfwilliams/burst2safe/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -25,59 +25,79 @@
 Requires-Dist: pytest; extra == "develop"
 
 # burst2safe
 Utility for converting ASF-derived Sentinel-1 burst SLC products to the ESA SAFE format.
 
 **This is still a work in progress, and we recommend waiting until the release of version 1.0.0 for use in production environments!**
 
-## Credentials
-To use `burst2safe`, you must provide your Earthdata Login credentials via two environment variables 
-(`EARTHDATA_USERNAME` and `EARTHDATA_PASSWORD`), or via your `.netrc` file.
-
-If you do not already have an Earthdata account, you can sign up [here](https://urs.earthdata.nasa.gov/home). 
-
-If you would like to set up Earthdata Login via your `.netrc` file, check out this [guide](https://harmony.earthdata.nasa.gov/docs#getting-started) to get started.
-
-## Usage
+## Setup
+### Installation
 To use the tool, install it via pip:
 
 ```bash
 pip install burst2safe
 ```
 
 Or conda:
 ```bash
 conda install -c conda-forge burst2safe
 ```
 
-Then, run the `burst2safe` command line tool using the following structure:
+### Credentials
+To use `burst2safe`, you must provide your Earthdata Login credentials via two environment variables 
+(`EARTHDATA_USERNAME` and `EARTHDATA_PASSWORD`), or via your `.netrc` file.
+
+If you do not already have an Earthdata account, you can sign up [here](https://urs.earthdata.nasa.gov/home). 
+
+If you would like to set up Earthdata Login via your `.netrc` file, check out this [guide](https://harmony.earthdata.nasa.gov/docs#getting-started) to get started.
+
+## burst2safe usage
+The `burst2safe` command line tool can be run using the following structure:
 ```bash
-burst2safe --orbit 32861 --bbox 53.57 27.54 53.78 27.60 --pols VV VH
+burst2safe --orbit 32861 --extent 53.57 27.54 53.78 27.60 --pols VV VH
 ```
 Where:
 
 * `--orbit` is the absolute orbit number of the Sentinel-1 data.
-* `--bbox` is the bounding box of the area of interest in the format `minlon minlat maxlon maxlat`.
+* `--extent` is the area of interest as a bounding box in the format `minlon minlat maxlon maxlat` or as a path to a GDAL-compatible vector file.
 * `--pols` is the polarization of the Sentinel-1 data. Options are `VV`, `VH`, `HV`, and `HH`.
 
+In addition, the user can specify the swaths they want data for using the `--swaths` argument, and you can specify a minimum number of bursts per polarization/swath combination using the `--min-bursts` argument.
+
+The `--min-bursts` argument is useful for workflows that require a minimum number of bursts, such as Enhanced Spectral Diversity (ESD) processing within InSAR processing chains.
+
 For more control over the burst group, you can also provide specific burst granule IDs to be merged into a SAFE file using the following structure:
 ```bash
 burst2safe S1_136231_IW2_20200604T022312_VV_7C85-BURST S1_136232_IW2_20200604T022315_VV_7C85-BURST S1_136231_IW2_20200604T022312_VH_7C85-BURST S1_136232_IW2_20200604T022315_VH_7C85-BURST
 ```
 This search is equivalent to the previous search.
 To be eligible for processing, all burst granules must:
 
 1. Have the same acquisition mode
 1. Be from the same absolute orbit
 1. Be contiguous in time and space.
 1. Have the same footprint for all polarizations.
 
 The tool should raise an error if any of these conditions are not met.
 
-The output SAFE file will be created in the current directory.
+The output SAFE file will be created in the directory specified using the `--output-dir` argument, which defaults to the current directory.
+
+## burst2stack usage
+For those who want to create stacks of SAFEs (SAFEs covering the same region but from different dates), we have created the `burst2stack` tool. This tool has a similar structure as `burst2safe`, but with small changes to the CLI arguments.
+
+This includes:
+- Exclusion of the granules pathway
+- Specifying the relative instead of absolute orbit number
+- Adding a start date and end date argument
+
+An example command that runs `burst2stack` for the same area as the previous examples, but for a range of dates can be seen below:
+```bash
+burst2stack --rel-orbit 64 --start-date 2020-06-03 --end-date 2020-06-17 --extent 53.57 27.54 53.78 27.60 --pols VV
+```
+The usage of the `--extent`, `--pols`, `--swaths`, and `--min-bursts` arguments is the same as in `burst2safe`.
 
 ## Strategy
 `burst2safe` combines and reformats individual bursts into a SAFE file following the procedure described in the [Sentinel-1 Product Specification Document](https://sentinel.esa.int/web/sentinel/user-guides/sentinel-1-sar/document-library/-/asset_publisher/1dO7RF5fJMbd/content/sentinel-1-product-specification-from-ipf-360?_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_assetEntryId=4846613&_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_redirect=https%3A%2F%2Fsentinel.esa.int%2Fweb%2Fsentinel%2Fuser-guides%2Fsentinel-1-sar%2Fdocument-library%3Fp_p_id%3Dcom_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd%26p_p_lifecycle%3D0%26p_p_state%3Dnormal%26p_p_mode%3Dview%26_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_assetEntryId%3D4846613%26_com_liferay_asset_publisher_web_portlet_AssetPublisherPortlet_INSTANCE_1dO7RF5fJMbd_cur%3D0%26p_r_p_resetCur%3Dfalse)
 In this document, ESA describes how to create an Assembled Sentinel-1 Level 1 product from individual Sentinel-1 Level 1 SAFEs. We use this same strategy to combine ASF-extracted burst SLC products into a SAFE file that should be compatible with any SAR processor currently capable of using Sentinel-1 Level SAFEs. For in-depth technical details of the implementation, we refer you to the Sentinel-1 Product Specification document above. However, it is important to know that ESA recommends merging Sentinel-1 data/metadata components using three primary strategies:
 
 ### Include
 A given data/metadata component is the same for all data slices, and any value can be used (i.e., polarization).
```

### Comparing `burst2safe-0.3.5/src/burst2safe.egg-info/SOURCES.txt` & `burst2safe-0.4.0/src/burst2safe.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,23 @@
 .github/workflows/pytest.yml
 .github/workflows/release-checklist-comment.yml
 .github/workflows/release.yml
 .github/workflows/static-analysis.yml
 src/burst2safe/auth.py
 src/burst2safe/base.py
 src/burst2safe/burst2safe.py
+src/burst2safe/burst2stack.py
 src/burst2safe/calibration.py
 src/burst2safe/manifest.py
 src/burst2safe/measurement.py
 src/burst2safe/noise.py
 src/burst2safe/product.py
 src/burst2safe/rfi.py
 src/burst2safe/safe.py
+src/burst2safe/search.py
 src/burst2safe/swath.py
 src/burst2safe/utils.py
 src/burst2safe.egg-info/PKG-INFO
 src/burst2safe.egg-info/SOURCES.txt
 src/burst2safe.egg-info/dependency_links.txt
 src/burst2safe.egg-info/entry_points.txt
 src/burst2safe.egg-info/not-zip-safe
@@ -78,14 +80,15 @@
 tests/test_ipf.py
 tests/test_manifest.py
 tests/test_measurement.py
 tests/test_noise.py
 tests/test_product.py
 tests/test_rfi.py
 tests/test_safe.py
+tests/test_search.py
 tests/test_swath.py
 tests/test_utils.py
 tests/etc/identify_ipf_differences.py
 tests/test_data/S1A_IW_SLC__1SDV_20240408T015045_20240408T015113_053336_06778C_CB5D_VV.xml
 tests/test_data/S1A_IW_SLC__1SDV_20240408T015111_20240408T015138_053336_06778C_CA9A_VV.xml
 tests/test_data/manifest_7C85.safe
 tests/test_data/ipf/S1A_IW_SLC__1SDV_20150117T170523_20150117T170551_004214_0051E7_AE35_VV.xml
```

### Comparing `burst2safe-0.3.5/tests/conftest.py` & `burst2safe-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/tests/etc/identify_ipf_differences.py` & `burst2safe-0.4.0/tests/etc/identify_ipf_differences.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/tests/helpers.py` & `burst2safe-0.4.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/tests/test_auth.py` & `burst2safe-0.4.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/tests/test_base.py` & `burst2safe-0.4.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/tests/test_data/S1A_IW_SLC__1SDV_20240408T015045_20240408T015113_053336_06778C_CB5D_VV.xml` & `burst2safe-0.4.0/tests/test_data/S1A_IW_SLC__1SDV_20240408T015045_20240408T015113_053336_06778C_CB5D_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/tests/test_data/S1A_IW_SLC__1SDV_20240408T015111_20240408T015138_053336_06778C_CA9A_VV.xml` & `burst2safe-0.4.0/tests/test_data/S1A_IW_SLC__1SDV_20240408T015111_20240408T015138_053336_06778C_CA9A_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150117T170523_20150117T170551_004214_0051E7_AE35_VV.xml` & `burst2safe-0.4.0/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150117T170523_20150117T170551_004214_0051E7_AE35_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150622T170528_20150622T170556_006489_0089B0_EFBC_VV.xml` & `burst2safe-0.4.0/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150622T170528_20150622T170556_006489_0089B0_EFBC_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/tests/test_data/ipf/S1A_IW_SLC__1SDV_20160124T170510_20160124T170538_009639_00E0BA_7CC5_VV.xml` & `burst2safe-0.4.0/tests/test_data/ipf/S1A_IW_SLC__1SDV_20160124T170510_20160124T170538_009639_00E0BA_7CC5_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/tests/test_data/ipf/S1A_IW_SLC__1SDV_20211223T170557_20211223T170624_041139_04E360_B8E2_VV.xml` & `burst2safe-0.4.0/tests/test_data/ipf/S1A_IW_SLC__1SDV_20211223T170557_20211223T170624_041139_04E360_B8E2_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/tests/test_data/ipf/S1A_IW_SLC__1SDV_20240130T170606_20240130T170634_052339_065425_9A35_VV.xml` & `burst2safe-0.4.0/tests/test_data/ipf/S1A_IW_SLC__1SDV_20240130T170606_20240130T170634_052339_065425_9A35_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/tests/test_data/ipf/S1B_IW_SLC__1SDV_20180507T170449_20180507T170517_010818_013C70_6B12_VV.xml` & `burst2safe-0.4.0/tests/test_data/ipf/S1B_IW_SLC__1SDV_20180507T170449_20180507T170517_010818_013C70_6B12_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/tests/test_data/manifest_7C85.safe` & `burst2safe-0.4.0/tests/test_data/manifest_7C85.safe`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/tests/test_ipf.py` & `burst2safe-0.4.0/tests/test_ipf.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/tests/test_manifest.py` & `burst2safe-0.4.0/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/tests/test_measurement.py` & `burst2safe-0.4.0/tests/test_measurement.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/tests/test_noise.py` & `burst2safe-0.4.0/tests/test_noise.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/tests/test_product.py` & `burst2safe-0.4.0/tests/test_product.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/tests/test_safe.py` & `burst2safe-0.4.0/tests/test_safe.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.5/tests/test_swath.py` & `burst2safe-0.4.0/tests/test_swath.py`

 * *Files identical despite different names*


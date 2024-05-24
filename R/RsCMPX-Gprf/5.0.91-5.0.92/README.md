# Comparing `tmp/RsCMPX_Gprf-5.0.91.tar.gz` & `tmp/RsCMPX_Gprf-5.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\RsCMPX_Gprf-5.0.91.tar", last modified: Wed Apr 24 14:08:01 2024, max compression
+gzip compressed data, was "dist\RsCMPX_Gprf-5.0.92.tar", last modified: Fri May 24 14:33:54 2024, max compression
```

## Comparing `RsCMPX_Gprf-5.0.91.tar` & `RsCMPX_Gprf-5.0.92.tar`

### file list

```diff
@@ -1,1131 +1,1132 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.938099 RsCMPX_Gprf-5.0.91/
--rw-rw-rw-   0        0        0     3474 2024-04-24 14:08:01.937101 RsCMPX_Gprf-5.0.91/PKG-INFO
--rw-rw-rw-   0        0        0     1868 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.397885 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.423816 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/CustomFiles/
--rw-rw-rw-   0        0        0       90 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/CustomFiles/__init__.py
--rw-rw-rw-   0        0        0     3725 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/CustomFiles/events.py
--rw-rw-rw-   0        0        0     4916 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/CustomFiles/reliability.py
--rw-rw-rw-   0        0        0    21844 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/CustomFiles/utilities.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.426807 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.428803 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.431795 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.433789 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/Attenuation/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.441768 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/
--rw-rw-rw-   0        0        0     1338 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/Globale.py
--rw-rw-rw-   0        0        0     1372 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/Tenvironment.py
--rw-rw-rw-   0        0        0     1363 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/__init__.py
--rw-rw-rw-   0        0        0     1121 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/Attenuation/__init__.py
--rw-rw-rw-   0        0        0     1062 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.443764 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.446754 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.453736 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/
--rw-rw-rw-   0        0        0     1219 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/Rx.py
--rw-rw-rw-   0        0        0     1219 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/Tx.py
--rw-rw-rw-   0        0        0     1243 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/__init__.py
--rw-rw-rw-   0        0        0     1091 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/__init__.py
--rw-rw-rw-   0        0        0     1044 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/__init__.py
--rw-rw-rw-   0        0        0     1289 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.455731 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.459720 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.461714 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.466701 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/ExtPwrSensor/
--rw-rw-rw-   0        0        0     2920 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/ExtPwrSensor/Zero.py
--rw-rw-rw-   0        0        0     1040 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/ExtPwrSensor/__init__.py
--rw-rw-rw-   0        0        0     1097 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/__init__.py
--rw-rw-rw-   0        0        0     1029 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.469693 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.472685 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.478670 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/Measurement/
--rw-rw-rw-   0        0        0     2351 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1077 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.480664 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Cdma/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.486649 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/
--rw-rw-rw-   0        0        0     2336 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Cdma/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.489640 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.492632 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.497618 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/
--rw-rw-rw-   0        0        0     1896 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/Group.py
--rw-rw-rw-   0        0        0     2676 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/__init__.py
--rw-rw-rw-   0        0        0     1031 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.505598 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/
--rw-rw-rw-   0        0        0      891 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/Ploss.py
--rw-rw-rw-   0        0        0     2406 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1269 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1312 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.508590 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gsm/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.513576 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/
--rw-rw-rw-   0        0        0     2333 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1047 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gsm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.515571 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Lte/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.530530 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Lte/Measurement/
--rw-rw-rw-   0        0        0     2333 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Lte/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Lte/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1047 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Lte/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.518563 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/LteDl/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.524546 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/LteDl/Measurement/
--rw-rw-rw-   0        0        0     2339 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/LteDl/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/LteDl/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/LteDl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.532525 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Niot/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.540504 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Niot/Measurement/
--rw-rw-rw-   0        0        0     2336 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Niot/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Niot/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Niot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.544494 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrDl/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.552473 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrDl/Measurement/
--rw-rw-rw-   0        0        0     2336 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrDl/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrDl/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrDl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.555465 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrMmw/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.560451 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrMmw/Measurement/
--rw-rw-rw-   0        0        0     2339 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrMmw/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrMmw/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrMmw/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.563444 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrSub/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.570425 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrSub/Measurement/
--rw-rw-rw-   0        0        0     2339 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrSub/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrSub/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrSub/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.578403 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.589374 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Attenuation/
--rw-rw-rw-   0        0        0     1238 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Attenuation/CorrectionTable.py
--rw-rw-rw-   0        0        0     1121 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Attenuation/__init__.py
--rw-rw-rw-   0        0        0      813 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Reset.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.605331 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Rf42/
--rw-rw-rw-   0        0        0      926 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Rf42/Box.py
--rw-rw-rw-   0        0        0      990 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Rf42/__init__.py
--rw-rw-rw-   0        0        0     1236 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Rrhead.py
--rw-rw-rw-   0        0        0     2122 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.611314 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Tenvironment/
--rw-rw-rw-   0        0        0     1241 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Tenvironment/Connectors.py
--rw-rw-rw-   0        0        0     1496 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Tenvironment/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.614307 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Uwb/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.621289 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Uwb/Measurement/
--rw-rw-rw-   0        0        0     2333 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Uwb/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Uwb/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1047 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Uwb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.624280 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wcdma/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.629267 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wcdma/Measurement/
--rw-rw-rw-   0        0        0     2339 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wcdma/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wcdma/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wcdma/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.632260 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wlan/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.638243 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wlan/Measurement/
--rw-rw-rw-   0        0        0     2336 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wlan/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wlan/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wlan/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.641235 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wpan/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.647220 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wpan/Measurement/
--rw-rw-rw-   0        0        0     2336 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wpan/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wpan/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wpan/__init__.py
--rw-rw-rw-   0        0        0     4439 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.650211 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.653203 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.656195 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.659187 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.662179 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.665171 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.671155 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/Tx/
--rw-rw-rw-   0        0        0     2556 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/Tx/Single.py
--rw-rw-rw-   0        0        0     1012 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/Tx/__init__.py
--rw-rw-rw-   0        0        0     3626 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/__init__.py
--rw-rw-rw-   0        0        0     2709 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/__init__.py
--rw-rw-rw-   0        0        0     1958 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/__init__.py
--rw-rw-rw-   0        0        0     2022 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.681128 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.691101 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/
--rw-rw-rw-   0        0        0     1377 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/IqFile.py
--rw-rw-rw-   0        0        0     3152 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/Sall.py
--rw-rw-rw-   0        0        0     4093 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/__init__.py
--rw-rw-rw-   0        0        0     1259 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Correction.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.703070 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/
--rw-rw-rw-   0        0        0     2461 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Attenuation.py
--rw-rw-rw-   0        0        0     2082 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Auto.py
--rw-rw-rw-   0        0        0     3239 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Average.py
--rw-rw-rw-   0        0        0     8936 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.710051 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/
--rw-rw-rw-   0        0        0     6166 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/PeakSearch.py
--rw-rw-rw-   0        0        0    12393 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.723016 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/
--rw-rw-rw-   0        0        0     2570 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/Capture.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.732989 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/
--rw-rw-rw-   0        0        0     1907 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/Bandpass.py
--rw-rw-rw-   0        0        0     1645 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/Gauss.py
--rw-rw-rw-   0        0        0     2459 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/__init__.py
--rw-rw-rw-   0        0        0     1370 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/IqSettings.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.746953 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/
--rw-rw-rw-   0        0        0     2731 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/EnvelopePower.py
--rw-rw-rw-   0        0        0     2675 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/Frequency.py
--rw-rw-rw-   0        0        0     2143 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/Sstop.py
--rw-rw-rw-   0        0        0     5475 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/__init__.py
--rw-rw-rw-   0        0        0     1479 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/Trigger.py
--rw-rw-rw-   0        0        0    15177 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.755929 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.775876 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/
--rw-rw-rw-   0        0        0     3789 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/EnvelopePower.py
--rw-rw-rw-   0        0        0     3053 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Frequency.py
--rw-rw-rw-   0        0        0     3118 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Retrigger.py
--rw-rw-rw-   0        0        0     2425 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Sstop.py
--rw-rw-rw-   0        0        0     5646 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/__init__.py
--rw-rw-rw-   0        0        0     1463 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/Trigger.py
--rw-rw-rw-   0        0        0    10961 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.780862 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.787843 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/
--rw-rw-rw-   0        0        0     1969 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/Frequency.py
--rw-rw-rw-   0        0        0     1891 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/__init__.py
--rw-rw-rw-   0        0        0     6078 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.795822 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.801806 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/ListPy/
--rw-rw-rw-   0        0        0     3163 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/ListPy/Frequency.py
--rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/ListPy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.808787 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/
--rw-rw-rw-   0        0        0     3270 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/File.py
--rw-rw-rw-   0        0        0     1904 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/__init__.py
--rw-rw-rw-   0        0        0     1386 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/View.py
--rw-rw-rw-   0        0        0     3556 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.818761 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/
--rw-rw-rw-   0        0        0      900 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/Catalog.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.829732 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/
--rw-rw-rw-   0        0        0     1469 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/Bandpass.py
--rw-rw-rw-   0        0        0     1445 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/Gauss.py
--rw-rw-rw-   0        0        0     2945 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.860648 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/
--rw-rw-rw-   0        0        0     2423 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Cidx.py
--rw-rw-rw-   0        0        0     3755 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/EnvelopePower.py
--rw-rw-rw-   0        0        0     3019 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Frequency.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.866633 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.875609 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/Catalog/
--rw-rw-rw-   0        0        0     1302 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/Catalog/Connection.py
--rw-rw-rw-   0        0        0     1069 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/Catalog/__init__.py
--rw-rw-rw-   0        0        0     2342 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/Connection.py
--rw-rw-rw-   0        0        0     2119 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/__init__.py
--rw-rw-rw-   0        0        0     3464 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/IqData.py
--rw-rw-rw-   0        0        0     3204 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Irepetition.py
--rw-rw-rw-   0        0        0     2828 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/ParameterSetList.py
--rw-rw-rw-   0        0        0     3080 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Retrigger.py
--rw-rw-rw-   0        0        0     2419 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Sstop.py
--rw-rw-rw-   0        0        0    15308 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.891566 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/
--rw-rw-rw-   0        0        0     1126 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Catalog.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.899545 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.907523 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandpass/
--rw-rw-rw-   0        0        0     3261 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandpass/Bandwidth.py
--rw-rw-rw-   0        0        0     1066 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandpass/__init__.py
--rw-rw-rw-   0        0        0     2729 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandwidth.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.913507 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Gauss/
--rw-rw-rw-   0        0        0     3285 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Gauss/Bandwidth.py
--rw-rw-rw-   0        0        0     1051 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Gauss/__init__.py
--rw-rw-rw-   0        0        0     4452 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/TypePy.py
--rw-rw-rw-   0        0        0     1780 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/__init__.py
--rw-rw-rw-   0        0        0     3391 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Mlength.py
--rw-rw-rw-   0        0        0     2509 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/PdefSet.py
--rw-rw-rw-   0        0        0     3053 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Slength.py
--rw-rw-rw-   0        0        0     3387 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/__init__.py
--rw-rw-rw-   0        0        0     1449 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/Trigger.py
--rw-rw-rw-   0        0        0    11165 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.920489 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/RfSettings/
--rw-rw-rw-   0        0        0     1285 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/RfSettings/LrStart.py
--rw-rw-rw-   0        0        0     9793 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/RfSettings/__init__.py
--rw-rw-rw-   0        0        0     1431 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Scenario.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.924478 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.936447 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/
--rw-rw-rw-   0        0        0     2118 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Rbw.py
--rw-rw-rw-   0        0        0     2188 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Swt.py
--rw-rw-rw-   0        0        0     2196 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Vbw.py
--rw-rw-rw-   0        0        0     3640 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.942430 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/Frequency/
--rw-rw-rw-   0        0        0     2365 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/Frequency/Span.py
--rw-rw-rw-   0        0        0     4653 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/Frequency/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.952404 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/
--rw-rw-rw-   0        0        0     3239 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/Rbw.py
--rw-rw-rw-   0        0        0     2184 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/Vbw.py
--rw-rw-rw-   0        0        0     3844 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/__init__.py
--rw-rw-rw-   0        0        0     5241 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/__init__.py
--rw-rw-rw-   0        0        0     3857 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1315 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.963374 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.967364 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.971353 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.983321 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/
--rw-rw-rw-   0        0        0     1672 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/Globale.py
--rw-rw-rw-   0        0        0     1706 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/Tenvironment.py
--rw-rw-rw-   0        0        0     1310 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/__init__.py
--rw-rw-rw-   0        0        0     1055 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/__init__.py
--rw-rw-rw-   0        0        0     1121 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.996287 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Control/
--rw-rw-rw-   0        0        0     1162 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Control/Reboot.py
--rw-rw-rw-   0        0        0     1171 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Control/Restart.py
--rw-rw-rw-   0        0        0     1180 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Control/Shutdown.py
--rw-rw-rw-   0        0        0     1525 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Control/__init__.py
--rw-rw-rw-   0        0        0     2171 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Edevice.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.009251 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/
--rw-rw-rw-   0        0        0     1645 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/HwProperties.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.017230 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Move/
--rw-rw-rw-   0        0        0     1377 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Move/To.py
--rw-rw-rw-   0        0        0      984 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Move/__init__.py
--rw-rw-rw-   0        0        0     1876 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Moving.py
--rw-rw-rw-   0        0        0     1669 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Versions.py
--rw-rw-rw-   0        0        0     2687 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.024212 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Recall/
--rw-rw-rw-   0        0        0     1723 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Recall/Partial.py
--rw-rw-rw-   0        0        0     1032 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Recall/__init__.py
--rw-rw-rw-   0        0        0      891 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Reset.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.028202 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.031193 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.040169 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/
--rw-rw-rw-   0        0        0     1861 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/Rx.py
--rw-rw-rw-   0        0        0     1825 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/Tx.py
--rw-rw-rw-   0        0        0     1205 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/__init__.py
--rw-rw-rw-   0        0        0     1817 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/__init__.py
--rw-rw-rw-   0        0        0      990 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.043161 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.046153 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.055131 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/
--rw-rw-rw-   0        0        0     1729 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/Rx.py
--rw-rw-rw-   0        0        0     1729 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/Tx.py
--rw-rw-rw-   0        0        0     1200 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/__init__.py
--rw-rw-rw-   0        0        0     1006 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/__init__.py
--rw-rw-rw-   0        0        0      992 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.062111 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Save/
--rw-rw-rw-   0        0        0     1173 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Save/Partial.py
--rw-rw-rw-   0        0        0     1022 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Save/__init__.py
--rw-rw-rw-   0        0        0     1856 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Vse.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.069092 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Z310/
--rw-rw-rw-   0        0        0     1323 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Z310/Attenuation.py
--rw-rw-rw-   0        0        0     1054 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Z310/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.075077 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Z320/
--rw-rw-rw-   0        0        0     1323 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Z320/Attenuation.py
--rw-rw-rw-   0        0        0     1054 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Z320/__init__.py
--rw-rw-rw-   0        0        0     3612 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.077071 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.086047 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.094026 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/
--rw-rw-rw-   0        0        0     1689 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/Rx.py
--rw-rw-rw-   0        0        0     1689 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/Tx.py
--rw-rw-rw-   0        0        0     1223 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.103002 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/
--rw-rw-rw-   0        0        0     1828 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/Rx.py
--rw-rw-rw-   0        0        0     1828 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/Tx.py
--rw-rw-rw-   0        0        0     1243 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/__init__.py
--rw-rw-rw-   0        0        0     1914 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Direction.py
--rw-rw-rw-   0        0        0     2359 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Info.py
--rw-rw-rw-   0        0        0     1847 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/__init__.py
--rw-rw-rw-   0        0        0     1044 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/__init__.py
--rw-rw-rw-   0        0        0     1542 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.105993 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.108985 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.111977 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/Attenuation/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.120953 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/
--rw-rw-rw-   0        0        0     1327 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/Globale.py
--rw-rw-rw-   0        0        0     1381 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/Tenvironment.py
--rw-rw-rw-   0        0        0     1363 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/__init__.py
--rw-rw-rw-   0        0        0     1121 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/Attenuation/__init__.py
--rw-rw-rw-   0        0        0     1062 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.126937 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/Tenvironment/
--rw-rw-rw-   0        0        0     1405 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/Tenvironment/Spath.py
--rw-rw-rw-   0        0        0     1044 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/Tenvironment/__init__.py
--rw-rw-rw-   0        0        0     1304 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.129930 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.131924 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.138905 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/
--rw-rw-rw-   0        0        0     1263 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/Connectors.py
--rw-rw-rw-   0        0        0     1056 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/__init__.py
--rw-rw-rw-   0        0        0     1027 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.140899 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.145886 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/Gprf/
--rw-rw-rw-   0        0        0     1225 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/Gprf/Measurement.py
--rw-rw-rw-   0        0        0     1054 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/Gprf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.147882 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.151872 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.153865 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.156857 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.161844 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/
--rw-rw-rw-   0        0        0     2337 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/FilterPy.py
--rw-rw-rw-   0        0        0     2757 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.167828 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Rpc/
--rw-rw-rw-   0        0        0     2325 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Rpc/FilterPy.py
--rw-rw-rw-   0        0        0     2740 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Rpc/__init__.py
--rw-rw-rw-   0        0        0     1216 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.171818 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.177802 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Psub/
--rw-rw-rw-   0        0        0     2337 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Psub/FilterPy.py
--rw-rw-rw-   0        0        0     2757 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Psub/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.198747 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Rpc/
--rw-rw-rw-   0        0        0     2325 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Rpc/FilterPy.py
--rw-rw-rw-   0        0        0     2740 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Rpc/__init__.py
--rw-rw-rw-   0        0        0     1216 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/__init__.py
--rw-rw-rw-   0        0        0     1238 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/__init__.py
--rw-rw-rw-   0        0        0     1025 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.213705 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Scpi/
--rw-rw-rw-   0        0        0     1981 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Scpi/Logging.py
--rw-rw-rw-   0        0        0     1024 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Scpi/__init__.py
--rw-rw-rw-   0        0        0     1229 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/__init__.py
--rw-rw-rw-   0        0        0     1258 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.217695 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.224676 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/Power/
--rw-rw-rw-   0        0        0     2255 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/Power/State.py
--rw-rw-rw-   0        0        0     1011 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/Power/__init__.py
--rw-rw-rw-   0        0        0     1009 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.228665 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Generic/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.236645 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Generic/Measurement/
--rw-rw-rw-   0        0        0     1191 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Generic/Measurement/Dapi.py
--rw-rw-rw-   0        0        0     1033 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Generic/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1067 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Generic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.239636 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.261577 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/
--rw-rw-rw-   0        0        0     1231 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Correction.py
--rw-rw-rw-   0        0        0      834 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfProperty.py
--rw-rw-rw-   0        0        0     1314 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfSettings.py
--rw-rw-rw-   0        0        0     1311 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfSetttings.py
--rw-rw-rw-   0        0        0     1211 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Rms.py
--rw-rw-rw-   0        0        0     2062 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Snumber.py
--rw-rw-rw-   0        0        0     3120 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.267562 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.273546 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Ploss/
--rw-rw-rw-   0        0        0     1320 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Ploss/Rnames.py
--rw-rw-rw-   0        0        0     2409 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Ploss/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.294489 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.300473 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Bandpass/
--rw-rw-rw-   0        0        0     2381 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Bandpass/Bandwidth.py
--rw-rw-rw-   0        0        0     1062 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Bandpass/__init__.py
--rw-rw-rw-   0        0        0      865 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Franges.py
--rw-rw-rw-   0        0        0     2332 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Frequency.py
--rw-rw-rw-   0        0        0     2276 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Fspan.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.307454 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Gauss/
--rw-rw-rw-   0        0        0     2363 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Gauss/Bandwidth.py
--rw-rw-rw-   0        0        0     1047 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Gauss/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.313438 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.319423 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Bandpass/
--rw-rw-rw-   0        0        0     2454 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Bandpass/Bandwidth.py
--rw-rw-rw-   0        0        0     1064 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Bandpass/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.325406 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Gauss/
--rw-rw-rw-   0        0        0     2436 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Gauss/Bandwidth.py
--rw-rw-rw-   0        0        0     1049 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Gauss/__init__.py
--rw-rw-rw-   0        0        0     2377 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Samples.py
--rw-rw-rw-   0        0        0     1536 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.331390 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/ListPy/
--rw-rw-rw-   0        0        0     2345 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/ListPy/Iranges.py
--rw-rw-rw-   0        0        0     1036 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/ListPy/__init__.py
--rw-rw-rw-   0        0        0     1357 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/LoFrequency.py
--rw-rw-rw-   0        0        0     2304 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/NbLevel.py
--rw-rw-rw-   0        0        0     2326 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/SymbolRate.py
--rw-rw-rw-   0        0        0     4175 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/__init__.py
--rw-rw-rw-   0        0        0     2046 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Snumber.py
--rw-rw-rw-   0        0        0     3535 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1313 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.337375 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Meas/
--rw-rw-rw-   0        0        0     1125 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Meas/Scpi.py
--rw-rw-rw-   0        0        0      996 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Meas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.339369 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.348345 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/
--rw-rw-rw-   0        0        0     1301 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/Generator.py
--rw-rw-rw-   0        0        0     1319 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/Measurement.py
--rw-rw-rw-   0        0        0     1314 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.354330 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/NrMmw/
--rw-rw-rw-   0        0        0     1325 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/NrMmw/Measurement.py
--rw-rw-rw-   0        0        0     1059 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/NrMmw/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.360313 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Uwb/
--rw-rw-rw-   0        0        0     1313 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Uwb/Measurement.py
--rw-rw-rw-   0        0        0     1049 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Uwb/__init__.py
--rw-rw-rw-   0        0        0     1441 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.363306 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.366298 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.372282 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/Debug/
--rw-rw-rw-   0        0        0     2310 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/Debug/Output.py
--rw-rw-rw-   0        0        0     1021 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/Debug/__init__.py
--rw-rw-rw-   0        0        0     1001 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/__init__.py
--rw-rw-rw-   0        0        0     1003 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/__init__.py
--rw-rw-rw-   0        0        0     2693 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.375273 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.378265 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.381258 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.387242 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/State/
--rw-rw-rw-   0        0        0     2115 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/State/All.py
--rw-rw-rw-   0        0        0     2756 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/State/__init__.py
--rw-rw-rw-   0        0        0     3733 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.390234 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.396217 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/State/
--rw-rw-rw-   0        0        0     2116 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/State/All.py
--rw-rw-rw-   0        0        0     2757 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/State/__init__.py
--rw-rw-rw-   0        0        0     6124 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.410180 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/
--rw-rw-rw-   0        0        0     1845 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Icomponent.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.419158 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/
--rw-rw-rw-   0        0        0     2613 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/Average.py
--rw-rw-rw-   0        0        0     2613 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/Current.py
--rw-rw-rw-   0        0        0     1273 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.436111 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/
--rw-rw-rw-   0        0        0     2034 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Average.py
--rw-rw-rw-   0        0        0     2034 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Current.py
--rw-rw-rw-   0        0        0     2034 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Maximum.py
--rw-rw-rw-   0        0        0     2034 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Minimum.py
--rw-rw-rw-   0        0        0     1761 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/__init__.py
--rw-rw-rw-   0        0        0     1845 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Qcomponent.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.442095 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/State/
--rw-rw-rw-   0        0        0     2121 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/State/All.py
--rw-rw-rw-   0        0        0     2762 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/State/__init__.py
--rw-rw-rw-   0        0        0     4744 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.459050 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/
--rw-rw-rw-   0        0        0     1553 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Bin.py
--rw-rw-rw-   0        0        0      944 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Reliability.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.465034 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/State/
--rw-rw-rw-   0        0        0     2118 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/State/All.py
--rw-rw-rw-   0        0        0     2759 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/State/__init__.py
--rw-rw-rw-   0        0        0      920 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/SymbolRate.py
--rw-rw-rw-   0        0        0     1656 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Talignment.py
--rw-rw-rw-   0        0        0     7279 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.486976 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/
--rw-rw-rw-   0        0        0     1792 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/FreqError.py
--rw-rw-rw-   0        0        0     1731 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Icomponent.py
--rw-rw-rw-   0        0        0     1708 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Level.py
--rw-rw-rw-   0        0        0     3029 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/OfError.py
--rw-rw-rw-   0        0        0     1708 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Phase.py
--rw-rw-rw-   0        0        0     1731 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Qcomponent.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.492959 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/State/
--rw-rw-rw-   0        0        0     2110 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/State/All.py
--rw-rw-rw-   0        0        0     2751 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/State/__init__.py
--rw-rw-rw-   0        0        0     5210 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.495952 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.502933 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/Sensor/
--rw-rw-rw-   0        0        0     4990 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/Sensor/Power.py
--rw-rw-rw-   0        0        0     1855 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/Sensor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.508917 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/State/
--rw-rw-rw-   0        0        0     2100 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/State/All.py
--rw-rw-rw-   0        0        0     2741 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/State/__init__.py
--rw-rw-rw-   0        0        0     3899 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.513903 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/
--rw-rw-rw-   0        0        0     1254 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Clear.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.528864 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/
--rw-rw-rw-   0        0        0     1062 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Eoo.py
--rw-rw-rw-   0        0        0     1062 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Ezo.py
--rw-rw-rw-   0        0        0     1062 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Ezz.py
--rw-rw-rw-   0        0        0     1097 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Frequency.py
--rw-rw-rw-   0        0        0     1686 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.541828 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/
--rw-rw-rw-   0        0        0     1708 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Frequency.py
--rw-rw-rw-   0        0        0     1452 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Gain.py
--rw-rw-rw-   0        0        0     1652 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/State.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.550805 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Trace/
--rw-rw-rw-   0        0        0     1733 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Trace/Frequency.py
--rw-rw-rw-   0        0        0     1477 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Trace/Gain.py
--rw-rw-rw-   0        0        0     1267 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Trace/__init__.py
--rw-rw-rw-   0        0        0     2778 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.556789 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Match/
--rw-rw-rw-   0        0        0     1348 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Match/State.py
--rw-rw-rw-   0        0        0     1861 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Match/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.563770 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Open/
--rw-rw-rw-   0        0        0     1634 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Open/State.py
--rw-rw-rw-   0        0        0     2026 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Open/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.568757 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Short/
--rw-rw-rw-   0        0        0     1638 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Short/State.py
--rw-rw-rw-   0        0        0     2037 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Short/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.574741 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/
--rw-rw-rw-   0        0        0     2103 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/All.py
--rw-rw-rw-   0        0        0     2744 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/__init__.py
--rw-rw-rw-   0        0        0     3588 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.587707 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/
--rw-rw-rw-   0        0        0     1152 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/AmplitudeProbDensity.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.594689 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Average/
--rw-rw-rw-   0        0        0     1620 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Average/Rms.py
--rw-rw-rw-   0        0        0     4648 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Average/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.609648 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/
--rw-rw-rw-   0        0        0     1741 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Power.py
--rw-rw-rw-   0        0        0     1340 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Probability.py
--rw-rw-rw-   0        0        0     1485 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Sample.py
--rw-rw-rw-   0        0        0     2322 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.625605 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/
--rw-rw-rw-   0        0        0     1656 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Maximum.py
--rw-rw-rw-   0        0        0     1656 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Minimum.py
--rw-rw-rw-   0        0        0     1620 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Rms.py
--rw-rw-rw-   0        0        0     5136 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/__init__.py
--rw-rw-rw-   0        0        0     1170 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ElapsedStats.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.631589 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqData/
--rw-rw-rw-   0        0        0     1518 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqData/Bin.py
--rw-rw-rw-   0        0        0     3002 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqData/__init__.py
--rw-rw-rw-   0        0        0     1998 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqInfo.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.646549 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/
--rw-rw-rw-   0        0        0     4420 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Average.py
--rw-rw-rw-   0        0        0     4420 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Current.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.652535 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Maximum/
--rw-rw-rw-   0        0        0     4498 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Maximum/Current.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Maximum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.659514 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Minimum/
--rw-rw-rw-   0        0        0     4498 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Minimum/Current.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Minimum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.669489 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/
--rw-rw-rw-   0        0        0     4471 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/Maximum.py
--rw-rw-rw-   0        0        0     4471 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/Minimum.py
--rw-rw-rw-   0        0        0     1270 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/__init__.py
--rw-rw-rw-   0        0        0     4462 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/StandardDev.py
--rw-rw-rw-   0        0        0     2263 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.679461 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/
--rw-rw-rw-   0        0        0     4111 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/Current.py
--rw-rw-rw-   0        0        0     1656 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/Maximum.py
--rw-rw-rw-   0        0        0     1283 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.689434 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/
--rw-rw-rw-   0        0        0     4111 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/Current.py
--rw-rw-rw-   0        0        0     1656 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/Minimum.py
--rw-rw-rw-   0        0        0     1283 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.698410 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/
--rw-rw-rw-   0        0        0     4084 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/Maximum.py
--rw-rw-rw-   0        0        0     4084 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/Minimum.py
--rw-rw-rw-   0        0        0     1268 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.704394 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/StandardDev/
--rw-rw-rw-   0        0        0     1676 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/StandardDev/Current.py
--rw-rw-rw-   0        0        0     4730 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/StandardDev/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.710379 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/State/
--rw-rw-rw-   0        0        0     2103 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/State/All.py
--rw-rw-rw-   0        0        0     2744 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/State/__init__.py
--rw-rw-rw-   0        0        0     6839 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.713370 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.733317 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/
--rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Average.py
--rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Current.py
--rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Maximum.py
--rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Minimum.py
--rw-rw-rw-   0        0        0     1771 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.740299 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Marker/
--rw-rw-rw-   0        0        0     2350 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Marker/Npeak.py
--rw-rw-rw-   0        0        0     1855 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Marker/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.756256 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/
--rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Average.py
--rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Current.py
--rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Maximum.py
--rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Minimum.py
--rw-rw-rw-   0        0        0     1771 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.775206 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/
--rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Average.py
--rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Current.py
--rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Maximum.py
--rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Minimum.py
--rw-rw-rw-   0        0        0     1771 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.791162 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/
--rw-rw-rw-   0        0        0     2059 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/Npeak.py
--rw-rw-rw-   0        0        0     2059 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/Speak.py
--rw-rw-rw-   0        0        0     1291 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.809115 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/
--rw-rw-rw-   0        0        0     1626 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Average.py
--rw-rw-rw-   0        0        0     1626 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Current.py
--rw-rw-rw-   0        0        0     1626 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Maximum.py
--rw-rw-rw-   0        0        0     1626 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Minimum.py
--rw-rw-rw-   0        0        0     1751 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.828064 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/
--rw-rw-rw-   0        0        0     1644 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Average.py
--rw-rw-rw-   0        0        0     1644 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Current.py
--rw-rw-rw-   0        0        0     1644 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Maximum.py
--rw-rw-rw-   0        0        0     1644 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Minimum.py
--rw-rw-rw-   0        0        0     1766 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.834047 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/State/
--rw-rw-rw-   0        0        0     1804 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/State/All.py
--rw-rw-rw-   0        0        0     2368 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/State/__init__.py
--rw-rw-rw-   0        0        0     3902 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/__init__.py
--rw-rw-rw-   0        0        0     3066 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.837041 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.840032 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.844021 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.853995 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/
--rw-rw-rw-   0        0        0     1329 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/Globale.py
--rw-rw-rw-   0        0        0     1363 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/Tenvironment.py
--rw-rw-rw-   0        0        0     1363 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/__init__.py
--rw-rw-rw-   0        0        0     1121 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/__init__.py
--rw-rw-rw-   0        0        0     1062 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/__init__.py
--rw-rw-rw-   0        0        0     1020 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.856986 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.859979 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.863969 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.873942 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/
--rw-rw-rw-   0        0        0     1293 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/Globale.py
--rw-rw-rw-   0        0        0     1327 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/Tenvironment.py
--rw-rw-rw-   0        0        0     1363 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/__init__.py
--rw-rw-rw-   0        0        0     1121 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/__init__.py
--rw-rw-rw-   0        0        0     1062 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.876933 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.879926 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.889899 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/
--rw-rw-rw-   0        0        0     1237 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/Rx.py
--rw-rw-rw-   0        0        0     1237 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/Tx.py
--rw-rw-rw-   0        0        0     1243 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/__init__.py
--rw-rw-rw-   0        0        0     1091 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/__init__.py
--rw-rw-rw-   0        0        0     1044 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/__init__.py
--rw-rw-rw-   0        0        0     1304 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.893888 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.896880 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.899873 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.906853 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/Power/
--rw-rw-rw-   0        0        0     1633 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/Power/Current.py
--rw-rw-rw-   0        0        0     1029 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/Power/__init__.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/__init__.py
--rw-rw-rw-   0        0        0     1009 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.909846 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.912837 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Bluetooth/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.917823 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Bluetooth/Measurement/
--rw-rw-rw-   0        0        0     1670 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Bluetooth/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Bluetooth/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1077 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Bluetooth/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.924805 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Cdma/
--rw-rw-rw-   0        0        0     1250 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Cdma/Measurement.py
--rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Cdma/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.927797 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.933781 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/
--rw-rw-rw-   0        0        0     1449 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/RfSettings.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.941760 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/Spath/
--rw-rw-rw-   0        0        0     2377 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/Spath/Group.py
--rw-rw-rw-   0        0        0     2525 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/Spath/__init__.py
--rw-rw-rw-   0        0        0     1299 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.950736 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/
--rw-rw-rw-   0        0        0     1441 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/RfSettings.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.956719 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Scenario/
--rw-rw-rw-   0        0        0      888 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Scenario/Catalog.py
--rw-rw-rw-   0        0        0     1044 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Scenario/__init__.py
--rw-rw-rw-   0        0        0     3754 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1561 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1312 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.959712 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gsm/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.965696 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gsm/Measurement/
--rw-rw-rw-   0        0        0     1616 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gsm/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gsm/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1047 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gsm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.968688 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Lte/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.985643 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Lte/Measurement/
--rw-rw-rw-   0        0        0     1616 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Lte/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Lte/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1047 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Lte/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.972678 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/LteDl/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.978661 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/LteDl/Measurement/
--rw-rw-rw-   0        0        0     1634 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/LteDl/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/LteDl/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/LteDl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.991627 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Niot/
--rw-rw-rw-   0        0        0     1250 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Niot/Measurement.py
--rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Niot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.995616 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrDl/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.001600 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrDl/Measurement/
--rw-rw-rw-   0        0        0     1625 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrDl/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrDl/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrDl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.004593 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrMmw/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.010576 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrMmw/Measurement/
--rw-rw-rw-   0        0        0     1634 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrMmw/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrMmw/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrMmw/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.013568 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrSub/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.022545 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrSub/Measurement/
--rw-rw-rw-   0        0        0     1634 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrSub/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrSub/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrSub/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.025536 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Uwb/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.034513 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Uwb/Measurement/
--rw-rw-rw-   0        0        0     1616 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Uwb/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Uwb/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1047 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Uwb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.038503 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wcdma/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.043488 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wcdma/Measurement/
--rw-rw-rw-   0        0        0     1634 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wcdma/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wcdma/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wcdma/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.046480 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wlan/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.053463 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wlan/Measurement/
--rw-rw-rw-   0        0        0     1625 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wlan/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wlan/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wlan/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.055456 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wpan/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.061440 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/
--rw-rw-rw-   0        0        0     1625 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wpan/__init__.py
--rw-rw-rw-   0        0        0     3909 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.064432 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.067428 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.070417 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.076400 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/
--rw-rw-rw-   0        0        0     1813 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/Ambient.py
--rw-rw-rw-   0        0        0     1049 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/__init__.py
--rw-rw-rw-   0        0        0     1073 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.079393 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/System/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.088368 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/System/Positioner/
--rw-rw-rw-   0        0        0     1124 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/System/Positioner/IsMoving.py
--rw-rw-rw-   0        0        0     1619 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/System/Positioner/Position.py
--rw-rw-rw-   0        0        0     2199 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/System/Positioner/__init__.py
--rw-rw-rw-   0        0        0     1054 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/System/__init__.py
--rw-rw-rw-   0        0        0     1235 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.091360 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.095349 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.107318 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.121281 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/
--rw-rw-rw-   0        0        0     4136 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/File.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.127264 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Marker/
--rw-rw-rw-   0        0        0     2565 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Marker/Delays.py
--rw-rw-rw-   0        0        0     1028 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Marker/__init__.py
--rw-rw-rw-   0        0        0     3268 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Msegment.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.133248 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Samples/
--rw-rw-rw-   0        0        0     2372 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Samples/Range.py
--rw-rw-rw-   0        0        0     1536 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Samples/__init__.py
--rw-rw-rw-   0        0        0     2323 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Segments.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.139232 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/UdMarker/
--rw-rw-rw-   0        0        0     1253 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/UdMarker/Clist.py
--rw-rw-rw-   0        0        0     3222 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/UdMarker/__init__.py
--rw-rw-rw-   0        0        0     9112 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.148209 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/
--rw-rw-rw-   0        0        0     2628 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/Level.py
--rw-rw-rw-   0        0        0     3652 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/Ofrequency.py
--rw-rw-rw-   0        0        0     2150 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/__init__.py
--rw-rw-rw-   0        0        0     3390 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/IqSettings.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.189099 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/
--rw-rw-rw-   0        0        0     2475 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Dgain.py
--rw-rw-rw-   0        0        0     2448 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Dtime.py
--rw-rw-rw-   0        0        0     1225 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Esingle.py
--rw-rw-rw-   0        0        0     3782 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Fill.py
--rw-rw-rw-   0        0        0     2507 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Frequency.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.195083 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Increment/
--rw-rw-rw-   0        0        0     1811 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Increment/Enabling.py
--rw-rw-rw-   0        0        0     2412 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Increment/__init__.py
--rw-rw-rw-   0        0        0     2531 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Irepetition.py
--rw-rw-rw-   0        0        0     2539 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Modulation.py
--rw-rw-rw-   0        0        0     2529 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Reenabling.py
--rw-rw-rw-   0        0        0     2607 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/RfLevel.py
--rw-rw-rw-   0        0        0     1207 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Rlist.py
--rw-rw-rw-   0        0        0     1207 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Slist.py
--rw-rw-rw-   0        0        0     2189 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Sstop.py
--rw-rw-rw-   0        0        0    10413 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/__init__.py
--rw-rw-rw-   0        0        0     2717 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Reliability.py
--rw-rw-rw-   0        0        0     5682 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/RfSettings.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.207051 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.254924 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/
--rw-rw-rw-   0        0        0     1635 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Check.py
--rw-rw-rw-   0        0        0     1762 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/CrcProtect.py
--rw-rw-rw-   0        0        0     1364 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Download.py
--rw-rw-rw-   0        0        0     1515 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Duration.py
--rw-rw-rw-   0        0        0     1544 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Paratio.py
--rw-rw-rw-   0        0        0     1627 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Path.py
--rw-rw-rw-   0        0        0     1518 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Poffset.py
--rw-rw-rw-   0        0        0     1694 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Reliability.py
--rw-rw-rw-   0        0        0     1733 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Rmessage.py
--rw-rw-rw-   0        0        0     1589 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Roption.py
--rw-rw-rw-   0        0        0     1510 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Samples.py
--rw-rw-rw-   0        0        0     1525 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/SymbolRate.py
--rw-rw-rw-   0        0        0     1591 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Waveform.py
--rw-rw-rw-   0        0        0     8460 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.260907 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Dtone/
--rw-rw-rw-   0        0        0     3565 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Dtone/Ofrequency.py
--rw-rw-rw-   0        0        0     1985 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Dtone/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.289830 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/
--rw-rw-rw-   0        0        0     2846 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Acycles.py
--rw-rw-rw-   0        0        0     2850 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Dgain.py
--rw-rw-rw-   0        0        0     2810 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Dtime.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.306785 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/
--rw-rw-rw-   0        0        0     1418 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Call.py
--rw-rw-rw-   0        0        0     1136 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Insert.py
--rw-rw-rw-   0        0        0     1126 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Mdown.py
--rw-rw-rw-   0        0        0     1110 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Mup.py
--rw-rw-rw-   0        0        0     2484 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.320748 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/
--rw-rw-rw-   0        0        0     1519 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Apply.py
--rw-rw-rw-   0        0        0     3570 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Dgain.py
--rw-rw-rw-   0        0        0     3758 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Frequency.py
--rw-rw-rw-   0        0        0     3507 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Lrms.py
--rw-rw-rw-   0        0        0     3555 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/__init__.py
--rw-rw-rw-   0        0        0     3163 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Frequency.py
--rw-rw-rw-   0        0        0     3702 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Itransition.py
--rw-rw-rw-   0        0        0     5060 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Lincrement.py
--rw-rw-rw-   0        0        0     2772 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Lrms.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.330721 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.341691 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/
--rw-rw-rw-   0        0        0     1312 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Cw.py
--rw-rw-rw-   0        0        0     1339 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Dtone.py
--rw-rw-rw-   0        0        0     1321 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Off.py
--rw-rw-rw-   0        0        0     5147 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/__init__.py
--rw-rw-rw-   0        0        0     2440 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Catalog.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.350668 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Index/
--rw-rw-rw-   0        0        0     2186 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Index/All.py
--rw-rw-rw-   0        0        0     2969 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Index/__init__.py
--rw-rw-rw-   0        0        0     2097 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Range.py
--rw-rw-rw-   0        0        0     3415 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.359644 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.364631 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.368619 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.376599 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/Tx/
--rw-rw-rw-   0        0        0     3080 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/Tx/Single.py
--rw-rw-rw-   0        0        0     1016 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/Tx/__init__.py
--rw-rw-rw-   0        0        0     4245 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/__init__.py
--rw-rw-rw-   0        0        0     3224 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/__init__.py
--rw-rw-rw-   0        0        0     1017 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/__init__.py
--rw-rw-rw-   0        0        0     1538 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/SymbolRate.py
--rw-rw-rw-   0        0        0     1519 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Ttime.py
--rw-rw-rw-   0        0        0     5939 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.379590 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.385574 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/Delays/
--rw-rw-rw-   0        0        0     2880 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/Delays/All.py
--rw-rw-rw-   0        0        0     3365 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/Delays/__init__.py
--rw-rw-rw-   0        0        0     1028 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/__init__.py
--rw-rw-rw-   0        0        0     2786 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Reliability.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.391559 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/RfSettings/
--rw-rw-rw-   0        0        0     2299 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/RfSettings/Spath.py
--rw-rw-rw-   0        0        0     1040 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/RfSettings/__init__.py
--rw-rw-rw-   0        0        0     1298 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Rmarker.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.397542 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/State/
--rw-rw-rw-   0        0        0     2146 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/State/All.py
--rw-rw-rw-   0        0        0     2133 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/State/__init__.py
--rw-rw-rw-   0        0        0     1343 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Tdd.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.400535 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.407515 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/Delay/
--rw-rw-rw-   0        0        0     2592 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/Delay/All.py
--rw-rw-rw-   0        0        0     2470 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/Delay/__init__.py
--rw-rw-rw-   0        0        0     1864 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/__init__.py
--rw-rw-rw-   0        0        0     7520 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.427462 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/State/
--rw-rw-rw-   0        0        0     2088 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/State/All.py
--rw-rw-rw-   0        0        0     1983 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/State/__init__.py
--rw-rw-rw-   0        0        0     3944 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/__init__.py
--rw-rw-rw-   0        0        0     1038 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/__init__.py
--rw-rw-rw-   0        0        0     1006 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.431452 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.434443 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.447409 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.460374 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/
--rw-rw-rw-   0        0        0     1256 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/Globale.py
--rw-rw-rw-   0        0        0     1309 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/Tenvironment.py
--rw-rw-rw-   0        0        0     1303 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/__init__.py
--rw-rw-rw-   0        0        0      805 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/Globale.py
--rw-rw-rw-   0        0        0      839 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/Tenvironment.py
--rw-rw-rw-   0        0        0     1573 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/__init__.py
--rw-rw-rw-   0        0        0     1119 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.468354 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Date/
--rw-rw-rw-   0        0        0     1988 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Date/Local.py
--rw-rw-rw-   0        0        0     1004 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Date/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.476332 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Time/
--rw-rw-rw-   0        0        0     2020 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Time/Local.py
--rw-rw-rw-   0        0        0     2496 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Time/__init__.py
--rw-rw-rw-   0        0        0     1500 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.483313 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Tenvironment/
--rw-rw-rw-   0        0        0      789 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Tenvironment/Spath.py
--rw-rw-rw-   0        0        0     1042 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Tenvironment/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.488300 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.491291 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.495281 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.502262 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/BhRate/
--rw-rw-rw-   0        0        0      899 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/BhRate/Catalog.py
--rw-rw-rw-   0        0        0     1932 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/BhRate/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.508246 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdr/
--rw-rw-rw-   0        0        0      890 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdr/Catalog.py
--rw-rw-rw-   0        0        0     1899 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.516232 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdrp/
--rw-rw-rw-   0        0        0      893 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdrp/Catalog.py
--rw-rw-rw-   0        0        0     1910 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdrp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.522209 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      912 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1973 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/MultiEval/__init__.py
--rw-rw-rw-   0        0        0     1741 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1077 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.526199 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.529191 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.535174 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      897 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1943 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/__init__.py
--rw-rw-rw-   0        0        0     1073 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.538167 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.541159 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.548140 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/
--rw-rw-rw-   0        0        0     1020 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Catalog.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.555122 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/
--rw-rw-rw-   0        0        0     1265 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/Execute.py
--rw-rw-rw-   0        0        0     1036 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.558115 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.566092 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/
--rw-rw-rw-   0        0        0     1321 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/Execute.py
--rw-rw-rw-   0        0        0     1038 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/__init__.py
--rw-rw-rw-   0        0        0     2034 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/__init__.py
--rw-rw-rw-   0        0        0     5898 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.577063 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/
--rw-rw-rw-   0        0        0     2189 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/IsMeas.py
--rw-rw-rw-   0        0        0     2238 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/IsTrigger.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.583047 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/
--rw-rw-rw-   0        0        0     1383 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/Execute.py
--rw-rw-rw-   0        0        0     1036 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/__init__.py
--rw-rw-rw-   0        0        0     2576 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/__init__.py
--rw-rw-rw-   0        0        0     2270 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.590028 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.599004 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/
--rw-rw-rw-   0        0        0     1056 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/Catalog.py
--rw-rw-rw-   0        0        0     2344 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/OsStop.py
--rw-rw-rw-   0        0        0     9301 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.604988 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqRecorder/
--rw-rw-rw-   0        0        0     1054 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqRecorder/Catalog.py
--rw-rw-rw-   0        0        0    10924 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqRecorder/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.610972 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqVsSlot/
--rw-rw-rw-   0        0        0     1044 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqVsSlot/Catalog.py
--rw-rw-rw-   0        0        0     9138 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqVsSlot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.616956 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/
--rw-rw-rw-   0        0        0     1034 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/Catalog.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.623937 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/
--rw-rw-rw-   0        0        0     2941 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/Offset.py
--rw-rw-rw-   0        0        0     1078 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/__init__.py
--rw-rw-rw-   0        0        0     9407 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/__init__.py
--rw-rw-rw-   0        0        0     4768 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Spectrum.py
--rw-rw-rw-   0        0        0     2074 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1313 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.626929 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.629921 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.636903 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      894 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1937 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/__init__.py
--rw-rw-rw-   0        0        0     1073 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1047 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.639894 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.654855 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.660838 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      894 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1937 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/MultiEval/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.666822 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Prach/
--rw-rw-rw-   0        0        0      878 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Prach/Catalog.py
--rw-rw-rw-   0        0        0     1885 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Prach/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.673804 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Srs/
--rw-rw-rw-   0        0        0      872 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Srs/Catalog.py
--rw-rw-rw-   0        0        0     1863 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Srs/__init__.py
--rw-rw-rw-   0        0        0     1513 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1047 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.642886 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.645879 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.651862 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      900 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1949 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/MultiEval/__init__.py
--rw-rw-rw-   0        0        0     1073 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.678791 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.683777 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.689761 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      897 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1943 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/MultiEval/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.695745 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/Prach/
--rw-rw-rw-   0        0        0      881 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/Prach/Catalog.py
--rw-rw-rw-   0        0        0     1891 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/Prach/__init__.py
--rw-rw-rw-   0        0        0     1301 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.700733 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.703725 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.709708 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      897 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1943 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/MultiEval/__init__.py
--rw-rw-rw-   0        0        0     1073 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.712700 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.716690 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.722673 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      900 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1949 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/MultiEval/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.728657 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/Prach/
--rw-rw-rw-   0        0        0      884 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/Prach/Catalog.py
--rw-rw-rw-   0        0        0     1897 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/Prach/__init__.py
--rw-rw-rw-   0        0        0     1301 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.731650 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.734641 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.740625 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      900 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1949 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/MultiEval/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.747607 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Prach/
--rw-rw-rw-   0        0        0      884 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Prach/Catalog.py
--rw-rw-rw-   0        0        0     1897 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Prach/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.754589 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Srs/
--rw-rw-rw-   0        0        0      878 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Srs/Catalog.py
--rw-rw-rw-   0        0        0     1875 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Srs/__init__.py
--rw-rw-rw-   0        0        0     1513 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.757581 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.760573 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.767554 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      894 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1937 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/MultiEval/__init__.py
--rw-rw-rw-   0        0        0     1073 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1047 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.770546 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.773537 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.780521 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      900 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1949 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/MultiEval/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.786503 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OlpControl/
--rw-rw-rw-   0        0        0      899 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OlpControl/Catalog.py
--rw-rw-rw-   0        0        0     1952 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OlpControl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.792488 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OoSync/
--rw-rw-rw-   0        0        0      887 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OoSync/Catalog.py
--rw-rw-rw-   0        0        0     1908 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OoSync/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.799468 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Prach/
--rw-rw-rw-   0        0        0      884 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Prach/Catalog.py
--rw-rw-rw-   0        0        0     1897 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Prach/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.805452 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Tpc/
--rw-rw-rw-   0        0        0      878 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Tpc/Catalog.py
--rw-rw-rw-   0        0        0     1875 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Tpc/__init__.py
--rw-rw-rw-   0        0        0     2018 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1058 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.809442 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.812434 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.819415 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      897 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1943 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/MultiEval/__init__.py
--rw-rw-rw-   0        0        0     1073 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.822407 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.826396 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.832380 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      897 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1943 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/MultiEval/__init__.py
--rw-rw-rw-   0        0        0     1073 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/__init__.py
--rw-rw-rw-   0        0        0     3920 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/__init__.py
--rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.934108 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/
--rw-rw-rw-   0        0        0      586 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgLinkedEventArgs.py
--rw-rw-rw-   0        0        0     4165 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgSingle.py
--rw-rw-rw-   0        0        0     1116 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgSingleList.py
--rw-rw-rw-   0        0        0     1145 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgSingleSuppressed.py
--rw-rw-rw-   0        0        0     9097 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgStringComposer.py
--rw-rw-rw-   0        0        0     5751 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgStruct.py
--rw-rw-rw-   0        0        0     3439 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgStructList.py
--rw-rw-rw-   0        0        0     2546 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgStructStringParser.py
--rw-rw-rw-   0        0        0     5238 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/CommandsGroup.py
--rw-rw-rw-   0        0        0    25419 2024-04-03 11:15:31.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/Conversions.py
--rw-rw-rw-   0        0        0     3775 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ConverterFromScpiString.py
--rw-rw-rw-   0        0        0     4768 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ConverterToScpiString.py
--rw-rw-rw-   0        0        0    14213 2024-04-03 11:15:31.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/Core.py
--rw-rw-rw-   0        0        0     1386 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/GlobalData.py
--rw-rw-rw-   0        0        0    60862 2024-04-03 11:15:31.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/Instrument.py
--rw-rw-rw-   0        0        0     4785 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/InstrumentErrors.py
--rw-rw-rw-   0        0        0     2225 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/InstrumentOptions.py
--rw-rw-rw-   0        0        0    16156 2024-04-03 11:15:31.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/InstrumentSettings.py
--rw-rw-rw-   0        0        0     3518 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/InternalLinker.py
--rw-rw-rw-   0        0        0     4390 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/IoTransferEventArgs.py
--rw-rw-rw-   0        0        0      387 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/Properties.py
--rw-rw-rw-   0        0        0     4289 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/RepeatedCapability.py
--rw-rw-rw-   0        0        0     4745 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ScpiEnums.py
--rw-rw-rw-   0        0        0    35525 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ScpiLogger.py
--rw-rw-rw-   0        0        0     5098 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/StreamReader.py
--rw-rw-rw-   0        0        0     5856 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/StreamWriter.py
--rw-rw-rw-   0        0        0     1114 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/StructBase.py
--rw-rw-rw-   0        0        0     3608 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/Types.py
--rw-rw-rw-   0        0        0     5498 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/Utilities.py
--rw-rw-rw-   0        0        0     5716 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/VisaPluginSocketIo.py
--rw-rw-rw-   0        0        0    51976 2024-04-03 11:15:31.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/VisaSession.py
--rw-rw-rw-   0        0        0     7512 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/VisaSessionSim.py
--rw-rw-rw-   0        0        0       29 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/__init__.py
--rw-rw-rw-   0        0        0    15874 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/RsCMPX_Gprf.py
--rw-rw-rw-   0        0        0      899 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/__init__.py
--rw-rw-rw-   0        0        0    11429 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/enums.py
--rw-rw-rw-   0        0        0     3704 2024-04-24 14:07:45.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/repcap.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.411848 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf.egg-info/
--rw-rw-rw-   0        0        0     3474 2024-04-24 14:07:58.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    53104 2024-04-24 14:07:58.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 14:07:58.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-24 14:07:58.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-24 14:07:58.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 14:08:01.938099 RsCMPX_Gprf-5.0.91/setup.cfg
--rw-rw-rw-   0        0        0     1480 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.641925 RsCMPX_Gprf-5.0.92/
+-rw-rw-rw-   0        0        0     3697 2024-05-24 14:33:54.640948 RsCMPX_Gprf-5.0.92/PKG-INFO
+-rw-rw-rw-   0        0        0     2055 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.401018 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.423464 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/CustomFiles/
+-rw-rw-rw-   0        0        0       90 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/CustomFiles/__init__.py
+-rw-rw-rw-   0        0        0     3725 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/CustomFiles/events.py
+-rw-rw-rw-   0        0        0     4916 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/CustomFiles/reliability.py
+-rw-rw-rw-   0        0        0    25093 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/CustomFiles/utilities.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.426392 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.428344 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.430296 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/System/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.433225 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/System/Attenuation/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.442009 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/
+-rw-rw-rw-   0        0        0     1338 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/Globale.py
+-rw-rw-rw-   0        0        0     1372 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/Tenvironment.py
+-rw-rw-rw-   0        0        0     1363 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/__init__.py
+-rw-rw-rw-   0        0        0     1121 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/System/Attenuation/__init__.py
+-rw-rw-rw-   0        0        0     1062 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/System/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.444937 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/Tenvironment/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.447865 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.456649 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/
+-rw-rw-rw-   0        0        0     1219 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/Rx.py
+-rw-rw-rw-   0        0        0     1219 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/Tx.py
+-rw-rw-rw-   0        0        0     1243 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/__init__.py
+-rw-rw-rw-   0        0        0     1091 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/__init__.py
+-rw-rw-rw-   0        0        0     1044 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/Tenvironment/__init__.py
+-rw-rw-rw-   0        0        0     1289 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.459576 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Calibration/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.461529 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Calibration/Gprf/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.464457 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.469336 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/ExtPwrSensor/
+-rw-rw-rw-   0        0        0     2920 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/ExtPwrSensor/Zero.py
+-rw-rw-rw-   0        0        0     1040 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/ExtPwrSensor/__init__.py
+-rw-rw-rw-   0        0        0     1097 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Calibration/Gprf/__init__.py
+-rw-rw-rw-   0        0        0     1029 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Calibration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.472265 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.474217 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.479097 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/Measurement/
+-rw-rw-rw-   0        0        0     2351 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1077 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.482025 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Cdma/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.486905 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/
+-rw-rw-rw-   0        0        0     2336 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Cdma/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.489832 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gprf/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.492761 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.499593 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/
+-rw-rw-rw-   0        0        0     1896 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/Group.py
+-rw-rw-rw-   0        0        0     2676 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/__init__.py
+-rw-rw-rw-   0        0        0     1031 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.510330 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/
+-rw-rw-rw-   0        0        0      891 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/Ploss.py
+-rw-rw-rw-   0        0        0     2406 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1269 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1312 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gprf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.512281 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gsm/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.518137 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/
+-rw-rw-rw-   0        0        0     2333 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1047 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gsm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.521065 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Lte/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.531802 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Lte/Measurement/
+-rw-rw-rw-   0        0        0     2333 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Lte/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Lte/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1047 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Lte/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.523017 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/LteDl/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.527898 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/LteDl/Measurement/
+-rw-rw-rw-   0        0        0     2339 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/LteDl/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/LteDl/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/LteDl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.534729 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Niot/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.539610 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Niot/Measurement/
+-rw-rw-rw-   0        0        0     2336 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Niot/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Niot/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Niot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.541561 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrDl/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.546441 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrDl/Measurement/
+-rw-rw-rw-   0        0        0     2336 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrDl/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrDl/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrDl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.548393 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrMmw/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.554249 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrMmw/Measurement/
+-rw-rw-rw-   0        0        0     2339 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrMmw/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrMmw/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrMmw/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.557178 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrSub/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.562058 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrSub/Measurement/
+-rw-rw-rw-   0        0        0     2339 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrSub/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrSub/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrSub/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.569865 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/System/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.575721 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/System/Attenuation/
+-rw-rw-rw-   0        0        0     1238 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/System/Attenuation/CorrectionTable.py
+-rw-rw-rw-   0        0        0     1121 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/System/Attenuation/__init__.py
+-rw-rw-rw-   0        0        0      813 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/System/Reset.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.580602 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/System/Rf42/
+-rw-rw-rw-   0        0        0      926 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/System/Rf42/Box.py
+-rw-rw-rw-   0        0        0      990 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/System/Rf42/__init__.py
+-rw-rw-rw-   0        0        0     1236 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/System/Rrhead.py
+-rw-rw-rw-   0        0        0     2122 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/System/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.585482 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Tenvironment/
+-rw-rw-rw-   0        0        0     1241 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Tenvironment/Connectors.py
+-rw-rw-rw-   0        0        0     1496 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Tenvironment/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.587434 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Uwb/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.592313 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Uwb/Measurement/
+-rw-rw-rw-   0        0        0     2333 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Uwb/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Uwb/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1047 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Uwb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.595241 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wcdma/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.600121 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wcdma/Measurement/
+-rw-rw-rw-   0        0        0     2339 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wcdma/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wcdma/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wcdma/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.603050 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wlan/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.607933 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wlan/Measurement/
+-rw-rw-rw-   0        0        0     2336 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wlan/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wlan/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wlan/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.610858 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wpan/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.615738 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wpan/Measurement/
+-rw-rw-rw-   0        0        0     2336 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wpan/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wpan/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wpan/__init__.py
+-rw-rw-rw-   0        0        0     4439 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.618666 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.621593 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.623547 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.626475 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.628426 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.631354 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.637210 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/Tx/
+-rw-rw-rw-   0        0        0     2556 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/Tx/Single.py
+-rw-rw-rw-   0        0        0     1012 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/Tx/__init__.py
+-rw-rw-rw-   0        0        0     3626 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/__init__.py
+-rw-rw-rw-   0        0        0     2709 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/__init__.py
+-rw-rw-rw-   0        0        0     1958 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/__init__.py
+-rw-rw-rw-   0        0        0     2022 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.643065 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.650875 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/
+-rw-rw-rw-   0        0        0     1377 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/IqFile.py
+-rw-rw-rw-   0        0        0     3152 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/Sall.py
+-rw-rw-rw-   0        0        0     4093 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/__init__.py
+-rw-rw-rw-   0        0        0     1259 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Correction.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.661610 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/
+-rw-rw-rw-   0        0        0     2461 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Attenuation.py
+-rw-rw-rw-   0        0        0     2082 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Auto.py
+-rw-rw-rw-   0        0        0     3239 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Average.py
+-rw-rw-rw-   0        0        0     8936 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.666490 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/
+-rw-rw-rw-   0        0        0     6166 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/PeakSearch.py
+-rw-rw-rw-   0        0        0    12393 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.679177 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/
+-rw-rw-rw-   0        0        0     2570 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/Capture.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.686986 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/
+-rw-rw-rw-   0        0        0     1907 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/Bandpass.py
+-rw-rw-rw-   0        0        0     1645 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/Gauss.py
+-rw-rw-rw-   0        0        0     2459 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/__init__.py
+-rw-rw-rw-   0        0        0     1370 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/IqSettings.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.697722 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/
+-rw-rw-rw-   0        0        0     2731 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/EnvelopePower.py
+-rw-rw-rw-   0        0        0     2675 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/Frequency.py
+-rw-rw-rw-   0        0        0     2143 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/Sstop.py
+-rw-rw-rw-   0        0        0     5475 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/__init__.py
+-rw-rw-rw-   0        0        0     1479 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/Trigger.py
+-rw-rw-rw-   0        0        0    15177 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.704555 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.720170 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/
+-rw-rw-rw-   0        0        0     3789 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/EnvelopePower.py
+-rw-rw-rw-   0        0        0     3053 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Frequency.py
+-rw-rw-rw-   0        0        0     3118 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Retrigger.py
+-rw-rw-rw-   0        0        0     2425 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Sstop.py
+-rw-rw-rw-   0        0        0     5646 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/__init__.py
+-rw-rw-rw-   0        0        0     1463 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/Trigger.py
+-rw-rw-rw-   0        0        0    10961 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.722122 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.727980 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/
+-rw-rw-rw-   0        0        0     1969 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/Frequency.py
+-rw-rw-rw-   0        0        0     1891 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/__init__.py
+-rw-rw-rw-   0        0        0     6078 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.732857 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.738714 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/ListPy/
+-rw-rw-rw-   0        0        0     3163 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/ListPy/Frequency.py
+-rw-rw-rw-   0        0        0     1052 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/ListPy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.744571 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/
+-rw-rw-rw-   0        0        0     3270 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/File.py
+-rw-rw-rw-   0        0        0     1904 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/__init__.py
+-rw-rw-rw-   0        0        0     1386 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/View.py
+-rw-rw-rw-   0        0        0     3556 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.752378 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/
+-rw-rw-rw-   0        0        0      900 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/Catalog.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.761163 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/
+-rw-rw-rw-   0        0        0     1469 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/Bandpass.py
+-rw-rw-rw-   0        0        0     1445 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/Gauss.py
+-rw-rw-rw-   0        0        0     2945 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.784589 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/
+-rw-rw-rw-   0        0        0     2423 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Cidx.py
+-rw-rw-rw-   0        0        0     3755 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/EnvelopePower.py
+-rw-rw-rw-   0        0        0     3019 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Frequency.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.789468 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.795323 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/Catalog/
+-rw-rw-rw-   0        0        0     1302 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/Catalog/Connection.py
+-rw-rw-rw-   0        0        0     1069 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/Catalog/__init__.py
+-rw-rw-rw-   0        0        0     2342 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/Connection.py
+-rw-rw-rw-   0        0        0     2119 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/__init__.py
+-rw-rw-rw-   0        0        0     3464 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/IqData.py
+-rw-rw-rw-   0        0        0     3204 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Irepetition.py
+-rw-rw-rw-   0        0        0     2828 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/ParameterSetList.py
+-rw-rw-rw-   0        0        0     3080 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Retrigger.py
+-rw-rw-rw-   0        0        0     2419 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Sstop.py
+-rw-rw-rw-   0        0        0    15308 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.808987 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/
+-rw-rw-rw-   0        0        0     1126 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Catalog.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.815818 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.821675 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandpass/
+-rw-rw-rw-   0        0        0     3261 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandpass/Bandwidth.py
+-rw-rw-rw-   0        0        0     1066 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandpass/__init__.py
+-rw-rw-rw-   0        0        0     2729 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandwidth.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.826556 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Gauss/
+-rw-rw-rw-   0        0        0     3285 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Gauss/Bandwidth.py
+-rw-rw-rw-   0        0        0     1051 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Gauss/__init__.py
+-rw-rw-rw-   0        0        0     4452 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/TypePy.py
+-rw-rw-rw-   0        0        0     1780 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/__init__.py
+-rw-rw-rw-   0        0        0     3391 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Mlength.py
+-rw-rw-rw-   0        0        0     2509 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/PdefSet.py
+-rw-rw-rw-   0        0        0     3053 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Slength.py
+-rw-rw-rw-   0        0        0     3387 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/__init__.py
+-rw-rw-rw-   0        0        0     1449 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/Trigger.py
+-rw-rw-rw-   0        0        0    11165 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.832411 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/RfSettings/
+-rw-rw-rw-   0        0        0     1285 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/RfSettings/LrStart.py
+-rw-rw-rw-   0        0        0     9793 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/RfSettings/__init__.py
+-rw-rw-rw-   0        0        0     1431 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Scenario.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.835339 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.849002 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/
+-rw-rw-rw-   0        0        0     2118 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Rbw.py
+-rw-rw-rw-   0        0        0     2188 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Swt.py
+-rw-rw-rw-   0        0        0     2196 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Vbw.py
+-rw-rw-rw-   0        0        0     3640 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.861691 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/Frequency/
+-rw-rw-rw-   0        0        0     2365 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/Frequency/Span.py
+-rw-rw-rw-   0        0        0     4653 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/Frequency/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.870474 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/
+-rw-rw-rw-   0        0        0     3239 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/Rbw.py
+-rw-rw-rw-   0        0        0     2184 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/Vbw.py
+-rw-rw-rw-   0        0        0     3844 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/__init__.py
+-rw-rw-rw-   0        0        0     5241 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/__init__.py
+-rw-rw-rw-   0        0        0     3857 2024-05-24 14:33:44.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1315 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.881212 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.884138 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.886091 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.894876 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/
+-rw-rw-rw-   0        0        0     1672 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/Globale.py
+-rw-rw-rw-   0        0        0     1706 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/Tenvironment.py
+-rw-rw-rw-   0        0        0     1310 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/__init__.py
+-rw-rw-rw-   0        0        0     1055 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/__init__.py
+-rw-rw-rw-   0        0        0     1121 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.906587 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Control/
+-rw-rw-rw-   0        0        0     1162 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Control/Reboot.py
+-rw-rw-rw-   0        0        0     1171 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Control/Restart.py
+-rw-rw-rw-   0        0        0     1180 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Control/Shutdown.py
+-rw-rw-rw-   0        0        0     1525 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Control/__init__.py
+-rw-rw-rw-   0        0        0     2171 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Edevice.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.919275 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Positioner/
+-rw-rw-rw-   0        0        0     1645 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Positioner/HwProperties.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.925132 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Move/
+-rw-rw-rw-   0        0        0     1377 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Move/To.py
+-rw-rw-rw-   0        0        0      984 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Move/__init__.py
+-rw-rw-rw-   0        0        0     1876 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Moving.py
+-rw-rw-rw-   0        0        0     1669 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Versions.py
+-rw-rw-rw-   0        0        0     2687 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Positioner/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.930010 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Recall/
+-rw-rw-rw-   0        0        0     1723 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Recall/Partial.py
+-rw-rw-rw-   0        0        0     1032 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Recall/__init__.py
+-rw-rw-rw-   0        0        0      891 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Reset.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.932939 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rf42/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.935867 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.943675 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/
+-rw-rw-rw-   0        0        0     1861 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/Rx.py
+-rw-rw-rw-   0        0        0     1825 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/Tx.py
+-rw-rw-rw-   0        0        0     1205 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/__init__.py
+-rw-rw-rw-   0        0        0     1817 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/__init__.py
+-rw-rw-rw-   0        0        0      990 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rf42/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.945627 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.948555 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.957340 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/
+-rw-rw-rw-   0        0        0     1729 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/Rx.py
+-rw-rw-rw-   0        0        0     1729 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/Tx.py
+-rw-rw-rw-   0        0        0     1200 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/__init__.py
+-rw-rw-rw-   0        0        0     1006 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/__init__.py
+-rw-rw-rw-   0        0        0      992 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.963196 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Save/
+-rw-rw-rw-   0        0        0     1173 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Save/Partial.py
+-rw-rw-rw-   0        0        0     1022 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Save/__init__.py
+-rw-rw-rw-   0        0        0     1856 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Vse.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.968076 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Z310/
+-rw-rw-rw-   0        0        0     1323 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Z310/Attenuation.py
+-rw-rw-rw-   0        0        0     1054 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Z310/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.972956 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Z320/
+-rw-rw-rw-   0        0        0     1323 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Z320/Attenuation.py
+-rw-rw-rw-   0        0        0     1054 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Z320/__init__.py
+-rw-rw-rw-   0        0        0     3612 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.975884 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.983692 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.991500 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/
+-rw-rw-rw-   0        0        0     1689 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/Rx.py
+-rw-rw-rw-   0        0        0     1689 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/Tx.py
+-rw-rw-rw-   0        0        0     1223 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.999308 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/
+-rw-rw-rw-   0        0        0     1828 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/Rx.py
+-rw-rw-rw-   0        0        0     1828 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/Tx.py
+-rw-rw-rw-   0        0        0     1243 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/__init__.py
+-rw-rw-rw-   0        0        0     1914 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Direction.py
+-rw-rw-rw-   0        0        0     2359 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Info.py
+-rw-rw-rw-   0        0        0     1847 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/__init__.py
+-rw-rw-rw-   0        0        0     1044 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/__init__.py
+-rw-rw-rw-   0        0        0     1542 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.002236 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Create/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.004188 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Create/System/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.007116 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Create/System/Attenuation/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.014923 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/
+-rw-rw-rw-   0        0        0     1327 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/Globale.py
+-rw-rw-rw-   0        0        0     1381 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/Tenvironment.py
+-rw-rw-rw-   0        0        0     1363 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/__init__.py
+-rw-rw-rw-   0        0        0     1121 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Create/System/Attenuation/__init__.py
+-rw-rw-rw-   0        0        0     1062 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Create/System/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.020779 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Create/Tenvironment/
+-rw-rw-rw-   0        0        0     1405 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Create/Tenvironment/Spath.py
+-rw-rw-rw-   0        0        0     1044 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Create/Tenvironment/__init__.py
+-rw-rw-rw-   0        0        0     1304 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Create/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.023708 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.026636 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.031515 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/
+-rw-rw-rw-   0        0        0     1263 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/Connectors.py
+-rw-rw-rw-   0        0        0     1056 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/__init__.py
+-rw-rw-rw-   0        0        0     1027 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.033467 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.038348 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/Gprf/
+-rw-rw-rw-   0        0        0     1225 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/Gprf/Measurement.py
+-rw-rw-rw-   0        0        0     1054 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/Gprf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.041277 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.043228 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.045180 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.047132 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.052988 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/
+-rw-rw-rw-   0        0        0     2337 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/FilterPy.py
+-rw-rw-rw-   0        0        0     2757 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.057869 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Rpc/
+-rw-rw-rw-   0        0        0     2325 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Rpc/FilterPy.py
+-rw-rw-rw-   0        0        0     2740 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Rpc/__init__.py
+-rw-rw-rw-   0        0        0     1216 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.060796 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.066652 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Psub/
+-rw-rw-rw-   0        0        0     2337 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Psub/FilterPy.py
+-rw-rw-rw-   0        0        0     2757 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Psub/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.072509 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Rpc/
+-rw-rw-rw-   0        0        0     2325 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Rpc/FilterPy.py
+-rw-rw-rw-   0        0        0     2740 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Rpc/__init__.py
+-rw-rw-rw-   0        0        0     1216 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/__init__.py
+-rw-rw-rw-   0        0        0     1238 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/__init__.py
+-rw-rw-rw-   0        0        0     1025 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.077388 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Scpi/
+-rw-rw-rw-   0        0        0     1981 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Scpi/Logging.py
+-rw-rw-rw-   0        0        0     1024 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Scpi/__init__.py
+-rw-rw-rw-   0        0        0     1229 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/__init__.py
+-rw-rw-rw-   0        0        0     1258 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.080316 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.085196 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/Power/
+-rw-rw-rw-   0        0        0     2255 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/Power/State.py
+-rw-rw-rw-   0        0        0     1011 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/Power/__init__.py
+-rw-rw-rw-   0        0        0     1009 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.088123 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Generic/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.093004 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Generic/Measurement/
+-rw-rw-rw-   0        0        0     1191 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Generic/Measurement/Dapi.py
+-rw-rw-rw-   0        0        0     1033 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Generic/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1067 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Generic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.094956 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.113501 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/
+-rw-rw-rw-   0        0        0     1231 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Correction.py
+-rw-rw-rw-   0        0        0      834 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfProperty.py
+-rw-rw-rw-   0        0        0     1314 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfSettings.py
+-rw-rw-rw-   0        0        0     1311 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfSetttings.py
+-rw-rw-rw-   0        0        0     1211 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Rms.py
+-rw-rw-rw-   0        0        0     2062 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Snumber.py
+-rw-rw-rw-   0        0        0     3120 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.119356 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.126188 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Ploss/
+-rw-rw-rw-   0        0        0     1320 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Ploss/Rnames.py
+-rw-rw-rw-   0        0        0     2409 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Ploss/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.146684 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.151564 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Bandpass/
+-rw-rw-rw-   0        0        0     2381 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Bandpass/Bandwidth.py
+-rw-rw-rw-   0        0        0     1062 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Bandpass/__init__.py
+-rw-rw-rw-   0        0        0      865 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Franges.py
+-rw-rw-rw-   0        0        0     2332 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Frequency.py
+-rw-rw-rw-   0        0        0     2276 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Fspan.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.156444 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Gauss/
+-rw-rw-rw-   0        0        0     2363 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Gauss/Bandwidth.py
+-rw-rw-rw-   0        0        0     1047 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Gauss/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.161324 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.165231 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Bandpass/
+-rw-rw-rw-   0        0        0     2454 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Bandpass/Bandwidth.py
+-rw-rw-rw-   0        0        0     1064 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Bandpass/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.171084 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Gauss/
+-rw-rw-rw-   0        0        0     2436 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Gauss/Bandwidth.py
+-rw-rw-rw-   0        0        0     1049 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Gauss/__init__.py
+-rw-rw-rw-   0        0        0     2377 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Samples.py
+-rw-rw-rw-   0        0        0     1536 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.176940 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/ListPy/
+-rw-rw-rw-   0        0        0     2345 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/ListPy/Iranges.py
+-rw-rw-rw-   0        0        0     1036 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/ListPy/__init__.py
+-rw-rw-rw-   0        0        0     1357 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/LoFrequency.py
+-rw-rw-rw-   0        0        0     2304 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/NbLevel.py
+-rw-rw-rw-   0        0        0     2326 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/SymbolRate.py
+-rw-rw-rw-   0        0        0     4175 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/__init__.py
+-rw-rw-rw-   0        0        0     2046 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Snumber.py
+-rw-rw-rw-   0        0        0     3535 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1313 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.182798 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Meas/
+-rw-rw-rw-   0        0        0     1125 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Meas/Scpi.py
+-rw-rw-rw-   0        0        0      996 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Meas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.185725 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Route/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.193532 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/
+-rw-rw-rw-   0        0        0     1301 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/Generator.py
+-rw-rw-rw-   0        0        0     1319 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/Measurement.py
+-rw-rw-rw-   0        0        0     1314 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.199389 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Route/NrMmw/
+-rw-rw-rw-   0        0        0     1325 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Route/NrMmw/Measurement.py
+-rw-rw-rw-   0        0        0     1059 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Route/NrMmw/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.204269 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Route/Uwb/
+-rw-rw-rw-   0        0        0     1313 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Route/Uwb/Measurement.py
+-rw-rw-rw-   0        0        0     1049 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Route/Uwb/__init__.py
+-rw-rw-rw-   0        0        0     1441 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Route/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.207198 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.209149 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.215005 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/Debug/
+-rw-rw-rw-   0        0        0     2310 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/Debug/Output.py
+-rw-rw-rw-   0        0        0     1021 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/Debug/__init__.py
+-rw-rw-rw-   0        0        0     1001 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/__init__.py
+-rw-rw-rw-   0        0        0     1003 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/__init__.py
+-rw-rw-rw-   0        0        0     2693 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.216957 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.219885 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.221837 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.226717 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/State/
+-rw-rw-rw-   0        0        0     2115 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/State/All.py
+-rw-rw-rw-   0        0        0     2756 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/State/__init__.py
+-rw-rw-rw-   0        0        0     3733 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.229645 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.233549 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/State/
+-rw-rw-rw-   0        0        0     2116 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/State/All.py
+-rw-rw-rw-   0        0        0     2757 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/State/__init__.py
+-rw-rw-rw-   0        0        0     6124 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.242333 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/
+-rw-rw-rw-   0        0        0     1845 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Icomponent.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.250141 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/
+-rw-rw-rw-   0        0        0     2613 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/Average.py
+-rw-rw-rw-   0        0        0     2613 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/Current.py
+-rw-rw-rw-   0        0        0     1273 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.265757 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/
+-rw-rw-rw-   0        0        0     2034 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Average.py
+-rw-rw-rw-   0        0        0     2034 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Current.py
+-rw-rw-rw-   0        0        0     2034 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Maximum.py
+-rw-rw-rw-   0        0        0     2034 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Minimum.py
+-rw-rw-rw-   0        0        0     1761 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/__init__.py
+-rw-rw-rw-   0        0        0     1845 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Qcomponent.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.270637 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/State/
+-rw-rw-rw-   0        0        0     2121 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/State/All.py
+-rw-rw-rw-   0        0        0     2762 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/State/__init__.py
+-rw-rw-rw-   0        0        0     4744 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.283326 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/
+-rw-rw-rw-   0        0        0     1553 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Bin.py
+-rw-rw-rw-   0        0        0      944 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Reliability.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.288205 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/State/
+-rw-rw-rw-   0        0        0     2118 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/State/All.py
+-rw-rw-rw-   0        0        0     2759 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/State/__init__.py
+-rw-rw-rw-   0        0        0      920 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/SymbolRate.py
+-rw-rw-rw-   0        0        0     1656 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Talignment.py
+-rw-rw-rw-   0        0        0     7279 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.308702 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/
+-rw-rw-rw-   0        0        0     1792 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/FreqError.py
+-rw-rw-rw-   0        0        0     1731 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Icomponent.py
+-rw-rw-rw-   0        0        0     1708 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Level.py
+-rw-rw-rw-   0        0        0     3029 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/OfError.py
+-rw-rw-rw-   0        0        0     1708 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Phase.py
+-rw-rw-rw-   0        0        0     1731 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Qcomponent.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.314557 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/State/
+-rw-rw-rw-   0        0        0     2110 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/State/All.py
+-rw-rw-rw-   0        0        0     2751 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/State/__init__.py
+-rw-rw-rw-   0        0        0     5210 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.318464 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.325295 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/Sensor/
+-rw-rw-rw-   0        0        0     4990 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/Sensor/Power.py
+-rw-rw-rw-   0        0        0     1855 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/Sensor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.331150 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/State/
+-rw-rw-rw-   0        0        0     2100 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/State/All.py
+-rw-rw-rw-   0        0        0     2741 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/State/__init__.py
+-rw-rw-rw-   0        0        0     3899 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.336029 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/
+-rw-rw-rw-   0        0        0     1254 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Clear.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.350669 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/
+-rw-rw-rw-   0        0        0     1062 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Eoo.py
+-rw-rw-rw-   0        0        0     1062 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Ezo.py
+-rw-rw-rw-   0        0        0     1062 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Ezz.py
+-rw-rw-rw-   0        0        0     1097 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Frequency.py
+-rw-rw-rw-   0        0        0     1686 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.361407 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/
+-rw-rw-rw-   0        0        0     1708 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Frequency.py
+-rw-rw-rw-   0        0        0     1452 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Gain.py
+-rw-rw-rw-   0        0        0     1652 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/State.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.369214 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Trace/
+-rw-rw-rw-   0        0        0     1733 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Trace/Frequency.py
+-rw-rw-rw-   0        0        0     1477 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Trace/Gain.py
+-rw-rw-rw-   0        0        0     1267 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Trace/__init__.py
+-rw-rw-rw-   0        0        0     2778 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.375070 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Match/
+-rw-rw-rw-   0        0        0     1348 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Match/State.py
+-rw-rw-rw-   0        0        0     1861 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Match/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.379949 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Open/
+-rw-rw-rw-   0        0        0     1634 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Open/State.py
+-rw-rw-rw-   0        0        0     2026 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Open/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.384830 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Short/
+-rw-rw-rw-   0        0        0     1638 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Short/State.py
+-rw-rw-rw-   0        0        0     2037 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Short/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.388734 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/
+-rw-rw-rw-   0        0        0     2103 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/All.py
+-rw-rw-rw-   0        0        0     2744 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/__init__.py
+-rw-rw-rw-   0        0        0     3588 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.399469 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/
+-rw-rw-rw-   0        0        0     1152 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/AmplitudeProbDensity.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.405325 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Average/
+-rw-rw-rw-   0        0        0     1620 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Average/Rms.py
+-rw-rw-rw-   0        0        0     4648 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Average/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.416061 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/
+-rw-rw-rw-   0        0        0     1741 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Power.py
+-rw-rw-rw-   0        0        0     1340 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Probability.py
+-rw-rw-rw-   0        0        0     1485 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Sample.py
+-rw-rw-rw-   0        0        0     2322 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.426798 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/
+-rw-rw-rw-   0        0        0     1656 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Maximum.py
+-rw-rw-rw-   0        0        0     1656 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Minimum.py
+-rw-rw-rw-   0        0        0     1620 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Rms.py
+-rw-rw-rw-   0        0        0     5136 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/__init__.py
+-rw-rw-rw-   0        0        0     1170 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ElapsedStats.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.431677 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqData/
+-rw-rw-rw-   0        0        0     1518 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqData/Bin.py
+-rw-rw-rw-   0        0        0     3002 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqData/__init__.py
+-rw-rw-rw-   0        0        0     1998 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqInfo.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.442415 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/
+-rw-rw-rw-   0        0        0     4420 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Average.py
+-rw-rw-rw-   0        0        0     4420 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Current.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.447294 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Maximum/
+-rw-rw-rw-   0        0        0     4498 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Maximum/Current.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Maximum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.453151 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Minimum/
+-rw-rw-rw-   0        0        0     4498 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Minimum/Current.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Minimum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.460959 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/
+-rw-rw-rw-   0        0        0     4471 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/Maximum.py
+-rw-rw-rw-   0        0        0     4471 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/Minimum.py
+-rw-rw-rw-   0        0        0     1270 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/__init__.py
+-rw-rw-rw-   0        0        0     4462 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/StandardDev.py
+-rw-rw-rw-   0        0        0     2263 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.469743 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/
+-rw-rw-rw-   0        0        0     4111 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/Current.py
+-rw-rw-rw-   0        0        0     1656 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/Maximum.py
+-rw-rw-rw-   0        0        0     1283 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.478526 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/
+-rw-rw-rw-   0        0        0     4111 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/Current.py
+-rw-rw-rw-   0        0        0     1656 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/Minimum.py
+-rw-rw-rw-   0        0        0     1283 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.487311 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/
+-rw-rw-rw-   0        0        0     4084 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/Maximum.py
+-rw-rw-rw-   0        0        0     4084 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/Minimum.py
+-rw-rw-rw-   0        0        0     1268 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.494142 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/StandardDev/
+-rw-rw-rw-   0        0        0     1676 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/StandardDev/Current.py
+-rw-rw-rw-   0        0        0     4730 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/StandardDev/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.499998 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/State/
+-rw-rw-rw-   0        0        0     2103 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/State/All.py
+-rw-rw-rw-   0        0        0     2744 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/State/__init__.py
+-rw-rw-rw-   0        0        0     6839 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.501951 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.516590 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/
+-rw-rw-rw-   0        0        0     1650 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Average.py
+-rw-rw-rw-   0        0        0     1650 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Current.py
+-rw-rw-rw-   0        0        0     1650 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Maximum.py
+-rw-rw-rw-   0        0        0     1650 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Minimum.py
+-rw-rw-rw-   0        0        0     1771 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.523423 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Marker/
+-rw-rw-rw-   0        0        0     2350 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Marker/Npeak.py
+-rw-rw-rw-   0        0        0     1855 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Marker/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.542943 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/
+-rw-rw-rw-   0        0        0     1650 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Average.py
+-rw-rw-rw-   0        0        0     1650 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Current.py
+-rw-rw-rw-   0        0        0     1650 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Maximum.py
+-rw-rw-rw-   0        0        0     1650 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Minimum.py
+-rw-rw-rw-   0        0        0     1771 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.561487 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/
+-rw-rw-rw-   0        0        0     1650 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Average.py
+-rw-rw-rw-   0        0        0     1650 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Current.py
+-rw-rw-rw-   0        0        0     1650 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Maximum.py
+-rw-rw-rw-   0        0        0     1650 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Minimum.py
+-rw-rw-rw-   0        0        0     1771 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.571246 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/
+-rw-rw-rw-   0        0        0     2059 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/Npeak.py
+-rw-rw-rw-   0        0        0     2059 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/Speak.py
+-rw-rw-rw-   0        0        0     1291 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.586862 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/
+-rw-rw-rw-   0        0        0     1626 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Average.py
+-rw-rw-rw-   0        0        0     1626 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Current.py
+-rw-rw-rw-   0        0        0     1626 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Maximum.py
+-rw-rw-rw-   0        0        0     1626 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Minimum.py
+-rw-rw-rw-   0        0        0     1751 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.601503 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/
+-rw-rw-rw-   0        0        0     1644 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Average.py
+-rw-rw-rw-   0        0        0     1644 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Current.py
+-rw-rw-rw-   0        0        0     1644 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Maximum.py
+-rw-rw-rw-   0        0        0     1644 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Minimum.py
+-rw-rw-rw-   0        0        0     1766 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.607360 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/State/
+-rw-rw-rw-   0        0        0     1804 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/State/All.py
+-rw-rw-rw-   0        0        0     2368 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/State/__init__.py
+-rw-rw-rw-   0        0        0     3902 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/__init__.py
+-rw-rw-rw-   0        0        0     3066 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.610288 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Modify/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.613216 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Modify/System/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.615167 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.623952 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/
+-rw-rw-rw-   0        0        0     1329 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/Globale.py
+-rw-rw-rw-   0        0        0     1363 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/Tenvironment.py
+-rw-rw-rw-   0        0        0     1363 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/__init__.py
+-rw-rw-rw-   0        0        0     1121 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/__init__.py
+-rw-rw-rw-   0        0        0     1062 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Modify/System/__init__.py
+-rw-rw-rw-   0        0        0     1020 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Modify/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.626880 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.629807 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/System/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.633713 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.643472 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/
+-rw-rw-rw-   0        0        0     1293 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/Globale.py
+-rw-rw-rw-   0        0        0     1327 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/Tenvironment.py
+-rw-rw-rw-   0        0        0     1363 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/__init__.py
+-rw-rw-rw-   0        0        0     1121 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/__init__.py
+-rw-rw-rw-   0        0        0     1062 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/System/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.646399 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/Tenvironment/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.648351 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.657135 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/
+-rw-rw-rw-   0        0        0     1237 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/Rx.py
+-rw-rw-rw-   0        0        0     1237 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/Tx.py
+-rw-rw-rw-   0        0        0     1243 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/__init__.py
+-rw-rw-rw-   0        0        0     1091 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/__init__.py
+-rw-rw-rw-   0        0        0     1044 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/Tenvironment/__init__.py
+-rw-rw-rw-   0        0        0     1304 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.660064 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Results/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.662991 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Results/Gprf/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.665920 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.671775 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/Power/
+-rw-rw-rw-   0        0        0     1633 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/Power/Current.py
+-rw-rw-rw-   0        0        0     1029 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/Power/__init__.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Results/Gprf/__init__.py
+-rw-rw-rw-   0        0        0     1009 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Results/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.674703 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.677631 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Bluetooth/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.683487 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Bluetooth/Measurement/
+-rw-rw-rw-   0        0        0     1670 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Bluetooth/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Bluetooth/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1077 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Bluetooth/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.689345 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Cdma/
+-rw-rw-rw-   0        0        0     1250 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Cdma/Measurement.py
+-rw-rw-rw-   0        0        0     1052 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Cdma/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.693248 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.698128 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/
+-rw-rw-rw-   0        0        0     1449 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/RfSettings.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.704959 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/Spath/
+-rw-rw-rw-   0        0        0     2377 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/Spath/Group.py
+-rw-rw-rw-   0        0        0     2525 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/Spath/__init__.py
+-rw-rw-rw-   0        0        0     1299 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.712767 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/
+-rw-rw-rw-   0        0        0     1441 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/RfSettings.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.718625 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Scenario/
+-rw-rw-rw-   0        0        0      888 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Scenario/Catalog.py
+-rw-rw-rw-   0        0        0     1044 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Scenario/__init__.py
+-rw-rw-rw-   0        0        0     3754 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1561 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1312 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.721551 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gsm/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.726432 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gsm/Measurement/
+-rw-rw-rw-   0        0        0     1616 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gsm/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gsm/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1047 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gsm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.730336 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Lte/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.755819 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Lte/Measurement/
+-rw-rw-rw-   0        0        0     1616 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Lte/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Lte/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1047 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Lte/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.734239 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/LteDl/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.744001 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/LteDl/Measurement/
+-rw-rw-rw-   0        0        0     1634 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/LteDl/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/LteDl/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/LteDl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.764497 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Niot/
+-rw-rw-rw-   0        0        0     1250 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Niot/Measurement.py
+-rw-rw-rw-   0        0        0     1052 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Niot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.768401 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrDl/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.777184 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrDl/Measurement/
+-rw-rw-rw-   0        0        0     1625 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrDl/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrDl/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrDl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.780112 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrMmw/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.784993 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrMmw/Measurement/
+-rw-rw-rw-   0        0        0     1634 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrMmw/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrMmw/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrMmw/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.787921 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrSub/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.795728 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrSub/Measurement/
+-rw-rw-rw-   0        0        0     1634 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrSub/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrSub/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrSub/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.799632 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Uwb/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.807441 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Uwb/Measurement/
+-rw-rw-rw-   0        0        0     1616 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Uwb/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Uwb/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1047 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Uwb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.810369 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wcdma/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.818176 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wcdma/Measurement/
+-rw-rw-rw-   0        0        0     1634 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wcdma/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wcdma/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wcdma/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.823057 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wlan/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.830864 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wlan/Measurement/
+-rw-rw-rw-   0        0        0     1625 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wlan/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wlan/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wlan/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.836721 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wpan/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.846480 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/
+-rw-rw-rw-   0        0        0     1625 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wpan/__init__.py
+-rw-rw-rw-   0        0        0     3909 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.849409 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.854293 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/Base/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.858192 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.865025 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/
+-rw-rw-rw-   0        0        0     1813 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/Ambient.py
+-rw-rw-rw-   0        0        0     1049 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/__init__.py
+-rw-rw-rw-   0        0        0     1073 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/Base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.867952 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/System/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.876737 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/System/Positioner/
+-rw-rw-rw-   0        0        0     1124 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/System/Positioner/IsMoving.py
+-rw-rw-rw-   0        0        0     1619 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/System/Positioner/Position.py
+-rw-rw-rw-   0        0        0     2199 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/System/Positioner/__init__.py
+-rw-rw-rw-   0        0        0     1054 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/System/__init__.py
+-rw-rw-rw-   0        0        0     1235 2024-05-24 14:33:47.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.880641 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.883568 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.896256 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.906016 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/
+-rw-rw-rw-   0        0        0     4136 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/File.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.911873 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Marker/
+-rw-rw-rw-   0        0        0     2565 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Marker/Delays.py
+-rw-rw-rw-   0        0        0     1028 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Marker/__init__.py
+-rw-rw-rw-   0        0        0     3268 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Msegment.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.916752 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Samples/
+-rw-rw-rw-   0        0        0     2372 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Samples/Range.py
+-rw-rw-rw-   0        0        0     1536 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Samples/__init__.py
+-rw-rw-rw-   0        0        0     2323 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Segments.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.922608 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/UdMarker/
+-rw-rw-rw-   0        0        0     1253 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/UdMarker/Clist.py
+-rw-rw-rw-   0        0        0     3222 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/UdMarker/__init__.py
+-rw-rw-rw-   0        0        0     9112 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.930416 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/
+-rw-rw-rw-   0        0        0     2628 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/Level.py
+-rw-rw-rw-   0        0        0     3652 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/Ofrequency.py
+-rw-rw-rw-   0        0        0     2150 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/__init__.py
+-rw-rw-rw-   0        0        0     3390 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/IqSettings.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.974338 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/
+-rw-rw-rw-   0        0        0     2475 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Dgain.py
+-rw-rw-rw-   0        0        0     2448 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Dtime.py
+-rw-rw-rw-   0        0        0     1225 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Esingle.py
+-rw-rw-rw-   0        0        0     3782 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Fill.py
+-rw-rw-rw-   0        0        0     2507 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Frequency.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.980193 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Increment/
+-rw-rw-rw-   0        0        0     1811 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Increment/Enabling.py
+-rw-rw-rw-   0        0        0     2412 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Increment/__init__.py
+-rw-rw-rw-   0        0        0     2531 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Irepetition.py
+-rw-rw-rw-   0        0        0     2539 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Modulation.py
+-rw-rw-rw-   0        0        0     2529 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Reenabling.py
+-rw-rw-rw-   0        0        0     2607 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/RfLevel.py
+-rw-rw-rw-   0        0        0     1207 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Rlist.py
+-rw-rw-rw-   0        0        0     1207 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Slist.py
+-rw-rw-rw-   0        0        0     2189 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Sstop.py
+-rw-rw-rw-   0        0        0    10413 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/__init__.py
+-rw-rw-rw-   0        0        0     2717 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Reliability.py
+-rw-rw-rw-   0        0        0     5682 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/RfSettings.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:53.991905 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.034849 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/
+-rw-rw-rw-   0        0        0     1635 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Check.py
+-rw-rw-rw-   0        0        0     1762 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/CrcProtect.py
+-rw-rw-rw-   0        0        0     1364 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Download.py
+-rw-rw-rw-   0        0        0     1515 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Duration.py
+-rw-rw-rw-   0        0        0     1544 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Paratio.py
+-rw-rw-rw-   0        0        0     1627 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Path.py
+-rw-rw-rw-   0        0        0     1518 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Poffset.py
+-rw-rw-rw-   0        0        0     1694 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Reliability.py
+-rw-rw-rw-   0        0        0     1733 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Rmessage.py
+-rw-rw-rw-   0        0        0     1589 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Roption.py
+-rw-rw-rw-   0        0        0     1510 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Samples.py
+-rw-rw-rw-   0        0        0     1525 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/SymbolRate.py
+-rw-rw-rw-   0        0        0     1591 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Waveform.py
+-rw-rw-rw-   0        0        0     8460 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.040705 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Dtone/
+-rw-rw-rw-   0        0        0     3565 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Dtone/Ofrequency.py
+-rw-rw-rw-   0        0        0     1985 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Dtone/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.071937 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/
+-rw-rw-rw-   0        0        0     2846 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Acycles.py
+-rw-rw-rw-   0        0        0     2850 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Dgain.py
+-rw-rw-rw-   0        0        0     2810 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Dtime.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.086577 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/
+-rw-rw-rw-   0        0        0     1418 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Call.py
+-rw-rw-rw-   0        0        0     1136 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Insert.py
+-rw-rw-rw-   0        0        0     1126 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Mdown.py
+-rw-rw-rw-   0        0        0     1110 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Mup.py
+-rw-rw-rw-   0        0        0     2484 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.101218 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/
+-rw-rw-rw-   0        0        0     1519 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Apply.py
+-rw-rw-rw-   0        0        0     3570 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Dgain.py
+-rw-rw-rw-   0        0        0     3758 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Frequency.py
+-rw-rw-rw-   0        0        0     3507 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Lrms.py
+-rw-rw-rw-   0        0        0     3555 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/__init__.py
+-rw-rw-rw-   0        0        0     3163 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Frequency.py
+-rw-rw-rw-   0        0        0     3702 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Itransition.py
+-rw-rw-rw-   0        0        0     5060 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Lincrement.py
+-rw-rw-rw-   0        0        0     2772 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Lrms.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.110002 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.120739 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/
+-rw-rw-rw-   0        0        0     1312 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Cw.py
+-rw-rw-rw-   0        0        0     1339 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Dtone.py
+-rw-rw-rw-   0        0        0     1321 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Off.py
+-rw-rw-rw-   0        0        0     5147 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/__init__.py
+-rw-rw-rw-   0        0        0     2440 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Catalog.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.126593 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Index/
+-rw-rw-rw-   0        0        0     2186 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Index/All.py
+-rw-rw-rw-   0        0        0     2969 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Index/__init__.py
+-rw-rw-rw-   0        0        0     2097 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Range.py
+-rw-rw-rw-   0        0        0     3415 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.129522 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.132450 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.134401 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.140257 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/Tx/
+-rw-rw-rw-   0        0        0     3080 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/Tx/Single.py
+-rw-rw-rw-   0        0        0     1016 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/Tx/__init__.py
+-rw-rw-rw-   0        0        0     4245 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/__init__.py
+-rw-rw-rw-   0        0        0     3224 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/__init__.py
+-rw-rw-rw-   0        0        0     1017 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/__init__.py
+-rw-rw-rw-   0        0        0     1538 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/SymbolRate.py
+-rw-rw-rw-   0        0        0     1519 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Ttime.py
+-rw-rw-rw-   0        0        0     5939 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.143185 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.148066 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/Delays/
+-rw-rw-rw-   0        0        0     2880 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/Delays/All.py
+-rw-rw-rw-   0        0        0     3365 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/Delays/__init__.py
+-rw-rw-rw-   0        0        0     1028 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/__init__.py
+-rw-rw-rw-   0        0        0     2786 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Reliability.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.152947 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/RfSettings/
+-rw-rw-rw-   0        0        0     2299 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/RfSettings/Spath.py
+-rw-rw-rw-   0        0        0     1040 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/RfSettings/__init__.py
+-rw-rw-rw-   0        0        0     1298 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Rmarker.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.158802 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/State/
+-rw-rw-rw-   0        0        0     2146 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/State/All.py
+-rw-rw-rw-   0        0        0     2133 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/State/__init__.py
+-rw-rw-rw-   0        0        0     1343 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Tdd.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.162706 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.170514 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/Delay/
+-rw-rw-rw-   0        0        0     2592 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/Delay/All.py
+-rw-rw-rw-   0        0        0     2470 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/Delay/__init__.py
+-rw-rw-rw-   0        0        0     1864 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/__init__.py
+-rw-rw-rw-   0        0        0     7520 2024-05-24 14:33:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.177346 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/State/
+-rw-rw-rw-   0        0        0     2088 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/State/All.py
+-rw-rw-rw-   0        0        0     1983 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/State/__init__.py
+-rw-rw-rw-   0        0        0     3944 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/__init__.py
+-rw-rw-rw-   0        0        0     1038 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/__init__.py
+-rw-rw-rw-   0        0        0     1006 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.180275 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.183203 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Attenuation/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.191987 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.199795 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/
+-rw-rw-rw-   0        0        0     1256 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/Globale.py
+-rw-rw-rw-   0        0        0     1309 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/Tenvironment.py
+-rw-rw-rw-   0        0        0     1303 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/__init__.py
+-rw-rw-rw-   0        0        0      805 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/Globale.py
+-rw-rw-rw-   0        0        0      839 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/Tenvironment.py
+-rw-rw-rw-   0        0        0     1573 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/__init__.py
+-rw-rw-rw-   0        0        0     1119 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Attenuation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.204674 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Date/
+-rw-rw-rw-   0        0        0     1988 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Date/Local.py
+-rw-rw-rw-   0        0        0     1004 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Date/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.210530 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Time/
+-rw-rw-rw-   0        0        0     2020 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Time/Local.py
+-rw-rw-rw-   0        0        0     2496 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Time/__init__.py
+-rw-rw-rw-   0        0        0     1500 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.216387 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Tenvironment/
+-rw-rw-rw-   0        0        0      789 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Tenvironment/Spath.py
+-rw-rw-rw-   0        0        0     1042 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Tenvironment/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.219315 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.223218 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.226146 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.232002 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/BhRate/
+-rw-rw-rw-   0        0        0      899 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/BhRate/Catalog.py
+-rw-rw-rw-   0        0        0     1932 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/BhRate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.236883 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdr/
+-rw-rw-rw-   0        0        0      890 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdr/Catalog.py
+-rw-rw-rw-   0        0        0     1899 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.242739 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdrp/
+-rw-rw-rw-   0        0        0      893 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdrp/Catalog.py
+-rw-rw-rw-   0        0        0     1910 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdrp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.248594 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      912 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1973 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     1741 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1077 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.251523 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Cdma/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.254450 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.261283 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      897 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1943 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     1073 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Cdma/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.264210 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.267138 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.272995 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/
+-rw-rw-rw-   0        0        0     1020 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Catalog.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.278850 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/
+-rw-rw-rw-   0        0        0     1265 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/Execute.py
+-rw-rw-rw-   0        0        0     1036 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.281779 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.287635 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/
+-rw-rw-rw-   0        0        0     1321 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/Execute.py
+-rw-rw-rw-   0        0        0     1038 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/__init__.py
+-rw-rw-rw-   0        0        0     2034 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/__init__.py
+-rw-rw-rw-   0        0        0     5898 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.296419 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/
+-rw-rw-rw-   0        0        0     2194 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/IsMeas.py
+-rw-rw-rw-   0        0        0     2238 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/IsTrigger.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.303251 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/
+-rw-rw-rw-   0        0        0     1383 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/Execute.py
+-rw-rw-rw-   0        0        0     1036 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/__init__.py
+-rw-rw-rw-   0        0        0     2576 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/__init__.py
+-rw-rw-rw-   0        0        0     2270 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.309107 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.316914 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/
+-rw-rw-rw-   0        0        0     1056 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/Catalog.py
+-rw-rw-rw-   0        0        0     2344 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/OsStop.py
+-rw-rw-rw-   0        0        0     9301 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.321795 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqRecorder/
+-rw-rw-rw-   0        0        0     1054 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqRecorder/Catalog.py
+-rw-rw-rw-   0        0        0    10924 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqRecorder/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.327651 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqVsSlot/
+-rw-rw-rw-   0        0        0     1044 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqVsSlot/Catalog.py
+-rw-rw-rw-   0        0        0     9138 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqVsSlot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.333508 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/
+-rw-rw-rw-   0        0        0     1034 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/Catalog.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.339364 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/
+-rw-rw-rw-   0        0        0     2941 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/Offset.py
+-rw-rw-rw-   0        0        0     1078 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/__init__.py
+-rw-rw-rw-   0        0        0     9407 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/__init__.py
+-rw-rw-rw-   0        0        0     4768 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Spectrum.py
+-rw-rw-rw-   0        0        0     2074 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1313 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.343268 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gsm/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.346196 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.352051 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      894 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1937 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     1073 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1047 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gsm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.354980 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Lte/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.369619 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.375477 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      894 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1937 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/MultiEval/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.387187 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Prach/
+-rw-rw-rw-   0        0        0      878 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Prach/Catalog.py
+-rw-rw-rw-   0        0        0     1885 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Prach/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.394995 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Srs/
+-rw-rw-rw-   0        0        0      872 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Srs/Catalog.py
+-rw-rw-rw-   0        0        0     1863 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Srs/__init__.py
+-rw-rw-rw-   0        0        0     1513 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1047 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Lte/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.357908 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/LteDl/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.361811 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.366691 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      900 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1949 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     1073 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/LteDl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.396948 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Niot/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.399875 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.405732 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      897 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1943 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/MultiEval/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.411587 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/Prach/
+-rw-rw-rw-   0        0        0      881 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/Prach/Catalog.py
+-rw-rw-rw-   0        0        0     1891 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/Prach/__init__.py
+-rw-rw-rw-   0        0        0     1301 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Niot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.414515 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrDl/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.417444 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.423299 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      897 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1943 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     1073 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrDl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.426227 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrMmw/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.429156 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.434036 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      900 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1949 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/MultiEval/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.438916 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/Prach/
+-rw-rw-rw-   0        0        0      884 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/Prach/Catalog.py
+-rw-rw-rw-   0        0        0     1897 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/Prach/__init__.py
+-rw-rw-rw-   0        0        0     1301 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrMmw/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.441844 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrSub/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.444771 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.450627 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      900 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1949 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/MultiEval/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.456483 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Prach/
+-rw-rw-rw-   0        0        0      884 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Prach/Catalog.py
+-rw-rw-rw-   0        0        0     1897 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Prach/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.462339 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Srs/
+-rw-rw-rw-   0        0        0      878 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Srs/Catalog.py
+-rw-rw-rw-   0        0        0     1875 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Srs/__init__.py
+-rw-rw-rw-   0        0        0     1513 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrSub/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.464291 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Uwb/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.467220 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.472099 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      894 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1937 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     1073 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1047 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Uwb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.475027 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.477956 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.482836 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      900 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1949 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/MultiEval/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.488691 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OlpControl/
+-rw-rw-rw-   0        0        0      899 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OlpControl/Catalog.py
+-rw-rw-rw-   0        0        0     1952 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OlpControl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.494548 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OoSync/
+-rw-rw-rw-   0        0        0      887 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OoSync/Catalog.py
+-rw-rw-rw-   0        0        0     1908 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OoSync/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.499428 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Prach/
+-rw-rw-rw-   0        0        0      884 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Prach/Catalog.py
+-rw-rw-rw-   0        0        0     1897 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Prach/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.506260 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Tpc/
+-rw-rw-rw-   0        0        0      878 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Tpc/Catalog.py
+-rw-rw-rw-   0        0        0     1875 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Tpc/__init__.py
+-rw-rw-rw-   0        0        0     2018 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1058 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.509188 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wlan/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.512117 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.517972 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      897 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1943 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     1073 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wlan/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.520899 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wpan/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.523828 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.529684 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      897 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1943 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     1073 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-05-24 14:33:46.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wpan/__init__.py
+-rw-rw-rw-   0        0        0     3920 2024-05-24 14:33:45.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/__init__.py
+-rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:54.638021 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/
+-rw-rw-rw-   0        0        0      586 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ArgLinkedEventArgs.py
+-rw-rw-rw-   0        0        0     4165 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ArgSingle.py
+-rw-rw-rw-   0        0        0     1116 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ArgSingleList.py
+-rw-rw-rw-   0        0        0     1145 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ArgSingleSuppressed.py
+-rw-rw-rw-   0        0        0     9097 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ArgStringComposer.py
+-rw-rw-rw-   0        0        0     5751 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ArgStruct.py
+-rw-rw-rw-   0        0        0     3439 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ArgStructList.py
+-rw-rw-rw-   0        0        0     2546 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ArgStructStringParser.py
+-rw-rw-rw-   0        0        0     5238 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/CommandsGroup.py
+-rw-rw-rw-   0        0        0     5389 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ContextManagers.py
+-rw-rw-rw-   0        0        0    26718 2024-05-17 08:05:58.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/Conversions.py
+-rw-rw-rw-   0        0        0     3775 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ConverterFromScpiString.py
+-rw-rw-rw-   0        0        0     4768 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ConverterToScpiString.py
+-rw-rw-rw-   0        0        0    15275 2024-05-17 08:01:40.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/Core.py
+-rw-rw-rw-   0        0        0     1386 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/GlobalData.py
+-rw-rw-rw-   0        0        0    62242 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/Instrument.py
+-rw-rw-rw-   0        0        0     4775 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/InstrumentErrors.py
+-rw-rw-rw-   0        0        0     2225 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/InstrumentOptions.py
+-rw-rw-rw-   0        0        0    16283 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/InstrumentSettings.py
+-rw-rw-rw-   0        0        0     3518 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/InternalLinker.py
+-rw-rw-rw-   0        0        0     4390 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/IoTransferEventArgs.py
+-rw-rw-rw-   0        0        0      387 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/Properties.py
+-rw-rw-rw-   0        0        0     4289 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/RepeatedCapability.py
+-rw-rw-rw-   0        0        0     4745 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ScpiEnums.py
+-rw-rw-rw-   0        0        0    35917 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ScpiLogger.py
+-rw-rw-rw-   0        0        0     5098 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/StreamReader.py
+-rw-rw-rw-   0        0        0     5856 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/StreamWriter.py
+-rw-rw-rw-   0        0        0     1114 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/StructBase.py
+-rw-rw-rw-   0        0        0     3608 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/Types.py
+-rw-rw-rw-   0        0        0     8077 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/Utilities.py
+-rw-rw-rw-   0        0        0     5716 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/VisaPluginSocketIo.py
+-rw-rw-rw-   0        0        0    51976 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/VisaSession.py
+-rw-rw-rw-   0        0        0     7512 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/VisaSessionSim.py
+-rw-rw-rw-   0        0        0       29 2024-04-29 11:38:43.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/__init__.py
+-rw-rw-rw-   0        0        0    15874 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/RsCMPX_Gprf.py
+-rw-rw-rw-   0        0        0      899 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/__init__.py
+-rw-rw-rw-   0        0        0    11429 2024-05-24 14:33:42.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/enums.py
+-rw-rw-rw-   0        0        0     3704 2024-05-24 14:33:39.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/repcap.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:33:52.413705 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf.egg-info/
+-rw-rw-rw-   0        0        0     3697 2024-05-24 14:33:51.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    53144 2024-05-24 14:33:51.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 14:33:51.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-24 14:33:51.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-24 14:33:51.000000 RsCMPX_Gprf-5.0.92/RsCMPX_Gprf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 14:33:54.642902 RsCMPX_Gprf-5.0.92/setup.cfg
+-rw-rw-rw-   0        0        0     1480 2024-05-24 14:33:48.000000 RsCMPX_Gprf-5.0.92/setup.py
```

### Comparing `RsCMPX_Gprf-5.0.91/PKG-INFO` & `RsCMPX_Gprf-5.0.92/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RsCMPX_Gprf
-Version: 5.0.91
+Version: 5.0.92
 Summary: CMX/CMP/PVT Global Purpose RF Remote-control module
 Home-page: UNKNOWN
 Author: Rohde & Schwarz GmbH & Co. KG
 License: MIT
 Description: ==================================
          RsCMPX_Gprf
         ==================================
@@ -44,15 +44,19 @@
         
         Examples: https://github.com/Rohde-Schwarz/Examples/
         
         
         Version history
         ----------------
         
-        	Latest release notes summary: Added missing measurement SCPI from MMI sub-system
+        	Latest release notes summary: New Core 1.80.0 with loosened data type assertions for lists
+        
+        	Version 5.0.92
+        		- New Core 1.80.0 with loosened data type assertions for lists
+        		- Corrected parameter for TRIGger:GPRF:GENerator<i>:SEQuencer:ISMeas:SOURce to scalar string
         
         	Version 5.0.91
         		- Added missing measurement SCPI from MMI sub-system
         
         	Version 5.0.90
         		- Update for CMP FW 5.0.90
```

### Comparing `RsCMPX_Gprf-5.0.91/README.rst` & `RsCMPX_Gprf-5.0.92/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -37,15 +37,19 @@
 
 Examples: https://github.com/Rohde-Schwarz/Examples/
 
 
 Version history
 ----------------
 
-	Latest release notes summary: Added missing measurement SCPI from MMI sub-system
+	Latest release notes summary: New Core 1.80.0 with loosened data type assertions for lists
+
+	Version 5.0.92
+		- New Core 1.80.0 with loosened data type assertions for lists
+		- Corrected parameter for TRIGger:GPRF:GENerator<i>:SEQuencer:ISMeas:SOURce to scalar string
 
 	Version 5.0.91
 		- Added missing measurement SCPI from MMI sub-system
 
 	Version 5.0.90
 		- Update for CMP FW 5.0.90
```

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/CustomFiles/events.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/CustomFiles/events.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/CustomFiles/reliability.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/CustomFiles/reliability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/CustomFiles/utilities.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/CustomFiles/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Utilities extending the driver for methods provided with RsInstrument."""
 
 from typing import List, Tuple
 import threading
 
 from ..Internal import Core
+from ..Internal.ContextManagers import InstrErrorSuppressor, VisaTimeoutSuppressor
 from ..Internal import Conversions as Conv
 from ..Internal.ScpiLogger import ScpiLogger
 
 
 class Utilities:
 	"""Common utility class.
 	Utility functions common for all types of drivers. \n
@@ -340,14 +341,42 @@
 		return self._core.io.query_bin_block(query)
 
 	def query_bin_block_with_opc(self, query: str, timeout: int = None) -> bytes:
 		"""Sends a OPC-synced query and returns binary data block to bytes.
 		If you do not provide timeout, the method uses current opc_timeout."""
 		return self._core.io.query_bin_block_with_opc(query, timeout)
 
+	def query_str_list(self, query: str, remove_blank_response: bool = False) -> List[str]:
+		"""Sends the string query to the instrument and returns the response as List of strings, where the delimiter is comma (',').
+		Each element of the list is trimmed for leading and trailing quotes.
+		Meaning of the 'remove_blank_response':
+			- False(default): whitespaces-only response is returned as a list with one empty element [''].
+			- True: whitespaces-only response is returned as an empty list []."""
+		return self._core.io.query_str_list(query, remove_blank_response)
+
+	def query_str_list_with_opc(self, query: str, timeout: int = None, remove_blank_response: bool = False) -> List[str]:
+		"""Sends a OPC-synced query and reads response from the instrument as csv-list.
+		If you do not provide timeout, the method uses current opc_timeout.
+		Meaning of the 'remove_blank_response':
+			- False(default): whitespaces-only response is returned as a list with one empty element [''].
+			- True: whitespaces-only response is returned as an empty list []."""
+		return self._core.io.query_str_list_with_opc(query, timeout, remove_blank_response)
+
+	def query_bool_list(self, query: str) -> List[bool]:
+		"""Sends the string query to the instrument and returns the response as List of booleans,
+		where the delimiter is comma (',').
+		Blank or empty response is returned as an empty list."""
+		return self._core.io.query_bool_list(query)
+
+	def query_bool_list_with_opc(self, query: str, timeout: int = None) -> List[bool]:
+		"""Sends a OPC-synced query and reads response from the instrument as csv-list of booleans.
+		If you do not provide timeout, the method uses current opc_timeout.
+		Blank or empty response is returned as an empty list."""
+		return self._core.io.query_bool_list_with_opc(query, timeout)
+
 	def query_bin_or_ascii_float_list(self, query: str) -> List[float]:
 		"""Queries a list of floating-point numbers that can be returned in ASCII format or in binary format.
 		- For ASCII format, the list numbers are decoded as comma-separated values.
 		- For Binary Format, the numbers are decoded based on the property BinFloatFormat, usually float 32-bit (FORM REAL,32)."""
 		return self._core.io.query_bin_or_ascii_float_list(query)
 
 	def query_bin_or_ascii_float_list_with_opc(self, query: str, timeout: int = None) -> List[float]:
@@ -434,14 +463,31 @@
 		"""Assigns the provided thread lock."""
 		self._core.io.assign_lock(lock)
 
 	def clear_lock(self):
 		"""Clears the existing thread lock, making the current session thread-independent from others that might share the current thread lock."""
 		self._core.io.clear_lock()
 
+	def instr_err_suppressor(self, visa_tout_ms: int = 0, suppress_only_codes: int or List[int] = None) -> InstrErrorSuppressor:
+		"""Returns Context Manager that suppresses the instrument errors.
+		Other exceptions types are still raised.
+		On entering the context, this class clears all the instrument status errors.
+		:param visa_tout_ms: VISA Timeout in milliseconds, that is set for this context. Afterward, it is changed back. Default value: do-not-change.
+		:param suppress_only_codes: You can enter a code or list of codes for errors to be suppressed. Other errors will be reported. Example: If you enter -113 here, only the 'Undefined Header' error will be suppressed. Default value: suppress-all-errors."""
+		return InstrErrorSuppressor(self._core.io, visa_tout_ms, suppress_only_codes)
+
+	def visa_tout_suppressor(self, visa_tout_ms: int = 0) -> VisaTimeoutSuppressor:
+		"""Returns Context Manager that suppresses the VISA timeout error.
+		Careful!!!: Only the very first VISA Timeout exception is suppressed,
+		and afterward the context ends. Therefore, use only one command per context manager,
+		if you do not want to skip the following ones.
+		:param visa_tout_ms: VISA Timeout in milliseconds, that is set for this context. Afterward, it is changed back. Default value: do-not-change.
+		"""
+		return VisaTimeoutSuppressor(self._core.io, visa_tout_ms)
+
 	def sync_from(self, source: 'Utilities') -> None:
 		"""Synchronises these Utils with the source."""
 		self.logger.sync_from(source.logger)
 		self.assign_lock(source.get_lock())
 		self.bin_float_numbers_format = source.bin_float_numbers_format
 		self.bin_int_numbers_format = source.bin_int_numbers_format
 		self.data_chunk_size = source.data_chunk_size
```

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/Globale.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/Globale.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/Tenvironment.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/Tenvironment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/Attenuation/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/System/Attenuation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/System/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/Rx.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/Rx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/Tx.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/Tx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/Tenvironment/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Add/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/ExtPwrSensor/Zero.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/ExtPwrSensor/Zero.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/ExtPwrSensor/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/ExtPwrSensor/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Calibration/Gprf/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Calibration/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Cdma/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Cdma/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/Group.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/Group.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/Ploss.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/Ploss.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gprf/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gsm/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Gsm/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Lte/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Lte/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Lte/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Lte/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Lte/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Lte/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/LteDl/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/LteDl/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/LteDl/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/LteDl/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/LteDl/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/LteDl/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Niot/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Niot/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Niot/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Niot/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Niot/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Niot/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrDl/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrDl/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrDl/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrDl/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrDl/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrDl/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrMmw/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrMmw/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrMmw/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrMmw/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrMmw/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrMmw/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrSub/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrSub/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrSub/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrSub/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrSub/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/NrSub/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Attenuation/CorrectionTable.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/System/Attenuation/CorrectionTable.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Attenuation/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/System/Attenuation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Reset.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/System/Reset.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Rf42/Box.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/System/Rf42/Box.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Rf42/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/System/Rf42/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Rrhead.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/System/Rrhead.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/System/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Tenvironment/Connectors.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Tenvironment/Connectors.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Tenvironment/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Tenvironment/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Uwb/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Uwb/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Uwb/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Uwb/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Uwb/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Uwb/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wcdma/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wcdma/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wcdma/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wcdma/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wcdma/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wcdma/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wlan/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wlan/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wlan/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wlan/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wlan/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wlan/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wpan/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wpan/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wpan/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wpan/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wpan/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/Wpan/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/Tx/Single.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/Tx/Single.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/Tx/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/Tx/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/IqFile.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/IqFile.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/Sall.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/Sall.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Correction.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Correction.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Attenuation.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Attenuation.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Auto.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Auto.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Average.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/PeakSearch.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/PeakSearch.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/Capture.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/Capture.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/Bandpass.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/Bandpass.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/Gauss.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/Gauss.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/IqSettings.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/IqSettings.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/EnvelopePower.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/EnvelopePower.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/Frequency.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/Sstop.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/Sstop.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/Trigger.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/Trigger.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/EnvelopePower.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/EnvelopePower.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Frequency.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Retrigger.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Retrigger.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Sstop.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Sstop.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/Trigger.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/Trigger.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/Frequency.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/ListPy/Frequency.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/ListPy/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/ListPy/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/ListPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/File.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/File.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/View.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/View.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/Bandpass.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/Bandpass.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/Gauss.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/Gauss.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Cidx.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Cidx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/EnvelopePower.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/EnvelopePower.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Frequency.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/Catalog/Connection.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/Catalog/Connection.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/Catalog/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/Catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/Connection.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/Connection.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/IqData.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/IqData.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Irepetition.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Irepetition.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/ParameterSetList.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/ParameterSetList.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Retrigger.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Retrigger.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Sstop.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Sstop.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandpass/Bandwidth.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandpass/Bandwidth.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandpass/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandpass/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandwidth.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandwidth.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Gauss/Bandwidth.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Gauss/Bandwidth.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Gauss/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Gauss/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/TypePy.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/TypePy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Mlength.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Mlength.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/PdefSet.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/PdefSet.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Slength.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Slength.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/Trigger.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/Trigger.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/RfSettings/LrStart.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/RfSettings/LrStart.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/RfSettings/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/RfSettings/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Scenario.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Scenario.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Rbw.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Rbw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Swt.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Swt.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Vbw.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Vbw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/Frequency/Span.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/Frequency/Span.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/Frequency/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/Frequency/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/Rbw.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/Rbw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/Vbw.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/Vbw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Gprf/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/Globale.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/Globale.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/Tenvironment.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/Tenvironment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Control/Reboot.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Control/Reboot.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Control/Restart.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Control/Restart.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Control/Shutdown.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Control/Shutdown.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Control/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Control/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Edevice.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Edevice.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/HwProperties.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Positioner/HwProperties.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Move/To.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Move/To.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Move/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Move/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Moving.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Moving.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Versions.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Versions.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Positioner/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Recall/Partial.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Recall/Partial.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Recall/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Recall/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Reset.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Reset.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/Rx.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/Rx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/Tx.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/Tx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rf42/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/Rx.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/Rx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/Tx.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/Tx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Save/Partial.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Save/Partial.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Save/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Save/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Vse.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Vse.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Z310/Attenuation.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Z310/Attenuation.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Z310/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Z310/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Z320/Attenuation.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Z320/Attenuation.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Z320/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/Z320/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/System/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/Rx.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/Rx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/Tx.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/Tx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/Rx.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/Rx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/Tx.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/Tx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Direction.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Direction.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Info.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Info.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/Tenvironment/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Configure/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/Globale.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/Globale.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/Tenvironment.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/Tenvironment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/Attenuation/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Create/System/Attenuation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Create/System/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/Tenvironment/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Create/Tenvironment/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/Tenvironment/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Create/Tenvironment/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Create/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/Connectors.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/Connectors.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/Gprf/Measurement.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/Gprf/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/Gprf/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/Gprf/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/FilterPy.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/FilterPy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Rpc/FilterPy.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Rpc/FilterPy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Rpc/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Psub/FilterPy.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Psub/FilterPy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Psub/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Psub/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Rpc/FilterPy.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Rpc/FilterPy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Rpc/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Scpi/Logging.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Scpi/Logging.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Scpi/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Scpi/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Configure/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/Power/State.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/Power/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/Power/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/Power/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Generic/Measurement/Dapi.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Generic/Measurement/Dapi.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Generic/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Generic/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Generic/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Generic/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Correction.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Correction.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfProperty.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfProperty.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfSettings.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfSettings.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfSetttings.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfSetttings.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Rms.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Rms.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Snumber.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Snumber.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Ploss/Rnames.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Ploss/Rnames.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Ploss/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Ploss/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Bandpass/Bandwidth.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Bandpass/Bandwidth.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Bandpass/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Bandpass/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Franges.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Franges.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Frequency.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Fspan.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Fspan.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Gauss/Bandwidth.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Gauss/Bandwidth.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Gauss/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Gauss/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Bandpass/Bandwidth.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Bandpass/Bandwidth.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Bandpass/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Bandpass/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Gauss/Bandwidth.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Gauss/Bandwidth.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Gauss/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Gauss/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Samples.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Samples.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/ListPy/Iranges.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/ListPy/Iranges.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/ListPy/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/ListPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/LoFrequency.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/LoFrequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/NbLevel.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/NbLevel.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/SymbolRate.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/SymbolRate.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Snumber.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Snumber.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Meas/Scpi.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Meas/Scpi.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Meas/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Meas/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/Generator.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/Generator.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/Measurement.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/NrMmw/Measurement.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Route/NrMmw/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/NrMmw/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Route/NrMmw/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Uwb/Measurement.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Route/Uwb/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Uwb/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Route/Uwb/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Route/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/Debug/Output.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/Debug/Output.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/Debug/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/Debug/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Diagnostic/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/State/All.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/State/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/State/All.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/State/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Icomponent.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Icomponent.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/Average.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/Current.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Average.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Current.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Maximum.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Minimum.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Qcomponent.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Qcomponent.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/State/All.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/State/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Bin.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Bin.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Reliability.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Reliability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/State/All.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/State/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/SymbolRate.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/SymbolRate.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Talignment.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Talignment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/FreqError.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/FreqError.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Icomponent.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Icomponent.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Level.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Level.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/OfError.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/OfError.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Phase.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Phase.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Qcomponent.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Qcomponent.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/State/All.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/State/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/Sensor/Power.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/Sensor/Power.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/Sensor/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/Sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/State/All.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/State/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Clear.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Clear.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Eoo.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Eoo.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Ezo.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Ezo.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Ezz.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Ezz.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Frequency.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Frequency.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Gain.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Gain.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/State.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Trace/Frequency.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Trace/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Trace/Gain.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Trace/Gain.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Trace/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Trace/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Match/State.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Match/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Match/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Match/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Open/State.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Open/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Open/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Open/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Short/State.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Short/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Short/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Short/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/All.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/AmplitudeProbDensity.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/AmplitudeProbDensity.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Average/Rms.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Average/Rms.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Average/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Average/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Power.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Power.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Probability.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Probability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Sample.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Sample.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Maximum.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Minimum.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Rms.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Rms.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ElapsedStats.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ElapsedStats.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqData/Bin.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqData/Bin.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqData/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqData/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqInfo.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqInfo.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Average.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Current.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Maximum/Current.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Maximum/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Maximum/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Maximum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Minimum/Current.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Minimum/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Minimum/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Minimum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/Maximum.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/Minimum.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/StandardDev.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/Current.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/Maximum.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/Current.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/Minimum.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/Maximum.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/Minimum.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/StandardDev/Current.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/StandardDev/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/StandardDev/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/StandardDev/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/State/All.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/State/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Average.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Current.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Maximum.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Minimum.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Marker/Npeak.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Marker/Npeak.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Marker/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Marker/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Average.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Current.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Maximum.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Minimum.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Average.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Current.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Maximum.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Minimum.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/Npeak.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/Npeak.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/Speak.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/Speak.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Average.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Current.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Maximum.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Minimum.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Average.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Current.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Maximum.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Minimum.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/State/All.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/State/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Gprf/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/Globale.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/Globale.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/Tenvironment.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/Tenvironment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Modify/System/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Modify/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/Globale.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/Globale.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/Tenvironment.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/Tenvironment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/System/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/Rx.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/Rx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/Tx.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/Tx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/Tenvironment/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Remove/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/Power/Current.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/Power/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/Power/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/Power/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Results/Gprf/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Results/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Bluetooth/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Bluetooth/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Bluetooth/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Bluetooth/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Bluetooth/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Bluetooth/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Cdma/Measurement.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Cdma/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Cdma/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Cdma/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/RfSettings.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/RfSettings.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/Spath/Group.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/Spath/Group.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/Spath/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/Spath/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/RfSettings.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/RfSettings.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Scenario/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Scenario/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Scenario/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Scenario/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gprf/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gsm/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gsm/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gsm/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gsm/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gsm/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Gsm/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Lte/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Lte/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Lte/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Lte/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Lte/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Lte/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/LteDl/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/LteDl/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/LteDl/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/LteDl/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/LteDl/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/LteDl/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Niot/Measurement.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Niot/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Niot/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Niot/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrDl/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrDl/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrDl/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrDl/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrDl/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrDl/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrMmw/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrMmw/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrMmw/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrMmw/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrMmw/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrMmw/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrSub/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrSub/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrSub/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrSub/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrSub/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/NrSub/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Uwb/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Uwb/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Uwb/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Uwb/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Uwb/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Uwb/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wcdma/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wcdma/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wcdma/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wcdma/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wcdma/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wcdma/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wlan/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wlan/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wlan/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wlan/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wlan/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wlan/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wpan/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/Wpan/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Route/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/Ambient.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/Ambient.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/Base/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/System/Positioner/IsMoving.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/System/Positioner/IsMoving.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/System/Positioner/Position.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/System/Positioner/Position.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/System/Positioner/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/System/Positioner/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/System/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/System/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Sense/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/File.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/File.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Marker/Delays.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Marker/Delays.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Marker/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Marker/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Msegment.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Msegment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Samples/Range.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Samples/Range.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Samples/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Samples/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Segments.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Segments.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/UdMarker/Clist.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/UdMarker/Clist.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/UdMarker/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/UdMarker/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/Level.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/Level.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/Ofrequency.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/Ofrequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/IqSettings.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/IqSettings.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Dgain.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Dgain.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Dtime.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Dtime.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Esingle.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Esingle.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Fill.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Fill.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Frequency.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Increment/Enabling.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Increment/Enabling.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Increment/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Increment/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Irepetition.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Irepetition.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Modulation.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Modulation.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Reenabling.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Reenabling.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/RfLevel.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/RfLevel.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Rlist.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Rlist.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Slist.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Slist.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Sstop.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Sstop.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Reliability.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Reliability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/RfSettings.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/RfSettings.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Check.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Check.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/CrcProtect.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/CrcProtect.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Download.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Download.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Duration.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Duration.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Paratio.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Paratio.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Path.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Path.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Poffset.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Poffset.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Reliability.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Reliability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Rmessage.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Rmessage.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Roption.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Roption.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Samples.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Samples.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/SymbolRate.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/SymbolRate.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Waveform.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Waveform.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Dtone/Ofrequency.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Dtone/Ofrequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Dtone/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Dtone/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Acycles.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Acycles.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Dgain.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Dgain.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Dtime.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Dtime.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Call.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Call.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Insert.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Insert.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Mdown.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Mdown.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Mup.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Mup.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Apply.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Apply.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Dgain.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Dgain.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Frequency.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Lrms.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Lrms.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Frequency.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Itransition.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Itransition.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Lincrement.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Lincrement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Lrms.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Lrms.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Cw.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Cw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Dtone.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Dtone.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Off.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Off.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Index/All.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Index/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Index/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Index/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Range.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Range.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/Tx/Single.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/Tx/Single.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/Tx/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/Tx/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/SymbolRate.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/SymbolRate.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Ttime.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Ttime.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/Delays/All.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/Delays/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/Delays/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/Delays/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Reliability.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Reliability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/RfSettings/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/RfSettings/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/RfSettings/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/RfSettings/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Rmarker.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Rmarker.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/State/All.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/State/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Tdd.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Tdd.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/Delay/All.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/Delay/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/Delay/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/Delay/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/State/All.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/State/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/Gprf/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Source/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/Globale.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/Globale.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/Tenvironment.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/Tenvironment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/Globale.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/Globale.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/Tenvironment.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/Tenvironment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Attenuation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Date/Local.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Date/Local.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Date/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Date/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Time/Local.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Time/Local.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Time/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/Time/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/System/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Tenvironment/Spath.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Tenvironment/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Tenvironment/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Tenvironment/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/BhRate/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/BhRate/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/BhRate/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/BhRate/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdr/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdr/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdr/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdr/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdrp/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdrp/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdrp/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdrp/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Cdma/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/Execute.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/Execute.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/Execute.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/Execute.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/IsMeas.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/IsMeas.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List
 
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
+from ......Internal.Utilities import trim_str_response
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class IsMeasCls:
 	"""IsMeas commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
@@ -18,26 +19,26 @@
 		Snippet: value: List[str] = driver.trigger.gprf.generator.sequencer.isMeas.get_catalog() \n
 		Queries all available measurement source strings. \n
 			:return: trigger: Comma-separated list of strings. Each string represents a supported source.
 		"""
 		response = self._core.io.query_str('TRIGger:GPRF:GENerator<Instance>:SEQuencer:ISMeas:CATalog?')
 		return Conversions.str_to_str_list(response)
 
-	def get_source(self) -> List[str]:
+	def get_source(self) -> str:
 		"""SCPI: TRIGger:GPRF:GENerator<Instance>:SEQuencer:ISMeas:SOURce \n
-		Snippet: value: List[str] = driver.trigger.gprf.generator.sequencer.isMeas.get_source() \n
+		Snippet: value: str = driver.trigger.gprf.generator.sequencer.isMeas.get_source() \n
 		Selects a measurement for triggering sequencer list incrementations. A complete list of all supported strings can be
 		queried using method RsCMPX_Gprf.Trigger.Gprf.Generator.Sequencer.IsMeas.catalog. \n
 			:return: trigger: No help available
 		"""
 		response = self._core.io.query_str('TRIGger:GPRF:GENerator<Instance>:SEQuencer:ISMeas:SOURce?')
-		return Conversions.str_to_str_list(response)
+		return trim_str_response(response)
 
-	def set_source(self, trigger: List[str]) -> None:
+	def set_source(self, trigger: str) -> None:
 		"""SCPI: TRIGger:GPRF:GENerator<Instance>:SEQuencer:ISMeas:SOURce \n
-		Snippet: driver.trigger.gprf.generator.sequencer.isMeas.set_source(trigger = ['abc1', 'abc2', 'abc3']) \n
+		Snippet: driver.trigger.gprf.generator.sequencer.isMeas.set_source(trigger = 'abc') \n
 		Selects a measurement for triggering sequencer list incrementations. A complete list of all supported strings can be
 		queried using method RsCMPX_Gprf.Trigger.Gprf.Generator.Sequencer.IsMeas.catalog. \n
 			:param trigger: No help available
 		"""
-		param = Conversions.list_to_csv_quoted_str(trigger)
+		param = Conversions.value_to_quoted_str(trigger)
 		self._core.io.write(f'TRIGger:GPRF:GENerator<Instance>:SEQuencer:ISMeas:SOURce {param}')
```

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/IsTrigger.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/IsTrigger.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/Execute.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/Execute.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/OsStop.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/OsStop.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqRecorder/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqRecorder/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqRecorder/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqRecorder/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqVsSlot/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqVsSlot/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqVsSlot/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqVsSlot/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/Offset.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/Offset.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Spectrum.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Spectrum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gprf/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Gsm/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Prach/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Prach/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Prach/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Prach/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Srs/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Srs/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Srs/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Srs/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Lte/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/LteDl/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/Prach/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/Prach/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/Prach/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/Prach/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Niot/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrDl/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/Prach/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/Prach/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/Prach/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/Prach/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrMmw/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Prach/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Prach/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Prach/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Prach/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Srs/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Srs/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Srs/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Srs/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/NrSub/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Uwb/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OlpControl/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OlpControl/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OlpControl/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OlpControl/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OoSync/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OoSync/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OoSync/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OoSync/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Prach/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Prach/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Prach/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Prach/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Tpc/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Tpc/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Tpc/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wcdma/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wlan/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/Wpan/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/__init__.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Implementations/Trigger/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgLinkedEventArgs.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ArgLinkedEventArgs.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgSingle.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ArgSingle.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgSingleList.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ArgSingleList.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgSingleSuppressed.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ArgSingleSuppressed.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgStringComposer.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ArgStringComposer.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgStruct.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ArgStruct.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgStructList.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ArgStructList.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgStructStringParser.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ArgStructStringParser.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/CommandsGroup.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/CommandsGroup.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/Conversions.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/Conversions.py`

 * *Files 6% similar despite different names*

```diff
@@ -369,41 +369,49 @@
 	"""Returns string enclosed by single quotes."""
 	assert_string_data(string)
 	return Properties.scpi_quotes + string + Properties.scpi_quotes
 
 
 def list_to_csv_str(value: List, delimiter: str = ',') -> str:
 	"""Converts list of elements to strings separated by commas.
+	The method also tolerates a scalar value, and handles it as list of one element.
 	Element types can differ on an individual basis.
 	Supported element types:
 	- int
 	- bool
 	- float
 	- string -> string no quotes
 	- enum"""
+	if isinstance(value, int) or isinstance(value, bool) or isinstance(value, float) or isinstance(value, str) or isinstance(value, Enum):
+		value = [value]
+
 	assert_list_data(value)
 	result = []
 	for x in value:
 		el = value_to_str(x)
 		if not el:
 			raise TypeError(f"List element type is not supported by Conversions.list_to_csv_str: '{x}'")
 		result.append(el)
 	return delimiter.join(result)
 
 
 def list_to_csv_quoted_str(value: List) -> str:
 	"""Converts list of elements to quoted strings separated by commas.
+	The method also tolerates a scalar value, and handles it as list of one element.
 	Only string elements are enclosed by single quotes
 	Element types can differ on an individual basis.
 	Supported element types:
 	- int
 	- bool
 	- float
 	- string -> string enclosed by quotes
 	- enum"""
+	if isinstance(value, int) or isinstance(value, bool) or isinstance(value, float) or isinstance(value, str) or isinstance(value, Enum):
+		value = [value]
+
 	assert_list_data(value)
 	result = []
 	for x in value:
 		if isinstance(x, str):
 			el = str_enclose_by_quotes(x)
 		else:
 			el = value_to_str(x)
@@ -486,67 +494,84 @@
 	- float
 	- string
 	- enum"""
 	return Properties.scpi_quotes + value_to_str(x) + Properties.scpi_quotes
 
 
 def str_to_float_list(string: str) -> List[float]:
-	"""Converts string with comma-separated values to list of Floats."""
+	"""Converts string with comma-separated values to list of floats.
+	Empty or blank string is converted to empty list."""
 	assert_string_data(string)
 	if not string:
 		return []
+	if string.isspace():
+		return []
 	result = [*map(str_to_float, string.split(','))]
 	return result
 
 
 def str_to_float_or_bool_list(string: str) -> List[float or bool]:
-	"""Converts string with comma-separated values to list of float or boolean values."""
+	"""Converts string with comma-separated values to list of float or boolean values.
+	Empty or blank string is converted to empty list."""
 	assert_string_data(string)
 	if not string:
 		return []
+	if string.isspace():
+		return []
 	result = [*map(str_to_float_or_bool, string.split(','))]
 	return result
 
 
 def str_to_int_list(string: str) -> List[int]:
-	"""Converts string with comma-separated values to list of Integers."""
+	"""Converts string with comma-separated values to list of integers.
+	Empty or blank string is converted to empty list."""
 	assert_string_data(string)
 	if not string:
 		return []
+	if string.isspace():
+		return []
 	result = [*map(str_to_int, string.split(','))]
 	return result
 
 
 def str_to_int_or_bool_list(string: str) -> List[int or bool]:
-	"""Converts string with comma-separated values to list of integer or boolean values."""
+	"""Converts string with comma-separated values to list of integer or boolean values.
+	Empty or blank string is converted to empty list."""
 	assert_string_data(string)
 	if not string:
 		return []
+	if string.isspace():
+		return []
 	result = [*map(str_to_int_or_bool, string.split(','))]
 	return result
 
 
 def str_to_bool_list(string: str) -> List[bool]:
-	"""Converts string with comma-separated values to list of booleans."""
+	"""Converts string with comma-separated values to list of booleans.
+	Empty or blank string is converted to empty list."""
 	assert_string_data(string)
 	if not string:
 		return []
+	if string.isspace():
+		return []
 	result = [*map(str_to_bool, string.split(','))]
 	return result
 
 
-def str_to_str_list(string: str, clear_one_empty_item: bool = False) -> List[str]:
+def str_to_str_list(string: str, remove_blank_response: bool = False) -> List[str]:
 	"""Converts string with comma-separated values to list of strings.
 	Each element is trimmed by trim_str_response().
-	If the clear_one_empty_item is set to True (default is False), and the result is exactly one empty string item, the method returns empty list."""
+	Meaning of the 'remove_empty_response':
+		- False(default): empty response is returned as a list with one empty element [''].
+		- True: empty response is returned as an empty list []."""
 	assert_string_data(string)
 	if not string:
 		return []
 	result = [*map(Utilities.trim_str_response, string.split(','))]
-	if clear_one_empty_item and len(result) == 1 and result[0] == '':
+	if remove_blank_response and len(result) == 1 and result[0] == '':
 		return []
 	return result
 
 
 def str_to_scalar_enum_helper(string: str, scpi_enum: ScpiEnum, array_search: bool, exc_if_not_found) -> Enum:
 	"""Converts string to one enum element.
 	array_search signal no need to force the comma removing,
@@ -592,15 +617,19 @@
 		value = value.replace('_', '')
 	if value in enum_members_mod:
 		return enum_type[enum_members[enum_members_mod.index(value)]]
 	return None
 
 
 def str_to_list_enum_helper(string: str, scpi_enum: ScpiEnum, exc_if_not_found: bool = True) -> List[Enum]:
-	"""Converts string to list of enum elements. separated by comma"""
+	"""Converts string to list of enum elements. separated by comma."""
+	if not string:
+		return []
+	if string.isspace():
+		return []
 	elements = string.split(',')
 	return [str_to_scalar_enum_helper(x, scpi_enum, True, exc_if_not_found) for x in elements]
 
 
 def enum_scalar_to_str(data, enum_type) -> str:
 	"""Converts enum scalar value to string."""
 	assert isinstance(data, enum_type), f"Expected command parameter {enum_type}, actual data type: {type(data)}. Value: {data}"
@@ -614,22 +643,28 @@
 		# Return string with quotes
 		return value_to_quoted_str(Utilities.trim_str_response(data))
 	assert isinstance(data, enum_type), f"Expected command parameter string or {enum_type}, actual data type: {type(data)}. Value: {data}"
 	return value_to_str(data)
 
 
 def enum_list_to_str(data: List, enum_type) -> str:
-	"""Converts enum list to csv-string."""
+	"""Converts enum list to csv-string.
+	The method also tolerates a scalar value, and handles it as list of one element."""
+	if isinstance(data, enum_type):
+		data = [data]
 	# For enums, check that each element is an enum
 	assert all(isinstance(x, enum_type) for x in data), f"Expected command parameter list of {enum_type}, detected one or more elements of non-enum type. Value: {data}"
 	return list_to_csv_str(data)
 
 
 def enum_ext_list_to_str(data: List, enum_type) -> str:
-	"""Converts enum list to csv-string. Allows the elements to be either enum or string."""
+	"""Converts enum list to csv-string. Allows the elements to be either enum or string.
+	The method also tolerates a scalar value, and handles it as list of one element."""
+	if isinstance(data, enum_type or str) or isinstance(data, str):
+		data = [data]
 	assert all((isinstance(x, enum_type or str) or isinstance(x, str)) for x in data), f"Expected command parameter list of strings or {enum_type}, detected one or more elements of non-enum/non-string type. Value: {data}"
 	return list_to_csv_quoted_str(data)
 
 
 def str_to_scalar_enum(string: str, enum_type) -> Enum:
 	"""Converts string to one enum element.
 	Throws exception if the string can not be converted to an enum element or a special value."""
```

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ConverterFromScpiString.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ConverterFromScpiString.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ConverterToScpiString.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ConverterToScpiString.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/Core.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/Core.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,168 +18,193 @@
 		- Main core constructor
 		- 'io' interface for all the write / query operations
 		- Command parameters string composer for single arguments...
 		- Link handlers adding / changing / deleting
 
 		Version history:
 
+		1.80.0 (17.05.2024)
+			- Loosened checking of list parameters - all the List params can also be scalar values.
+
+		1.71.0 (25.04.2024)
+			- To all query_str_list_xxx() methods, added non-mandatory parameter 'remove_blank_response'
+			- Added Context Managers for ignoring errors and ignoring VISA Timeouts.
+			- Logger: added new variable to the format string: %SCPI_COMMAND%, where you can only log SCPI commands to your log data.
+			- Added to Utilities interface: query_str_list(), query_str_list_with_opc(), query_bool_list(), query_bool_list_with_opc()
+			- Added Utility functions: value_to_si_string(), size_to_kb_mb_gb_string().
+			- Changed behaviour of the Conversion functions to list:
+				- str_to_float_list()
+				- str_to_float_or_bool_list()
+				- str_to_int_list()
+				- str_to_int_or_bool_list()
+				- str_to_bool_list()
+				These functions previously returned a list of one element if the input value was whitespace-only string.
+				Now, in such case they return empty list.
+
 		1.70.0 (27.02.2024)
 			- Added settings profile 'XK41' for R&S Software Defined Radios.
 			- Added settings 'FirstCmds' where you can send the defined commands right after the init. Send more commands in a row with ';;' separator.
 			- Added settings 'EachCmdPrefix' - this prefix is added to each command sent to the instrument. Supported values are also 'lf', 'cr', 'tab'
 
 		1.60.0 (31.01.2024)
 			- Added Properties script for global properties.
 			- Added Properties.scpi_quotes, string option settings token: 'ScpiQuotes'. Example: ScpiQuotes=double. Default: Single
 			- Fixed VisaPluginSocketIo read() method for cases where the session is lost. The method now generates exception in that case.
-			- Added settings 'OpcSyncQueryMechanism' with values: Standard, AlsoCheckMav, ClsOnlyCheckMavErrQueue, OnlyCheckMavErrQueue
+			- Added settings 'OpcSyncQueryMechanism' with values: Standard, AlsoCheckMav, ClsOnlyCheckMavErrQueue, OnlyCheckMavErrQueue.
 
 		1.54.0 (27.06.2023)
 			- Added new options profile for ATS chambers.
-			- Added settings boolean token EachCmdAsQuery. Example: EachCmdAsQuery=True. Default: False
+			- Added settings boolean token EachCmdAsQuery. Example: EachCmdAsQuery=True. Default: False.
 
 		1.53.0 (18.10.2022)
 			- Improved mode where the instrument works with a session from another object.
 			- Silently ignoring invalid *IDN? string.
 			- Added new options profile 'Minimal' for non-SCPI-99 instruments.
 
 		1.52.0 (28.09.2022)
 			- Fixed DisableOpcQuery=True settings effect.
 			- Improved robustness of the TerminationCharacter option value entry.
 			- Added new options profile for CMQ500.
 
 		1.51.0 (08.09.2022)
 			- Changed the accepted IDN? response to more permissive.
-			- added methods go_to_remote() and go_to_local()
-			- added methods file_exists() and get_file_size()
+			- added methods go_to_remote() and go_to_local().
+			- added methods file_exists() and get_file_size().
 
 		1.50.0 (23.06.2022)
 			- Added relative timestamp to the logger.
 			- ScpiLogger can read GlobalData class variables making it possible to define common target and reference timestamp for all instances.
 			- Logger stream entries are by default immediately flushed, making sure that the log is complete.
 			- Added time statistic methods get_total_execution_time(), get_total_time(), reset_time_statistics().
 
 		1.24.0 (03.06.2022)
 			- Changed parsing of SYST:ERR? response to tolerate +0,"No Error" response.
-			- Added settings integer token OpenTimeout. Example: OpenTimeout=5000. Default: 0
-			- Added settings boolean token ExclusiveLock. Example: ExclusiveLock=True. Default: False
+			- Added settings integer token OpenTimeout. Example: OpenTimeout=5000. Default: 0.
+			- Added settings boolean token ExclusiveLock. Example: ExclusiveLock=True. Default: False.
 
 		1.23.0 (24.05.2022)
 			- Added stripping of trailing commas when parsing the *IDN? response.
-			- If the Resource Manager does not find any default VISA implementation, it falls back to R&S VISA - relevant for LINUX or macOS
+			- If the Resource Manager does not find any default VISA implementation, it falls back to R&S VISA - relevant for LINUX or macOS.
 			- Other typos and formatting corrections.
 
 		1.22.0 (20.04.2022)
-			- Added optional parameter timeout to reset()
-			- Added query list methods:  query_bool_list, query_bool_list_with_opc
+			- Added optional parameter timeout to reset().
+			- Added query list methods:  query_bool_list, query_bool_list_with_opc.
 
 		1.21.0 (07.01.2022)
-			- Added logging to UDP port (49200) to integrate with new R&S Instrument Control plugin for Pycharm
+			- Added logging to UDP port (49200) to integrate with new R&S Instrument Control plugin for Pycharm.
 
 		1.20.0 (19.11.2021)
-			- Fixed logging strings when device name was a substring of the resource name
+			- Fixed logging strings when device name was a substring of the resource name.
 
 		1.18.0 (build 64) 05.11.2021
-			- Added setting profile for non-standard instruments. Example of the options string: options='Profile=hm8123'
+			- Added setting profile for non-standard instruments. Example of the options string: options='Profile=hm8123'.
 
 		1.17.0 (build 63) 15.10.2021
-			- Added correct conversion of strings with SI suffixes (e.g.: MHz, KHz, THz, GHz, ms, us) to float and integer
+			- Added correct conversion of strings with SI suffixes (e.g.: MHz, KHz, THz, GHz, ms, us) to float and integer.
 
 		1.16.0 (build 62) 31.08.2021
 			- Changed default encoding of string<=>bin from utf-8 to charmap.
 			- Added settable encoding for the session. Property: RsInstrument.encoding
 
 		1.15.0 (build 61) 17.08.2021
-			- Added support for EnumExt and EnumExtList
-			- Added support for custom scpi enums
+			- Added support for EnumExt and EnumExtList.
+			- Added support for custom scpi enums.
 			- Improved exception handling in cases where the instrument session is closed.
-			- Fixed warning in Instrument.py
-			- Fixed Instrument.query_bin_block() for timeout errors
-			- Repeated capabilities are now allowed to be integer numbers as well
+			- Fixed warning in Instrument.py.
+			- Fixed Instrument.query_bin_block() for timeout errors.
+			- Repeated capabilities are now allowed to be integer numbers as well.
 
 		1.14.0 (build 53) 12.07.2021
-			- Scpi logger time entries now support not only datetime tuples, but also float timestamps
-			- changed handling of the syst:err? responses - now they are always Tuple (code, message)
-			- StatusException has new field errors_list: List[ Tuple[code, message] ]
-			- Added logger.log_status_check_ok property. This allows for skipping lines with 'Status check: OK'
+			- Scpi logger time entries now support not only datetime tuples, but also float timestamps.
+			- Changed handling of the syst:err? responses - now they are always Tuple (code, message).
+			- StatusException has new field errors_list: List[ Tuple[code, message] ].
+			- Added logger.log_status_check_ok property. This allows for skipping lines with 'Status check: OK'.
 
 		1.12.0 (build 50) 26.06.2021
-			- Added SCPI Logger
+			- Added SCPI Logger.
 			- Simplified constructor's options string format - removed DriverSetup=() syntax:
-			Instead of "DriverSetup=(TerminationCharacter='\n')", you use "TerminationCharacter='\n'"
+			Instead of "DriverSetup=(TerminationCharacter='\n')", you use "TerminationCharacter='\n'".
 			The original format is still supported.
 
-			- Fixed calling SYST:ERR? even if *STB? returned 0
-			- Replaced @ni backend with @ivi for resource manager - this is necessary for the future pyvisa version 1.12+
+			- Fixed calling SYST:ERR? even if *STB? returned 0.
+			- Replaced @ni backend with @ivi for resource manager - this is necessary for the future pyvisa version 1.12+.
 
 		1.11.0 (build 49) 09.06.2021
-			- Added is_connection_active() + reconnect()
+			- Added is_connection_active() + reconnect().
 
 		1.10.1 (build 47) 01.06.2021
-			- Fixed bug with error checking when events are defined
+			- Fixed bug with error checking when events are defined.
 
 		1.10.0 (build 46) 03.05.2021
-			- Added methods to Instrument: query_struct_with_opc(), query_str_suppressed_with_opc()
+			- Added methods to Instrument: query_struct_with_opc(), query_str_suppressed_with_opc().
 
 		1.9.0 (build 45) 13.04.2021
-			- Added option to set callbacks before_write and before_query
-			- When a RepCap has a member with integer number 0 defined, the command string interpretation of such member is '0', not empty string
+			- Added option to set callbacks before_write and before_query.
+			- When a RepCap has a member with integer number 0 defined, the command string interpretation of such member is '0', not empty string.
 
 		1.8.0 (build 43) 19.01.2021
-			- Added matching of Enum instrument responses also in short/long form
+			- Added matching of Enum instrument responses also in short/long form.
 
 		1.7.7 (build 42) 26.11.2020
-			- Extended ArgSingleList.compose_cmd_string() to 9 arguments
+			- Extended ArgSingleList.compose_cmd_string() to 9 arguments.
 
 		1.7.6 (build 41) 23.11.2020
-			- Extended data types for IntegerExt, FloatExt, IntegerExtArray, FloatExtArray
+			- Extended data types for IntegerExt, FloatExt, IntegerExtArray, FloatExtArray.
 
 		1.7.5 (build 40) 12.11.2020
-			- Extended 'Conversions' method str_to_str_list() by parameter 'clear_one_empty_item' with default value False
+			- Extended 'Conversions' method str_to_str_list() by parameter 'clear_one_empty_item' with default value False.
 
 		1.7.4 (build 39) 11.09.2020
-			- Fixed parsing of the instrument errors when an error message contains two double quotes
+			- Fixed parsing of the instrument errors when an error message contains two double quotes.
 
 		1.7.3 (build 38) 21.10.2020
-			- Added 'UND' to the list of float numbers that are represented as NaN
+			- Added 'UND' to the list of float numbers that are represented as NaN.
 
 		1.7.2 (build 37) 10.10.2020
-			- SCPI response string conversion to scalar enum: if the string contains ',', the content after it inclusive the comma is ignored
+			- SCPI response string conversion to scalar enum: if the string contains ',', the content after it inclusive the comma is ignored.
 
 		1.7.1 (build 36) 08.10.2020
-			- Fixed Python 3.8.5+ warnings
+			- Fixed Python 3.8.5+ warnings.
 
 		1.7.0 (build 34) 30.09.2020
-			- Added option to set the termination characters for reading and writing. Until now, it was fixed to '\n' (Linefeed)
-			- Replaced 'import visa' with 'import pyvisa' to remove Python 3.8 pyvisa warnings
+			- Added option to set the termination characters for reading and writing. Until now, it was fixed to '\n' (Linefeed).
+			- Replaced 'import visa' with 'import pyvisa' to remove Python 3.8 pyvisa warnings.
 
 		Version History:
 		1.6.0 (build 33) 17.09.2020
-			- Added special characters encoding/decoding in enums
+			- Added special characters encoding/decoding in enums.
 
 		1.4.0 (build 32) 17.09.2020
-			- Added recognition of RsVisa library location for linux when using options string 'SelectVisa=rs'
-			- Fixed bug in reading binary data 16 bit
+			- Added recognition of RsVisa library location for linux when using options string 'SelectVisa=rs'.
+			- Fixed bug in reading binary data 16 bit.
 
 		1.3.0 (build 31) 04.09.2020
-			- added DRIVERSETUP_QUERYOPT to the driver's option string
+			- added DRIVERSETUP_QUERYOPT to the driver's option string.
 			- *OPT? is no longer performed at the init, but only at the first access to the options string.
-				In addition, the *OPT? query is executed with 1000 ms timeout, and the errors are suppressed
+				In addition, the *OPT? query is executed with 1000 ms timeout, and the errors are suppressed.
 
 		1.2.0 (build 30), 03.08.2020
-			- Fixed NRP-Z session parameters: vxi_capable = False, io_segment_size = 1000000
+			- Fixed NRP-Z session parameters: vxi_capable = False, io_segment_size = 1000000.
 
 		1.1.0 (build 29), 20.06.2020
-			- Added RepeatedCapability and base class CommandsGroup
-			- Fixed simulation mode switching
+			- Added RepeatedCapability and base class CommandsGroup.
+			- Fixed simulation mode switching.
+
+		0.9.3 (build 25), 23.04.2020
+			- Fixed composition of optional arguments in ArgSingleList and ArgSingle.
+
+		0.9.2 (build 24), 13.11.2019
+			- Added recognition of special values for enum return strings.
+
+		0.9.1
+			- Added read / write to file, refactored internals to work with streams.
 
-		0.9.3 (build 25), 23.04.2020 - Fixed composition of optional arguments in ArgSingleList and ArgSingle
-		0.9.2 (build 24), 13.11.2019 - Added recognition of special values for enum return strings
-		0.9.1 - Added read / write to file, refactored internals to work with streams
-		0.9.0 - First Version created."""
+		0.9.0
+			- First Version created."""
 
 	driver_version: str = ''
 	"""Placeholder for the driver version string."""
 
 	def __init__(
 			self,
 			resource_name: str,
@@ -187,15 +212,15 @@
 			reset: bool = False,
 			driver_options: str = None,
 			user_options: str = None,
 			direct_session: object = None):
 		"""Initializes new driver session. For cleaner code, use the class methods: \n
 		- Core.from_existing_session() - initializes a new Core with an existing pyvisa session."""
 
-		self.core_version = '1.55.0'
+		self.core_version = '1.80.0'
 		self.resource_name = resource_name
 
 		# Typical settings for the Core
 		self._instrumentSettings = InstrumentSettings(
 			InstrViClearMode.execute_on_all,  # Instrument viClear mode
 			False,  # Full model name. True: SMW200A, False: SMW
 			0,  # Delay by each write
```

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/GlobalData.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/GlobalData.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/Instrument.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/Instrument.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from . import Utilities, InstrumentSettings, InstrumentOptions, Conversions as Conv
 from .ArgSingleSuppressed import ArgSingleSuppressed
 from .ArgStructList import ArgStructList
 from .InternalLinker import InternalLinker
 from .IoTransferEventArgs import IoTransferEventArgs
 from .StreamReader import StreamReader
 from .StreamWriter import StreamWriter
-from .Utilities import trim_str_response, size_to_kb_mb_string
+from .Utilities import size_to_kb_mb_string
 from .VisaSession import VisaSession, EventArgsChunk
 from .VisaSessionSim import VisaSessionSim
 from .RepeatedCapability import RepeatedCapability
 from .ScpiLogger import ScpiLogger
 from .InstrumentErrors import *
 
 
@@ -76,15 +76,15 @@
 				# noinspection PyTypeChecker
 				self._set_session(VisaSessionSim(resource_name, self._settings, direct_session))
 				self._init_logger(self._session.resource_name)
 				self._log_start_segment(direct_start_time)
 				self._lock = self._session.get_lock()
 				self._instr_options = InstrumentOptions.Options('K0', InstrumentOptions.ParseMode.KeepOriginal)
 				self._session.write('*OPT K0')
-				self._log_info('Simulation session init', f"Simulation device{dir_str} '{self.resource_name}'")
+				self._log_info('Simulation session init', f"Simulation device{dir_str} '{self.resource_name}'", "@INIT_SIMULATION_SESSION")
 				self._log_end_segment()
 				return
 
 			self._set_session(VisaSession(resource_name, self._settings, direct_session))
 			self._init_logger(self._session.resource_name)
 			self._log_start_segment(direct_start_time)
 
@@ -106,15 +106,15 @@
 				# NRP-Z session coercing
 				if self._session.is_rsnrp_session():
 					self._settings.instr_options_parse_mode = InstrumentOptions.ParseMode.Skip
 					self.stb_in_error_check = False
 
 				self.instr_options_parse_mode = self._settings.instr_options_parse_mode
 
-			self._log_info('Session init', f"Device{dir_str} '{self.resource_name}' IDN: {self.idn_string}")
+			self._log_info('Session init', f"Device{dir_str} '{self.resource_name}' IDN: {self.idn_string}", "@INIT_SESSION")
 
 		except RsInstrException as e:
 			if not self.logger:
 				self._assure_logger_exists()
 				self._log_start_segment(direct_start_time)
 			self._log_error('Session init error', e.args[0], self._start_time, datetime.now())
 			raise
@@ -138,14 +138,16 @@
 		if self._settings.logging_name is not None and self._settings.logging_name != rsrc_name:
 			self.logger.device_name = self._settings.logging_name
 		self.logger.allow_log_string_adjust = False
 		self.logger.mode = self._settings.logging_mode
 		self.logger.log_to_console = self._settings.log_to_console
 		self.logger.log_to_udp = self._settings.log_to_udp
 		self.logger.udp_port = self._settings.log_udp_port
+		if self._settings.logging_format is not None:
+			self.logger.set_format_string(self._settings.logging_format)
 		if self._settings.log_to_global_target:
 			self.logger.set_logging_target_global()
 
 	def _assure_logger_exists(self) -> None:
 		"""Initializes backup logger if the VisaSession ended with exception causing main logger to not be initialized.
 		If the logger instance exists, the method does nothing."""
 		if self.logger:
@@ -187,36 +189,36 @@
 		Returns True, if the reconnection has been performed."""
 		if not self.allow_reconnect:
 			raise RsInstrException('Reused sessions do not support reconnection')
 		self._start_time = datetime.now()
 		active = self.is_connection_active()
 		log_info = 'Forced Reconnection' if force_close else 'Reconnection'
 		if force_close and active:
-			self._log_info(log_info, 'Session was active, closing the session')
+			self._log_info(log_info, 'Session was active, closing the session', None)
 			self.close(log_info)
 			active = False
 		if active is True:
-			self._log_info(log_info, 'Session is still active, no action needed')
+			self._log_info(log_info, 'Session is still active, no action needed', None)
 			return False
 		if not active:
 			# Connect again
 			try:
 				dir_str = ' from direct session' if self._direct_session else ''
 				sim = ' simulation' if self._direct_session else ''
 				init_method = VisaSessionSim if self._simulating else VisaSession
 
 				self._log_start_segment()
 				self.__session = init_method(self.resource_name, self._settings, self._direct_session)
-				self._log_info(log_info, f"Session init,{sim} device{dir_str} '{self.resource_name}, IDN: {self.idn_string}'")
+				self._log_info(log_info, f"Session init,{sim} device{dir_str} '{self.resource_name}, IDN: {self.idn_string}'", "@RECONNECT")
 				self._log_end_segment()
 				with self._lock:
 					self._session.clear_before_read()
 			except RsInstrException as e:
 				if self.logger:
-					self._log_error(log_info, e.args[0])
+					self._log_error(log_info, e.args[0], "@RECONNECT")
 				raise
 			finally:
 				if self.logger:
 					self._log_end_segment()
 			return True
 
 	def set_simulating_cmds(self) -> None:
@@ -263,59 +265,59 @@
 		self._last_error_log = None
 		if direct_start_time:
 			self._start_time = direct_start_time
 		else:
 			self._start_time = datetime.now()
 		self.logger.start_new_segment()
 
-	def _log_info(self, log_string_info: str, log_string: str) -> None:
+	def _log_info(self, log_string_info: str, log_string: str, cmd: str or None) -> None:
 		"""Logs an ASCII entry."""
 		self._last_exc_log = None
-		self.logger.info(self._start_time, datetime.now(), log_string_info, log_string)
+		self.logger.info(self._start_time, datetime.now(), log_string_info, log_string, cmd)
 
-	def _log_info_list(self, log_string_info: str, list_data: List) -> None:
+	def _log_info_list(self, log_string_info: str, list_data: List, cmd: str or None) -> None:
 		"""Logs a List entry."""
 		self._last_exc_log = None
-		self.logger.info_list(self._start_time, datetime.now(), log_string_info, list_data)
+		self.logger.info_list(self._start_time, datetime.now(), log_string_info, cmd, list_data)
 
-	def _log_info_bin(self, log_string_info: str, log_data: bytes) -> None:
+	def _log_info_bin(self, log_string_info: str, log_data: bytes, cmd: str or None) -> None:
 		"""Logs a binary entry."""
 		self._last_exc_log = None
-		self.logger.info_bin(self._start_time, datetime.now(), log_string_info, log_data)
+		self.logger.info_bin(self._start_time, datetime.now(), log_string_info, cmd, log_data)
 
-	def _log_info_var_stream(self, log_string_info: str, binary: bool, content: AnyStr) -> None:
+	def _log_info_var_stream(self, log_string_info: str, binary: bool, content: AnyStr, cmd: str or None) -> None:
 		"""Logs a stream entry - must be variable only, but can be binary or ascii."""
 		self._last_exc_log = None
 		if binary:
-			self.logger.info_bin(self._start_time, datetime.now(), log_string_info, content)
+			self.logger.info_bin(self._start_time, datetime.now(), log_string_info, cmd, content)
 		else:
-			self.logger.info(self._start_time, datetime.now(), log_string_info, content)
+			self.logger.info(self._start_time, datetime.now(), log_string_info, cmd, content)
 
-	def _log_error(self, log_string_info: str, log_string: str, start_time: datetime = None, end_time: datetime = None) -> None:
+	def _log_error(self, log_string_info: str, log_string: str, cmd: str or None, start_time: datetime = None, end_time: datetime = None) -> None:
 		"""Logs an ASCII error entry."""
-		self.logger.error(start_time, end_time, log_string_info, log_string)
+		self.logger.error(start_time, end_time, log_string_info, log_string, cmd)
 
-	def _log_exception(self, e: Exception, context: str = None, start_time: datetime = None, end_time: datetime = None) -> None:
+	def _log_exception(self, e: Exception, cmd: str or None, context: str = None, start_time: datetime = None, end_time: datetime = None) -> None:
 		"""Logs an ASCII error entry taken from the exception message."""
 		if start_time is None:
 			start_time = self._start_time
 		if end_time is None:
 			end_time = datetime.now()
 
 		msg: str = e.args[0]
 		if isinstance(e, StatusException):
 			# Status exceptions are handled specially to prevent duplicate logging of the same StatusException
 			if msg == self._last_exc_log:
 				return
 			self._last_exc_log = msg
 			msg = f'{e.__class__.__name__}: {msg}'
-			self.logger.error(start_time, end_time, context, msg)
+			self.logger.error(start_time, end_time, context, msg, cmd)
 		else:
 			self._last_exc_log = None
-			self.logger.error(start_time, end_time, context, f'{e.__class__.__name__}: {msg}')
+			self.logger.error(start_time, end_time, context, f'{e.__class__.__name__}: {msg}', cmd)
 
 	def _log_end_segment(self) -> None:
 		"""Ends logging segment."""
 
 		if self._start_time:
 			# Accumulate the spent times
 			end_time = datetime.now()
@@ -494,17 +496,17 @@
 				log_info = 'Query Instrument Options'
 				try:
 					self._log_start_segment()
 					opts = self._session.query_str_no_tout_err('*OPT?', 1000)
 					if opts is None:
 						opts = 'Cannot read the instrument options - *OPT? query is not supported'
 					self._instr_options = InstrumentOptions.Options(opts, mode)
-					self._log_info(log_info, f'*OPT? {opts}')
+					self._log_info(log_info, f'*OPT? {opts}', '*OPT?')
 				except RsInstrException as e:
-					self._log_exception(e, log_info)
+					self._log_exception(e, '*OPT?', log_info)
 					raise
 				finally:
 					self._log_end_segment()
 
 	def add_global_repcap(self, name: str, rep_cap: RepeatedCapability) -> None:
 		"""Adds the global repcap name to the list of global repcaps
 		and sets its value to the provided default value."""
@@ -539,17 +541,17 @@
 			return True
 		with self._lock:
 			try:
 				self._log_start_segment()
 				self.start_send_read_event('*OPC?', False)
 				opc: bool = self._session.query_opc(timeout)
 				self.end_send_read_event()
-				self._log_info('Query OPC', '1' if opc else '0')
+				self._log_info('Query OPC', '1' if opc else '0', '*OPC?')
 			except RsInstrException as e:
-				self._log_exception(e, 'Query OPC')
+				self._log_exception(e, '*OPC?', 'Query OPC')
 				raise
 			finally:
 				self._log_end_segment()
 			return opc
 
 	def query_all_syst_errors(self, include_codes: bool = True, enable_log: bool = True) -> List[str] or List[int, str] or None:
 		"""Returns all errors in the instrument's error queue. If no error is detected, the return value is None.
@@ -571,27 +573,27 @@
 						entries = [f"{x[1]},'{x[0]}'" for x in errors]
 					else:
 						errors = [x[1] for x in errors]
 						entries = errors
 				# Return errors as list of strings
 				if enable_log is True:
 					if errors is None or len(errors) == 0:
-						self._log_info(log_info, 'No errors')
+						self._log_info(log_info, 'No errors', 'SYST:ERROR?')
 					elif len(errors) == 1:
-						self._log_info(log_info, f'1 error detected - {entries[0]}')
+						self._log_info(log_info, f'1 error detected - {entries[0]}', 'SYST:ERROR?')
 					else:
-						self._log_info(log_info, f'{len(errors)} errors detected (last one on top)')
+						self._log_info(log_info, f'{len(errors)} errors detected (last one on top)', 'SYST:ERROR?')
 						i = 1
 						for x in entries:
-							self._log_info(f'SYST:ERROR? {i}', x)
+							self._log_info(f'SYST:ERROR? {i}', x, 'SYST:ERROR?')
 							i += 1
 			except RsInstrException as e:
 				# General errors: log the exception message
 				if enable_log is True:
-					self._log_exception(e, log_info, start_time=self._start_time, end_time=datetime.now())
+					self._log_exception(e, 'SYST:ERROR?', log_info, start_time=self._start_time, end_time=datetime.now())
 				raise
 			return errors
 
 	def check_status(self) -> None:
 		"""Throws InstrumentStatusException in case of an error in the instrument's error queue.
 		The procedure is skipped, if the QueryInstrumentStatus is set to false."""
 		with self._lock:
@@ -601,18 +603,18 @@
 				self._start_time = datetime.now()
 			try:
 				call_syst_error = self._session.error_in_error_queue() if self.stb_in_error_check else True
 				if call_syst_error:
 					errors = self.query_all_syst_errors(enable_log=False)
 					assert_no_instrument_status_errors(self.resource_name, errors)
 				if self.logger.log_status_check_ok:
-					self._log_info('Status check', 'OK')
+					self._log_info('Status check', 'OK', '*STB?')
 			except RsInstrException as e:
 				# General errors: log the exception message
-				self._log_exception(e, 'Status check', start_time=self._start_time, end_time=datetime.now())
+				self._log_exception(e, '*STB?', 'Status check', start_time=self._start_time, end_time=datetime.now())
 				raise
 
 	def is_connection_active(self) -> bool:
 		"""Returns true, if the VISA connection is active and the communication with the instrument still works.
 		This is achieved by:
 		- checking the session property timeout
 		- sending the *IDN? query"""
@@ -623,17 +625,17 @@
 	def clear_status(self) -> None:
 		"""Clears instrument's status subsystem."""
 		with self._lock:
 			try:
 				self._log_start_segment()
 				self._session.clear()
 				self._session.clear_before_read()
-				self._log_info('Clear status', 'OK')
+				self._log_info('Clear status', 'OK', '*CLS')
 			except RsInstrException as e:
-				self._log_exception(e, 'Clear status')
+				self._log_exception(e, '*CLS', 'Clear status')
 				raise
 			finally:
 				self._log_end_segment()
 
 	def reset(self, timeout: int = 0) -> None:
 		"""Resets the instrument and clears its status.
 		If you define timeout > 0, the VISA timeout is set to that value just for this method call."""
@@ -665,18 +667,18 @@
 				cmd = self._replace_global_repcaps(cmd)
 				self._call_before_write_handler(cmd, block_callback)
 				self._session.write(cmd)
 				if self.opc_query_after_write:
 					self._session.query_opc()
 				if self.on_write_handler:
 					self.send_write_str_event(cmd, False)
-				self._log_info(log_info, cmd)
+				self._log_info(log_info, cmd, cmd)
 				self.check_status()
 			except RsInstrException as e:
-				self._log_exception(e, log_info)
+				self._log_exception(e, cmd, log_info)
 				raise
 			finally:
 				self._log_end_segment()
 
 	def write_with_opc(self, cmd: str, timeout: int = None, block_callback: bool = False, log_info: str = 'Write string with OPC') -> None:
 		"""Writes a OPC-synced command.
 		Also performs error checking if the property self.query_instr_status is set to True.
@@ -689,18 +691,18 @@
 				self._log_start_segment()
 				cmd = self._replace_global_repcaps(cmd)
 				self._call_before_write_handler(cmd, block_callback)
 				self._session.write_with_opc(cmd, timeout)
 				self._session.query_and_clear_esr()
 				if self.on_write_handler:
 					self.send_write_str_event(cmd, True)
-				self._log_info(log_info, cmd)
+				self._log_info(log_info, cmd, cmd)
 				self.check_status()
 			except RsInstrException as e:
-				self._log_exception(e, log_info)
+				self._log_exception(e, cmd, log_info)
 				raise
 			finally:
 				self._log_end_segment()
 
 	def write_struct(self, cmd: str, struct: object) -> None:
 		"""Writes command to the instrument with the parameter composed of the entered structure."""
 		with self._lock:
@@ -725,18 +727,18 @@
 			try:
 				self._log_start_segment()
 				query = self._replace_global_repcaps(query)
 				self.start_send_read_event(query, False)
 				self._call_pre_query_handler(query, block_callback)
 				response = self._session.query_str(query)
 				self.end_send_read_event()
-				self._log_info(log_info, f'{query} {response}')
+				self._log_info(log_info, f'{query} {response}', query)
 				self.check_status()
 			except RsInstrException as e:
-				self._log_exception(e, log_info)
+				self._log_exception(e, query, log_info)
 				raise
 			finally:
 				self._log_end_segment()
 			return response
 
 	def query_str_with_opc(self, query: str, timeout: int = None, block_callback: bool = False, log_info: str = 'Query string with OPC') -> str:
 		"""Sends a OPC-synced query.
@@ -749,18 +751,18 @@
 				query = self._replace_global_repcaps(query)
 				self.start_send_read_event(query, True)
 				self._call_pre_query_handler(query, block_callback)
 				response = self._session.query_str_with_opc(query, timeout, log_info)
 				self.end_send_read_event()
 				if self._session.clear_status_after_query_with_opc():
 					self._session.query_and_clear_esr()
-				self._log_info(log_info, f'{query} {response}')
+				self._log_info(log_info, f'{query} {response}', query)
 				self.check_status()
 			except RsInstrException as e:
-				self._log_exception(e, log_info)
+				self._log_exception(e, query, log_info)
 				raise
 			finally:
 				self._log_end_segment()
 			return response
 
 	def query_bin_block(self, query: str, log_info: str = 'Query binary block') -> bytes:
 		"""Queries binary data block to bytes and returns data as bytes.
@@ -772,18 +774,18 @@
 					self._log_start_segment()
 					query = self._replace_global_repcaps(query)
 					self.start_send_read_event(query, False)
 					self._call_pre_query_handler(query, False)
 					self._session.query_bin_block(query, stream, True)
 					self.end_send_read_event()
 					content = stream.content
-					self._log_info_var_stream(f'{log_info}, received', stream.binary, content)
+					self._log_info_var_stream(f'{log_info}, received', stream.binary, content, query)
 					self.check_status()
 				except RsInstrException as e:
-					self._log_exception(e, log_info)
+					self._log_exception(e, query, log_info)
 					raise
 				finally:
 					self._log_end_segment()
 				return content
 
 	def query_bin_block_with_opc(self, query: str, timeout: int = None, log_info: str = 'Query binary block with OPC') -> bytes:
 		"""Sends a OPC-synced query and returns data as bytes.
@@ -796,18 +798,18 @@
 					query = self._replace_global_repcaps(query)
 					self.start_send_read_event(query, True)
 					self._call_pre_query_handler(query, False)
 					self._session.query_bin_block_with_opc(query, stream, True, timeout)
 					self.end_send_read_event()
 					self._session.query_and_clear_esr()
 					content = stream.content
-					self._log_info_var_stream(f'{log_info}, received', stream.binary, content)
+					self._log_info_var_stream(f'{log_info}, received', stream.binary, content, query)
 					self.check_status()
 				except RsInstrException as e:
-					self._log_exception(e, log_info)
+					self._log_exception(e, query, log_info)
 					raise
 				finally:
 					self._log_end_segment()
 				return content
 
 	def query_bin_block_to_file(self, query: str, file_path: str, append: bool = False, log_info='Query binary block to file') -> None:
 		"""Queries binary data block to the provided file.
@@ -820,18 +822,18 @@
 					self._log_start_segment()
 					query = self._replace_global_repcaps(query)
 					self.start_send_read_event(query, False)
 					self._call_pre_query_handler(query, False)
 					self._session.query_bin_block(query, stream, True)
 					self.end_send_read_event()
 					add_str = 'target file' if append is False else 'appended to target file'
-					self._log_info(log_info, f'Query {query} - written {size_to_kb_mb_string(stream.written_len, True)}, {add_str} {file_path}')
+					self._log_info(log_info, f'Query {query} - written {size_to_kb_mb_string(stream.written_len, True)}, {add_str} {file_path}', query)
 					self.check_status()
 				except RsInstrException as e:
-					self._log_exception(e, log_info)
+					self._log_exception(e, query, log_info)
 					raise
 				finally:
 					self._log_end_segment()
 
 	def query_bin_block_to_file_with_opc(self, query: str, file_path: str, append: bool = False, timeout: int = None, log_info='Query binary block to file with OPC') -> None:
 		"""Sends a OPC-synced query and writes the returned data to the provided file.
 		If append is False, any existing file content is discarded.
@@ -846,18 +848,18 @@
 					self.start_send_read_event(query, True)
 					self._call_pre_query_handler(query, False)
 					self._session.query_bin_block_with_opc(query, stream, True, timeout)
 					self.end_send_read_event()
 					if self._session.clear_status_after_query_with_opc():
 						self._session.query_and_clear_esr()
 					add_str = 'target file' if append is False else 'appended to target file'
-					self._log_info(log_info, f'Query {query} - written {size_to_kb_mb_string(stream.written_len, True)}, {add_str} {file_path}')
+					self._log_info(log_info, f'Query {query} - written {size_to_kb_mb_string(stream.written_len, True)}, {add_str} {file_path}', query)
 					self.check_status()
 				except RsInstrException as e:
-					self._log_exception(e, log_info)
+					self._log_exception(e, query, log_info)
 					raise
 				finally:
 					self._log_end_segment()
 
 	def query_int(self, query: str) -> int:
 		"""Sends a query and reads response from the instrument as integer."""
 		with self._lock:
@@ -905,50 +907,59 @@
 		If you do not provide timeout, the method uses current opc_timeout."""
 		with self._lock:
 			string = self.query_str_with_opc(query, timeout, log_info='Query boolean with OPC')
 			if self._simulating and self._sim_cached_value_not_found(string):
 				return False
 			return Conv.str_to_bool(string)
 
-	def query_str_list(self, query: str) -> List[str]:
-		"""Sends a query and reads response from the instrument as csv-list."""
+	def query_str_list(self, query: str, remove_blank_response: bool = False) -> List[str]:
+		"""Sends a query and reads response from the instrument as a csv-list.
+		Empty response is returned as an empty list [].
+		Meaning of the 'remove_blank_response':
+			- False(default): whitespaces-only response is returned as a list with one empty element [''].
+			- True: whitespaces-only response is returned as an empty list []."""
 		with self._lock:
 			string = self.query_str(query, log_info='Query string list')
 			if self._simulating and self._sim_cached_value_not_found(string):
 				string = 'AAA,BBB,CCC,DDD,EEE,FFF,GGG,HHH,III,JJJ'
-			response = [trim_str_response(x) for x in string.split(',')]
+			response = Conv.str_to_str_list(string, remove_blank_response)
 			return response
 
-	def query_str_list_with_opc(self, query: str, timeout: int = None) -> List[str]:
+	def query_str_list_with_opc(self, query: str, timeout: int = None, remove_blank_response: bool = False) -> List[str]:
 		"""Sends a OPC-synced query and reads response from the instrument as csv-list.
-		If you do not provide timeout, the method uses current opc_timeout."""
+		If you do not provide timeout, the method uses current opc_timeout.
+		Meaning of the 'remove_blank_response':
+			- False(default): whitespaces-only response is returned as a list with one empty element [''].
+			- True: whitespaces-only response is returned as an empty list []."""
 		with self._lock:
 			string = self.query_str_with_opc(query, timeout, log_info='Query string list with OPC')
 			if self._simulating and self._sim_cached_value_not_found(string):
 				string = 'AAA,BBB,CCC,DDD,EEE,FFF,GGG,HHH,III,JJJ'
-			response = [trim_str_response(x) for x in string.split(',')]
+			response = Conv.str_to_str_list(string, remove_blank_response)
 			return response
 
 	def query_bool_list(self, query: str) -> List[bool]:
-		"""Sends a query and reads response from the instrument as csv-list of booleans."""
+		"""Sends a query and reads response from the instrument as csv-list of booleans.
+		Blank or empty response is returned as an empty list."""
 		with self._lock:
 			string = self.query_str(query, log_info='Query boolean list')
 			if self._simulating and self._sim_cached_value_not_found(string):
 				string = 'True,False,0,1,1,True,true,false,true,false'
-			response = [Conv.str_to_bool(x) for x in string.split(',')]
+			response = Conv.str_to_bool_list(string)
 			return response
 
 	def query_bool_list_with_opc(self, query: str, timeout: int = None) -> List[bool]:
 		"""Sends a OPC-synced query and reads response from the instrument as csv-list of booleans.
+		Blank or empty response is returned as an empty list.
 		If you do not provide timeout, the method uses current opc_timeout."""
 		with self._lock:
 			string = self.query_str_with_opc(query, timeout, log_info='Query boolean list with OPC')
 			if self._simulating and self._sim_cached_value_not_found(string):
 				string = 'True,False,0,1,1,True,true,false,true,false'
-			response = [Conv.str_to_bool(x) for x in string.split(',')]
+			response = Conv.str_to_bool_list(string)
 			return response
 
 	def write_bin_block(self, cmd: str, payload: bytes, log_info: str = 'Write binary block') -> None:
 		"""Writes all the payload as binary data block to the instrument.
 		The binary data header is added at the beginning of the transmission automatically, do not include it in the payload!!!"""
 		with self._lock:
 			try:
@@ -956,18 +967,18 @@
 				cmd = self._replace_global_repcaps(cmd)
 				self._call_before_write_handler(cmd, False)
 				stream = StreamReader.as_bin_var(payload)
 				if self.on_write_handler:
 					self.start_send_write_bin_event(cmd)
 				self._session.write_bin_block(cmd, stream)
 				self.end_send_write_bin_event()
-				self._log_info_bin(f'{log_info} {cmd}, binary data', payload)
+				self._log_info_bin(f'{log_info} {cmd}, binary data', payload, cmd)
 				self.check_status()
 			except RsInstrException as e:
-				self._log_exception(e, log_info)
+				self._log_exception(e, cmd, log_info)
 				raise
 			finally:
 				self._log_end_segment()
 
 	def write_bin_block_from_file(self, cmd: str, file_path: str, log_info: str = 'Write binary block from file') -> None:
 		"""Writes all the file content as binary data block to the instrument.
 		The binary data header is added at the beginning of the transmission automatically, do not include it in the file content!!!"""
@@ -977,18 +988,18 @@
 					self._log_start_segment()
 					cmd = self._replace_global_repcaps(cmd)
 					self._call_before_write_handler(cmd, False)
 					if self.on_write_handler:
 						self.start_send_write_bin_event(cmd)
 					self._session.write_bin_block(cmd, stream)
 					self.end_send_write_bin_event()
-					self._log_info(log_info, f'Command {cmd} - written {size_to_kb_mb_string(stream.read_len, True)}, source file {file_path}')
+					self._log_info(log_info, f'Command {cmd} - written {size_to_kb_mb_string(stream.read_len, True)}, source file {file_path}', cmd)
 					self.check_status()
 				except RsInstrException as e:
-					self._log_exception(e, log_info)
+					self._log_exception(e, cmd, log_info)
 					raise
 				finally:
 					self._log_end_segment()
 
 	def send_file_from_pc_to_instrument(self, source_pc_file: str, target_instr_file: str) -> None:
 		"""SCPI Command: MMEM:DATA \n
 		Sends file from PC to the instrument"""
@@ -1009,21 +1020,21 @@
 		log_info = 'Testing file existence'
 		with self._lock:
 			try:
 				self._log_start_segment()
 				self._call_pre_query_handler(query, False)
 				length = self._session.get_bin_data_length(query)
 				if length is None:
-					self._log_info(log_info, f'File {instr_file} does not exist.')
+					self._log_info(log_info, f'File {instr_file} does not exist.', query)
 				else:
-					self._log_info(log_info, f'File {instr_file} exists, size {size_to_kb_mb_string(length, True)}')
+					self._log_info(log_info, f'File {instr_file} exists, size {size_to_kb_mb_string(length, True)}', query)
 				self.check_status()
 				return length
 			except RsInstrException as e:
-				self._log_exception(e, log_info)
+				self._log_exception(e, query, log_info)
 				raise
 			finally:
 				self._log_end_segment()
 
 	def query_bin_or_ascii_float_list(self, query: str, log_info: str = 'Query binary or ascii float list') -> List[float]:
 		"""Queries a list of floating-point numbers that can be read in ASCII format or in binary format.
 		- For ASCII format, the list numbers are decoded as comma-separated values.
@@ -1038,22 +1049,22 @@
 				self._call_pre_query_handler(query, False)
 				self._session.query_bin_block(query, stream, False)
 				self.end_send_read_event()
 				if self._simulating and not self._session.cached_to_stream:
 					return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
 				if stream.binary:
 					result = Conv.bytes_to_list_of_floats(stream.content, self.bin_float_numbers_format)
-					self._log_info_list(f'{log_info}, received binary format list {size_to_kb_mb_string(stream.written_len, True)} {stream.written_len // len(result)} bytes per number', result)
+					self._log_info_list(f'{log_info}, received binary format list {size_to_kb_mb_string(stream.written_len, True)} {stream.written_len // len(result)} bytes per number', result, query)
 				else:
 					result = Conv.str_to_float_list(stream.content)
-					self._log_info_list(f'{log_info}, received ascii format list', result)
+					self._log_info_list(f'{log_info}, received ascii format list', result, query)
 				self.check_status()
 				return result
 			except RsInstrException as e:
-				self._log_exception(e, log_info)
+				self._log_exception(e, query, log_info)
 				raise
 			finally:
 				self._log_end_segment()
 
 	def query_bin_or_ascii_float_list_with_opc(self, query: str, timeout: int = None, log_info: str = 'Query binary or ascii float list with OPC') -> List[float]:
 		"""Sends a OPC-synced query and reads a list of floating-point numbers that can be read in ASCII format or in binary format.
 		- For ASCII format, the list numbers are decoded as comma-separated values.
@@ -1069,24 +1080,24 @@
 				self._call_pre_query_handler(query, False)
 				self._session.query_bin_block_with_opc(query, stream, False, timeout)
 				self.end_send_read_event()
 				if self._simulating and not self._session.cached_to_stream:
 					return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
 				if stream.binary:
 					result = Conv.bytes_to_list_of_floats(stream.content, self.bin_float_numbers_format)
-					self._log_info_list(f'{log_info}, received binary format list {size_to_kb_mb_string(stream.written_len, True)} {stream.written_len // len(result)} bytes per number', result)
+					self._log_info_list(f'{log_info}, received binary format list {size_to_kb_mb_string(stream.written_len, True)} {stream.written_len // len(result)} bytes per number', result, query)
 				else:
 					result = Conv.str_to_float_list(stream.content)
-					self._log_info_list(f'{log_info}, received ascii format list', result)
+					self._log_info_list(f'{log_info}, received ascii format list', result, query)
 				if self._session.clear_status_after_query_with_opc():
 					self._session.query_and_clear_esr()
 				self.check_status()
 				return result
 			except RsInstrException as e:
-				self._log_exception(e, log_info)
+				self._log_exception(e, query, log_info)
 				raise
 			finally:
 				self._log_end_segment()
 
 	def query_bin_or_ascii_float_list_suppressed(self, query: str, suppressed: ArgSingleSuppressed) -> List[float]:
 		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of floats.
 		The current implementation allows for the rest of the string to be only ASCII format."""
@@ -1122,22 +1133,22 @@
 				self._call_pre_query_handler(query, False)
 				self._session.query_bin_block(query, stream, False)
 				self.end_send_read_event()
 				if self._simulating and not self._session.cached_to_stream:
 					return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
 				if stream.binary:
 					result = Conv.bytes_to_list_of_integers(stream.content, self.bin_int_numbers_format)
-					self._log_info_list(f'{log_info}, received binary format list {size_to_kb_mb_string(stream.written_len, True)} {stream.written_len // len(result)} bytes per number', result)
+					self._log_info_list(f'{log_info}, received binary format list {size_to_kb_mb_string(stream.written_len, True)} {stream.written_len // len(result)} bytes per number', result, query)
 				else:
 					result = Conv.str_to_int_list(stream.content)
-					self._log_info_list(f'{log_info}, received ascii format list', result)
+					self._log_info_list(f'{log_info}, received ascii format list', result, query)
 				self.check_status()
 				return result
 			except RsInstrException as e:
-				self._log_exception(e, log_info)
+				self._log_exception(e, query, log_info)
 				raise
 			finally:
 				self._log_end_segment()
 
 	def query_bin_or_ascii_int_list_with_opc(self, query: str, timeout: int = None, log_info: str = 'Query binary or ascii integer list with OPC') -> List[int]:
 		"""Sends a OPC-synced query and reads a list of integer numbers that can be read in ASCII format or in binary format.
 		- For ASCII format, the list numbers are decoded as comma-separated values.
@@ -1153,24 +1164,24 @@
 				self._call_pre_query_handler(query, False)
 				self._session.query_bin_block_with_opc(query, stream, False, timeout)
 				self.end_send_read_event()
 				if self._simulating and not self._session.cached_to_stream:
 					return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
 				if stream.binary:
 					result = Conv.bytes_to_list_of_integers(stream.content, self.bin_int_numbers_format)
-					self._log_info_list(f'{log_info}, received binary format list {size_to_kb_mb_string(stream.written_len, True)} {stream.written_len // len(result)} bytes per number', result)
+					self._log_info_list(f'{log_info}, received binary format list {size_to_kb_mb_string(stream.written_len, True)} {stream.written_len // len(result)} bytes per number', result, query)
 				else:
 					result = Conv.str_to_int_list(stream.content)
-					self._log_info_list(f'{log_info}, received ascii format list', result)
+					self._log_info_list(f'{log_info}, received ascii format list', result, query)
 				if self._session.clear_status_after_query_with_opc():
 					self._session.query_and_clear_esr()
 				self.check_status()
 				return result
 			except RsInstrException as e:
-				self._log_exception(e, log_info)
+				self._log_exception(e, query, log_info)
 				raise
 			finally:
 				self._log_end_segment()
 
 	def query_bin_or_ascii_int_list_suppressed(self, query: str, suppressed: ArgSingleSuppressed) -> List[int]:
 		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of integers.
 		The current implementation allows for the rest of the string to be only ASCII format."""
@@ -1253,31 +1264,31 @@
 	def go_to_local(self) -> None:
 		"""Puts the instrument into local state."""
 		with self._lock:
 			log_info = 'Go To Local'
 			try:
 				self._log_start_segment()
 				self._session.go_to_local()
-				self._log_info(log_info, 'Going to Local State')
+				self._log_info(log_info, 'Going to Local State', '@GTL')
 			except RsInstrException as e:
-				self._log_exception(e, log_info)
+				self._log_exception(e, '@GTL', log_info)
 				raise
 			finally:
 				self._log_end_segment()
 
 	def go_to_remote(self) -> None:
 		"""Puts the instrument into remote state."""
 		with self._lock:
 			log_info = 'Go To Remote'
 			try:
 				self._log_start_segment()
 				self._session.go_to_remote()
-				self._log_info(log_info, 'Going to Remote State')
+				self._log_info(log_info, 'Going to Remote State', '@GTR')
 			except RsInstrException as e:
-				self._log_exception(e, log_info)
+				self._log_exception(e, '@GTR', log_info)
 				raise
 			finally:
 				self._log_end_segment()
 
 	def get_session_handle(self) -> object:
 		"""Returns the underlying pyvisa session."""
 		return self._session.get_session_handle()
@@ -1291,20 +1302,20 @@
 					reused = self._session.reusing_session
 					self._session.close()
 					self._clear_session()
 					try:
 						# Tolerate error when trying to log to the closed stream.
 						# This is only tolerated in the close() method.
 						log_string = 'Closing reused session' if reused else 'Closing session'
-						self._log_info(log_info, log_string)
+						self._log_info(log_info, log_string, '@CLOSE_SESSION')
 					except RsInstrException as e:
 						if 'Error logging to the stream' not in e.args[0]:
 							raise
 			except RsInstrException as e:
-				self._log_exception(e, log_info)
+				self._log_exception(e, None, log_info)
 				raise
 			finally:
 				self._log_end_segment()
 
 	# Events part -------------------------------------------------------------
 	@property
 	def io_events_include_data(self) -> bool:
```

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/InstrumentErrors.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/InstrumentErrors.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 	def __init__(self, message: str):
 		super(TimeoutException, self).__init__(message)
 
 
 class StatusException(RsInstrException):
 	"""Exception for instrument status errors.
 	Tje field  errors_list contains the complete list of all the errors with messages and codes."""
-	def __init__(self, rsrc_name: str, message: str, errors_list: List[Tuple[int, str]], first_exc: Exception = None):
+	def __init__(self, rsrc_name: str, message: str, errors_list: List[Tuple[int, str]], first_exc: type = None):
 		self.rsrc_name: str = rsrc_name
-		self.first_exc: Exception = first_exc
+		self.first_exc: type = first_exc
 		self.errors_list: List[Tuple[int, str]] = errors_list
 		super(StatusException, self).__init__(message)
 
 
 class UnexpectedResponseException(RsInstrException):
 	"""Exception for instrument unexpected responses."""
 	def __init__(self, rsrc_name: str, message: str):
```

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/InstrumentOptions.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/InstrumentOptions.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/InstrumentSettings.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/InstrumentSettings.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 		self.bin_int_numbers_format = bin_int_numbers_format
 		self.opc_query_after_write = opc_query_after_write
 		self.opc_query_after_write = opc_query_after_write
 		self.opc_query_sync_mechanism = opc_query_sync_mechanism
 
 		self.logging_mode = logging_mode
 		self.logging_name = None
+		self.logging_format = None
 		self.log_to_global_target = False
 		self.log_to_console = False
 		self.log_to_udp = False
 		self.log_udp_port = 49200
 
 		self.assure_write_with_tc = False
 		self.term_char = '\n'
@@ -331,14 +332,18 @@
 			self.logging_mode = enum_value
 
 		# Logging
 		value = self._get_driversetup_item('LoggingName')
 		if value:
 			self.logging_name = value
 
+		value = self._get_driversetup_item('LoggingFormat')
+		if value:
+			self.logging_format = value
+
 		value = self._get_driversetup_item('LogToGlobalTarget')
 		if value:
 			self.log_to_global_target = Conv.str_to_bool(value)
 
 		value = self._get_driversetup_item('LoggingToConsole')
 		if value:
 			self.log_to_console = Conv.str_to_bool(value)
```

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/InternalLinker.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/InternalLinker.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/IoTransferEventArgs.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/IoTransferEventArgs.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/RepeatedCapability.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/RepeatedCapability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ScpiEnums.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ScpiEnums.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ScpiLogger.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/ScpiLogger.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,55 +20,56 @@
     Errors = 2  # Only log errors. This is like 'Off', with the exception, that VisaIOErrors are logged.
     Default = 3  # Default mode
 
 
 class LogEntry:
     """One entry in the log Defined by content, which has all the variables resolved except the START_TIME and the end_time."""
 
-    _tab_var_re = re.compile(r'PAD_(LEFT|RIGHT)(\d+)\(%(START_TIME|END_TIME|DURATION|DEVICE_NAME|LOG_STRING_INFO|LOG_STRING)%\)')
-    _var_re = re.compile(r'%(START_TIME|END_TIME|DURATION|DEVICE_NAME|LOG_STRING_INFO|LOG_STRING)%')
+    _tab_var_re = re.compile(r'PAD_(LEFT|RIGHT)(\d+)\(%(START_TIME|END_TIME|DURATION|DEVICE_NAME|LOG_STRING_INFO|LOG_STRING|SCPI_COMMAND)%\)')
+    _var_re = re.compile(r'%(START_TIME|END_TIME|DURATION|DEVICE_NAME|LOG_STRING_INFO|LOG_STRING|SCPI_COMMAND)%')
 
-    def __init__(self, start_time: datetime or None or float, end_time: datetime or None or float, device_name: str, log_string_info: str, log_string: str, add_new_line: bool, error: bool, raw: bool, binary: bool):
+    def __init__(self, start_time: datetime or None or float, end_time: datetime or None or float, device_name: str, log_string_info: str, log_string: str, cmd: str or None, add_new_line: bool, error: bool, raw: bool, binary: bool):
         self._start_time: datetime = start_time
         self._end_time: datetime = end_time
         self._device_name: str = device_name
         self._log_string_info: str = log_string_info
         self._log_string: str = log_string
+        self._cmd: str or None = cmd
         self._raw: bool = raw
         self._binary: bool = binary
         self._timestamp_reference_time: datetime or None = None
 
         # Public properties
         self.add_new_line: bool = add_new_line
         self.error: bool = error
 
     @classmethod
     def as_raw_content(cls, content: str, add_new_line: bool) -> 'LogEntry':
         """Create the entry as raw"""
-        return cls(start_time=None, end_time=None, device_name='', log_string_info='', log_string=content, add_new_line=add_new_line, error=False, raw=True, binary=False)
+        return cls(start_time=None, end_time=None, device_name='', log_string_info='', log_string=content, cmd=None, add_new_line=add_new_line, error=False, raw=True, binary=False)
 
     @classmethod
     def as_raw_error_content(cls, content: str, add_new_line: bool) -> 'LogEntry':
         """Create the entry as raw"""
-        return cls(start_time=None, end_time=None, device_name='', log_string_info='', log_string=content, add_new_line=add_new_line, error=True, raw=True, binary=False)
+        return cls(start_time=None, end_time=None, device_name='', log_string_info='', log_string=content, cmd=None, add_new_line=add_new_line, error=True, raw=True, binary=False)
 
     @classmethod
-    def as_info_entry(cls, start_time: datetime or None, end_time: datetime or None, device_name: str, log_string_info: str, log_string: str, add_new_line: bool) -> 'LogEntry':
+    def as_info_entry(cls, start_time: datetime or None, end_time: datetime or None, device_name: str, log_string_info: str, log_string: str, cmd: str or None, add_new_line: bool) -> 'LogEntry':
         """Create the entry as info entry."""
-        return cls(start_time=start_time, end_time=end_time, device_name=device_name, log_string_info=log_string_info, log_string=log_string, add_new_line=add_new_line, error=False, raw=False, binary=False)
+        return cls(start_time=start_time, end_time=end_time, device_name=device_name, log_string_info=log_string_info, log_string=log_string, cmd=cmd, add_new_line=add_new_line, error=False, raw=False, binary=False)
 
     @classmethod
-    def as_error_entry(cls, start_time: datetime or None, end_time: datetime or None, device_name: str, log_string_info: str, log_string: str, add_new_line: bool) -> 'LogEntry':
+    def as_error_entry(cls, start_time: datetime or None, end_time: datetime or None, device_name: str, log_string_info: str, log_string: str, cmd: str or None, add_new_line: bool) -> 'LogEntry':
         """Create the entry as info entry."""
-        return cls(start_time=start_time, end_time=end_time, device_name=device_name, log_string_info=log_string_info, log_string=log_string, add_new_line=add_new_line, error=True, raw=False, binary=False)
+        return cls(start_time=start_time, end_time=end_time, device_name=device_name, log_string_info=log_string_info, log_string=log_string, cmd=cmd, add_new_line=add_new_line, error=True, raw=False, binary=False)
 
     @classmethod
-    def as_info_bin_entry(cls, start_time: datetime or None, end_time: datetime or None, device_name: str, log_string_info: str, log_string: str, add_new_line: bool) -> 'LogEntry':
+    def as_info_bin_entry(cls, start_time: datetime or None, end_time: datetime or None, device_name: str, log_string_info: str, log_string: str, cmd: str or None, add_new_line: bool) -> 'LogEntry':
         """Create the entry as info entry."""
-        return cls(start_time=start_time, end_time=end_time, device_name=device_name, log_string_info=log_string_info, log_string=log_string, add_new_line=add_new_line, error=False, raw=False, binary=True)
+        return cls(start_time=start_time, end_time=end_time, device_name=device_name, log_string_info=log_string_info, log_string=log_string, cmd=cmd, add_new_line=add_new_line, error=False, raw=False, binary=True)
 
     def set_timestamp_reference_time(self, ref_time: datetime):
         """Sets reference time for the start time. None (default value) means the start time is absolute."""
         self._timestamp_reference_time = ref_time
 
     def get_resolved_content(self, template: str, encoding: str) -> str:
         """Returns the resolved content. For raw entry it means only the log_string."""
@@ -95,24 +96,22 @@
                 value = value.rjust(spaces) if pos_left else value.ljust(spaces)
                 content = content[:m.start()] + value + content[m.end():]
                 continue
             m = self._var_re.search(content)
             if m:
                 var_name = m.group(1)
                 value = self._get_log_string_variable_values(var_name)
-                if not value:
-                    print(f'Value: {value} var_name "{var_name}" log_info: {self._log_string_info}')
                 content = content[:m.start()] + value + content[m.end():]
                 continue
             break
         return content
 
     def _get_log_string_variable_values(self, name: str) -> str:
         """Returns the required variable value.
-        Recognised names: START_TIME, END_TIME, DURATION, DEVICE_NAME, LOG_STRING_INFO, LOG_STRING"""
+        Recognised names: START_TIME, END_TIME, DURATION, DEVICE_NAME, LOG_STRING_INFO, LOG_STRING, SCPI_COMMAND"""
         if name == 'START_TIME':
             if self._start_time is None:
                 return ''
             if self._timestamp_reference_time is None:
                 return get_timestamp_string(self._start_time)
             else:
                 return get_timedelta_fixed_string(self._timestamp_reference_time, self._start_time)
@@ -130,14 +129,18 @@
             return self._device_name
         if name == 'LOG_STRING_INFO':
             if self._log_string_info is None:
                 return ''
             return self._log_string_info
         if name == 'LOG_STRING':
             return self._log_string
+        if name == 'SCPI_COMMAND':
+            if self._cmd is None:
+                return ''
+            return self._cmd
 
 
 class Segment:
     """Segment of logs"""
 
     def __init__(self):
         self.error_present = False
@@ -278,15 +281,17 @@
                 # If error mode is on, and the segment contains at least one error entry, write the segment entries to the log
                 for entry in curr_segment.entries:
                     self._write_to_log(entry)
 
     def set_format_string(self, value: str, line_divider: str = '\n') -> None:
         """Sets new format string and line divider.
         If you just want to set the line divider, set the format string value=None
-        The original format string is: ``PAD_LEFT12(%START_TIME%) PAD_LEFT25(%DEVICE_NAME%) PAD_LEFT12(%DURATION%)  %LOG_STRING_INFO%: %LOG_STRING%`` """
+        The original format string is: ``PAD_LEFT12(%START_TIME%) PAD_LEFT25(%DEVICE_NAME%) PAD_LEFT12(%DURATION%)  %LOG_STRING_INFO%: %LOG_STRING%``\n
+        Additional variables to use: ``%SCPI_COMMAND%``."""
+
         if value is not None:
             self._format_string = value
         self._line_divider = line_divider
 
     def restore_format_string(self) -> None:
         """Restores the original format string and the line divider to LF """
         self._format_string = 'PAD_LEFT12(%START_TIME%) PAD_LEFT30(%DEVICE_NAME%) PAD_LEFT12(%DURATION%)  %LOG_STRING_INFO%: %LOG_STRING%'
@@ -393,15 +398,15 @@
     @log_status_check_ok.setter
     def log_status_check_ok(self, value: bool) -> None:
         """Sets new logging of status checking OK.
         If True (default), the log contains logging of the status checking 'Status check: OK'.
         If False, the 'Status check: OK' is skipped - the log is more compact.
         Errors will still be logged."""
         self._log_status_check_ok = value
-        self.info(datetime.now(), None, 'Logging of \'Status Check OK\'', 'ON' if value is True else 'OFF')
+        self.info(datetime.now(), None, 'Logging of \'Status Check OK\'', 'ON' if value is True else 'OFF', None)
 
     @property
     def log_to_console(self) -> bool:
         """Returns logging to console status."""
         return self._log_to_console
 
     @log_to_console.setter
@@ -507,15 +512,15 @@
             self._segment.add_to_segment(entry)
             return
         if not self._target_exists():
             # No target is defined yet, cache the entries internally for now
             self._cached.append(entry)
             return
 
-        # only now, before writing to the log target, resolve the content.
+        # Only now, before writing to the log target, resolve the content.
         entry.set_timestamp_reference_time(self.get_relative_timestamp())
         content = entry.get_resolved_content(self._format_string, self.encoding)
 
         if self.log_to_console:
             print(content)
         if self.log_to_udp:
             self._send_to_udp(content, entry.error)
@@ -561,44 +566,44 @@
         if self._mode == LoggingMode.Errors:
             # For errors logging mode, log the info only if the segment is active.
             # That means, it might be logged eventually as a context when the segment ends with an error
             if not self._segment:
                 return
         self._write_to_log(log_entry)
 
-    def info(self, start_time: datetime or float or None, end_time: datetime or float or None, log_string_info: str, log_string: str) -> None:
+    def info(self, start_time: datetime or float or None, end_time: datetime or float or None, log_string_info: str, log_string: str, cmd: str or None) -> None:
         """Method for logging one info entry. For binary log_string, use the info_bin()"""
         if self.mode == LoggingMode.Off:
             return
-        entry = self._compose_log_entry(start_time, end_time, log_string_info, log_string, self.abbreviated_max_len_ascii)
+        entry = self._compose_log_entry(start_time, end_time, log_string_info, log_string, cmd, self.abbreviated_max_len_ascii)
         entry.add_new_line = True
         self._info_as_raw_entry(entry)
 
-    def info_bin(self, start_time: datetime or float or None, end_time: datetime or float or None, log_string_info: str, log_data: bytes) -> None:
+    def info_bin(self, start_time: datetime or float or None, end_time: datetime or float or None, log_string_info: str, cmd: str or None, log_data: bytes) -> None:
         """Method for logging one info entry where the log_data is binary (bytes)."""
         if self.mode == LoggingMode.Off:
             return
-        entry = self._compose_bin_log_entry(start_time, end_time, log_string_info, log_data)
+        entry = self._compose_bin_log_entry(start_time, end_time, log_string_info, cmd, log_data)
         entry.add_new_line = True
         self._info_as_raw_entry(entry)
 
-    def info_list(self, start_time: datetime or float or None, end_time: datetime or float or None, log_string_info: str, list_data: List) -> None:
+    def info_list(self, start_time: datetime or float or None, end_time: datetime or float or None, log_string_info: str, cmd: str or None, list_data: List) -> None:
         """Method for logging one info entry where the list_data is decimal List[]."""
         if self.mode == LoggingMode.Off:
             return
         delimiter = ', '
         if len(list_data) <= self.abbreviated_max_len_list:
             log_string = f'List size {len(list_data)}: {list_to_csv_str(list_data, delimiter=delimiter)}'
         else:
             chunk = self.abbreviated_max_len_list // 2
             log_string = f'List size {len(list_data)}, showing first and last {chunk} elements: '
             log_string += list_to_csv_str(list_data[:chunk], delimiter=delimiter)
             log_string += ' .... '
             log_string += list_to_csv_str(list_data[-chunk:], delimiter=delimiter)
-        entry = self._compose_log_entry(start_time, end_time, log_string_info, log_string, max_log_string_len=None)
+        entry = self._compose_log_entry(start_time, end_time, log_string_info, log_string, cmd, max_log_string_len=None)
         entry.add_new_line = True
         self._info_as_raw_entry(entry)
 
     def error_raw(self, log_entry: str, add_new_line: bool = True) -> None:
         """Method for logging one error entry without any formatting. Setting the error flag to True."""
         if self.mode == LoggingMode.Off:
             return
@@ -613,19 +618,19 @@
             return
         if self._segment:
             self._segment.error_present = True
         log_entry.error = True
         log_entry.add_new_line = True
         self._write_to_log(log_entry)
 
-    def error(self, start_time: datetime or float or None, end_time: datetime or float or None, log_string_info: str, log_string: str) -> None:
+    def error(self, start_time: datetime or float or None, end_time: datetime or float or None, log_string_info: str, log_string: str, cmd: str or None) -> None:
         """Method for logging one error entry."""
         if self.mode == LoggingMode.Off:
             return
-        entry = self._compose_log_entry(start_time, end_time, log_string_info, log_string, self.abbreviated_max_len_ascii)
+        entry = self._compose_log_entry(start_time, end_time, log_string_info, log_string, cmd, self.abbreviated_max_len_ascii)
         self._error_as_raw_entry(entry)
 
     def _adjust_log_strings(self, value: str) -> str:
         """Adjusts the log string to prevent repeating of the information in the fields."""
         # Prevent repeating of the device name:
         if self.allow_log_string_adjust and 'DEVICE_NAME' in self._format_string:
             value = value.replace(f"'{self._orig_resource_name}': ", '')
@@ -639,33 +644,33 @@
         if 'LOG_STRING_INFO' in self._format_string:
             log_string = log_string.replace(f'{log_string_info}: ', '')
             log_string = log_string.replace(f'{log_string_info} ', '')
             log_string = log_string.replace(f'{log_string_info}', '')
             log_string = log_string.replace(log_string_info, '')
         return log_string
 
-    def _compose_log_entry(self, start_time: datetime or float, end_time: datetime or float, log_string_info: str, log_string: str, max_log_string_len: int = None) -> LogEntry:
+    def _compose_log_entry(self, start_time: datetime or float, end_time: datetime or float, log_string_info: str, log_string: str, cmd: str or None, max_log_string_len: int = None) -> LogEntry:
         """Composes the log string with the format defined in the self._format_string"""
         log_string_info = self._adjust_log_strings(log_string_info)
         log_string = self._adjust_log_strings(log_string)
         log_string = self._adjust_for_repeated_log_string_info(log_string_info, log_string)
         orig_len = len(log_string)
         # Shorten the long log strings
         if max_log_string_len is not None:
             if orig_len > self.abbreviated_max_len_ascii:
                 log_string = shorten_string_middle(log_string, max_log_string_len)
-        entry = LogEntry(start_time, end_time, self.device_name, log_string_info, log_string, add_new_line=False, error=False, raw=False, binary=False)
+        entry = LogEntry(start_time, end_time, self.device_name, log_string_info, log_string, cmd, add_new_line=False, error=False, raw=False, binary=False)
         return entry
 
-    def _compose_bin_log_entry(self, start_time: datetime or float, end_time: datetime or float, log_string_info: str, log_data: bytes) -> LogEntry:
+    def _compose_bin_log_entry(self, start_time: datetime or float, end_time: datetime or float, log_string_info: str, cmd: str or None, log_data: bytes) -> LogEntry:
         """Composes the binary log string with the format defined in the self._format_string"""
         log_string_info = self._adjust_log_strings(log_string_info)
         log_string_info = escape_nonprintable_chars(log_string_info, self.encoding)
         log_string = self._compose_hexdump(log_data, offset_left=20)
-        entry = LogEntry(start_time, end_time, self.device_name, log_string_info, log_string, add_new_line=False, error=False, raw=False, binary=True)
+        entry = LogEntry(start_time, end_time, self.device_name, log_string_info, log_string, cmd, add_new_line=False, error=False, raw=False, binary=True)
         return entry
 
     def _compose_hexdump(self, value: str or bytes, offset_left: int) -> str:
         """Composes hexdump string from string or bytes.
         The hex dump is organised in the groups of 16 bytes per line."""
         if isinstance(value, str):
             value = bytes(value, self.encoding)
```

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/StreamReader.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/StreamReader.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/StreamWriter.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/StreamWriter.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/StructBase.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/StructBase.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/Types.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/Types.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/VisaPluginSocketIo.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/VisaPluginSocketIo.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/VisaSession.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/VisaSession.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/VisaSessionSim.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/Internal/VisaSessionSim.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/RsCMPX_Gprf.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/RsCMPX_Gprf.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from . import repcap
 from .Internal.RepeatedCapability import RepeatedCapability
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class RsCMPX_Gprf:
 	"""859 total commands, 16 Subgroups, 0 group commands"""
-	_driver_options = "SupportedInstrModels = CMX/CMP/CMW/PVT, SupportedIdnPatterns = CMX/CMP/CMW/PVT, SimulationIdnString = 'Rohde&Schwarz,CMX500,100001,5.0.91.0048'"
+	_driver_options = "SupportedInstrModels = CMX/CMP/CMW/PVT, SupportedIdnPatterns = CMX/CMP/CMW/PVT, SimulationIdnString = 'Rohde&Schwarz,CMX500,100001,5.0.92.0050'"
 	_global_logging_relative_timestamp: ClassVar[datetime] = None
 	_global_logging_target_stream: ClassVar = None
 
 	def __init__(self, resource_name: str, id_query: bool = True, reset: bool = False, options: str = None, direct_session: object = None):
 		"""Initializes new RsCMPX_Gprf session. \n
 		Parameter options tokens examples:
 			- ``Simulate=True`` - starts the session in simulation mode. Default: ``False``
@@ -44,15 +44,15 @@
 			- ``LoggingUdpPort = 49200`` - UDP port to log to. Default: 49200
 		:param resource_name: VISA resource name, e.g. 'TCPIP::192.168.2.1::INSTR'
 		:param id_query: if True, the instrument's model name is verified against the models supported by the driver and eventually throws an exception.
 		:param reset: Resets the instrument (sends *RST command) and clears its status sybsystem.
 		:param options: string tokens alternating the driver settings.
 		:param direct_session: Another driver object or pyVisa object to reuse the session instead of opening a new session."""
 		self._core = Core(resource_name, id_query, reset, RsCMPX_Gprf._driver_options, options, direct_session)
-		self._core.driver_version = '5.0.91.0048'
+		self._core.driver_version = '5.0.92.0050'
 		self._options = options
 		self._add_all_global_repcaps()
 		self._custom_properties_init()
 		self.utilities.default_instrument_setup()
 		# noinspection PyTypeChecker
 		self._cmd_group = CommandsGroup("ROOT", self._core, None)
 
@@ -124,25 +124,25 @@
 		self._core.io.reset_time_statistics()
 
 	@staticmethod
 	def assert_minimum_version(min_version: str) -> None:
 		"""Asserts that the driver version fulfills the minimum required version you have entered.
 		This way you make sure your installed driver is of the entered version or newer."""
 		min_version_list = min_version.split('.')
-		curr_version_list = '5.0.91.0048'.split('.')
+		curr_version_list = '5.0.92.0050'.split('.')
 		count_min = len(min_version_list)
 		count_curr = len(curr_version_list)
 		count = count_min if count_min < count_curr else count_curr
 		for i in range(count):
 			minimum = int(min_version_list[i])
 			curr = int(curr_version_list[i])
 			if curr > minimum:
 				break
 			if curr < minimum:
-				raise RsInstrException(f"Assertion for minimum RsCMPX_Gprf version failed. Current version: '5.0.91.0048', minimum required version: '{min_version}'")
+				raise RsInstrException(f"Assertion for minimum RsCMPX_Gprf version failed. Current version: '5.0.92.0050', minimum required version: '{min_version}'")
 
 	@staticmethod
 	def list_resources(expression: str = '?*::INSTR', visa_select: str = None) -> List[str]:
 		"""Finds all the resources defined by the expression
 			- '?*' - matches all the available instruments
 			- 'USB::?*' - matches all the USB instruments
 			- 'TCPIP::192?*' - matches all the LAN instruments with the IP address starting with 192
```

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/enums.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/enums.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/repcap.py` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf/repcap.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf.egg-info/PKG-INFO` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RsCMPX-Gprf
-Version: 5.0.91
+Version: 5.0.92
 Summary: CMX/CMP/PVT Global Purpose RF Remote-control module
 Home-page: UNKNOWN
 Author: Rohde & Schwarz GmbH & Co. KG
 License: MIT
 Description: ==================================
          RsCMPX_Gprf
         ==================================
@@ -44,15 +44,19 @@
         
         Examples: https://github.com/Rohde-Schwarz/Examples/
         
         
         Version history
         ----------------
         
-        	Latest release notes summary: Added missing measurement SCPI from MMI sub-system
+        	Latest release notes summary: New Core 1.80.0 with loosened data type assertions for lists
+        
+        	Version 5.0.92
+        		- New Core 1.80.0 with loosened data type assertions for lists
+        		- Corrected parameter for TRIGger:GPRF:GENerator<i>:SEQuencer:ISMeas:SOURce to scalar string
         
         	Version 5.0.91
         		- Added missing measurement SCPI from MMI sub-system
         
         	Version 5.0.90
         		- Update for CMP FW 5.0.90
```

### Comparing `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf.egg-info/SOURCES.txt` & `RsCMPX_Gprf-5.0.92/RsCMPX_Gprf.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -745,14 +745,15 @@
 RsCMPX_Gprf/Internal/ArgSingleList.py
 RsCMPX_Gprf/Internal/ArgSingleSuppressed.py
 RsCMPX_Gprf/Internal/ArgStringComposer.py
 RsCMPX_Gprf/Internal/ArgStruct.py
 RsCMPX_Gprf/Internal/ArgStructList.py
 RsCMPX_Gprf/Internal/ArgStructStringParser.py
 RsCMPX_Gprf/Internal/CommandsGroup.py
+RsCMPX_Gprf/Internal/ContextManagers.py
 RsCMPX_Gprf/Internal/Conversions.py
 RsCMPX_Gprf/Internal/ConverterFromScpiString.py
 RsCMPX_Gprf/Internal/ConverterToScpiString.py
 RsCMPX_Gprf/Internal/Core.py
 RsCMPX_Gprf/Internal/GlobalData.py
 RsCMPX_Gprf/Internal/Instrument.py
 RsCMPX_Gprf/Internal/InstrumentErrors.py
```

### Comparing `RsCMPX_Gprf-5.0.91/setup.py` & `RsCMPX_Gprf-5.0.92/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.rst").read_text()
 
 # This call to setup() does all the work
 setup(
     name="RsCMPX_Gprf",
-    version="5.0.91",
+    version="5.0.92",
     description="CMX/CMP/PVT Global Purpose RF Remote-control module",
     long_description=README,
     long_description_content_type="text/x-rst",
     author="Rohde & Schwarz GmbH & Co. KG",
     copyright="Copyright © Rohde & Schwarz GmbH & Co. KG 2022",
     license="MIT",
     classifiers=['License :: OSI Approved :: MIT License',
```


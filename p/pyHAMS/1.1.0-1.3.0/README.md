# Comparing `tmp/pyHAMS-1.1.0.tar.gz` & `tmp/pyhams-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyHAMS-1.1.0.tar", last modified: Thu Apr 20 14:55:07 2023, max compression
+gzip compressed data, was "pyhams-1.3.0.tar", last modified: Fri May 24 04:15:44 2024, max compression
```

## Comparing `pyHAMS-1.1.0.tar` & `pyhams-1.3.0.tar`

### file list

```diff
@@ -1,130 +1,30 @@
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.899370 pyHAMS-1.1.0/
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.752876 pyHAMS-1.1.0/.github/
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.755646 pyHAMS-1.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)      405 2021-01-10 00:25:16.000000 pyHAMS-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)      301 2021-01-10 00:25:16.000000 pyHAMS-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     1515 2021-01-10 00:25:16.000000 pyHAMS-1.1.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.759926 pyHAMS-1.1.0/.github/workflows/
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3328 2023-04-19 11:47:57.000000 pyHAMS-1.1.0/.github/workflows/CI_pyHAMS.yml
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     1829 2021-02-13 18:12:24.000000 pyHAMS-1.1.0/.gitignore
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    11357 2021-02-13 18:08:50.000000 pyHAMS-1.1.0/LICENSE
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     1110 2023-04-20 14:55:07.898883 pyHAMS-1.1.0/PKG-INFO
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)       81 2022-12-27 22:37:17.000000 pyHAMS-1.1.0/README.md
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)      143 2023-01-11 22:31:20.000000 pyHAMS-1.1.0/environment.yml
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     2285 2023-01-31 19:39:18.000000 pyHAMS-1.1.0/meson.build
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.742425 pyHAMS-1.1.0/meson_build/
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.760665 pyHAMS-1.1.0/meson_build/meson-logs/
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    12433 2023-04-20 14:55:02.000000 pyHAMS-1.1.0/meson_build/meson-logs/meson-log.txt
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.762631 pyHAMS-1.1.0/meson_build/meson-private/
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)      156 2023-04-20 14:55:03.000000 pyHAMS-1.1.0/meson_build/meson-private/cmd_line.txt
--rwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    16536 2023-04-20 14:55:00.000000 pyHAMS-1.1.0/meson_build/meson-private/sanitycheckc.exe
--rwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    49832 2023-04-20 14:55:00.000000 pyHAMS-1.1.0/meson_build/meson-private/sanitycheckf.exe
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.763310 pyHAMS-1.1.0/meson_build/pyhams/
--rwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)   324864 2023-04-20 14:55:07.000000 pyHAMS-1.1.0/meson_build/pyhams/_hams.cpython-310-darwin.so
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)      704 2023-01-11 22:31:27.000000 pyHAMS-1.1.0/meson_options.txt
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.767635 pyHAMS-1.1.0/pyHAMS.egg-info/
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     1110 2023-04-20 14:55:07.000000 pyHAMS-1.1.0/pyHAMS.egg-info/PKG-INFO
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3819 2023-04-20 14:55:07.000000 pyHAMS-1.1.0/pyHAMS.egg-info/SOURCES.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        1 2023-04-20 14:55:07.000000 pyHAMS-1.1.0/pyHAMS.egg-info/dependency_links.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        1 2023-03-08 22:58:11.000000 pyHAMS-1.1.0/pyHAMS.egg-info/not-zip-safe
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)       40 2023-04-20 14:55:07.000000 pyHAMS-1.1.0/pyHAMS.egg-info/requires.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)       44 2023-04-20 14:55:07.000000 pyHAMS-1.1.0/pyHAMS.egg-info/top_level.txt
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.773704 pyHAMS-1.1.0/pyhams/
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2021-02-13 17:30:28.000000 pyHAMS-1.1.0/pyhams/__init__.py
--rwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)   324864 2023-04-20 14:55:07.000000 pyHAMS-1.1.0/pyhams/_hams.cpython-310-darwin.so
--rwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)   309480 2023-03-08 22:58:10.000000 pyHAMS-1.1.0/pyhams/_hams.cpython-39-darwin.so
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.787786 pyHAMS-1.1.0/pyhams/bin/
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217) 10156032 2023-04-20 14:32:27.000000 pyHAMS-1.1.0/pyhams/bin/HAMS_x64.exe
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)  2030632 2023-03-08 22:48:24.000000 pyHAMS-1.1.0/pyhams/bin/libiomp5md.dll
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     2527 2023-01-11 22:31:27.000000 pyHAMS-1.1.0/pyhams/meson.build
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    14056 2023-03-08 22:44:54.000000 pyHAMS-1.1.0/pyhams/pyhams.py
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.815487 pyHAMS-1.1.0/pyhams/src/
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    10733 2021-05-21 13:02:25.000000 pyHAMS-1.1.0/pyhams/src/AssbMatx.f90
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    16701 2021-05-21 13:02:25.000000 pyHAMS-1.1.0/pyhams/src/AssbMatx_irr.f90
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     5729 2021-05-21 13:02:25.000000 pyHAMS-1.1.0/pyhams/src/BodyIntgr.f90
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     6734 2022-12-26 09:45:59.000000 pyHAMS-1.1.0/pyhams/src/BodyIntgr_irr.f90
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     6772 2021-05-21 13:02:25.000000 pyHAMS-1.1.0/pyhams/src/CalGreenFunc.f90
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    91497 2021-05-21 13:02:25.000000 pyHAMS-1.1.0/pyhams/src/FinGreen3D.f90
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    28795 2022-12-27 21:20:45.000000 pyHAMS-1.1.0/pyhams/src/FinGrnExtSubs.f90
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    11834 2022-12-27 21:20:45.000000 pyHAMS-1.1.0/pyhams/src/HAMS_Prog.f90
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3180 2022-12-27 21:20:45.000000 pyHAMS-1.1.0/pyhams/src/HydroStatic.f90
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     4203 2022-12-26 09:45:59.000000 pyHAMS-1.1.0/pyhams/src/ImplementSubs.f90
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    22260 2023-04-20 14:32:27.000000 pyHAMS-1.1.0/pyhams/src/InfGreen_Appr.f90
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    15374 2022-12-26 09:45:59.000000 pyHAMS-1.1.0/pyhams/src/InputFiles.f90
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    13486 2021-05-21 13:02:25.000000 pyHAMS-1.1.0/pyhams/src/NormalProcess.f90
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3884 2022-12-26 09:45:59.000000 pyHAMS-1.1.0/pyhams/src/PatclVelct.f90
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     7942 2023-04-20 14:32:27.000000 pyHAMS-1.1.0/pyhams/src/PotentWavForce.f90
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    11927 2021-07-02 11:21:19.000000 pyHAMS-1.1.0/pyhams/src/PressureElevation.f90
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     9423 2021-05-21 13:02:25.000000 pyHAMS-1.1.0/pyhams/src/PrintOutput.f90
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     4232 2022-12-26 09:45:59.000000 pyHAMS-1.1.0/pyhams/src/ReadPanelMesh.f90
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    26614 2021-05-21 13:02:25.000000 pyHAMS-1.1.0/pyhams/src/SingularIntgr.f90
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3588 2021-05-21 13:33:46.000000 pyHAMS-1.1.0/pyhams/src/SolveMotion.f90
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     6201 2021-05-21 17:28:25.000000 pyHAMS-1.1.0/pyhams/src/WavDynMods.f90
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     4176 2021-05-21 13:02:25.000000 pyHAMS-1.1.0/pyhams/src/WavDynSubs.f90
--rwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)   433808 2023-04-20 14:33:28.000000 pyHAMS-1.1.0/pyhams/src/libhams.so
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     2480 2023-01-11 22:31:20.000000 pyHAMS-1.1.0/pyhams/src/makefile
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3766 2023-04-20 14:45:33.000000 pyHAMS-1.1.0/pyproject.toml
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)       38 2023-04-20 14:55:07.899531 pyHAMS-1.1.0/setup.cfg
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     6126 2023-04-20 14:46:00.000000 pyHAMS-1.1.0/setup.py
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.816552 pyHAMS-1.1.0/test/
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.745926 pyHAMS-1.1.0/test/Cylinder/
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.820913 pyHAMS-1.1.0/test/Cylinder/Input/
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)      890 2023-03-08 23:20:50.000000 pyHAMS-1.1.0/test/Cylinder/Input/ControlFile.in
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    29427 2022-12-27 22:37:07.000000 pyHAMS-1.1.0/test/Cylinder/Input/HullMesh.pnl
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     2801 2023-03-08 23:20:50.000000 pyHAMS-1.1.0/test/Cylinder/Input/Hydrostatic.in
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    13455 2022-12-27 22:37:07.000000 pyHAMS-1.1.0/test/Cylinder/Input/WaterplaneMesh.pnl
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.822088 pyHAMS-1.1.0/test/Cylinder/Output/
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)      105 2023-03-08 23:20:54.000000 pyHAMS-1.1.0/test/Cylinder/Output/ErrorCheck.txt
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.849227 pyHAMS-1.1.0/test/Cylinder/Output/Hams_format/
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:54.000000 pyHAMS-1.1.0/test/Cylinder/Output/Hams_format/OAMASS1.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:54.000000 pyHAMS-1.1.0/test/Cylinder/Output/Hams_format/OAMASS2.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:54.000000 pyHAMS-1.1.0/test/Cylinder/Output/Hams_format/OAMASS3.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:54.000000 pyHAMS-1.1.0/test/Cylinder/Output/Hams_format/OAMASS4.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:54.000000 pyHAMS-1.1.0/test/Cylinder/Output/Hams_format/OAMASS5.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:54.000000 pyHAMS-1.1.0/test/Cylinder/Output/Hams_format/OAMASS6.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:54.000000 pyHAMS-1.1.0/test/Cylinder/Output/Hams_format/ODAMPING1.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:54.000000 pyHAMS-1.1.0/test/Cylinder/Output/Hams_format/ODAMPING2.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:54.000000 pyHAMS-1.1.0/test/Cylinder/Output/Hams_format/ODAMPING3.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:54.000000 pyHAMS-1.1.0/test/Cylinder/Output/Hams_format/ODAMPING4.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:54.000000 pyHAMS-1.1.0/test/Cylinder/Output/Hams_format/ODAMPING5.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:54.000000 pyHAMS-1.1.0/test/Cylinder/Output/Hams_format/ODAMPING6.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    51840 2023-03-08 23:20:54.000000 pyHAMS-1.1.0/test/Cylinder/Output/Hams_format/OEXFOR1.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    51840 2023-03-08 23:20:54.000000 pyHAMS-1.1.0/test/Cylinder/Output/Hams_format/OEXFOR2.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    51840 2023-03-08 23:20:54.000000 pyHAMS-1.1.0/test/Cylinder/Output/Hams_format/OEXFOR3.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    51840 2023-03-08 23:20:54.000000 pyHAMS-1.1.0/test/Cylinder/Output/Hams_format/OEXFOR4.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    51840 2023-03-08 23:20:54.000000 pyHAMS-1.1.0/test/Cylinder/Output/Hams_format/OEXFOR5.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    51840 2023-03-08 23:20:54.000000 pyHAMS-1.1.0/test/Cylinder/Output/Hams_format/OEXFOR6.txt
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.860069 pyHAMS-1.1.0/test/Cylinder/truth/
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    59400 2023-03-08 23:20:44.000000 pyHAMS-1.1.0/test/Cylinder/truth/Buoy.1
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)   589680 2023-03-08 23:16:49.000000 pyHAMS-1.1.0/test/Cylinder/truth/Buoy.3
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)   589680 2023-03-08 23:16:49.000000 pyHAMS-1.1.0/test/Cylinder/truth/Buoy.4
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2022-12-22 09:42:02.000000 pyHAMS-1.1.0/test/Cylinder/truth/Buoy.6p
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     1044 2023-03-08 23:16:49.000000 pyHAMS-1.1.0/test/Cylinder/truth/Buoy.hst
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.746735 pyHAMS-1.1.0/test/Cylinder_headings/
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.864069 pyHAMS-1.1.0/test/Cylinder_headings/Input/
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)      877 2023-03-08 23:20:54.000000 pyHAMS-1.1.0/test/Cylinder_headings/Input/ControlFile.in
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    29427 2023-03-08 22:44:54.000000 pyHAMS-1.1.0/test/Cylinder_headings/Input/HullMesh.pnl
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     2801 2023-03-08 23:20:54.000000 pyHAMS-1.1.0/test/Cylinder_headings/Input/Hydrostatic.in
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    13455 2023-03-08 22:44:54.000000 pyHAMS-1.1.0/test/Cylinder_headings/Input/WaterplaneMesh.pnl
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.864990 pyHAMS-1.1.0/test/Cylinder_headings/Output/
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)      105 2023-03-08 23:20:58.000000 pyHAMS-1.1.0/test/Cylinder_headings/Output/ErrorCheck.txt
-drwxr-xr-x   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)        0 2023-04-20 14:55:07.897654 pyHAMS-1.1.0/test/Cylinder_headings/Output/Hams_format/
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:58.000000 pyHAMS-1.1.0/test/Cylinder_headings/Output/Hams_format/OAMASS1.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:58.000000 pyHAMS-1.1.0/test/Cylinder_headings/Output/Hams_format/OAMASS2.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:58.000000 pyHAMS-1.1.0/test/Cylinder_headings/Output/Hams_format/OAMASS3.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:58.000000 pyHAMS-1.1.0/test/Cylinder_headings/Output/Hams_format/OAMASS4.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:58.000000 pyHAMS-1.1.0/test/Cylinder_headings/Output/Hams_format/OAMASS5.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:58.000000 pyHAMS-1.1.0/test/Cylinder_headings/Output/Hams_format/OAMASS6.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:58.000000 pyHAMS-1.1.0/test/Cylinder_headings/Output/Hams_format/ODAMPING1.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:58.000000 pyHAMS-1.1.0/test/Cylinder_headings/Output/Hams_format/ODAMPING2.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:58.000000 pyHAMS-1.1.0/test/Cylinder_headings/Output/Hams_format/ODAMPING3.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:58.000000 pyHAMS-1.1.0/test/Cylinder_headings/Output/Hams_format/ODAMPING4.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:58.000000 pyHAMS-1.1.0/test/Cylinder_headings/Output/Hams_format/ODAMPING5.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     3232 2023-03-08 23:20:58.000000 pyHAMS-1.1.0/test/Cylinder_headings/Output/Hams_format/ODAMPING6.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    10080 2023-03-08 23:20:58.000000 pyHAMS-1.1.0/test/Cylinder_headings/Output/Hams_format/OEXFOR1.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    10080 2023-03-08 23:20:58.000000 pyHAMS-1.1.0/test/Cylinder_headings/Output/Hams_format/OEXFOR2.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    10080 2023-03-08 23:20:58.000000 pyHAMS-1.1.0/test/Cylinder_headings/Output/Hams_format/OEXFOR3.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    10080 2023-03-08 23:20:58.000000 pyHAMS-1.1.0/test/Cylinder_headings/Output/Hams_format/OEXFOR4.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    10080 2023-03-08 23:20:58.000000 pyHAMS-1.1.0/test/Cylinder_headings/Output/Hams_format/OEXFOR5.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)    10080 2023-03-08 23:20:58.000000 pyHAMS-1.1.0/test/Cylinder_headings/Output/Hams_format/OEXFOR6.txt
--rw-r--r--   0 gbarter  (1797763346) NREL_NT\Domain Users (18434217)     5209 2023-03-08 23:52:44.000000 pyHAMS-1.1.0/test/test_cylinder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 04:15:44.205446 pyhams-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 04:15:28.000000 pyhams-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-24 04:15:44.205446 pyhams-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-24 04:15:28.000000 pyhams-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 04:15:44.197446 pyhams-1.3.0/meson_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 04:15:44.201446 pyhams-1.3.0/meson_build/meson-logs/
+-rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-05-24 04:15:40.000000 pyhams-1.3.0/meson_build/meson-logs/meson-log.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 04:15:44.201446 pyhams-1.3.0/meson_build/meson-private/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-24 04:15:40.000000 pyhams-1.3.0/meson_build/meson-private/cmd_line.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-24 04:15:40.000000 pyhams-1.3.0/meson_build/meson-private/pycompile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15784 2024-05-24 04:15:40.000000 pyhams-1.3.0/meson_build/meson-private/sanitycheckc.exe
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16216 2024-05-24 04:15:40.000000 pyhams-1.3.0/meson_build/meson-private/sanitycheckf.exe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 04:15:44.201446 pyhams-1.3.0/meson_build/pyhams/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   649848 2024-05-24 04:15:44.000000 pyhams-1.3.0/meson_build/pyhams/_hams.cpython-310-x86_64-linux-gnu.so
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 04:15:44.205446 pyhams-1.3.0/pyHAMS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-24 04:15:44.000000 pyhams-1.3.0/pyHAMS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-24 04:15:44.000000 pyhams-1.3.0/pyHAMS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 04:15:44.000000 pyhams-1.3.0/pyHAMS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 04:15:40.000000 pyhams-1.3.0/pyHAMS.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-24 04:15:44.000000 pyhams-1.3.0/pyHAMS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-24 04:15:44.000000 pyhams-1.3.0/pyHAMS.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 04:15:44.205446 pyhams-1.3.0/pyhams/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 04:15:28.000000 pyhams-1.3.0/pyhams/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   649848 2024-05-24 04:15:44.000000 pyhams-1.3.0/pyhams/_hams.cpython-310-x86_64-linux-gnu.so
+-rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-05-24 04:15:28.000000 pyhams-1.3.0/pyhams/pyhams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-24 04:15:28.000000 pyhams-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 04:15:44.205446 pyhams-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-24 04:15:28.000000 pyhams-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 04:15:44.205446 pyhams-1.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-24 04:15:28.000000 pyhams-1.3.0/test/test_cylinder.py
```

### Comparing `pyHAMS-1.1.0/LICENSE` & `pyhams-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyHAMS-1.1.0/pyhams/pyhams.py` & `pyhams-1.3.0/pyhams/pyhams.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import os
 import os.path as osp
-import platform
 import numpy as np
 
-if not platform.system() == 'Windows':
-    import pyhams._hams as hams
-else:
-    import subprocess as sub
+import pyhams._hams as hams
 
 def nemohmesh_to_pnl(nemohMeshPath, writeDir=None):
     '''
     convert mesh from .nemoh format to HAMS .pnl format
 
     Parameters
     ----------
@@ -321,21 +317,25 @@
 def read_wamit1(pathWamit1, TFlag=0):
     '''
     Read added mass and damping from .1 file (WAMIT format)
     '''
     pathWamit1 = osp.normpath(pathWamit1)
     # Check if the file contains the infinite and zero frequency points
     try:
-        freq_test = np.loadtxt(pathWamit1, usecols=(0,1,2,3), max_rows=72)
-        if np.array_equal(np.unique(freq_test[:,0]), np.array([-1.0, 0.0])):
-            other_freqs = np.loadtxt(pathWamit1, usecols=(0,1,2,3,4), skiprows=72)
-            freq_test   = np.c_[freq_test, np.nan*np.ones(72)]
-            wamit1      = np.vstack((freq_test, other_freqs))
-        else:
-            wamit1 = np.loadtxt(pathWamit1)
+        # extract the first 72 rows to see how many are infinite and zero
+        freq_test = np.loadtxt(pathWamit1, usecols=(0,1,2,3), max_rows=73)  # add one extra (73) for formatting/syntax
+        # find the row in the file that is not a zero or infinite frequency
+        for i in range(len(freq_test)):     
+            if freq_test[i,0] != 0.0 and freq_test[i,0] != -1.0:
+                break
+        # create new arrays based on the number of nonzero values in the matrices
+        inf_zero_freqs = np.loadtxt(pathWamit1, usecols=(0,1,2,3), max_rows=i)
+        other_freqs = np.loadtxt(pathWamit1, usecols=(0,1,2,3,4), skiprows=i)
+        inf_zero_freqs_full   = np.c_[inf_zero_freqs, np.nan*np.ones(i)]
+        wamit1      = np.vstack((inf_zero_freqs_full, other_freqs))
     except:
         wamit1 = np.loadtxt(pathWamit1)
 
     # Get unique frequencies and index vector
     w, iw = np.unique(wamit1[:,0], return_inverse=True)
     nfreq = len(w)
     
@@ -396,22 +396,14 @@
     phase[ih, idx, iw] = phaseCol
     real[ ih, idx, iw] = realCol
     imag[ ih, idx, iw] = imagCol
     
     return mod, phase, real, imag, w, headings
 
 def run_hams(projectDir):
-    '''call the HAMS_x64.exe program in the specified project directory'''
-    # get absolute path to the local HAMS_x64.exe program
-    hamsDir = osp.dirname(__file__)
-    hamsExe = './bin/HAMS_x64.exe'
-    hamsPath = osp.abspath(osp.join(hamsDir, hamsExe))
     # change directory to where the HAMS input files are
     workingDir = os.getcwd()
     os.chdir(projectDir)
     # run HAMS
-    if platform.system() == 'Windows':
-        sub.run([f'{hamsPath}'])
-    else:
-        hams.hams_full.exec()
+    hams.hams_full.exec()
     # change back to working directory
     os.chdir(workingDir)
```

### Comparing `pyHAMS-1.1.0/pyproject.toml` & `pyhams-1.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools", "meson>=1.1", "numpy", "ninja", "wheel"]
+requires = ["setuptools", "numpy", "ninja", "meson>=1.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyHAMS"
-version = "1.1.0"
+version = "1.3.0"
 description = "Python module wrapping around HAMS"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "Apache-2.0"}
 keywords = ["wind", "turbine", "mdao", "design", "optimization"]
 authors = [
   {name = "NREL WISDEM Team", email = "systems.engineering@nrel.gov" }
@@ -32,70 +32,79 @@
   # Specify the Python versions you support here. In particular, ensure
   # that you indicate you support Python 3. These classifiers are *not*
   # checked by "pip install". See instead "python_requires" below.
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Fortran",
+  "Operating System :: Microsoft :: Windows",
+  "Operating System :: POSIX :: Linux",
+  "Operating System :: POSIX",
+  "Operating System :: Unix",
+  "Operating System :: MacOS",
 ]
 
 dependencies = [
-  "numpy",
+  "numpy","meson","ninja",
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
 #   $ pip install sampleproject[dev]
 #
 # Similar to `dependencies` above, these must be valid existing
 # projects.
 [project.optional-dependencies] # Optional
-dev = ["meson", "ninja"]
 test = ["pytest"]
 
 # List URLs that are relevant to your project
 #
 # This field corresponds to the "Project-URL" and "Home-Page" metadata fields:
 # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
 # https://packaging.python.org/specifications/core-metadata/#home-page-optional
 #
 # Examples listed include a pattern for specifying where the package tracks
 # issues, where the source is hosted, where to say thanks to the package
 # maintainers, and where to support the project financially. The key is
 # what's used to render the link text on PyPI.
 [project.urls]  # Optional
-"Homepage" = "https://github.com/WISDEM/pyHAMS"
-"Project" = "https://github.com/YingyiLiu/HAMS"
+homepage = "https://github.com/WISDEM/pyHAMS"
+documentation = "https://github.com/YingyiLiu/HAMS"
+source = "https://github.com/WISDEM/pyHAMS"
+download = "https://github.com/WISDEM/pyHAMS/releases"
+tracker = "https://github.com/WISDEM/pyHAMS/issues"
+
+# This is configuration specific to the `meson-python` build backend.
+#[tool.meson-python.args]
+#setup = ['--python.install-env=auto']
+#install = ['--tags=runtime,python-runtime,bin']
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 [tool.setuptools]
 zip-safe = false
 include-package-data = true
 
-#[tool.setuptools.packages]
-#find = {}
-
 [tool.setuptools.packages.find]
-#where = ["wisdem"]
 exclude = ["Cylinder", "test"]
 namespaces = true
 
 [tool.setuptools.package-data]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 "*" = ["*.yaml", "*.xlsx", "*.txt", "*.so", "*.lib", "*.pyd", "*.pdb", "*.dylib", "*.dll", "*.exe"]
 
 [tool.black]
 line-length = 120
-target-version = ['py39']
+target-version = ['py311']
 include = '\.pyi?$'
 exclude = '''
 /(
     \.git
   | \.hg
   | \.mypy_cache
   | \.tox
@@ -121,9 +130,23 @@
 skip_glob = ['__init__.py']
 atomic = true
 #lines_after_imports = 2
 #lines_between_types = 1
 #src_paths=isort,test
 
 [tool.cibuildwheel]
-skip = ["cp36-*", "cp37-*", "cp38-*", "*-win32", "*arm64", "pp*"]
-build-frontend = "build"
+skip = ["pp*", "cp36-*", "cp37-*", "cp38-*", "*-win32", "*-win_arm64"] #, "*-musllinux*"]
+build-frontend = { name = "build", args = ["-w","-n"] }
+before-build = "pip install numpy ninja meson meson-python setuptools wheel"
+build-verbosity = "3"
+
+# https://github.com/pdfo/pdfo
+[[tool.cibuildwheel.overrides]]
+select = "*-win_amd64"
+environment = { PKG_CONFIG_PATH="c:/opt/64/lib/pkgconfig" }
+
+[tool.cibuildwheel.windows]
+repair-wheel-command = "bash .github/tools/cibw_repair_wheel_command_windows.sh {wheel} {dest_dir}"
+
+# On an Linux Intel runner with qemu installed, build Intel and ARM wheels (aarch64) for Docker.  Ignoring: ppc64le s390x
+[tool.cibuildwheel.linux]
+archs = ["auto", "aarch64"]
```

### Comparing `pyHAMS-1.1.0/test/test_cylinder.py` & `pyhams-1.3.0/test/test_cylinder.py`

 * *Files identical despite different names*


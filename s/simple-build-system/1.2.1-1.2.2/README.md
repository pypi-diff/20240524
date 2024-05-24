# Comparing `tmp/simple_build_system-1.2.1.tar.gz` & `tmp/simple_build_system-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_build_system-1.2.1.tar", last modified: Thu May 23 08:53:48 2024, max compression
+gzip compressed data, was "simple_build_system-1.2.2.tar", last modified: Fri May 24 11:36:15 2024, max compression
```

## Comparing `simple_build_system-1.2.1.tar` & `simple_build_system-1.2.2.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.693988 simple_build_system-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14092 2024-05-23 08:53:48.693988 simple_build_system-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 08:53:48.693988 simple_build_system-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.669988 simple_build_system-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.677988 simple_build_system-1.2.1/src/_simple_build_system/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/_determine_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/_export_jsoncmds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/_sphinxext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/_sphinxutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20990 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/build_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     8493 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/cfgbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/cfglocate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/col.py
--rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/cpudetect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.677988 simple_build_system-1.2.1/src/_simple_build_system/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cfgtemplate.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.681988 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/Detect.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/ExtDep_Python.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/ExtDep_pybind11.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/ExtractFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/Utils.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/WriteResults.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/extract_flags_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.685988 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_ASE.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_DL.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_Fortran.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_Garfield.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_Geant4.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_Gemmi.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_HDF5.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_Mantidpython.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_NCrystal.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_Numpy.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_OSG.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_Pandas.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_Pymatgen.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_ROOT.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_Scipy.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_Spglib.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_Threads.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_ZLib.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_matplotlib.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_mpmath.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.685988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.685988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.685988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/app_cmakebuildtype/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/app_cmakebuildtype/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.685988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libinc/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libinc/FPE.hh
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libinc/File.hh
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libinc/FindData.hh
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libinc/Python.hh
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libinc/String.hh
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libinc/Types.hh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.685988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libsrc/
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libsrc/FPE.cc
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libsrc/File.cc
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libsrc/FindData.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libsrc/String.cc
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libsrc/static_asserts.cc
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/pkg.info
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.685988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/pycpp_FPE/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/pycpp_FPE/mod.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.685988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/pycpp_misc/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/pycpp_misc/mod.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.685988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/python/CpuDetect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/python/FindData.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/python/FindData3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/python/System.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/python/find_libpython.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.689988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3061 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/scripts/extdeps
--rwxr-xr-x   0 runner    (1001) docker     (127)      600 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/scripts/finddata
--rwxr-xr-x   0 runner    (1001) docker     (127)     2825 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/scripts/queryenv
--rwxr-xr-x   0 runner    (1001) docker     (127)     6199 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/scripts/reflogupdate
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/simplebuild.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.689988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.689988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.689988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/app_test/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/app_test/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.689988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/libsrc/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/libsrc/sometest.cc
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/pkg.info
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.689988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.689988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_build_is_debug/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_build_is_debug/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.689988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_forcefpe/
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_forcefpe/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.689988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testfile/
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testfile/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.689988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testformat/
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testformat/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.689988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testpycpp/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testpycpp/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.689988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testsdk/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testsdk/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.689988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_teststring/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_teststring/main.cc
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/pkg.info
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.689988 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      691 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testfpe
--rwxr-xr-x   0 runner    (1001) docker     (127)     1279 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testlibsymbols
--rwxr-xr-x   0 runner    (1001) docker     (127)     1180 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testnodostxt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1824 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testpylibsymbols
--rwxr-xr-x   0 runner    (1001) docker     (127)       96 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testpyquery
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/simplebuild.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.689988 simple_build_system-1.2.1/src/_simple_build_system/data/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/resources/shellrc_snippet.sh
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/data/resources/shellrc_snippet_deactivate.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/dirs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/dotgen.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/envcfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/envsetup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/extractenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/find.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/findpkgdirs.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/formatlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    18720 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/grep.py
--rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/incinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/includes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/init_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/instsl.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/instsl2.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/langs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16357 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/loadpkgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/makefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/mtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    13833 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/parse_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/pkgfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/pkgutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/replace.py
--rw-r--r--   0 runner    (1001) docker     (127)    17097 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/singlecfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/target_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/target_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/testlauncher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/testxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/tfact_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/tfact_headerdeps.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/tfact_libavail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/tfact_prepinc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/tfact_pyinit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/tfact_reflogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/tfact_symlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-05-23 08:53:42.000000 simple_build_system-1.2.1/src/_simple_build_system/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:53:48.693988 simple_build_system-1.2.1/src/simple_build_system.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14092 2024-05-23 08:53:48.000000 simple_build_system-1.2.1/src/simple_build_system.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-05-23 08:53:48.000000 simple_build_system-1.2.1/src/simple_build_system.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:53:48.000000 simple_build_system-1.2.1/src/simple_build_system.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-23 08:53:48.000000 simple_build_system-1.2.1/src/simple_build_system.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-23 08:53:48.000000 simple_build_system-1.2.1/src/simple_build_system.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 08:53:48.000000 simple_build_system-1.2.1/src/simple_build_system.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.797889 simple_build_system-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14092 2024-05-24 11:36:15.797889 simple_build_system-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 11:36:15.797889 simple_build_system-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.773889 simple_build_system-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.781889 simple_build_system-1.2.2/src/_simple_build_system/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/_determine_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/_export_jsoncmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/_sphinxext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/_sphinxutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20990 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/build_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8493 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/cfgbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/cfglocate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/col.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/cpudetect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.785889 simple_build_system-1.2.2/src/_simple_build_system/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cfgtemplate.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.785889 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/Detect.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/ExtDep_Python.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/ExtDep_pybind11.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/ExtractFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/Utils.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/WriteResults.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/extract_flags_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.789889 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_ASE.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_DL.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_Fortran.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_Garfield.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_Geant4.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_Gemmi.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_HDF5.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_Mantidpython.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_NCrystal.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_Numpy.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_OSG.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_Pandas.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_Pymatgen.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_ROOT.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_Scipy.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_Spglib.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_Threads.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_ZLib.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_matplotlib.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_mpmath.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.789889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.789889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.789889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/app_cmakebuildtype/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/app_cmakebuildtype/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.789889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libinc/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libinc/FPE.hh
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libinc/File.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libinc/FindData.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libinc/Python.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libinc/String.hh
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libinc/Types.hh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.789889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libsrc/
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libsrc/FPE.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libsrc/File.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libsrc/FindData.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libsrc/String.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libsrc/static_asserts.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/pkg.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.789889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/pycpp_FPE/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/pycpp_FPE/mod.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.789889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/pycpp_misc/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/pycpp_misc/mod.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.793889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/python/CpuDetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/python/FindData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/python/FindData3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/python/System.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/python/find_libpython.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.793889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3061 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/scripts/extdeps
+-rwxr-xr-x   0 runner    (1001) docker     (127)      600 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/scripts/finddata
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2825 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/scripts/queryenv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6199 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/scripts/reflogupdate
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/simplebuild.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.793889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.793889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.793889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/app_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/app_test/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.793889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/libsrc/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/libsrc/sometest.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/pkg.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.793889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.793889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_build_is_debug/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_build_is_debug/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.793889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_forcefpe/
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_forcefpe/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.793889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testfile/
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testfile/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.793889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testformat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testformat/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.793889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testpycpp/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testpycpp/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.793889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testsdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testsdk/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.793889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_teststring/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_teststring/main.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/pkg.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.797889 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      691 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testfpe
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1279 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testlibsymbols
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1180 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testnodostxt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1824 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testpylibsymbols
+-rwxr-xr-x   0 runner    (1001) docker     (127)       96 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testpyquery
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/simplebuild.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.797889 simple_build_system-1.2.2/src/_simple_build_system/data/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/resources/shellrc_snippet.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/data/resources/shellrc_snippet_deactivate.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/dirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/dotgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/envcfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/envsetup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/extractenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/find.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/findpkgdirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/formatlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18720 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/grep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/incinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/includes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/init_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/instsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/instsl2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/langs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16357 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/loadpkgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/mtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13833 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/parse_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/pkgfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/pkgutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/replace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17097 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/singlecfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/target_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/target_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/testlauncher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/testxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/tfact_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/tfact_headerdeps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/tfact_libavail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/tfact_prepinc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/tfact_pyinit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/tfact_reflogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/tfact_symlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-05-24 11:36:09.000000 simple_build_system-1.2.2/src/_simple_build_system/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:36:15.797889 simple_build_system-1.2.2/src/simple_build_system.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14092 2024-05-24 11:36:15.000000 simple_build_system-1.2.2/src/simple_build_system.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-05-24 11:36:15.000000 simple_build_system-1.2.2/src/simple_build_system.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 11:36:15.000000 simple_build_system-1.2.2/src/simple_build_system.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-24 11:36:15.000000 simple_build_system-1.2.2/src/simple_build_system.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-24 11:36:15.000000 simple_build_system-1.2.2/src/simple_build_system.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-24 11:36:15.000000 simple_build_system-1.2.2/src/simple_build_system.egg-info/top_level.txt
```

### Comparing `simple_build_system-1.2.1/LICENSE` & `simple_build_system-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/MANIFEST.in` & `simple_build_system-1.2.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/PKG-INFO` & `simple_build_system-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-build-system
-Version: 1.2.1
+Version: 1.2.2
 Summary: A very simple to use build system for projects with primarily C++/Python code, intended for usage by scientific developers without a strong SW-engineering background.
 Author-email: Thomas Kittelmann <thomas.kittelmann@ess.eu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `simple_build_system-1.2.1/pyproject.toml` & `simple_build_system-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/_cli.py` & `simple_build_system-1.2.2/src/_simple_build_system/_cli.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/_export_jsoncmds.py` & `simple_build_system-1.2.2/src/_simple_build_system/_export_jsoncmds.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/_sphinxext.py` & `simple_build_system-1.2.2/src/_simple_build_system/_sphinxext.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/_sphinxutils.py` & `simple_build_system-1.2.2/src/_simple_build_system/_sphinxutils.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/backend.py` & `simple_build_system-1.2.2/src/_simple_build_system/backend.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/build_summary.py` & `simple_build_system-1.2.2/src/_simple_build_system/build_summary.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/cfgbuilder.py` & `simple_build_system-1.2.2/src/_simple_build_system/cfgbuilder.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/cfglocate.py` & `simple_build_system-1.2.2/src/_simple_build_system/cfglocate.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/col.py` & `simple_build_system-1.2.2/src/_simple_build_system/col.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/conf.py` & `simple_build_system-1.2.2/src/_simple_build_system/conf.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/cpudetect.py` & `simple_build_system-1.2.2/src/_simple_build_system/cpudetect.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cfgtemplate.txt` & `simple_build_system-1.2.2/src/_simple_build_system/data/cfgtemplate.txt`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cmake/CMakeLists.txt` & `simple_build_system-1.2.2/src/_simple_build_system/data/cmake/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,16 @@
 endif()
 
 set( sbld_extra_ccxx_cflags "")
 if ( NOT "${CMAKE_BUILD_TYPE}" STREQUAL "Debug" )
   #Aggressively target native platform + a few other optimisations (see also
   #https://github.com/mctools/simplebuild/issues/73). For now we assume the
   #compiler understands all of these:
-  set( sbld_extra_ccxx_cflags "${sbld_extra_ccxx_cflags} -O3 -DNDEBUG -fno-math-errno -march=native -mtune=native")
+  #NB: -march=native -mtune=native changes results in some NCrystal unit tests.
+  set( sbld_extra_ccxx_cflags "${sbld_extra_ccxx_cflags} -O3 -DNDEBUG -fno-math-errno")# -march=native -mtune=native")
   #Disabling -flto for now, I suspect if causes issues on macos...:
   if ( NOT SBLD_ISINTEL )
     #NB: Not adding -flto=auto for now, since we saw some weird errors of uncaught exceptions on macos.
     set( sbld_extra_ccxx_cflags "${sbld_extra_ccxx_cflags} -ftree-vectorize")
   endif()
 endif()
 if ( SBLD_ISINTEL )
```

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cmake/Detect.cmake` & `simple_build_system-1.2.2/src/_simple_build_system/data/cmake/Detect.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cmake/ExtDep_Python.cmake` & `simple_build_system-1.2.2/src/_simple_build_system/data/cmake/ExtDep_Python.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cmake/ExtDep_pybind11.cmake` & `simple_build_system-1.2.2/src/_simple_build_system/data/cmake/ExtDep_pybind11.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cmake/ExtractFlags.cmake` & `simple_build_system-1.2.2/src/_simple_build_system/data/cmake/ExtractFlags.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cmake/Utils.cmake` & `simple_build_system-1.2.2/src/_simple_build_system/data/cmake/Utils.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cmake/WriteResults.cmake` & `simple_build_system-1.2.2/src/_simple_build_system/data/cmake/WriteResults.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cmake/extract_flags_helper.py` & `simple_build_system-1.2.2/src/_simple_build_system/data/cmake/extract_flags_helper.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_DL.cmake` & `simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_DL.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_Fortran.cmake` & `simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_Fortran.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_Garfield.cmake` & `simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_Garfield.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_Geant4.cmake` & `simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_Geant4.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_HDF5.cmake` & `simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_HDF5.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_NCrystal.cmake` & `simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_NCrystal.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_Numpy.cmake` & `simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_Numpy.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_OSG.cmake` & `simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_OSG.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_Pandas.cmake` & `simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_Pandas.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_ROOT.cmake` & `simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_ROOT.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_Scipy.cmake` & `simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_Scipy.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_ZLib.cmake` & `simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_ZLib.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/cmake/optional/ExtDep_matplotlib.cmake` & `simple_build_system-1.2.2/src/_simple_build_system/data/cmake/optional/ExtDep_matplotlib.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libinc/FPE.hh` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libinc/FPE.hh`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libinc/File.hh` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libinc/File.hh`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libinc/FindData.hh` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libinc/FindData.hh`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libinc/Python.hh` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libinc/Python.hh`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libinc/String.hh` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libinc/String.hh`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libinc/Types.hh` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libinc/Types.hh`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libsrc/FPE.cc` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libsrc/FPE.cc`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libsrc/File.cc` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libsrc/File.cc`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libsrc/FindData.cc` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libsrc/FindData.cc`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/libsrc/String.cc` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/libsrc/String.cc`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/pycpp_FPE/mod.cc` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/pycpp_FPE/mod.cc`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/python/CpuDetect.py` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/python/CpuDetect.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/python/FindData.py` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/python/FindData.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/python/FindData3.py` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/python/FindData3.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/python/System.py` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/python/System.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/python/find_libpython.py` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/python/find_libpython.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/scripts/extdeps` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/scripts/extdeps`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/scripts/finddata` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/scripts/finddata`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/scripts/queryenv` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/scripts/queryenv`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core/Core/scripts/reflogupdate` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core/Core/scripts/reflogupdate`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_forcefpe/main.cc` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_forcefpe/main.cc`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testfile/main.cc` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testfile/main.cc`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testformat/main.cc` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testformat/main.cc`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_teststring/main.cc` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_teststring/main.cc`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testfpe` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testfpe`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testlibsymbols` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testlibsymbols`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testnodostxt` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testnodostxt`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testpylibsymbols` & `simple_build_system-1.2.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testpylibsymbols`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/resources/shellrc_snippet.sh` & `simple_build_system-1.2.2/src/_simple_build_system/data/resources/shellrc_snippet.sh`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/data/resources/shellrc_snippet_deactivate.sh` & `simple_build_system-1.2.2/src/_simple_build_system/data/resources/shellrc_snippet_deactivate.sh`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/db.py` & `simple_build_system-1.2.2/src/_simple_build_system/db.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/dirs.py` & `simple_build_system-1.2.2/src/_simple_build_system/dirs.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/dotgen.py` & `simple_build_system-1.2.2/src/_simple_build_system/dotgen.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/envcfg.py` & `simple_build_system-1.2.2/src/_simple_build_system/envcfg.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/envsetup.py` & `simple_build_system-1.2.2/src/_simple_build_system/envsetup.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/error.py` & `simple_build_system-1.2.2/src/_simple_build_system/error.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/extractenv.py` & `simple_build_system-1.2.2/src/_simple_build_system/extractenv.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/find.py` & `simple_build_system-1.2.2/src/_simple_build_system/find.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/formatlist.py` & `simple_build_system-1.2.2/src/_simple_build_system/formatlist.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/frontend.py` & `simple_build_system-1.2.2/src/_simple_build_system/frontend.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/grep.py` & `simple_build_system-1.2.2/src/_simple_build_system/grep.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/incinfo.py` & `simple_build_system-1.2.2/src/_simple_build_system/incinfo.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/includes.py` & `simple_build_system-1.2.2/src/_simple_build_system/includes.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/init_project.py` & `simple_build_system-1.2.2/src/_simple_build_system/init_project.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/instsl.py` & `simple_build_system-1.2.2/src/_simple_build_system/instsl.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/instsl2.py` & `simple_build_system-1.2.2/src/_simple_build_system/instsl2.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/io.py` & `simple_build_system-1.2.2/src/_simple_build_system/io.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/langs.py` & `simple_build_system-1.2.2/src/_simple_build_system/langs.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/loadpkgs.py` & `simple_build_system-1.2.2/src/_simple_build_system/loadpkgs.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/makefile.py` & `simple_build_system-1.2.2/src/_simple_build_system/makefile.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/mtime.py` & `simple_build_system-1.2.2/src/_simple_build_system/mtime.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/parse_args.py` & `simple_build_system-1.2.2/src/_simple_build_system/parse_args.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/pkgfilter.py` & `simple_build_system-1.2.2/src/_simple_build_system/pkgfilter.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/pkgutils.py` & `simple_build_system-1.2.2/src/_simple_build_system/pkgutils.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/replace.py` & `simple_build_system-1.2.2/src/_simple_build_system/replace.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/singlecfg.py` & `simple_build_system-1.2.2/src/_simple_build_system/singlecfg.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/target_base.py` & `simple_build_system-1.2.2/src/_simple_build_system/target_base.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/target_builder.py` & `simple_build_system-1.2.2/src/_simple_build_system/target_builder.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/testlauncher.py` & `simple_build_system-1.2.2/src/_simple_build_system/testlauncher.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/testxml.py` & `simple_build_system-1.2.2/src/_simple_build_system/testxml.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/tfact_binary.py` & `simple_build_system-1.2.2/src/_simple_build_system/tfact_binary.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/tfact_headerdeps.py` & `simple_build_system-1.2.2/src/_simple_build_system/tfact_headerdeps.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/tfact_libavail.py` & `simple_build_system-1.2.2/src/_simple_build_system/tfact_libavail.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/tfact_prepinc.py` & `simple_build_system-1.2.2/src/_simple_build_system/tfact_prepinc.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/tfact_pyinit.py` & `simple_build_system-1.2.2/src/_simple_build_system/tfact_pyinit.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/tfact_reflogs.py` & `simple_build_system-1.2.2/src/_simple_build_system/tfact_reflogs.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/tfact_symlink.py` & `simple_build_system-1.2.2/src/_simple_build_system/tfact_symlink.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/_simple_build_system/utils.py` & `simple_build_system-1.2.2/src/_simple_build_system/utils.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.2.1/src/simple_build_system.egg-info/PKG-INFO` & `simple_build_system-1.2.2/src/simple_build_system.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-build-system
-Version: 1.2.1
+Version: 1.2.2
 Summary: A very simple to use build system for projects with primarily C++/Python code, intended for usage by scientific developers without a strong SW-engineering background.
 Author-email: Thomas Kittelmann <thomas.kittelmann@ess.eu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `simple_build_system-1.2.1/src/simple_build_system.egg-info/SOURCES.txt` & `simple_build_system-1.2.2/src/simple_build_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*


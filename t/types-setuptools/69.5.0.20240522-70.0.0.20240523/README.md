# Comparing `tmp/types-setuptools-69.5.0.20240522.tar.gz` & `tmp/types-setuptools-70.0.0.20240523.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-setuptools-69.5.0.20240522.tar", last modified: Wed May 22 02:22:14 2024, max compression
+gzip compressed data, was "types-setuptools-70.0.0.20240523.tar", last modified: Thu May 23 02:21:52 2024, max compression
```

## Comparing `types-setuptools-69.5.0.20240522.tar` & `types-setuptools-70.0.0.20240523.tar`

### file list

```diff
@@ -1,146 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.776876 types-setuptools-69.5.0.20240522/
--rw-r--r--   0 runner    (1001) docker     (127)    18241 2024-05-22 02:22:12.000000 types-setuptools-69.5.0.20240522/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 02:22:12.000000 types-setuptools-69.5.0.20240522/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-22 02:22:14.776876 types-setuptools-69.5.0.20240522/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.760876 types-setuptools-69.5.0.20240522/distutils-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-22 02:22:12.000000 types-setuptools-69.5.0.20240522/distutils-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/_modified.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/archive_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/ccompiler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/cmd.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.764876 types-setuptools-69.5.0.20240522/distutils-stubs/command/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/bdist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/bdist_rpm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/upload.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.764876 types-setuptools-69.5.0.20240522/distutils-stubs/compat/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/compat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:12.000000 types-setuptools-69.5.0.20240522/distutils-stubs/compat/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/dep_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/extension.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/filelist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/sysconfig.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.764876 types-setuptools-69.5.0.20240522/pkg_resources-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-22 02:22:12.000000 types-setuptools-69.5.0.20240522/pkg_resources-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)    20179 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/pkg_resources-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.764876 types-setuptools-69.5.0.20240522/pkg_resources-stubs/_vendored_packaging/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/pkg_resources-stubs/_vendored_packaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/pkg_resources-stubs/_vendored_packaging/markers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/pkg_resources-stubs/_vendored_packaging/requirements.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/pkg_resources-stubs/_vendored_packaging/specifiers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/pkg_resources-stubs/_vendored_packaging/version.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.764876 types-setuptools-69.5.0.20240522/pkg_resources-stubs/extern/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/pkg_resources-stubs/extern/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:12.000000 types-setuptools-69.5.0.20240522/pkg_resources-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 02:22:14.776876 types-setuptools-69.5.0.20240522/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-05-22 02:22:12.000000 types-setuptools-69.5.0.20240522/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.768876 types-setuptools-69.5.0.20240522/setuptools-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-22 02:22:12.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.768876 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/_modified.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/archive_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/ccompiler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/cmd.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.772876 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/bdist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/bdist_rpm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/upload.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.772876 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/compat/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/compat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/dep_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/extension.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/filelist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/sysconfig.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/archive_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/build_meta.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.776876 types-setuptools-69.5.0.20240522/setuptools-stubs/command/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/alias.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/bdist_egg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/bdist_rpm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/develop.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/dist_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/easy_install.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/editable_wheel.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/egg_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/install_egg_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/rotate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/saveopts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/setopt.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/test.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/upload.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/upload_docs.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.776876 types-setuptools-69.5.0.20240522/setuptools-stubs/compat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/compat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/compat/py310.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/compat/py311.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/compat/py39.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.776876 types-setuptools-69.5.0.20240522/setuptools-stubs/config/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/config/expand.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/config/pyprojecttoml.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/config/setupcfg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/dep_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/depends.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/discovery.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/extension.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.776876 types-setuptools-69.5.0.20240522/setuptools-stubs/extern/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/extern/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/glob.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/installer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/launch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/logging.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/modified.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/monkey.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/msvc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/namespaces.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/package_index.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:12.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/sandbox.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/unicode_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/warnings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/wheel.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/windows_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.776876 types-setuptools-69.5.0.20240522/types_setuptools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-22 02:22:14.000000 types-setuptools-69.5.0.20240522/types_setuptools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-22 02:22:14.000000 types-setuptools-69.5.0.20240522/types_setuptools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:22:14.000000 types-setuptools-69.5.0.20240522/types_setuptools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 02:22:14.000000 types-setuptools-69.5.0.20240522/types_setuptools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:52.654161 types-setuptools-70.0.0.20240523/
+-rw-r--r--   0 runner    (1001) docker     (127)    18364 2024-05-23 02:21:51.000000 types-setuptools-70.0.0.20240523/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 02:21:51.000000 types-setuptools-70.0.0.20240523/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-23 02:21:52.654161 types-setuptools-70.0.0.20240523/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:52.638160 types-setuptools-70.0.0.20240523/distutils-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-23 02:21:51.000000 types-setuptools-70.0.0.20240523/distutils-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/_modified.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/archive_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/ccompiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/cmd.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:52.642160 types-setuptools-70.0.0.20240523/distutils-stubs/command/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/command/bdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/command/bdist_rpm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/command/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/command/upload.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:52.642160 types-setuptools-70.0.0.20240523/distutils-stubs/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/compat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:51.000000 types-setuptools-70.0.0.20240523/distutils-stubs/compat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/dep_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/filelist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/sysconfig.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/distutils-stubs/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:52.642160 types-setuptools-70.0.0.20240523/pkg_resources-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-23 02:21:51.000000 types-setuptools-70.0.0.20240523/pkg_resources-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    20301 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/pkg_resources-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:52.642160 types-setuptools-70.0.0.20240523/pkg_resources-stubs/_vendored_packaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/pkg_resources-stubs/_vendored_packaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/pkg_resources-stubs/_vendored_packaging/markers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/pkg_resources-stubs/_vendored_packaging/requirements.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/pkg_resources-stubs/_vendored_packaging/specifiers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/pkg_resources-stubs/_vendored_packaging/version.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:52.642160 types-setuptools-70.0.0.20240523/pkg_resources-stubs/extern/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/pkg_resources-stubs/extern/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:51.000000 types-setuptools-70.0.0.20240523/pkg_resources-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 02:21:52.654161 types-setuptools-70.0.0.20240523/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-23 02:21:51.000000 types-setuptools-70.0.0.20240523/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:52.646160 types-setuptools-70.0.0.20240523/setuptools-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-23 02:21:51.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:52.646160 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/_modified.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/archive_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/ccompiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/cmd.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:52.650160 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/bdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/bdist_rpm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/upload.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:52.650160 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/compat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/dep_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/filelist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/sysconfig.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/archive_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/build_meta.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:52.654161 types-setuptools-70.0.0.20240523/setuptools-stubs/command/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/alias.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/bdist_egg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/bdist_rpm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/develop.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/dist_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/easy_install.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/editable_wheel.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/egg_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/install_egg_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/rotate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/saveopts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/setopt.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/test.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/upload.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/command/upload_docs.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:52.654161 types-setuptools-70.0.0.20240523/setuptools-stubs/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/compat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/compat/py310.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/compat/py311.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/compat/py39.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:52.654161 types-setuptools-70.0.0.20240523/setuptools-stubs/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/config/expand.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/config/pyprojecttoml.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/config/setupcfg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/depends.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/discovery.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/extension.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:52.654161 types-setuptools-70.0.0.20240523/setuptools-stubs/extern/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/extern/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/glob.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/installer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/launch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/logging.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/modified.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/monkey.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/msvc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/namespaces.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/package_index.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:51.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/sandbox.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/unicode_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/warnings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/wheel.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-23 02:21:41.000000 types-setuptools-70.0.0.20240523/setuptools-stubs/windows_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:52.654161 types-setuptools-70.0.0.20240523/types_setuptools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-23 02:21:52.000000 types-setuptools-70.0.0.20240523/types_setuptools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-05-23 02:21:52.000000 types-setuptools-70.0.0.20240523/types_setuptools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 02:21:52.000000 types-setuptools-70.0.0.20240523/types_setuptools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 02:21:52.000000 types-setuptools-70.0.0.20240523/types_setuptools.egg-info/top_level.txt
```

### Comparing `types-setuptools-69.5.0.20240522/CHANGELOG.md` & `types-setuptools-70.0.0.20240523/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 70.0.0.20240523 (2024-05-23)
+
+Make `shutil.rmtree.onexc` parameter optional (#12002)
+
+Bump setuptools to 70.0 (#11994)
+
 ## 69.5.0.20240522 (2024-05-22)
 
 `distutils` & `setuptools`: Relax path related params (#11948)
 
 Co-authored-by: Jelle Zijlstra <jelle.zijlstra@gmail.com>
 
 ## 69.5.0.20240519 (2024-05-19)
```

### Comparing `types-setuptools-69.5.0.20240522/PKG-INFO` & `types-setuptools-70.0.0.20240523/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-setuptools
-Version: 69.5.0.20240522
+Version: 70.0.0.20240523
 Summary: Typing stubs for setuptools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `setuptools`.
 
 This version of `types-setuptools` aims to provide accurate annotations
-for `setuptools==69.5.*`.
+for `setuptools==70.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `489e8dbf41d3350388331b2303bd4f3d13ecbfff` and was tested
-with mypy 1.10.0, pyright 1.1.363, and
+This package was generated from typeshed commit `f7c03486ee01c8ea74823db75e017341bf3c2ad0` and was tested
+with mypy 1.10.0, pyright 1.1.364, and
 pytype 2024.4.11.
```

### Comparing `types-setuptools-69.5.0.20240522/pkg_resources-stubs/__init__.pyi` & `types-setuptools-70.0.0.20240523/pkg_resources-stubs/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import types
 import zipimport
 from _typeshed import BytesPath, Incomplete, StrOrBytesPath, StrPath, Unused
 from collections.abc import Callable, Generator, Iterable, Iterator, Sequence
 from io import BytesIO
 from itertools import chain
 from pkgutil import get_importer as get_importer
@@ -170,21 +171,14 @@
         full_env: Environment | None = None,
         installer: _InstallerType = None,
         fallback: bool = True,
     ) -> tuple[list[Distribution], dict[Distribution, Exception]]: ...
     def require(self, *requirements: _NestedStr) -> Sequence[Distribution]: ...
     def subscribe(self, callback: Callable[[Distribution], object], existing: bool = True) -> None: ...
 
-working_set: WorkingSet
-require = working_set.require
-iter_entry_points = working_set.iter_entry_points
-add_activation_listener = working_set.subscribe
-run_script = working_set.run_script
-run_main = run_script
-
 class Environment:
     def __init__(
         self, search_path: Iterable[str] | None = None, platform: str | None = ..., python: str | None = ...
     ) -> None: ...
     def can_add(self, dist: Distribution) -> bool: ...
     def remove(self, dist: Distribution) -> None: ...
     def scan(self, search_path: Iterable[str] | None = None) -> None: ...
@@ -285,24 +279,14 @@
     def resource_listdir(self, package_or_requirement: _PkgReqType, resource_name: str) -> list[str]: ...
     def extraction_error(self) -> NoReturn: ...
     def get_cache_path(self, archive_name: str, names: Iterable[StrPath] = ()) -> str: ...
     def postprocess(self, tempname: StrOrBytesPath, filename: str) -> None: ...
     def set_extraction_path(self, path: str) -> None: ...
     def cleanup_resources(self, force: bool = False) -> list[str]: ...
 
-__resource_manager: ResourceManager  # Doesn't exist at runtime
-resource_exists = __resource_manager.resource_exists
-resource_isdir = __resource_manager.resource_isdir
-resource_filename = __resource_manager.resource_filename
-resource_stream = __resource_manager.resource_stream
-resource_string = __resource_manager.resource_string
-resource_listdir = __resource_manager.resource_listdir
-set_extraction_path = __resource_manager.set_extraction_path
-cleanup_resources = __resource_manager.cleanup_resources
-
 @overload
 def get_provider(moduleOrReq: str) -> IResourceProvider: ...
 @overload
 def get_provider(moduleOrReq: Requirement) -> Distribution: ...
 
 class IMetadataProvider(Protocol):
     def has_metadata(self, name: str) -> bool: ...
@@ -494,7 +478,29 @@
 def ensure_directory(path: StrOrBytesPath) -> None: ...
 @overload
 def normalize_path(filename: StrPath) -> str: ...
 @overload
 def normalize_path(filename: BytesPath) -> bytes: ...
 
 class PkgResourcesDeprecationWarning(Warning): ...
+
+__resource_manager: ResourceManager  # Doesn't exist at runtime
+resource_exists = __resource_manager.resource_exists
+resource_isdir = __resource_manager.resource_isdir
+resource_filename = __resource_manager.resource_filename
+resource_stream = __resource_manager.resource_stream
+resource_string = __resource_manager.resource_string
+resource_listdir = __resource_manager.resource_listdir
+set_extraction_path = __resource_manager.set_extraction_path
+cleanup_resources = __resource_manager.cleanup_resources
+
+working_set: WorkingSet
+require = working_set.require
+iter_entry_points = working_set.iter_entry_points
+add_activation_listener = working_set.subscribe
+run_script = working_set.run_script
+run_main = run_script
+
+if sys.version_info >= (3, 10):
+    LOCALE_ENCODING: Final = "locale"
+else:
+    LOCALE_ENCODING: Final = None
```

### Comparing `types-setuptools-69.5.0.20240522/pkg_resources-stubs/_vendored_packaging/markers.pyi` & `types-setuptools-70.0.0.20240523/pkg_resources-stubs/_vendored_packaging/markers.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/pkg_resources-stubs/_vendored_packaging/specifiers.pyi` & `types-setuptools-70.0.0.20240523/pkg_resources-stubs/_vendored_packaging/specifiers.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/pkg_resources-stubs/_vendored_packaging/version.pyi` & `types-setuptools-70.0.0.20240523/pkg_resources-stubs/_vendored_packaging/version.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/pkg_resources-stubs/extern/__init__.pyi` & `types-setuptools-70.0.0.20240523/pkg_resources-stubs/extern/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setup.py` & `types-setuptools-70.0.0.20240523/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,40 +11,40 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `setuptools`.
 
 This version of `types-setuptools` aims to provide accurate annotations
-for `setuptools==69.5.*`.
+for `setuptools==70.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `489e8dbf41d3350388331b2303bd4f3d13ecbfff` and was tested
-with mypy 1.10.0, pyright 1.1.363, and
+This package was generated from typeshed commit `f7c03486ee01c8ea74823db75e017341bf3c2ad0` and was tested
+with mypy 1.10.0, pyright 1.1.364, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="69.5.0.20240522",
+      version="70.0.0.20240523",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['pkg_resources-stubs', 'distutils-stubs', 'setuptools-stubs'],
-      package_data={'pkg_resources-stubs': ['__init__.pyi', '_vendored_packaging/__init__.pyi', '_vendored_packaging/markers.pyi', '_vendored_packaging/requirements.pyi', '_vendored_packaging/specifiers.pyi', '_vendored_packaging/version.pyi', 'extern/__init__.pyi', 'METADATA.toml', 'py.typed'], 'distutils-stubs': ['_modified.pyi', 'archive_util.pyi', 'ccompiler.pyi', 'cmd.pyi', 'command/bdist.pyi', 'command/bdist_rpm.pyi', 'command/build.pyi', 'command/build_clib.pyi', 'command/build_ext.pyi', 'command/build_py.pyi', 'command/install.pyi', 'command/install_lib.pyi', 'command/install_scripts.pyi', 'command/register.pyi', 'command/sdist.pyi', 'command/upload.pyi', 'compat/__init__.pyi', 'config.pyi', 'dep_util.pyi', 'dist.pyi', 'errors.pyi', 'extension.pyi', 'filelist.pyi', 'sysconfig.pyi', 'util.pyi', 'METADATA.toml', 'compat/py.typed'], 'setuptools-stubs': ['__init__.pyi', '_distutils/_modified.pyi', '_distutils/archive_util.pyi', '_distutils/ccompiler.pyi', '_distutils/cmd.pyi', '_distutils/command/bdist.pyi', '_distutils/command/bdist_rpm.pyi', '_distutils/command/build.pyi', '_distutils/command/build_clib.pyi', '_distutils/command/build_ext.pyi', '_distutils/command/build_py.pyi', '_distutils/command/install.pyi', '_distutils/command/install_lib.pyi', '_distutils/command/install_scripts.pyi', '_distutils/command/register.pyi', '_distutils/command/sdist.pyi', '_distutils/command/upload.pyi', '_distutils/compat/__init__.pyi', '_distutils/config.pyi', '_distutils/dep_util.pyi', '_distutils/dist.pyi', '_distutils/errors.pyi', '_distutils/extension.pyi', '_distutils/filelist.pyi', '_distutils/sysconfig.pyi', '_distutils/util.pyi', 'archive_util.pyi', 'build_meta.pyi', 'command/__init__.pyi', 'command/alias.pyi', 'command/bdist_egg.pyi', 'command/bdist_rpm.pyi', 'command/build.pyi', 'command/build_clib.pyi', 'command/build_ext.pyi', 'command/build_py.pyi', 'command/develop.pyi', 'command/dist_info.pyi', 'command/easy_install.pyi', 'command/editable_wheel.pyi', 'command/egg_info.pyi', 'command/install.pyi', 'command/install_egg_info.pyi', 'command/install_lib.pyi', 'command/install_scripts.pyi', 'command/register.pyi', 'command/rotate.pyi', 'command/saveopts.pyi', 'command/sdist.pyi', 'command/setopt.pyi', 'command/test.pyi', 'command/upload.pyi', 'command/upload_docs.pyi', 'compat/__init__.pyi', 'compat/py310.pyi', 'compat/py311.pyi', 'compat/py39.pyi', 'config/__init__.pyi', 'config/expand.pyi', 'config/pyprojecttoml.pyi', 'config/setupcfg.pyi', 'dep_util.pyi', 'depends.pyi', 'discovery.pyi', 'dist.pyi', 'errors.pyi', 'extension.pyi', 'extern/__init__.pyi', 'glob.pyi', 'installer.pyi', 'launch.pyi', 'logging.pyi', 'modified.pyi', 'monkey.pyi', 'msvc.pyi', 'namespaces.pyi', 'package_index.pyi', 'sandbox.pyi', 'unicode_utils.pyi', 'version.pyi', 'warnings.pyi', 'wheel.pyi', 'windows_support.pyi', 'METADATA.toml', 'py.typed']},
+      package_data={'pkg_resources-stubs': ['__init__.pyi', '_vendored_packaging/__init__.pyi', '_vendored_packaging/markers.pyi', '_vendored_packaging/requirements.pyi', '_vendored_packaging/specifiers.pyi', '_vendored_packaging/version.pyi', 'extern/__init__.pyi', 'METADATA.toml', 'py.typed'], 'distutils-stubs': ['_modified.pyi', 'archive_util.pyi', 'ccompiler.pyi', 'cmd.pyi', 'command/bdist.pyi', 'command/bdist_rpm.pyi', 'command/build.pyi', 'command/build_clib.pyi', 'command/build_ext.pyi', 'command/build_py.pyi', 'command/install.pyi', 'command/install_lib.pyi', 'command/install_scripts.pyi', 'command/register.pyi', 'command/sdist.pyi', 'command/upload.pyi', 'compat/__init__.pyi', 'config.pyi', 'dep_util.pyi', 'dist.pyi', 'errors.pyi', 'extension.pyi', 'filelist.pyi', 'sysconfig.pyi', 'util.pyi', 'METADATA.toml', 'compat/py.typed'], 'setuptools-stubs': ['__init__.pyi', '_distutils/_modified.pyi', '_distutils/archive_util.pyi', '_distutils/ccompiler.pyi', '_distutils/cmd.pyi', '_distutils/command/bdist.pyi', '_distutils/command/bdist_rpm.pyi', '_distutils/command/build.pyi', '_distutils/command/build_clib.pyi', '_distutils/command/build_ext.pyi', '_distutils/command/build_py.pyi', '_distutils/command/install.pyi', '_distutils/command/install_lib.pyi', '_distutils/command/install_scripts.pyi', '_distutils/command/register.pyi', '_distutils/command/sdist.pyi', '_distutils/command/upload.pyi', '_distutils/compat/__init__.pyi', '_distutils/config.pyi', '_distutils/dep_util.pyi', '_distutils/dist.pyi', '_distutils/errors.pyi', '_distutils/extension.pyi', '_distutils/filelist.pyi', '_distutils/sysconfig.pyi', '_distutils/util.pyi', 'archive_util.pyi', 'build_meta.pyi', 'command/__init__.pyi', 'command/alias.pyi', 'command/bdist_egg.pyi', 'command/bdist_rpm.pyi', 'command/build.pyi', 'command/build_clib.pyi', 'command/build_ext.pyi', 'command/build_py.pyi', 'command/develop.pyi', 'command/dist_info.pyi', 'command/easy_install.pyi', 'command/editable_wheel.pyi', 'command/egg_info.pyi', 'command/install.pyi', 'command/install_egg_info.pyi', 'command/install_lib.pyi', 'command/install_scripts.pyi', 'command/register.pyi', 'command/rotate.pyi', 'command/saveopts.pyi', 'command/sdist.pyi', 'command/setopt.pyi', 'command/test.pyi', 'command/upload.pyi', 'command/upload_docs.pyi', 'compat/__init__.pyi', 'compat/py310.pyi', 'compat/py311.pyi', 'compat/py39.pyi', 'config/__init__.pyi', 'config/expand.pyi', 'config/pyprojecttoml.pyi', 'config/setupcfg.pyi', 'depends.pyi', 'discovery.pyi', 'dist.pyi', 'errors.pyi', 'extension.pyi', 'extern/__init__.pyi', 'glob.pyi', 'installer.pyi', 'launch.pyi', 'logging.pyi', 'modified.pyi', 'monkey.pyi', 'msvc.pyi', 'namespaces.pyi', 'package_index.pyi', 'sandbox.pyi', 'unicode_utils.pyi', 'version.pyi', 'warnings.pyi', 'wheel.pyi', 'windows_support.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/__init__.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/_modified.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/_modified.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/archive_util.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/archive_util.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/ccompiler.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/ccompiler.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/cmd.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/cmd.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/bdist.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/bdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/bdist_rpm.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/bdist_rpm.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/build.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/build.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/build_clib.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/build_clib.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/build_ext.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/build_ext.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/build_py.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/build_py.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/install.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/install.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/install_lib.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/install_lib.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/register.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/register.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/sdist.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/sdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/upload.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/command/upload.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/dist.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/dist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/errors.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/extension.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/filelist.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/filelist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/sysconfig.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/sysconfig.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/util.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/_distutils/util.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/archive_util.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/archive_util.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/build_meta.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/build_meta.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/command/bdist_egg.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/command/bdist_egg.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/command/build_ext.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/command/build_ext.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/command/build_py.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/command/build_py.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/command/develop.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/command/develop.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/command/easy_install.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/command/easy_install.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/command/editable_wheel.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/command/editable_wheel.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete, StrPath
+from collections.abc import Iterator
 from enum import Enum
 from pathlib import Path
 from types import TracebackType
 from typing import Protocol
 from typing_extensions import Self, TypeAlias
 
 from .. import Command, errors, namespaces
@@ -59,14 +60,16 @@
         self, _exc_type: type[BaseException] | None, _exc_value: BaseException | None, _traceback: TracebackType | None
     ) -> None: ...
 
 class _TopLevelFinder:
     dist: Incomplete
     name: Incomplete
     def __init__(self, dist: Distribution, name: str) -> None: ...
+    def template_vars(self) -> tuple[str, str, dict[str, str], dict[str, list[str]]]: ...
+    def get_implementation(self) -> Iterator[tuple[str, bytes]]: ...
     def __call__(self, wheel: _WheelFile, files: list[str], mapping: dict[str, str]): ...
     def __enter__(self) -> Self: ...
     def __exit__(
         self, _exc_type: type[BaseException] | None, _exc_value: BaseException | None, _traceback: TracebackType | None
     ) -> None: ...
 
 class _NamespaceInstaller(namespaces.Installer):
```

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/command/egg_info.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/command/egg_info.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/command/install.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/command/install.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/command/install_lib.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/command/install_lib.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/command/sdist.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/command/sdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/command/setopt.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/command/setopt.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/command/test.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/command/test.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/command/upload_docs.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/command/upload_docs.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/config/expand.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/config/expand.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/config/pyprojecttoml.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/config/pyprojecttoml.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/config/setupcfg.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/config/setupcfg.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/depends.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/depends.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/discovery.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/discovery.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/dist.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/dist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/errors.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/extension.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/extern/__init__.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/extern/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/msvc.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/msvc.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/package_index.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/package_index.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/setuptools-stubs/sandbox.pyi` & `types-setuptools-70.0.0.20240523/setuptools-stubs/sandbox.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240522/types_setuptools.egg-info/PKG-INFO` & `types-setuptools-70.0.0.20240523/types_setuptools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-setuptools
-Version: 69.5.0.20240522
+Version: 70.0.0.20240523
 Summary: Typing stubs for setuptools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `setuptools`.
 
 This version of `types-setuptools` aims to provide accurate annotations
-for `setuptools==69.5.*`.
+for `setuptools==70.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `489e8dbf41d3350388331b2303bd4f3d13ecbfff` and was tested
-with mypy 1.10.0, pyright 1.1.363, and
+This package was generated from typeshed commit `f7c03486ee01c8ea74823db75e017341bf3c2ad0` and was tested
+with mypy 1.10.0, pyright 1.1.364, and
 pytype 2024.4.11.
```

### Comparing `types-setuptools-69.5.0.20240522/types_setuptools.egg-info/SOURCES.txt` & `types-setuptools-70.0.0.20240523/types_setuptools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 pkg_resources-stubs/_vendored_packaging/specifiers.pyi
 pkg_resources-stubs/_vendored_packaging/version.pyi
 pkg_resources-stubs/extern/__init__.pyi
 setuptools-stubs/METADATA.toml
 setuptools-stubs/__init__.pyi
 setuptools-stubs/archive_util.pyi
 setuptools-stubs/build_meta.pyi
-setuptools-stubs/dep_util.pyi
 setuptools-stubs/depends.pyi
 setuptools-stubs/discovery.pyi
 setuptools-stubs/dist.pyi
 setuptools-stubs/errors.pyi
 setuptools-stubs/extension.pyi
 setuptools-stubs/glob.pyi
 setuptools-stubs/installer.pyi
```


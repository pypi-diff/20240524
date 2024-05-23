# Comparing `tmp/pylibCZIrw-4.1.0.tar.gz` & `tmp/pylibCZIrw-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibCZIrw-4.1.0.tar", last modified: Mon Jan 22 12:57:28 2024, max compression
+gzip compressed data, was "pylibCZIrw-4.1.1.tar", last modified: Thu May 23 16:17:40 2024, max compression
```

## Comparing `pylibCZIrw-4.1.0.tar` & `pylibCZIrw-4.1.1.tar`

### file list

```diff
@@ -1,587 +1,589 @@
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.396634 pylibCZIrw-4.1.0/
--rw-rw-rw-   0        0        0     2212 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/CMakeLists.txt
--rw-rw-rw-   0        0        0      787 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/CMakeSettings.json
--rw-rw-rw-   0        0        0     7815 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/COPYING.LESSER.txt
--rw-rw-rw-   0        0        0    35821 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/COPYING.txt
--rw-rw-rw-   0        0        0     2729 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/INFO.md
--rw-rw-rw-   0        0        0      344 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      191 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/NOTICE.txt
--rw-rw-rw-   0        0        0     3689 2024-01-22 12:57:28.396634 pylibCZIrw-4.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:27.541821 pylibCZIrw-4.1.0/_pylibCZIrw/
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.129705 pylibCZIrw-4.1.0/_pylibCZIrw/src/
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.129705 pylibCZIrw-4.1.0/_pylibCZIrw/src/api/
--rw-rw-rw-   0        0        0      625 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/_pylibCZIrw/src/api/CMakeLists.txt
--rw-rw-rw-   0        0        0     5743 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/_pylibCZIrw/src/api/CZIreadAPI.cpp
--rw-rw-rw-   0        0        0     5121 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/_pylibCZIrw/src/api/CZIreadAPI.h
--rw-rw-rw-   0        0        0    10797 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/_pylibCZIrw/src/api/CZIwriteAPI.cpp
--rw-rw-rw-   0        0        0     6496 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/_pylibCZIrw/src/api/CZIwriteAPI.h
--rw-rw-rw-   0        0        0     1232 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/_pylibCZIrw/src/api/PImage.cpp
--rw-rw-rw-   0        0        0     1740 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/_pylibCZIrw/src/api/PImage.h
--rw-rw-rw-   0        0        0     5758 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/_pylibCZIrw/src/api/StaticContext.cpp
--rw-rw-rw-   0        0        0     1292 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/_pylibCZIrw/src/api/StaticContext.h
--rw-rw-rw-   0        0        0     1083 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/_pylibCZIrw/src/api/SubBlockCache.h
--rw-rw-rw-   0        0        0       75 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/_pylibCZIrw/src/api/inc_libCzi.h
--rw-rw-rw-   0        0        0      577 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/_pylibCZIrw/src/api/site.cpp
--rw-rw-rw-   0        0        0      366 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/_pylibCZIrw/src/api/site.h
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.129705 pylibCZIrw-4.1.0/_pylibCZIrw/src/bindings/
--rw-rw-rw-   0        0        0      454 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/_pylibCZIrw/src/bindings/CMakeLists.txt
--rw-rw-rw-   0        0        0    10669 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/_pylibCZIrw/src/bindings/CZIrw.cpp
--rw-rw-rw-   0        0        0     1405 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/_pylibCZIrw/src/bindings/PbHelper.cpp
--rw-rw-rw-   0        0        0     1774 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/_pylibCZIrw/src/bindings/PbHelper.h
--rw-rw-rw-   0        0        0      671 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/_pylibCZIrw/src/bindings/include_python.h
--rw-rw-rw-   0        0        0      114 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/_pylibCZIrw/src/pylibCZIrw_Config.h.in
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.129705 pylibCZIrw-4.1.0/_pylibCZIrw/tests/
--rw-rw-rw-   0        0        0      355 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/_pylibCZIrw/tests/CMakeLists.txt
--rw-rw-rw-   0        0        0     1486 2024-01-22 12:56:28.000000 pylibCZIrw-4.1.0/_pylibCZIrw/tests/main.cpp
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:27.541821 pylibCZIrw-4.1.0/libs/
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.145272 pylibCZIrw-4.1.0/libs/libCZIrw/
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.145272 pylibCZIrw-4.1.0/libs/libCZIrw/.devcontainer/
--rw-rw-rw-   0        0        0      975 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/.devcontainer/Dockerfile
--rw-rw-rw-   0        0        0     1390 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/.devcontainer/devcontainer.json
--rw-rw-rw-   0        0        0     1858 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/.devcontainer/reinstall-cmake.sh
--rw-rw-rw-   0        0        0     3111 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/.editorconfig
--rw-rw-rw-   0        0        0       41 2024-01-22 12:56:33.000000 pylibCZIrw-4.1.0/libs/libCZIrw/.git
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.145272 pylibCZIrw-4.1.0/libs/libCZIrw/.github/
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.145272 pylibCZIrw-4.1.0/libs/libCZIrw/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0      872 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-rw-   0        0        0      615 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-rw-   0        0        0     1409 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/.github/PULL_REQUEST_TEMPLATE.md
--rw-rw-rw-   0        0        0      676 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/.github/codecov.yml
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.145272 pylibCZIrw-4.1.0/libs/libCZIrw/.github/workflows/
--rw-rw-rw-   0        0        0      590 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/.github/workflows/cla.yml
--rw-rw-rw-   0        0        0     4267 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/.github/workflows/cmake.yml
--rw-rw-rw-   0        0        0     2129 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/.github/workflows/codeql.yml
--rw-rw-rw-   0        0        0     1143 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/.github/workflows/mega-linter.yml
--rw-rw-rw-   0        0        0     1283 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/.github/workflows/pages.yml
--rw-rw-rw-   0        0        0      296 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/.github/workflows/reuse.yml
--rw-rw-rw-   0        0        0     5437 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/.gitignore
--rw-rw-rw-   0        0        0      999 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/.mega-linter.yml
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.145272 pylibCZIrw-4.1.0/libs/libCZIrw/.reuse/
--rw-rw-rw-   0        0        0      731 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/.reuse/dep5
--rw-rw-rw-   0        0        0     5415 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/CMakeLists.txt
--rw-rw-rw-   0        0        0     5500 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0     2687 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    35819 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/COPYING
--rw-rw-rw-   0        0        0     7815 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/COPYING.LESSER
--rw-rw-rw-   0        0        0      973 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/CPPLINT.cfg
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.145272 pylibCZIrw-4.1.0/libs/libCZIrw/LICENSES/
--rw-rw-rw-   0        0        0     1471 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/LICENSES/BSD-3-Clause.txt
--rw-rw-rw-   0        0        0     7169 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/LICENSES/CC0-1.0.txt
--rw-rw-rw-   0        0        0    42402 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/LICENSES/LGPL-3.0-or-later.txt
--rw-rw-rw-   0        0        0     1087 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/LICENSES/MIT.txt
--rw-rw-rw-   0        0        0      878 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/LICENSES/RSA-MD.txt
--rw-rw-rw-   0        0        0     4257 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/README.md
--rw-rw-rw-   0        0        0      814 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/SECURITY.md
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.145272 pylibCZIrw-4.1.0/libs/libCZIrw/Src/
--rw-rw-rw-   0        0        0     2855 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/CMakeLists.txt
--rw-rw-rw-   0        0        0   129711 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/Doxyfile
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.160898 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/
--rw-rw-rw-   0        0        0     5138 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/CMakeLists.txt
--rw-rw-rw-   0        0        0    20850 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/JxrDecode.cpp
--rw-rw-rw-   0        0        0     6781 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/JxrDecode.h
--rw-rw-rw-   0        0        0     1539 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/JxrDecode_Config.h.in
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:27.541821 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:27.541821 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/common/
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.160898 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/common/include/
--rw-rw-rw-   0        0        0     2965 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/common/include/guiddef.h
--rw-rw-rw-   0        0        0      500 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/common/include/log.h
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.160898 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/common/src/
--rw-rw-rw-   0        0        0     1070 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/common/src/log.c
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:27.541821 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.160898 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/
--rw-rw-rw-   0        0        0    46506 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/JXRTranscode.c
--rw-rw-rw-   0        0        0     6737 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/decode.c
--rw-rw-rw-   0        0        0     5153 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/decode.h
--rw-rw-rw-   0        0        0    10548 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/postprocess.c
--rw-rw-rw-   0        0        0    44298 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/segdec.c
--rw-rw-rw-   0        0        0    68553 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/strInvTransform.c
--rw-rw-rw-   0        0        0    18366 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/strPredQuantDec.c
--rw-rw-rw-   0        0        0   150752 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/strdec.c
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.160898 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/
--rw-rw-rw-   0        0        0     5373 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/encode.c
--rw-rw-rw-   0        0        0     4279 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/encode.h
--rw-rw-rw-   0        0        0    44030 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/segenc.c
--rw-rw-rw-   0        0        0    38152 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/strFwdTransform.c
--rw-rw-rw-   0        0        0    18689 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/strPredQuantEnc.c
--rw-rw-rw-   0        0        0    97739 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/strenc.c
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.176522 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/
--rw-rw-rw-   0        0        0    13131 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/adapthuff.c
--rw-rw-rw-   0        0        0     2078 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/ansi.h
--rw-rw-rw-   0        0        0     4872 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/common.h
--rw-rw-rw-   0        0        0     6113 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/image.c
--rw-rw-rw-   0        0        0    10566 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/strPredQuant.c
--rw-rw-rw-   0        0        0     2627 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/strTransform.c
--rw-rw-rw-   0        0        0     2377 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/strTransform.h
--rw-rw-rw-   0        0        0    41874 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/strcodec.c
--rw-rw-rw-   0        0        0    21813 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/strcodec.h
--rw-rw-rw-   0        0        0    18575 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/windowsmediaphoto.h
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.176522 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/
--rw-rw-rw-   0        0        0    33150 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRGlue.c
--rw-rw-rw-   0        0        0    31007 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRGlue.h
--rw-rw-rw-   0        0        0    81704 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRGlueJxr.c
--rw-rw-rw-   0        0        0    71873 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRGluePFC.c
--rw-rw-rw-   0        0        0    28280 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRMeta.c
--rw-rw-rw-   0        0        0     8988 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRMeta.h
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.223399 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/
--rw-rw-rw-   0        0        0    17269 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/BitmapOperations.cpp
--rw-rw-rw-   0        0        0     5407 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/BitmapOperations.h
--rw-rw-rw-   0        0        0    25778 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/BitmapOperations.hpp
--rw-rw-rw-   0        0        0    12422 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CMakeLists.txt
--rw-rw-rw-   0        0        0    15396 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CZIReader.cpp
--rw-rw-rw-   0        0        0     3063 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CZIReader.h
--rw-rw-rw-   0        0        0     3416 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CreateBitmap.cpp
--rw-rw-rw-   0        0        0     1053 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziAttachment.cpp
--rw-rw-rw-   0        0        0      804 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziAttachment.h
--rw-rw-rw-   0        0        0     4873 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziAttachmentsDirectory.cpp
--rw-rw-rw-   0        0        0     2880 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziAttachmentsDirectory.h
--rw-rw-rw-   0        0        0     6271 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziDimensionInfo.cpp
--rw-rw-rw-   0        0        0     3447 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziDimensionInfo.h
--rw-rw-rw-   0        0        0    14595 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziDisplaySettings.cpp
--rw-rw-rw-   0        0        0     1867 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziDisplaySettings.h
--rw-rw-rw-   0        0        0     7038 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziMetadata.cpp
--rw-rw-rw-   0        0        0     1733 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziMetadata.h
--rw-rw-rw-   0        0        0    38124 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziMetadataBuilder.cpp
--rw-rw-rw-   0        0        0     4798 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziMetadataBuilder.h
--rw-rw-rw-   0        0        0    16535 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo.cpp
--rw-rw-rw-   0        0        0     1522 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo.h
--rw-rw-rw-   0        0        0    71829 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo2.cpp
--rw-rw-rw-   0        0        0    41047 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo2.h
--rw-rw-rw-   0        0        0     1668 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziMetadataSegment.cpp
--rw-rw-rw-   0        0        0      773 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziMetadataSegment.h
--rw-rw-rw-   0        0        0    37512 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziParse.cpp
--rw-rw-rw-   0        0        0    10286 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziParse.h
--rw-rw-rw-   0        0        0    37542 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziReaderWriter.cpp
--rw-rw-rw-   0        0        0     7889 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziReaderWriter.h
--rw-rw-rw-   0        0        0     7162 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziStructs.cpp
--rw-rw-rw-   0        0        0     9712 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziStructs.h
--rw-rw-rw-   0        0        0     2258 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziSubBlock.cpp
--rw-rw-rw-   0        0        0     1001 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziSubBlock.h
--rw-rw-rw-   0        0        0    23357 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziSubBlockDirectory.cpp
--rw-rw-rw-   0        0        0     7190 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziSubBlockDirectory.h
--rw-rw-rw-   0        0        0     6794 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziUtils.cpp
--rw-rw-rw-   0        0        0     2510 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziUtils.h
--rw-rw-rw-   0        0        0    60370 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziWriter.cpp
--rw-rw-rw-   0        0        0    16641 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziWriter.h
--rw-rw-rw-   0        0        0     8017 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/DimCoordinate.cpp
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.239024 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/
--rw-rw-rw-   0        0        0    28556 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/CZICmd_usage.markdown
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.255989 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/
--rw-rw-rw-   0        0        0    15042 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/CZI_1.PNG
--rw-rw-rw-   0        0        0    11631 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/CZI_2.PNG
--rw-rw-rw-   0        0        0   629984 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/ScalingSingleChannelTileAccessor1.png
--rw-rw-rw-   0        0        0    15606 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_1.PNG
--rw-rw-rw-   0        0        0     6597 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_2.PNG
--rw-rw-rw-   0        0        0   508732 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_3.PNG
--rw-rw-rw-   0        0        0   435548 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_4.PNG
--rw-rw-rw-   0        0        0    22752 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/Tinting-LUT.png
--rw-rw-rw-   0        0        0    95014 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/VisualStudio_cmake1.png
--rw-rw-rw-   0        0        0   947057 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/ZEN_screenshot_1.PNG
--rw-rw-rw-   0        0        0   149904 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/ZEN_screenshot_2.PNG
--rw-rw-rw-   0        0        0   242149 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_1_raspi.PNG
--rw-rw-rw-   0        0        0    32954 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_1_raspi_help_freetype.PNG
--rw-rw-rw-   0        0        0   270106 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_install_raspi1.PNG
--rw-rw-rw-   0        0        0    59883 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_raspi_unittests_1.PNG
--rw-rw-rw-   0        0        0    14602 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/compositors_1.png
--rw-rw-rw-   0        0        0     4107 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/compositors_2.png
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.255989 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/drawings/
--rw-rw-rw-   0        0        0   100864 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/drawings/VS-project.pub
--rw-rw-rw-   0        0        0   108032 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/drawings/VS-project_2.pub
--rw-rw-rw-   0        0        0    10567 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/gradationcurve_1.PNG
--rw-rw-rw-   0        0        0     8316 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/gradationcurve_2.PNG
--rw-rw-rw-   0        0        0     7632 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept1.PNG
--rw-rw-rw-   0        0        0    20658 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept2.PNG
--rw-rw-rw-   0        0        0    14836 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept3.PNG
--rw-rw-rw-   0        0        0    29100 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept4.PNG
--rw-rw-rw-   0        0        0     1966 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Todos.markdown
--rw-rw-rw-   0        0        0     2964 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/accessors.markdown
--rw-rw-rw-   0        0        0     3817 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/building_libCZI.markdown
--rw-rw-rw-   0        0        0    92375 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/drawings.docx
--rw-rw-rw-   0        0        0     3983 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/image_document_concept.markdown
--rw-rw-rw-   0        0        0     5655 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/mainpage.markdown
--rw-rw-rw-   0        0        0     2275 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/multichannelcomposition.markdown
--rw-rw-rw-   0        0        0    11999 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/using_libCZI.markdown
--rw-rw-rw-   0        0        0     2013 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/version-history.markdown
--rw-rw-rw-   0        0        0     5534 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/write_czi.markdown
--rw-rw-rw-   0        0        0     2537 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/FileHeaderSegmentData.h
--rw-rw-rw-   0        0        0      631 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/ImportExport.h
--rw-rw-rw-   0        0        0     5302 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/IndexSet.cpp
--rw-rw-rw-   0        0        0      992 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/IndexSet.h
--rw-rw-rw-   0        0        0     8780 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/MD5Sum.cpp
--rw-rw-rw-   0        0        0     5318 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/MD5Sum.h
--rw-rw-rw-   0        0        0    56438 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/MultiChannelCompositor.cpp
--rw-rw-rw-   0        0        0      166 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/MultiChannelCompositor.h
--rw-rw-rw-   0        0        0     7936 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/SingleChannelAccessorBase.cpp
--rw-rw-rw-   0        0        0     5951 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/SingleChannelAccessorBase.h
--rw-rw-rw-   0        0        0    11414 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/SingleChannelPyramidLevelTileAccessor.cpp
--rw-rw-rw-   0        0        0     2849 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/SingleChannelPyramidLevelTileAccessor.h
--rw-rw-rw-   0        0        0    22239 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/SingleChannelScalingTileAccessor.cpp
--rw-rw-rw-   0        0        0     3646 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/SingleChannelScalingTileAccessor.h
--rw-rw-rw-   0        0        0     7799 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/SingleChannelTileAccessor.cpp
--rw-rw-rw-   0        0        0     1847 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/SingleChannelTileAccessor.h
--rw-rw-rw-   0        0        0     2095 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/SingleChannelTileCompositor.cpp
--rw-rw-rw-   0        0        0      333 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/SingleChannelTileCompositor.h
--rw-rw-rw-   0        0        0      187 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Site.h
--rw-rw-rw-   0        0        0    15063 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamImpl.cpp
--rw-rw-rw-   0        0        0     4171 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamImpl.h
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.255989 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamsLib/
--rw-rw-rw-   0        0        0    13960 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamsLib/curlhttpinputstream.cpp
--rw-rw-rw-   0        0        0     3121 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamsLib/curlhttpinputstream.h
--rw-rw-rw-   0        0        0     1611 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamsLib/preadfileinputstream.cpp
--rw-rw-rw-   0        0        0      903 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamsLib/preadfileinputstream.h
--rw-rw-rw-   0        0        0     2296 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamsLib/simplefileinputstream.cpp
--rw-rw-rw-   0        0        0      966 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamsLib/simplefileinputstream.h
--rw-rw-rw-   0        0        0     7597 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamsLib/streamsFactory.cpp
--rw-rw-rw-   0        0        0     1998 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamsLib/windowsfileinputstream.cpp
--rw-rw-rw-   0        0        0      916 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamsLib/windowsfileinputstream.h
--rw-rw-rw-   0        0        0    13988 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/XmlNodeWrapper.h
--rw-rw-rw-   0        0        0     5713 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/bitmapData.h
--rw-rw-rw-   0        0        0     3694 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/decoder.cpp
--rw-rw-rw-   0        0        0      514 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/decoder.h
--rw-rw-rw-   0        0        0    17564 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/decoder_wic.cpp
--rw-rw-rw-   0        0        0      774 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/decoder_wic.h
--rw-rw-rw-   0        0        0     7668 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/decoder_zstd.cpp
--rw-rw-rw-   0        0        0      773 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/decoder_zstd.h
--rw-rw-rw-   0        0        0      264 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/inc_libCZI_Config.h
--rw-rw-rw-   0        0        0     3896 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/jxrlibcompress.cpp
--rw-rw-rw-   0        0        0    39613 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI.h
--rw-rw-rw-   0        0        0    42075 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Compositor.h
--rw-rw-rw-   0        0        0     2186 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Config.h.in
--rw-rw-rw-   0        0        0    17832 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_DimCoordinate.h
--rw-rw-rw-   0        0        0     9650 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Helpers.h
--rw-rw-rw-   0        0        0     4319 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Lib.cpp
--rw-rw-rw-   0        0        0    72195 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Metadata.h
--rw-rw-rw-   0        0        0    63505 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Metadata2.h
--rw-rw-rw-   0        0        0    14650 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Pixels.h
--rw-rw-rw-   0        0        0     9656 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_ReadWrite.h
--rw-rw-rw-   0        0        0     5040 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Site.cpp
--rw-rw-rw-   0        0        0     6262 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Site.h
--rw-rw-rw-   0        0        0    16268 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_StreamsLib.h
--rw-rw-rw-   0        0        0    24057 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Utilities.cpp
--rw-rw-rw-   0        0        0    22615 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Utilities.h
--rw-rw-rw-   0        0        0    33411 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Write.h
--rw-rw-rw-   0        0        0    42911 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_compress.h
--rw-rw-rw-   0        0        0    14559 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_exceptions.h
--rw-rw-rw-   0        0        0     3060 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/pugiconfig.hpp
--rw-rw-rw-   0        0        0   407937 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/pugixml.cpp
--rw-rw-rw-   0        0        0    60454 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/pugixml.hpp
--rw-rw-rw-   0        0        0     3343 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/splines.cpp
--rw-rw-rw-   0        0        0      554 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/splines.h
--rw-rw-rw-   0        0        0     1553 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/stdAllocator.cpp
--rw-rw-rw-   0        0        0      593 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/stdAllocator.h
--rw-rw-rw-   0        0        0     4792 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/subblock_cache.cpp
--rw-rw-rw-   0        0        0     1843 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/subblock_cache.h
--rw-rw-rw-   0        0        0    20294 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/utilities.cpp
--rw-rw-rw-   0        0        0    10179 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/utilities.h
--rw-rw-rw-   0        0        0    12099 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/utilities_simd.cpp
--rw-rw-rw-   0        0        0    18572 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/zstdCompress.cpp
--rw-rw-rw-   0        0        0     6291 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/THIRD_PARTY_LICENSES.txt
--rw-rw-rw-   0        0        0     6882 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/cla_corporate.txt
--rw-rw-rw-   0        0        0     6571 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/cla_individual.txt
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.255989 pylibCZIrw-4.1.0/libs/libCZIrw/cmake/
--rw-rw-rw-   0        0        0      990 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/cmake/ExternalEIGEN3.cmake
--rw-rw-rw-   0        0        0     4609 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/cmake/TestLargeFile.cmake
--rw-rw-rw-   0        0        0     1842 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/cmake/check_can_use_neon_intrinsics.cmake
--rw-rw-rw-   0        0        0     2656 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/cmake/check_unaligned_access.cmake
--rw-rw-rw-   0        0        0      150 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/libCZIrw/opencppcoverage.txt
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.271630 pylibCZIrw-4.1.0/libs/pybind11/
--rw-rw-rw-   0        0        0     1306 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.appveyor.yml
--rw-rw-rw-   0        0        0     1034 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.clang-format
--rw-rw-rw-   0        0        0     2682 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.clang-tidy
--rw-rw-rw-   0        0        0     2269 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.cmake-format.yaml
--rw-rw-rw-   0        0        0     1332 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.codespell-ignore-lines
--rw-rw-rw-   0        0        0       41 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.git
--rw-rw-rw-   0        0        0       19 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.gitattributes
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.271630 pylibCZIrw-4.1.0/libs/pybind11/.github/
--rw-rw-rw-   0        0        0      191 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.github/CODEOWNERS
--rw-rw-rw-   0        0        0    15672 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.github/CONTRIBUTING.md
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.271630 pylibCZIrw-4.1.0/libs/pybind11/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0     2622 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-rw-rw-   0        0        0      336 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-rw-   0        0        0      169 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.github/dependabot.yml
--rw-rw-rw-   0        0        0      124 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.github/labeler.yml
--rw-rw-rw-   0        0        0       53 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.github/labeler_merged.yml
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.271630 pylibCZIrw-4.1.0/libs/pybind11/.github/matchers/
--rw-rw-rw-   0        0        0      700 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.github/matchers/pylint.json
--rw-rw-rw-   0        0        0      664 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.github/pull_request_template.md
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.271630 pylibCZIrw-4.1.0/libs/pybind11/.github/workflows/
--rw-rw-rw-   0        0        0    35326 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.github/workflows/ci.yml
--rw-rw-rw-   0        0        0     2364 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.github/workflows/configure.yml
--rw-rw-rw-   0        0        0     1551 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.github/workflows/format.yml
--rw-rw-rw-   0        0        0      666 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.github/workflows/labeler.yml
--rw-rw-rw-   0        0        0     2742 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.github/workflows/pip.yml
--rw-rw-rw-   0        0        0     2992 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.github/workflows/upstream.yml
--rw-rw-rw-   0        0        0      548 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.gitignore
--rw-rw-rw-   0        0        0     3859 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0       65 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/.readthedocs.yml
--rw-rw-rw-   0        0        0    12389 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/CMakeLists.txt
--rw-rw-rw-   0        0        0     1713 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/LICENSE
--rw-rw-rw-   0        0        0      253 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/MANIFEST.in
--rw-rw-rw-   0        0        0     7867 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/README.rst
--rw-rw-rw-   0        0        0      701 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/SECURITY.md
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.287255 pylibCZIrw-4.1.0/libs/pybind11/docs/
--rw-rw-rw-   0        0        0      628 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/Doxyfile
--rw-rw-rw-   0        0        0     7609 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/Makefile
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:27.541821 pylibCZIrw-4.1.0/libs/pybind11/docs/_static/
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.287255 pylibCZIrw-4.1.0/libs/pybind11/docs/_static/css/
--rw-rw-rw-   0        0        0       40 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/_static/css/custom.css
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.287255 pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.302880 pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/cast/
--rw-rw-rw-   0        0        0     4018 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/cast/chrono.rst
--rw-rw-rw-   0        0        0     3522 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/cast/custom.rst
--rw-rw-rw-   0        0        0    14593 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/cast/eigen.rst
--rw-rw-rw-   0        0        0     3998 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/cast/functional.rst
--rw-rw-rw-   0        0        0     1599 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/cast/index.rst
--rw-rw-rw-   0        0        0    12541 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/cast/overview.rst
--rw-rw-rw-   0        0        0     9835 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/cast/stl.rst
--rw-rw-rw-   0        0        0     9415 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/cast/strings.rst
--rw-rw-rw-   0        0        0    49131 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/classes.rst
--rw-rw-rw-   0        0        0     8722 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/embedding.rst
--rw-rw-rw-   0        0        0    18197 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/exceptions.rst
--rw-rw-rw-   0        0        0    27343 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/functions.rst
--rw-rw-rw-   0        0        0    16051 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/misc.rst
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.302880 pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/pycpp/
--rw-rw-rw-   0        0        0      291 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/pycpp/index.rst
--rw-rw-rw-   0        0        0    17616 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/pycpp/numpy.rst
--rw-rw-rw-   0        0        0     9316 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/pycpp/object.rst
--rw-rw-rw-   0        0        0     5865 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/pycpp/utilities.rst
--rw-rw-rw-   0        0        0     6551 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/smart_ptrs.rst
--rw-rw-rw-   0        0        0     9547 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/basics.rst
--rw-rw-rw-   0        0        0     2943 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/benchmark.py
--rw-rw-rw-   0        0        0     3263 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/benchmark.rst
--rw-rw-rw-   0        0        0   122400 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/changelog.rst
--rw-rw-rw-   0        0        0    17645 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/classes.rst
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.302880 pylibCZIrw-4.1.0/libs/pybind11/docs/cmake/
--rw-rw-rw-   0        0        0      281 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/cmake/index.rst
--rw-rw-rw-   0        0        0    26478 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/compiling.rst
--rw-rw-rw-   0        0        0    11942 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/conf.py
--rw-rw-rw-   0        0        0    13601 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/faq.rst
--rw-rw-rw-   0        0        0      661 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/index.rst
--rw-rw-rw-   0        0        0     3382 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/installing.rst
--rw-rw-rw-   0        0        0     3151 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/limitations.rst
--rw-rw-rw-   0        0        0    61034 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/pybind11-logo.png
--rw-rw-rw-   0        0        0    44653 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/pybind11_vs_boost_python1.png
--rw-rw-rw-   0        0        0    87708 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-rw-rw-   0        0        0    41121 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/pybind11_vs_boost_python2.png
--rw-rw-rw-   0        0        0    85853 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-rw-rw-   0        0        0     2777 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/reference.rst
--rw-rw-rw-   0        0        0     4676 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/release.rst
--rw-rw-rw-   0        0        0      155 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/requirements.txt
--rw-rw-rw-   0        0        0    24601 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/docs/upgrade.rst
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:27.541821 pylibCZIrw-4.1.0/libs/pybind11/include/
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.318507 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/
--rw-rw-rw-   0        0        0    25024 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/attr.h
--rw-rw-rw-   0        0        0     7958 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/buffer_info.h
--rw-rw-rw-   0        0        0    69016 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/cast.h
--rw-rw-rw-   0        0        0     8683 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/chrono.h
--rw-rw-rw-   0        0        0      122 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/common.h
--rw-rw-rw-   0        0        0     2170 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/complex.h
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.318507 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/detail/
--rw-rw-rw-   0        0        0    29261 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/detail/class.h
--rw-rw-rw-   0        0        0    54735 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/detail/common.h
--rw-rw-rw-   0        0        0     6133 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/detail/descr.h
--rw-rw-rw-   0        0        0    18293 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/detail/init.h
--rw-rw-rw-   0        0        0    28877 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/detail/internals.h
--rw-rw-rw-   0        0        0    49541 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/detail/type_caster_base.h
--rw-rw-rw-   0        0        0     1690 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/detail/typeid.h
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.318507 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/eigen/
--rw-rw-rw-   0        0        0      387 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/eigen/common.h
--rw-rw-rw-   0        0        0    32849 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/eigen/matrix.h
--rw-rw-rw-   0        0        0    18958 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/eigen/tensor.h
--rw-rw-rw-   0        0        0      328 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/eigen.h
--rw-rw-rw-   0        0        0    13775 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/embed.h
--rw-rw-rw-   0        0        0     4887 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/eval.h
--rw-rw-rw-   0        0        0     5139 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/functional.h
--rw-rw-rw-   0        0        0     8501 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/gil.h
--rw-rw-rw-   0        0        0     9127 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/iostream.h
--rw-rw-rw-   0        0        0    81723 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/numpy.h
--rw-rw-rw-   0        0        0     9305 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/operators.h
--rw-rw-rw-   0        0        0     2826 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/options.h
--rw-rw-rw-   0        0        0   129596 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/pybind11.h
--rw-rw-rw-   0        0        0   101012 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/pytypes.h
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.318507 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/stl/
--rw-rw-rw-   0        0        0     4301 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/stl/filesystem.h
--rw-rw-rw-   0        0        0    15924 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/stl.h
--rw-rw-rw-   0        0        0    30748 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/stl_bind.h
--rw-rw-rw-   0        0        0     1990 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/type_caster_pyobject_ptr.h
--rw-rw-rw-   0        0        0     2872 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/noxfile.py
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.318507 pylibCZIrw-4.1.0/libs/pybind11/pybind11/
--rw-rw-rw-   0        0        0      446 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/pybind11/__init__.py
--rw-rw-rw-   0        0        0     1606 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/pybind11/__main__.py
--rw-rw-rw-   0        0        0      240 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/pybind11/_version.py
--rw-rw-rw-   0        0        0     1244 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/pybind11/commands.py
--rw-rw-rw-   0        0        0        0 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/pybind11/py.typed
--rw-rw-rw-   0        0        0    17973 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/pybind11/setup_helpers.py
--rw-rw-rw-   0        0        0     2396 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/pyproject.toml
--rw-rw-rw-   0        0        0     1538 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/setup.cfg
--rw-rw-rw-   0        0        0     5005 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.381009 pylibCZIrw-4.1.0/libs/pybind11/tests/
--rw-rw-rw-   0        0        0    22317 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/CMakeLists.txt
--rw-rw-rw-   0        0        0     5840 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/conftest.py
--rw-rw-rw-   0        0        0    12058 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/constructor_stats.h
--rw-rw-rw-   0        0        0     3686 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/cross_module_gil_utils.cpp
--rw-rw-rw-   0        0        0     1827 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/cross_module_interleaved_error_already_set.cpp
--rw-rw-rw-   0        0        0      410 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
--rw-rw-rw-   0        0        0      953 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/env.py
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.381009 pylibCZIrw-4.1.0/libs/pybind11/tests/extra_python_package/
--rw-rw-rw-   0        0        0        0 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/extra_python_package/pytest.ini
--rw-rw-rw-   0        0        0     8694 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/extra_python_package/test_files.py
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.381009 pylibCZIrw-4.1.0/libs/pybind11/tests/extra_setuptools/
--rw-rw-rw-   0        0        0        0 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/extra_setuptools/pytest.ini
--rw-rw-rw-   0        0        0     4304 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-rw-rw-   0        0        0     2939 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/local_bindings.h
--rw-rw-rw-   0        0        0     5948 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/object.h
--rw-rw-rw-   0        0        0     6413 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-rw-rw-   0        0        0     4640 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/pybind11_tests.cpp
--rw-rw-rw-   0        0        0     2770 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/pybind11_tests.h
--rw-rw-rw-   0        0        0      790 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/pytest.ini
--rw-rw-rw-   0        0        0      610 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/requirements.txt
--rw-rw-rw-   0        0        0      880 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_async.cpp
--rw-rw-rw-   0        0        0      560 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_async.py
--rw-rw-rw-   0        0        0    10807 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_buffers.cpp
--rw-rw-rw-   0        0        0     7172 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_buffers.py
--rw-rw-rw-   0        0        0    16417 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_builtin_casters.cpp
--rw-rw-rw-   0        0        0    17771 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_builtin_casters.py
--rw-rw-rw-   0        0        0     4233 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_call_policies.cpp
--rw-rw-rw-   0        0        0     6796 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_call_policies.py
--rw-rw-rw-   0        0        0    11138 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_callbacks.cpp
--rw-rw-rw-   0        0        0     7014 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_callbacks.py
--rw-rw-rw-   0        0        0     3451 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_chrono.cpp
--rw-rw-rw-   0        0        0     5896 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_chrono.py
--rw-rw-rw-   0        0        0    25506 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_class.cpp
--rw-rw-rw-   0        0        0    15242 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_class.py
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.381009 pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/
--rw-rw-rw-   0        0        0     2665 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-rw-rw-   0        0        0      696 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/embed.cpp
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.381009 pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/installed_embed/
--rw-rw-rw-   0        0        0     1199 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.381009 pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/installed_function/
--rw-rw-rw-   0        0        0     1332 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.381009 pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/installed_target/
--rw-rw-rw-   0        0        0     1731 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-rw-rw-   0        0        0      158 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/main.cpp
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.381009 pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-rw-rw-   0        0        0     1394 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.381009 pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-rw-rw-   0        0        0     1198 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.381009 pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-rw-rw-   0        0        0     1409 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-rw-rw-   0        0        0      206 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/test.py
--rw-rw-rw-   0        0        0     3886 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_const_name.cpp
--rw-rw-rw-   0        0        0      622 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_const_name.py
--rw-rw-rw-   0        0        0     5864 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_constants_and_functions.cpp
--rw-rw-rw-   0        0        0     1607 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_constants_and_functions.py
--rw-rw-rw-   0        0        0    26597 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_copy_move.cpp
--rw-rw-rw-   0        0        0     4928 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_copy_move.py
--rw-rw-rw-   0        0        0     7489 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_custom_type_casters.cpp
--rw-rw-rw-   0        0        0     4114 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_custom_type_casters.py
--rw-rw-rw-   0        0        0     1300 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_custom_type_setup.cpp
--rw-rw-rw-   0        0        0     1139 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_custom_type_setup.py
--rw-rw-rw-   0        0        0     4698 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_docstring_options.cpp
--rw-rw-rw-   0        0        0     2487 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_docstring_options.py
--rw-rw-rw-   0        0        0    19778 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_eigen_matrix.cpp
--rw-rw-rw-   0        0        0    29835 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_eigen_matrix.py
--rw-rw-rw-   0        0        0      491 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_eigen_tensor.cpp
--rw-rw-rw-   0        0        0    10923 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_eigen_tensor.inl
--rw-rw-rw-   0        0        0     9702 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_eigen_tensor.py
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.396634 pylibCZIrw-4.1.0/libs/pybind11/tests/test_embed/
--rw-rw-rw-   0        0        0     1845 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_embed/CMakeLists.txt
--rw-rw-rw-   0        0        0     1358 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_embed/catch.cpp
--rw-rw-rw-   0        0        0      563 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_embed/external_module.cpp
--rw-rw-rw-   0        0        0    17884 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_embed/test_interpreter.cpp
--rw-rw-rw-   0        0        0      251 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_embed/test_interpreter.py
--rw-rw-rw-   0        0        0      291 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_embed/test_trampoline.py
--rw-rw-rw-   0        0        0     5855 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_enum.cpp
--rw-rw-rw-   0        0        0     9205 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_enum.py
--rw-rw-rw-   0        0        0     3286 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_eval.cpp
--rw-rw-rw-   0        0        0     1193 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_eval.py
--rw-rw-rw-   0        0        0      123 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_eval_call.py
--rw-rw-rw-   0        0        0    12429 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_exceptions.cpp
--rw-rw-rw-   0        0        0      412 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_exceptions.h
--rw-rw-rw-   0        0        0    14274 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_exceptions.py
--rw-rw-rw-   0        0        0    18585 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_factory_constructors.cpp
--rw-rw-rw-   0        0        0    17007 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_factory_constructors.py
--rw-rw-rw-   0        0        0     5455 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_gil_scoped.cpp
--rw-rw-rw-   0        0        0     8749 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_gil_scoped.py
--rw-rw-rw-   0        0        0     4086 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_iostream.cpp
--rw-rw-rw-   0        0        0     7435 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_iostream.py
--rw-rw-rw-   0        0        0     9725 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-rw-rw-   0        0        0    13989 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_kwargs_and_defaults.py
--rw-rw-rw-   0        0        0     4507 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_local_bindings.cpp
--rw-rw-rw-   0        0        0     8311 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_local_bindings.py
--rw-rw-rw-   0        0        0    22704 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_methods_and_attributes.cpp
--rw-rw-rw-   0        0        0    18879 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_methods_and_attributes.py
--rw-rw-rw-   0        0        0     4246 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_modules.cpp
--rw-rw-rw-   0        0        0     4079 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_modules.py
--rw-rw-rw-   0        0        0    12646 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_multiple_inheritance.cpp
--rw-rw-rw-   0        0        0    12367 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_multiple_inheritance.py
--rw-rw-rw-   0        0        0    21488 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_numpy_array.cpp
--rw-rw-rw-   0        0        0    23554 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_numpy_array.py
--rw-rw-rw-   0        0        0    21728 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_numpy_dtypes.cpp
--rw-rw-rw-   0        0        0    14712 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_numpy_dtypes.py
--rw-rw-rw-   0        0        0     4594 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_numpy_vectorize.cpp
--rw-rw-rw-   0        0        0     9924 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_numpy_vectorize.py
--rw-rw-rw-   0        0        0     2854 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_opaque_types.cpp
--rw-rw-rw-   0        0        0     1905 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_opaque_types.py
--rw-rw-rw-   0        0        0     9413 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_operator_overloading.cpp
--rw-rw-rw-   0        0        0     4483 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_operator_overloading.py
--rw-rw-rw-   0        0        0     6913 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_pickling.cpp
--rw-rw-rw-   0        0        0     2813 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_pickling.py
--rw-rw-rw-   0        0        0    31911 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_pytypes.cpp
--rw-rw-rw-   0        0        0    24790 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_pytypes.py
--rw-rw-rw-   0        0        0    21734 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_sequences_and_iterators.cpp
--rw-rw-rw-   0        0        0     8291 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_sequences_and_iterators.py
--rw-rw-rw-   0        0        0    19368 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_smart_ptr.cpp
--rw-rw-rw-   0        0        0     9845 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_smart_ptr.py
--rw-rw-rw-   0        0        0    22138 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_stl.cpp
--rw-rw-rw-   0        0        0    12688 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_stl.py
--rw-rw-rw-   0        0        0     6401 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_stl_binders.cpp
--rw-rw-rw-   0        0        0    10159 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_stl_binders.py
--rw-rw-rw-   0        0        0     4764 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-rw-rw-   0        0        0      769 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_tagbased_polymorphic.py
--rw-rw-rw-   0        0        0     1921 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_thread.cpp
--rw-rw-rw-   0        0        0      868 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_thread.py
--rw-rw-rw-   0        0        0     4631 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_type_caster_pyobject_ptr.cpp
--rw-rw-rw-   0        0        0     3364 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_type_caster_pyobject_ptr.py
--rw-rw-rw-   0        0        0      625 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_union.cpp
--rw-rw-rw-   0        0        0      156 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_union.py
--rw-rw-rw-   0        0        0      883 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_unnamed_namespace_a.cpp
--rw-rw-rw-   0        0        0     1175 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_unnamed_namespace_a.py
--rw-rw-rw-   0        0        0      354 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_unnamed_namespace_b.cpp
--rw-rw-rw-   0        0        0      148 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_unnamed_namespace_b.py
--rw-rw-rw-   0        0        0     1525 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_vector_unique_ptr_member.cpp
--rw-rw-rw-   0        0        0      343 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_vector_unique_ptr_member.py
--rw-rw-rw-   0        0        0    23583 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_virtual_functions.cpp
--rw-rw-rw-   0        0        0    13371 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/test_virtual_functions.py
--rw-rw-rw-   0        0        0     3366 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/valgrind-numpy-scipy.supp
--rw-rw-rw-   0        0        0     2774 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tests/valgrind-python.supp
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.396634 pylibCZIrw-4.1.0/libs/pybind11/tools/
--rw-rw-rw-   0        0        0     2525 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tools/FindCatch.cmake
--rw-rw-rw-   0        0        0     3191 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tools/FindEigen3.cmake
--rw-rw-rw-   0        0        0    11477 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tools/FindPythonLibsNew.cmake
--rw-rw-rw-   0        0        0      840 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tools/JoinPaths.cmake
--rw-rw-rw-   0        0        0     1467 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tools/check-style.sh
--rw-rw-rw-   0        0        0      975 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tools/cmake_uninstall.cmake.in
--rw-rw-rw-   0        0        0     1156 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-rw-rw-   0        0        0     1067 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tools/libsize.py
--rw-rw-rw-   0        0        0     1373 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tools/make_changelog.py
--rw-rw-rw-   0        0        0      203 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tools/pybind11.pc.in
--rw-rw-rw-   0        0        0    14854 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tools/pybind11Common.cmake
--rw-rw-rw-   0        0        0     7334 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tools/pybind11Config.cmake.in
--rw-rw-rw-   0        0        0     9216 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tools/pybind11NewTools.cmake
--rw-rw-rw-   0        0        0     8594 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tools/pybind11Tools.cmake
--rw-rw-rw-   0        0        0       97 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tools/pyproject.toml
--rw-rw-rw-   0        0        0     2167 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tools/setup_global.py.in
--rw-rw-rw-   0        0        0     1278 2024-01-22 12:56:35.000000 pylibCZIrw-4.1.0/libs/pybind11/tools/setup_main.py.in
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.396634 pylibCZIrw-4.1.0/pylibCZIrw/
--rw-rw-rw-   0        0        0      896 2024-01-22 12:56:29.000000 pylibCZIrw-4.1.0/pylibCZIrw/__init__.py
--rw-rw-rw-   0        0        0    50379 2024-01-22 12:56:29.000000 pylibCZIrw-4.1.0/pylibCZIrw/czi.py
--rw-rw-rw-   0        0        0   575191 2024-01-22 12:56:29.000000 pylibCZIrw-4.1.0/pylibCZIrw-documentation.html
-drwxrwxrwx   0        0        0        0 2024-01-22 12:57:28.396634 pylibCZIrw-4.1.0/pylibCZIrw.egg-info/
--rw-rw-rw-   0        0        0     3689 2024-01-22 12:57:27.000000 pylibCZIrw-4.1.0/pylibCZIrw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    22504 2024-01-22 12:57:27.000000 pylibCZIrw-4.1.0/pylibCZIrw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-22 12:57:27.000000 pylibCZIrw-4.1.0/pylibCZIrw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-01-22 12:57:27.000000 pylibCZIrw-4.1.0/pylibCZIrw.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       33 2024-01-22 12:57:27.000000 pylibCZIrw-4.1.0/pylibCZIrw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-01-22 12:57:27.000000 pylibCZIrw-4.1.0/pylibCZIrw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1683 2024-01-22 12:57:28.396634 pylibCZIrw-4.1.0/setup.cfg
--rw-rw-rw-   0        0        0     9364 2024-01-22 12:56:29.000000 pylibCZIrw-4.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.108487 pylibCZIrw-4.1.1/
+-rw-rw-rw-   0        0        0     2212 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/CMakeLists.txt
+-rw-rw-rw-   0        0        0      787 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/CMakeSettings.json
+-rw-rw-rw-   0        0        0     7815 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/COPYING.LESSER.txt
+-rw-rw-rw-   0        0        0    35821 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/COPYING.txt
+-rw-rw-rw-   0        0        0     2729 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/INFO.md
+-rw-rw-rw-   0        0        0      344 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      191 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/NOTICE.txt
+-rw-rw-rw-   0        0        0     3689 2024-05-23 16:17:40.108487 pylibCZIrw-4.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.795982 pylibCZIrw-4.1.1/_pylibCZIrw/
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.811605 pylibCZIrw-4.1.1/_pylibCZIrw/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.827229 pylibCZIrw-4.1.1/_pylibCZIrw/src/api/
+-rw-rw-rw-   0        0        0      625 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/_pylibCZIrw/src/api/CMakeLists.txt
+-rw-rw-rw-   0        0        0     5743 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/_pylibCZIrw/src/api/CZIreadAPI.cpp
+-rw-rw-rw-   0        0        0     5121 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/_pylibCZIrw/src/api/CZIreadAPI.h
+-rw-rw-rw-   0        0        0    10797 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/_pylibCZIrw/src/api/CZIwriteAPI.cpp
+-rw-rw-rw-   0        0        0     6496 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/_pylibCZIrw/src/api/CZIwriteAPI.h
+-rw-rw-rw-   0        0        0     1232 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/_pylibCZIrw/src/api/PImage.cpp
+-rw-rw-rw-   0        0        0     1740 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/_pylibCZIrw/src/api/PImage.h
+-rw-rw-rw-   0        0        0     5758 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/_pylibCZIrw/src/api/StaticContext.cpp
+-rw-rw-rw-   0        0        0     1292 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/_pylibCZIrw/src/api/StaticContext.h
+-rw-rw-rw-   0        0        0     1083 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/_pylibCZIrw/src/api/SubBlockCache.h
+-rw-rw-rw-   0        0        0       75 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/_pylibCZIrw/src/api/inc_libCzi.h
+-rw-rw-rw-   0        0        0      577 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/_pylibCZIrw/src/api/site.cpp
+-rw-rw-rw-   0        0        0      366 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/_pylibCZIrw/src/api/site.h
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.827229 pylibCZIrw-4.1.1/_pylibCZIrw/src/bindings/
+-rw-rw-rw-   0        0        0      454 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/_pylibCZIrw/src/bindings/CMakeLists.txt
+-rw-rw-rw-   0        0        0    10669 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/_pylibCZIrw/src/bindings/CZIrw.cpp
+-rw-rw-rw-   0        0        0     1405 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/_pylibCZIrw/src/bindings/PbHelper.cpp
+-rw-rw-rw-   0        0        0     1774 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/_pylibCZIrw/src/bindings/PbHelper.h
+-rw-rw-rw-   0        0        0      671 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/_pylibCZIrw/src/bindings/include_python.h
+-rw-rw-rw-   0        0        0      114 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/_pylibCZIrw/src/pylibCZIrw_Config.h.in
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.827229 pylibCZIrw-4.1.1/_pylibCZIrw/tests/
+-rw-rw-rw-   0        0        0      355 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/_pylibCZIrw/tests/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1486 2024-05-23 16:16:39.000000 pylibCZIrw-4.1.1/_pylibCZIrw/tests/main.cpp
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.795982 pylibCZIrw-4.1.1/libs/
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.827229 pylibCZIrw-4.1.1/libs/libCZIrw/
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.827229 pylibCZIrw-4.1.1/libs/libCZIrw/.devcontainer/
+-rw-rw-rw-   0        0        0      975 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/.devcontainer/Dockerfile
+-rw-rw-rw-   0        0        0     1390 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/.devcontainer/devcontainer.json
+-rw-rw-rw-   0        0        0     1858 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/.devcontainer/reinstall-cmake.sh
+-rw-rw-rw-   0        0        0     3111 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/.editorconfig
+-rw-rw-rw-   0        0        0       41 2024-05-23 16:16:44.000000 pylibCZIrw-4.1.1/libs/libCZIrw/.git
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.827229 pylibCZIrw-4.1.1/libs/libCZIrw/.github/
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.843108 pylibCZIrw-4.1.1/libs/libCZIrw/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0      872 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-rw-   0        0        0      615 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-rw-   0        0        0     1409 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/.github/PULL_REQUEST_TEMPLATE.md
+-rw-rw-rw-   0        0        0      676 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/.github/codecov.yml
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.843108 pylibCZIrw-4.1.1/libs/libCZIrw/.github/workflows/
+-rw-rw-rw-   0        0        0      590 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/.github/workflows/cla.yml
+-rw-rw-rw-   0        0        0     4352 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/.github/workflows/cmake.yml
+-rw-rw-rw-   0        0        0     2129 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/.github/workflows/codeql.yml
+-rw-rw-rw-   0        0        0     1143 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/.github/workflows/mega-linter.yml
+-rw-rw-rw-   0        0        0     1283 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/.github/workflows/pages.yml
+-rw-rw-rw-   0        0        0      296 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/.github/workflows/reuse.yml
+-rw-rw-rw-   0        0        0     5437 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/.gitignore
+-rw-rw-rw-   0        0        0      999 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/.mega-linter.yml
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.843108 pylibCZIrw-4.1.1/libs/libCZIrw/.reuse/
+-rw-rw-rw-   0        0        0      731 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/.reuse/dep5
+-rw-rw-rw-   0        0        0     5415 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/CMakeLists.txt
+-rw-rw-rw-   0        0        0     5500 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0     2687 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    35819 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/COPYING
+-rw-rw-rw-   0        0        0     7815 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/COPYING.LESSER
+-rw-rw-rw-   0        0        0      973 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/CPPLINT.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.843108 pylibCZIrw-4.1.1/libs/libCZIrw/LICENSES/
+-rw-rw-rw-   0        0        0     1471 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/LICENSES/BSD-3-Clause.txt
+-rw-rw-rw-   0        0        0     7169 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/LICENSES/CC0-1.0.txt
+-rw-rw-rw-   0        0        0    42402 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/LICENSES/LGPL-3.0-or-later.txt
+-rw-rw-rw-   0        0        0     1087 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/LICENSES/MIT.txt
+-rw-rw-rw-   0        0        0      878 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/LICENSES/RSA-MD.txt
+-rw-rw-rw-   0        0        0     4257 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/README.md
+-rw-rw-rw-   0        0        0      814 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/SECURITY.md
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.843108 pylibCZIrw-4.1.1/libs/libCZIrw/Src/
+-rw-rw-rw-   0        0        0     2855 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/CMakeLists.txt
+-rw-rw-rw-   0        0        0   129711 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/Doxyfile
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.843108 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/
+-rw-rw-rw-   0        0        0     5138 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/CMakeLists.txt
+-rw-rw-rw-   0        0        0    20850 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/JxrDecode.cpp
+-rw-rw-rw-   0        0        0     6781 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/JxrDecode.h
+-rw-rw-rw-   0        0        0     1539 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/JxrDecode_Config.h.in
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.795982 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.795982 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/common/
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.843108 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/common/include/
+-rw-rw-rw-   0        0        0     2965 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/common/include/guiddef.h
+-rw-rw-rw-   0        0        0      500 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/common/include/log.h
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.843108 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/common/src/
+-rw-rw-rw-   0        0        0     1070 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/common/src/log.c
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.795982 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.858480 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/
+-rw-rw-rw-   0        0        0    46506 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/JXRTranscode.c
+-rw-rw-rw-   0        0        0     6737 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/decode.c
+-rw-rw-rw-   0        0        0     5153 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/decode.h
+-rw-rw-rw-   0        0        0    10548 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/postprocess.c
+-rw-rw-rw-   0        0        0    44298 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/segdec.c
+-rw-rw-rw-   0        0        0    68553 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/strInvTransform.c
+-rw-rw-rw-   0        0        0    18366 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/strPredQuantDec.c
+-rw-rw-rw-   0        0        0   150752 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/strdec.c
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.858480 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/
+-rw-rw-rw-   0        0        0     5373 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/encode.c
+-rw-rw-rw-   0        0        0     4279 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/encode.h
+-rw-rw-rw-   0        0        0    44030 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/segenc.c
+-rw-rw-rw-   0        0        0    38152 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/strFwdTransform.c
+-rw-rw-rw-   0        0        0    18689 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/strPredQuantEnc.c
+-rw-rw-rw-   0        0        0    97747 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/strenc.c
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.858480 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/
+-rw-rw-rw-   0        0        0    13131 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/adapthuff.c
+-rw-rw-rw-   0        0        0     2078 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/ansi.h
+-rw-rw-rw-   0        0        0     4872 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/common.h
+-rw-rw-rw-   0        0        0     6113 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/image.c
+-rw-rw-rw-   0        0        0    10566 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/strPredQuant.c
+-rw-rw-rw-   0        0        0     2627 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/strTransform.c
+-rw-rw-rw-   0        0        0     2377 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/strTransform.h
+-rw-rw-rw-   0        0        0    41874 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/strcodec.c
+-rw-rw-rw-   0        0        0    21813 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/strcodec.h
+-rw-rw-rw-   0        0        0    18575 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/windowsmediaphoto.h
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.858480 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/
+-rw-rw-rw-   0        0        0    33166 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRGlue.c
+-rw-rw-rw-   0        0        0    31007 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRGlue.h
+-rw-rw-rw-   0        0        0    81710 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRGlueJxr.c
+-rw-rw-rw-   0        0        0    71873 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRGluePFC.c
+-rw-rw-rw-   0        0        0    28280 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRMeta.c
+-rw-rw-rw-   0        0        0     8988 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRMeta.h
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.936610 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/
+-rw-rw-rw-   0        0        0    17269 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/BitmapOperations.cpp
+-rw-rw-rw-   0        0        0     5407 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/BitmapOperations.h
+-rw-rw-rw-   0        0        0    25778 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/BitmapOperations.hpp
+-rw-rw-rw-   0        0        0    12486 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CMakeLists.txt
+-rw-rw-rw-   0        0        0    11845 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CZIReader.cpp
+-rw-rw-rw-   0        0        0     3063 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CZIReader.h
+-rw-rw-rw-   0        0        0     3416 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CreateBitmap.cpp
+-rw-rw-rw-   0        0        0     1053 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziAttachment.cpp
+-rw-rw-rw-   0        0        0      804 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziAttachment.h
+-rw-rw-rw-   0        0        0     4873 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziAttachmentsDirectory.cpp
+-rw-rw-rw-   0        0        0     2880 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziAttachmentsDirectory.h
+-rw-rw-rw-   0        0        0     6271 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziDimensionInfo.cpp
+-rw-rw-rw-   0        0        0     3447 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziDimensionInfo.h
+-rw-rw-rw-   0        0        0    14595 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziDisplaySettings.cpp
+-rw-rw-rw-   0        0        0     1867 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziDisplaySettings.h
+-rw-rw-rw-   0        0        0     7038 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziMetadata.cpp
+-rw-rw-rw-   0        0        0     1733 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziMetadata.h
+-rw-rw-rw-   0        0        0    38124 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziMetadataBuilder.cpp
+-rw-rw-rw-   0        0        0     4798 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziMetadataBuilder.h
+-rw-rw-rw-   0        0        0    16535 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo.cpp
+-rw-rw-rw-   0        0        0     1522 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo.h
+-rw-rw-rw-   0        0        0    71829 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo2.cpp
+-rw-rw-rw-   0        0        0    41047 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo2.h
+-rw-rw-rw-   0        0        0     1668 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziMetadataSegment.cpp
+-rw-rw-rw-   0        0        0      773 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziMetadataSegment.h
+-rw-rw-rw-   0        0        0    37871 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziParse.cpp
+-rw-rw-rw-   0        0        0    10286 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziParse.h
+-rw-rw-rw-   0        0        0     4294 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziReaderCommon.cpp
+-rw-rw-rw-   0        0        0     1262 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziReaderCommon.h
+-rw-rw-rw-   0        0        0    37267 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziReaderWriter.cpp
+-rw-rw-rw-   0        0        0     7889 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziReaderWriter.h
+-rw-rw-rw-   0        0        0     7162 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziStructs.cpp
+-rw-rw-rw-   0        0        0     9712 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziStructs.h
+-rw-rw-rw-   0        0        0     2258 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziSubBlock.cpp
+-rw-rw-rw-   0        0        0     1001 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziSubBlock.h
+-rw-rw-rw-   0        0        0    23357 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziSubBlockDirectory.cpp
+-rw-rw-rw-   0        0        0     7190 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziSubBlockDirectory.h
+-rw-rw-rw-   0        0        0     6794 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziUtils.cpp
+-rw-rw-rw-   0        0        0     2510 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziUtils.h
+-rw-rw-rw-   0        0        0    60431 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziWriter.cpp
+-rw-rw-rw-   0        0        0    16641 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziWriter.h
+-rw-rw-rw-   0        0        0     8017 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/DimCoordinate.cpp
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.936610 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/
+-rw-rw-rw-   0        0        0    28556 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/CZICmd_usage.markdown
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.967861 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/
+-rw-rw-rw-   0        0        0    15042 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/CZI_1.PNG
+-rw-rw-rw-   0        0        0    11631 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/CZI_2.PNG
+-rw-rw-rw-   0        0        0   629984 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/ScalingSingleChannelTileAccessor1.png
+-rw-rw-rw-   0        0        0    15606 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_1.PNG
+-rw-rw-rw-   0        0        0     6597 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_2.PNG
+-rw-rw-rw-   0        0        0   508732 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_3.PNG
+-rw-rw-rw-   0        0        0   435548 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_4.PNG
+-rw-rw-rw-   0        0        0    22752 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/Tinting-LUT.png
+-rw-rw-rw-   0        0        0    95014 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/VisualStudio_cmake1.png
+-rw-rw-rw-   0        0        0   947057 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/ZEN_screenshot_1.PNG
+-rw-rw-rw-   0        0        0   149904 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/ZEN_screenshot_2.PNG
+-rw-rw-rw-   0        0        0   242149 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_1_raspi.PNG
+-rw-rw-rw-   0        0        0    32954 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_1_raspi_help_freetype.PNG
+-rw-rw-rw-   0        0        0   270106 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_install_raspi1.PNG
+-rw-rw-rw-   0        0        0    59883 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_raspi_unittests_1.PNG
+-rw-rw-rw-   0        0        0    14602 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/compositors_1.png
+-rw-rw-rw-   0        0        0     4107 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/compositors_2.png
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.967861 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/drawings/
+-rw-rw-rw-   0        0        0   100864 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/drawings/VS-project.pub
+-rw-rw-rw-   0        0        0   108032 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/drawings/VS-project_2.pub
+-rw-rw-rw-   0        0        0    10567 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/gradationcurve_1.PNG
+-rw-rw-rw-   0        0        0     8316 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/gradationcurve_2.PNG
+-rw-rw-rw-   0        0        0     7632 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept1.PNG
+-rw-rw-rw-   0        0        0    20658 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept2.PNG
+-rw-rw-rw-   0        0        0    14836 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept3.PNG
+-rw-rw-rw-   0        0        0    29100 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept4.PNG
+-rw-rw-rw-   0        0        0     1966 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Todos.markdown
+-rw-rw-rw-   0        0        0     2964 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/accessors.markdown
+-rw-rw-rw-   0        0        0     3817 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/building_libCZI.markdown
+-rw-rw-rw-   0        0        0    92375 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/drawings.docx
+-rw-rw-rw-   0        0        0     3983 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/image_document_concept.markdown
+-rw-rw-rw-   0        0        0     5655 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/mainpage.markdown
+-rw-rw-rw-   0        0        0     2275 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/multichannelcomposition.markdown
+-rw-rw-rw-   0        0        0    11999 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/using_libCZI.markdown
+-rw-rw-rw-   0        0        0     2849 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/version-history.markdown
+-rw-rw-rw-   0        0        0     5534 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/write_czi.markdown
+-rw-rw-rw-   0        0        0     2537 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/FileHeaderSegmentData.h
+-rw-rw-rw-   0        0        0      631 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/ImportExport.h
+-rw-rw-rw-   0        0        0     5302 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/IndexSet.cpp
+-rw-rw-rw-   0        0        0      992 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/IndexSet.h
+-rw-rw-rw-   0        0        0     8780 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/MD5Sum.cpp
+-rw-rw-rw-   0        0        0     5318 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/MD5Sum.h
+-rw-rw-rw-   0        0        0    56438 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/MultiChannelCompositor.cpp
+-rw-rw-rw-   0        0        0      166 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/MultiChannelCompositor.h
+-rw-rw-rw-   0        0        0     7936 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/SingleChannelAccessorBase.cpp
+-rw-rw-rw-   0        0        0     5951 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/SingleChannelAccessorBase.h
+-rw-rw-rw-   0        0        0    11414 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/SingleChannelPyramidLevelTileAccessor.cpp
+-rw-rw-rw-   0        0        0     2849 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/SingleChannelPyramidLevelTileAccessor.h
+-rw-rw-rw-   0        0        0    22239 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/SingleChannelScalingTileAccessor.cpp
+-rw-rw-rw-   0        0        0     3646 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/SingleChannelScalingTileAccessor.h
+-rw-rw-rw-   0        0        0     7799 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/SingleChannelTileAccessor.cpp
+-rw-rw-rw-   0        0        0     1847 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/SingleChannelTileAccessor.h
+-rw-rw-rw-   0        0        0     2095 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/SingleChannelTileCompositor.cpp
+-rw-rw-rw-   0        0        0      333 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/SingleChannelTileCompositor.h
+-rw-rw-rw-   0        0        0      187 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Site.h
+-rw-rw-rw-   0        0        0    15556 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamImpl.cpp
+-rw-rw-rw-   0        0        0     4171 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamImpl.h
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.967861 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamsLib/
+-rw-rw-rw-   0        0        0    14353 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamsLib/curlhttpinputstream.cpp
+-rw-rw-rw-   0        0        0     3121 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamsLib/curlhttpinputstream.h
+-rw-rw-rw-   0        0        0     1611 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamsLib/preadfileinputstream.cpp
+-rw-rw-rw-   0        0        0      903 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamsLib/preadfileinputstream.h
+-rw-rw-rw-   0        0        0     2296 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamsLib/simplefileinputstream.cpp
+-rw-rw-rw-   0        0        0      966 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamsLib/simplefileinputstream.h
+-rw-rw-rw-   0        0        0     9927 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamsLib/streamsFactory.cpp
+-rw-rw-rw-   0        0        0     2012 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamsLib/windowsfileinputstream.cpp
+-rw-rw-rw-   0        0        0      916 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamsLib/windowsfileinputstream.h
+-rw-rw-rw-   0        0        0    13988 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/XmlNodeWrapper.h
+-rw-rw-rw-   0        0        0     5713 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/bitmapData.h
+-rw-rw-rw-   0        0        0     3694 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/decoder.cpp
+-rw-rw-rw-   0        0        0      514 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/decoder.h
+-rw-rw-rw-   0        0        0    17564 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/decoder_wic.cpp
+-rw-rw-rw-   0        0        0      774 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/decoder_wic.h
+-rw-rw-rw-   0        0        0     7668 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/decoder_zstd.cpp
+-rw-rw-rw-   0        0        0      773 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/decoder_zstd.h
+-rw-rw-rw-   0        0        0      264 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/inc_libCZI_Config.h
+-rw-rw-rw-   0        0        0     3896 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/jxrlibcompress.cpp
+-rw-rw-rw-   0        0        0    39840 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI.h
+-rw-rw-rw-   0        0        0    42075 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Compositor.h
+-rw-rw-rw-   0        0        0     2186 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Config.h.in
+-rw-rw-rw-   0        0        0    17832 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_DimCoordinate.h
+-rw-rw-rw-   0        0        0     9650 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Helpers.h
+-rw-rw-rw-   0        0        0     4319 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Lib.cpp
+-rw-rw-rw-   0        0        0    72195 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Metadata.h
+-rw-rw-rw-   0        0        0    63505 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Metadata2.h
+-rw-rw-rw-   0        0        0    14650 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Pixels.h
+-rw-rw-rw-   0        0        0     9861 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_ReadWrite.h
+-rw-rw-rw-   0        0        0     5040 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Site.cpp
+-rw-rw-rw-   0        0        0     6262 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Site.h
+-rw-rw-rw-   0        0        0    17551 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_StreamsLib.h
+-rw-rw-rw-   0        0        0    24057 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Utilities.cpp
+-rw-rw-rw-   0        0        0    22615 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Utilities.h
+-rw-rw-rw-   0        0        0    33411 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Write.h
+-rw-rw-rw-   0        0        0    42911 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_compress.h
+-rw-rw-rw-   0        0        0    14559 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_exceptions.h
+-rw-rw-rw-   0        0        0     3060 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/pugiconfig.hpp
+-rw-rw-rw-   0        0        0   407937 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/pugixml.cpp
+-rw-rw-rw-   0        0        0    60454 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/pugixml.hpp
+-rw-rw-rw-   0        0        0     3343 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/splines.cpp
+-rw-rw-rw-   0        0        0      554 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/splines.h
+-rw-rw-rw-   0        0        0     1553 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/stdAllocator.cpp
+-rw-rw-rw-   0        0        0      593 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/stdAllocator.h
+-rw-rw-rw-   0        0        0     4792 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/subblock_cache.cpp
+-rw-rw-rw-   0        0        0     1843 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/subblock_cache.h
+-rw-rw-rw-   0        0        0    20294 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/utilities.cpp
+-rw-rw-rw-   0        0        0    10179 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/utilities.h
+-rw-rw-rw-   0        0        0    12099 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/utilities_simd.cpp
+-rw-rw-rw-   0        0        0    18572 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/zstdCompress.cpp
+-rw-rw-rw-   0        0        0     6291 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/THIRD_PARTY_LICENSES.txt
+-rw-rw-rw-   0        0        0     6882 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/cla_corporate.txt
+-rw-rw-rw-   0        0        0     6571 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/cla_individual.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.967861 pylibCZIrw-4.1.1/libs/libCZIrw/cmake/
+-rw-rw-rw-   0        0        0      990 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/cmake/ExternalEIGEN3.cmake
+-rw-rw-rw-   0        0        0     4609 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/cmake/TestLargeFile.cmake
+-rw-rw-rw-   0        0        0     1842 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/cmake/check_can_use_neon_intrinsics.cmake
+-rw-rw-rw-   0        0        0     2656 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/cmake/check_unaligned_access.cmake
+-rw-rw-rw-   0        0        0      150 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/libCZIrw/opencppcoverage.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.983485 pylibCZIrw-4.1.1/libs/pybind11/
+-rw-rw-rw-   0        0        0     1306 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.appveyor.yml
+-rw-rw-rw-   0        0        0     1034 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.clang-format
+-rw-rw-rw-   0        0        0     2682 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.clang-tidy
+-rw-rw-rw-   0        0        0     2269 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.cmake-format.yaml
+-rw-rw-rw-   0        0        0     1332 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.codespell-ignore-lines
+-rw-rw-rw-   0        0        0       41 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.git
+-rw-rw-rw-   0        0        0       19 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.gitattributes
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.983485 pylibCZIrw-4.1.1/libs/pybind11/.github/
+-rw-rw-rw-   0        0        0      191 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.github/CODEOWNERS
+-rw-rw-rw-   0        0        0    15672 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.github/CONTRIBUTING.md
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.983485 pylibCZIrw-4.1.1/libs/pybind11/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0     2622 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-rw-rw-   0        0        0      336 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-rw-   0        0        0      169 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.github/dependabot.yml
+-rw-rw-rw-   0        0        0      124 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.github/labeler.yml
+-rw-rw-rw-   0        0        0       53 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.github/labeler_merged.yml
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.983485 pylibCZIrw-4.1.1/libs/pybind11/.github/matchers/
+-rw-rw-rw-   0        0        0      700 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.github/matchers/pylint.json
+-rw-rw-rw-   0        0        0      664 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.github/pull_request_template.md
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.983485 pylibCZIrw-4.1.1/libs/pybind11/.github/workflows/
+-rw-rw-rw-   0        0        0    35326 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.github/workflows/ci.yml
+-rw-rw-rw-   0        0        0     2364 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.github/workflows/configure.yml
+-rw-rw-rw-   0        0        0     1551 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.github/workflows/format.yml
+-rw-rw-rw-   0        0        0      666 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.github/workflows/labeler.yml
+-rw-rw-rw-   0        0        0     2742 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.github/workflows/pip.yml
+-rw-rw-rw-   0        0        0     2992 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.github/workflows/upstream.yml
+-rw-rw-rw-   0        0        0      548 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.gitignore
+-rw-rw-rw-   0        0        0     3859 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0       65 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/.readthedocs.yml
+-rw-rw-rw-   0        0        0    12389 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1713 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/LICENSE
+-rw-rw-rw-   0        0        0      253 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/MANIFEST.in
+-rw-rw-rw-   0        0        0     7867 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/README.rst
+-rw-rw-rw-   0        0        0      701 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/SECURITY.md
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.999112 pylibCZIrw-4.1.1/libs/pybind11/docs/
+-rw-rw-rw-   0        0        0      628 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/Doxyfile
+-rw-rw-rw-   0        0        0     7609 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/Makefile
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.811605 pylibCZIrw-4.1.1/libs/pybind11/docs/_static/
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.999112 pylibCZIrw-4.1.1/libs/pybind11/docs/_static/css/
+-rw-rw-rw-   0        0        0       40 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/_static/css/custom.css
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.999112 pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.014735 pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/cast/
+-rw-rw-rw-   0        0        0     4018 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/cast/chrono.rst
+-rw-rw-rw-   0        0        0     3522 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/cast/custom.rst
+-rw-rw-rw-   0        0        0    14593 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/cast/eigen.rst
+-rw-rw-rw-   0        0        0     3998 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/cast/functional.rst
+-rw-rw-rw-   0        0        0     1599 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/cast/index.rst
+-rw-rw-rw-   0        0        0    12541 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/cast/overview.rst
+-rw-rw-rw-   0        0        0     9835 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/cast/stl.rst
+-rw-rw-rw-   0        0        0     9415 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/cast/strings.rst
+-rw-rw-rw-   0        0        0    49131 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/classes.rst
+-rw-rw-rw-   0        0        0     8722 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/embedding.rst
+-rw-rw-rw-   0        0        0    18197 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/exceptions.rst
+-rw-rw-rw-   0        0        0    27343 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/functions.rst
+-rw-rw-rw-   0        0        0    16051 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/misc.rst
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.014735 pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/pycpp/
+-rw-rw-rw-   0        0        0      291 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/pycpp/index.rst
+-rw-rw-rw-   0        0        0    17616 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-rw-rw-   0        0        0     9316 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/pycpp/object.rst
+-rw-rw-rw-   0        0        0     5865 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-rw-rw-   0        0        0     6551 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/smart_ptrs.rst
+-rw-rw-rw-   0        0        0     9547 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/basics.rst
+-rw-rw-rw-   0        0        0     2943 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/benchmark.py
+-rw-rw-rw-   0        0        0     3263 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/benchmark.rst
+-rw-rw-rw-   0        0        0   122400 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/changelog.rst
+-rw-rw-rw-   0        0        0    17645 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/classes.rst
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.014735 pylibCZIrw-4.1.1/libs/pybind11/docs/cmake/
+-rw-rw-rw-   0        0        0      281 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/cmake/index.rst
+-rw-rw-rw-   0        0        0    26478 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/compiling.rst
+-rw-rw-rw-   0        0        0    11942 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/conf.py
+-rw-rw-rw-   0        0        0    13601 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/faq.rst
+-rw-rw-rw-   0        0        0      661 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/index.rst
+-rw-rw-rw-   0        0        0     3382 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/installing.rst
+-rw-rw-rw-   0        0        0     3151 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/limitations.rst
+-rw-rw-rw-   0        0        0    61034 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/pybind11-logo.png
+-rw-rw-rw-   0        0        0    44653 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-rw-rw-   0        0        0    87708 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-rw-rw-   0        0        0    41121 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-rw-rw-   0        0        0    85853 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-rw-rw-   0        0        0     2777 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/reference.rst
+-rw-rw-rw-   0        0        0     4676 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/release.rst
+-rw-rw-rw-   0        0        0      155 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/requirements.txt
+-rw-rw-rw-   0        0        0    24601 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/docs/upgrade.rst
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:39.811605 pylibCZIrw-4.1.1/libs/pybind11/include/
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.014735 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/
+-rw-rw-rw-   0        0        0    25024 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/attr.h
+-rw-rw-rw-   0        0        0     7958 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/buffer_info.h
+-rw-rw-rw-   0        0        0    69016 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/cast.h
+-rw-rw-rw-   0        0        0     8683 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/chrono.h
+-rw-rw-rw-   0        0        0      122 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/common.h
+-rw-rw-rw-   0        0        0     2170 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/complex.h
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.030363 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/detail/
+-rw-rw-rw-   0        0        0    29261 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/detail/class.h
+-rw-rw-rw-   0        0        0    54735 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/detail/common.h
+-rw-rw-rw-   0        0        0     6133 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/detail/descr.h
+-rw-rw-rw-   0        0        0    18293 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/detail/init.h
+-rw-rw-rw-   0        0        0    28877 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/detail/internals.h
+-rw-rw-rw-   0        0        0    49541 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-rw-rw-   0        0        0     1690 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/detail/typeid.h
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.030363 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/eigen/
+-rw-rw-rw-   0        0        0      387 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/eigen/common.h
+-rw-rw-rw-   0        0        0    32849 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/eigen/matrix.h
+-rw-rw-rw-   0        0        0    18958 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/eigen/tensor.h
+-rw-rw-rw-   0        0        0      328 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/eigen.h
+-rw-rw-rw-   0        0        0    13775 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/embed.h
+-rw-rw-rw-   0        0        0     4887 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/eval.h
+-rw-rw-rw-   0        0        0     5139 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/functional.h
+-rw-rw-rw-   0        0        0     8501 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/gil.h
+-rw-rw-rw-   0        0        0     9127 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/iostream.h
+-rw-rw-rw-   0        0        0    81723 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/numpy.h
+-rw-rw-rw-   0        0        0     9305 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/operators.h
+-rw-rw-rw-   0        0        0     2826 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/options.h
+-rw-rw-rw-   0        0        0   129596 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/pybind11.h
+-rw-rw-rw-   0        0        0   101012 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/pytypes.h
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.030363 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/stl/
+-rw-rw-rw-   0        0        0     4301 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/stl/filesystem.h
+-rw-rw-rw-   0        0        0    15924 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/stl.h
+-rw-rw-rw-   0        0        0    30748 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/stl_bind.h
+-rw-rw-rw-   0        0        0     1990 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/type_caster_pyobject_ptr.h
+-rw-rw-rw-   0        0        0     2872 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/noxfile.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.030363 pylibCZIrw-4.1.1/libs/pybind11/pybind11/
+-rw-rw-rw-   0        0        0      446 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/pybind11/__init__.py
+-rw-rw-rw-   0        0        0     1606 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/pybind11/__main__.py
+-rw-rw-rw-   0        0        0      240 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/pybind11/_version.py
+-rw-rw-rw-   0        0        0     1244 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/pybind11/commands.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/pybind11/py.typed
+-rw-rw-rw-   0        0        0    17973 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/pybind11/setup_helpers.py
+-rw-rw-rw-   0        0        0     2396 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/pyproject.toml
+-rw-rw-rw-   0        0        0     1538 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/setup.cfg
+-rw-rw-rw-   0        0        0     5005 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.092865 pylibCZIrw-4.1.1/libs/pybind11/tests/
+-rw-rw-rw-   0        0        0    22317 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/CMakeLists.txt
+-rw-rw-rw-   0        0        0     5840 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/conftest.py
+-rw-rw-rw-   0        0        0    12058 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/constructor_stats.h
+-rw-rw-rw-   0        0        0     3686 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/cross_module_gil_utils.cpp
+-rw-rw-rw-   0        0        0     1827 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/cross_module_interleaved_error_already_set.cpp
+-rw-rw-rw-   0        0        0      410 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
+-rw-rw-rw-   0        0        0      953 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/env.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.092865 pylibCZIrw-4.1.1/libs/pybind11/tests/extra_python_package/
+-rw-rw-rw-   0        0        0        0 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/extra_python_package/pytest.ini
+-rw-rw-rw-   0        0        0     8694 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/extra_python_package/test_files.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.092865 pylibCZIrw-4.1.1/libs/pybind11/tests/extra_setuptools/
+-rw-rw-rw-   0        0        0        0 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/extra_setuptools/pytest.ini
+-rw-rw-rw-   0        0        0     4304 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-rw-rw-   0        0        0     2939 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/local_bindings.h
+-rw-rw-rw-   0        0        0     5948 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/object.h
+-rw-rw-rw-   0        0        0     6413 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-rw-rw-   0        0        0     4640 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/pybind11_tests.cpp
+-rw-rw-rw-   0        0        0     2770 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/pybind11_tests.h
+-rw-rw-rw-   0        0        0      790 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/pytest.ini
+-rw-rw-rw-   0        0        0      610 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/requirements.txt
+-rw-rw-rw-   0        0        0      880 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_async.cpp
+-rw-rw-rw-   0        0        0      560 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_async.py
+-rw-rw-rw-   0        0        0    10807 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_buffers.cpp
+-rw-rw-rw-   0        0        0     7172 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_buffers.py
+-rw-rw-rw-   0        0        0    16417 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_builtin_casters.cpp
+-rw-rw-rw-   0        0        0    17771 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_builtin_casters.py
+-rw-rw-rw-   0        0        0     4233 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_call_policies.cpp
+-rw-rw-rw-   0        0        0     6796 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_call_policies.py
+-rw-rw-rw-   0        0        0    11138 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_callbacks.cpp
+-rw-rw-rw-   0        0        0     7014 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_callbacks.py
+-rw-rw-rw-   0        0        0     3451 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_chrono.cpp
+-rw-rw-rw-   0        0        0     5896 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_chrono.py
+-rw-rw-rw-   0        0        0    25506 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_class.cpp
+-rw-rw-rw-   0        0        0    15242 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_class.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.092865 pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/
+-rw-rw-rw-   0        0        0     2665 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-rw-rw-   0        0        0      696 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/embed.cpp
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.092865 pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/installed_embed/
+-rw-rw-rw-   0        0        0     1199 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.092865 pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/installed_function/
+-rw-rw-rw-   0        0        0     1332 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.092865 pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/installed_target/
+-rw-rw-rw-   0        0        0     1731 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-rw-rw-   0        0        0      158 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/main.cpp
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.092865 pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-rw-rw-   0        0        0     1394 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.092865 pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-rw-rw-   0        0        0     1198 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.092865 pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-rw-rw-   0        0        0     1409 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-rw-rw-   0        0        0      206 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/test.py
+-rw-rw-rw-   0        0        0     3886 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_const_name.cpp
+-rw-rw-rw-   0        0        0      622 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_const_name.py
+-rw-rw-rw-   0        0        0     5864 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_constants_and_functions.cpp
+-rw-rw-rw-   0        0        0     1607 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_constants_and_functions.py
+-rw-rw-rw-   0        0        0    26597 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_copy_move.cpp
+-rw-rw-rw-   0        0        0     4928 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_copy_move.py
+-rw-rw-rw-   0        0        0     7489 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_custom_type_casters.cpp
+-rw-rw-rw-   0        0        0     4114 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_custom_type_casters.py
+-rw-rw-rw-   0        0        0     1300 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_custom_type_setup.cpp
+-rw-rw-rw-   0        0        0     1139 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_custom_type_setup.py
+-rw-rw-rw-   0        0        0     4698 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_docstring_options.cpp
+-rw-rw-rw-   0        0        0     2487 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_docstring_options.py
+-rw-rw-rw-   0        0        0    19778 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_eigen_matrix.cpp
+-rw-rw-rw-   0        0        0    29835 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_eigen_matrix.py
+-rw-rw-rw-   0        0        0      491 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_eigen_tensor.cpp
+-rw-rw-rw-   0        0        0    10923 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_eigen_tensor.inl
+-rw-rw-rw-   0        0        0     9702 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_eigen_tensor.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.092865 pylibCZIrw-4.1.1/libs/pybind11/tests/test_embed/
+-rw-rw-rw-   0        0        0     1845 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_embed/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1358 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_embed/catch.cpp
+-rw-rw-rw-   0        0        0      563 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_embed/external_module.cpp
+-rw-rw-rw-   0        0        0    17884 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-rw-rw-   0        0        0      251 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_embed/test_interpreter.py
+-rw-rw-rw-   0        0        0      291 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_embed/test_trampoline.py
+-rw-rw-rw-   0        0        0     5855 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_enum.cpp
+-rw-rw-rw-   0        0        0     9205 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_enum.py
+-rw-rw-rw-   0        0        0     3286 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_eval.cpp
+-rw-rw-rw-   0        0        0     1193 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_eval.py
+-rw-rw-rw-   0        0        0      123 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_eval_call.py
+-rw-rw-rw-   0        0        0    12429 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_exceptions.cpp
+-rw-rw-rw-   0        0        0      412 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_exceptions.h
+-rw-rw-rw-   0        0        0    14274 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_exceptions.py
+-rw-rw-rw-   0        0        0    18585 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_factory_constructors.cpp
+-rw-rw-rw-   0        0        0    17007 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_factory_constructors.py
+-rw-rw-rw-   0        0        0     5455 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_gil_scoped.cpp
+-rw-rw-rw-   0        0        0     8749 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_gil_scoped.py
+-rw-rw-rw-   0        0        0     4086 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_iostream.cpp
+-rw-rw-rw-   0        0        0     7435 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_iostream.py
+-rw-rw-rw-   0        0        0     9725 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-rw-rw-   0        0        0    13989 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_kwargs_and_defaults.py
+-rw-rw-rw-   0        0        0     4507 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_local_bindings.cpp
+-rw-rw-rw-   0        0        0     8311 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_local_bindings.py
+-rw-rw-rw-   0        0        0    22704 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_methods_and_attributes.cpp
+-rw-rw-rw-   0        0        0    18879 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_methods_and_attributes.py
+-rw-rw-rw-   0        0        0     4246 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_modules.cpp
+-rw-rw-rw-   0        0        0     4079 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_modules.py
+-rw-rw-rw-   0        0        0    12646 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_multiple_inheritance.cpp
+-rw-rw-rw-   0        0        0    12367 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_multiple_inheritance.py
+-rw-rw-rw-   0        0        0    21488 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_numpy_array.cpp
+-rw-rw-rw-   0        0        0    23554 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_numpy_array.py
+-rw-rw-rw-   0        0        0    21728 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_numpy_dtypes.cpp
+-rw-rw-rw-   0        0        0    14712 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_numpy_dtypes.py
+-rw-rw-rw-   0        0        0     4594 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_numpy_vectorize.cpp
+-rw-rw-rw-   0        0        0     9924 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_numpy_vectorize.py
+-rw-rw-rw-   0        0        0     2854 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_opaque_types.cpp
+-rw-rw-rw-   0        0        0     1905 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_opaque_types.py
+-rw-rw-rw-   0        0        0     9413 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_operator_overloading.cpp
+-rw-rw-rw-   0        0        0     4483 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_operator_overloading.py
+-rw-rw-rw-   0        0        0     6913 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_pickling.cpp
+-rw-rw-rw-   0        0        0     2813 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_pickling.py
+-rw-rw-rw-   0        0        0    31911 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_pytypes.cpp
+-rw-rw-rw-   0        0        0    24790 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_pytypes.py
+-rw-rw-rw-   0        0        0    21734 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-rw-rw-   0        0        0     8291 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_sequences_and_iterators.py
+-rw-rw-rw-   0        0        0    19368 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_smart_ptr.cpp
+-rw-rw-rw-   0        0        0     9845 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_smart_ptr.py
+-rw-rw-rw-   0        0        0    22138 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_stl.cpp
+-rw-rw-rw-   0        0        0    12688 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_stl.py
+-rw-rw-rw-   0        0        0     6401 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_stl_binders.cpp
+-rw-rw-rw-   0        0        0    10159 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_stl_binders.py
+-rw-rw-rw-   0        0        0     4764 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-rw-rw-   0        0        0      769 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_tagbased_polymorphic.py
+-rw-rw-rw-   0        0        0     1921 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_thread.cpp
+-rw-rw-rw-   0        0        0      868 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_thread.py
+-rw-rw-rw-   0        0        0     4631 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_type_caster_pyobject_ptr.cpp
+-rw-rw-rw-   0        0        0     3364 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_type_caster_pyobject_ptr.py
+-rw-rw-rw-   0        0        0      625 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_union.cpp
+-rw-rw-rw-   0        0        0      156 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_union.py
+-rw-rw-rw-   0        0        0      883 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_unnamed_namespace_a.cpp
+-rw-rw-rw-   0        0        0     1175 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_unnamed_namespace_a.py
+-rw-rw-rw-   0        0        0      354 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_unnamed_namespace_b.cpp
+-rw-rw-rw-   0        0        0      148 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_unnamed_namespace_b.py
+-rw-rw-rw-   0        0        0     1525 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_vector_unique_ptr_member.cpp
+-rw-rw-rw-   0        0        0      343 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_vector_unique_ptr_member.py
+-rw-rw-rw-   0        0        0    23583 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_virtual_functions.cpp
+-rw-rw-rw-   0        0        0    13371 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/test_virtual_functions.py
+-rw-rw-rw-   0        0        0     3366 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-rw-rw-   0        0        0     2774 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tests/valgrind-python.supp
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.108487 pylibCZIrw-4.1.1/libs/pybind11/tools/
+-rw-rw-rw-   0        0        0     2525 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tools/FindCatch.cmake
+-rw-rw-rw-   0        0        0     3191 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tools/FindEigen3.cmake
+-rw-rw-rw-   0        0        0    11477 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tools/FindPythonLibsNew.cmake
+-rw-rw-rw-   0        0        0      840 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tools/JoinPaths.cmake
+-rw-rw-rw-   0        0        0     1467 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tools/check-style.sh
+-rw-rw-rw-   0        0        0      975 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tools/cmake_uninstall.cmake.in
+-rw-rw-rw-   0        0        0     1156 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-rw-rw-   0        0        0     1067 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tools/libsize.py
+-rw-rw-rw-   0        0        0     1373 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tools/make_changelog.py
+-rw-rw-rw-   0        0        0      203 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tools/pybind11.pc.in
+-rw-rw-rw-   0        0        0    14854 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tools/pybind11Common.cmake
+-rw-rw-rw-   0        0        0     7334 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tools/pybind11Config.cmake.in
+-rw-rw-rw-   0        0        0     9216 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tools/pybind11NewTools.cmake
+-rw-rw-rw-   0        0        0     8594 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tools/pybind11Tools.cmake
+-rw-rw-rw-   0        0        0       97 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tools/pyproject.toml
+-rw-rw-rw-   0        0        0     2167 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tools/setup_global.py.in
+-rw-rw-rw-   0        0        0     1278 2024-05-23 16:16:46.000000 pylibCZIrw-4.1.1/libs/pybind11/tools/setup_main.py.in
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.108487 pylibCZIrw-4.1.1/pylibCZIrw/
+-rw-rw-rw-   0        0        0      896 2024-05-23 16:16:40.000000 pylibCZIrw-4.1.1/pylibCZIrw/__init__.py
+-rw-rw-rw-   0        0        0    50379 2024-05-23 16:16:40.000000 pylibCZIrw-4.1.1/pylibCZIrw/czi.py
+-rw-rw-rw-   0        0        0   575191 2024-05-23 16:16:40.000000 pylibCZIrw-4.1.1/pylibCZIrw-documentation.html
+drwxrwxrwx   0        0        0        0 2024-05-23 16:17:40.108487 pylibCZIrw-4.1.1/pylibCZIrw.egg-info/
+-rw-rw-rw-   0        0        0     3689 2024-05-23 16:17:39.000000 pylibCZIrw-4.1.1/pylibCZIrw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    22592 2024-05-23 16:17:39.000000 pylibCZIrw-4.1.1/pylibCZIrw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 16:17:39.000000 pylibCZIrw-4.1.1/pylibCZIrw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-23 16:17:39.000000 pylibCZIrw-4.1.1/pylibCZIrw.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       33 2024-05-23 16:17:39.000000 pylibCZIrw-4.1.1/pylibCZIrw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-23 16:17:39.000000 pylibCZIrw-4.1.1/pylibCZIrw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1683 2024-05-23 16:17:40.108487 pylibCZIrw-4.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     9364 2024-05-23 16:16:40.000000 pylibCZIrw-4.1.1/setup.py
```

### Comparing `pylibCZIrw-4.1.0/CMakeLists.txt` & `pylibCZIrw-4.1.1/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 cmake_minimum_required(VERSION 3.11)
 
 cmake_policy(SET CMP0091 NEW) # enable new "MSVC runtime library selection" (https://cmake.org/cmake/help/latest/variable/CMAKE_MSVC_RUNTIME_LIBRARY.html)
 
-project(_pylibCZIrw VERSION 4.1.0)
+project(_pylibCZIrw VERSION 4.1.1)
 
 # Set library version in the code
 configure_file(${CMAKE_CURRENT_SOURCE_DIR}/_pylibCZIrw/src/pylibCZIrw_Config.h.in ${CMAKE_CURRENT_SOURCE_DIR}/_pylibCZIrw/src/pylibCZIrw_Config.h @ONLY)
 
  # Instruct to use the static-version of the runtime library (on Windows) -> c.f. https://cmake.org/cmake/help/latest/variable/CMAKE_MSVC_RUNTIME_LIBRARY.html
 set(CMAKE_MSVC_RUNTIME_LIBRARY "MultiThreaded$<$<CONFIG:Debug>:Debug>")
```

### Comparing `pylibCZIrw-4.1.0/CMakeSettings.json` & `pylibCZIrw-4.1.1/CMakeSettings.json`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/COPYING.LESSER.txt` & `pylibCZIrw-4.1.1/COPYING.LESSER.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/COPYING.txt` & `pylibCZIrw-4.1.1/COPYING.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/INFO.md` & `pylibCZIrw-4.1.1/INFO.md`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/PKG-INFO` & `pylibCZIrw-4.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibCZIrw
-Version: 4.1.0
+Version: 4.1.1
 Summary: A python wrapper around the libCZI C++ library with reading and writing functionality.
 Author: Sebastian Soyer
 Author-email: sebastian.soyer@zeiss.com
 Keywords: czi,imaging
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pylibCZIrw-4.1.0/_pylibCZIrw/src/api/CMakeLists.txt` & `pylibCZIrw-4.1.1/_pylibCZIrw/src/api/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/_pylibCZIrw/src/api/CZIreadAPI.cpp` & `pylibCZIrw-4.1.1/_pylibCZIrw/src/api/CZIreadAPI.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/_pylibCZIrw/src/api/CZIreadAPI.h` & `pylibCZIrw-4.1.1/_pylibCZIrw/src/api/CZIreadAPI.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/_pylibCZIrw/src/api/CZIwriteAPI.cpp` & `pylibCZIrw-4.1.1/_pylibCZIrw/src/api/CZIwriteAPI.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/_pylibCZIrw/src/api/CZIwriteAPI.h` & `pylibCZIrw-4.1.1/_pylibCZIrw/src/api/CZIwriteAPI.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/_pylibCZIrw/src/api/PImage.cpp` & `pylibCZIrw-4.1.1/_pylibCZIrw/src/api/PImage.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/_pylibCZIrw/src/api/PImage.h` & `pylibCZIrw-4.1.1/_pylibCZIrw/src/api/PImage.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/_pylibCZIrw/src/api/StaticContext.cpp` & `pylibCZIrw-4.1.1/_pylibCZIrw/src/api/StaticContext.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/_pylibCZIrw/src/api/StaticContext.h` & `pylibCZIrw-4.1.1/_pylibCZIrw/src/api/StaticContext.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/_pylibCZIrw/src/api/SubBlockCache.h` & `pylibCZIrw-4.1.1/_pylibCZIrw/src/api/SubBlockCache.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/_pylibCZIrw/src/api/site.cpp` & `pylibCZIrw-4.1.1/_pylibCZIrw/src/api/site.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/_pylibCZIrw/src/bindings/CZIrw.cpp` & `pylibCZIrw-4.1.1/_pylibCZIrw/src/bindings/CZIrw.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/_pylibCZIrw/src/bindings/PbHelper.cpp` & `pylibCZIrw-4.1.1/_pylibCZIrw/src/bindings/PbHelper.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/_pylibCZIrw/src/bindings/PbHelper.h` & `pylibCZIrw-4.1.1/_pylibCZIrw/src/bindings/PbHelper.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/_pylibCZIrw/src/bindings/include_python.h` & `pylibCZIrw-4.1.1/_pylibCZIrw/src/bindings/include_python.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/_pylibCZIrw/tests/main.cpp` & `pylibCZIrw-4.1.1/_pylibCZIrw/tests/main.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/.devcontainer/Dockerfile` & `pylibCZIrw-4.1.1/libs/libCZIrw/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/.devcontainer/devcontainer.json` & `pylibCZIrw-4.1.1/libs/libCZIrw/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/.devcontainer/reinstall-cmake.sh` & `pylibCZIrw-4.1.1/libs/libCZIrw/.devcontainer/reinstall-cmake.sh`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/.editorconfig` & `pylibCZIrw-4.1.1/libs/libCZIrw/.editorconfig`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/.github/ISSUE_TEMPLATE/bug_report.md` & `pylibCZIrw-4.1.1/libs/libCZIrw/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/.github/ISSUE_TEMPLATE/feature_request.md` & `pylibCZIrw-4.1.1/libs/libCZIrw/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/.github/PULL_REQUEST_TEMPLATE.md` & `pylibCZIrw-4.1.1/libs/libCZIrw/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/.github/codecov.yml` & `pylibCZIrw-4.1.1/libs/libCZIrw/.github/codecov.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/.github/workflows/cla.yml` & `pylibCZIrw-4.1.1/libs/libCZIrw/.github/workflows/cla.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/.github/workflows/cmake.yml` & `pylibCZIrw-4.1.1/libs/libCZIrw/.github/workflows/cmake.yml`

 * *Files 6% similar despite different names*

```diff
@@ -69,26 +69,27 @@
         # Use debug flag to show all exeucted tests
         run: ctest --debug -C ${{matrix.build}}
 
       # Coverage collection based on https://about.codecov.io/blog/how-to-set-up-codecov-with-c-plus-plus-and-github-actions/
       - name: Prepare Coverage
         if: ${{ (matrix.OS == 'windows-latest') && ( matrix.build == 'Debug') }}
         run: |
-          choco install OpenCppCoverage -y
+          choco install OpenCppCoverage -y --no-progress
           echo "C:\Program Files\OpenCppCoverage" >> "$env:GITHUB_PATH"
 
       - name: Get Coverage
         if: ${{ (matrix.OS == 'windows-latest') && ( matrix.build == 'Debug') }}
         working-directory: ${{github.workspace}}/build/Src/libCZI_UnitTests/${{matrix.build}}
         shell: cmd
         run: OpenCppCoverage.exe --export_type cobertura:${{github.workspace}}\coverage.xml --config_file "${{github.workspace}}\opencppcoverage.txt" -- libCZI_UnitTests.exe
 
       - name: Upload Coverage
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         if: ${{ (matrix.OS == 'windows-latest') && ( matrix.build == 'Debug') }}
         with:
           files: ./coverage.xml
           fail_ci_if_error: true
           verbose: true
           # Only one flag to be safe with
           # https://docs.codecov.com/docs/flags#one-to-one-relationship-of-flags-to-uploads
           flags: ${{matrix.OS}}
+          token: e9a842e5-9f84-48a6-9320-8f67a28f0260 #gitleaks:allow
```

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/.github/workflows/codeql.yml` & `pylibCZIrw-4.1.1/libs/libCZIrw/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/.github/workflows/mega-linter.yml` & `pylibCZIrw-4.1.1/libs/libCZIrw/.github/workflows/mega-linter.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/.github/workflows/pages.yml` & `pylibCZIrw-4.1.1/libs/libCZIrw/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/.gitignore` & `pylibCZIrw-4.1.1/libs/libCZIrw/.gitignore`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/.mega-linter.yml` & `pylibCZIrw-4.1.1/libs/libCZIrw/.mega-linter.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/.reuse/dep5` & `pylibCZIrw-4.1.1/libs/libCZIrw/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/CMakeLists.txt` & `pylibCZIrw-4.1.1/libs/libCZIrw/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 cmake_minimum_required(VERSION 3.15)
 
 cmake_policy(SET CMP0091 NEW) # enable new "MSVC runtime library selection" (https://cmake.org/cmake/help/latest/variable/CMAKE_MSVC_RUNTIME_LIBRARY.html)
 
 project(libCZI 
-      VERSION 0.57.2
+      VERSION 0.58.4
       HOMEPAGE_URL "https://github.com/ZEISS/libczi"
       DESCRIPTION "libCZI is an Open Source Cross-Platform C++ library to read and write CZI")
 
 list (APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/cmake")
 
 include(GNUInstallDirs)
```

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/CODE_OF_CONDUCT.md` & `pylibCZIrw-4.1.1/libs/libCZIrw/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/CONTRIBUTING.md` & `pylibCZIrw-4.1.1/libs/libCZIrw/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/COPYING` & `pylibCZIrw-4.1.1/libs/libCZIrw/COPYING`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/COPYING.LESSER` & `pylibCZIrw-4.1.1/libs/libCZIrw/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/CPPLINT.cfg` & `pylibCZIrw-4.1.1/libs/libCZIrw/CPPLINT.cfg`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/LICENSES/BSD-3-Clause.txt` & `pylibCZIrw-4.1.1/libs/libCZIrw/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/LICENSES/CC0-1.0.txt` & `pylibCZIrw-4.1.1/libs/libCZIrw/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/LICENSES/LGPL-3.0-or-later.txt` & `pylibCZIrw-4.1.1/libs/libCZIrw/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/LICENSES/MIT.txt` & `pylibCZIrw-4.1.1/libs/libCZIrw/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/LICENSES/RSA-MD.txt` & `pylibCZIrw-4.1.1/libs/libCZIrw/LICENSES/RSA-MD.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/README.md` & `pylibCZIrw-4.1.1/libs/libCZIrw/README.md`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/SECURITY.md` & `pylibCZIrw-4.1.1/libs/libCZIrw/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/CMakeLists.txt` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/Doxyfile` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/Doxyfile`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/CMakeLists.txt` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/JxrDecode.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/JxrDecode.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/JxrDecode.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/JxrDecode.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/JxrDecode_Config.h.in` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/JxrDecode_Config.h.in`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/common/include/guiddef.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/common/include/guiddef.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/common/src/log.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/common/src/log.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/JXRTranscode.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/JXRTranscode.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/decode.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/decode.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/decode.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/decode.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/postprocess.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/postprocess.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/segdec.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/segdec.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/strInvTransform.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/strInvTransform.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/strPredQuantDec.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/strPredQuantDec.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/strdec.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/decode/strdec.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/encode.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/encode.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/encode.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/encode.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/segenc.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/segenc.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/strFwdTransform.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/strFwdTransform.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/strPredQuantEnc.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/strPredQuantEnc.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/strenc.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/encode/strenc.c`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
                 putBit16(pIO, pTile->cNumQPLP - 1, 4);
 
                 pTile->cBitsLP = dquantBits(pTile->cNumQPLP);
 
                 for (i = 0; i < pTile->cNumQPLP; i++) {
                     pTile->cChModeLP[i] = (U8)(rand() & 3); // channel mode, just for concept proofing!
 
-                    for (j = 0; j < pSC->m_param.cNumChannels; j++)
+                    for (j = 0; j < (U8)pSC->m_param.cNumChannels; j++)
                         pTile->pQuantizerLP[j][i].iIndex = (U8)((rand() & 0xfe) + 1); // QP indexes, just for concept proofing!
                     formatQuantizer(pTile->pQuantizerLP, pTile->cChModeLP[i], pSC->m_param.cNumChannels, i, TRUE, pSC->m_param.bScaledArith);
                     writeQuantizer(pTile->pQuantizerLP, pIO, pTile->cChModeLP[i], pSC->m_param.cNumChannels, i);
                 }
             }
         }
         pSC = pSC->m_pNextSC;
@@ -185,15 +185,15 @@
             else {
                 putBit16(pIO, pTile->cNumQPHP - 1, 4);
                 pTile->cBitsHP = dquantBits(pTile->cNumQPHP);
 
                 for (i = 0; i < pTile->cNumQPHP; i++) {
                     pTile->cChModeHP[i] = (U8)(rand() & 3); // channel mode, just for concept proofing!
 
-                    for (j = 0; j < pSC->m_param.cNumChannels; j++)
+                    for (j = 0; j < (U8)pSC->m_param.cNumChannels; j++)
                         pTile->pQuantizerHP[j][i].iIndex = (U8)((rand() & 0xfe) + 1); // QP indexes, just for concept proofing!
                     formatQuantizer(pTile->pQuantizerHP, pTile->cChModeHP[i], pSC->m_param.cNumChannels, i, FALSE, pSC->m_param.bScaledArith);
                     writeQuantizer(pTile->pQuantizerHP, pIO, pTile->cChModeHP[i], pSC->m_param.cNumChannels, i);
                 }
             }
         }
         pSC = pSC->m_pNextSC;
```

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/adapthuff.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/adapthuff.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/ansi.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/ansi.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/common.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/common.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/image.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/image.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/strPredQuant.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/strPredQuant.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/strTransform.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/strTransform.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/strTransform.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/strTransform.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/strcodec.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/strcodec.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/strcodec.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/strcodec.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/windowsmediaphoto.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/image/sys/windowsmediaphoto.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRGlue.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRGlue.c`

 * *Files 0% similar despite different names*

```diff
@@ -674,15 +674,15 @@
     if (&GUID_PKPixelFormat12bppYUV420 == pPITo.pGUIDPixFmt
         || &GUID_PKPixelFormat16bppYUV422 == pPITo.pGUIDPixFmt)
         cbStrideTo >>= 1;
 
     cbStride = cbStrideFrom > cbStrideTo ? cbStrideFrom : cbStrideTo;//  max(cbStrideFrom, cbStrideTo);
 
     // actual dec/enc with local buffer
-    Call(PKAllocAligned((void**)&pb, cbStride * pRect->Height, 128));
+    Call(PKAllocAligned((void**)&pb, (size_t)cbStride * pRect->Height, 128));
 
     Call(pFC->Copy(pFC, pRect, pb, cbStride));
 
     Call(pIE->WritePixels(pIE, pRect->Height, pb, cbStride));
 
 Cleanup:
     PKFreeAligned((void**)&pb);
@@ -775,15 +775,15 @@
         cParam.bIgnoreOverlap = pFC->pDecoder->WMP.bIgnoreOverlap;
 
         Call(pIE->Transcode(pIE, pFC->pDecoder, &cParam));
     }
     else
     {
         // actual dec/enc with local buffer
-        Call(PKAllocAligned((void**)&pb, cbStride * pRect->Height, 128));
+        Call(PKAllocAligned((void**)&pb, (size_t)cbStride * pRect->Height, 128));
         Call(pFC->Copy(pFC, pRect, pb, cbStride));
         Call(pIE->WritePixels(pIE, pRect->Height, pb, cbStride));
     }
 
 Cleanup:
     PKFreeAligned((void**)&pb);
     return err;
```

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRGlue.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRGlue.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRGlueJxr.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRGlueJxr.c`

 * *Files 0% similar despite different names*

```diff
@@ -2046,15 +2046,15 @@
                 // update cMBRow if whole MB row cropped
                 cMBRow++;
             }
         }
         wmiBI.pv = pbLowMemAdj;
 
         // If we're past the top of the image, then we're done, so terminate.
-        if (linesperMBRow * (cMBRow - 1) >= (U32)pID->WMP.cLinesCropped + pID->WMP.wmiI.cROIHeight) {
+        if (linesperMBRow * (size_t)(cMBRow - 1) >= pID->WMP.cLinesCropped + pID->WMP.wmiI.cROIHeight) {
             FailIf(ICERR_OK != ImageStrDecTerm(pID->WMP.ctxSC), WMP_errFail);
         }
         pID->WMP.DecoderCurrMBRow = cMBRow; // Set to next possible MBRow that is decodable
 
 #else
         FailIf(ICERR_OK != ImageStrDecInit(&pID->WMP.wmiI, &pID->WMP.wmiSCP, &pID->WMP.ctxSC), WMP_errFail);
         FailIf(ICERR_OK != ImageStrDecDecode(pID->WMP.ctxSC, &wmiBI), WMP_errFail);
@@ -2128,15 +2128,15 @@
             size_t cLinesDecoded;
             wmiBI.uiFirstMBRow = i;
             wmiBI.uiLastMBRow = i;
             FailIf(ICERR_OK != ImageStrDecDecode(pID->WMP.ctxSC_Alpha, &wmiBI, &cLinesDecoded), WMP_errFail);
         }
 
         // If we're past the top of the image, then we're done, so terminate
-        if (linesperMBRow * (cMBRow - 1) >= (U32)pID->WMP.cLinesCropped + pID->WMP.wmiI.cROIHeight) {
+        if (linesperMBRow * (size_t)(cMBRow - 1) >= pID->WMP.cLinesCropped + pID->WMP.wmiI.cROIHeight) {
             FailIf(ICERR_OK != ImageStrDecTerm(pID->WMP.ctxSC_Alpha), WMP_errFail);
         }
         pID->WMP.DecoderCurrAlphaMBRow = cMBRow; // Set to next possible MBRow that is decodable
         wmiBI.pv = pb;
 #else
         FailIf(ICERR_OK != ImageStrDecInit(&pID->WMP.wmiI_Alpha, &pID->WMP.wmiSCP_Alpha, &pID->WMP.ctxSC_Alpha), WMP_errFail);
         FailIf(ICERR_OK != ImageStrDecDecode(pID->WMP.ctxSC_Alpha, &wmiBI), WMP_errFail);
```

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRGluePFC.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRGluePFC.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRMeta.c` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRMeta.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRMeta.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/JxrDecode/jxrlib/jxrgluelib/JXRMeta.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/BitmapOperations.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/BitmapOperations.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/BitmapOperations.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/BitmapOperations.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/BitmapOperations.hpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/BitmapOperations.hpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CMakeLists.txt` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
             CziMetadata.cpp
             CziMetadataBuilder.cpp
             CziMetadataDocumentInfo.cpp
             CziMetadataDocumentInfo2.cpp
             CziMetadataSegment.cpp
             CziParse.cpp
             CZIReader.cpp
+            CziReaderCommon.cpp
             CziReaderWriter.cpp
             CziStructs.cpp
             CziSubBlock.cpp
             CziSubBlockDirectory.cpp
             CziUtils.cpp
             CziWriter.cpp
             decoder.cpp
@@ -56,14 +57,15 @@
             CziDisplaySettings.h
             CziMetadata.h
             CziMetadataBuilder.h
             CziMetadataDocumentInfo.h
             CziMetadataDocumentInfo2.h
             CziMetadataSegment.h
             CziParse.h
+            CziReaderCommon.h
             CZIReader.h
             CziReaderWriter.h
             CziStructs.h
             CziSubBlock.h
             CziSubBlockDirectory.h
             CziUtils.h
             CziWriter.h
@@ -226,15 +228,15 @@
 
 if (LIBCZI_BUILD_PREFER_EXTERNALPACKAGE_ZSTD)
   find_package(zstd CONFIG REQUIRED)
 else()
   FetchContent_Declare(
     zstd
     GIT_REPOSITORY https://github.com/facebook/zstd.git
-    GIT_TAG "v1.5.5"
+    GIT_TAG "v1.5.6"
   )
 
   if(NOT zstd_POPULATED)
     message(STATUS "Fetching zstd...")
     set(ZSTD_BUILD_PROGRAMS  OFF CACHE BOOL "" FORCE)
     set(ZSTD_BUILD_SHARED    OFF CACHE BOOL "" FORCE)
     set(ZSTD_BUILD_TESTS     OFF CACHE BOOL "" FORCE)
```

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CZIReader.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CZIReader.cpp`

 * *Files 25% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 #include "CZIReader.h"
 #include "CziParse.h"
 #include "CziSubBlock.h"
 #include "CziMetadataSegment.h"
 #include "CziUtils.h"
 #include "utilities.h"
 #include "CziAttachment.h"
+#include "CziReaderCommon.h"
 
 using namespace std;
 using namespace libCZI;
 
 static CCZIParse::SubblockDirectoryParseOptions GetParseOptionsFromOpenOptions(const ICZIReader::OpenOptions& options)
 {
     CCZIParse::SubblockDirectoryParseOptions parse_options;
@@ -97,23 +98,15 @@
 
 /*virtual*/void CCZIReader::EnumerateSubBlocks(const std::function<bool(int index, const SubBlockInfo& info)>& funcEnum)
 {
     this->ThrowIfNotOperational();
     this->subBlkDir.EnumSubBlocks(
         [&](int index, const CCziSubBlockDirectory::SubBlkEntry& entry)->bool
         {
-            SubBlockInfo info;
-            info.compressionModeRaw = entry.Compression;
-            info.pixelType = CziUtils::PixelTypeFromInt(entry.PixelType);
-            info.coordinate = entry.coordinate;
-            info.logicalRect = IntRect{ entry.x,entry.y,entry.width,entry.height };
-            info.physicalSize = IntSize{ (std::uint32_t)entry.storedWidth, (std::uint32_t)entry.storedHeight };
-            info.mIndex = entry.mIndex;
-            info.pyramidType = CziUtils::PyramidTypeFromByte(entry.pyramid_type_from_spare);
-            return funcEnum(index, info);
+            return funcEnum(index, CziReaderCommon::ConvertToSubBlockInfo(entry));
         });
 }
 
 /*virtual*/void CCZIReader::EnumerateSubBlocksEx(const std::function<bool(int index, const DirectorySubBlockInfo& info)>& funcEnum)
 {
     this->ThrowIfNotOperational();
     this->subBlkDir.EnumSubBlocks(
@@ -131,38 +124,15 @@
             return funcEnum(index, info);
         });
 }
 
 /*virtual*/void CCZIReader::EnumSubset(const IDimCoordinate* planeCoordinate, const IntRect* roi, bool onlyLayer0, const std::function<bool(int index, const SubBlockInfo& info)>& funcEnum)
 {
     this->ThrowIfNotOperational();
-
-    // TODO:
-    // Ok... for a first tentative, experimental and quick-n-dirty implementation, simply
-    //      walk through all the subblocks. We surely want to have something more elaborated
-    //      here.
-    this->EnumerateSubBlocks(
-        [&](int index, const SubBlockInfo& info)->bool
-        {
-            // TODO: we only deal with layer 0 currently... or, more precisely, we do not take "zoom" into account at all
-            //        -> well... added that boolean "onlyLayer0" - is this sufficient...?
-            if (onlyLayer0 == false || (info.physicalSize.w == info.logicalRect.w && info.physicalSize.h == info.logicalRect.h))
-            {
-                if (planeCoordinate == nullptr || CziUtils::CompareCoordinate(planeCoordinate, &info.coordinate) == true)
-                {
-                    if (roi == nullptr || Utilities::DoIntersect(*roi, info.logicalRect))
-                    {
-                        bool b = funcEnum(index, info);
-                        return b;
-                    }
-                }
-            }
-
-            return true;
-        });
+    CziReaderCommon::EnumSubset(this, planeCoordinate, roi, onlyLayer0, funcEnum);
 }
 
 /*virtual*/std::shared_ptr<ISubBlock> CCZIReader::ReadSubBlock(int index)
 {
     this->ThrowIfNotOperational();
     CCziSubBlockDirectory::SubBlkEntry entry;
     if (this->subBlkDir.TryGetSubBlock(index, entry) == false)
@@ -172,68 +142,28 @@
 
     return this->ReadSubBlock(entry);
 }
 
 /*virtual*/bool CCZIReader::TryGetSubBlockInfoOfArbitrarySubBlockInChannel(int channelIndex, SubBlockInfo& info)
 {
     this->ThrowIfNotOperational();
-
-    // TODO: we should be able to gather this information when constructing the subblock-list
-    //  for the time being... just walk through the whole list
-    //  
-    bool foundASubBlock = false;
-    SubBlockStatistics s = this->subBlkDir.GetStatistics();
-    if (!s.dimBounds.IsValid(DimensionIndex::C))
-    {
-        // in this case -> just take the first subblock...
-        this->EnumerateSubBlocks(
-            [&](int index, const SubBlockInfo& sbinfo)->bool
-            {
-                info = sbinfo;
-                foundASubBlock = true;
-                return false;
-            });
-    }
-    else
-    {
-        this->EnumerateSubBlocks(
-            [&](int index, const SubBlockInfo& sbinfo)->bool
-            {
-                int c;
-                if (sbinfo.coordinate.TryGetPosition(DimensionIndex::C, &c) == true && c == channelIndex)
-                {
-                    info = sbinfo;
-                    foundASubBlock = true;
-                    return false;
-                }
-
-                return true;
-            });
-    }
-
-    return foundASubBlock;
+    return CziReaderCommon::TryGetSubBlockInfoOfArbitrarySubBlockInChannel(this, channelIndex, info);
 }
 
 /*virtual*/bool CCZIReader::TryGetSubBlockInfo(int index, SubBlockInfo* info) const
 {
     CCziSubBlockDirectory::SubBlkEntry entry;
     if (this->subBlkDir.TryGetSubBlock(index, entry) == false)
     {
         return false;
     }
 
     if (info != nullptr)
     {
-        info->compressionModeRaw = entry.Compression;
-        info->pixelType = CziUtils::PixelTypeFromInt(entry.PixelType);
-        info->coordinate = entry.coordinate;
-        info->logicalRect = IntRect{ entry.x,entry.y,entry.width,entry.height };
-        info->physicalSize = IntSize{ static_cast<std::uint32_t>(entry.storedWidth), static_cast<std::uint32_t>(entry.storedHeight) };
-        info->mIndex = entry.mIndex;
-        info->pyramidType = CziUtils::PyramidTypeFromByte(entry.pyramid_type_from_spare);
+        *info = CziReaderCommon::ConvertToSubBlockInfo(entry);
     }
 
     return true;
 }
 
 /*virtual*/std::shared_ptr<libCZI::IAccessor> CCZIReader::CreateAccessor(libCZI::AccessorType accessorType)
 {
@@ -269,33 +199,19 @@
             return b;
         });
 }
 
 /*virtual*/void CCZIReader::EnumerateSubset(const char* contentFileType, const char* name, const std::function<bool(int index, const libCZI::AttachmentInfo& info)>& funcEnum)
 {
     this->ThrowIfNotOperational();
-    libCZI::AttachmentInfo ai;
-    ai.contentFileType[sizeof(ai.contentFileType) - 1] = '\0';
-    this->attachmentDir.EnumAttachments(
-        [&](int index, const CCziAttachmentsDirectory::AttachmentEntry& ae)
-        {
-            if (contentFileType == nullptr || strcmp(contentFileType, ae.ContentFileType) == 0)
-            {
-                if (name == nullptr || strcmp(name, ae.Name) == 0)
-                {
-                    ai.contentGuid = ae.ContentGuid;
-                    memcpy(ai.contentFileType, ae.ContentFileType, sizeof(ae.ContentFileType));
-                    ai.name = ae.Name;
-                    bool b = funcEnum(index, ai);
-                    return b;
-                }
-            }
-
-            return true;
-        });
+    CziReaderCommon::EnumerateSubset(
+        std::bind(&CCziAttachmentsDirectory::EnumAttachments, &this->attachmentDir, std::placeholders::_1),
+        contentFileType, 
+        name, 
+        funcEnum);
 }
 
 /*virtual*/std::shared_ptr<libCZI::IAttachment> CCZIReader::ReadAttachment(int index)
 {
     this->ThrowIfNotOperational();
     CCziAttachmentsDirectory::AttachmentEntry entry;
     if (this->attachmentDir.TryGetAttachment(index, entry) == false)
```

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CZIReader.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CZIReader.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CreateBitmap.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CreateBitmap.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziAttachment.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziAttachment.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziAttachment.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziAttachment.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziAttachmentsDirectory.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziAttachmentsDirectory.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziAttachmentsDirectory.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziAttachmentsDirectory.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziDimensionInfo.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziDimensionInfo.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziDimensionInfo.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziDimensionInfo.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziDisplaySettings.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziDisplaySettings.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziDisplaySettings.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziDisplaySettings.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziMetadata.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziMetadata.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziMetadata.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziMetadata.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziMetadataBuilder.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziMetadataBuilder.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziMetadataBuilder.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziMetadataBuilder.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo2.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo2.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo2.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo2.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziMetadataSegment.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziMetadataSegment.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziMetadataSegment.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziMetadataSegment.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziParse.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziParse.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,15 @@
     CCZIParse::ReadAttachmentsDirectory(str, offset, [&](const CCziAttachmentsDirectoryBase::AttachmentEntry& ae)->void {attDir.AddAttachmentEntry(ae); }, nullptr);
     return attDir;
 }
 
 /*static*/void CCZIParse::ReadAttachmentsDirectory(libCZI::IStream* str, std::uint64_t offset, const std::function<void(const CCziAttachmentsDirectoryBase::AttachmentEntry&)>& addFunc, SegmentSizes* segmentSizes/*= nullptr*/)
 {
     AttachmentDirectorySegment attachmentDirSegment;
-    std::uint64_t bytesRead;
+    uint64_t bytesRead;
     try
     {
         str->Read(offset, &attachmentDirSegment, sizeof(attachmentDirSegment), &bytesRead);
     }
     catch (const std::exception&)
     {
         std::throw_with_nested(LibCZIIOException("Error reading AttachmentDirectorySegment", offset, sizeof(attachmentDirSegment)));
@@ -197,53 +197,57 @@
     {
         segmentSizes->UsedSize = attachmentDirSegment.header.UsedSize;
         segmentSizes->AllocatedSize = attachmentDirSegment.header.AllocatedSize;
     }
 
     // TODO: we can add a couple of consistency checks here
 
-    // now read the AttachmentEntries
-    std::uint64_t attachmentEntriesSize = ((std::uint64_t)attachmentDirSegment.data.EntryCount) * sizeof(AttachmentEntryA1);
-
-    std::unique_ptr<AttachmentEntryA1, decltype(free)*> pBuffer((AttachmentEntryA1*)malloc((size_t)attachmentEntriesSize), free);
-
-    // now read the attachment-entries
-    try
-    {
-        str->Read(offset + sizeof(attachmentDirSegment), pBuffer.get(), attachmentEntriesSize, &bytesRead);
-    }
-    catch (const std::exception&)
-    {
-        std::throw_with_nested(LibCZIIOException("Error reading FileHeaderSegment", offset + sizeof(attachmentDirSegment), attachmentEntriesSize));
-    }
-
-    if (bytesRead != attachmentEntriesSize)
-    {
-        CCZIParse::ThrowNotEnoughDataRead(offset + sizeof(attachmentDirSegment), attachmentEntriesSize, bytesRead);
-    }
+    // an empty attachment-directory (with zero entries) is valid and in this
+    //  case we can skip the rest of the processing
+    if (attachmentDirSegment.data.EntryCount > 0)
+    {
+        // now read the AttachmentEntries
+        const uint64_t attachmentEntriesSize = static_cast<uint64_t>(attachmentDirSegment.data.EntryCount) * sizeof(AttachmentEntryA1);
+        unique_ptr<AttachmentEntryA1, decltype(free)*> pBuffer(static_cast<AttachmentEntryA1*>(malloc((size_t)attachmentEntriesSize)), free);
 
-    for (int i = 0; i < attachmentDirSegment.data.EntryCount; ++i)
-    {
-        ConvertToHostByteOrder::Convert(pBuffer.get() + i);
+        // now read the attachment-entries
+        try
+        {
+            str->Read(offset + sizeof(attachmentDirSegment), pBuffer.get(), attachmentEntriesSize, &bytesRead);
+        }
+        catch (const std::exception&)
+        {
+            std::throw_with_nested(LibCZIIOException("Error reading FileHeaderSegment", offset + sizeof(attachmentDirSegment), attachmentEntriesSize));
+        }
 
-        const AttachmentEntryA1* pSrc = pBuffer.get() + i;
-        CCziAttachmentsDirectoryBase::AttachmentEntry ae;
-        bool b = CheckAttachmentSchemaType((const char*)&pSrc->SchemaType[0], 2);
-        if (b == false)
+        if (bytesRead != attachmentEntriesSize)
         {
-            // TODO: what do we do if we encounter this...?
-            continue;
+            CCZIParse::ThrowNotEnoughDataRead(offset + sizeof(attachmentDirSegment), attachmentEntriesSize, bytesRead);
         }
 
-        ae.FilePosition = pSrc->FilePosition;
-        ae.ContentGuid = pSrc->ContentGuid;
-        memcpy(&ae.ContentFileType[0], &pSrc->ContentFileType[0], sizeof(AttachmentEntryA1::ContentFileType));
-        memcpy(&ae.Name[0], &pSrc->Name[0], sizeof(AttachmentEntryA1::Name));
-        ae.Name[sizeof(AttachmentEntryA1::Name) - 1] = '\0';
-        addFunc(ae);
+        for (int i = 0; i < attachmentDirSegment.data.EntryCount; ++i)
+        {
+            ConvertToHostByteOrder::Convert(pBuffer.get() + i);
+
+            const AttachmentEntryA1* pSrc = pBuffer.get() + i;
+            CCziAttachmentsDirectoryBase::AttachmentEntry ae;
+            bool b = CheckAttachmentSchemaType(reinterpret_cast<const char*>(&pSrc->SchemaType[0]), 2);
+            if (b == false)
+            {
+                // TODO: what do we do if we encounter this...?
+                continue;
+            }
+
+            ae.FilePosition = pSrc->FilePosition;
+            ae.ContentGuid = pSrc->ContentGuid;
+            memcpy(&ae.ContentFileType[0], &pSrc->ContentFileType[0], sizeof(AttachmentEntryA1::ContentFileType));
+            memcpy(&ae.Name[0], &pSrc->Name[0], sizeof(AttachmentEntryA1::Name));
+            ae.Name[sizeof(AttachmentEntryA1::Name) - 1] = '\0';
+            addFunc(ae);
+        }
     }
 }
 
 /*static*/CCZIParse::SubBlockData CCZIParse::ReadSubBlock(libCZI::IStream* str, std::uint64_t offset, const SubBlockStorageAllocate& allocateInfo)
 {
     SubBlockSegment subBlckSegment;
     std::uint64_t bytesRead;
```

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziParse.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziParse.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziReaderWriter.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziReaderWriter.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #include "libCZI_Utilities.h"
 #include "CziUtils.h"
 #include "libCZI_exceptions.h"
 #include "CziMetadataBuilder.h"
 #include "utilities.h"
 #include "CziSubBlock.h"
 #include "CziAttachment.h"
+#include "CziReaderCommon.h"
 
 using namespace libCZI;
 using namespace std;
 
 struct AddHelper
 {
     ICziReaderWriter* t;
@@ -126,16 +127,16 @@
     }
 
     CWriterUtils::WriteInfo wi;
     wi.segmentPos = this->nextSegmentInfo.GetNextSegmentPos();
     wi.writeFunc = std::bind(&CCziReaderWriter::WriteToOutputStream, this, placeholders::_1, placeholders::_2, placeholders::_3, placeholders::_4, placeholders::_5);
     wi.useSpecifiedAllocatedSize = false;
 
-    auto sizeOfSbBlk = CWriterUtils::WriteSubBlock(wi, addSbBlkInfo);
-    this->nextSegmentInfo.SetNextSegmentPos(wi.segmentPos + sizeOfSbBlk /*+ sizeof(SegmentHeader)*/);
+    const auto sizeOfSbBlk = CWriterUtils::WriteSubBlock(wi, addSbBlkInfo);
+    this->nextSegmentInfo.SetNextSegmentPos(wi.segmentPos + sizeOfSbBlk);
 }
 
 /*virtual*/void CCziReaderWriter::SyncAddAttachment(const libCZI::AddAttachmentInfo& addAttachmentInfo)
 {
     this->ThrowIfNotOperational();
 
     // check arguments
@@ -264,24 +265,24 @@
             sbBlkDirWriteInfo.existingSegmentPos = 0;
             sbBlkDirWriteInfo.sizeExistingSegmentPos = 0;
             sbBlkDirWriteInfo.markAsDeletedIfExistingSegmentIsNotUsed = false;
         }
 
         sbBlkDirWriteInfo.segmentPosForNewSegment = this->nextSegmentInfo.GetNextSegmentPos();
         sbBlkDirWriteInfo.enumEntriesFunc = [&](const std::function<void(size_t, const CCziSubBlockDirectoryBase::SubBlkEntry&)>& f)->void
-        {
-            this->sbBlkDirectory.EnumEntries(
-                [&](size_t index, const CCziSubBlockDirectoryBase::SubBlkEntry& e)->bool
-                {
-                    f(index, e);
-            return true;
-                });
-        };
+            {
+                this->sbBlkDirectory.EnumEntries(
+                    [&](size_t index, const CCziSubBlockDirectoryBase::SubBlkEntry& e)->bool
+                    {
+                        f(index, e);
+                        return true;
+                    });
+            };
         sbBlkDirWriteInfo.writeFunc = std::bind(&CCziReaderWriter::WriteToOutputStream, this, placeholders::_1, placeholders::_2, placeholders::_3, placeholders::_4, placeholders::_5);
-        auto posAndSize = CWriterUtils::WriteSubBlkDirectory(sbBlkDirWriteInfo);
+        const auto posAndSize = CWriterUtils::WriteSubBlkDirectory(sbBlkDirWriteInfo);
         this->subBlockDirectorySegment.SetPositionAndAllocatedSize(get<0>(posAndSize), get<1>(posAndSize), false);
         if (get<0>(posAndSize) == sbBlkDirWriteInfo.segmentPosForNewSegment)
         {
             // ie the subblock-directory was appended at the end
             this->nextSegmentInfo.SetNextSegmentPos(get<0>(posAndSize) + get<1>(posAndSize));
         }
     }
@@ -302,24 +303,24 @@
             attchmntDirWriteInfo.existingSegmentPos = 0;
             attchmntDirWriteInfo.sizeExistingSegmentPos = 0;
         }
 
         attchmntDirWriteInfo.segmentPosForNewSegment = this->nextSegmentInfo.GetNextSegmentPos();
         attchmntDirWriteInfo.entryCnt = this->attachmentDirectory.GetEntryCnt();
         attchmntDirWriteInfo.enumEntriesFunc = [&](const std::function<void(size_t, const CCziAttachmentsDirectoryBase::AttachmentEntry&)>& f)->void
-        {
-            this->attachmentDirectory.EnumEntries(
-                [&](size_t index, const CCziAttachmentsDirectoryBase::AttachmentEntry& e)->bool
-                {
-                    f(index, e);
-            return true;
-                });
-        };
+            {
+                this->attachmentDirectory.EnumEntries(
+                    [&](size_t index, const CCziAttachmentsDirectoryBase::AttachmentEntry& e)->bool
+                    {
+                        f(index, e);
+                        return true;
+                    });
+            };
         attchmntDirWriteInfo.writeFunc = std::bind(&CCziReaderWriter::WriteToOutputStream, this, placeholders::_1, placeholders::_2, placeholders::_3, placeholders::_4, placeholders::_5);
-        auto posAndSize = CWriterUtils::WriteAttachmentDirectory(attchmntDirWriteInfo);
+        const auto posAndSize = CWriterUtils::WriteAttachmentDirectory(attchmntDirWriteInfo);
         this->attachmentDirectorySegment.SetPositionAndAllocatedSize(get<0>(posAndSize), get<1>(posAndSize), false);
         if (get<0>(posAndSize) == attchmntDirWriteInfo.segmentPosForNewSegment)
         {
             // ie the attachment-directory was appended at the end
             this->nextSegmentInfo.SetNextSegmentPos(get<0>(posAndSize) + get<1>(posAndSize));
         }
     }
@@ -376,15 +377,15 @@
     }
 
     if (cziHeaderSuccessfullyRead)
     {
         if (this->info->GetForceFileGuid())
         {
             // we then immediately update the File-Guid
-            auto newGuid = this->UpdateFileHeaderGuid();
+            const auto newGuid = this->UpdateFileHeaderGuid();
             memcpy(&fileHeaderSegment.FileGuid, &newGuid, sizeof(newGuid));
             memcpy(&fileHeaderSegment.PrimaryFileGuid, &newGuid, sizeof(newGuid));
         }
 
         this->hdrSegmentData = CFileHeaderSegmentData(&fileHeaderSegment);
 
         CCZIParse::SegmentSizes sbBlkDirSegmentSize;
@@ -411,21 +412,22 @@
                 pos,
                 [&](const CCziAttachmentsDirectoryBase::AttachmentEntry& ae)->void
                 {
                     this->attachmentDirectory.AddAttachment(ae);
                 },
                 &attchmntDirSegmentSize);
 
+            this->attachmentDirectory.SetModified(false);
             this->attachmentDirectorySegment.SetPositionAndAllocatedSize(pos, attchmntDirSegmentSize.AllocatedSize, false);
         }
 
         pos = this->hdrSegmentData.GetMetadataPosition();
         if (pos != 0)
         {
-            auto segmentSize = CCZIParse::ReadSegmentHeader(CCZIParse::SegmentType::Metadata, this->stream.get(), this->hdrSegmentData.GetMetadataPosition());
+            const auto segmentSize = CCZIParse::ReadSegmentHeader(CCZIParse::SegmentType::Metadata, this->stream.get(), this->hdrSegmentData.GetMetadataPosition());
             this->metadataSegment.SetPositionAndAllocatedSize(pos, segmentSize.AllocatedSize, false);
         }
     }
     else
     {
         // if there is no valid CZI-file-header, we now write one
         FileHeaderSegment fhs = { 0 };
@@ -477,26 +479,26 @@
         [&](size_t index, const CCziSubBlockDirectoryBase::SubBlkEntry& sbBlkEntry)->bool
         {
             if (sbBlkEntry.FilePosition > lastSegmentPos)
             {
                 lastSegmentPos = sbBlkEntry.FilePosition;
             }
 
-    return true;
+            return true;
         });
 
     this->attachmentDirectory.EnumEntries(
         [&](size_t index, const CCziAttachmentsDirectoryBase::AttachmentEntry& attEntry)->bool
         {
             if (uint64_t(attEntry.FilePosition) > lastSegmentPos)
             {
                 lastSegmentPos = attEntry.FilePosition;
             }
 
-    return true;
+            return true;
         });
 
     if (this->hdrSegmentData.GetIsSubBlockDirectoryPositionValid())
     {
         lastSegmentPos = (std::max)(lastSegmentPos, this->hdrSegmentData.GetSubBlockDirectoryPosition());
     }
 
@@ -636,28 +638,22 @@
 
 /*virtual*/void CCziReaderWriter::EnumerateSubBlocks(const std::function<bool(int index, const libCZI::SubBlockInfo& info)>& funcEnum)
 {
     this->ThrowIfNotOperational();
     this->sbBlkDirectory.EnumEntries(
         [&](int index, const CCziSubBlockDirectory::SubBlkEntry& entry)->bool
         {
-            SubBlockInfo info;
-    info.coordinate = entry.coordinate;
-    info.logicalRect = IntRect{ entry.x,entry.y,entry.width,entry.height };
-    info.physicalSize = IntSize{ (std::uint32_t)entry.storedWidth, (std::uint32_t)entry.storedHeight };
-    info.mIndex = entry.mIndex;
-    info.pixelType = CziUtils::PixelTypeFromInt(entry.PixelType);
-    return funcEnum(index, info);
+            return funcEnum(index, CziReaderCommon::ConvertToSubBlockInfo(entry));
         });
 }
 
 /*virtual*/void CCziReaderWriter::EnumSubset(const libCZI::IDimCoordinate* planeCoordinate, const libCZI::IntRect* roi, bool onlyLayer0, const std::function<bool(int index, const libCZI::SubBlockInfo& info)>& funcEnum)
 {
     this->ThrowIfNotOperational();
-    throw std::runtime_error("Not Implemented");
+    CziReaderCommon::EnumSubset(this, planeCoordinate, roi, onlyLayer0, funcEnum);
 }
 
 /*virtual*/std::shared_ptr<libCZI::ISubBlock> CCziReaderWriter::ReadSubBlock(int index)
 {
     this->ThrowIfNotOperational();
     CCziSubBlockDirectoryBase::SubBlkEntry entry;
     if (this->sbBlkDirectory.TryGetSubBlock(index, &entry) == false)
@@ -688,30 +684,24 @@
     if (this->sbBlkDirectory.TryGetSubBlock(index, &entry) == false)
     {
         return false;
     }
 
     if (info != nullptr)
     {
-        info->compressionModeRaw = entry.Compression;
-        info->pixelType = CziUtils::PixelTypeFromInt(entry.PixelType);
-        info->coordinate = entry.coordinate;
-        info->logicalRect = IntRect{ entry.x,entry.y,entry.width,entry.height };
-        info->physicalSize = IntSize{ static_cast<std::uint32_t>(entry.storedWidth), static_cast<std::uint32_t>(entry.storedHeight) };
-        info->mIndex = entry.mIndex;
-        info->pyramidType = CziUtils::PyramidTypeFromByte(entry.pyramid_type_from_spare);
+        *info = CziReaderCommon::ConvertToSubBlockInfo(entry);
     }
 
     return true;
 }
 
 /*virtual*/bool CCziReaderWriter::TryGetSubBlockInfoOfArbitrarySubBlockInChannel(int channelIndex, libCZI::SubBlockInfo& info)
 {
     this->ThrowIfNotOperational();
-    throw std::runtime_error("Not Implemented");
+    return CziReaderCommon::TryGetSubBlockInfoOfArbitrarySubBlockInChannel(this, channelIndex, info);
 }
 
 /*virtual*/libCZI::SubBlockStatistics CCziReaderWriter::GetStatistics()
 {
     this->ThrowIfNotOperational();
     return this->sbBlkDirectory.GetStatistics();
 }
@@ -725,26 +715,30 @@
 /*virtual*/void CCziReaderWriter::EnumerateAttachments(const std::function<bool(int index, const libCZI::AttachmentInfo& info)>& funcEnum)
 {
     this->ThrowIfNotOperational();
     this->attachmentDirectory.EnumEntries(
         [&](int index, const CCziAttachmentsDirectoryBase::AttachmentEntry& entry)->bool
         {
             libCZI::AttachmentInfo info;
-    info.contentGuid = entry.ContentGuid;
-    memcpy(info.contentFileType, entry.ContentFileType, sizeof(entry.ContentFileType));
-    info.name = entry.Name;
-    bool b = funcEnum(index, info);
-    return b;
+            info.contentGuid = entry.ContentGuid;
+            memcpy(info.contentFileType, entry.ContentFileType, sizeof(entry.ContentFileType));
+            info.name = entry.Name;
+            bool b = funcEnum(index, info);
+            return b;
         });
 }
 
 /*virtual*/void CCziReaderWriter::EnumerateSubset(const char* contentFileType, const char* name, const std::function<bool(int index, const libCZI::AttachmentInfo& infi)>& funcEnum)
 {
     this->ThrowIfNotOperational();
-    throw std::runtime_error("Not Implemented");
+    CziReaderCommon::EnumerateSubset(
+        std::bind(&CReaderWriterCziAttachmentsDirectory::EnumEntries, &this->attachmentDirectory, std::placeholders::_1),
+        contentFileType,
+        name,
+        funcEnum);
 }
 
 /*virtual*/std::shared_ptr<libCZI::IAttachment> CCziReaderWriter::ReadAttachment(int index)
 {
     this->ThrowIfNotOperational();
     CCziAttachmentsDirectoryBase::AttachmentEntry entry;
     if (this->attachmentDirectory.TryGetAttachment(index, &entry) == false)
```

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziReaderWriter.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziReaderWriter.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziStructs.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziStructs.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziStructs.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziStructs.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziSubBlock.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziSubBlock.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziSubBlock.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziSubBlock.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziSubBlockDirectory.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziSubBlockDirectory.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziSubBlockDirectory.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziSubBlockDirectory.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziUtils.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziUtils.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziUtils.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziUtils.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziWriter.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziWriter.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -729,28 +729,30 @@
 
     ConvertToHostByteOrder::Convert(&attchmntDirSegment);
     info.writeFunc(attchmDirPos, &attchmntDirSegment, sizeof(attchmntDirSegment), &bytesWritten, "AttachmentDirSegment");
     totalBytesWritten += bytesWritten;
 
     std::unique_ptr<AttachmentEntryA1, void(*)(AttachmentEntryA1*)> upAttchmntData((AttachmentEntryA1*)malloc(sizeAttchmntEntries), [](AttachmentEntryA1* p)->void {free(p); });
 
+    size_t index_count = 0;
     info.enumEntriesFunc(
         [&](size_t index, const CCziAttachmentsDirectoryBase::AttachmentEntry& entry)->bool
         {
-            AttachmentEntryA1* p = (upAttchmntData.get() + index);
+            AttachmentEntryA1* p = upAttchmntData.get() + index_count;
             p->SchemaType[0] = 'A';
             p->SchemaType[1] = '1';
             memset(&p->_spare[0], 0, sizeof(p->_spare));
             p->FilePosition = entry.FilePosition;
             p->FilePart = 0;
             p->ContentGuid = entry.ContentGuid;
             memcpy(&p->ContentFileType[0], &entry.ContentFileType[0], sizeof(p->ContentFileType));
             memcpy(&p->Name[0], &entry.Name[0], sizeof(p->Name));
 
             ConvertToHostByteOrder::Convert(p);
+            ++index_count;
             return true;
         });
 
     info.writeFunc(attchmDirPos + totalBytesWritten, upAttchmntData.get(), sizeAttchmntEntries, &bytesWritten, "AttachmentDirData");
     totalBytesWritten += bytesWritten;
 
     if (totalBytesWritten < attchmntDirSegmentHeaderAllocatedSize + sizeof(SegmentHeader))
```

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/CziWriter.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/CziWriter.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/DimCoordinate.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/DimCoordinate.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/CZICmd_usage.markdown` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/CZICmd_usage.markdown`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/CZI_1.PNG` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/CZI_1.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/CZI_2.PNG` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/CZI_2.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/ScalingSingleChannelTileAccessor1.png` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/ScalingSingleChannelTileAccessor1.png`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_1.PNG` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_1.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_2.PNG` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_2.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_3.PNG` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_3.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_4.PNG` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_4.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/Tinting-LUT.png` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/Tinting-LUT.png`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/VisualStudio_cmake1.png` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/VisualStudio_cmake1.png`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/ZEN_screenshot_1.PNG` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/ZEN_screenshot_1.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/ZEN_screenshot_2.PNG` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/ZEN_screenshot_2.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_1_raspi.PNG` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_1_raspi.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_1_raspi_help_freetype.PNG` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_1_raspi_help_freetype.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_install_raspi1.PNG` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_install_raspi1.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_raspi_unittests_1.PNG` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_raspi_unittests_1.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/compositors_1.png` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/compositors_1.png`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/compositors_2.png` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/compositors_2.png`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/drawings/VS-project.pub` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/drawings/VS-project.pub`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/drawings/VS-project_2.pub` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/drawings/VS-project_2.pub`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/gradationcurve_1.PNG` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/gradationcurve_1.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/gradationcurve_2.PNG` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/gradationcurve_2.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept1.PNG` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept1.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept2.PNG` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept2.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept3.PNG` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept3.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept4.PNG` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept4.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/Todos.markdown` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/Todos.markdown`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/accessors.markdown` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/accessors.markdown`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/building_libCZI.markdown` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/building_libCZI.markdown`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/drawings.docx` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/drawings.docx`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/image_document_concept.markdown` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/image_document_concept.markdown`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/mainpage.markdown` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/mainpage.markdown`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/multichannelcomposition.markdown` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/multichannelcomposition.markdown`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/using_libCZI.markdown` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/using_libCZI.markdown`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/version-history.markdown` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/version-history.markdown`

 * *Files 5% similar despite different names*

```diff
@@ -10,8 +10,14 @@
  0.54.2             | [74](https://github.com/ZEISS/libczi/pull/74)        | minor bug fix
  0.54.3             | [79](https://github.com/ZEISS/libczi/pull/79)        | add option _kCurlHttp_FollowLocation_ to follow HTTP redirects tp curl_http_inputstream
  0.55.0             | [78](https://github.com/ZEISS/libczi/pull/78)        | optimization: for multi-tile-composition, check relevant tiles for visibility before loading them (and do not load/decode non-visible tiles)
  0.55.1             | [80](https://github.com/ZEISS/libczi/pull/80)        | bugfix for above optimization
  0.56.0             | [82](https://github.com/ZEISS/libczi/pull/82)        | add option "kCurlHttp_CaInfo" & "kCurlHttp_CaInfoBlob", allow to retrieve properties from a stream-class
  0.57.0             | [84](https://github.com/ZEISS/libczi/pull/84)        | add caching for accessors, update CLI11 to version 2.3.2
  0.57.1             | [86](https://github.com/ZEISS/libczi/pull/86)        | small improvement for CMake-build: allow to use an apt-provided CURL-package
- 0.57.2             | [90](https://github.com/ZEISS/libczi/pull/90)        | improve thread-safety of CziReader
+ 0.57.2             | [90](https://github.com/ZEISS/libczi/pull/90)        | improve thread-safety of CziReader
+ 0.57.3             | [91](https://github.com/ZEISS/libczi/pull/91)        | improve error-message
+ 0.58.0             | [92](https://github.com/ZEISS/libczi/pull/92)        | export a list with properties for streams-property-bag
+ 0.58.1             | [95](https://github.com/ZEISS/libczi/pull/95)        | some fixes for CziReaderWriter
+ 0.58.2             | [96](https://github.com/ZEISS/libczi/pull/96)        | small fixes for deficiencies reported by CodeQL
+ 0.58.3             | [97](https://github.com/ZEISS/libczi/pull/97)        | update zstd to [version 1.5.6](https://github.com/facebook/zstd/releases/tag/v1.5.6)
+ 0.58.4             | [99](https://github.com/ZEISS/libczi/pull/99)        | fix a rare issue with curl_http_inputstream which would fail to read CZIs with an attachment-directory containing zero entries
```

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/Doc/write_czi.markdown` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/Doc/write_czi.markdown`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/FileHeaderSegmentData.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/FileHeaderSegmentData.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/ImportExport.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/ImportExport.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/IndexSet.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/IndexSet.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/IndexSet.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/IndexSet.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/MD5Sum.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/MD5Sum.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/MD5Sum.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/MD5Sum.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/MultiChannelCompositor.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/MultiChannelCompositor.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/SingleChannelAccessorBase.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/SingleChannelAccessorBase.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/SingleChannelAccessorBase.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/SingleChannelAccessorBase.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/SingleChannelPyramidLevelTileAccessor.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/SingleChannelPyramidLevelTileAccessor.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/SingleChannelPyramidLevelTileAccessor.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/SingleChannelPyramidLevelTileAccessor.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/SingleChannelScalingTileAccessor.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/SingleChannelScalingTileAccessor.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/SingleChannelScalingTileAccessor.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/SingleChannelScalingTileAccessor.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/SingleChannelTileAccessor.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/SingleChannelTileAccessor.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/SingleChannelTileAccessor.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/SingleChannelTileAccessor.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/SingleChannelTileCompositor.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/SingleChannelTileCompositor.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamImpl.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamImpl.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -97,37 +97,42 @@
         CloseHandle(this->handle);
         this->handle = INVALID_HANDLE_VALUE;
     }
 }
 
 /*virtual*/void CSimpleOutputStreamImplWindows::Write(std::uint64_t offset, const void* pv, std::uint64_t size, std::uint64_t* ptrBytesWritten)
 {
-    OVERLAPPED ol = { 0 };
-    ol.Offset = (DWORD)(offset);
-    ol.OffsetHigh = (DWORD)(offset >> 32);
-    DWORD bytesWritten;
-    BOOL B = WriteFile(this->handle, pv, (DWORD)size, &bytesWritten, &ol);
+    if (size > (std::numeric_limits<DWORD>::max)())
+    {
+        throw std::runtime_error("size is too large");
+    }
+
+    OVERLAPPED ol = {};
+    ol.Offset = static_cast<DWORD>(offset);
+    ol.OffsetHigh = static_cast<DWORD>(offset >> 32);
+    DWORD bytes_written;
+    const BOOL B = WriteFile(this->handle, pv, static_cast<DWORD>(size), &bytes_written, &ol);
     if (!B)
     {
-        DWORD lastError = GetLastError();
+        const DWORD last_error = GetLastError();
         std::stringstream ss;
-        ss << "Error writing to file (LastError=" << std::setfill('0') << std::setw(8) << std::showbase << lastError << ")";
+        ss << "Error writing to file (LastError=" << std::hex << std::setfill('0') << std::setw(8) << std::showbase << last_error << ")";
         throw std::runtime_error(ss.str());
     }
 
     if (ptrBytesWritten != nullptr)
     {
-        *ptrBytesWritten = bytesWritten;
+        *ptrBytesWritten = bytes_written;
     }
 }
 #endif
 
 //----------------------------------------------------------------------------
 CStreamImplInMemory::CStreamImplInMemory(std::shared_ptr<const void> ptr, std::size_t dataSize)
-    : rawData(ptr), dataBufferSize(dataSize)
+    : rawData(std::move(ptr)), dataBufferSize(dataSize)
 {
 }
 
 CStreamImplInMemory::CStreamImplInMemory(libCZI::IAttachment* attachement)
 {
     this->rawData = attachement->GetRawData(&this->dataBufferSize);
 }
@@ -332,51 +337,61 @@
     {
         CloseHandle(this->handle);
     }
 }
 
 /*virtual*/void CSimpleInputOutputStreamImplWindows::Read(std::uint64_t offset, void* pv, std::uint64_t size, std::uint64_t* ptrBytesRead)
 {
-    OVERLAPPED ol = { 0 };
+    if (size > (std::numeric_limits<DWORD>::max)())
+    {
+        throw std::runtime_error("size is too large");
+    }
+
+    OVERLAPPED ol = {};
     ol.Offset = static_cast<DWORD>(offset);
     ol.OffsetHigh = static_cast<DWORD>(offset >> 32);
-    DWORD bytesRead;
-    BOOL B = ReadFile(this->handle, pv, static_cast<DWORD>(size), &bytesRead, &ol);
+    DWORD bytes_read;
+    const BOOL B = ReadFile(this->handle, pv, static_cast<DWORD>(size), &bytes_read, &ol);
     if (!B)
     {
-        const DWORD lastError = GetLastError();
+        const DWORD last_error = GetLastError();
         ostringstream ss;
-        ss << "Error reading from file (LastError=" << std::setfill('0') << std::setw(8) << std::showbase << lastError << ")";
+        ss << "Error reading from file (LastError=" << std::hex << std::setfill('0') << std::setw(8) << std::showbase << last_error << ")";
         throw std::runtime_error(ss.str());
     }
 
     if (ptrBytesRead != nullptr)
     {
-        *ptrBytesRead = bytesRead;
+        *ptrBytesRead = bytes_read;
     }
 }
 
 /*virtual*/void CSimpleInputOutputStreamImplWindows::Write(std::uint64_t offset, const void* pv, std::uint64_t size, std::uint64_t* ptrBytesWritten)
 {
-    OVERLAPPED ol = { 0 };
+    if (size > (std::numeric_limits<DWORD>::max)())
+    {
+        throw std::runtime_error("size is too large");
+    }
+
+    OVERLAPPED ol = {};
     ol.Offset = static_cast<DWORD>(offset);
     ol.OffsetHigh = static_cast<DWORD>(offset >> 32);
-    DWORD bytesWritten;
-    BOOL B = WriteFile(this->handle, pv, static_cast<DWORD>(size), &bytesWritten, &ol);
+    DWORD bytes_written;
+    const BOOL B = WriteFile(this->handle, pv, static_cast<DWORD>(size), &bytes_written, &ol);
     if (!B)
     {
-        DWORD lastError = GetLastError();
+        const DWORD last_error = GetLastError();
         ostringstream ss;
-        ss << "Error writing to file (LastError=" << std::setfill('0') << std::setw(8) << std::showbase << lastError << ")";
+        ss << "Error writing to file (LastError=" << std::hex << std::setfill('0') << std::setw(8) << std::showbase << last_error << ")";
         throw std::runtime_error(ss.str());
     }
 
     if (ptrBytesWritten != nullptr)
     {
-        *ptrBytesWritten = bytesWritten;
+        *ptrBytesWritten = bytes_written;
     }
 }
 #endif
 
 //-----------------------------------------------------------------------------
 
 CSimpleInputOutputStreamImpl::CSimpleInputOutputStreamImpl(const wchar_t* filename)
```

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamImpl.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamImpl.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamsLib/curlhttpinputstream.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamsLib/curlhttpinputstream.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,16 @@
         string_stream << "curl_url_set(..) failed with error code " << return_code_url << " (" << curl_url_strerror(return_code_url) << ")";
         throw std::runtime_error(string_stream.str());
     }
 
     CURLcode return_code = curl_easy_setopt(up_curl_handle.get(), CURLOPT_CURLU, up_curl_url_handle.get());
     ThrowIfCurlSetOptError(return_code, "CURLOPT_CURLU");
 
+    // for debugging purposes, set verbose mode to 1, and libcurl will output information about the operation
+    //  to stdout
     return_code = curl_easy_setopt(up_curl_handle.get(), CURLOPT_VERBOSE, 0L/*1L*/);
     ThrowIfCurlSetOptError(return_code, "CURLOPT_VERBOSE");
 
     /* disable progress meter, set to 0L to enable it */
     return_code = curl_easy_setopt(up_curl_handle.get(), CURLOPT_NOPROGRESS, 1L);
     ThrowIfCurlSetOptError(return_code, "CURLOPT_NOPROGRESS");
 
@@ -229,14 +231,25 @@
 
     this->curl_handle_ = up_curl_handle.release();
     this->curl_url_handle_ = up_curl_url_handle.release();
 }
 
 /*virtual*/void CurlHttpInputStream::Read(std::uint64_t offset, void* pv, std::uint64_t size, std::uint64_t* ptrBytesRead)
 {
+    // we handle the case of size == 0 explicitly, because the "curl_easy_perform" would not work with a size of 0
+    if (size == 0)
+    {
+        if (ptrBytesRead != nullptr)
+        {
+            *ptrBytesRead = 0;
+        }
+
+        return;
+    }
+
     stringstream ss;
     ss << offset << "-" << offset + size - 1;
 
     {
         std::lock_guard<std::mutex> lck(this->request_mutex_);
 
         // TODO(JBL): We may be able to use a "header-function" (https://curl.se/libcurl/c/CURLOPT_HEADERFUNCTION.html) in order to find out
```

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamsLib/curlhttpinputstream.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamsLib/curlhttpinputstream.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamsLib/preadfileinputstream.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamsLib/preadfileinputstream.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamsLib/preadfileinputstream.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamsLib/preadfileinputstream.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamsLib/simplefileinputstream.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamsLib/simplefileinputstream.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamsLib/simplefileinputstream.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamsLib/simplefileinputstream.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamsLib/windowsfileinputstream.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamsLib/windowsfileinputstream.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -46,17 +46,17 @@
     OVERLAPPED ol = {};
     ol.Offset = static_cast<DWORD>(offset);
     ol.OffsetHigh = static_cast<DWORD>(offset >> 32);
     DWORD bytes_read;
     const BOOL read_file_return_code = ReadFile(this->handle, pv, static_cast<DWORD>(size), &bytes_read, &ol);
     if (!read_file_return_code)
     {
-        const DWORD lastError = GetLastError();
+        const DWORD last_error = GetLastError();
         std::stringstream ss;
-        ss << "Error reading from file (LastError=" << std::setfill('0') << std::setw(8) << std::showbase << lastError << ")";
+        ss << "Error reading from file (LastError=" << std::hex << std::setfill('0') << std::setw(8) << std::showbase << last_error << ")";
         throw std::runtime_error(ss.str());
     }
 
     if (ptrBytesRead != nullptr)
     {
         *ptrBytesRead = bytes_read;
     }
```

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/StreamsLib/windowsfileinputstream.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/StreamsLib/windowsfileinputstream.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/XmlNodeWrapper.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/XmlNodeWrapper.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/bitmapData.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/bitmapData.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/decoder.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/decoder.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/decoder.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/decoder.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/decoder_wic.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/decoder_wic.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/decoder_wic.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/decoder_wic.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/decoder_zstd.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/decoder_zstd.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/decoder_zstd.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/decoder_zstd.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/jxrlibcompress.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/jxrlibcompress.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI.h`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,17 @@
     class IStream
     {
     public:
         /// Reads the specified amount of data from the stream at the specified position. This method
         /// is expected to throw an exception for any kind of I/O-related error. It must not throw
         /// an exception if reading past the end of a file - instead, it must return the number of
         /// bytes actually read accordingly.
+        /// For the special case of size==0, the behavior should be as follows: the method should
+        /// operate as for a size>0, but it should not read any data. The method should return 0 in
+        /// ptrBytesRead.
         ///
         /// \param offset                The offset to start reading from.
         /// \param [out] pv              The caller-provided buffer for the data. Must be non-null.
         /// \param size                  The size of the buffer.
         /// \param [out] ptrBytesRead    If non-null, the variable pointed to will receive the number of bytes actually read.
         virtual void Read(std::uint64_t offset, void* pv, std::uint64_t size, std::uint64_t* ptrBytesRead) = 0;
```

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Compositor.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Compositor.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Config.h.in` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Config.h.in`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_DimCoordinate.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_DimCoordinate.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Helpers.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Helpers.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Lib.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Lib.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Metadata.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Metadata.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Metadata2.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Metadata2.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Pixels.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Pixels.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_ReadWrite.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_ReadWrite.h`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,17 @@
     /// Interface for "in-place-editing" of a CZI. All write-operations immediately go into the file. If the data does not fit into the
     /// existing segments, a new segment is appended at the end (and the existing one is marked "DELETED").
     /// All operation is strictly single-threaded. Only exactly one method may be executing at a given point in time.
     /// Notes:
     /// - The indices (or "keys") for a subblock/attachment do not change during the lifetime of the object (even if deleting some).  
     /// - Contrary to ICziWriter, this object does not attempt to verify the consistency of the coordinates - which is due the fact  
     ///    that we aim at allowing arbitrary modifications. We do not require to specify in advance the number of dimensions or the bounds.
-    /// - The information returned by ISubBlockRepository::GetStatistics is valid (taking into consideration the current state).
+    /// - The information returned by ISubBlockRepository::GetStatistics is valid (taking into consideration the current state).  
+    /// - When enumerating subblocks/attachments, mutations (i.e. adding/removing items) of the respective subblock/attachment-collection are not allowed  
+    ///    and result in undefined behavior.
     class LIBCZI_API ICziReaderWriter : public ISubBlockRepository, public IAttachmentRepository
     {
     public:
 
         /// Initialize the object.
         ///
         /// \param stream The read-write stream to operate on.
```

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Site.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Site.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Site.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Site.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_StreamsLib.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_StreamsLib.h`

 * *Files 4% similar despite different names*

```diff
@@ -239,36 +239,54 @@
         struct LIBCZI_API CreateStreamInfo
         {
             std::string class_name; ///< Name of the class (this uniquely identifies the class).
 
             std::map<int, Property> property_bag; ///< A property-bag with options for creating the stream-object.
         };
 
+        /// Information about a property for the property bag when creating a stream object.
+        struct StreamPropertyBagPropertyInfo
+        {
+            const char* property_name;              ///< (Proposed) name of the property. This is a null-terminated static string. It is enum name with the initial "k" removed.
+            int property_id;                        ///< The numerical identifier for the property.
+            Property::Type property_type;           ///< Type of the property.
+        };
+
+        /// Gets a (static) list of all properties which can be used for the property bag when creating a stream object.
+        /// This list is terminated by an entry with a null property_name. The list is static and will not change during 
+        /// the lifetime of the application, the returned pointer is valid until the application terminates. It is 
+        /// pointing to static memory and must not be freed.
+        ///
+        /// \param [out] count   If non-null, the number of valid elements (not including the terminal element) is put here.
+        ///
+        /// \returns    A pointer to an array containing property-bag information.
+        static const StreamPropertyBagPropertyInfo* GetStreamPropertyBagPropertyInfo(int* count);
+
         /// Perform one-time initialization of the streams objects.
         /// Some stream objects may require some one-time initialization for being operational (this is e.g. the case with
         /// the libcurl-based ones). It is considered good practice to call this function before using any of the other methods.
         /// Calling it multiple times is not a problem (and subsequent calls after the first are ignored).
         static void Initialize();
 
         /// Creates and initializes a new instance of the specified stream class. If the specified
         /// class is not known, then this function will return nullptr. In case of an error when
         /// initializing the stream, an exception will be thrown.
         ///
         /// \param  stream_info     Information describing the stream.
-        /// \param  file_identifier The filename (or, more generally, an URI of some sort) identifying the file to be opened in UTF8-encoding.
+        /// \param  file_identifier The filename (or, more generally, a URI of some sort) identifying the file to be opened in UTF8-encoding.
         ///
         /// \returns    The newly created and initialized stream.
         static std::shared_ptr<libCZI::IStream> CreateStream(const CreateStreamInfo& stream_info, const std::string& file_identifier);
 
         /// Creates and initializes a new instance of the specified stream class. If the specified
         /// class is not known, then this function will return nullptr. In case of an error when
         /// initializing the stream, an exception will be thrown.
         ///
         /// \param  stream_info     Information describing the stream.
-        /// \param  file_identifier The filename (or, more generally, an URI of some sort) identifying the file to be opened.
+        /// \param  file_identifier The filename (or, more generally, a URI of some sort) identifying the file to be opened.
         ///
         /// \returns    The newly created and initialized stream.
         static std::shared_ptr<libCZI::IStream> CreateStream(const CreateStreamInfo& stream_info, const std::wstring& file_identifier);
 
         /// This structure gathers information about a stream class.
         struct LIBCZI_API StreamClassInfo
         {
```

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Utilities.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Utilities.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Utilities.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Utilities.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_Write.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_Write.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_compress.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_compress.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/libCZI_exceptions.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/libCZI_exceptions.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/pugiconfig.hpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/pugiconfig.hpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/pugixml.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/pugixml.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/pugixml.hpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/pugixml.hpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/splines.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/splines.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/splines.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/splines.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/stdAllocator.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/stdAllocator.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/stdAllocator.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/stdAllocator.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/subblock_cache.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/subblock_cache.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/subblock_cache.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/subblock_cache.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/utilities.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/utilities.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/utilities.h` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/utilities.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/utilities_simd.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/utilities_simd.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/Src/libCZI/zstdCompress.cpp` & `pylibCZIrw-4.1.1/libs/libCZIrw/Src/libCZI/zstdCompress.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/THIRD_PARTY_LICENSES.txt` & `pylibCZIrw-4.1.1/libs/libCZIrw/THIRD_PARTY_LICENSES.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/cla_corporate.txt` & `pylibCZIrw-4.1.1/libs/libCZIrw/cla_corporate.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/cla_individual.txt` & `pylibCZIrw-4.1.1/libs/libCZIrw/cla_individual.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/cmake/ExternalEIGEN3.cmake` & `pylibCZIrw-4.1.1/libs/libCZIrw/cmake/ExternalEIGEN3.cmake`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/cmake/TestLargeFile.cmake` & `pylibCZIrw-4.1.1/libs/libCZIrw/cmake/TestLargeFile.cmake`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/cmake/check_can_use_neon_intrinsics.cmake` & `pylibCZIrw-4.1.1/libs/libCZIrw/cmake/check_can_use_neon_intrinsics.cmake`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/libCZIrw/cmake/check_unaligned_access.cmake` & `pylibCZIrw-4.1.1/libs/libCZIrw/cmake/check_unaligned_access.cmake`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/.appveyor.yml` & `pylibCZIrw-4.1.1/libs/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/.clang-format` & `pylibCZIrw-4.1.1/libs/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/.clang-tidy` & `pylibCZIrw-4.1.1/libs/pybind11/.clang-tidy`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/.cmake-format.yaml` & `pylibCZIrw-4.1.1/libs/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/.codespell-ignore-lines` & `pylibCZIrw-4.1.1/libs/pybind11/.codespell-ignore-lines`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/.github/CONTRIBUTING.md` & `pylibCZIrw-4.1.1/libs/pybind11/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml` & `pylibCZIrw-4.1.1/libs/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/.github/matchers/pylint.json` & `pylibCZIrw-4.1.1/libs/pybind11/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/.github/pull_request_template.md` & `pylibCZIrw-4.1.1/libs/pybind11/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/.github/workflows/ci.yml` & `pylibCZIrw-4.1.1/libs/pybind11/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/.github/workflows/configure.yml` & `pylibCZIrw-4.1.1/libs/pybind11/.github/workflows/configure.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/.github/workflows/format.yml` & `pylibCZIrw-4.1.1/libs/pybind11/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/.github/workflows/labeler.yml` & `pylibCZIrw-4.1.1/libs/pybind11/.github/workflows/labeler.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/.github/workflows/pip.yml` & `pylibCZIrw-4.1.1/libs/pybind11/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/.github/workflows/upstream.yml` & `pylibCZIrw-4.1.1/libs/pybind11/.github/workflows/upstream.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/.gitignore` & `pylibCZIrw-4.1.1/libs/pybind11/.gitignore`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/.pre-commit-config.yaml` & `pylibCZIrw-4.1.1/libs/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/CMakeLists.txt` & `pylibCZIrw-4.1.1/libs/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/LICENSE` & `pylibCZIrw-4.1.1/libs/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/README.rst` & `pylibCZIrw-4.1.1/libs/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/SECURITY.md` & `pylibCZIrw-4.1.1/libs/pybind11/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/Doxyfile` & `pylibCZIrw-4.1.1/libs/pybind11/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/Makefile` & `pylibCZIrw-4.1.1/libs/pybind11/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/cast/chrono.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/cast/custom.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/cast/eigen.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/cast/functional.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/cast/index.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/cast/overview.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/cast/stl.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/cast/strings.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/classes.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/embedding.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/exceptions.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/functions.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/misc.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/pycpp/numpy.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/pycpp/object.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/pycpp/utilities.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/advanced/smart_ptrs.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/basics.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/benchmark.py` & `pylibCZIrw-4.1.1/libs/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/benchmark.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/changelog.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/classes.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/compiling.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/conf.py` & `pylibCZIrw-4.1.1/libs/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/faq.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/index.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/installing.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/limitations.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/pybind11-logo.png` & `pylibCZIrw-4.1.1/libs/pybind11/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/pybind11_vs_boost_python1.png` & `pylibCZIrw-4.1.1/libs/pybind11/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/pybind11_vs_boost_python1.svg` & `pylibCZIrw-4.1.1/libs/pybind11/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/pybind11_vs_boost_python2.png` & `pylibCZIrw-4.1.1/libs/pybind11/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/pybind11_vs_boost_python2.svg` & `pylibCZIrw-4.1.1/libs/pybind11/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/reference.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/release.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/release.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/docs/upgrade.rst` & `pylibCZIrw-4.1.1/libs/pybind11/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/attr.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/buffer_info.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/cast.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/chrono.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/complex.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/detail/class.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/detail/common.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/detail/descr.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/detail/init.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/detail/internals.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/detail/type_caster_base.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/detail/typeid.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/eigen/matrix.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/eigen/tensor.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/embed.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/eval.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/functional.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/gil.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/iostream.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/numpy.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/operators.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/options.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/pybind11.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/pytypes.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/stl/filesystem.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/stl.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/stl_bind.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/include/pybind11/type_caster_pyobject_ptr.h` & `pylibCZIrw-4.1.1/libs/pybind11/include/pybind11/type_caster_pyobject_ptr.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/noxfile.py` & `pylibCZIrw-4.1.1/libs/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/pybind11/__main__.py` & `pylibCZIrw-4.1.1/libs/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/pybind11/commands.py` & `pylibCZIrw-4.1.1/libs/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/pybind11/setup_helpers.py` & `pylibCZIrw-4.1.1/libs/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/pyproject.toml` & `pylibCZIrw-4.1.1/libs/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/setup.cfg` & `pylibCZIrw-4.1.1/libs/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/setup.py` & `pylibCZIrw-4.1.1/libs/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/CMakeLists.txt` & `pylibCZIrw-4.1.1/libs/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/conftest.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/constructor_stats.h` & `pylibCZIrw-4.1.1/libs/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/cross_module_gil_utils.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/cross_module_interleaved_error_already_set.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/cross_module_interleaved_error_already_set.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/env.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/env.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/extra_python_package/test_files.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/extra_setuptools/test_setuphelper.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/local_bindings.h` & `pylibCZIrw-4.1.1/libs/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/object.h` & `pylibCZIrw-4.1.1/libs/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/pybind11_cross_module_tests.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/pybind11_tests.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/pybind11_tests.h` & `pylibCZIrw-4.1.1/libs/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/pytest.ini` & `pylibCZIrw-4.1.1/libs/pybind11/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/requirements.txt` & `pylibCZIrw-4.1.1/libs/pybind11/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_async.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_async.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_buffers.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_buffers.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_builtin_casters.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_builtin_casters.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_call_policies.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_call_policies.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_callbacks.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_callbacks.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_chrono.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_chrono.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_class.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_class.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/CMakeLists.txt` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/embed.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_const_name.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_const_name.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_const_name.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_const_name.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_constants_and_functions.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_constants_and_functions.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_copy_move.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_copy_move.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_custom_type_casters.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_custom_type_casters.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_custom_type_setup.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_custom_type_setup.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_custom_type_setup.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_custom_type_setup.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_docstring_options.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_docstring_options.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_eigen_matrix.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_eigen_matrix.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_eigen_matrix.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_eigen_matrix.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_eigen_tensor.inl` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_eigen_tensor.inl`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_eigen_tensor.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_eigen_tensor.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_embed/CMakeLists.txt` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_embed/catch.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_embed/external_module.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_embed/test_interpreter.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_enum.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_enum.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_eval.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_eval.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_exceptions.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_exceptions.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_factory_constructors.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_factory_constructors.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_gil_scoped.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_gil_scoped.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_iostream.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_iostream.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_kwargs_and_defaults.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_kwargs_and_defaults.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_local_bindings.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_local_bindings.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_methods_and_attributes.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_methods_and_attributes.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_modules.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_modules.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_multiple_inheritance.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_multiple_inheritance.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_numpy_array.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_numpy_array.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_numpy_dtypes.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_numpy_dtypes.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_numpy_vectorize.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_numpy_vectorize.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_opaque_types.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_opaque_types.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_operator_overloading.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_operator_overloading.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_pickling.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_pickling.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_pytypes.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_pytypes.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_sequences_and_iterators.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_sequences_and_iterators.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_smart_ptr.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_smart_ptr.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_stl.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_stl.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_stl_binders.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_stl_binders.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_tagbased_polymorphic.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_tagbased_polymorphic.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_thread.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_thread.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_thread.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_type_caster_pyobject_ptr.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_type_caster_pyobject_ptr.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_type_caster_pyobject_ptr.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_type_caster_pyobject_ptr.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_union.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_unnamed_namespace_a.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_unnamed_namespace_a.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_unnamed_namespace_a.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_unnamed_namespace_a.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_vector_unique_ptr_member.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_vector_unique_ptr_member.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_virtual_functions.cpp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/test_virtual_functions.py` & `pylibCZIrw-4.1.1/libs/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/valgrind-numpy-scipy.supp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tests/valgrind-python.supp` & `pylibCZIrw-4.1.1/libs/pybind11/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tools/FindCatch.cmake` & `pylibCZIrw-4.1.1/libs/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tools/FindEigen3.cmake` & `pylibCZIrw-4.1.1/libs/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tools/FindPythonLibsNew.cmake` & `pylibCZIrw-4.1.1/libs/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tools/JoinPaths.cmake` & `pylibCZIrw-4.1.1/libs/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tools/check-style.sh` & `pylibCZIrw-4.1.1/libs/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tools/cmake_uninstall.cmake.in` & `pylibCZIrw-4.1.1/libs/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tools/codespell_ignore_lines_from_errors.py` & `pylibCZIrw-4.1.1/libs/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tools/libsize.py` & `pylibCZIrw-4.1.1/libs/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tools/make_changelog.py` & `pylibCZIrw-4.1.1/libs/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tools/pybind11Common.cmake` & `pylibCZIrw-4.1.1/libs/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tools/pybind11Config.cmake.in` & `pylibCZIrw-4.1.1/libs/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tools/pybind11NewTools.cmake` & `pylibCZIrw-4.1.1/libs/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tools/pybind11Tools.cmake` & `pylibCZIrw-4.1.1/libs/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tools/setup_global.py.in` & `pylibCZIrw-4.1.1/libs/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/libs/pybind11/tools/setup_main.py.in` & `pylibCZIrw-4.1.1/libs/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/pylibCZIrw/__init__.py` & `pylibCZIrw-4.1.1/pylibCZIrw/__init__.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/pylibCZIrw/czi.py` & `pylibCZIrw-4.1.1/pylibCZIrw/czi.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/pylibCZIrw-documentation.html` & `pylibCZIrw-4.1.1/pylibCZIrw-documentation.html`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/pylibCZIrw.egg-info/PKG-INFO` & `pylibCZIrw-4.1.1/pylibCZIrw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibCZIrw
-Version: 4.1.0
+Version: 4.1.1
 Summary: A python wrapper around the libCZI C++ library with reading and writing functionality.
 Author: Sebastian Soyer
 Author-email: sebastian.soyer@zeiss.com
 Keywords: czi,imaging
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pylibCZIrw-4.1.0/pylibCZIrw.egg-info/SOURCES.txt` & `pylibCZIrw-4.1.1/pylibCZIrw.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,16 @@
 libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo.h
 libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo2.cpp
 libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo2.h
 libs/libCZIrw/Src/libCZI/CziMetadataSegment.cpp
 libs/libCZIrw/Src/libCZI/CziMetadataSegment.h
 libs/libCZIrw/Src/libCZI/CziParse.cpp
 libs/libCZIrw/Src/libCZI/CziParse.h
+libs/libCZIrw/Src/libCZI/CziReaderCommon.cpp
+libs/libCZIrw/Src/libCZI/CziReaderCommon.h
 libs/libCZIrw/Src/libCZI/CziReaderWriter.cpp
 libs/libCZIrw/Src/libCZI/CziReaderWriter.h
 libs/libCZIrw/Src/libCZI/CziStructs.cpp
 libs/libCZIrw/Src/libCZI/CziStructs.h
 libs/libCZIrw/Src/libCZI/CziSubBlock.cpp
 libs/libCZIrw/Src/libCZI/CziSubBlock.h
 libs/libCZIrw/Src/libCZI/CziSubBlockDirectory.cpp
```

### Comparing `pylibCZIrw-4.1.0/setup.cfg` & `pylibCZIrw-4.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-4.1.0/setup.py` & `pylibCZIrw-4.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import platform
 import re
 import subprocess
 import sys
 from distutils.version import LooseVersion
 from typing import List
 
-VERSION = "4.1.0"
+VERSION = "4.1.1"
 
 with open("INFO.md") as readme_file:
     readme = readme_file.read()
 
 # List any runtime requirements here
 requirements = ["numpy", "cmake", "xmltodict", "validators"]
```


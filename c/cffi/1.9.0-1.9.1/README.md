# Comparing `tmp/cffi-1.9.0.tar.gz` & `tmp/cffi-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cffi-1.9.0.tar", last modified: Sat Nov 12 13:32:57 2016, max compression
+gzip compressed data, was "dist/cffi-1.9.1.tar", last modified: Sat Nov 12 13:46:13 2016, max compression
```

## Comparing `cffi-1.9.0.tar` & `cffi-1.9.1.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/
--rw-r--r--   0 arigo     (1000) arigo     (1000)     7384 2016-11-12 13:32:52.000000 cffi-1.9.0/setup.py
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/cffi.egg-info/
--rw-r--r--   0 arigo     (1000) arigo     (1000)        1 2016-11-12 13:32:57.000000 cffi-1.9.0/cffi.egg-info/not-zip-safe
--rw-r--r--   0 arigo     (1000) arigo     (1000)       19 2016-11-12 13:32:57.000000 cffi-1.9.0/cffi.egg-info/top_level.txt
--rw-r--r--   0 arigo     (1000) arigo     (1000)        1 2016-11-12 13:32:57.000000 cffi-1.9.0/cffi.egg-info/dependency_links.txt
--rw-r--r--   0 arigo     (1000) arigo     (1000)       76 2016-11-12 13:32:57.000000 cffi-1.9.0/cffi.egg-info/entry_points.txt
--rw-r--r--   0 arigo     (1000) arigo     (1000)     4769 2016-11-12 13:32:57.000000 cffi-1.9.0/cffi.egg-info/SOURCES.txt
--rw-r--r--   0 arigo     (1000) arigo     (1000)       10 2016-11-12 13:32:57.000000 cffi-1.9.0/cffi.egg-info/requires.txt
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1163 2016-11-12 13:32:57.000000 cffi-1.9.0/cffi.egg-info/PKG-INFO
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/testing/
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/testing/cffi0/
--rw-r--r--   0 arigo     (1000) arigo     (1000)     6386 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/test_zintegration.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    16879 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/test_function.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      316 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/test_verify2.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    14845 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/test_parsing.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    69698 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/backend_tests.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1211 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/callback_in_thread.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     4624 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/test_model.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    82986 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/test_verify.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      328 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/test_vgen.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      925 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/test_cdata.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     2178 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/test_unicode_literals.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     8534 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/test_ownlib.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     2106 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/test_version.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/__init__.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    11766 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/test_zdistutils.py
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/testing/cffi0/snippets/
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/testing/cffi0/snippets/setuptools_module/
--rw-r--r--   0 arigo     (1000) arigo     (1000)      202 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/snippets/setuptools_module/setup.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      428 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/snippets/setuptools_module/snip_setuptools_verify.py
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/testing/cffi0/snippets/distutils_package_2/
--rw-r--r--   0 arigo     (1000) arigo     (1000)      210 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/snippets/distutils_package_2/setup.py
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/testing/cffi0/snippets/distutils_package_2/snip_basic_verify2/
--rw-r--r--   0 arigo     (1000) arigo     (1000)      467 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/snippets/distutils_package_2/snip_basic_verify2/__init__.py
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/testing/cffi0/snippets/distutils_module/
--rw-r--r--   0 arigo     (1000) arigo     (1000)      171 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/snippets/distutils_module/setup.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      428 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/snippets/distutils_module/snip_basic_verify.py
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/testing/cffi0/snippets/setuptools_package_1/
--rw-r--r--   0 arigo     (1000) arigo     (1000)      203 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/snippets/setuptools_package_1/setup.py
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/testing/cffi0/snippets/setuptools_package_1/snip_setuptools_verify1/
--rw-r--r--   0 arigo     (1000) arigo     (1000)      428 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/snippets/setuptools_package_1/snip_setuptools_verify1/__init__.py
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/testing/cffi0/snippets/infrastructure/
--rw-r--r--   0 arigo     (1000) arigo     (1000)      100 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/snippets/infrastructure/setup.py
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/testing/cffi0/snippets/infrastructure/snip_infrastructure/
--rw-r--r--   0 arigo     (1000) arigo     (1000)       27 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/snippets/infrastructure/snip_infrastructure/__init__.py
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/testing/cffi0/snippets/distutils_package_1/
--rw-r--r--   0 arigo     (1000) arigo     (1000)      172 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/snippets/distutils_package_1/setup.py
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/testing/cffi0/snippets/distutils_package_1/snip_basic_verify1/
--rw-r--r--   0 arigo     (1000) arigo     (1000)      428 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/snippets/distutils_package_1/snip_basic_verify1/__init__.py
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/testing/cffi0/snippets/setuptools_package_2/
--rw-r--r--   0 arigo     (1000) arigo     (1000)      246 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/snippets/setuptools_package_2/setup.py
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/testing/cffi0/snippets/setuptools_package_2/snip_setuptools_verify2/
--rw-r--r--   0 arigo     (1000) arigo     (1000)      472 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/snippets/setuptools_package_2/snip_setuptools_verify2/__init__.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      858 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/test_platform.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1572 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/test_ctypes.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      425 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/test_vgen2.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    19357 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi0/test_ffi_backend.py
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/testing/embedding/
--rw-r--r--   0 arigo     (1000) arigo     (1000)      362 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/test_tlocal.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1931 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/perf-test.c
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1028 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/thread2-test.c
--rw-r--r--   0 arigo     (1000) arigo     (1000)      639 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/add1.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      475 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/add_recursive-test.c
--rw-r--r--   0 arigo     (1000) arigo     (1000)      174 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/add1-test.c
--rw-r--r--   0 arigo     (1000) arigo     (1000)      626 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/test_recursive.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      313 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/perf.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      833 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/tlocal-test.c
--rw-r--r--   0 arigo     (1000) arigo     (1000)     7256 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/test_basic.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      446 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/add3.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1791 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/test_performance.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      150 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/empty.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      670 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/tlocal.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1050 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/thread3-test.c
--rw-r--r--   0 arigo     (1000) arigo     (1000)      733 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/add_recursive.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/__init__.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     2641 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/test_thread.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     2245 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/thread-test.h
--rw-r--r--   0 arigo     (1000) arigo     (1000)      211 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/add2-test.c
--rw-r--r--   0 arigo     (1000) arigo     (1000)      558 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/add2.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      744 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/embedding/thread1-test.c
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1815 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/support.py
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/testing/cffi1/
--rw-r--r--   0 arigo     (1000) arigo     (1000)      720 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi1/test_cffi_binary.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      918 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi1/test_commontypes.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     2484 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi1/test_realize_c_type.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     6836 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi1/test_re_python.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    76693 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi1/test_verify1.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    64617 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi1/test_new_ffi_1.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1092 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi1/test_unicode_literals.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    14910 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi1/test_parse_c_type.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     7123 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi1/test_dlopen.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi1/__init__.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    16496 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi1/test_ffi_obj.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    73918 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi1/test_recompiler.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    16789 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi1/test_zdist.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      186 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/cffi1/test_dlopen_unicode_literals.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/__init__.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      287 2016-11-12 13:32:52.000000 cffi-1.9.0/testing/udir.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      913 2016-11-12 13:32:52.000000 cffi-1.9.0/setup_base.py
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/demo/
--rwxr-xr-x   0 arigo     (1000) arigo     (1000)      862 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/py.cleanup
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1004 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/gmp.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1789 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/readdir_ctypes.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     3399 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/pyobj.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      827 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/readdir.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      193 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/setup_manual.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      326 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/bsdopendirtype_setup.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1370 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/recopendirtype.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      166 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/pwuid.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1210 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/winclipboard.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      393 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/recopendirtype_build.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     8868 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/_curses_build.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     8352 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/fastcsv.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      249 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/readdir_setup.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      983 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/embedding_test.c
--rw-r--r--   0 arigo     (1000) arigo     (1000)      305 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/_curses_setup.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      762 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/xclient.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      749 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/xclient_build.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      575 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/bsdopendirtype_build.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      707 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/gmp_build.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      844 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/winclipboard_build.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1119 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/btrfs-snap.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      779 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/readdir2_build.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      961 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/readdir2.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1338 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/extern_python_varargs.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      890 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/readdir_build.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1643 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/api.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      358 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/pwuid_build.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      201 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/readdir2_setup.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      460 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/extern_python.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      398 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/embedding.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1175 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/manual2.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    30644 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/_curses.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1240 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/bsdopendirtype.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     3354 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/cffi-cocoa.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     3521 2016-11-12 13:32:52.000000 cffi-1.9.0/demo/manual.c
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/cffi/
--rw-r--r--   0 arigo     (1000) arigo     (1000)    41373 2016-11-12 13:32:52.000000 cffi-1.9.0/cffi/vengine_cpy.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    21352 2016-11-12 13:32:52.000000 cffi-1.9.0/cffi/model.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     2678 2016-11-12 13:32:52.000000 cffi-1.9.0/cffi/commontypes.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    41745 2016-11-12 13:32:52.000000 cffi-1.9.0/cffi/backend_ctypes.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    37419 2016-11-12 13:32:52.000000 cffi-1.9.0/cffi/cparser.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     5835 2016-11-12 13:32:52.000000 cffi-1.9.0/cffi/parse_c_type.h
--rw-r--r--   0 arigo     (1000) arigo     (1000)     3860 2016-11-12 13:32:52.000000 cffi-1.9.0/cffi/ffiplatform.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    26633 2016-11-12 13:32:52.000000 cffi-1.9.0/cffi/vengine_gen.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    37242 2016-11-12 13:32:52.000000 cffi-1.9.0/cffi/api.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)      747 2016-11-12 13:32:52.000000 cffi-1.9.0/cffi/lock.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    17274 2016-11-12 13:32:52.000000 cffi-1.9.0/cffi/_embedding.h
--rw-r--r--   0 arigo     (1000) arigo     (1000)      483 2016-11-12 13:32:52.000000 cffi-1.9.0/cffi/__init__.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     7366 2016-11-12 13:32:52.000000 cffi-1.9.0/cffi/setuptools_ext.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     5477 2016-11-12 13:32:52.000000 cffi-1.9.0/cffi/cffi_opcode.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    10238 2016-11-12 13:32:52.000000 cffi-1.9.0/cffi/_cffi_include.h
--rw-r--r--   0 arigo     (1000) arigo     (1000)    11518 2016-11-12 13:32:52.000000 cffi-1.9.0/cffi/verifier.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    61394 2016-11-12 13:32:52.000000 cffi-1.9.0/cffi/recompiler.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1294 2016-11-12 13:32:52.000000 cffi-1.9.0/LICENSE
--rw-r--r--   0 arigo     (1000) arigo     (1000)      280 2016-11-12 13:32:52.000000 cffi-1.9.0/MANIFEST.in
--rw-r--r--   0 arigo     (1000) arigo     (1000)       59 2016-11-12 13:32:57.000000 cffi-1.9.0/setup.cfg
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1163 2016-11-12 13:32:57.000000 cffi-1.9.0/PKG-INFO
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/c/
--rw-r--r--   0 arigo     (1000) arigo     (1000)    25212 2016-11-12 13:32:52.000000 cffi-1.9.0/c/realize_c_type.c
--rw-r--r--   0 arigo     (1000) arigo     (1000)   229733 2016-11-12 13:32:52.000000 cffi-1.9.0/c/_cffi_backend.c
--rw-r--r--   0 arigo     (1000) arigo     (1000)    13591 2016-11-12 13:32:52.000000 cffi-1.9.0/c/cdlopen.c
--rw-r--r--   0 arigo     (1000) arigo     (1000)     4844 2016-11-12 13:32:52.000000 cffi-1.9.0/c/malloc_closure.h
--rw-r--r--   0 arigo     (1000) arigo     (1000)     3351 2016-11-12 13:32:52.000000 cffi-1.9.0/c/cglob.c
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/c/libffi_msvc/
--rw-r--r--   0 arigo     (1000) arigo     (1000)     2699 2016-11-12 13:32:52.000000 cffi-1.9.0/c/libffi_msvc/ffitarget.h
--rw-r--r--   0 arigo     (1000) arigo     (1000)     3556 2016-11-12 13:32:52.000000 cffi-1.9.0/c/libffi_msvc/types.c
--rw-r--r--   0 arigo     (1000) arigo     (1000)     4713 2016-11-12 13:32:52.000000 cffi-1.9.0/c/libffi_msvc/win32.c
--rw-r--r--   0 arigo     (1000) arigo     (1000)     2114 2016-11-12 13:32:52.000000 cffi-1.9.0/c/libffi_msvc/ffi_common.h
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1176 2016-11-12 13:32:52.000000 cffi-1.9.0/c/libffi_msvc/win64.obj
--rw-r--r--   0 arigo     (1000) arigo     (1000)     9297 2016-11-12 13:32:52.000000 cffi-1.9.0/c/libffi_msvc/ffi.h
--rw-r--r--   0 arigo     (1000) arigo     (1000)     5620 2016-11-12 13:32:52.000000 cffi-1.9.0/c/libffi_msvc/prep_cif.c
--rw-r--r--   0 arigo     (1000) arigo     (1000)     3096 2016-11-12 13:32:52.000000 cffi-1.9.0/c/libffi_msvc/win64.asm
--rw-r--r--   0 arigo     (1000) arigo     (1000)    12096 2016-11-12 13:32:52.000000 cffi-1.9.0/c/libffi_msvc/ffi.c
--rw-r--r--   0 arigo     (1000) arigo     (1000)     2973 2016-11-12 13:32:52.000000 cffi-1.9.0/c/libffi_msvc/fficonfig.h
--rw-r--r--   0 arigo     (1000) arigo     (1000)     3450 2016-11-12 13:32:52.000000 cffi-1.9.0/c/wchar_helper.h
--rw-r--r--   0 arigo     (1000) arigo     (1000)     3896 2016-11-12 13:32:52.000000 cffi-1.9.0/c/misc_thread_common.h
--rw-r--r--   0 arigo     (1000) arigo     (1000)     1411 2016-11-12 13:32:52.000000 cffi-1.9.0/c/misc_thread_posix.h
--rw-r--r--   0 arigo     (1000) arigo     (1000)    25661 2016-11-12 13:32:52.000000 cffi-1.9.0/c/parse_c_type.c
--rw-r--r--   0 arigo     (1000) arigo     (1000)     6270 2016-11-12 13:32:52.000000 cffi-1.9.0/c/misc_win32.h
--rw-r--r--   0 arigo     (1000) arigo     (1000)     8952 2016-11-12 13:32:52.000000 cffi-1.9.0/c/minibuffer.h
--rw-r--r--   0 arigo     (1000) arigo     (1000)    22667 2016-11-12 13:32:52.000000 cffi-1.9.0/c/lib_obj.c
--rw-r--r--   0 arigo     (1000) arigo     (1000)     6256 2016-11-12 13:32:52.000000 cffi-1.9.0/c/commontypes.c
--rw-r--r--   0 arigo     (1000) arigo     (1000)     8765 2016-11-12 13:32:52.000000 cffi-1.9.0/c/call_python.c
--rw-r--r--   0 arigo     (1000) arigo     (1000)     2215 2016-11-12 13:32:52.000000 cffi-1.9.0/c/file_emulator.h
--rw-r--r--   0 arigo     (1000) arigo     (1000)   135163 2016-11-12 13:32:52.000000 cffi-1.9.0/c/test_c.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    43233 2016-11-12 13:32:52.000000 cffi-1.9.0/c/ffi_obj.c
--rw-r--r--   0 arigo     (1000) arigo     (1000)     6935 2016-11-12 13:32:52.000000 cffi-1.9.0/c/cffi1_module.c
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/doc/
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/doc/source/
--rw-r--r--   0 arigo     (1000) arigo     (1000)    39254 2016-11-12 13:32:52.000000 cffi-1.9.0/doc/source/cdef.rst
--rw-r--r--   0 arigo     (1000) arigo     (1000)    31370 2016-11-12 13:32:52.000000 cffi-1.9.0/doc/source/ref.rst
--rw-r--r--   0 arigo     (1000) arigo     (1000)    35075 2016-11-12 13:32:52.000000 cffi-1.9.0/doc/source/using.rst
--rw-r--r--   0 arigo     (1000) arigo     (1000)     3060 2016-11-12 13:32:52.000000 cffi-1.9.0/doc/source/index.rst
--rw-r--r--   0 arigo     (1000) arigo     (1000)    15560 2016-11-12 13:32:52.000000 cffi-1.9.0/doc/source/overview.rst
--rw-r--r--   0 arigo     (1000) arigo     (1000)     6737 2016-11-12 13:32:52.000000 cffi-1.9.0/doc/source/installation.rst
--rw-r--r--   0 arigo     (1000) arigo     (1000)     6333 2016-11-12 13:32:52.000000 cffi-1.9.0/doc/source/conf.py
--rw-r--r--   0 arigo     (1000) arigo     (1000)    18908 2016-11-12 13:32:52.000000 cffi-1.9.0/doc/source/embedding.rst
--rw-r--r--   0 arigo     (1000) arigo     (1000)    16028 2016-11-12 13:32:52.000000 cffi-1.9.0/doc/source/whatsnew.rst
--rw-r--r--   0 arigo     (1000) arigo     (1000)     3126 2016-11-12 13:32:52.000000 cffi-1.9.0/doc/Makefile
-drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:32:57.000000 cffi-1.9.0/doc/misc/
--rw-r--r--   0 arigo     (1000) arigo     (1000)     2779 2016-11-12 13:32:52.000000 cffi-1.9.0/doc/misc/design.rst
--rw-r--r--   0 arigo     (1000) arigo     (1000)     5445 2016-11-12 13:32:52.000000 cffi-1.9.0/doc/misc/grant-cffi-1.0.rst
--rw-r--r--   0 arigo     (1000) arigo     (1000)     2253 2016-11-12 13:32:52.000000 cffi-1.9.0/doc/misc/parse_c_type.rst
--rw-r--r--   0 arigo     (1000) arigo     (1000)     3071 2016-11-12 13:32:52.000000 cffi-1.9.0/doc/make.bat
--rw-r--r--   0 arigo     (1000) arigo     (1000)      208 2016-11-12 13:32:52.000000 cffi-1.9.0/AUTHORS
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     7384 2016-11-12 13:45:24.000000 cffi-1.9.1/setup.py
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/cffi.egg-info/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)        1 2016-11-12 13:46:13.000000 cffi-1.9.1/cffi.egg-info/not-zip-safe
+-rw-r--r--   0 arigo     (1000) arigo     (1000)       19 2016-11-12 13:46:13.000000 cffi-1.9.1/cffi.egg-info/top_level.txt
+-rw-r--r--   0 arigo     (1000) arigo     (1000)        1 2016-11-12 13:46:13.000000 cffi-1.9.1/cffi.egg-info/dependency_links.txt
+-rw-r--r--   0 arigo     (1000) arigo     (1000)       76 2016-11-12 13:46:13.000000 cffi-1.9.1/cffi.egg-info/entry_points.txt
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     4769 2016-11-12 13:46:13.000000 cffi-1.9.1/cffi.egg-info/SOURCES.txt
+-rw-r--r--   0 arigo     (1000) arigo     (1000)       10 2016-11-12 13:46:13.000000 cffi-1.9.1/cffi.egg-info/requires.txt
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1163 2016-11-12 13:46:13.000000 cffi-1.9.1/cffi.egg-info/PKG-INFO
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/testing/
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/testing/cffi0/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     6386 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/test_zintegration.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    16879 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/test_function.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      316 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/test_verify2.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    14845 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/test_parsing.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    69698 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/backend_tests.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1211 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/callback_in_thread.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     4624 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/test_model.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    82986 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/test_verify.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      328 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/test_vgen.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      925 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/test_cdata.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     2178 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/test_unicode_literals.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     8534 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/test_ownlib.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     2106 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/test_version.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/__init__.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    11766 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/test_zdistutils.py
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/testing/cffi0/snippets/
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/testing/cffi0/snippets/setuptools_module/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      202 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/snippets/setuptools_module/setup.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      428 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/snippets/setuptools_module/snip_setuptools_verify.py
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/testing/cffi0/snippets/distutils_package_2/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      210 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/snippets/distutils_package_2/setup.py
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/testing/cffi0/snippets/distutils_package_2/snip_basic_verify2/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      467 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/snippets/distutils_package_2/snip_basic_verify2/__init__.py
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/testing/cffi0/snippets/distutils_module/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      171 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/snippets/distutils_module/setup.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      428 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/snippets/distutils_module/snip_basic_verify.py
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/testing/cffi0/snippets/setuptools_package_1/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      203 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/snippets/setuptools_package_1/setup.py
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/testing/cffi0/snippets/setuptools_package_1/snip_setuptools_verify1/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      428 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/snippets/setuptools_package_1/snip_setuptools_verify1/__init__.py
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/testing/cffi0/snippets/infrastructure/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      100 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/snippets/infrastructure/setup.py
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/testing/cffi0/snippets/infrastructure/snip_infrastructure/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)       27 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/snippets/infrastructure/snip_infrastructure/__init__.py
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/testing/cffi0/snippets/distutils_package_1/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      172 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/snippets/distutils_package_1/setup.py
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/testing/cffi0/snippets/distutils_package_1/snip_basic_verify1/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      428 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/snippets/distutils_package_1/snip_basic_verify1/__init__.py
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/testing/cffi0/snippets/setuptools_package_2/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      246 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/snippets/setuptools_package_2/setup.py
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/testing/cffi0/snippets/setuptools_package_2/snip_setuptools_verify2/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      472 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/snippets/setuptools_package_2/snip_setuptools_verify2/__init__.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      858 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/test_platform.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1572 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/test_ctypes.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      425 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/test_vgen2.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    19357 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi0/test_ffi_backend.py
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/testing/embedding/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      362 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/test_tlocal.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1931 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/perf-test.c
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1028 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/thread2-test.c
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      639 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/add1.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      475 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/add_recursive-test.c
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      174 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/add1-test.c
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      626 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/test_recursive.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      313 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/perf.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      833 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/tlocal-test.c
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     7256 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/test_basic.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      446 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/add3.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1791 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/test_performance.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      150 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/empty.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      670 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/tlocal.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1050 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/thread3-test.c
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      733 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/add_recursive.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/__init__.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     2641 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/test_thread.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     2245 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/thread-test.h
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      211 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/add2-test.c
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      558 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/add2.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      744 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/embedding/thread1-test.c
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1815 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/support.py
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/testing/cffi1/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      720 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi1/test_cffi_binary.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      918 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi1/test_commontypes.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     2484 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi1/test_realize_c_type.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     6836 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi1/test_re_python.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    76693 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi1/test_verify1.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    64617 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi1/test_new_ffi_1.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1092 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi1/test_unicode_literals.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    14910 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi1/test_parse_c_type.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     7123 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi1/test_dlopen.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi1/__init__.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    16496 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi1/test_ffi_obj.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    73918 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi1/test_recompiler.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    16789 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi1/test_zdist.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      186 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/cffi1/test_dlopen_unicode_literals.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/__init__.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      287 2016-11-12 13:45:16.000000 cffi-1.9.1/testing/udir.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      913 2016-11-12 13:45:16.000000 cffi-1.9.1/setup_base.py
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/demo/
+-rwxr-xr-x   0 arigo     (1000) arigo     (1000)      862 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/py.cleanup
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1004 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/gmp.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1789 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/readdir_ctypes.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     3399 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/pyobj.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      827 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/readdir.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      193 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/setup_manual.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      326 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/bsdopendirtype_setup.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1370 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/recopendirtype.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      166 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/pwuid.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1210 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/winclipboard.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      393 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/recopendirtype_build.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     8868 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/_curses_build.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     8352 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/fastcsv.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      249 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/readdir_setup.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      983 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/embedding_test.c
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      305 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/_curses_setup.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      762 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/xclient.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      749 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/xclient_build.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      575 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/bsdopendirtype_build.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      707 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/gmp_build.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      844 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/winclipboard_build.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1119 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/btrfs-snap.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      779 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/readdir2_build.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      961 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/readdir2.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1338 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/extern_python_varargs.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      890 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/readdir_build.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1643 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/api.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      358 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/pwuid_build.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      201 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/readdir2_setup.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      460 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/extern_python.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      398 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/embedding.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1175 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/manual2.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    30644 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/_curses.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1240 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/bsdopendirtype.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     3354 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/cffi-cocoa.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     3521 2016-11-12 13:45:16.000000 cffi-1.9.1/demo/manual.c
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/cffi/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    41373 2016-11-12 13:45:16.000000 cffi-1.9.1/cffi/vengine_cpy.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    21352 2016-11-12 13:45:16.000000 cffi-1.9.1/cffi/model.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     2678 2016-11-12 13:45:16.000000 cffi-1.9.1/cffi/commontypes.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    41745 2016-11-12 13:45:16.000000 cffi-1.9.1/cffi/backend_ctypes.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    37419 2016-11-12 13:45:16.000000 cffi-1.9.1/cffi/cparser.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     5835 2016-11-12 13:45:16.000000 cffi-1.9.1/cffi/parse_c_type.h
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     3860 2016-11-12 13:45:16.000000 cffi-1.9.1/cffi/ffiplatform.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    26633 2016-11-12 13:45:16.000000 cffi-1.9.1/cffi/vengine_gen.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    37242 2016-11-12 13:45:16.000000 cffi-1.9.1/cffi/api.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      747 2016-11-12 13:45:16.000000 cffi-1.9.1/cffi/lock.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    17274 2016-11-12 13:45:24.000000 cffi-1.9.1/cffi/_embedding.h
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      483 2016-11-12 13:45:24.000000 cffi-1.9.1/cffi/__init__.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     7366 2016-11-12 13:45:16.000000 cffi-1.9.1/cffi/setuptools_ext.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     5477 2016-11-12 13:45:16.000000 cffi-1.9.1/cffi/cffi_opcode.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    10238 2016-11-12 13:45:16.000000 cffi-1.9.1/cffi/_cffi_include.h
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    11518 2016-11-12 13:45:16.000000 cffi-1.9.1/cffi/verifier.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    61394 2016-11-12 13:45:16.000000 cffi-1.9.1/cffi/recompiler.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1294 2016-11-12 13:45:16.000000 cffi-1.9.1/LICENSE
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      280 2016-11-12 13:45:16.000000 cffi-1.9.1/MANIFEST.in
+-rw-r--r--   0 arigo     (1000) arigo     (1000)       59 2016-11-12 13:46:13.000000 cffi-1.9.1/setup.cfg
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1163 2016-11-12 13:46:13.000000 cffi-1.9.1/PKG-INFO
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/c/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    25212 2016-11-12 13:45:16.000000 cffi-1.9.1/c/realize_c_type.c
+-rw-r--r--   0 arigo     (1000) arigo     (1000)   229744 2016-11-12 13:45:24.000000 cffi-1.9.1/c/_cffi_backend.c
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    13591 2016-11-12 13:45:16.000000 cffi-1.9.1/c/cdlopen.c
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     4844 2016-11-12 13:45:16.000000 cffi-1.9.1/c/malloc_closure.h
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     3351 2016-11-12 13:45:16.000000 cffi-1.9.1/c/cglob.c
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/c/libffi_msvc/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     2699 2016-11-12 13:45:16.000000 cffi-1.9.1/c/libffi_msvc/ffitarget.h
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     3556 2016-11-12 13:45:16.000000 cffi-1.9.1/c/libffi_msvc/types.c
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     4713 2016-11-12 13:45:16.000000 cffi-1.9.1/c/libffi_msvc/win32.c
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     2114 2016-11-12 13:45:16.000000 cffi-1.9.1/c/libffi_msvc/ffi_common.h
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1176 2016-11-12 13:45:16.000000 cffi-1.9.1/c/libffi_msvc/win64.obj
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     9297 2016-11-12 13:45:16.000000 cffi-1.9.1/c/libffi_msvc/ffi.h
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     5620 2016-11-12 13:45:16.000000 cffi-1.9.1/c/libffi_msvc/prep_cif.c
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     3096 2016-11-12 13:45:16.000000 cffi-1.9.1/c/libffi_msvc/win64.asm
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    12096 2016-11-12 13:45:16.000000 cffi-1.9.1/c/libffi_msvc/ffi.c
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     2973 2016-11-12 13:45:16.000000 cffi-1.9.1/c/libffi_msvc/fficonfig.h
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     3450 2016-11-12 13:45:16.000000 cffi-1.9.1/c/wchar_helper.h
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     3896 2016-11-12 13:45:16.000000 cffi-1.9.1/c/misc_thread_common.h
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     1411 2016-11-12 13:45:16.000000 cffi-1.9.1/c/misc_thread_posix.h
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    25661 2016-11-12 13:45:16.000000 cffi-1.9.1/c/parse_c_type.c
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     6270 2016-11-12 13:45:16.000000 cffi-1.9.1/c/misc_win32.h
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     8952 2016-11-12 13:45:16.000000 cffi-1.9.1/c/minibuffer.h
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    22667 2016-11-12 13:45:16.000000 cffi-1.9.1/c/lib_obj.c
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     6256 2016-11-12 13:45:16.000000 cffi-1.9.1/c/commontypes.c
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     8765 2016-11-12 13:45:16.000000 cffi-1.9.1/c/call_python.c
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     2215 2016-11-12 13:45:16.000000 cffi-1.9.1/c/file_emulator.h
+-rw-r--r--   0 arigo     (1000) arigo     (1000)   135163 2016-11-12 13:45:24.000000 cffi-1.9.1/c/test_c.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    43233 2016-11-12 13:45:16.000000 cffi-1.9.1/c/ffi_obj.c
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     6935 2016-11-12 13:45:16.000000 cffi-1.9.1/c/cffi1_module.c
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/doc/
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/doc/source/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    39254 2016-11-12 13:45:16.000000 cffi-1.9.1/doc/source/cdef.rst
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    31370 2016-11-12 13:45:16.000000 cffi-1.9.1/doc/source/ref.rst
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    35075 2016-11-12 13:45:16.000000 cffi-1.9.1/doc/source/using.rst
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     3060 2016-11-12 13:45:16.000000 cffi-1.9.1/doc/source/index.rst
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    15560 2016-11-12 13:45:16.000000 cffi-1.9.1/doc/source/overview.rst
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     6737 2016-11-12 13:45:24.000000 cffi-1.9.1/doc/source/installation.rst
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     6333 2016-11-12 13:45:24.000000 cffi-1.9.1/doc/source/conf.py
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    18908 2016-11-12 13:45:16.000000 cffi-1.9.1/doc/source/embedding.rst
+-rw-r--r--   0 arigo     (1000) arigo     (1000)    16028 2016-11-12 13:45:16.000000 cffi-1.9.1/doc/source/whatsnew.rst
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     3126 2016-11-12 13:45:16.000000 cffi-1.9.1/doc/Makefile
+drwxr-xr-x   0 arigo     (1000) arigo     (1000)        0 2016-11-12 13:46:13.000000 cffi-1.9.1/doc/misc/
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     2779 2016-11-12 13:45:16.000000 cffi-1.9.1/doc/misc/design.rst
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     5445 2016-11-12 13:45:16.000000 cffi-1.9.1/doc/misc/grant-cffi-1.0.rst
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     2253 2016-11-12 13:45:16.000000 cffi-1.9.1/doc/misc/parse_c_type.rst
+-rw-r--r--   0 arigo     (1000) arigo     (1000)     3071 2016-11-12 13:45:16.000000 cffi-1.9.1/doc/make.bat
+-rw-r--r--   0 arigo     (1000) arigo     (1000)      208 2016-11-12 13:45:16.000000 cffi-1.9.1/AUTHORS
```

### Comparing `cffi-1.9.0/setup.py` & `cffi-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 Please see the `Documentation <http://cffi.readthedocs.org/>`_.
 
 Contact
 -------
 
 `Mailing list <https://groups.google.com/forum/#!forum/python-cffi>`_
 """,
-        version='1.9.0',
+        version='1.9.1',
         packages=['cffi'] if cpython else [],
         package_data={'cffi': ['_cffi_include.h', 'parse_c_type.h', 
                                '_embedding.h']}
                      if cpython else {},
         zip_safe=False,
 
         url='http://cffi.readthedocs.org',
```

### Comparing `cffi-1.9.0/cffi.egg-info/SOURCES.txt` & `cffi-1.9.1/cffi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/cffi.egg-info/PKG-INFO` & `cffi-1.9.1/cffi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cffi
-Version: 1.9.0
+Version: 1.9.1
 Summary: Foreign Function Interface for Python calling C code.
 Home-page: http://cffi.readthedocs.org
 Author: Armin Rigo, Maciej Fijalkowski
 Author-email: python-cffi@googlegroups.com
 License: MIT
 Description: 
         CFFI
```

### Comparing `cffi-1.9.0/testing/cffi0/test_zintegration.py` & `cffi-1.9.1/testing/cffi0/test_zintegration.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi0/test_function.py` & `cffi-1.9.1/testing/cffi0/test_function.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi0/test_parsing.py` & `cffi-1.9.1/testing/cffi0/test_parsing.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi0/backend_tests.py` & `cffi-1.9.1/testing/cffi0/backend_tests.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi0/callback_in_thread.py` & `cffi-1.9.1/testing/cffi0/callback_in_thread.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi0/test_model.py` & `cffi-1.9.1/testing/cffi0/test_model.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi0/test_verify.py` & `cffi-1.9.1/testing/cffi0/test_verify.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi0/test_cdata.py` & `cffi-1.9.1/testing/cffi0/test_cdata.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi0/test_unicode_literals.py` & `cffi-1.9.1/testing/cffi0/test_unicode_literals.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi0/test_ownlib.py` & `cffi-1.9.1/testing/cffi0/test_ownlib.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi0/test_version.py` & `cffi-1.9.1/testing/cffi0/test_version.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi0/test_zdistutils.py` & `cffi-1.9.1/testing/cffi0/test_zdistutils.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi0/test_platform.py` & `cffi-1.9.1/testing/cffi0/test_platform.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi0/test_ctypes.py` & `cffi-1.9.1/testing/cffi0/test_ctypes.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi0/test_ffi_backend.py` & `cffi-1.9.1/testing/cffi0/test_ffi_backend.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/embedding/perf-test.c` & `cffi-1.9.1/testing/embedding/perf-test.c`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/embedding/thread2-test.c` & `cffi-1.9.1/testing/embedding/thread2-test.c`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/embedding/add1.py` & `cffi-1.9.1/testing/embedding/add1.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/embedding/test_recursive.py` & `cffi-1.9.1/testing/embedding/test_recursive.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/embedding/tlocal-test.c` & `cffi-1.9.1/testing/embedding/tlocal-test.c`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/embedding/test_basic.py` & `cffi-1.9.1/testing/embedding/test_basic.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/embedding/test_performance.py` & `cffi-1.9.1/testing/embedding/test_performance.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/embedding/tlocal.py` & `cffi-1.9.1/testing/embedding/tlocal.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/embedding/thread3-test.c` & `cffi-1.9.1/testing/embedding/thread3-test.c`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/embedding/add_recursive.py` & `cffi-1.9.1/testing/embedding/add_recursive.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/embedding/test_thread.py` & `cffi-1.9.1/testing/embedding/test_thread.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/embedding/thread-test.h` & `cffi-1.9.1/testing/embedding/thread-test.h`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/embedding/add2.py` & `cffi-1.9.1/testing/embedding/add2.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/embedding/thread1-test.c` & `cffi-1.9.1/testing/embedding/thread1-test.c`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/support.py` & `cffi-1.9.1/testing/support.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi1/test_cffi_binary.py` & `cffi-1.9.1/testing/cffi1/test_cffi_binary.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi1/test_commontypes.py` & `cffi-1.9.1/testing/cffi1/test_commontypes.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi1/test_realize_c_type.py` & `cffi-1.9.1/testing/cffi1/test_realize_c_type.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi1/test_re_python.py` & `cffi-1.9.1/testing/cffi1/test_re_python.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi1/test_verify1.py` & `cffi-1.9.1/testing/cffi1/test_verify1.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi1/test_new_ffi_1.py` & `cffi-1.9.1/testing/cffi1/test_new_ffi_1.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi1/test_unicode_literals.py` & `cffi-1.9.1/testing/cffi1/test_unicode_literals.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi1/test_parse_c_type.py` & `cffi-1.9.1/testing/cffi1/test_parse_c_type.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi1/test_dlopen.py` & `cffi-1.9.1/testing/cffi1/test_dlopen.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi1/test_ffi_obj.py` & `cffi-1.9.1/testing/cffi1/test_ffi_obj.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi1/test_recompiler.py` & `cffi-1.9.1/testing/cffi1/test_recompiler.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/testing/cffi1/test_zdist.py` & `cffi-1.9.1/testing/cffi1/test_zdist.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/setup_base.py` & `cffi-1.9.1/setup_base.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/py.cleanup` & `cffi-1.9.1/demo/py.cleanup`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/gmp.py` & `cffi-1.9.1/demo/gmp.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/readdir_ctypes.py` & `cffi-1.9.1/demo/readdir_ctypes.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/pyobj.py` & `cffi-1.9.1/demo/pyobj.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/readdir.py` & `cffi-1.9.1/demo/readdir.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/recopendirtype.py` & `cffi-1.9.1/demo/recopendirtype.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/winclipboard.py` & `cffi-1.9.1/demo/winclipboard.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/_curses_build.py` & `cffi-1.9.1/demo/_curses_build.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/fastcsv.py` & `cffi-1.9.1/demo/fastcsv.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/embedding_test.c` & `cffi-1.9.1/demo/embedding_test.c`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/xclient.py` & `cffi-1.9.1/demo/xclient.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/xclient_build.py` & `cffi-1.9.1/demo/xclient_build.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/bsdopendirtype_build.py` & `cffi-1.9.1/demo/bsdopendirtype_build.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/gmp_build.py` & `cffi-1.9.1/demo/gmp_build.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/winclipboard_build.py` & `cffi-1.9.1/demo/winclipboard_build.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/btrfs-snap.py` & `cffi-1.9.1/demo/btrfs-snap.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/readdir2_build.py` & `cffi-1.9.1/demo/readdir2_build.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/readdir2.py` & `cffi-1.9.1/demo/readdir2.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/extern_python_varargs.py` & `cffi-1.9.1/demo/extern_python_varargs.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/readdir_build.py` & `cffi-1.9.1/demo/readdir_build.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/api.py` & `cffi-1.9.1/demo/api.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/manual2.py` & `cffi-1.9.1/demo/manual2.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/_curses.py` & `cffi-1.9.1/demo/_curses.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/bsdopendirtype.py` & `cffi-1.9.1/demo/bsdopendirtype.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/cffi-cocoa.py` & `cffi-1.9.1/demo/cffi-cocoa.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/demo/manual.c` & `cffi-1.9.1/demo/manual.c`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/cffi/vengine_cpy.py` & `cffi-1.9.1/cffi/vengine_cpy.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/cffi/model.py` & `cffi-1.9.1/cffi/model.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/cffi/commontypes.py` & `cffi-1.9.1/cffi/commontypes.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/cffi/backend_ctypes.py` & `cffi-1.9.1/cffi/backend_ctypes.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/cffi/cparser.py` & `cffi-1.9.1/cffi/cparser.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/cffi/parse_c_type.h` & `cffi-1.9.1/cffi/parse_c_type.h`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/cffi/ffiplatform.py` & `cffi-1.9.1/cffi/ffiplatform.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/cffi/vengine_gen.py` & `cffi-1.9.1/cffi/vengine_gen.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/cffi/api.py` & `cffi-1.9.1/cffi/api.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/cffi/lock.py` & `cffi-1.9.1/cffi/lock.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/cffi/_embedding.h` & `cffi-1.9.1/cffi/_embedding.h`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
         Py_XDECREF(exception);
         Py_XDECREF(v);
         Py_XDECREF(tb);
 
         f = PySys_GetObject((char *)"stderr");
         if (f != NULL && f != Py_None) {
             PyFile_WriteString("\nFrom: " _CFFI_MODULE_NAME
-                               "\ncompiled with cffi version: 1.9.0"
+                               "\ncompiled with cffi version: 1.9.1"
                                "\n_cffi_backend module: ", f);
             modules = PyImport_GetModuleDict();
             mod = PyDict_GetItemString(modules, "_cffi_backend");
             if (mod == NULL) {
                 PyFile_WriteString("not loaded", f);
             }
             else {
```

### Comparing `cffi-1.9.0/cffi/setuptools_ext.py` & `cffi-1.9.1/cffi/setuptools_ext.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/cffi/cffi_opcode.py` & `cffi-1.9.1/cffi/cffi_opcode.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/cffi/_cffi_include.h` & `cffi-1.9.1/cffi/_cffi_include.h`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/cffi/verifier.py` & `cffi-1.9.1/cffi/verifier.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/cffi/recompiler.py` & `cffi-1.9.1/cffi/recompiler.py`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/LICENSE` & `cffi-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/PKG-INFO` & `cffi-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cffi
-Version: 1.9.0
+Version: 1.9.1
 Summary: Foreign Function Interface for Python calling C code.
 Home-page: http://cffi.readthedocs.org
 Author: Armin Rigo, Maciej Fijalkowski
 Author-email: python-cffi@googlegroups.com
 License: MIT
 Description: 
         CFFI
```

### Comparing `cffi-1.9.0/c/realize_c_type.c` & `cffi-1.9.1/c/realize_c_type.c`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/_cffi_backend.c` & `cffi-1.9.1/c/_cffi_backend.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
 #include "structmember.h"
 
-#define CFFI_VERSION  "1.9.0"
+#define CFFI_VERSION  "1.9.1"
 
 #ifdef MS_WIN32
 #include <windows.h>
 #include "misc_win32.h"
 #else
 #include <stddef.h>
 #include <stdint.h>
@@ -2149,27 +2149,28 @@
     bounds[1] = stop - start;
     return ct;
 }
 
 static PyObject *
 cdata_slice(CDataObject *cd, PySliceObject *slice)
 {
+    char *cdata;
     Py_ssize_t bounds[2];
     CTypeDescrObject *ct = _cdata_getslicearg(cd, slice, bounds);
     if (ct == NULL)
         return NULL;
 
     if (ct->ct_stuff == NULL) {
         ct->ct_stuff = new_array_type(ct, -1);
         if (ct->ct_stuff == NULL)
             return NULL;
     }
     ct = (CTypeDescrObject *)ct->ct_stuff;
 
-    char *cdata = cd->c_data + ct->ct_itemdescr->ct_size * bounds[0];
+    cdata = cd->c_data + ct->ct_itemdescr->ct_size * bounds[0];
     return new_sized_cdata(cdata, ct, bounds[1]);
 }
 
 static int
 cdata_ass_slice(CDataObject *cd, PySliceObject *slice, PyObject *v)
 {
     Py_ssize_t bounds[2], i, length, itemsize;
```

### Comparing `cffi-1.9.0/c/cdlopen.c` & `cffi-1.9.1/c/cdlopen.c`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/malloc_closure.h` & `cffi-1.9.1/c/malloc_closure.h`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/cglob.c` & `cffi-1.9.1/c/cglob.c`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/libffi_msvc/ffitarget.h` & `cffi-1.9.1/c/libffi_msvc/ffitarget.h`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/libffi_msvc/types.c` & `cffi-1.9.1/c/libffi_msvc/types.c`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/libffi_msvc/win32.c` & `cffi-1.9.1/c/libffi_msvc/win32.c`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/libffi_msvc/ffi_common.h` & `cffi-1.9.1/c/libffi_msvc/ffi_common.h`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/libffi_msvc/win64.obj` & `cffi-1.9.1/c/libffi_msvc/win64.obj`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/libffi_msvc/ffi.h` & `cffi-1.9.1/c/libffi_msvc/ffi.h`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/libffi_msvc/prep_cif.c` & `cffi-1.9.1/c/libffi_msvc/prep_cif.c`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/libffi_msvc/win64.asm` & `cffi-1.9.1/c/libffi_msvc/win64.asm`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/libffi_msvc/ffi.c` & `cffi-1.9.1/c/libffi_msvc/ffi.c`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/libffi_msvc/fficonfig.h` & `cffi-1.9.1/c/libffi_msvc/fficonfig.h`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/wchar_helper.h` & `cffi-1.9.1/c/wchar_helper.h`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/misc_thread_common.h` & `cffi-1.9.1/c/misc_thread_common.h`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/misc_thread_posix.h` & `cffi-1.9.1/c/misc_thread_posix.h`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/parse_c_type.c` & `cffi-1.9.1/c/parse_c_type.c`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/misc_win32.h` & `cffi-1.9.1/c/misc_win32.h`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/minibuffer.h` & `cffi-1.9.1/c/minibuffer.h`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/lib_obj.c` & `cffi-1.9.1/c/lib_obj.c`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/commontypes.c` & `cffi-1.9.1/c/commontypes.c`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/call_python.c` & `cffi-1.9.1/c/call_python.c`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/file_emulator.h` & `cffi-1.9.1/c/file_emulator.h`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/test_c.py` & `cffi-1.9.1/c/test_c.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 _setup_path()
 from _cffi_backend import *
 from _cffi_backend import _testfunc, _get_types, _get_common_types, __version__
 
 # ____________________________________________________________
 
 import sys
-assert __version__ == "1.9.0", ("This test_c.py file is for testing a version"
+assert __version__ == "1.9.1", ("This test_c.py file is for testing a version"
                                 " of cffi that differs from the one that we"
                                 " get from 'import _cffi_backend'")
 if sys.version_info < (3,):
     type_or_class = "type"
     mandatory_b_prefix = ''
     mandatory_u_prefix = 'u'
     bytechr = chr
```

### Comparing `cffi-1.9.0/c/ffi_obj.c` & `cffi-1.9.1/c/ffi_obj.c`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/c/cffi1_module.c` & `cffi-1.9.1/c/cffi1_module.c`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/doc/source/cdef.rst` & `cffi-1.9.1/doc/source/cdef.rst`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/doc/source/ref.rst` & `cffi-1.9.1/doc/source/ref.rst`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/doc/source/using.rst` & `cffi-1.9.1/doc/source/using.rst`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/doc/source/index.rst` & `cffi-1.9.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/doc/source/overview.rst` & `cffi-1.9.1/doc/source/overview.rst`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/doc/source/installation.rst` & `cffi-1.9.1/doc/source/installation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 * `py.test`_ is needed to run the tests of CFFI itself.
 
 .. _`py.test`: http://pypi.python.org/pypi/pytest
 
 Download and Installation:
 
-* http://pypi.python.org/packages/source/c/cffi/cffi-1.9.0.tar.gz
+* http://pypi.python.org/packages/source/c/cffi/cffi-1.9.1.tar.gz
 
    - MD5: ...
 
    - SHA: ...
 
    - SHA256: ...
```

### Comparing `cffi-1.9.0/doc/source/conf.py` & `cffi-1.9.1/doc/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '1.9'
 # The full version, including alpha/beta/rc tags.
-release = '1.9.0'
+release = '1.9.1'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `cffi-1.9.0/doc/source/embedding.rst` & `cffi-1.9.1/doc/source/embedding.rst`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/doc/source/whatsnew.rst` & `cffi-1.9.1/doc/source/whatsnew.rst`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/doc/Makefile` & `cffi-1.9.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/doc/misc/design.rst` & `cffi-1.9.1/doc/misc/design.rst`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/doc/misc/grant-cffi-1.0.rst` & `cffi-1.9.1/doc/misc/grant-cffi-1.0.rst`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/doc/misc/parse_c_type.rst` & `cffi-1.9.1/doc/misc/parse_c_type.rst`

 * *Files identical despite different names*

### Comparing `cffi-1.9.0/doc/make.bat` & `cffi-1.9.1/doc/make.bat`

 * *Files identical despite different names*


# Comparing `tmp/structstore-0.1.5.tar.gz` & `tmp/structstore-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structstore-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "structstore-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `structstore-0.1.5.tar` & `structstore-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     4654 2024-05-21 07:26:59.509136 structstore-0.1.5/CMakeLists.txt
--rw-r--r--   0        0        0     1489 2022-11-06 13:29:39.097613 structstore-0.1.5/LICENSE
--rw-r--r--   0        0        0     3879 2024-05-21 06:58:01.634087 structstore-0.1.5/README.md
--rw-r--r--   0        0        0      709 2024-05-14 11:34:33.427123 structstore-0.1.5/cmake/NanobindStubgen.cmake
--rw-r--r--   0        0        0      462 2024-05-14 11:34:33.427123 structstore-0.1.5/cmake/StructStoreConfig.cmake.in
--rw-r--r--   0        0        0      378 2024-05-14 11:34:33.427123 structstore-0.1.5/cmake/StructStoreConfigVersion.cmake.in
--rw-r--r--   0        0        0      385 2024-05-21 06:58:01.634087 structstore-0.1.5/include/structstore/structstore.hpp
--rw-r--r--   0        0        0    13883 2024-05-16 12:14:20.969152 structstore-0.1.5/include/structstore/stst_alloc.hpp
--rw-r--r--   0        0        0     5117 2024-05-21 07:26:43.262447 structstore-0.1.5/include/structstore/stst_containers.hpp
--rw-r--r--   0        0        0     4712 2024-05-21 07:26:43.262447 structstore-0.1.5/include/structstore/stst_field.hpp
--rw-r--r--   0        0        0     1178 2024-05-21 06:57:50.027421 structstore-0.1.5/include/structstore/stst_hashstring.hpp
--rw-r--r--   0        0        0     1578 2024-05-21 06:57:50.027421 structstore-0.1.5/include/structstore/stst_lock.hpp
--rw-r--r--   0        0        0     1255 2024-05-21 06:58:01.634087 structstore-0.1.5/include/structstore/stst_serialization.hpp
--rw-r--r--   0        0        0     4230 2024-05-21 06:57:50.027421 structstore-0.1.5/include/structstore/stst_shared.hpp
--rw-r--r--   0        0        0     5402 2024-05-21 06:58:01.634087 structstore-0.1.5/include/structstore/stst_structstore.hpp
--rw-r--r--   0        0        0     1422 2024-05-14 11:34:33.427123 structstore-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1250 2022-11-18 12:53:02.673000 structstore-0.1.5/src/main.bak.cpp
--rw-r--r--   0        0        0     1355 2022-11-20 10:32:04.499910 structstore-0.1.5/src/main.cpp
--rw-r--r--   0        0        0     1024 2024-05-21 06:58:01.634087 structstore-0.1.5/src/structstore.cpp
--rw-r--r--   0        0        0      246 2024-05-21 07:26:59.519136 structstore-0.1.5/src/structstore/__init__.py
--rw-r--r--   0        0        0    16485 2024-05-21 07:26:43.262447 structstore-0.1.5/src/structstore_bindings.cpp
--rw-r--r--   0        0        0     1069 2024-05-21 07:26:43.262447 structstore-0.1.5/src/structstore_containers.cpp
--rw-r--r--   0        0        0      336 2024-05-21 06:58:01.634087 structstore-0.1.5/src/structstore_field.cpp
--rw-r--r--   0        0        0     2644 2024-05-21 06:58:01.637420 structstore-0.1.5/src/structstore_serialization.cpp
--rw-r--r--   0        0        0     8919 2024-05-21 06:58:01.637420 structstore-0.1.5/src/structstore_shared.cpp
--rw-r--r--   0        0        0     4220 1970-01-01 00:00:00.000000 structstore-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     4654 2024-05-24 08:36:55.614930 structstore-0.1.6/CMakeLists.txt
+-rw-r--r--   0        0        0     1489 2022-11-06 13:29:39.097613 structstore-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3879 2024-05-24 08:35:53.462654 structstore-0.1.6/README.md
+-rw-r--r--   0        0        0      709 2024-05-14 11:34:33.427123 structstore-0.1.6/cmake/NanobindStubgen.cmake
+-rw-r--r--   0        0        0      462 2024-05-14 11:34:33.427123 structstore-0.1.6/cmake/StructStoreConfig.cmake.in
+-rw-r--r--   0        0        0      378 2024-05-14 11:34:33.427123 structstore-0.1.6/cmake/StructStoreConfigVersion.cmake.in
+-rw-r--r--   0        0        0      385 2024-05-24 08:35:53.462654 structstore-0.1.6/include/structstore/structstore.hpp
+-rw-r--r--   0        0        0    13883 2024-05-24 08:35:51.869348 structstore-0.1.6/include/structstore/stst_alloc.hpp
+-rw-r--r--   0        0        0     5117 2024-05-24 08:37:04.284781 structstore-0.1.6/include/structstore/stst_containers.hpp
+-rw-r--r--   0        0        0     4712 2024-05-24 08:35:53.465988 structstore-0.1.6/include/structstore/stst_field.hpp
+-rw-r--r--   0        0        0     1178 2024-05-24 08:35:53.465988 structstore-0.1.6/include/structstore/stst_hashstring.hpp
+-rw-r--r--   0        0        0     1578 2024-05-24 08:35:53.465988 structstore-0.1.6/include/structstore/stst_lock.hpp
+-rw-r--r--   0        0        0     1255 2024-05-24 08:35:53.465988 structstore-0.1.6/include/structstore/stst_serialization.hpp
+-rw-r--r--   0        0        0     4230 2024-05-24 08:35:53.465988 structstore-0.1.6/include/structstore/stst_shared.hpp
+-rw-r--r--   0        0        0     5402 2024-05-24 08:35:53.465988 structstore-0.1.6/include/structstore/stst_structstore.hpp
+-rw-r--r--   0        0        0     1422 2024-05-24 08:38:19.676815 structstore-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1250 2022-11-18 12:53:02.673000 structstore-0.1.6/src/main.bak.cpp
+-rw-r--r--   0        0        0     1355 2022-11-20 10:32:04.499910 structstore-0.1.6/src/main.cpp
+-rw-r--r--   0        0        0     1024 2024-05-24 08:35:53.465988 structstore-0.1.6/src/structstore.cpp
+-rw-r--r--   0        0        0      246 2024-05-24 08:36:55.608263 structstore-0.1.6/src/structstore/__init__.py
+-rw-r--r--   0        0        0    16485 2024-05-24 08:35:53.465988 structstore-0.1.6/src/structstore_bindings.cpp
+-rw-r--r--   0        0        0     1069 2024-05-24 08:35:53.465988 structstore-0.1.6/src/structstore_containers.cpp
+-rw-r--r--   0        0        0      336 2024-05-24 08:35:53.465988 structstore-0.1.6/src/structstore_field.cpp
+-rw-r--r--   0        0        0     2644 2024-05-24 08:35:53.465988 structstore-0.1.6/src/structstore_serialization.cpp
+-rw-r--r--   0        0        0     8919 2024-05-24 08:35:53.465988 structstore-0.1.6/src/structstore_shared.cpp
+-rw-r--r--   0        0        0     4220 1970-01-01 00:00:00.000000 structstore-0.1.6/PKG-INFO
```

### Comparing `structstore-0.1.5/CMakeLists.txt` & `structstore-0.1.6/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 cmake_minimum_required(VERSION 3.10)
-project(structstore VERSION 0.1.5)
+project(structstore VERSION 0.1.6)
 
 set(PY_VERSION_SUFFIX "")
 set(PY_FULL_VERSION ${PROJECT_VERSION}${PY_VERSION_SUFFIX})
 
 # make sure that the Python and CMake versions match
 if (DEFINED PY_BUILD_CMAKE_PACKAGE_VERSION)
     if (NOT "${PY_BUILD_CMAKE_PACKAGE_VERSION}" MATCHES "^${PY_FULL_VERSION}$")
```

### Comparing `structstore-0.1.5/LICENSE` & `structstore-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `structstore-0.1.5/README.md` & `structstore-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `structstore-0.1.5/cmake/NanobindStubgen.cmake` & `structstore-0.1.6/cmake/NanobindStubgen.cmake`

 * *Files identical despite different names*

### Comparing `structstore-0.1.5/include/structstore/stst_alloc.hpp` & `structstore-0.1.6/include/structstore/stst_alloc.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.5/include/structstore/stst_containers.hpp` & `structstore-0.1.6/include/structstore/stst_containers.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 };
 
 template<>
 void List::push_back<const char*>(const char* const& value);
 
 class Matrix {
 public:
-    static constexpr int MAX_DIMS = 4;
+    static constexpr int MAX_DIMS = 8;
 
 protected:
     MiniMalloc& mm_alloc;
     size_t _ndim;
     size_t _shape[MAX_DIMS] = {};
     double* _data;
```

### Comparing `structstore-0.1.5/include/structstore/stst_field.hpp` & `structstore-0.1.6/include/structstore/stst_field.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.5/include/structstore/stst_hashstring.hpp` & `structstore-0.1.6/include/structstore/stst_hashstring.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.5/include/structstore/stst_lock.hpp` & `structstore-0.1.6/include/structstore/stst_lock.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.5/include/structstore/stst_serialization.hpp` & `structstore-0.1.6/include/structstore/stst_serialization.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.5/include/structstore/stst_shared.hpp` & `structstore-0.1.6/include/structstore/stst_shared.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.5/include/structstore/stst_structstore.hpp` & `structstore-0.1.6/include/structstore/stst_structstore.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.5/pyproject.toml` & `structstore-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `structstore-0.1.5/src/main.bak.cpp` & `structstore-0.1.6/src/main.bak.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.5/src/main.cpp` & `structstore-0.1.6/src/main.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.5/src/structstore.cpp` & `structstore-0.1.6/src/structstore.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.5/src/structstore_bindings.cpp` & `structstore-0.1.6/src/structstore_bindings.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.5/src/structstore_containers.cpp` & `structstore-0.1.6/src/structstore_containers.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.5/src/structstore_serialization.cpp` & `structstore-0.1.6/src/structstore_serialization.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.5/src/structstore_shared.cpp` & `structstore-0.1.6/src/structstore_shared.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.5/PKG-INFO` & `structstore-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structstore
-Version: 0.1.5
+Version: 0.1.6
 Summary: Structured object storage, dynamically typed, to be shared between processes
 Author-email: Max Mertens <max.mail@dameweb.de>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: nanobind
 Project-URL: Homepage, https://github.com/mertemba/structstore
```


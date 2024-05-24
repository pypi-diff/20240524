# Comparing `tmp/little_atf_programmer-2024.1008.tar.gz` & `tmp/little_atf_programmer-2024.1010.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "little_atf_programmer-2024.1008.tar", last modified: Sat Apr 27 22:16:46 2024, max compression
+gzip compressed data, was "little_atf_programmer-2024.1010.tar", last modified: Fri May 24 21:35:32 2024, max compression
```

## Comparing `little_atf_programmer-2024.1008.tar` & `little_atf_programmer-2024.1010.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:16:46.510581 little_atf_programmer-2024.1008/
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    12452 2024-04-27 22:16:46.510581 little_atf_programmer-2024.1008/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:16:46.510581 little_atf_programmer-2024.1008/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:16:46.502581 little_atf_programmer-2024.1008/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:16:46.502581 little_atf_programmer-2024.1008/src/atfu/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:16:46.502581 little_atf_programmer-2024.1008/src/atfu/converter/
--rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu/converter/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu/converter/fuseconv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu/converter/jed2svf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu/converter/jesd3.py
--rw-r--r--   0 runner    (1001) docker     (127)    31099 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu/converter/svf2xsvf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu/converter/svfeventhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu/erase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:16:46.502581 little_atf_programmer-2024.1008/src/atfu/little_board/
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu/little_board/jtag_programmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu/program.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu/programmer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:16:46.506581 little_atf_programmer-2024.1008/src/atfu/standard_vectors/
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu/standard_vectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27936 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu/standard_vectors/bc1502.xsvf
--rw-r--r--   0 runner    (1001) docker     (127)    34858 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu/standard_vectors/bc1504.xsvf
--rw-r--r--   0 runner    (1001) docker     (127)    51652 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu/standard_vectors/bc1508.xsvf
--rw-r--r--   0 runner    (1001) docker     (127)    27916 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu/standard_vectors/e1502.xsvf
--rw-r--r--   0 runner    (1001) docker     (127)    34838 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu/standard_vectors/e1504.xsvf
--rw-r--r--   0 runner    (1001) docker     (127)    51632 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu/standard_vectors/e1508.xsvf
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-27 22:16:29.000000 little_atf_programmer-2024.1008/src/atfu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:16:46.506581 little_atf_programmer-2024.1008/src/little_atf_programmer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12452 2024-04-27 22:16:46.000000 little_atf_programmer-2024.1008/src/little_atf_programmer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-27 22:16:46.000000 little_atf_programmer-2024.1008/src/little_atf_programmer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:16:46.000000 little_atf_programmer-2024.1008/src/little_atf_programmer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-27 22:16:46.000000 little_atf_programmer-2024.1008/src/little_atf_programmer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-27 22:16:46.000000 little_atf_programmer-2024.1008/src/little_atf_programmer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-27 22:16:46.000000 little_atf_programmer-2024.1008/src/little_atf_programmer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:35:32.173519 little_atf_programmer-2024.1010/
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12451 2024-05-24 21:35:32.173519 little_atf_programmer-2024.1010/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 21:35:32.173519 little_atf_programmer-2024.1010/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:35:32.169519 little_atf_programmer-2024.1010/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:35:32.169519 little_atf_programmer-2024.1010/src/atfu/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:35:32.169519 little_atf_programmer-2024.1010/src/atfu/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu/converter/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu/converter/fuseconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu/converter/jed2svf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu/converter/jesd3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31144 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu/converter/svf2xsvf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu/converter/svfeventhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu/erase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:35:32.169519 little_atf_programmer-2024.1010/src/atfu/little_board/
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu/little_board/jtag_programmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu/programmer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:35:32.173519 little_atf_programmer-2024.1010/src/atfu/standard_vectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu/standard_vectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27936 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu/standard_vectors/bc1502.xsvf
+-rw-r--r--   0 runner    (1001) docker     (127)    34858 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu/standard_vectors/bc1504.xsvf
+-rw-r--r--   0 runner    (1001) docker     (127)    51652 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu/standard_vectors/bc1508.xsvf
+-rw-r--r--   0 runner    (1001) docker     (127)    27916 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu/standard_vectors/e1502.xsvf
+-rw-r--r--   0 runner    (1001) docker     (127)    34838 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu/standard_vectors/e1504.xsvf
+-rw-r--r--   0 runner    (1001) docker     (127)    51632 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu/standard_vectors/e1508.xsvf
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-24 21:35:15.000000 little_atf_programmer-2024.1010/src/atfu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:35:32.173519 little_atf_programmer-2024.1010/src/little_atf_programmer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12451 2024-05-24 21:35:32.000000 little_atf_programmer-2024.1010/src/little_atf_programmer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-24 21:35:32.000000 little_atf_programmer-2024.1010/src/little_atf_programmer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 21:35:32.000000 little_atf_programmer-2024.1010/src/little_atf_programmer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-24 21:35:32.000000 little_atf_programmer-2024.1010/src/little_atf_programmer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-24 21:35:32.000000 little_atf_programmer-2024.1010/src/little_atf_programmer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-24 21:35:32.000000 little_atf_programmer-2024.1010/src/little_atf_programmer.egg-info/top_level.txt
```

### Comparing `little_atf_programmer-2024.1008/LICENSE.md` & `little_atf_programmer-2024.1010/LICENSE.md`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1008/PKG-INFO` & `little_atf_programmer-2024.1010/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: little-atf-programmer
-Version: 2024.1008
+Version: 2024.1010
 Summary: Little ATF150x Programmer Board utility programs
 Author-email: The Really Old-School Company Limited <info@rosco-m68k.com>
 License: Copyright (c) 2024 The Really Old-School Company Limited
         
         Permission is hereby granted, free of charge, to any person obtaining 
         a copy of this software and associated documentation files (the "Software"),
         to deal in the Software without restriction, including without limitation 
@@ -100,15 +100,15 @@
         
         
 Project-URL: Homepage, https://github.com/roscopeco/atfprog-tools
 Keywords: cpld,atf1502,atf1504,atf1508,logic,programmer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: pyserial==3.5
 Requires-Dist: pyparsing==3.1.2
 Requires-Dist: bitarray==2.9.2
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: progress==1.6
```

### Comparing `little_atf_programmer-2024.1008/README.md` & `little_atf_programmer-2024.1010/README.md`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1008/pyproject.toml` & `little_atf_programmer-2024.1010/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "little-atf-programmer"
-version = "2024.1008"
+version = "2024.1010"
 description = "Little ATF150x Programmer Board utility programs"
 readme = "README.md"
 authors = [{ name = "The Really Old-School Company Limited", email = "info@rosco-m68k.com" }]
 license = { file = "LICENSE.md" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -19,30 +19,30 @@
     "pyserial==3.5",
     "pyparsing==3.1.2",
     "bitarray==2.9.2",
     "tabulate==0.9.0",
     "progress==1.6",
     "tqdm==4.66.2",
 ]
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "pre-commit", "isort", "pip-tools", "pytest", "sure", "httpretty"]
 
 [project.scripts]
 atfu = "atfu.command:main"
 
 [project.urls]
 Homepage = "https://github.com/roscopeco/atfprog-tools"
 
 [tool.setuptools.package-data]
 "atfu.standard_vectors" = ["*.xsvf"]
 
 [tool.bumpver]
-current_version = "2024.1008"
+current_version = "2024.1010"
 version_pattern = "YYYY.BUILD[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = true
@@ -66,8 +66,8 @@
       | dist
     )/
     '''
 
 [tool.pytest.ini_options]
 pythonpath = [
   "src"
-]
+]
```

### Comparing `little_atf_programmer-2024.1008/src/atfu/check.py` & `little_atf_programmer-2024.1010/src/atfu/check.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1008/src/atfu/command.py` & `little_atf_programmer-2024.1010/src/atfu/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import atfu.program
 import atfu.erase
 import atfu.check
 import atfu.programmer
 
 BOARDNAME = "Little ATF150x Programmer Board"
 PROGNAME = f"{BOARDNAME} Utility"
-VERSION = "2024.1008"
+VERSION = "2024.1010"
 
 
 def main():
     args = _arg_parser().parse_args()
     args.func(args)
```

### Comparing `little_atf_programmer-2024.1008/src/atfu/converter/device.py` & `little_atf_programmer-2024.1010/src/atfu/converter/device.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1008/src/atfu/converter/fuseconv.py` & `little_atf_programmer-2024.1010/src/atfu/converter/fuseconv.py`

 * *Files 10% similar despite different names*

```diff
@@ -108,39 +108,45 @@
     def emit_program(address, data):
         file.write("// ISC program word\n")
         file.write("SIR 10 TDI ({:03x});\n".format(ATF15xxInstr.ISC_ADDRESS))
         file.write("SDR 11 TDI ({:03x});\n".format(address))
         file.write(
             "SIR 10 TDI ({:03x});\n".format(ATF15xxInstr.ISC_DATA | (address >> 8))
         )
-        file.write(
-            "SDR {} TDI ({:0{}x});\n".format(
-                len(data), int(data.to01()[::-1], 2), len(data) // 4
-            )
-        )
+
+        # TODO this is a bit of a hack...
+        hexout = "{:0{}x}".format(int(data.to01()[::-1], 2), len(data) // 4)
+        if (len(data) // 4) & 0x1:
+            hexout = "0" + hexout
+
+        file.write("SDR {} TDI ({});\n".format(len(data), hexout))
         file.write("SIR 10 TDI ({:03x});\n".format(ATF15xxInstr.ISC_PROGRAM_ERASE))
         file.write("RUNTEST IDLE 30E-3 SEC;\n")
         emit_unknown()
 
     def emit_verify(address, data):
         file.write("// ISC verify word\n")
         file.write("SIR 10 TDI ({:03x});\n".format(ATF15xxInstr.ISC_ADDRESS))
         file.write("SDR 11 TDI ({:03x});\n".format(address))
         file.write("SIR 10 TDI ({:03x});\n".format(ATF15xxInstr.ISC_READ))
         file.write("RUNTEST IDLE 20E-3 SEC;\n")
         file.write(
             "SIR 10 TDI ({:03x});\n".format(ATF15xxInstr.ISC_DATA | (address >> 8))
         )
+
+        # TODO this is the same hack as above...
+        hexout = "{:0{}x}".format(int(data.to01()[::-1], 2), len(data) // 4)
+        if (len(data) // 4) & 0x1:
+            hexout = "0" + hexout
+
         file.write(
-            "SDR {} TDI ({:0{}x})\n\tTDO ({:0{}x})\n\tMASK ({:0{}x});\n".format(
+            "SDR {} TDI ({})\n\tTDO ({})\n\tMASK ({:0{}x});\n".format(
                 len(data),
-                int(data.to01()[::-1], 2),
-                len(data) // 4,
-                int(data.to01()[::-1], 2),
-                len(data) // 4,
+                hexout,
+                hexout,
                 (1 << len(data)) - 1,
                 len(data) // 4,
             )
         )
 
     emit_header()
     emit_check_idcode(device.idcode)
```

### Comparing `little_atf_programmer-2024.1008/src/atfu/converter/jed2svf.py` & `little_atf_programmer-2024.1010/src/atfu/converter/jed2svf.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1008/src/atfu/converter/jesd3.py` & `little_atf_programmer-2024.1010/src/atfu/converter/jesd3.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1008/src/atfu/converter/svf2xsvf.py` & `little_atf_programmer-2024.1010/src/atfu/converter/svf2xsvf.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,16 @@
 # doCOMMENTs = True  # Save XCOMMENTs in the output xsvf file
 doCOMMENTs = False  # Save XCOMMENTs in the output xsvf file
 
 # pick your file encoding
 # file_encoding = "ISO-8859-1"
 file_encoding = "utf-8"
 
+tokLn = 0
+inputFilename = ""
 
 xrepeat = 0  # argument to XREPEAT, gives retry count for masked compares
 
 
 # -----< Lexer >---------------------------------------------------------------
 
 StateBin = (
@@ -435,15 +437,15 @@
     tokens = scanner.scan(input)[0]
 
     input = None  # allow gc to reclaim memory holding file
 
     # for tokenType, tokenValue, ln in tokens: print( "line %d: %s" % (ln, tokenType), tokenValue )
 
     # -----<parser>-----------------------------------------------------------------
-
+    global tokLn
     tokVal = tokType = tokLn = None
 
     tup = iter(tokens)
 
     # one of the commands that take the shiftParts after the length, the parse
     # template for all of these commands is identical
     shiftOps = ("SDR", "SIR", "LSDR", "HDR", "HIR", "TDR", "TIR")
```

### Comparing `little_atf_programmer-2024.1008/src/atfu/converter/svfeventhandler.py` & `little_atf_programmer-2024.1010/src/atfu/converter/svfeventhandler.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1008/src/atfu/erase.py` & `little_atf_programmer-2024.1010/src/atfu/erase.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1008/src/atfu/little_board/jtag_programmer.py` & `little_atf_programmer-2024.1010/src/atfu/little_board/jtag_programmer.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1008/src/atfu/output.py` & `little_atf_programmer-2024.1010/src/atfu/output.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1008/src/atfu/program.py` & `little_atf_programmer-2024.1010/src/atfu/program.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1008/src/atfu/programmer.py` & `little_atf_programmer-2024.1010/src/atfu/programmer.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1008/src/atfu/standard_vectors/__init__.py` & `little_atf_programmer-2024.1010/src/atfu/standard_vectors/__init__.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1008/src/atfu/standard_vectors/bc1502.xsvf` & `little_atf_programmer-2024.1010/src/atfu/standard_vectors/bc1502.xsvf`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1008/src/atfu/standard_vectors/bc1504.xsvf` & `little_atf_programmer-2024.1010/src/atfu/standard_vectors/bc1504.xsvf`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1008/src/atfu/standard_vectors/bc1508.xsvf` & `little_atf_programmer-2024.1010/src/atfu/standard_vectors/bc1508.xsvf`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1008/src/atfu/standard_vectors/e1502.xsvf` & `little_atf_programmer-2024.1010/src/atfu/standard_vectors/e1502.xsvf`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1008/src/atfu/standard_vectors/e1504.xsvf` & `little_atf_programmer-2024.1010/src/atfu/standard_vectors/e1504.xsvf`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1008/src/atfu/standard_vectors/e1508.xsvf` & `little_atf_programmer-2024.1010/src/atfu/standard_vectors/e1508.xsvf`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1008/src/little_atf_programmer.egg-info/PKG-INFO` & `little_atf_programmer-2024.1010/src/little_atf_programmer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: little-atf-programmer
-Version: 2024.1008
+Version: 2024.1010
 Summary: Little ATF150x Programmer Board utility programs
 Author-email: The Really Old-School Company Limited <info@rosco-m68k.com>
 License: Copyright (c) 2024 The Really Old-School Company Limited
         
         Permission is hereby granted, free of charge, to any person obtaining 
         a copy of this software and associated documentation files (the "Software"),
         to deal in the Software without restriction, including without limitation 
@@ -100,15 +100,15 @@
         
         
 Project-URL: Homepage, https://github.com/roscopeco/atfprog-tools
 Keywords: cpld,atf1502,atf1504,atf1508,logic,programmer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: pyserial==3.5
 Requires-Dist: pyparsing==3.1.2
 Requires-Dist: bitarray==2.9.2
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: progress==1.6
```

### Comparing `little_atf_programmer-2024.1008/src/little_atf_programmer.egg-info/SOURCES.txt` & `little_atf_programmer-2024.1010/src/little_atf_programmer.egg-info/SOURCES.txt`

 * *Files identical despite different names*


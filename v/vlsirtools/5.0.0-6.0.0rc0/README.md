# Comparing `tmp/vlsirtools-5.0.0.tar.gz` & `tmp/vlsirtools-6.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlsirtools-5.0.0.tar", last modified: Tue Nov 14 18:39:55 2023, max compression
+gzip compressed data, was "vlsirtools-6.0.0rc0.tar", last modified: Fri May 24 16:31:51 2024, max compression
```

## Comparing `vlsirtools-5.0.0.tar` & `vlsirtools-6.0.0rc0.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:39:55.898109 vlsirtools-5.0.0/
--rw-r--r--   0 dan        (501) staff       (20)     2772 2023-06-26 21:21:08.000000 vlsirtools-5.0.0/.gitignore
--rw-r--r--   0 dan        (501) staff       (20)     1521 2023-06-26 21:21:08.000000 vlsirtools-5.0.0/LICENSE
--rw-r--r--   0 dan        (501) staff       (20)     2673 2023-11-14 18:39:55.897933 vlsirtools-5.0.0/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)     2368 2023-06-26 21:21:08.000000 vlsirtools-5.0.0/readme.md
--rw-r--r--   0 dan        (501) staff       (20)       38 2023-11-14 18:39:55.898167 vlsirtools-5.0.0/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)     1149 2023-11-14 18:32:13.000000 vlsirtools-5.0.0/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:39:55.893154 vlsirtools-5.0.0/tests/
--rw-r--r--   0 dan        (501) staff       (20)        0 2022-06-13 20:36:42.000000 vlsirtools-5.0.0/tests/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     3790 2023-06-28 18:09:23.000000 vlsirtools-5.0.0/tests/test_primitives.py
--rw-r--r--   0 dan        (501) staff       (20)    21806 2023-08-30 20:52:59.000000 vlsirtools-5.0.0/tests/test_vlsirtools.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:39:55.893875 vlsirtools-5.0.0/vlsirtools/
--rw-r--r--   0 dan        (501) staff       (20)      596 2023-06-26 21:21:08.000000 vlsirtools-5.0.0/vlsirtools/__init__.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:39:55.895885 vlsirtools-5.0.0/vlsirtools/netlist/
--rw-r--r--   0 dan        (501) staff       (20)     3571 2023-06-26 21:21:08.000000 vlsirtools-5.0.0/vlsirtools/netlist/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)    31961 2023-08-30 20:52:59.000000 vlsirtools-5.0.0/vlsirtools/netlist/base.py
--rw-r--r--   0 dan        (501) staff       (20)    14534 2023-06-28 18:09:27.000000 vlsirtools-5.0.0/vlsirtools/netlist/spectre.py
--rw-r--r--   0 dan        (501) staff       (20)     2112 2023-06-26 21:21:08.000000 vlsirtools-5.0.0/vlsirtools/netlist/spectre_spice_shared.py
--rw-r--r--   0 dan        (501) staff       (20)    26453 2023-08-30 20:52:59.000000 vlsirtools-5.0.0/vlsirtools/netlist/spice.py
--rw-r--r--   0 dan        (501) staff       (20)    10660 2023-06-28 18:09:27.000000 vlsirtools-5.0.0/vlsirtools/netlist/verilog.py
--rw-r--r--   0 dan        (501) staff       (20)    16643 2023-08-30 20:52:59.000000 vlsirtools-5.0.0/vlsirtools/primitives.py
--rw-r--r--   0 dan        (501) staff       (20)     6456 2023-06-26 21:21:08.000000 vlsirtools-5.0.0/vlsirtools/pytest.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:39:55.896062 vlsirtools-5.0.0/vlsirtools/spectre/
--rw-r--r--   0 dan        (501) staff       (20)      122 2023-06-26 21:21:08.000000 vlsirtools-5.0.0/vlsirtools/spectre/__init__.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:39:55.897394 vlsirtools-5.0.0/vlsirtools/spice/
--rw-r--r--   0 dan        (501) staff       (20)       84 2023-06-26 21:21:08.000000 vlsirtools-5.0.0/vlsirtools/spice/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     5453 2023-11-14 18:31:14.000000 vlsirtools-5.0.0/vlsirtools/spice/base.py
--rw-r--r--   0 dan        (501) staff       (20)    12654 2023-06-26 21:21:08.000000 vlsirtools-5.0.0/vlsirtools/spice/ngspice.py
--rw-r--r--   0 dan        (501) staff       (20)     7030 2023-06-26 21:21:08.000000 vlsirtools-5.0.0/vlsirtools/spice/sim_data.py
--rw-r--r--   0 dan        (501) staff       (20)    11233 2023-11-14 18:31:14.000000 vlsirtools-5.0.0/vlsirtools/spice/spectre.py
--rw-r--r--   0 dan        (501) staff       (20)     5711 2023-11-14 18:31:14.000000 vlsirtools-5.0.0/vlsirtools/spice/spice.py
--rw-r--r--   0 dan        (501) staff       (20)    14053 2023-06-26 21:21:08.000000 vlsirtools-5.0.0/vlsirtools/spice/xyce.py
--rw-r--r--   0 dan        (501) staff       (20)     3459 2023-06-26 21:21:08.000000 vlsirtools-5.0.0/vlsirtools/spicetype.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:39:55.897723 vlsirtools-5.0.0/vlsirtools/xyce/
--rw-r--r--   0 dan        (501) staff       (20)      113 2023-06-26 21:21:08.000000 vlsirtools-5.0.0/vlsirtools/xyce/__init__.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:39:55.894674 vlsirtools-5.0.0/vlsirtools.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)     2673 2023-11-14 18:39:55.000000 vlsirtools-5.0.0/vlsirtools.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      805 2023-11-14 18:39:55.000000 vlsirtools-5.0.0/vlsirtools.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-11-14 18:39:55.000000 vlsirtools-5.0.0/vlsirtools.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)       94 2023-11-14 18:39:55.000000 vlsirtools-5.0.0/vlsirtools.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       17 2023-11-14 18:39:55.000000 vlsirtools-5.0.0/vlsirtools.egg-info/top_level.txt
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 16:31:51.354662 vlsirtools-6.0.0rc0/
+-rw-r--r--   0 dan        (501) staff       (20)     2772 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/.gitignore
+-rw-r--r--   0 dan        (501) staff       (20)     1521 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/LICENSE
+-rw-r--r--   0 dan        (501) staff       (20)     2676 2024-05-24 16:31:51.354413 vlsirtools-6.0.0rc0/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)     2368 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/readme.md
+-rw-r--r--   0 dan        (501) staff       (20)       38 2024-05-24 16:31:51.354719 vlsirtools-6.0.0rc0/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)     1149 2024-05-24 16:25:05.000000 vlsirtools-6.0.0rc0/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 16:31:51.345793 vlsirtools-6.0.0rc0/tests/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2022-06-13 20:36:42.000000 vlsirtools-6.0.0rc0/tests/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)      807 2024-05-24 16:07:55.000000 vlsirtools-6.0.0rc0/tests/test_netlist.py
+-rw-r--r--   0 dan        (501) staff       (20)     3790 2023-06-28 18:09:23.000000 vlsirtools-6.0.0rc0/tests/test_primitives.py
+-rw-r--r--   0 dan        (501) staff       (20)    21823 2024-05-24 16:27:03.000000 vlsirtools-6.0.0rc0/tests/test_vlsirtools.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 16:31:51.347183 vlsirtools-6.0.0rc0/vlsirtools/
+-rw-r--r--   0 dan        (501) staff       (20)      613 2024-05-24 16:27:15.000000 vlsirtools-6.0.0rc0/vlsirtools/__init__.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 16:31:51.350625 vlsirtools-6.0.0rc0/vlsirtools/netlist/
+-rw-r--r--   0 dan        (501) staff       (20)      428 2024-05-24 16:07:55.000000 vlsirtools-6.0.0rc0/vlsirtools/netlist/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)    31961 2023-08-30 20:52:59.000000 vlsirtools-6.0.0rc0/vlsirtools/netlist/base.py
+-rw-r--r--   0 dan        (501) staff       (20)     3283 2024-05-24 16:07:55.000000 vlsirtools-6.0.0rc0/vlsirtools/netlist/fmt.py
+-rw-r--r--   0 dan        (501) staff       (20)     2460 2024-05-24 16:07:55.000000 vlsirtools-6.0.0rc0/vlsirtools/netlist/main.py
+-rw-r--r--   0 dan        (501) staff       (20)    14534 2023-06-28 18:09:27.000000 vlsirtools-6.0.0rc0/vlsirtools/netlist/spectre.py
+-rw-r--r--   0 dan        (501) staff       (20)     2112 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/vlsirtools/netlist/spectre_spice_shared.py
+-rw-r--r--   0 dan        (501) staff       (20)    26453 2023-08-30 20:52:59.000000 vlsirtools-6.0.0rc0/vlsirtools/netlist/spice.py
+-rw-r--r--   0 dan        (501) staff       (20)    10660 2023-06-28 18:09:27.000000 vlsirtools-6.0.0rc0/vlsirtools/netlist/verilog.py
+-rw-r--r--   0 dan        (501) staff       (20)    16643 2023-08-30 20:52:59.000000 vlsirtools-6.0.0rc0/vlsirtools/primitives.py
+-rw-r--r--   0 dan        (501) staff       (20)     6456 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/vlsirtools/pytest.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 16:31:51.351187 vlsirtools-6.0.0rc0/vlsirtools/spectre/
+-rw-r--r--   0 dan        (501) staff       (20)      122 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/vlsirtools/spectre/__init__.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 16:31:51.353351 vlsirtools-6.0.0rc0/vlsirtools/spice/
+-rw-r--r--   0 dan        (501) staff       (20)       84 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/vlsirtools/spice/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     5453 2023-11-14 18:31:14.000000 vlsirtools-6.0.0rc0/vlsirtools/spice/base.py
+-rw-r--r--   0 dan        (501) staff       (20)    12654 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/vlsirtools/spice/ngspice.py
+-rw-r--r--   0 dan        (501) staff       (20)     7030 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/vlsirtools/spice/sim_data.py
+-rw-r--r--   0 dan        (501) staff       (20)    11233 2023-11-14 18:31:14.000000 vlsirtools-6.0.0rc0/vlsirtools/spice/spectre.py
+-rw-r--r--   0 dan        (501) staff       (20)     5711 2023-11-14 18:31:14.000000 vlsirtools-6.0.0rc0/vlsirtools/spice/spice.py
+-rw-r--r--   0 dan        (501) staff       (20)    14053 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/vlsirtools/spice/xyce.py
+-rw-r--r--   0 dan        (501) staff       (20)     3459 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/vlsirtools/spicetype.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 16:31:51.353909 vlsirtools-6.0.0rc0/vlsirtools/xyce/
+-rw-r--r--   0 dan        (501) staff       (20)      113 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/vlsirtools/xyce/__init__.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 16:31:51.348291 vlsirtools-6.0.0rc0/vlsirtools.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)     2676 2024-05-24 16:31:51.000000 vlsirtools-6.0.0rc0/vlsirtools.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      880 2024-05-24 16:31:51.000000 vlsirtools-6.0.0rc0/vlsirtools.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-24 16:31:51.000000 vlsirtools-6.0.0rc0/vlsirtools.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)       97 2024-05-24 16:31:51.000000 vlsirtools-6.0.0rc0/vlsirtools.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       17 2024-05-24 16:31:51.000000 vlsirtools-6.0.0rc0/vlsirtools.egg-info/top_level.txt
```

### Comparing `vlsirtools-5.0.0/.gitignore` & `vlsirtools-6.0.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `vlsirtools-5.0.0/LICENSE` & `vlsirtools-6.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `vlsirtools-5.0.0/PKG-INFO` & `vlsirtools-6.0.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlsirtools
-Version: 5.0.0
+Version: 6.0.0rc0
 Summary: Tools for the Vlsir IC Design Schema
 Home-page: https://github.com/Vlsir/Vlsir
 Author: Dan Fritchman
 Author-email: dan@fritch.mn
 Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `vlsirtools-5.0.0/readme.md` & `vlsirtools-6.0.0rc0/readme.md`

 * *Files identical despite different names*

### Comparing `vlsirtools-5.0.0/setup.py` & `vlsirtools-6.0.0rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 import pathlib
 
 # Get the long description from the README file
 here = pathlib.Path(__file__).parent.resolve()
 readme = here / "readme.md"
 long_description = "" if not readme.exists() else readme.read_text(encoding="utf-8")
 
-_VLSIR_VERSION = "5.0.0"
+VLSIR_VERSION = "6.0.0rc0"
 
 setup(
     name="vlsirtools",
-    version=_VLSIR_VERSION,
+    version=VLSIR_VERSION,
     description="Tools for the Vlsir IC Design Schema",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Vlsir/Vlsir",
     author="Dan Fritchman",
     author_email="dan@fritch.mn",
     packages=find_packages(),
     python_requires=">=3.7, <3.12",
     install_requires=[
-        f"vlsir=={_VLSIR_VERSION}",  # VLSIR Core Python Bindings
+        f"vlsir=={VLSIR_VERSION}",  # VLSIR Core Python Bindings
         "numpy~=1.21",  # For `sim_data` simulation results
         "pandas~=1.3",  # For CSV reading
     ],
     extras_require={
         "dev": ["pytest==7.1", "coverage", "pytest-cov", "black==22.6", "twine"]
     },
 )
```

### Comparing `vlsirtools-5.0.0/tests/test_primitives.py` & `vlsirtools-6.0.0rc0/tests/test_primitives.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-5.0.0/tests/test_vlsirtools.py` & `vlsirtools-6.0.0rc0/tests/test_vlsirtools.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 def _prim(name: str) -> Reference:
     """Create a `Reference` to primitive `name`"""
     return Reference(external=QualifiedName(domain="vlsir.primitives", name=name))
 
 
 def test_version():
-    assert vlsirtools.__version__ == "2.0.dev0"
+    assert vlsirtools.__version__ == "6.0.0rc0"  # VLSIR_VERSION
 
 
 def test_verilog_netlist1():
     """Test netlisting to a handful of formats, including Verilog-compatible contents."""
 
     # "Verilog Compatibility" requires:
     # * All ports must be directed. No "NONE" directions.
```

### Comparing `vlsirtools-5.0.0/vlsirtools/__init__.py` & `vlsirtools-6.0.0rc0/vlsirtools/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 # Vlsir Tools
 """
 
-__version__ = "2.0.dev0"
+__version__ = "6.0.0rc0"  # VLSIR_VERSION
 
 # Python module namespaces
 from . import spice
 from . import spicetype
 from .spicetype import SpiceType
 
 # Primitive Definitions
```

### Comparing `vlsirtools-5.0.0/vlsirtools/netlist/__init__.py` & `vlsirtools-6.0.0rc0/vlsirtools/netlist/fmt.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """ 
-# Vlsir Netlisting 
-
-Exports `vlsir.circuit.Package` to a netlist format.
+# Netlist Formats
 """
 
 # Std-Lib Imports
-from typing import Union, IO, Optional
 from enum import Enum
-from dataclasses import dataclass
+from typing import Union
 
 # Local Imports
 import vlsir
 
 # Locally-defined netlister classes
 from .spectre import SpectreNetlister
 from .verilog import VerilogNetlister
@@ -37,15 +34,16 @@
     XYCE = "xyce"
     HSPICE = "hspice"
     CDL = "cdl"
 
     @staticmethod
     def get(spec: "NetlistFormatSpec") -> "NetlistFormat":
         """Get the format specified by `spec`, in either enum or string terms.
-        Only does real work in the case when `spec` is a string, otherwise returns it unchanged."""
+        Only does real work in the case when `spec` is a string, otherwise returns it unchanged.
+        """
         if isinstance(spec, (NetlistFormat, str)):
             return NetlistFormat(spec)
         raise TypeError
 
     def netlister(self) -> type:
         """Get the paired netlister-class"""
         if self == NetlistFormat.SPECTRE:
@@ -58,71 +56,51 @@
             return HspiceNetlister
         if self == NetlistFormat.NGSPICE:
             return NgspiceNetlister
         if self == NetlistFormat.XYCE:
             return XyceNetlister
         if self == NetlistFormat.CDL:
             return CdlNetlister
-        raise ValueError
-
+        raise ValueError(f"Unknown NetlistFormat: {self}")
 
-@dataclass
-class NetlistOptions:
-    """Options for netlisting."""
+    def to_proto(self) -> vlsir.netlist.NetlistFormat:
+        """Convert a `NetlistFormat` to a protobuf `NetlistFormat`."""
+        F = vlsir.netlist.NetlistFormat
+        if self == NetlistFormat.SPECTRE:
+            return F.SPECTRE
+        if self == NetlistFormat.SPICE:
+            return F.SPICE
+        if self == NetlistFormat.NGSPICE:
+            return F.NGSPICE
+        if self == NetlistFormat.XYCE:
+            return F.XYCE
+        if self == NetlistFormat.HSPICE:
+            return F.HSPICE
+        if self == NetlistFormat.CDL:
+            return F.CDL
+        if self == NetlistFormat.VERILOG:
+            return F.VERILOG
+        raise ValueError(f"Unknown NetlistFormat: {self}")
 
-    indent: str = 2 * " "  # Indentation. Defaults to two spaces.
-    width: int = 80  # Line-width. Defaults to 80.
+    @staticmethod
+    def from_proto(proto: vlsir.netlist.NetlistFormat) -> "NetlistFormat":
+        """Convert a protobuf `NetlistFormat` to a `NetlistFormat` enum."""
+        F = vlsir.netlist.NetlistFormat
+        if proto == F.UNSPECIFIED or proto == F.SPECTRE:
+            return NetlistFormat.SPECTRE
+        if proto == F.SPICE:
+            return NetlistFormat.SPICE
+        if proto == F.NGSPICE:
+            return NetlistFormat.NGSPICE
+        if proto == F.XYCE:
+            return NetlistFormat.XYCE
+        if proto == F.HSPICE:
+            return NetlistFormat.HSPICE
+        if proto == F.CDL:
+            return NetlistFormat.CDL
+        if proto == F.VERILOG:
+            return NetlistFormat.VERILOG
+        raise ValueError(f"Unknown NetlistFormat: {proto}")
 
 
 # Type-alias for specifying format, either in enum or string terms
 NetlistFormatSpec = Union[NetlistFormat, str]
-
-## FIXME: add more `Netlistable`s
-##Netlistable = Union[vlsir.circuit.Package]
-Netlistable = vlsir.circuit.Package
-
-
-def netlist(
-    pkg: Netlistable,  ## FIXME: rename
-    dest: IO,
-    fmt: NetlistFormatSpec = "spectre",
-    opts: Optional[NetlistOptions] = None,
-) -> None:
-    """Netlist proto-Package `pkg` to destination `dest`.
-
-    Example usages:
-    ```python
-    h.netlist(pkg, dest=open('mynetlist.v', 'w'), fmt='verilog')
-    ```
-    ```python
-    s = StringIO()
-    h.netlist(pkg, dest=s, fmt='spectre')
-    ```
-    ```python
-    import sys
-    h.netlist(pkg, dest=sys.stdout, fmt='spice')
-    ```
-
-    Primary argument `pkg` must be a `vlsir.circuit.Package`.
-    Destination `dest` may be anything that supports the `typing.IO` bundle,
-    commonly including open file-handles. `StringIO` is particularly helpful
-    for producing a netlist in an in-memory string.
-    Format-specifier `fmt` may be any of the `NetlistFormatSpec` enumerated values
-    or their string equivalents.
-    """
-
-    if opts is not None:
-        raise NotImplementedError("NetlistOptions not yet implemented.")  # FIXME!
-
-    # If `fmt` is a string, turn it into an enum
-    fmt_enum = NetlistFormat.get(fmt)
-
-    # Get the corresponding `Netlister` class and instantiate it
-    netlister_cls = fmt_enum.netlister()
-    netlister = netlister_cls(dest=dest)
-
-    # Write the netlist
-    return netlister.write_package(pkg)
-
-
-# Set our exported content for star-imports
-__all__ = ["netlist", "NetlistFormat", "NetlistFormatSpec"]
```

### Comparing `vlsirtools-5.0.0/vlsirtools/netlist/base.py` & `vlsirtools-6.0.0rc0/vlsirtools/netlist/base.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-5.0.0/vlsirtools/netlist/spectre.py` & `vlsirtools-6.0.0rc0/vlsirtools/netlist/spectre.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-5.0.0/vlsirtools/netlist/spectre_spice_shared.py` & `vlsirtools-6.0.0rc0/vlsirtools/netlist/spectre_spice_shared.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-5.0.0/vlsirtools/netlist/spice.py` & `vlsirtools-6.0.0rc0/vlsirtools/netlist/spice.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-5.0.0/vlsirtools/netlist/verilog.py` & `vlsirtools-6.0.0rc0/vlsirtools/netlist/verilog.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-5.0.0/vlsirtools/primitives.py` & `vlsirtools-6.0.0rc0/vlsirtools/primitives.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-5.0.0/vlsirtools/pytest.py` & `vlsirtools-6.0.0rc0/vlsirtools/pytest.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-5.0.0/vlsirtools/spice/base.py` & `vlsirtools-6.0.0rc0/vlsirtools/spice/base.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-5.0.0/vlsirtools/spice/ngspice.py` & `vlsirtools-6.0.0rc0/vlsirtools/spice/ngspice.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-5.0.0/vlsirtools/spice/sim_data.py` & `vlsirtools-6.0.0rc0/vlsirtools/spice/sim_data.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-5.0.0/vlsirtools/spice/spectre.py` & `vlsirtools-6.0.0rc0/vlsirtools/spice/spectre.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-5.0.0/vlsirtools/spice/spice.py` & `vlsirtools-6.0.0rc0/vlsirtools/spice/spice.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-5.0.0/vlsirtools/spice/xyce.py` & `vlsirtools-6.0.0rc0/vlsirtools/spice/xyce.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-5.0.0/vlsirtools/spicetype.py` & `vlsirtools-6.0.0rc0/vlsirtools/spicetype.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-5.0.0/vlsirtools.egg-info/PKG-INFO` & `vlsirtools-6.0.0rc0/vlsirtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlsirtools
-Version: 5.0.0
+Version: 6.0.0rc0
 Summary: Tools for the Vlsir IC Design Schema
 Home-page: https://github.com/Vlsir/Vlsir
 Author: Dan Fritchman
 Author-email: dan@fritch.mn
 Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `vlsirtools-5.0.0/vlsirtools.egg-info/SOURCES.txt` & `vlsirtools-6.0.0rc0/vlsirtools.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 .gitignore
 LICENSE
 readme.md
 setup.py
 tests/__init__.py
+tests/test_netlist.py
 tests/test_primitives.py
 tests/test_vlsirtools.py
 vlsirtools/__init__.py
 vlsirtools/primitives.py
 vlsirtools/pytest.py
 vlsirtools/spicetype.py
 vlsirtools.egg-info/PKG-INFO
 vlsirtools.egg-info/SOURCES.txt
 vlsirtools.egg-info/dependency_links.txt
 vlsirtools.egg-info/requires.txt
 vlsirtools.egg-info/top_level.txt
 vlsirtools/netlist/__init__.py
 vlsirtools/netlist/base.py
+vlsirtools/netlist/fmt.py
+vlsirtools/netlist/main.py
 vlsirtools/netlist/spectre.py
 vlsirtools/netlist/spectre_spice_shared.py
 vlsirtools/netlist/spice.py
 vlsirtools/netlist/verilog.py
 vlsirtools/spectre/__init__.py
 vlsirtools/spice/__init__.py
 vlsirtools/spice/base.py
```


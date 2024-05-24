# Comparing `tmp/clickhouse-connect-micropip-0.7.0.tar.gz` & `tmp/clickhouse_connect_micropip-0.7.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhouse-connect-micropip-0.7.0.tar", last modified: Wed Jan 24 20:22:29 2024, max compression
+gzip compressed data, was "clickhouse_connect_micropip-0.7.10.tar", last modified: Fri May 24 16:39:20 2024, max compression
```

## Comparing `clickhouse-connect-micropip-0.7.0.tar` & `clickhouse_connect_micropip-0.7.10.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:22:29.795166 clickhouse-connect-micropip-0.7.0/
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)    11389 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/LICENSE
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)       26 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/MANIFEST.in
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     2762 2024-01-24 20:22:29.795166 clickhouse-connect-micropip-0.7.0/PKG-INFO
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     1521 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/README.md
-drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:22:29.785166 clickhouse-connect-micropip-0.7.0/clickhouse_connect/
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      111 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/__init__.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)       18 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/__version__.py
-drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:22:29.785166 clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      204 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/__init__.py
-drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:22:29.785166 clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/datatypes/
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)       59 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/datatypes/__init__.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     4798 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/datatypes/base.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)    13683 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py
-drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:22:29.785166 clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/ddl/
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/ddl/__init__.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     1709 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/ddl/custom.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     7649 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     3780 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/dialect.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     2539 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/inspector.py
-drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:22:29.785166 clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/sql/
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      460 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/sql/__init__.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      903 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      283 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/sql/preparer.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     2534 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/common.py
-drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:22:29.785166 clickhouse-connect-micropip-0.7.0/clickhouse_connect/datatypes/
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      311 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/datatypes/__init__.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)    14783 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/datatypes/base.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)    11642 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/datatypes/container.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     2568 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/datatypes/format.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     4686 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/datatypes/network.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)    11285 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/datatypes/numeric.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     2424 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/datatypes/registry.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     4114 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/datatypes/special.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     5070 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/datatypes/string.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     8422 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/datatypes/temporal.py
-drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:22:29.785166 clickhouse-connect-micropip-0.7.0/clickhouse_connect/dbapi/
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      882 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/dbapi/__init__.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     1531 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/dbapi/connection.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     4368 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/dbapi/cursor.py
-drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:22:29.795166 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     6849 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/__init__.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     4383 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/buffer.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)    39745 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/client.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     6065 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/common.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     1756 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/compression.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)       80 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/constants.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     2769 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/context.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     1538 2024-01-24 20:21:04.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/ctypes.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     4327 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/dataconv.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      825 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/ddl.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      338 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/errors.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     2842 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/exceptions.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     5286 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/external.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)    22267 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/httpclient.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     8153 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/httputil.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     8717 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/insert.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      830 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/models.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      316 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/npconv.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     4304 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/npquery.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     1354 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/options.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     5723 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/parser.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)    20620 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/query.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     1202 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/summary.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     1256 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/tools.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     5236 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/transform.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     1011 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/types.py
-drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:22:29.795166 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driverc/
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driverc/__init__.pxd
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driverc/__init__.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      547 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driverc/buffer.pxd
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)    11180 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driverc/buffer.pyx
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)    11482 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driverc/dataconv.pyx
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      410 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/driverc/npconv.pyx
--rwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)     1163 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/entry_points.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     1307 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/json_impl.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/py.typed
-drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:22:29.795166 clickhouse-connect-micropip-0.7.0/clickhouse_connect/tools/
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/tools/__init__.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     8182 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/tools/datagen.py
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     2174 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect/tools/testing.py
-drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:22:29.795166 clickhouse-connect-micropip-0.7.0/clickhouse_connect_micropip.egg-info/
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     2762 2024-01-24 20:22:29.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect_micropip.egg-info/PKG-INFO
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     2958 2024-01-24 20:22:29.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect_micropip.egg-info/SOURCES.txt
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)        1 2024-01-24 20:22:29.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect_micropip.egg-info/dependency_links.txt
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      178 2024-01-24 20:22:29.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect_micropip.egg-info/entry_points.txt
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      144 2024-01-24 20:22:29.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect_micropip.egg-info/requires.txt
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)       19 2024-01-24 20:22:29.000000 clickhouse-connect-micropip-0.7.0/clickhouse_connect_micropip.egg-info/top_level.txt
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      189 2024-01-24 20:09:27.000000 clickhouse-connect-micropip-0.7.0/pyproject.toml
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)       38 2024-01-24 20:22:29.795166 clickhouse-connect-micropip-0.7.0/setup.cfg
--rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     3476 2024-01-24 20:21:45.000000 clickhouse-connect-micropip-0.7.0/setup.py
+drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-05-24 16:39:20.874820 clickhouse_connect_micropip-0.7.10/
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)    11389 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/LICENSE
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)       26 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/MANIFEST.in
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     2881 2024-05-24 16:39:20.874820 clickhouse_connect_micropip-0.7.10/PKG-INFO
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     1521 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/README.md
+drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-05-24 16:39:20.824820 clickhouse_connect_micropip-0.7.10/clickhouse_connect/
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      111 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/__init__.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)       19 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/__version__.py
+drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-05-24 16:39:20.824820 clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      204 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/__init__.py
+drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-05-24 16:39:20.824820 clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/datatypes/
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)       59 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/datatypes/__init__.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     4805 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/datatypes/base.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)    13684 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py
+drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-05-24 16:39:20.824820 clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/ddl/
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/ddl/__init__.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     1709 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/ddl/custom.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     8027 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     3780 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/dialect.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     2539 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/inspector.py
+drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-05-24 16:39:20.834820 clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/sql/
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      460 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/sql/__init__.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      903 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      283 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/sql/preparer.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     2534 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/common.py
+drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-05-24 16:39:20.834820 clickhouse_connect_micropip-0.7.10/clickhouse_connect/datatypes/
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      311 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/datatypes/__init__.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)    14783 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/datatypes/base.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)    11642 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/datatypes/container.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     2568 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/datatypes/format.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     4686 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/datatypes/network.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)    11305 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/datatypes/numeric.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     2424 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/datatypes/registry.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     4114 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/datatypes/special.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     5070 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/datatypes/string.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     8422 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/datatypes/temporal.py
+drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-05-24 16:39:20.844820 clickhouse_connect_micropip-0.7.10/clickhouse_connect/dbapi/
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      882 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/dbapi/__init__.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     1531 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/dbapi/connection.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     4677 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/dbapi/cursor.py
+drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-05-24 16:39:20.854820 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     6878 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/__init__.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     4383 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/buffer.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)    43255 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/client.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     6113 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/common.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     1756 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/compression.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)       80 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/constants.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     2429 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/context.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     1538 2024-01-24 20:21:04.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/ctypes.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     4332 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/dataconv.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      825 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/ddl.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      338 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/errors.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     2842 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/exceptions.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     5310 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/external.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)    23637 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/httpclient.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     8166 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/httputil.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     8717 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/insert.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      830 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/models.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      316 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/npconv.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     4510 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/npquery.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     1354 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/options.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     5723 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/parser.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)    20794 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/query.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     1202 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/summary.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     1396 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/tools.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     5305 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/transform.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     1011 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/types.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     1451 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/tzutil.py
+drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-05-24 16:39:20.864820 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driverc/
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driverc/__init__.pxd
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driverc/__init__.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      547 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driverc/buffer.pxd
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)    11180 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driverc/buffer.pyx
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)    11482 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driverc/dataconv.pyx
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      410 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/driverc/npconv.pyx
+-rwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)     1163 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/entry_points.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     1307 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/json_impl.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/py.typed
+drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-05-24 16:39:20.864820 clickhouse_connect_micropip-0.7.10/clickhouse_connect/tools/
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/tools/__init__.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     8182 2024-01-24 20:09:27.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/tools/datagen.py
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     2296 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect/tools/testing.py
+drwxr-xr-x   0 c0mm4nd   (1000) c0mm4nd   (1000)        0 2024-05-24 16:39:20.874820 clickhouse_connect_micropip-0.7.10/clickhouse_connect_micropip.egg-info/
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     2881 2024-05-24 16:39:20.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect_micropip.egg-info/PKG-INFO
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     2994 2024-05-24 16:39:20.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect_micropip.egg-info/SOURCES.txt
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)        1 2024-05-24 16:39:20.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect_micropip.egg-info/dependency_links.txt
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      178 2024-05-24 16:39:20.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect_micropip.egg-info/entry_points.txt
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      163 2024-05-24 16:39:20.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect_micropip.egg-info/requires.txt
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)       19 2024-05-24 16:39:20.000000 clickhouse_connect_micropip-0.7.10/clickhouse_connect_micropip.egg-info/top_level.txt
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)      190 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/pyproject.toml
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)       38 2024-05-24 16:39:20.874820 clickhouse_connect_micropip-0.7.10/setup.cfg
+-rw-r--r--   0 c0mm4nd   (1000) c0mm4nd   (1000)     3663 2024-05-24 16:36:44.000000 clickhouse_connect_micropip-0.7.10/setup.py
```

### Comparing `clickhouse-connect-micropip-0.7.0/LICENSE` & `clickhouse_connect_micropip-0.7.10/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2022-2023 ClickHouse, Inc.
+Copyright 2022-2024 ClickHouse, Inc.
 
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `clickhouse-connect-micropip-0.7.0/PKG-INFO` & `clickhouse_connect_micropip-0.7.10/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: clickhouse-connect-micropip
-Version: 0.7.0
+Version: 0.7.10
 Summary: ClickHouse Database Core Driver for Python, Pandas, and Superset
 Home-page: https://github.com/ClickHouse/clickhouse-connect
 Author: ClickHouse Inc.
 Author-email: clients@clickhouse.com
 License: Apache License 2.0
 Keywords: clickhouse,superset,sqlalchemy,http,driver
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: certifi
 Requires-Dist: urllib3>=1.26
 Requires-Dist: pytz
 Requires-Dist: zstandard
@@ -28,14 +29,16 @@
 Requires-Dist: numpy; extra == "numpy"
 Provides-Extra: pandas
 Requires-Dist: pandas; extra == "pandas"
 Provides-Extra: arrow
 Requires-Dist: pyarrow; extra == "arrow"
 Provides-Extra: orjson
 Requires-Dist: orjson; extra == "orjson"
+Provides-Extra: tzlocal
+Requires-Dist: tzlocal; extra == "tzlocal"
 
 ## ClickHouse Connect
 
 A high performance core database driver for connecting ClickHouse to Python, Pandas, and Superset
 * Pandas DataFrames
 * Numpy Arrays
 * PyArrow Tables
```

### Comparing `clickhouse-connect-micropip-0.7.0/README.md` & `clickhouse_connect_micropip-0.7.10/README.md`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/datatypes/base.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/datatypes/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from typing import Dict, Type
 
 from sqlalchemy.exc import CompileError
 
 from clickhouse_connect.datatypes.base import ClickHouseType, TypeDef, EMPTY_TYPE_DEF
 from clickhouse_connect.datatypes.registry import parse_name, type_map
-from clickhouse_connect.driver.query import format_query_value
+from clickhouse_connect.driver.query import str_query_value
 
 logger = logging.getLogger(__name__)
 
 
 class ChSqlaType:
     """
     A SQLAlchemy TypeEngine that wraps a ClickHouseType.  We don't extend TypeEngine directly, instead all concrete
@@ -92,20 +92,20 @@
     @staticmethod
     def _cached_literal_processor(*_):
         """
         Override for the SqlAlchemy TypeEngine _cached_literal_processor. We delegate to the driver format_query_value
         method and should be able to ignore literal_processor definitions in the dialect, which are verbose and
         confusing.
         """
-        return format_query_value
+        return str_query_value
 
     def _compiler_dispatch(self, _visitor, **_):
         """
         Override for the SqlAlchemy TypeEngine _compiler_dispatch method to sidestep unnecessary layers and complexity
-        when generating the type name.  The underlying ClickHouseType generates the correct name
+        when generating the type name.  The underlying ClickHouseType generates the correct name for the type
         :return: Name generated by the underlying driver.
         """
         return self.name
 
 
 class CaseInsensitiveDict(dict):
     def __setitem__(self, key, value):
```

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,15 +231,15 @@
         SqlaDateTime.__init__(self)
 
 
 class DateTime64(ChSqlaType, SqlaDateTime):
     def __init__(self, precision: int = None, tz: str = None, type_def: TypeDef = None):
         """
         Date time constructor with precision and timezone parameters if not constructed with TypeDef
-        :param precision:   Usually 3/6/9 for mill/micro/nansecond precision on ClickHouse side
+        :param precision:   Usually 3/6/9 for mill/micro/nanosecond precision on ClickHouse side
         :param tz: Timezone string as defined in pytz
         :param type_def: TypeDef from parse_name function
         """
         if not type_def:
             if tz:
                 pytz.timezone(tz)
                 type_def = TypeDef(values=(precision, f"'{tz}'"))
```

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/ddl/custom.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/ddl/custom.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py`

 * *Files 6% similar despite different names*

```diff
@@ -143,14 +143,18 @@
     def __init__(self, order_by: str = None, primary_key: str = None,
                  partition_by: str = None, sample_by: str = None):
         if not order_by and not primary_key:
             raise ArgumentError(None, 'Either PRIMARY KEY or ORDER BY must be specified')
         super().__init__(locals())
 
 
+class SharedMergeTree(MergeTree):
+    pass
+
+
 class SummingMergeTree(MergeTree):
     pass
 
 
 class AggregatingMergeTree(MergeTree):
     pass
 
@@ -222,14 +226,34 @@
     pass
 
 
 class ReplicatedSummingMergeTree(ReplicatedMergeTree):
     pass
 
 
+class SharedReplacingMergeTree(ReplacingMergeTree):
+    pass
+
+
+class SharedAggregatingMergeTree(AggregatingMergeTree):
+    pass
+
+
+class SharedSummingMergeTree(SummingMergeTree):
+    pass
+
+
+class SharedVersionedCollapsingMergeTree(VersionedCollapsingMergeTree):
+    pass
+
+
+class SharedGraphiteMergeTree(GraphiteMergeTree):
+    pass
+
+
 def build_engine(full_engine: str) -> Optional[TableEngine]:
     """
     Factory function to create TableEngine class from ClickHouse full_engine expression
     :param full_engine
     :return: TableEngine DDL element
     """
     if not full_engine:
```

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/dialect.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/inspector.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/inspector.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/common.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/common.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/datatypes/base.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/datatypes/container.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/datatypes/container.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/datatypes/format.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/datatypes/format.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/datatypes/network.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/datatypes/network.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/datatypes/numeric.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/datatypes/numeric.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,17 +287,17 @@
 
     def _write_column_binary(self, column: Union[Sequence, MutableSequence], dest: bytearray, _ctx):
         with decimal.localcontext() as ctx:
             ctx.prec = self.prec
             dec = decimal.Decimal
             mult = self._mult
             if self.nullable:
-                write_array(self._array_type, [int(dec(x) * mult) if x else 0 for x in column], dest)
+                write_array(self._array_type, [int(dec(str(x)) * mult) if x else 0 for x in column], dest)
             else:
-                write_array(self._array_type, [int(dec(x) * mult) for x in column], dest)
+                write_array(self._array_type, [int(dec(str(x)) * mult) for x in column], dest)
 
     def _active_null(self, ctx: QueryContext):
         if ctx.use_none:
             return None
         digits = str('0').rjust(self.prec, '0')
         scale = self.scale
         return decimal.Decimal(f'{digits[:-scale]}.{digits[-scale:]}')
@@ -331,18 +331,18 @@
             ctx.prec = self.prec
             mult = decimal.Decimal(f"{self._mult}.{'0' * self.scale}")
             sz = self.byte_size
             itb = int.to_bytes
             if self.nullable:
                 v = self._zeros
                 for x in column:
-                    dest += v if not x else itb(int(decimal.Decimal(x) * mult), sz, 'little', signed=True)
+                    dest += v if not x else itb(int(decimal.Decimal(str(x)) * mult), sz, 'little', signed=True)
             else:
                 for x in column:
-                    dest += itb(int(decimal.Decimal(x) * mult), sz, 'little', signed=True)
+                    dest += itb(int(decimal.Decimal(str(x)) * mult), sz, 'little', signed=True)
 
 
 class Decimal32(Decimal):
     dec_size = 32
 
 
 class Decimal64(Decimal):
```

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/datatypes/registry.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/datatypes/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     elif base.startswith('Nested'):
         keys, values = parse_columns(base[6:])
         base = 'Nested'
     elif base.startswith('Tuple'):
         keys, values = parse_columns(base[5:])
         base = 'Tuple'
     elif base == 'Point':
-        values = ['Float64', 'Float64']
+        values = ('Float64', 'Float64')
     else:
         try:
             base, values, _ = parse_callable(base)
         except IndexError:
             raise InternalError(f'Can not parse ClickHouse data type: {name}') from None
     return base, name, TypeDef(tuple(wrappers), keys, values)
```

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/datatypes/special.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/datatypes/special.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/datatypes/string.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/datatypes/string.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/datatypes/temporal.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/datatypes/temporal.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/dbapi/__init__.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/dbapi/connection.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/dbapi/cursor.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/dbapi/cursor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import re
 
-from typing import Optional, Sequence
+from typing import Optional, Sequence, List, Dict
 
 from clickhouse_connect.datatypes.registry import get_from_name
 from clickhouse_connect.driver.common import unescape_identifier
 from clickhouse_connect.driver.exceptions import ProgrammingError
 from clickhouse_connect.driver import Client
 from clickhouse_connect.driver.parser import parse_callable
 from clickhouse_connect.driver.query import remove_sql_comments
@@ -13,47 +13,54 @@
 logger = logging.getLogger(__name__)
 
 insert_re = re.compile(r'^\s*INSERT\s+INTO\s+(.*$)', re.IGNORECASE)
 str_type = get_from_name('String')
 int_type = get_from_name('Int32')
 
 
+# pylint: disable=too-many-instance-attributes
 class Cursor:
     """
     See :ref:`https://peps.python.org/pep-0249/`
     """
 
     def __init__(self, client: Client):
         self.client = client
         self.arraysize = 1
         self.data: Optional[Sequence] = None
         self.names = []
         self.types = []
         self._rowcount = 0
+        self._summary: List[Dict[str, str]] = []
         self._ix = 0
 
     def check_valid(self):
         if self.data is None:
             raise ProgrammingError('Cursor is not valid')
 
     @property
     def description(self):
         return [(n, t, None, None, None, None, True) for n, t in zip(self.names, self.types)]
 
     @property
     def rowcount(self):
         return self._rowcount
 
+    @property
+    def summary(self) -> List[Dict[str, str]]:
+        return self._summary
+
     def close(self):
         self.data = None
 
     def execute(self, operation: str, parameters=None):
         query_result = self.client.query(operation, parameters)
         self.data = query_result.result_set
         self._rowcount = len(self.data)
+        self._summary.append(query_result.summary)
         if query_result.column_names:
             self.names = query_result.column_names
             self.types = [x.name for x in query_result.column_types]
         elif self.data:
             self.names = [f'col_{x}' for x in range(len(self.data[0]))]
             self.types = [x.__class__ for x in self.data[0]]
 
@@ -90,14 +97,15 @@
                 if self.names or self.types:
                     if query_result.column_names != self.names:
                         logger.warning('Inconsistent column names %s : %s for operation %s in cursor executemany',
                                        self.names, query_result.column_names, operation)
                 else:
                     self.names = query_result.column_names
                     self.types = query_result.column_types
+                self._summary.append(query_result.summary)
         except TypeError as ex:
             raise ProgrammingError(f'Invalid parameters {parameters} passed to cursor executemany') from ex
         self._rowcount = len(self.data)
 
     def fetchall(self):
         self.check_valid()
         ret = self.data
```

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/__init__.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,16 @@
         username = username or parsed.username
         password = password or parsed.password
         host = host or parsed.hostname
         port = port or parsed.port
         if parsed.path and (not database or database == '__default__'):
             database = parsed.path[1:].split('/')[0]
         database = database or parsed.path
-        kwargs.update(dict(parse_qs(parsed.query)))
+        for k, v in parse_qs(parsed.query).items():
+            kwargs[k] = v[0]
     use_tls = str(secure).lower() == 'true' or interface == 'https' or (not interface and port in (443, 8443))
     if not host:
         host = 'localhost'
     if not interface:
         interface = 'https' if use_tls else 'http'
     port = port or default_port(interface, use_tls)
     if username is None and 'user' in kwargs:
```

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/buffer.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/buffer.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/client.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import io
 import logging
-from datetime import tzinfo, datetime
+from datetime import tzinfo
 
 import pytz
 
 from abc import ABC, abstractmethod
 from typing import Iterable, Optional, Any, Union, Sequence, Dict, Generator, BinaryIO
 from pytz.exceptions import UnknownTimeZoneError
 
 from clickhouse_connect import common
 from clickhouse_connect.common import version
 from clickhouse_connect.datatypes.registry import get_from_name
 from clickhouse_connect.datatypes.base import ClickHouseType
+from clickhouse_connect.driver import tzutil
 from clickhouse_connect.driver.common import dict_copy, StreamContext, coerce_int, coerce_bool
 from clickhouse_connect.driver.constants import CH_VERSION_WITH_PROTOCOL, PROTOCOL_VERSION_WITH_LOW_CARD
 from clickhouse_connect.driver.exceptions import ProgrammingError, OperationalError
 from clickhouse_connect.driver.external import ExternalData
 from clickhouse_connect.driver.insert import InsertContext
 from clickhouse_connect.driver.summary import QuerySummary
 from clickhouse_connect.driver.models import ColumnDef, SettingDef, SettingStatus
-from clickhouse_connect.driver.query import QueryResult, to_arrow, QueryContext, arrow_buffer
+from clickhouse_connect.driver.query import QueryResult, to_arrow, to_arrow_batches, QueryContext, arrow_buffer, \
+    quote_identifier
 
 io.DEFAULT_BUFFER_SIZE = 1024 * 256
 logger = logging.getLogger(__name__)
 arrow_str_setting = 'output_format_arrow_string_as_string'
 
 
 # pylint: disable=too-many-public-methods, too-many-instance-attributes
@@ -34,41 +36,51 @@
     compression: str = None
     write_compression: str = None
     protocol_version = 0
     valid_transport_settings = set()
     optional_transport_settings = set()
     database = None
     max_error_message = 0
+    apply_server_timezone = False
+    show_clickhouse_errors = True
 
     def __init__(self,
                  database: str,
                  query_limit: int,
                  uri: str,
                  query_retries: int,
                  server_host_name: Optional[str],
-                 apply_server_timezone: Optional[Union[str, bool]]):
+                 apply_server_timezone: Optional[Union[str, bool]],
+                 show_clickhouse_errors: Optional[bool]):
         """
         Shared initialization of ClickHouse Connect client
         :param database: database name
         :param query_limit: default LIMIT for queries
         :param uri: uri for error messages
         """
         self.query_limit = coerce_int(query_limit)
         self.query_retries = coerce_int(query_retries)
+        if show_clickhouse_errors is not None:
+            self.show_clickhouse_errors = coerce_bool(show_clickhouse_errors)
         self.server_host_name = server_host_name
-        self.server_tz = pytz.UTC
+        self.server_tz, dst_safe = pytz.UTC, True
         self.server_version, server_tz = \
             tuple(self.command('SELECT version(), timezone()', use_database=False))
         try:
-            self.server_tz = pytz.timezone(server_tz)
+            server_tz = pytz.timezone(server_tz)
+            server_tz, dst_safe = tzutil.normalize_timezone(server_tz)
+            if apply_server_timezone is None:
+                apply_server_timezone = dst_safe
+            self.apply_server_timezone = apply_server_timezone == 'always' or coerce_bool(apply_server_timezone)
         except UnknownTimeZoneError:
             logger.warning('Warning, server is using an unrecognized timezone %s, will use UTC default', server_tz)
-        offsets_differ = datetime.now().astimezone().utcoffset() != datetime.now(tz=self.server_tz).utcoffset()
-        self.apply_server_timezone = apply_server_timezone == 'always' or (
-                coerce_bool(apply_server_timezone) and offsets_differ)
+
+        if not self.apply_server_timezone and not tzutil.local_tz_dst_safe:
+            logger.warning('local timezone %s may return unexpected times due to Daylight Savings Time/' +
+                           'Summer Time differences', tzutil.local_tz.tzname(None))
         readonly = 'readonly'
         if not self.min_version('19.17'):
             readonly = common.get_setting('readonly')
         server_settings = self.query(f'SELECT name, value, {readonly} as readonly FROM system.settings LIMIT 10000')
         self.server_settings = {row['name']: SettingDef(**row) for row in server_settings.named_results()}
         if database and not database == '__default__':
             self.database = database
@@ -153,15 +165,15 @@
         """
         :param key: The setting key
         :return: The string value of the setting, if it exists, or None
         """
 
     # pylint: disable=too-many-arguments,unused-argument,too-many-locals
     def query(self,
-              query: str = None,
+              query: Optional[str] = None,
               parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
               settings: Optional[Dict[str, Any]] = None,
               query_formats: Optional[Dict[str, str]] = None,
               column_formats: Optional[Dict[str, Union[str, Dict[str, str]]]] = None,
               encoding: Optional[str] = None,
               use_none: Optional[bool] = None,
               column_oriented: Optional[bool] = None,
@@ -189,15 +201,15 @@
                                     external_data=query_context.external_data)
             if isinstance(response, QuerySummary):
                 return response.as_query_result()
             return QueryResult([response] if isinstance(response, list) else [[response]])
         return self._query_with_context(query_context)
 
     def query_column_block_stream(self,
-                                  query: str = None,
+                                  query: Optional[str] = None,
                                   parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
                                   settings: Optional[Dict[str, Any]] = None,
                                   query_formats: Optional[Dict[str, str]] = None,
                                   column_formats: Optional[Dict[str, Union[str, Dict[str, str]]]] = None,
                                   encoding: Optional[str] = None,
                                   use_none: Optional[bool] = None,
                                   context: QueryContext = None,
@@ -208,15 +220,15 @@
         Variation of main query method that returns a stream of column oriented blocks. For
         parameters, see the create_query_context method.
         :return: StreamContext -- Iterable stream context that returns column oriented blocks
         """
         return self._context_query(locals(), use_numpy=False, streaming=True).column_block_stream
 
     def query_row_block_stream(self,
-                               query: str = None,
+                               query: Optional[str] = None,
                                parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
                                settings: Optional[Dict[str, Any]] = None,
                                query_formats: Optional[Dict[str, str]] = None,
                                column_formats: Optional[Dict[str, Union[str, Dict[str, str]]]] = None,
                                encoding: Optional[str] = None,
                                use_none: Optional[bool] = None,
                                context: QueryContext = None,
@@ -227,15 +239,15 @@
         Variation of main query method that returns a stream of row oriented blocks. For
         parameters, see the create_query_context method.
         :return: StreamContext -- Iterable stream context that returns blocks of rows
         """
         return self._context_query(locals(), use_numpy=False, streaming=True).row_block_stream
 
     def query_rows_stream(self,
-                          query: str = None,
+                          query: Optional[str] = None,
                           parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
                           settings: Optional[Dict[str, Any]] = None,
                           query_formats: Optional[Dict[str, str]] = None,
                           column_formats: Optional[Dict[str, Union[str, Dict[str, str]]]] = None,
                           encoding: Optional[str] = None,
                           use_none: Optional[bool] = None,
                           context: QueryContext = None,
@@ -264,17 +276,36 @@
         :param fmt: ClickHouse output format
         :param use_database  Send the database parameter to ClickHouse so the command will be executed in the client
          database context.
         :param external_data  External data to send with the query
         :return: bytes representing raw ClickHouse return value based on format
         """
 
+    @abstractmethod
+    def raw_stream(self, query: str,
+                   parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
+                   settings: Optional[Dict[str, Any]] = None,
+                   fmt: str = None,
+                   use_database: bool = True,
+                   external_data: Optional[ExternalData] = None) -> io.IOBase:
+        """
+       Query method that returns the result as an io.IOBase iterator
+       :param query: Query statement/format string
+       :param parameters: Optional dictionary used to format the query
+       :param settings: Optional dictionary of ClickHouse settings (key/string values)
+       :param fmt: ClickHouse output format
+       :param use_database  Send the database parameter to ClickHouse so the command will be executed in the client
+        database context.
+       :param external_data  External data to send with the query
+       :return: io.IOBase stream/iterator for the result
+       """
+
     # pylint: disable=duplicate-code,too-many-arguments,unused-argument
     def query_np(self,
-                 query: str = None,
+                 query: Optional[str] = None,
                  parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
                  settings: Optional[Dict[str, Any]] = None,
                  query_formats: Optional[Dict[str, str]] = None,
                  column_formats: Optional[Dict[str, str]] = None,
                  encoding: Optional[str] = None,
                  use_none: Optional[bool] = None,
                  max_str_len: Optional[int] = None,
@@ -285,15 +316,15 @@
         create_query_context method
         :return: Numpy array representing the result set
         """
         return self._context_query(locals(), use_numpy=True).np_result
 
     # pylint: disable=duplicate-code,too-many-arguments,unused-argument
     def query_np_stream(self,
-                        query: str = None,
+                        query: Optional[str] = None,
                         parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
                         settings: Optional[Dict[str, Any]] = None,
                         query_formats: Optional[Dict[str, str]] = None,
                         column_formats: Optional[Dict[str, str]] = None,
                         encoding: Optional[str] = None,
                         use_none: Optional[bool] = None,
                         max_str_len: Optional[int] = None,
@@ -304,15 +335,15 @@
         create_query_context method
         :return: Generator that yield a numpy array per block representing the result set
         """
         return self._context_query(locals(), use_numpy=True, streaming=True).np_stream
 
     # pylint: disable=duplicate-code,too-many-arguments,unused-argument
     def query_df(self,
-                 query: str = None,
+                 query: Optional[str] = None,
                  parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
                  settings: Optional[Dict[str, Any]] = None,
                  query_formats: Optional[Dict[str, str]] = None,
                  column_formats: Optional[Dict[str, str]] = None,
                  encoding: Optional[str] = None,
                  use_none: Optional[bool] = None,
                  max_str_len: Optional[int] = None,
@@ -327,15 +358,15 @@
         create_query_context method
         :return: Pandas dataframe representing the result set
         """
         return self._context_query(locals(), use_numpy=True, as_pandas=True).df_result
 
     # pylint: disable=duplicate-code,too-many-arguments,unused-argument
     def query_df_stream(self,
-                        query: str = None,
+                        query: Optional[str] = None,
                         parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
                         settings: Optional[Dict[str, Any]] = None,
                         query_formats: Optional[Dict[str, str]] = None,
                         column_formats: Optional[Dict[str, str]] = None,
                         encoding: Optional[str] = None,
                         use_none: Optional[bool] = None,
                         max_str_len: Optional[int] = None,
@@ -344,22 +375,22 @@
                         column_tzs: Optional[Dict[str, Union[str, tzinfo]]] = None,
                         context: QueryContext = None,
                         external_data: Optional[ExternalData] = None,
                         use_extended_dtypes: Optional[bool] = None) -> StreamContext:
         """
         Query method that returns the results as a StreamContext.  For parameter values, see the
         create_query_context method
-        :return: Pandas dataframe representing the result set
+        :return: Generator that yields a Pandas dataframe per block representing the result set
         """
         return self._context_query(locals(), use_numpy=True,
                                    as_pandas=True,
                                    streaming=True).df_stream
 
     def create_query_context(self,
-                             query: str = None,
+                             query: Optional[str] = None,
                              parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
                              settings: Optional[Dict[str, Any]] = None,
                              query_formats: Optional[Dict[str, str]] = None,
                              column_formats: Optional[Dict[str, Union[str, Dict[str, str]]]] = None,
                              encoding: Optional[str] = None,
                              use_none: Optional[bool] = None,
                              column_oriented: Optional[bool] = None,
@@ -458,30 +489,58 @@
         :param query: Query statement/format string
         :param parameters: Optional dictionary used to format the query
         :param settings: Optional dictionary of ClickHouse settings (key/string values)
         :param use_strings:  Convert ClickHouse String type to Arrow string type (instead of binary)
         :param external_data ClickHouse "external data" to send with query
         :return: PyArrow.Table
         """
+        settings = self._update_arrow_settings(settings, use_strings)
+        return to_arrow(self.raw_query(query,
+                                       parameters,
+                                       settings,
+                                       fmt='Arrow',
+                                       external_data=external_data))
+
+    def query_arrow_stream(self,
+                           query: str,
+                           parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
+                           settings: Optional[Dict[str, Any]] = None,
+                           use_strings: Optional[bool] = None,
+                           external_data: Optional[ExternalData] = None) -> StreamContext:
+        """
+        Query method that returns the results as a stream of Arrow tables
+        :param query: Query statement/format string
+        :param parameters: Optional dictionary used to format the query
+        :param settings: Optional dictionary of ClickHouse settings (key/string values)
+        :param use_strings:  Convert ClickHouse String type to Arrow string type (instead of binary)
+        :param external_data ClickHouse "external data" to send with query
+        :return: Generator that yields a PyArrow.Table for per block representing the result set
+        """
+        settings = self._update_arrow_settings(settings, use_strings)
+        return to_arrow_batches(self.raw_stream(query,
+                                                parameters,
+                                                settings,
+                                                fmt='ArrowStream',
+                                                external_data=external_data))
+
+    def _update_arrow_settings(self,
+                               settings: Optional[Dict[str, Any]],
+                               use_strings: Optional[bool]) -> Dict[str, Any]:
         settings = dict_copy(settings)
         if self.database:
             settings['database'] = self.database
         str_status = self._setting_status(arrow_str_setting)
         if use_strings is None:
             if str_status.is_writable and not str_status.is_set:
                 settings[arrow_str_setting] = '1'  # Default to returning strings if possible
         elif use_strings != str_status.is_set:
             if not str_status.is_writable:
                 raise OperationalError(f'Cannot change readonly {arrow_str_setting} to {use_strings}')
             settings[arrow_str_setting] = '1' if use_strings else '0'
-        return to_arrow(self.raw_query(query,
-                                       parameters,
-                                       settings,
-                                       fmt='Arrow',
-                                       external_data=external_data))
+        return settings
 
     @abstractmethod
     def command(self,
                 cmd: str,
                 parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
                 data: Union[str, bytes] = None,
                 settings: Dict[str, Any] = None,
@@ -625,15 +684,20 @@
            types nor column type names are set, actual column types will be retrieved from the server.
         :param column_type_names: ClickHouse column type names.  Specified column types by name string
         :param column_oriented: If true the data is already "pivoted" in column form
         :param settings: Optional dictionary of ClickHouse settings (key/string values)
         :param data: Initial dataset for insert
         :return Reusable insert context
         """
-        full_table = table if '.' in table or not database else f'{database}.{table}'
+        full_table = table
+        if '.' not in table:
+            if database:
+                full_table = f'{quote_identifier(database)}.{quote_identifier(table)}'
+            else:
+                full_table = quote_identifier(table)
         column_defs = []
         if column_types is None and column_type_names is None:
             describe_result = self.query(f'DESCRIBE TABLE {full_table}')
             column_defs = [ColumnDef(**row) for row in describe_result.named_results()
                            if row['default_type'] not in ('ALIAS', 'MATERIALIZED')]
         if column_names is None or isinstance(column_names, str) and column_names == '*':
             column_names = [cd.name for cd in column_defs]
```

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/common.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         return 0
     return int(val)
 
 
 def coerce_bool(val: Optional[Union[str, bool]]):
     if not val:
         return False
-    return val in (True, 'True', 'true', '1')
+    return val is True or (isinstance(val, str) and val.lower() in ('true', '1', 'y', 'yes'))
 
 
 class SliceView(Sequence):
     """
     Provides a view into a sequence rather than copying.  Borrows liberally from
     https://gist.github.com/mathieucaroff/0cf094325fb5294fb54c6a577f05a2c1
     Also see the discussion on SO: https://stackoverflow.com/questions/3485475/can-i-create-a-view-on-a-python-list
```

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/compression.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/compression.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/context.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 import logging
 import re
-from datetime import datetime
 from typing import Optional, Dict, Union, Any
 
-import pytz
-
 logger = logging.getLogger(__name__)
 
 _empty_map = {}
 
 
 # pylint: disable=too-many-instance-attributes
 class BaseQueryContext:
-    local_tz: pytz.timezone
 
     def __init__(self,
                  settings: Optional[Dict[str, Any]] = None,
                  query_formats: Optional[Dict[str, str]] = None,
                  column_formats: Optional[Dict[str, Union[str, Dict[str, str]]]] = None,
                  encoding: Optional[str] = None,
                  use_extended_dtypes: bool = False,
@@ -56,17 +52,7 @@
         for type_pattern, fmt in self._active_col_type_fmts.items():
             if type_pattern.match(ch_type):
                 return fmt
         for type_pattern, fmt in self.type_formats.items():
             if type_pattern.match(ch_type):
                 return fmt
         return None
-
-
-def _init_context_cls():
-    local_tz = datetime.now().astimezone().tzinfo
-    if local_tz.tzname(datetime.now()) in ('UTC', 'GMT', 'Universal', 'GMT-0', 'Zulu', 'Greenwich'):
-        local_tz = pytz.UTC
-    BaseQueryContext.local_tz = local_tz
-
-
-_init_context_cls()
```

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/ctypes.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/ctypes.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/dataconv.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/dataconv.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             if not nullable and x is None:
                 return NONE_IN_NULLABLE_COLUMN
             app(0)
         else:
             if encoding:
                 x = x.encode(encoding)
             else:
-                x = b''
+                x = bytes(x)
             sz = len(x)
             while True:
                 b = sz & 0x7f
                 sz >>= 7
                 if sz == 0:
                     app(b)
                     break
```

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/ddl.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/ddl.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/exceptions.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/exceptions.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/external.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/external.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                 self.name = path_base
                 self.file_name = path_name
             else:
                 self.name = file_name.rsplit('.', maxsplit=1)[0]
                 self.file_name = file_name
                 if file_name != path_name and path_base != self.name:
                     logger.warning('External data name %s and file_path %s use different names', file_name, path_name)
-        elif data:
+        elif data is not None:
             if not file_name:
                 raise ProgrammingError('Name is required for query external data')
             self.data = data
             self.name = file_name.rsplit('.', maxsplit=1)[0]
             self.file_name = file_name
         else:
             raise ProgrammingError('Either data or file_path must be specified for external data')
@@ -81,15 +81,15 @@
                  file_name: Optional[str] = None,
                  data: Optional[bytes] = None,
                  fmt: Optional[str] = None,
                  types: Optional[Union[str, Sequence[str]]] = None,
                  structure: Optional[Union[str, Sequence[str]]] = None,
                  mime_type: Optional[str] = None):
         self.files: list[ExternalFile] = []
-        if file_path or data:
+        if file_path or data is not None:
             first_file = ExternalFile(file_path=file_path,
                                       file_name=file_name,
                                       data=data,
                                       fmt=fmt,
                                       types=types,
                                       structure=structure,
                                       mime_type=mime_type)
```

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/httpclient.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/httpclient.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import io
 import json
 import logging
 import re
 import uuid
 from base64 import b64encode
 from typing import Optional, Dict, Any, Sequence, Union, List, Callable, Generator, BinaryIO
 from urllib.parse import urlencode
@@ -17,15 +18,15 @@
 from clickhouse_connect.driver.ctypes import RespBuffCls
 from clickhouse_connect.driver.client import Client
 from clickhouse_connect.driver.common import dict_copy, coerce_bool, coerce_int
 from clickhouse_connect.driver.compression import available_compression
 from clickhouse_connect.driver.exceptions import DatabaseError, OperationalError, ProgrammingError
 from clickhouse_connect.driver.external import ExternalData
 from clickhouse_connect.driver.httputil import ResponseSource, get_pool_manager, get_response_data, \
-    default_pool_manager, get_proxy_manager, all_managers, check_env_proxy, check_conn_reset
+    default_pool_manager, get_proxy_manager, all_managers, check_env_proxy, check_conn_expiration
 from clickhouse_connect.driver.insert import InsertContext
 from clickhouse_connect.driver.summary import QuerySummary
 from clickhouse_connect.driver.query import QueryResult, QueryContext, quote_identifier, bind_query
 from clickhouse_connect.driver.transform import NativeTransform
 
 logger = logging.getLogger(__name__)
 columns_only_re = re.compile(r'LIMIT 0\s*$', re.IGNORECASE)
@@ -63,15 +64,16 @@
                  client_cert_key: Optional[str] = None,
                  session_id: Optional[str] = None,
                  settings: Optional[Dict[str, Any]] = None,
                  pool_mgr: Optional[PoolManager] = None,
                  http_proxy: Optional[str] = None,
                  https_proxy: Optional[str] = None,
                  server_host_name: Optional[str] = None,
-                 apply_server_timezone: Optional[Union[str, bool]] = True):
+                 apply_server_timezone: Optional[Union[str, bool]] = None,
+                 show_clickhouse_errors: Optional[bool] = None):
         """
         Create an HTTP ClickHouse Connect client
         See clickhouse_connect.get_client for parameters
         """
         self.url = f'{interface}://{host}:{port}'
         self.headers = {}
         ch_settings = dict_copy(settings, self.params)
@@ -109,15 +111,15 @@
 
         if not client_cert and username:
             self.headers['Authorization'] = 'Basic ' + b64encode(f'{username}:{password}'.encode()).decode()
         self.headers['User-Agent'] = common.build_client_name(client_name)
         self._read_format = self._write_format = 'Native'
         self._transform = NativeTransform()
 
-        # There is use cases when client need to disable timeouts.
+        # There are use cases when the client needs to disable timeouts.
         if connect_timeout is not None:
             connect_timeout = coerce_int(connect_timeout)
         if send_receive_timeout is not None:
             send_receive_timeout = coerce_int(send_receive_timeout)
         self.timeout = Timeout(connect=connect_timeout, read=send_receive_timeout)
         self.http_retries = 1
         self._send_progress = None
@@ -142,15 +144,16 @@
             compression = None
 
         super().__init__(database=database,
                          uri=self.url,
                          query_limit=query_limit,
                          query_retries=query_retries,
                          server_host_name=server_host_name,
-                         apply_server_timezone=apply_server_timezone)
+                         apply_server_timezone=apply_server_timezone,
+                         show_clickhouse_errors=show_clickhouse_errors)
         self.params = self._validate_settings(ch_settings)
         comp_setting = self._setting_status('enable_http_compression')
         self._send_comp_setting = not comp_setting.is_set and comp_setting.is_writable
         if comp_setting.is_set or comp_setting.is_writable:
             self.compression = compression
         send_setting = self._setting_status('send_progress_in_http_headers')
         self._send_progress = not send_setting.is_set and send_setting.is_writable
@@ -160,22 +163,21 @@
 
     def set_client_setting(self, key, value):
         str_value = self._validate_setting(key, value, common.get_setting('invalid_setting_action'))
         if str_value is not None:
             self.params[key] = str_value
 
     def get_client_setting(self, key) -> Optional[str]:
-        values = self.params.get(key)
-        return values[0] if values else None
+        return self.params.get(key)
 
     def _prep_query(self, context: QueryContext):
         final_query = super()._prep_query(context)
         if context.is_insert:
             return final_query
-        return f'{final_query}\n FORMAT {self._write_format}'
+        return f'{final_query}\n FORMAT {self._read_format}'
 
     def _query_with_context(self, context: QueryContext) -> QueryResult:
         headers = {}
         params = {}
         if self.database:
             params['database'] = self.database
         if self.protocol_version:
@@ -352,16 +354,19 @@
             err_content = get_response_data(response)
         except Exception: # pylint: disable=broad-except
             err_content = None
         finally:
             response.close()
 
         if err_content:
-            err_msg = common.format_error(err_content.decode(errors='backslashreplace'))
-            err_str = f':{err_str}\n {err_msg}'
+            if self.show_clickhouse_errors:
+                err_msg = common.format_error(err_content.decode(errors='backslashreplace'))
+                err_str = f':{err_str}\n {err_msg}'
+            else:
+                err_str = 'The ClickHouse server returned an error.'
         raise OperationalError(err_str) if retried else DatabaseError(err_str) from None
 
     def _raw_request(self,
                      data,
                      params: Dict[str, str],
                      headers: Optional[Dict[str, Any]] = None,
                      method: str = 'POST',
@@ -394,15 +399,15 @@
         if self.server_host_name:
             kwargs['assert_same_host'] = False
             kwargs['headers'].update({'Host': self.server_host_name})
         if fields:
             kwargs['fields'] = fields
         else:
             kwargs['body'] = data
-        check_conn_reset(self.http)
+        check_conn_expiration(self.http)
         query_session = final_params.get('session_id')
         while True:
             attempts += 1
             if query_session:
                 if query_session == self._active_session:
                     raise ProgrammingError('Attempt to execute concurrent queries within the same session.' +
                                            'Please use a separate client instance per thread/process.')
@@ -432,32 +437,44 @@
                     self._error_handler(response, True)
                 logger.debug('Retrying requests with status code %d', response.status)
             elif error_handler:
                 error_handler(response)
             else:
                 self._error_handler(response)
 
-    def ping(self):
+    def raw_query(self, query: str,
+                  parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
+                  settings: Optional[Dict[str, Any]] = None,
+                  fmt: str = None,
+                  use_database: bool = True,
+                  external_data: Optional[ExternalData] = None) -> bytes:
         """
         See BaseClient doc_string for this method
         """
-        try:
-            response = self.http.request('GET', f'{self.url}/ping', timeout=3)
-            return 200 <= response.status < 300
-        except HTTPError:
-            logger.debug('ping failed', exc_info=True)
-            return False
+        body, params, fields = self._prep_raw_query(query, parameters, settings, fmt, use_database, external_data)
+        return self._raw_request(body, params, fields=fields).data
 
-    def raw_query(self, query: str,
-                  parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
-                  settings: Optional[Dict[str, Any]] = None, fmt: str = None,
-                  use_database: bool = True, external_data: Optional[ExternalData] = None) -> bytes:
+    def raw_stream(self, query: str,
+                   parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
+                   settings: Optional[Dict[str, Any]] = None,
+                   fmt: str = None,
+                   use_database: bool = True,
+                   external_data: Optional[ExternalData] = None) -> io.IOBase:
         """
         See BaseClient doc_string for this method
         """
+        body, params, fields = self._prep_raw_query(query, parameters, settings, fmt, use_database, external_data)
+        return self._raw_request(body, params, fields=fields, stream=True)
+
+    def _prep_raw_query(self, query: str,
+                        parameters: Optional[Union[Sequence, Dict[str, Any]]],
+                        settings: Optional[Dict[str, Any]],
+                        fmt: str,
+                        use_database: bool,
+                        external_data: Optional[ExternalData]):
         final_query, bind_params = bind_query(query, parameters, self.server_tz)
         if fmt:
             final_query += f'\n FORMAT {fmt}'
         params = self._validate_settings(settings or {})
         if use_database and self.database:
             params['database'] = self.database
         params.update(bind_params)
@@ -465,13 +482,24 @@
             body = bytes()
             params['query'] = final_query
             params.update(external_data.query_params)
             fields = external_data.form_data
         else:
             body = final_query
             fields = None
-        return self._raw_request(body, params, fields=fields).data
+        return body, params, fields
+
+    def ping(self):
+        """
+        See BaseClient doc_string for this method
+        """
+        try:
+            response = self.http.request('GET', f'{self.url}/ping', timeout=3)
+            return 200 <= response.status < 300
+        except HTTPError:
+            logger.debug('ping failed', exc_info=True)
+            return False
 
     def close(self):
         if self._owns_pool_manager:
             self.http.clear()
             all_managers.pop(self.http, None)
```

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/httputil.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/httputil.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from urllib3.response import HTTPResponse
 
 from clickhouse_connect.driver.exceptions import ProgrammingError
 from clickhouse_connect import common
 
 logger = logging.getLogger(__name__)
 
-# We disable this warning.  Verify must explicitly set to false, so we assume the user knows what they're doing
+# We disable this warning.  Verify must be explicitly set to false, so we assume the user knows what they're doing
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 # Increase this number just to be safe when ClickHouse is returning progress headers
 http.client._MAXHEADERS = 10000  # pylint: disable=protected-access
 
 DEFAULT_KEEP_INTERVAL = 30
 DEFAULT_KEEP_COUNT = 3
@@ -114,21 +114,21 @@
         manager = ProxyManager(https_proxy, **options)
     else:
         manager = PoolManager(**options)
     all_managers[manager] = int(time.time())
     return manager
 
 
-def check_conn_reset(manager: PoolManager):
+def check_conn_expiration(manager: PoolManager):
     reset_seconds = common.get_setting('max_connection_age')
     if reset_seconds:
         last_reset = all_managers.get(manager, 0)
         now = int(time.time())
         if last_reset < now - reset_seconds:
-            logger.debug('connection reset')
+            logger.debug('connection expiration')
             manager.clear()
             all_managers[manager] = now
 
 
 def get_proxy_manager(host: str, http_proxy):
     key = f'{host}__{http_proxy}'
     if key in _proxy_managers:
```

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/insert.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/insert.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/models.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/models.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/npquery.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/npquery.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import itertools
 from typing import Generator, Sequence, Tuple
 
 from clickhouse_connect.driver.common import empty_gen, StreamContext
 from clickhouse_connect.driver.exceptions import StreamClosedError
 from clickhouse_connect.driver.types import Closable
 from clickhouse_connect.driver.options import np, pd
 
@@ -89,22 +90,25 @@
             self._numpy_result = pieces[0]
         else:
             self._numpy_result = np.empty((0,))
         self.close()
         return self
 
     def close_df(self):
-        pieces = list(self._df_stream())
-        pieces = [piece for piece in pieces if not piece.empty]
-        if len(pieces) > 1:
-            self._df_result = pd.concat(pieces, ignore_index=True)
-        elif len(pieces) == 1:
-            self._df_result = pieces[0]
-        else:
-            self._df_result = pd.DataFrame()
+        if self._block_gen is None:
+            raise StreamClosedError
+        bg = self._block_gen
+        chain = itertools.chain
+        chains = [chain(b) for b in zip(*bg)]
+        new_df_series = []
+        for c in chains:
+            series = [pd.Series(piece, copy=False) for piece in c if len(piece) > 0]
+            if len(series) > 0:
+                new_df_series.append(pd.concat(series, copy=False, ignore_index=True))
+        self._df_result = pd.DataFrame(dict(zip(self.column_names, new_df_series)))
         self.close()
         return self
 
     @property
     def np_result(self):
         if self._numpy_result is None:
             self.close_numpy()
```

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/options.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/options.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/parser.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/parser.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/query.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import ipaddress
 import logging
 import re
 import uuid
 import pytz
 
 from enum import Enum
+from io import IOBase
 from typing import Any, Tuple, Dict, Sequence, Optional, Union, Generator
 from datetime import date, datetime, tzinfo
 
 from pytz.exceptions import UnknownTimeZoneError
 
 from clickhouse_connect import common
+from clickhouse_connect.driver import tzutil
 from clickhouse_connect.driver.common import dict_copy, empty_gen, StreamContext
 from clickhouse_connect.driver.external import ExternalData
 from clickhouse_connect.driver.types import Matrix, Closable
 from clickhouse_connect.json_impl import any_to_json
 from clickhouse_connect.driver.exceptions import StreamClosedError, ProgrammingError
 from clickhouse_connect.driver.options import check_arrow, pd_extended_dtypes
 from clickhouse_connect.driver.context import BaseQueryContext
@@ -165,18 +167,16 @@
         elif self.query_tz:
             active_tz = self.query_tz
         elif self.response_tz:
             active_tz = self.response_tz
         elif self.apply_server_tz:
             active_tz = self.server_tz
         else:
-            active_tz = self.local_tz
-        #  Special case where if everything is UTC, including the local timezone, we use naive timezones
-        #  for performance reasons
-        if active_tz == pytz.UTC and active_tz.utcoffset(datetime.now()) == self.local_tz.utcoffset(datetime.now()):
+            active_tz = tzutil.local_tz
+        if active_tz == pytz.UTC:
             return None
         return active_tz
 
     def updated_copy(self,
                      query: Optional[str] = None,
                      parameters: Optional[Dict[str, Any]] = None,
                      settings: Optional[Dict[str, Any]] = None,
@@ -300,16 +300,15 @@
     def row_block_stream(self):
         return StreamContext(self, self._row_block_stream())
 
     @property
     def rows_stream(self) -> StreamContext:
         def stream():
             for block in self._row_block_stream():
-                for row in block:
-                    yield row
+                yield from block
 
         return StreamContext(self, stream())
 
     def named_results(self) -> Generator[dict, None, None]:
         for row in zip(*self.result_set) if self.column_oriented else self.result_set:
             yield dict(zip(self.column_names, row))
 
@@ -337,36 +336,40 @@
             self.source = None
         if self._block_gen is not None:
             self._block_gen.close()
             self._block_gen = None
 
 
 BS = '\\'
-must_escape = (BS, '\'', '`')
+must_escape = (BS, '\'', '`', '\t', '\n')
 
 
 def quote_identifier(identifier: str):
     first_char = identifier[0]
     if first_char in ('`', '"') and identifier[-1] == first_char:
         # Identifier is already quoted, assume that it's valid
         return identifier
     return f'`{escape_str(identifier)}`'
 
 
 def finalize_query(query: str, parameters: Optional[Union[Sequence, Dict[str, Any]]],
                    server_tz: Optional[tzinfo] = None) -> str:
+    while query.endswith(';'):
+        query = query[:-1]
     if not parameters:
         return query
     if hasattr(parameters, 'items'):
         return query % {k: format_query_value(v, server_tz) for k, v in parameters.items()}
     return query % tuple(format_query_value(v) for v in parameters)
 
 
 def bind_query(query: str, parameters: Optional[Union[Sequence, Dict[str, Any]]],
                server_tz: Optional[tzinfo] = None) -> Tuple[str, Dict[str, str]]:
+    while query.endswith(';'):
+        query = query[:-1]
     if not parameters:
         return query, {}
     if external_bind_re.search(query) is None:
         return finalize_query(query, parameters, server_tz), {}
     return query, {f'param_{k}': format_bind_value(v, server_tz) for k, v in parameters.items()}
 
 
@@ -393,28 +396,32 @@
     if isinstance(value, datetime):
         if value.tzinfo is not None or server_tz != pytz.UTC:
             value = value.astimezone(server_tz)
         return f"'{value.strftime('%Y-%m-%d %H:%M:%S')}'"
     if isinstance(value, date):
         return f"'{value.isoformat()}'"
     if isinstance(value, list):
-        return f"[{', '.join(format_query_value(x, server_tz) for x in value)}]"
+        return f"[{', '.join(str_query_value(x, server_tz) for x in value)}]"
     if isinstance(value, tuple):
-        return f"({', '.join(format_query_value(x, server_tz) for x in value)})"
+        return f"({', '.join(str_query_value(x, server_tz) for x in value)})"
     if isinstance(value, dict):
         if common.get_setting('dict_parameter_format') == 'json':
             return format_str(any_to_json(value).decode())
-        pairs = [format_query_value(k, server_tz) + ':' + format_query_value(v, server_tz)
+        pairs = [str_query_value(k, server_tz) + ':' + str_query_value(v, server_tz)
                  for k, v in value.items()]
         return f"{{{', '.join(pairs)}}}"
     if isinstance(value, Enum):
         return format_query_value(value.value, server_tz)
     if isinstance(value, (uuid.UUID, ipaddress.IPv4Address, ipaddress.IPv6Address)):
         return f"'{value}'"
-    return str(value)
+    return value
+
+
+def str_query_value(value: Any, server_tz: tzinfo = pytz.UTC):
+    return str(format_query_value(value, server_tz))
 
 
 # pylint: disable=too-many-branches
 def format_bind_value(value: Any, server_tz: tzinfo = pytz.UTC, top_level: bool = True):
     """
     Format Python values in a ClickHouse query
     :param value: Python object
@@ -430,16 +437,15 @@
         return '\\N'
     if isinstance(value, str):
         if top_level:
             # At the top levels, strings must not be surrounded by quotes
             return escape_str(value)
         return format_str(value)
     if isinstance(value, datetime):
-        if value.tzinfo is None:
-            value = value.replace(tzinfo=server_tz)
+        value = value.astimezone(server_tz)
         val = value.strftime('%Y-%m-%d %H:%M:%S')
         if top_level:
             return val
         return f"'{val}'"
     if isinstance(value, date):
         if top_level:
             return value.isoformat()
@@ -484,13 +490,19 @@
 
 def to_arrow(content: bytes):
     pyarrow = check_arrow()
     reader = pyarrow.ipc.RecordBatchFileReader(content)
     return reader.read_all()
 
 
+def to_arrow_batches(buffer: IOBase) -> StreamContext:
+    pyarrow = check_arrow()
+    reader = pyarrow.ipc.open_stream(buffer)
+    return StreamContext(buffer, reader)
+
+
 def arrow_buffer(table) -> Tuple[Sequence[str], bytes]:
     pyarrow = check_arrow()
     sink = pyarrow.BufferOutputStream()
     with pyarrow.RecordBatchFileWriter(sink, table.schema) as writer:
         writer.write(table)
     return table.schema.names, sink.getvalue()
```

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/summary.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/summary.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/tools.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,20 @@
                 table: str,
                 file_path: str,
                 fmt: Optional[str] = None,
                 column_names: Optional[Sequence[str]] = None,
                 database: Optional[str] = None,
                 settings: Optional[Dict[str, Any]] = None,
                 compression: Optional[str] = None) -> QuerySummary:
-    full_table = f'{quote_identifier(database)}.{quote_identifier(table)}' if database else quote_identifier(table)
+    if not database and table[0] not in ('`', "'") and table.find('.') > 0:
+        full_table = table
+    elif database:
+        full_table = f'{quote_identifier(database)}.{quote_identifier(table)}'
+    else:
+        full_table = quote_identifier(table)
     if not fmt:
         fmt = 'CSV' if column_names else 'CSVWithNames'
     if compression is None:
         if file_path.endswith('.gzip') or file_path.endswith('.gz'):
             compression = 'gzip'
     with open(file_path, 'rb') as file:
         return client.raw_insert(full_table,
```

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/transform.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,18 +89,20 @@
         def chunk_gen():
             for block in context.next_block():
                 output = bytearray()
                 output += block.prefix
                 write_leb128(block.column_count, output)
                 write_leb128(block.row_count, output)
                 for col_name, col_type, data in zip(block.column_names, block.column_types, block.column_data):
-                    write_leb128(len(col_name), output)
-                    output += col_name.encode()
-                    write_leb128(len(col_type.name), output)
-                    output += col_type.name.encode()
+                    col_enc = col_name.encode()
+                    write_leb128(len(col_enc), output)
+                    output += col_enc
+                    col_enc = col_type.name.encode()
+                    write_leb128(len(col_enc), output)
+                    output += col_enc
                     context.start_column(col_name)
                     try:
                         col_type.write_column(data, output, context)
                     except Exception as ex:  # pylint: disable=broad-except
                         # This is hideous, but some low level serializations can fail while streaming
                         # the insert if the user has included bad data in the column.  We need to ensure that the
                         # insert fails (using garbage data) to avoid a partial insert, and use the context to
```

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driver/types.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driver/types.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driverc/buffer.pxd` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driverc/buffer.pxd`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driverc/buffer.pyx` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driverc/buffer.pyx`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/driverc/dataconv.pyx` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/driverc/dataconv.pyx`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/entry_points.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/entry_points.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/json_impl.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/json_impl.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/tools/datagen.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/tools/datagen.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect/tools/testing.py` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect/tools/testing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 from typing import Sequence, Optional, Union, Dict, Any
 
 from clickhouse_connect.driver import Client
-from clickhouse_connect.driver.query import format_query_value, quote_identifier
+from clickhouse_connect.driver.query import quote_identifier, str_query_value
 
 
 class TableContext:
     def __init__(self, client: Client,
                  table: str,
                  columns: Union[str, Sequence[str]],
                  column_types: Optional[Sequence[str]] = None,
                  engine: str = 'MergeTree',
                  order_by: str = None,
                  settings: Optional[Dict[str, Any]] = None):
         self.client = client
-        self.table = table
+        if '.' in table:
+            self.table = table
+        else:
+            self.table = quote_identifier(table)
         self.settings = settings
         if isinstance(columns, str):
             columns = columns.split(',')
         if column_types is None:
             self.column_names = []
             self.column_types = []
             for col in columns:
                 col = col.strip()
                 ix = col.find(' ')
                 self.column_types.append(col[ix + 1:].strip())
-                self.column_names.append(col[:ix].strip())
+                self.column_names.append(quote_identifier(col[:ix].strip()))
         else:
-            self.column_names = columns
+            self.column_names = [quote_identifier(name) for name in columns]
             self.column_types = column_types
         self.engine = engine
-        self.order_by = quote_identifier(self.column_names[0]) if order_by is None else order_by
+        self.order_by = self.column_names[0] if order_by is None else order_by
 
     def __enter__(self):
         if self.client.min_version('19'):
             self.client.command(f'DROP TABLE IF EXISTS {self.table}')
         else:
             self.client.command(f'DROP TABLE IF EXISTS {self.table} SYNC')
         col_defs = ','.join(f'{quote_identifier(name)} {col_type}' for name, col_type in zip(self.column_names, self.column_types))
         create_cmd = f'CREATE TABLE {self.table} ({col_defs}) ENGINE {self.engine} ORDER BY {self.order_by}'
         if self.settings:
             create_cmd += ' SETTINGS '
             for key, value in self.settings.items():
-
-                create_cmd += f'{key} = {format_query_value(value)}, '
+                create_cmd += f'{key} = {str_query_value(value)}, '
             if create_cmd.endswith(', '):
                 create_cmd = create_cmd[:-2]
         self.client.command(create_cmd)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.client.command(f'DROP TABLE IF EXISTS {self.table}')
```

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect_micropip.egg-info/PKG-INFO` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect_micropip.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: clickhouse-connect-micropip
-Version: 0.7.0
+Version: 0.7.10
 Summary: ClickHouse Database Core Driver for Python, Pandas, and Superset
 Home-page: https://github.com/ClickHouse/clickhouse-connect
 Author: ClickHouse Inc.
 Author-email: clients@clickhouse.com
 License: Apache License 2.0
 Keywords: clickhouse,superset,sqlalchemy,http,driver
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: certifi
 Requires-Dist: urllib3>=1.26
 Requires-Dist: pytz
 Requires-Dist: zstandard
@@ -28,14 +29,16 @@
 Requires-Dist: numpy; extra == "numpy"
 Provides-Extra: pandas
 Requires-Dist: pandas; extra == "pandas"
 Provides-Extra: arrow
 Requires-Dist: pyarrow; extra == "arrow"
 Provides-Extra: orjson
 Requires-Dist: orjson; extra == "orjson"
+Provides-Extra: tzlocal
+Requires-Dist: tzlocal; extra == "tzlocal"
 
 ## ClickHouse Connect
 
 A high performance core database driver for connecting ClickHouse to Python, Pandas, and Superset
 * Pandas DataFrames
 * Numpy Arrays
 * PyArrow Tables
```

### Comparing `clickhouse-connect-micropip-0.7.0/clickhouse_connect_micropip.egg-info/SOURCES.txt` & `clickhouse_connect_micropip-0.7.10/clickhouse_connect_micropip.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 clickhouse_connect/driver/options.py
 clickhouse_connect/driver/parser.py
 clickhouse_connect/driver/query.py
 clickhouse_connect/driver/summary.py
 clickhouse_connect/driver/tools.py
 clickhouse_connect/driver/transform.py
 clickhouse_connect/driver/types.py
+clickhouse_connect/driver/tzutil.py
 clickhouse_connect/driverc/__init__.pxd
 clickhouse_connect/driverc/__init__.py
 clickhouse_connect/driverc/buffer.pxd
 clickhouse_connect/driverc/buffer.pyx
 clickhouse_connect/driverc/dataconv.pyx
 clickhouse_connect/driverc/npconv.pyx
 clickhouse_connect/tools/__init__.py
```

### Comparing `clickhouse-connect-micropip-0.7.0/setup.py` & `clickhouse_connect_micropip-0.7.10/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,17 +33,18 @@
 
     version = 'development'
     if os.path.isfile('.dev_version'):
         with open(os.path.join(project_dir, '.dev_version'), encoding='utf-8') as version_file:
             version = version_file.readline()
     else:
         with open(os.path.join(project_dir, 'clickhouse_connect', '__version__.py'), encoding='utf-8') as version_file:
-            match = re.search(r"version\s*=\s*'(.+)'", version_file.read().strip())
+            file_version = version_file.read().strip()
+            match = re.search(r"version\s*=\s*'(.+)'", file_version)
             if match is None:
-                raise ValueError(f'invalid version in clickhouse_connect/__version__.py')
+                raise ValueError(f'invalid version {file_version} in clickhouse_connect/__version__.py')
             version = match.group(1)
 
     setup(
         name='clickhouse-connect-micropip',
         author='ClickHouse Inc.',
         author_email='clients@clickhouse.com',
         keywords=['clickhouse', 'superset', 'sqlalchemy', 'http', 'driver'],
@@ -65,31 +66,34 @@
         ],
         extras_require={
             'sqlalchemy': ['sqlalchemy>1.3.21,<2.0'],
             'numpy': ['numpy'],
             'pandas': ['pandas'],
             'arrow': ['pyarrow'],
             'orjson': ['orjson'],
+            'tzlocal': ['tzlocal'],
         },
         tests_require=['pytest'],
         entry_points={
             'sqlalchemy.dialects': ['clickhousedb.connect=clickhouse_connect.cc_sqlalchemy.dialect:ClickHouseDialect',
                                     'clickhousedb=clickhouse_connect.cc_sqlalchemy.dialect:ClickHouseDialect']
         },
         classifiers=[
             'Development Status :: 4 - Beta',
             'Intended Audience :: Developers',
             'License :: OSI Approved :: Apache Software License',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
-            'Programming Language :: Python :: 3.11'
+            'Programming Language :: Python :: 3.11',
+            'Programming Language :: Python :: 3.12',
         ],
         **kwargs
     )
 
 
 try:
     run_setup()
+# pylint: disable=broad-exception-caught
 except (Exception, IOError, SystemExit) as e:
     print(f'Unable to compile C extensions for faster performance due to {e}, will use pure Python')
     run_setup(False)
```


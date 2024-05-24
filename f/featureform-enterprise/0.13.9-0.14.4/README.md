# Comparing `tmp/featureform_enterprise-0.13.9.tar.gz` & `tmp/featureform_enterprise-0.14.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featureform_enterprise-0.13.9.tar", last modified: Fri May 17 20:04:10 2024, max compression
+gzip compressed data, was "featureform_enterprise-0.14.4.tar", last modified: Fri May 24 16:18:02 2024, max compression
```

## Comparing `featureform_enterprise-0.13.9.tar` & `featureform_enterprise-0.14.4.tar`

### file list

```diff
@@ -1,411 +1,411 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.646153 featureform_enterprise-0.13.9/
--rw-r--r--   0 runner    (1001) docker     (127)    16724 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-17 20:04:10.646153 featureform_enterprise-0.13.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-17 20:04:10.650153 featureform_enterprise-0.13.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.562153 featureform_enterprise-0.13.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.570153 featureform_enterprise-0.13.9/src/featureform/
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    38222 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.562153 featureform_enterprise-0.13.9/src/featureform/dashboard/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.570153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/
--rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/404.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.570153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/[type]/
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/[type]/[entity].html
--rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/[type].html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.562153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.562153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.570153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.618153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (127)    83441 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/72a30a16.feed22892a5cf9b7.js
--rw-r--r--   0 runner    (1001) docker     (127)    73108 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/7679.f81bbdabe01d6434.js
--rw-r--r--   0 runner    (1001) docker     (127)    21477 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/7856.a10f149ec0da2cc4.js
--rw-r--r--   0 runner    (1001) docker     (127)   199780 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.8aaacf4430f8899f.js
--rw-r--r--   0 runner    (1001) docker     (127)   130088 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/framework-f44ba79936f400b5.js
--rw-r--r--   0 runner    (1001) docker     (127)   108180 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/main-b492e665e4469b62.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.626153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/404-8d282ae638ce5722.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.626153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-2f83fe1ff7f9d94c.js
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/[type]-7bfcb609b1affd61.js
--rw-r--r--   0 runner    (1001) docker     (127)  4255345 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/_app-574fe43e4223620b.js
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/_error-e18771d792fd8fe7.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.626153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.626153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/
--rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/[groupName]-4ba8b6abfb4b13ca.js
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.626153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/
--rw-r--r--   0 runner    (1001) docker     (127)    17357 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/[roleName]-a4f4cefefad41418.js
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/roles-a560426c6514c003.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.626153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/
--rw-r--r--   0 runner    (1001) docker     (127)    11061 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/[userName]-5a66d4c05c9e7453.js
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/connections-f98076127418a04b.js
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/index-142e8557e4889163.js
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/query-5a171bd499b8d4eb.js
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/search-abfa6bb494904a10.js
--rw-r--r--   0 runner    (1001) docker     (127)    13985 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/tasks-70243ca2c0452223.js
--rw-r--r--   0 runner    (1001) docker     (127)    91460 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.626153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/
--rw-r--r--   0 runner    (1001) docker     (127)    35573 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.9d4c892d6ec3e998.js
--rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.1110d811936eb535.js
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.1cceaa6cbbc063ac.js
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.eb2d7c5e73071e92.js
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.7cda0a8b4fd10c8e.js
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.d3bb3d49b9c1d80b.js
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.a8dc93d57de022d3.js
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.5c26573759f9c121.js
--rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.7c2ee867e260f0e7.js
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.b157974fb0a5a751.js
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.5b503b684163ddee.js
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.3767e3821cef0636.js
--rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.588ecfde90e6c6a6.js
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arff.7b558400037bbf48.js
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.b830bba5a58a571f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.e5835ab195bd9150.js
--rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.c9f609621defe122.js
--rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.cbb253b90d4065f6.js
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.12fc5c16e5a165ee.js
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.24015a609992c2a0.js
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.a83f04a28cfc5c13.js
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.95f68b8f15b82829.js
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.e02e26748402cb2f.js
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.a21b937dd852d3c5.js
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bnf.79939abf3c1e11a8.js
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brainfuck.dbf25fee2d30d81a.js
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.f36b9b8a53d85766.js
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.51b85e9ce6ac77e9.js
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.0f747e26266b02a2.js
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.0dcb315084b7163e.js
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.b594f920dc05a67e.js
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.588914f5988d8070.js
--rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.ee070d344f3affd6.js
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.1cb9d96b33822dc8.js
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.0d5ec818ecef9324.js
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.628102c989f49555.js
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.d2924ae4e73b1223.js
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.3f60a647075d636f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.24b8d9cafb06d199.js
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.8c0ef98ac4f8e8a2.js
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.40ae09135f82f50e.js
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.8aaf8e216bf41dfe.js
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.841bb10e71e1c449.js
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.bc56944969bce274.js
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.ca9c2b431c04ca17.js
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.b5f4b6f514528d1d.js
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.3b8da30965ace8d0.js
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.a4e379d50aabc89d.js
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.31cb364f97f4e824.js
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.e13b9d3271de18f9.js
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.e2654a73b0584dec.js
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_editorconfig.503837d41162f24d.js
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.da3b3e0fae942646.js
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.399f0ab013510453.js
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a7425f8edef285f7.js
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.155ab93349c67ccd.js
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.c6479c75f219ea50.js
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.58f937c9dbd9989e.js
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.a021feea122d3ab8.js
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.15c4fc0252344391.js
--rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.746dde9caa36bd3a.js
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.7866c582058e46fd.js
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.7724b491752c429c.js
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.d1dd2d2dd76819de.js
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.c6da2507c50d21c4.js
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.d3fa954b1b6c7ddf.js
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gcode.9a929c1c9b2638ee.js
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.a7092d9f281d4e48.js
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.8ccf09a496d63a6f.js
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1d47fcfbbb4f7aae.js
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_git.1f58545eb203e18f.js
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.63e1bd7540f5f024.js
--rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.ec6db56efdb346a0.js
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e29c5a5287592d58.js
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.d0376c6facb31ca5.js
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.b47b77184d88114f.js
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.78c84ccf0f96ba85.js
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.c75feab6b678db77.js
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.508502701a02090a.js
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.d426610fe97ba28f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f181bbcd52749298.js
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.75b381c93a6b3e68.js
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hpkp.5a6e695471cb4195.js
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hsts.e90979a55a3b2795.js
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.16f39c180893252d.js
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.650dab668c7e4fd7.js
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.64a2195a59fd1547.js
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.80cf156f114fd8cf.js
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.b64600096e2ca9ed.js
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.01d852003dbb136c.js
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.5aae66009f81a97f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.f89efc1289945c39.js
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.da89585e43cc625e.js
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.c33d2207767fa3ea.js
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.dffcd987fd2af796.js
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.9a225e869035cf5e.js
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.33073eaf6ea575b1.js
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.bb74c766d6f802c5.js
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.746cbe8d4f665f4e.js
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.cfac9943bd3aa8c6.js
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.8b59c21ed9aa0df8.js
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e3cb4a5604d89cfa.js
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.12cb2d9917a6aab2.js
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.a3b5dc1c4d26ae4c.js
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsonp.cb40bb8da99d6066.js
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.a43af9cbcc3d056e.js
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.fb4387bc9a5ead37.js
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.794412054be66c77.js
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.47962934ccb42723.js
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.0df6c8ce29df587c.js
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.40eef7387c672247.js
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.c777981c76bf526a.js
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.80fd5c9b26494fb4.js
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b0db7f0ee3f15673.js
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.8b1345b4f614c39f.js
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.31982856fa816d70.js
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.f17164273275fd38.js
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.2f587faa9c12f894.js
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.02e16f89cc645033.js
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.dd5a243970406aba.js
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.acb704c99ae042b7.js
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.52a0bfb16d6c2b98.js
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.9a0f06e32359ab5f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.69a4a948327f0b94.js
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.8c3fb04cf18de9ad.js
--rw-r--r--   0 runner    (1001) docker     (127)    16943 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.fdc98b1cdb606d74.js
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.8fca60ed2df5e72a.js
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.c6bd9f3fa6de96e2.js
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.74938f19e891fdf5.js
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.fc51859d62024c0c.js
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.722d26c11b333d29.js
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a9e892235dc65f7b.js
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.a38fd3d408351597.js
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.374dabbd7a65bb7e.js
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.79a60949255a30ef.js
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b8f96e57ccaae943.js
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.c394be68ff73cffa.js
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.2017f4173ae7ddfb.js
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.b409945670f221f7.js
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.83a26a43f4df0850.js
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.51aa798f8d7e5f9d.js
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.67ac42fc89d5c984.js
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.83317f3b3977639c.js
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.b5b55f9072af7a5d.js
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.859e58b02983b520.js
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.478f7d5866f2865d.js
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.7494238f7c6ad706.js
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.199e2ba708699dcb.js
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.98e2ba9a44a80b8d.js
--rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.36058e7553ffa345.js
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.48de1152e01ba572.js
--rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.7a521a109d6461ca.js
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.c091a192bf82f926.js
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.badf407c7a6f2db0.js
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.213c3d6af366a76e.js
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.93772d4fe83877f5.js
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_prolog.a271ae92c5d426c4.js
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_properties.bb3235d2b44fb9b3.js
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.3a384d03bec6f703.js
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.9cdb03119b332984.js
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.e79ec6009494dfce.js
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.7766acfcd5f91811.js
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.e0ae21e641671328.js
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.26d85ff3fe699cbb.js
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.f36a4d3fb726f719.js
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.fcda67b8e3d7ff14.js
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.72882aebe76845de.js
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.2e295de118cafdef.js
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.e1cdb5c5cec33e2e.js
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.7e7c3d8167ac74f6.js
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.790c6f46fa4e9d8b.js
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.1f694c1ce3fcc4d1.js
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.3aa230ff56d754c5.js
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.ae739446f2d00124.js
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.e221063f635f2e9f.js
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.e3b79e7ad6d1e67b.js
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.67dc98b63dd3081e.js
--rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.49c692f8bc2d227f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.60d8ff3f62a0dde3.js
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.241341676d07c7c5.js
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.edc1a3543d37dac7.js
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.2ae7f1f871d749d9.js
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.11864bd2178e2c08.js
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.cf7ba940ae593d96.js
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.d61bc93d9240911c.js
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.7dc2e8495b82afa0.js
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.cc6c20111eef392b.js
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.28dda31a087b27dc.js
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.2a65ffecac1e4433.js
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.f3ac4fdc10100a71.js
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.e5cbb81e295d94aa.js
--rw-r--r--   0 runner    (1001) docker     (127)    33526 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.8fd37bd46bcdef8e.js
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.021da63363b275e2.js
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.7047500798cae5bd.js
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.37b21bb61cb7da6e.js
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.987edd5fb1761cdf.js
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.f4f05ad29882de17.js
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.74a04f9bd98b3d92.js
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.63c6b3c7dbad89c3.js
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.a961a8a3e36733d2.js
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.5c35ca803e68095b.js
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.b314e238d6967a8f.js
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.1d0f9c7b17d4bc2b.js
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.790da421b54213dd.js
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.a9cf0d3dab52d046.js
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.8efe0bec8cec6f08.js
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.cfc4809f40a5b725.js
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2127ec25c75e4984.js
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.62a04a024d699193.js
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.f45aa85f3888e4f5.js
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.a26c328f4cf8b171.js
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.ea05c1dd27403a55.js
--rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.d6af4f6428d66d9a.js
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.74e478ac085e3404.js
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.92e6c66e598bc5b0.js
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.5be2e1ec1d76cc74.js
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.aa5faeff88cffc63.js
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.97f81f55c7dda273.js
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xmlDoc.b941e6f1f8370030.js
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.2eea9520afb8e6ea.js
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.df4e0a4839a040a1.js
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.e1a7f78fb87ff37c.js
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yang.758f2e9ec02ed81c.js
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.4ddc9ac973a0065e.js
--rw-r--r--   0 runner    (1001) docker     (127)    22536 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/webpack-4ca33bb86fc5510e.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.626153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/css/85a2addfd2efc882.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.626153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)    81048 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.630153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.630153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.630153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/yVmVSX0ksIXzzxWh3Ff_1/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.630153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.630153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/group/
--rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/group/[groupName].html
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/groups.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.630153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/role/
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/role/[roleName].html
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/roles.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.630153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/user/
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/user/[userName].html
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/users.html
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/connections.html
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/query.html
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/search.html
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.638153 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Apache_Spark_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Capital_One_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_White.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Featureform_logo_pink.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Kubernetes_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Postgresql_elephant.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Redis_Logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Snowflake_Logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/amazon_dynamoDB.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/amazon_redshift.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/amazon_s3.svg
--rw-r--r--   0 runner    (1001) docker     (127)    26573 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/apache_cassandra.svg
--rw-r--r--   0 runner    (1001) docker     (127)    60161 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/apache_hadoop.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/azure_storage_accounts.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/base_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/clearIcon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/clickhouse-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    35853 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/creature.png
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/file_store.svg
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/google_bigquery.svg
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/google_cloud_storage.svg
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/google_firestore.svg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/localmode.png
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/logo192.png
--rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/logo512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/mongoDB.svg
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/offline_store.svg
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/online_store.svg
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/owner_bubble.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (127)   175958 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/welcomebackground.png
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-17 20:04:06.000000 featureform_enterprise-0.13.9/src/featureform/dashboard/out/tasks.html
--rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/grpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.638153 featureform_enterprise-0.13.9/src/featureform/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18213 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/lib/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.642153 featureform_enterprise-0.13.9/src/featureform/proto/
--rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-17 20:03:16.000000 featureform_enterprise-0.13.9/src/featureform/proto/metadata.proto
--rw-r--r--   0 runner    (1001) docker     (127)    31926 2024-05-17 20:03:17.000000 featureform_enterprise-0.13.9/src/featureform/proto/metadata_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    60934 2024-05-17 20:03:17.000000 featureform_enterprise-0.13.9/src/featureform/proto/metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   112884 2024-05-17 20:03:17.000000 featureform_enterprise-0.13.9/src/featureform/proto/metadata_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-17 20:03:16.000000 featureform_enterprise-0.13.9/src/featureform/proto/serving.proto
--rw-r--r--   0 runner    (1001) docker     (127)    10160 2024-05-17 20:03:17.000000 featureform_enterprise-0.13.9/src/featureform/proto/serving_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-05-17 20:03:17.000000 featureform_enterprise-0.13.9/src/featureform/proto/serving_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16586 2024-05-17 20:03:17.000000 featureform_enterprise-0.13.9/src/featureform/proto/serving_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)   203902 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/register.py
--rw-r--r--   0 runner    (1001) docker     (127)    84275 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    30878 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/serving.py
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/status_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/tls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/train_test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/type_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    33892 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/variant_names_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/src/featureform/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.646153 featureform_enterprise-0.13.9/src/featureform_enterprise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-17 20:04:10.000000 featureform_enterprise-0.13.9/src/featureform_enterprise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    34961 2024-05-17 20:04:10.000000 featureform_enterprise-0.13.9/src/featureform_enterprise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 20:04:10.000000 featureform_enterprise-0.13.9/src/featureform_enterprise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-17 20:04:10.000000 featureform_enterprise-0.13.9/src/featureform_enterprise.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-17 20:04:10.000000 featureform_enterprise-0.13.9/src/featureform_enterprise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 20:04:10.000000 featureform_enterprise-0.13.9/src/featureform_enterprise.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:04:10.646153 featureform_enterprise-0.13.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_autogenerated_variants.py
--rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_class_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    43785 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_executor_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_getting_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_multi_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_ondemand_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_resource_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    14620 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_serving_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_source_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_source_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_spark_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    28897 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_tags_and_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_train_test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_training_set_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-17 20:02:30.000000 featureform_enterprise-0.13.9/tests/test_updating_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.695352 featureform_enterprise-0.14.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    16724 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-24 16:18:02.695352 featureform_enterprise-0.14.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-24 16:18:02.695352 featureform_enterprise-0.14.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.547352 featureform_enterprise-0.14.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.555352 featureform_enterprise-0.14.4/src/featureform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40209 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.543352 featureform_enterprise-0.14.4/src/featureform/dashboard/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.559352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/404.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.559352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/[type]/
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/[type]/[entity].html
+-rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/[type].html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.543352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.547352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.559352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.627352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (127)    83441 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/72a30a16.feed22892a5cf9b7.js
+-rw-r--r--   0 runner    (1001) docker     (127)    73108 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/7679.f81bbdabe01d6434.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21477 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/7856.a10f149ec0da2cc4.js
+-rw-r--r--   0 runner    (1001) docker     (127)   199780 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.8aaacf4430f8899f.js
+-rw-r--r--   0 runner    (1001) docker     (127)   130088 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/framework-f44ba79936f400b5.js
+-rw-r--r--   0 runner    (1001) docker     (127)   108180 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/main-b492e665e4469b62.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.639352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/404-8d282ae638ce5722.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.639352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-2f83fe1ff7f9d94c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/[type]-7bfcb609b1affd61.js
+-rw-r--r--   0 runner    (1001) docker     (127)  4257430 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/_app-569252d467889e35.js
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/_error-e18771d792fd8fe7.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.643352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.643352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/
+-rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/[groupName]-4ba8b6abfb4b13ca.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.643352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/
+-rw-r--r--   0 runner    (1001) docker     (127)    17357 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/[roleName]-a4f4cefefad41418.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/admin/roles-a560426c6514c003.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.643352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/
+-rw-r--r--   0 runner    (1001) docker     (127)    11061 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/[userName]-5a66d4c05c9e7453.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/connections-f98076127418a04b.js
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/index-142e8557e4889163.js
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/query-5a171bd499b8d4eb.js
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/search-abfa6bb494904a10.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13985 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/tasks-70243ca2c0452223.js
+-rw-r--r--   0 runner    (1001) docker     (127)    91460 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.643352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/
+-rw-r--r--   0 runner    (1001) docker     (127)    35573 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.9d4c892d6ec3e998.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.1110d811936eb535.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.1cceaa6cbbc063ac.js
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.eb2d7c5e73071e92.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.7cda0a8b4fd10c8e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.d3bb3d49b9c1d80b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.a8dc93d57de022d3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.5c26573759f9c121.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.7c2ee867e260f0e7.js
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.b157974fb0a5a751.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.5b503b684163ddee.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.3767e3821cef0636.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.588ecfde90e6c6a6.js
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arff.7b558400037bbf48.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.b830bba5a58a571f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.e5835ab195bd9150.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.c9f609621defe122.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.cbb253b90d4065f6.js
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.12fc5c16e5a165ee.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.24015a609992c2a0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.a83f04a28cfc5c13.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.95f68b8f15b82829.js
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.e02e26748402cb2f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.a21b937dd852d3c5.js
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bnf.79939abf3c1e11a8.js
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brainfuck.dbf25fee2d30d81a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.f36b9b8a53d85766.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.51b85e9ce6ac77e9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.0f747e26266b02a2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.0dcb315084b7163e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.b594f920dc05a67e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.588914f5988d8070.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.ee070d344f3affd6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.1cb9d96b33822dc8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.0d5ec818ecef9324.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.628102c989f49555.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.d2924ae4e73b1223.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.3f60a647075d636f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.24b8d9cafb06d199.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.8c0ef98ac4f8e8a2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.40ae09135f82f50e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.8aaf8e216bf41dfe.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.841bb10e71e1c449.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.bc56944969bce274.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.ca9c2b431c04ca17.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.b5f4b6f514528d1d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.3b8da30965ace8d0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.a4e379d50aabc89d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.31cb364f97f4e824.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.e13b9d3271de18f9.js
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.e2654a73b0584dec.js
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_editorconfig.503837d41162f24d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.da3b3e0fae942646.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.399f0ab013510453.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a7425f8edef285f7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.155ab93349c67ccd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.c6479c75f219ea50.js
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.58f937c9dbd9989e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.a021feea122d3ab8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.15c4fc0252344391.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.746dde9caa36bd3a.js
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.7866c582058e46fd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.7724b491752c429c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.d1dd2d2dd76819de.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.c6da2507c50d21c4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.d3fa954b1b6c7ddf.js
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gcode.9a929c1c9b2638ee.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.a7092d9f281d4e48.js
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.8ccf09a496d63a6f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1d47fcfbbb4f7aae.js
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_git.1f58545eb203e18f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.63e1bd7540f5f024.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.ec6db56efdb346a0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e29c5a5287592d58.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.d0376c6facb31ca5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.b47b77184d88114f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.78c84ccf0f96ba85.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.c75feab6b678db77.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.508502701a02090a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.d426610fe97ba28f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f181bbcd52749298.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.75b381c93a6b3e68.js
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hpkp.5a6e695471cb4195.js
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hsts.e90979a55a3b2795.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.16f39c180893252d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.650dab668c7e4fd7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.64a2195a59fd1547.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.80cf156f114fd8cf.js
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.b64600096e2ca9ed.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.01d852003dbb136c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.5aae66009f81a97f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.f89efc1289945c39.js
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.da89585e43cc625e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.c33d2207767fa3ea.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.dffcd987fd2af796.js
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.9a225e869035cf5e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.33073eaf6ea575b1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.bb74c766d6f802c5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.746cbe8d4f665f4e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.cfac9943bd3aa8c6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.8b59c21ed9aa0df8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e3cb4a5604d89cfa.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.12cb2d9917a6aab2.js
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.a3b5dc1c4d26ae4c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsonp.cb40bb8da99d6066.js
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.a43af9cbcc3d056e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.fb4387bc9a5ead37.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.794412054be66c77.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.47962934ccb42723.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.0df6c8ce29df587c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.40eef7387c672247.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.c777981c76bf526a.js
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.80fd5c9b26494fb4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b0db7f0ee3f15673.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.8b1345b4f614c39f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.31982856fa816d70.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.f17164273275fd38.js
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.2f587faa9c12f894.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.02e16f89cc645033.js
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.dd5a243970406aba.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.acb704c99ae042b7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.52a0bfb16d6c2b98.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.9a0f06e32359ab5f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.69a4a948327f0b94.js
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.8c3fb04cf18de9ad.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16943 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.fdc98b1cdb606d74.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.8fca60ed2df5e72a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.c6bd9f3fa6de96e2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.74938f19e891fdf5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.fc51859d62024c0c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.722d26c11b333d29.js
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a9e892235dc65f7b.js
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.a38fd3d408351597.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.374dabbd7a65bb7e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.79a60949255a30ef.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b8f96e57ccaae943.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.c394be68ff73cffa.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.2017f4173ae7ddfb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.b409945670f221f7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.83a26a43f4df0850.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.51aa798f8d7e5f9d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.67ac42fc89d5c984.js
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.83317f3b3977639c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.b5b55f9072af7a5d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.859e58b02983b520.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.478f7d5866f2865d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.7494238f7c6ad706.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.199e2ba708699dcb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.98e2ba9a44a80b8d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.36058e7553ffa345.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.48de1152e01ba572.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.7a521a109d6461ca.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.c091a192bf82f926.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.badf407c7a6f2db0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.213c3d6af366a76e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.93772d4fe83877f5.js
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_prolog.a271ae92c5d426c4.js
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_properties.bb3235d2b44fb9b3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.3a384d03bec6f703.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.9cdb03119b332984.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.e79ec6009494dfce.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.7766acfcd5f91811.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.e0ae21e641671328.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.26d85ff3fe699cbb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.f36a4d3fb726f719.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.fcda67b8e3d7ff14.js
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.72882aebe76845de.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.2e295de118cafdef.js
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.e1cdb5c5cec33e2e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.7e7c3d8167ac74f6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.790c6f46fa4e9d8b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.1f694c1ce3fcc4d1.js
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.3aa230ff56d754c5.js
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.ae739446f2d00124.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.e221063f635f2e9f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.e3b79e7ad6d1e67b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.67dc98b63dd3081e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.49c692f8bc2d227f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.60d8ff3f62a0dde3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.241341676d07c7c5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.edc1a3543d37dac7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.2ae7f1f871d749d9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.11864bd2178e2c08.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.cf7ba940ae593d96.js
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.d61bc93d9240911c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.7dc2e8495b82afa0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.cc6c20111eef392b.js
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.28dda31a087b27dc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.2a65ffecac1e4433.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.f3ac4fdc10100a71.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.e5cbb81e295d94aa.js
+-rw-r--r--   0 runner    (1001) docker     (127)    33526 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.8fd37bd46bcdef8e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.021da63363b275e2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.7047500798cae5bd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.37b21bb61cb7da6e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.987edd5fb1761cdf.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.f4f05ad29882de17.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.74a04f9bd98b3d92.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.63c6b3c7dbad89c3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.a961a8a3e36733d2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.5c35ca803e68095b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.b314e238d6967a8f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.1d0f9c7b17d4bc2b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.790da421b54213dd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.a9cf0d3dab52d046.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.8efe0bec8cec6f08.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.cfc4809f40a5b725.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2127ec25c75e4984.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.62a04a024d699193.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.f45aa85f3888e4f5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.a26c328f4cf8b171.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.ea05c1dd27403a55.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.d6af4f6428d66d9a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.74e478ac085e3404.js
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.92e6c66e598bc5b0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.5be2e1ec1d76cc74.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.aa5faeff88cffc63.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.97f81f55c7dda273.js
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xmlDoc.b941e6f1f8370030.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.2eea9520afb8e6ea.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.df4e0a4839a040a1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.e1a7f78fb87ff37c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yang.758f2e9ec02ed81c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.4ddc9ac973a0065e.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22536 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/webpack-4ca33bb86fc5510e.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.647352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/css/85a2addfd2efc882.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.647352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    81048 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.647352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.647352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.647352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.651352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.651352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/admin/group/
+-rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/admin/group/[groupName].html
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/admin/groups.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.651352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/admin/role/
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/admin/role/[roleName].html
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/admin/roles.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.651352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/admin/user/
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/admin/user/[userName].html
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/admin/users.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/connections.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/query.html
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.671352 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/Apache_Spark_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/Capital_One_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_White.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/Featureform_logo_pink.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/Kubernetes_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/Postgresql_elephant.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/Redis_Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/Snowflake_Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/amazon_dynamoDB.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/amazon_redshift.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/amazon_s3.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    26573 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/apache_cassandra.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    60161 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/apache_hadoop.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/azure_storage_accounts.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/base_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/clearIcon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/clickhouse-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    35853 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/creature.png
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/file_store.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/google_bigquery.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/google_cloud_storage.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/google_firestore.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/localmode.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/mongoDB.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/offline_store.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/online_store.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/owner_bubble.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   175958 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/welcomebackground.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-24 16:17:57.000000 featureform_enterprise-0.14.4/src/featureform/dashboard/out/tasks.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/grpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.671352 featureform_enterprise-0.14.4/src/featureform/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19222 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/lib/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.679352 featureform_enterprise-0.14.4/src/featureform/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-24 16:17:03.000000 featureform_enterprise-0.14.4/src/featureform/proto/metadata.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    31926 2024-05-24 16:17:05.000000 featureform_enterprise-0.14.4/src/featureform/proto/metadata_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60934 2024-05-24 16:17:05.000000 featureform_enterprise-0.14.4/src/featureform/proto/metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   112884 2024-05-24 16:17:05.000000 featureform_enterprise-0.14.4/src/featureform/proto/metadata_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-24 16:17:03.000000 featureform_enterprise-0.14.4/src/featureform/proto/serving.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    10591 2024-05-24 16:17:04.000000 featureform_enterprise-0.14.4/src/featureform/proto/serving_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23537 2024-05-24 16:17:04.000000 featureform_enterprise-0.14.4/src/featureform/proto/serving_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-05-24 16:17:04.000000 featureform_enterprise-0.14.4/src/featureform/proto/serving_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)   205635 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84725 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31349 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/serving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/status_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/train_test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/type_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33892 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/variant_names_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/src/featureform/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.695352 featureform_enterprise-0.14.4/src/featureform_enterprise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-24 16:18:02.000000 featureform_enterprise-0.14.4/src/featureform_enterprise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    34961 2024-05-24 16:18:02.000000 featureform_enterprise-0.14.4/src/featureform_enterprise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 16:18:02.000000 featureform_enterprise-0.14.4/src/featureform_enterprise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 16:18:02.000000 featureform_enterprise-0.14.4/src/featureform_enterprise.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-24 16:18:02.000000 featureform_enterprise-0.14.4/src/featureform_enterprise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 16:18:02.000000 featureform_enterprise-0.14.4/src/featureform_enterprise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:02.695352 featureform_enterprise-0.14.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_autogenerated_variants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_class_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43785 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_executor_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_getting_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_multi_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_ondemand_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_resource_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14620 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_serving_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_source_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_source_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_spark_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28897 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_tags_and_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_train_test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_training_set_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-24 16:16:17.000000 featureform_enterprise-0.14.4/tests/test_updating_provider.py
```

### Comparing `featureform_enterprise-0.13.9/LICENSE` & `featureform_enterprise-0.14.4/LICENSE`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/PKG-INFO` & `featureform_enterprise-0.14.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featureform-enterprise
-Version: 0.13.9
+Version: 0.14.4
 Summary: Package for the Featureform Enterprise Feature Store
 Home-page: https://featureform.com
 Author: FeatureForm, Inc.
 Author-email: hello@featureform.com
 Project-URL: Bug Tracker, https://github.com/featureform/featureform/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -34,14 +34,15 @@
 Requires-Dist: fastparquet
 Requires-Dist: pinecone-client
 Requires-Dist: weaviate-client
 Requires-Dist: docker
 Requires-Dist: okta-jwt-verifier
 Requires-Dist: googleapis-common-protos
 Requires-Dist: uuid
+Requires-Dist: importlib-metadata
 
 # Featureform Python Client
 
 ## Overview
 
 Featureform’s Python client is a SDK for defining, managing and serving resources (e.g. infrastructure providers, data sources, transformations, etc.). At a high level, the API is divided into two parts:
```

### Comparing `featureform_enterprise-0.13.9/README.md` & `featureform_enterprise-0.14.4/README.md`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/setup.cfg` & `featureform_enterprise-0.14.4/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = featureform-enterprise
-version = 0.13.9
+version = 0.14.4
 author = FeatureForm, Inc.
 author_email = hello@featureform.com
 description = Package for the Featureform Enterprise Feature Store
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://featureform.com
 project_urls = 
@@ -43,14 +43,15 @@
 	fastparquet
 	pinecone-client
 	weaviate-client
 	docker
 	okta-jwt-verifier
 	googleapis-common-protos
 	uuid
+	importlib-metadata
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	featureform = featureform.cli:cli
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/__init__.py` & `featureform_enterprise-0.14.4/src/featureform/__init__.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/cli.py` & `featureform_enterprise-0.14.4/src/featureform/cli.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/client.py` & `featureform_enterprise-0.14.4/src/featureform/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datetime import datetime
 from typing import List, Optional, Union
 
 from google.protobuf.timestamp_pb2 import Timestamp
 from typeguard import typechecked
 
 from .constants import NO_RECORD_LIMIT
-from .enums import ResourceType
+from .enums import FileFormat, ResourceType
 from .lib import auth
 from .proto import metadata_pb2 as pb
 from .register import (
     FeatureColumnResource,
     FileStoreProvider,
     OfflineSQLProvider,
     OfflineSparkProvider,
@@ -117,14 +117,15 @@
     def dataframe(
         self,
         source: Union[
             SourceRegistrar, SubscriptableTransformation, ResourceVariant, str
         ],
         variant: Optional[str] = None,
         limit=NO_RECORD_LIMIT,
+        spark_session=None,
         asynchronous=False,
         verbose=False,
     ):
         """
         Return a dataframe from a registered source or transformation
 
         **Example:**
@@ -134,14 +135,15 @@
         avg_user_transaction_df = transactions_df.groupby("CustomerID")["TransactionAmount"].mean()
         ```
 
         Args:
             source (Union[SourceRegistrar, SubscriptableTransformation, str]): The source or transformation to compute the dataframe from
             variant (str): The source variant; can't be None if source is a string
             limit (int): The maximum number of records to return; defaults to NO_RECORD_LIMIT
+            spark_session: Specifices to read as a spark session.
             asynchronous (bool): Flag to determine whether the client should wait for resources to be in either a READY or FAILED state before returning. Defaults to False to ensure that newly registered resources are in a READY state prior to serving them as dataframes.
 
         Returns:
             df (pandas.DataFrame): The dataframe computed from the source or transformation
 
         """
         self.apply(asynchronous=asynchronous, verbose=verbose)
@@ -156,16 +158,66 @@
             if variant == "":
                 raise ValueError("variant cannot be an empty string")
         else:
             raise ValueError(
                 f"source must be of type SourceRegistrar, SubscriptableTransformation or str, not {type(source)}\n"
                 "use client.dataframe(name, variant) or client.dataframe(source) or client.dataframe(transformation)"
             )
+        if spark_session is not None:
+            if isinstance(source, str):
+                raise ValueError(
+                    "Name/variant strings not supported with spark session. Use object."
+                )
+            return self._spark_dataframe(source, spark_session)
         return self.impl._get_source_as_df(name, variant, limit)
 
+    # TODO, combine this with the dataset logic in serving.py
+    def _spark_dataframe(self, source, spark_session):
+        location = self.location(source)
+
+        # If the location is a part-file, we want to get the directory instead.
+        is_individual_part_file = location.split("/")[-1].startswith("part-")
+        if is_individual_part_file:
+            location = "/".join(location.split("/")[:-1])
+
+        # If the schema is s3://, we want to convert it to s3a://.
+        location = (
+            location.replace("s3://", "s3a://")
+            if location.startswith("s3://")
+            else location
+        )
+        file_format = FileFormat.get_format(location, default="parquet")
+        if file_format not in FileFormat.supported_formats():
+            raise Exception(
+                f"file type '{file_format}' is not supported. Please use 'csv' or 'parquet'"
+            )
+
+        try:
+            df = (
+                spark_session.read.option("header", "true")
+                .option("recursiveFileLookup", "true")
+                .format(file_format)
+                .load(location)
+            )
+
+            label_column_name = ""
+            for col in df.columns:
+                if col.startswith("Label__"):
+                    label_column_name = col
+                    break
+
+            if label_column_name != "":
+                df = df.withColumnRenamed(label_column_name, "Label")
+        except Exception as e:
+            raise Exception(
+                f"please make sure the spark session has ability to read '{location}': {e}"
+            )
+
+        return df
+
     def nearest(self, feature, vector, k):
         """
         Query the K nearest neighbors of a provider vector in the index of a registered feature variant
 
         **Example:**
 
         ```py title="definitions.py"
@@ -265,16 +317,16 @@
         Args:
             source (Union[SourceRegistrar, SubscriptableTransformation, str]): The source or transformation to compute the dataframe from
             variant (str): The source variant; can't be None if source is a string
             resource_type (ResourceType): The type of resource; can be one of ff.SOURCE, ff.FEATURE, ff.LABEL, or ff.TRAINING_SET
         """
         if isinstance(source, (SourceRegistrar, SubscriptableTransformation)):
             name, variant = source.name_variant()
-            resource_type = ResourceType.SOURCE
-        elif isinstance(source, featureform.resources.TrainingSetVariant):
+            resource_type = ResourceType.TRANSFORMATION
+        elif isinstance(source, TrainingSetVariant):
             name = source.name
             variant = source.variant
             resource_type = ResourceType.TRAINING_SET
         elif isinstance(source, str):
             name = source
             if variant is None:
                 raise ValueError("variant must be specified if source is a string")
@@ -284,15 +336,15 @@
             if resource_type is None:
                 raise ValueError(
                     "resource_type must be specified if source is a string"
                 )
 
         else:
             raise ValueError(
-                f"source must be of type SourceRegistrar, SubscriptableTransformation or str, not {type(resource)}\n"
+                f"source must be of type SourceRegistrar, SubscriptableTransformation or str, not {type(source)}\n"
                 "use client.dataframe(name, variant) or client.dataframe(source) or client.dataframe(transformation)"
             )
 
         location = self.impl.location(name, variant, resource_type)
         return location
 
     def close(self):
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/404.html` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/admin/users.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/404-8d282ae638ce5722.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-569252d467889e35.js" defer=""></script><script src="/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_buildManifest.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/404","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/users","query":{},"buildId":"tU2e0PPhQ-QR0Wjh2ilIZ","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/[type]/[entity].html` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D/%5Bentity%5D-2f83fe1ff7f9d94c.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-569252d467889e35.js" defer=""></script><script src="/_next/static/chunks/pages/index-142e8557e4889163.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_buildManifest.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]/[entity]","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"tU2e0PPhQ-QR0Wjh2ilIZ","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/[type].html` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/connections.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D-7bfcb609b1affd61.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-569252d467889e35.js" defer=""></script><script src="/_next/static/chunks/pages/connections-f98076127418a04b.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_buildManifest.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/connections","query":{},"buildId":"tU2e0PPhQ-QR0Wjh2ilIZ","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/72a30a16.feed22892a5cf9b7.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/72a30a16.feed22892a5cf9b7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/7679.f81bbdabe01d6434.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/7679.f81bbdabe01d6434.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/7856.a10f149ec0da2cc4.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/7856.a10f149ec0da2cc4.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.8aaacf4430f8899f.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.8aaacf4430f8899f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/framework-f44ba79936f400b5.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/framework-f44ba79936f400b5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/main-b492e665e4469b62.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/main-b492e665e4469b62.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-2f83fe1ff7f9d94c.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-2f83fe1ff7f9d94c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/_app-574fe43e4223620b.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/_app-569252d467889e35.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -97806,24 +97806,24 @@
                 })
             }, window.__NEXT_PRELOADREADY = h.preloadReady, a.default = h
         },
         22487: function(e, a, t) {
             "use strict";
             t.r(a), t.d(a, {
                 MyApp: function() {
-                    return eX
+                    return eQ
                 },
                 ThemeWrapper: function() {
-                    return e1
+                    return e0
                 },
                 default: function() {
-                    return e0
+                    return e2
                 },
                 views: function() {
-                    return eQ
+                    return e1
                 }
             });
             var n, r = t(99534),
                 i = t(85893),
                 o = t(66720),
                 l = t(69980),
                 s = t(33299),
@@ -98873,105 +98873,107 @@
                         a.meta.requestId === e.requestId && (e.loading = !1, e.failed = !0)
                     }), n)
                 });
             eK.actions.modifyInstances, eK.actions.modifyMetrics;
             var eG = eK.reducer;
             t(5813);
             var eF = (0, eg.oM)({
-                name: "homePageSections",
-                initialState: {
-                    features: [{
-                        type: "TrainingSet",
-                        disabled: !1
-                    }, {
-                        type: "Feature",
-                        disabled: !1
-                    }, {
-                        type: "Entity",
-                        disabled: !1
-                    }, {
-                        type: "Label",
-                        disabled: !1
-                    }, {
-                        type: "Model",
-                        disabled: !1
-                    }, {
-                        type: "Source",
-                        disabled: !1
-                    }, {
-                        type: "Provider",
-                        disabled: !1
-                    }]
-                }
-            }).reducer;
+                    name: "homePageSections",
+                    initialState: {
+                        features: [{
+                            type: "TrainingSet",
+                            disabled: !1
+                        }, {
+                            type: "Feature",
+                            disabled: !1
+                        }, {
+                            type: "Entity",
+                            disabled: !1
+                        }, {
+                            type: "Label",
+                            disabled: !1
+                        }, {
+                            type: "Model",
+                            disabled: !1
+                        }, {
+                            type: "Source",
+                            disabled: !1
+                        }, {
+                            type: "Provider",
+                            disabled: !1
+                        }]
+                    }
+                }).reducer,
+                eZ = t(61790);
             t(6518), t(88802);
-            var eZ = t(16332),
-                eV = t(5378),
-                eU = t(93432);
+            var eV = t(16332),
+                eU = t(5378),
+                eW = t(93432);
             t(85931);
-            var eW = t(75820),
-                eJ = (0, ex.UY)({
-                    resourceList: eZ.ZP,
-                    selectedVariant: eU.ZP,
-                    selectedTags: eV.ZP,
+            var eJ = t(75820),
+                eY = (0, ex.UY)({
+                    resourceList: eV.ZP,
+                    selectedVariant: eW.ZP,
+                    selectedTags: eU.ZP,
                     homePageSections: eF,
                     breadCrumbs: eb,
                     entityPage: eS.Z,
-                    searchResults: eW.ZP,
+                    searchResults: eJ.ZP,
                     timeRange: eI.Z,
                     metricsSelect: eG,
                     connectionStatus: ek.Z,
-                    aggregates: eN
+                    aggregates: eN,
+                    currentPage: eZ.ZP
                 }),
-                eY = (0, eg.xC)({
-                    reducer: eJ
+                eq = (0, eg.xC)({
+                    reducer: eY
                 }),
-                eq = function(e) {
+                e$ = function(e) {
                     var a = e.children,
                         t = e.store;
                     return (0, i.jsx)(P.zt, {
                         store: t,
                         children: a
                     })
                 };
             t(2989);
-            var e$ = t(48535),
-                eX = function(e) {
+            var eX = t(48535),
+                eQ = function(e) {
                     var a = e.Component,
                         t = e.pageProps.session,
                         n = (0, r.Z)(e.pageProps, ["session"]);
                     return (0, i.jsx)(u.StrictMode, {
                         children: (0, i.jsx)(s.SessionProvider, {
                             session: t,
-                            children: (0, i.jsx)(eq, {
-                                store: eY,
-                                children: (0, i.jsx)(e1, {
+                            children: (0, i.jsx)(e$, {
+                                store: eq,
+                                children: (0, i.jsx)(e0, {
                                     children: (0, i.jsx)(T, {
                                         children: (0, i.jsx)(ev, {
                                             Component: a,
                                             pageProps: n
                                         })
                                     })
                                 })
                             })
                         })
                     })
                 },
-                eQ = {
+                e1 = {
                     RESOURCE_LIST: "ResourceList",
                     EMPTY: "Empty"
                 },
-                e1 = function(e) {
+                e0 = function(e) {
                     var a = e.children;
                     return (0, i.jsxs)(l.Z, {
-                        theme: e$.ZP,
+                        theme: eX.ZP,
                         children: [(0, i.jsx)(o.ZP, {}), a]
                     })
                 },
-                e0 = eX
+                e2 = eQ
         },
         52672: function(e, a, t) {
             "use strict";
             t.d(a, {
                 T: function() {
                     return l
                 }
@@ -99203,23 +99205,28 @@
                                 }
                             })
                         })()
                     }
                 }, {
                     key: "fetchResources",
                     value: function(e) {
-                        var a, t = u.Z[e];
-                        return a = "".concat(m + "/data").concat(t.urlPath), "true" === c.env.REACT_APP_EMPTY_RESOURCE_VIEW && (a = "/data/lists/wine-data-empty.json"), (0, s.ax)(a, {
+                        var a, t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0,
+                            n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : 0,
+                            r = u.Z[e];
+                        return a = "".concat(m + "/data").concat(r.urlPath, "?pageSize=").concat(t, "&offset=").concat(n), "true" === c.env.REACT_APP_EMPTY_RESOURCE_VIEW && (a = "/data/lists/wine-data-empty.json"), (0, s.ax)(a, {
+                            method: "POST",
                             headers: {
                                 "Content-Type": "application/json"
                             }
                         }).then(function(e) {
                             return e.json().then(function(e) {
+                                var a, t;
                                 return {
-                                    data: e
+                                    data: null !== (a = null == e ? void 0 : e.resourceList) && void 0 !== a ? a : [],
+                                    count: null !== (t = null == e ? void 0 : e.count) && void 0 !== t ? t : 0
                                 }
                             })
                         }).catch(function(e) {
                             console.error(e)
                         })
                     }
                 }, {
@@ -99638,15 +99645,15 @@
                 l = t(98970),
                 s = t(6518),
                 u = new r.ZP,
                 c = function(e) {
                     var a = e.type,
                         t = i.Z.pathToType[a],
                         r = (0, n.jsx)(n.Fragment, {});
-                    return r = void 0 === a && void 0 === t ? (0, n.jsx)(o.x, {}) : t ? (0, n.jsx)(s.Z, {
+                    return r = void 0 === a && void 0 === t ? (0, n.jsx)(o.x, {}) : t ? (0, n.jsx)(s.ZP, {
                         api: u,
                         type: t
                     }) : (0, n.jsx)(l.Z, {}), (0, n.jsx)(n.Fragment, {
                         children: r
                     })
                 };
             a.Z = c
@@ -105112,19 +105119,53 @@
                             children: i
                         }), '" exists.']
                     })]
                 })
             };
             a.Z = r
         },
+        61790: function(e, a, t) {
+            "use strict";
+            t.d(a, {
+                D4: function() {
+                    return s
+                }
+            });
+            var n = t(77236),
+                r = t(21286),
+                i = function(e, a) {
+                    return e[a] = {
+                        currentPage: 0
+                    }, e
+                },
+                o = r.Z.resourceTypes.reduce(i, {}),
+                l = (0, n.oM)({
+                    name: "resourcePage",
+                    initialState: o,
+                    reducers: {
+                        setCurrentPage: function(e, a) {
+                            var t = a.payload,
+                                n = t.type,
+                                i = t.currentPage,
+                                o = n;
+                            r.Z.typeToName[n] && (o = r.Z.typeToName[n]), e[o] && (e[o].currentPage = void 0 === i ? 0 : i)
+                        }
+                    }
+                }),
+                s = l.actions.setCurrentPage;
+            a.ZP = l.reducer
+        },
         6518: function(e, a, t) {
             "use strict";
             t.d(a, {
-                Z: function() {
-                    return eo
+                hn: function() {
+                    return en
+                },
+                ZP: function() {
+                    return es
                 }
             });
             var n, r = t(51438),
                 i = t(52951);
 
             function o(e, a) {
                 return (o = Object.setPrototypeOf || function(e, a) {
@@ -105237,54 +105278,54 @@
                 }),
                 O = function(e) {
                     var a = e.title,
                         t = e.columns,
                         n = e.resources,
                         r = e.type,
                         i = e.loading,
-                        o = e.redirect,
-                        l = void 0 === o ? function() {
+                        o = e.count,
+                        l = e.currentPage,
+                        s = e.setPage,
+                        c = void 0 === s ? function() {
                             return null
-                        } : o,
-                        s = null != n ? n : [],
-                        c = I();
+                        } : s,
+                        d = e.redirect,
+                        p = void 0 === d ? function() {
+                            return null
+                        } : d,
+                        f = null != n ? n : [],
+                        h = I();
                     return (0, u.jsx)(u.Fragment, {
                         children: i ? (0, u.jsx)(T.x, {}) : (0, u.jsxs)(u.Fragment, {
                             children: [(0, u.jsx)("h3", {
                                 children: a
-                            }), (null == s ? void 0 : s.length) ? (0, u.jsx)(u.Fragment, {
+                            }), (null == f ? void 0 : f.length) ? (0, u.jsx)(u.Fragment, {
                                 children: (0, u.jsx)(E._, {
                                     disableVirtualization: !0,
                                     autoHeight: !0,
                                     "aria-label": a,
-                                    rows: s,
+                                    rows: f,
                                     columns: t,
-                                    className: c.dataGrid,
+                                    className: h.dataGrid,
                                     rowHeight: 65,
                                     hideFooterSelectedRowCount: !0,
                                     disableColumnFilter: !0,
                                     disableColumnMenu: !0,
                                     disableColumnSelector: !0,
-                                    initialState: {
-                                        pagination: {
-                                            paginationModel: {
-                                                page: 0,
-                                                pageSize: 10
-                                            }
-                                        },
-                                        sorting: [{
-                                            field: "name",
-                                            sort: "desc"
-                                        }]
+                                    paginationMode: "server",
+                                    onPageChange: function(e) {
+                                        console.log("onPageChange", e), c(e)
                                     },
-                                    pageSize: 10,
-                                    rowsPerPageOptions: [10],
+                                    rowCount: o,
+                                    page: l,
+                                    pageSize: en,
+                                    rowsPerPageOptions: [en],
                                     onRowClick: function(e, a) {
                                         var t;
-                                        null == a || a.preventDefault(), (null == e ? void 0 : null === (t = e.row) || void 0 === t ? void 0 : t.name) && l(e.row.name)
+                                        null == a || a.preventDefault(), (null == e ? void 0 : null === (t = e.row) || void 0 === t ? void 0 : t.name) && p(e.row.name)
                                     },
                                     getRowId: function(e) {
                                         return e.name
                                     }
                                 })
                             }) : (0, u.jsx)(P, {
                                 type: r
@@ -105429,27 +105470,33 @@
                         })
                     }
                 }, ],
                 j = function(e) {
                     var a = e.resources,
                         t = e.type,
                         n = e.loading,
-                        r = (0, S.useRouter)(),
-                        i = function() {
+                        r = e.count,
+                        i = e.currentPage,
+                        o = e.setPage,
+                        l = (0, S.useRouter)(),
+                        s = function() {
                             var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "";
-                            r.push("/sources/".concat(e))
+                            l.push("/sources/".concat(e))
                         };
                     return (0, u.jsx)(u.Fragment, {
                         children: (0, u.jsx)(O, {
                             title: "Datasets",
                             type: t,
                             columns: B,
                             resources: null != a ? a : [],
                             loading: n,
-                            redirect: i
+                            redirect: s,
+                            count: r,
+                            currentPage: i,
+                            setPage: o
                         })
                     })
                 },
                 H = [{
                     field: "id",
                     headerName: "id",
                     flex: 1,
@@ -105532,26 +105579,32 @@
                         })
                     }
                 }, ],
                 z = function(e) {
                     var a = e.resources,
                         t = e.type,
                         n = e.loading,
-                        r = (0, S.useRouter)(),
-                        i = function() {
+                        r = e.count,
+                        i = e.currentPage,
+                        o = e.setPage,
+                        l = (0, S.useRouter)(),
+                        s = function() {
                             var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "";
-                            r.push("/entities/".concat(e))
+                            l.push("/entities/".concat(e))
                         };
                     return (0, u.jsx)(O, {
                         title: "Entities",
                         type: t,
                         columns: H,
                         resources: null != a ? a : [],
                         loading: n,
-                        redirect: i
+                        redirect: s,
+                        count: r,
+                        currentPage: i,
+                        setPage: o
                     })
                 },
                 K = [{
                     field: "id",
                     headerName: "id",
                     flex: 1,
                     editable: !1,
@@ -105681,26 +105734,32 @@
                         })
                     }
                 }, ],
                 G = function(e) {
                     var a = e.resources,
                         t = e.type,
                         n = e.loading,
-                        r = (0, S.useRouter)(),
-                        i = function() {
+                        r = e.count,
+                        i = e.currentPage,
+                        o = e.setPage,
+                        l = (0, S.useRouter)(),
+                        s = function() {
                             var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "";
-                            r.push("/features/".concat(e))
+                            l.push("/features/".concat(e))
                         };
                     return (0, u.jsx)(O, {
                         title: "Features",
                         type: t,
                         columns: K,
                         resources: null != a ? a : [],
                         loading: n,
-                        redirect: i
+                        redirect: s,
+                        count: r,
+                        currentPage: i,
+                        setPage: o
                     })
                 },
                 F = [{
                     field: "id",
                     headerName: "id",
                     flex: 1,
                     editable: !1,
@@ -105830,26 +105889,32 @@
                         })
                     }
                 }, ],
                 Z = function(e) {
                     var a = e.resources,
                         t = e.type,
                         n = e.loading,
-                        r = (0, S.useRouter)(),
-                        i = function() {
+                        r = e.count,
+                        i = e.currentPage,
+                        o = e.setPage,
+                        l = (0, S.useRouter)(),
+                        s = function() {
                             var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "";
-                            r.push("/labels/".concat(e))
+                            l.push("/labels/".concat(e))
                         };
                     return (0, u.jsx)(O, {
                         title: "Labels",
                         type: t,
                         columns: F,
                         resources: null != a ? a : [],
                         loading: n,
-                        redirect: i
+                        redirect: s,
+                        count: r,
+                        currentPage: i,
+                        setPage: o
                     })
                 },
                 V = [{
                     field: "id",
                     headerName: "id",
                     flex: 1,
                     width: 150,
@@ -105942,32 +106007,39 @@
                         })
                     }
                 }, ],
                 U = function(e) {
                     var a = e.resources,
                         t = e.type,
                         n = e.loading,
-                        r = (0, S.useRouter)(),
-                        i = function() {
+                        r = e.count,
+                        i = e.currentPage,
+                        o = e.setPage,
+                        l = (0, S.useRouter)(),
+                        s = function() {
                             var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "";
-                            r.push("/models/".concat(e))
+                            l.push("/models/".concat(e))
                         };
                     return (0, u.jsx)(u.Fragment, {
                         children: (0, u.jsx)(O, {
                             title: "Models",
                             type: t,
                             columns: V,
                             resources: null != a ? a : [],
                             loading: n,
-                            redirect: i
+                            redirect: s,
+                            count: r,
+                            currentPage: i,
+                            setPage: o
                         })
                     })
                 },
-                W = t(13824),
-                J = [{
+                W = t(61790),
+                J = t(13824),
+                Y = [{
                     field: "id",
                     headerName: "id",
                     flex: 1,
                     editable: !1,
                     sortable: !1,
                     filterable: !1,
                     hide: !0
@@ -105984,15 +106056,15 @@
                         return (0, u.jsxs)(u.Fragment, {
                             children: [(0, u.jsx)("img", {
                                 alt: e.row.software,
                                 style: {
                                     width: "6em",
                                     height: "2.5em"
                                 },
-                                src: W.vI[null === (a = e.row.software) || void 0 === a ? void 0 : a.toUpperCase()]
+                                src: J.vI[null === (a = e.row.software) || void 0 === a ? void 0 : a.toUpperCase()]
                             }), (0, u.jsx)(k.Z, {
                                 variant: "body1",
                                 sx: {
                                     marginLeft: 1
                                 },
                                 children: e.row.name
                             })]
@@ -106072,54 +106144,60 @@
                     headerName: "Status",
                     flex: 1,
                     width: 350,
                     editable: !1,
                     sortable: !1,
                     filterable: !1,
                     renderCell: function(e) {
-                        var a, t, n = "#6DDE6A",
-                            r = "#DA1E28";
-                        return (null == e ? void 0 : null === (a = e.row) || void 0 === a ? void 0 : a.status) && (null == e ? void 0 : null === (t = e.row) || void 0 === t ? void 0 : t.status) === "READY" && (r = n), (0, u.jsxs)(u.Fragment, {
+                        var a, t, n, r = "#6DDE6A",
+                            i = "#DA1E28";
+                        return (null == e ? void 0 : null === (a = e.row) || void 0 === a ? void 0 : a.status) === "READY" ? i = r : (null == e ? void 0 : null === (t = e.row) || void 0 === t ? void 0 : t.status) === "CREATED" && ["MEMORY", "LOCAL_FILESYSTEM", "AZURE", "GLUE", "S3", "GCS", "HDFS", ].includes(null == e ? void 0 : null === (n = e.row) || void 0 === n ? void 0 : n["provider-type"]) && (i = r), (0, u.jsxs)(u.Fragment, {
                             children: [(0, u.jsx)(_, {
-                                fill: r,
+                                fill: i,
                                 height: "20",
                                 width: "20"
                             }), (0, u.jsx)(k.Z, {
                                 variant: "body1",
                                 sx: {
                                     marginLeft: 1
                                 },
-                                children: r === n ? "Connected" : "Disconnected"
+                                children: i === r ? "Connected" : "Disconnected"
                             })]
                         })
                     }
                 }, ],
-                Y = function(e) {
+                q = function(e) {
                     var a = e.resources,
                         t = e.type,
                         n = e.loading,
-                        r = (0, S.useRouter)(),
-                        i = function() {
+                        r = e.count,
+                        i = e.currentPage,
+                        o = e.setPage,
+                        l = (0, S.useRouter)(),
+                        s = function() {
                             var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "";
-                            r.push("/providers/".concat(e))
+                            l.push("/providers/".concat(e))
                         };
                     return (0, u.jsx)(u.Fragment, {
                         children: (0, u.jsx)(O, {
                             title: "Providers",
                             type: t,
-                            columns: J,
+                            columns: Y,
                             resources: null != a ? a : [],
                             loading: n,
-                            redirect: i
+                            redirect: s,
+                            count: r,
+                            currentPage: i,
+                            setPage: o
                         })
                     })
                 },
-                q = t(16332),
-                $ = t(5378),
-                X = [{
+                $ = t(16332),
+                X = t(5378),
+                Q = [{
                     field: "id",
                     headerName: "id",
                     flex: 1,
                     editable: !1,
                     sortable: !1,
                     filterable: !1,
                     hide: !0
@@ -106254,44 +106332,51 @@
                                     },
                                     children: null == n ? void 0 : n.owner
                                 })]
                             })]
                         })
                     }
                 }, ],
-                Q = function(e) {
+                ee = function(e) {
                     var a = e.resources,
                         t = e.type,
                         n = e.loading,
-                        r = (0, S.useRouter)(),
-                        i = function() {
+                        r = e.count,
+                        i = e.currentPage,
+                        o = e.setPage,
+                        l = (0, S.useRouter)(),
+                        s = function() {
                             var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "";
-                            r.push("/training-sets/".concat(e))
+                            l.push("/training-sets/".concat(e))
                         };
                     return (0, u.jsx)(O, {
                         title: "Training Sets",
                         type: t,
-                        columns: X,
+                        columns: Q,
                         resources: null != a ? a : [],
                         loading: n,
-                        redirect: i
+                        redirect: s,
+                        count: r,
+                        currentPage: i,
+                        setPage: o
                     })
                 },
-                ee = t(93432),
-                ea = p()(function() {
+                ea = t(93432),
+                et = p()(function() {
                     return Promise.resolve().then(t.bind(t, 88802))
                 }, {
                     loadableGenerated: {
                         webpack: function() {
                             return [88802]
                         }
                     },
                     ssr: !1
                 }),
-                et = function(e) {
+                en = 10,
+                er = function(e) {
                     var a = function(a) {
                             return a.resourceList[e].resources
                         },
                         t = function(a) {
                             return a.selectedTags[e]
                         },
                         n = function(a) {
@@ -106304,63 +106389,77 @@
                             var r, i = t[e.name] ? t[e.name] : e["default-variant"];
                             return (e.variants[i].tags || []).filter(function(e) {
                                 return e in a
                             }).length === n
                         })
                     })
                 },
-                en = function(e, a) {
+                ei = function(e, a) {
                     return function(e) {
-                        var t, n = e.resourceList.selectedType || a.type,
-                            r = et(n),
-                            i = e.resourceList[n],
-                            o = e.selectedVariant[n],
-                            l = e.selectedTags[n];
-                        return {
-                            title: n,
-                            resources: r(e),
-                            loading: i.loading,
-                            failed: i.failed,
-                            activeVariants: o,
-                            activeTags: l
+                        var t, n = e.resourceList.selectedType,
+                            r = n || a.type,
+                            i = null === (t = e.resourceList[n]) || void 0 === t ? void 0 : t.count,
+                            o = er(r),
+                            l = e.resourceList[r],
+                            s = e.selectedVariant[r],
+                            u = e.selectedTags[r];
+                        return console.log(e.currentPage[r]), {
+                            title: r,
+                            resources: o(e),
+                            loading: l.loading,
+                            failed: l.failed,
+                            activeVariants: s,
+                            activeTags: u,
+                            pageSize: en,
+                            currentPage: e.currentPage[r].currentPage,
+                            count: i
                         }
                     }
                 },
-                er = function(e, a) {
+                eo = function(e, a) {
                     return function(e) {
                         return {
                             setCurrentType: function(a) {
-                                e((0, q.h_)({
+                                e((0, $.h_)({
                                     selectedType: a
                                 }))
                             },
-                            fetch: function(t) {
-                                e((0, q.eL)({
+                            fetch: function(t, n) {
+                                e((0, $.eL)({
                                     api: a.api,
-                                    type: t || a.type
+                                    type: t || a.type,
+                                    pageSize: en,
+                                    offset: n
                                 }))
                             },
                             setVariant: function(a, t, n) {
-                                e((0, ee.jO)({
+                                e((0, ea.jO)({
                                     type: a,
                                     name: t,
                                     variant: n
                                 }))
                             },
                             toggleTag: function(t) {
                                 var n = a.type;
-                                e((0, $.av)({
+                                e((0, X.av)({
                                     type: n,
                                     tag: t
                                 }))
+                            },
+                            setPage: function(t) {
+                                var n = a.type;
+                                e((0, W.D4)({
+                                    type: n,
+                                    currentPage: t
+                                }))
                             }
                         }
                     }
                 },
-                ei = function(e) {
+                el = function(e) {
                     ! function(e, a) {
                         if ("function" != typeof a && null !== a) throw TypeError("Super expression must either be null or a function");
                         if (e.prototype = Object.create(a && a.prototype, {
                                 constructor: {
                                     value: e,
                                     writable: !0,
                                     configurable: !0
@@ -106392,29 +106491,29 @@
 
                     function c() {
                         return (0, r.Z)(this, c), n.apply(this, arguments)
                     }
                     return (0, i.Z)(c, [{
                         key: "componentDidMount",
                         value: function() {
-                            this.props.fetch(), this.props.setCurrentType(this.props.type)
+                            this.props.fetch(this.props.type, this.props.currentPage), this.props.setCurrentType(this.props.type)
                         }
                     }, {
                         key: "componentDidUpdate",
                         value: function(e) {
-                            e.type !== this.props.type && (this.props.fetch(this.props.type), this.props.setCurrentType(this.props.type))
+                            e.type !== this.props.type ? (this.props.setPage(0), this.props.fetch(this.props.type), this.props.setCurrentType(this.props.type)) : e.currentPage !== this.props.currentPage && this.props.fetch(this.props.type, this.props.currentPage)
                         }
                     }, {
                         key: "render",
                         value: function() {
                             var e = (0, l.Z)({}, this.props);
                             delete e.api, delete e.fetch;
                             var a = (0, u.jsx)(g, {}),
-                                t = (0, u.jsx)(Y, (0, l.Z)({}, e)),
-                                n = (0, u.jsx)(Q, (0, l.Z)({}, e)),
+                                t = (0, u.jsx)(q, (0, l.Z)({}, e)),
+                                n = (0, u.jsx)(ee, (0, l.Z)({}, e)),
                                 r = (0, u.jsx)(G, (0, l.Z)({}, e)),
                                 i = (0, u.jsx)(z, (0, l.Z)({}, e)),
                                 o = (0, u.jsx)(Z, (0, l.Z)({}, e)),
                                 s = (0, u.jsx)(U, (0, l.Z)({}, e)),
                                 c = (0, u.jsx)(j, (0, l.Z)({}, e)),
                                 d = null,
                                 p = {
@@ -106422,27 +106521,30 @@
                                     TrainingSet: n,
                                     Feature: r,
                                     Entity: i,
                                     Label: o,
                                     Model: s,
                                     Source: c
                                 };
-                            return e.failed ? a : e.type in p ? p[e.type] : (0, u.jsx)(ea, (0, l.Z)({}, e))
+                            return e.failed ? a : e.type in p ? p[e.type] : (0, u.jsx)(et, (0, l.Z)({}, e))
                         }
                     }]), c
                 }(m.Component);
-            ei.propTypes = {
+            el.propTypes = {
                 type: h().string.isRequired,
                 api: h().object.isRequired,
                 title: h().string,
                 resources: h().array,
                 loading: h().bool,
-                failed: h().bool
+                failed: h().bool,
+                pageSize: h().number,
+                currentPage: h().number,
+                count: h().number
             };
-            var eo = (0, v.$j)(en, er)(ei)
+            var es = (0, v.$j)(ei, eo)(el)
         },
         88802: function(e, a, t) {
             "use strict";
             t.r(a), t.d(a, {
                 ResourceListView: function() {
                     return O
                 },
@@ -107078,21 +107180,21 @@
                             t &= c(e["all-variants"].includes(a), "Variant in variant object not in variant list")
                         })
                     }) : e.forEach(function(e) {
                         t &= c("name" in e, "Resource has no name element")
                     }), t
                 },
                 p = (0, s.hg)("resourceList/fetchByType", (r = (0, i.Z)(function(e, a) {
-                    var t, n, r, i;
-                    return (0, l.__generator)(this, function(i) {
-                        switch (i.label) {
+                    var t, n, r, i, o, s;
+                    return (0, l.__generator)(this, function(l) {
+                        switch (l.label) {
                             case 0:
-                                return t = e.api, n = e.type, r = a.signal, [4, t.fetchResources(n, r)];
+                                return t = e.api, n = e.type, r = e.pageSize, i = e.offset, o = a.signal, [4, t.fetchResources(n, r, i, o)];
                             case 1:
-                                return [2, i.sent().data]
+                                return [2, l.sent()]
                         }
                     })
                 }), function(e, a) {
                     return r.apply(this, arguments)
                 }), {
                     condition: function(e, a) {
                         var t = e.type;
@@ -107117,20 +107219,20 @@
                         var t = a.meta.arg.type,
                             n = a.meta.requestId;
                         e[t].requestId = n, e[t].resources = null, e[t].loading = !0, e[t].failed = !1
                     }), (0, o.Z)(n, p.fulfilled, function(e, a) {
                         var t = a.meta.arg.type;
                         if (a.meta.requestId === e[t].requestId) {
                             var n = !0;
-                            if (a.payload.length > 0) {
+                            if (a.payload.data.length > 0) {
                                 n = !1;
-                                var r = a.payload[0].type.hasVariants;
-                                n = d(a.payload, r)
+                                var r = a.payload.data[0].type.hasVariants;
+                                n = d(a.payload.data, r)
                             }
-                            n ? (e[t].resources = a.payload, e[t].loading = !1, e[t].failed = !1) : (e[t].resources = null, e[t].loading = !1, e[t].failed = !0)
+                            n ? (e[t].resources = a.payload.data, e[t].count = a.payload.count, e[t].loading = !1, e[t].failed = !1) : (e[t].resources = null, e[t].count = 0, e[t].loading = !1, e[t].failed = !0)
                         }
                     }), (0, o.Z)(n, p.rejected, function(e, a) {
                         var t = a.meta.arg.type;
                         a.meta.requestId === e[t].requestId && (e[t].loading = !1, e[t].failed = !0)
                     }), n)
                 }),
                 v = m.actions.setCurrentType;
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/[groupName]-4ba8b6abfb4b13ca.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/[groupName]-4ba8b6abfb4b13ca.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/[roleName]-a4f4cefefad41418.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/[roleName]-a4f4cefefad41418.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/roles-a560426c6514c003.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/admin/roles-a560426c6514c003.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/[userName]-5a66d4c05c9e7453.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/[userName]-5a66d4c05c9e7453.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/index-142e8557e4889163.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/index-142e8557e4889163.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/pages/tasks-70243ca2c0452223.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/pages/tasks-70243ca2c0452223.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.9d4c892d6ec3e998.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.9d4c892d6ec3e998.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.1110d811936eb535.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.1110d811936eb535.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.1cceaa6cbbc063ac.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.1cceaa6cbbc063ac.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.eb2d7c5e73071e92.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.eb2d7c5e73071e92.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.7cda0a8b4fd10c8e.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.7cda0a8b4fd10c8e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.d3bb3d49b9c1d80b.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.d3bb3d49b9c1d80b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.a8dc93d57de022d3.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.a8dc93d57de022d3.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.5c26573759f9c121.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.5c26573759f9c121.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.7c2ee867e260f0e7.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.7c2ee867e260f0e7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.b157974fb0a5a751.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.b157974fb0a5a751.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.5b503b684163ddee.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.5b503b684163ddee.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.3767e3821cef0636.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.3767e3821cef0636.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.588ecfde90e6c6a6.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.588ecfde90e6c6a6.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.b830bba5a58a571f.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.b830bba5a58a571f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.e5835ab195bd9150.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.e5835ab195bd9150.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.c9f609621defe122.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.c9f609621defe122.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.cbb253b90d4065f6.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.cbb253b90d4065f6.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.12fc5c16e5a165ee.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.12fc5c16e5a165ee.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.24015a609992c2a0.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.24015a609992c2a0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.a83f04a28cfc5c13.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.a83f04a28cfc5c13.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.95f68b8f15b82829.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.95f68b8f15b82829.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.e02e26748402cb2f.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.e02e26748402cb2f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.a21b937dd852d3c5.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.a21b937dd852d3c5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.f36b9b8a53d85766.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.f36b9b8a53d85766.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.51b85e9ce6ac77e9.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.51b85e9ce6ac77e9.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.0f747e26266b02a2.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.0f747e26266b02a2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.0dcb315084b7163e.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.0dcb315084b7163e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.b594f920dc05a67e.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.b594f920dc05a67e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.588914f5988d8070.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.588914f5988d8070.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.ee070d344f3affd6.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.ee070d344f3affd6.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.1cb9d96b33822dc8.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.1cb9d96b33822dc8.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.0d5ec818ecef9324.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.0d5ec818ecef9324.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.628102c989f49555.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.628102c989f49555.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.d2924ae4e73b1223.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.d2924ae4e73b1223.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.3f60a647075d636f.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.3f60a647075d636f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.24b8d9cafb06d199.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.24b8d9cafb06d199.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.8c0ef98ac4f8e8a2.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.8c0ef98ac4f8e8a2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.40ae09135f82f50e.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.40ae09135f82f50e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.8aaf8e216bf41dfe.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.8aaf8e216bf41dfe.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.841bb10e71e1c449.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.841bb10e71e1c449.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.bc56944969bce274.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.bc56944969bce274.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.ca9c2b431c04ca17.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.ca9c2b431c04ca17.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.b5f4b6f514528d1d.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.b5f4b6f514528d1d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.3b8da30965ace8d0.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.3b8da30965ace8d0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.a4e379d50aabc89d.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.a4e379d50aabc89d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.31cb364f97f4e824.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.31cb364f97f4e824.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.e13b9d3271de18f9.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.e13b9d3271de18f9.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.e2654a73b0584dec.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.e2654a73b0584dec.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.da3b3e0fae942646.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.da3b3e0fae942646.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.399f0ab013510453.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.399f0ab013510453.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a7425f8edef285f7.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a7425f8edef285f7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.155ab93349c67ccd.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.155ab93349c67ccd.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.c6479c75f219ea50.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.c6479c75f219ea50.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.58f937c9dbd9989e.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.58f937c9dbd9989e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.a021feea122d3ab8.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.a021feea122d3ab8.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.15c4fc0252344391.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.15c4fc0252344391.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.746dde9caa36bd3a.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.746dde9caa36bd3a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.7866c582058e46fd.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.7866c582058e46fd.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.7724b491752c429c.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.7724b491752c429c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.d1dd2d2dd76819de.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.d1dd2d2dd76819de.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.c6da2507c50d21c4.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.c6da2507c50d21c4.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.d3fa954b1b6c7ddf.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.d3fa954b1b6c7ddf.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.a7092d9f281d4e48.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.a7092d9f281d4e48.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.8ccf09a496d63a6f.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.8ccf09a496d63a6f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1d47fcfbbb4f7aae.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1d47fcfbbb4f7aae.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.63e1bd7540f5f024.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.63e1bd7540f5f024.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.ec6db56efdb346a0.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.ec6db56efdb346a0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e29c5a5287592d58.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e29c5a5287592d58.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.d0376c6facb31ca5.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.d0376c6facb31ca5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.b47b77184d88114f.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.b47b77184d88114f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.78c84ccf0f96ba85.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.78c84ccf0f96ba85.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.c75feab6b678db77.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.c75feab6b678db77.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.508502701a02090a.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.508502701a02090a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.d426610fe97ba28f.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.d426610fe97ba28f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f181bbcd52749298.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f181bbcd52749298.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.75b381c93a6b3e68.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.75b381c93a6b3e68.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.16f39c180893252d.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.16f39c180893252d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.650dab668c7e4fd7.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.650dab668c7e4fd7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.64a2195a59fd1547.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.64a2195a59fd1547.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.80cf156f114fd8cf.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.80cf156f114fd8cf.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.b64600096e2ca9ed.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.b64600096e2ca9ed.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.01d852003dbb136c.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.01d852003dbb136c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.5aae66009f81a97f.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.5aae66009f81a97f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.f89efc1289945c39.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.f89efc1289945c39.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.da89585e43cc625e.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.da89585e43cc625e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.c33d2207767fa3ea.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.c33d2207767fa3ea.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.dffcd987fd2af796.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.dffcd987fd2af796.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.9a225e869035cf5e.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.9a225e869035cf5e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.33073eaf6ea575b1.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.33073eaf6ea575b1.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.bb74c766d6f802c5.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.bb74c766d6f802c5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.746cbe8d4f665f4e.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.746cbe8d4f665f4e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.cfac9943bd3aa8c6.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.cfac9943bd3aa8c6.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.8b59c21ed9aa0df8.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.8b59c21ed9aa0df8.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e3cb4a5604d89cfa.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e3cb4a5604d89cfa.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.12cb2d9917a6aab2.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.12cb2d9917a6aab2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.a3b5dc1c4d26ae4c.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.a3b5dc1c4d26ae4c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.a43af9cbcc3d056e.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.a43af9cbcc3d056e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.fb4387bc9a5ead37.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.fb4387bc9a5ead37.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.794412054be66c77.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.794412054be66c77.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.47962934ccb42723.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.47962934ccb42723.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.0df6c8ce29df587c.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.0df6c8ce29df587c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.40eef7387c672247.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.40eef7387c672247.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.c777981c76bf526a.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.c777981c76bf526a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.80fd5c9b26494fb4.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.80fd5c9b26494fb4.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b0db7f0ee3f15673.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b0db7f0ee3f15673.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.8b1345b4f614c39f.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.8b1345b4f614c39f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.31982856fa816d70.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.31982856fa816d70.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.f17164273275fd38.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.f17164273275fd38.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.2f587faa9c12f894.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.2f587faa9c12f894.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.02e16f89cc645033.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.02e16f89cc645033.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.dd5a243970406aba.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.dd5a243970406aba.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.acb704c99ae042b7.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.acb704c99ae042b7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.52a0bfb16d6c2b98.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.52a0bfb16d6c2b98.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.9a0f06e32359ab5f.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.9a0f06e32359ab5f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.69a4a948327f0b94.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.69a4a948327f0b94.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.8c3fb04cf18de9ad.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.8c3fb04cf18de9ad.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.fdc98b1cdb606d74.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.fdc98b1cdb606d74.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.8fca60ed2df5e72a.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.8fca60ed2df5e72a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.c6bd9f3fa6de96e2.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.c6bd9f3fa6de96e2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.74938f19e891fdf5.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.74938f19e891fdf5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.fc51859d62024c0c.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.fc51859d62024c0c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.722d26c11b333d29.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.722d26c11b333d29.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.a38fd3d408351597.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.a38fd3d408351597.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.374dabbd7a65bb7e.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.374dabbd7a65bb7e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.79a60949255a30ef.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.79a60949255a30ef.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b8f96e57ccaae943.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b8f96e57ccaae943.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.c394be68ff73cffa.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.c394be68ff73cffa.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.2017f4173ae7ddfb.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.2017f4173ae7ddfb.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.b409945670f221f7.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.b409945670f221f7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.83a26a43f4df0850.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.83a26a43f4df0850.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.51aa798f8d7e5f9d.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.51aa798f8d7e5f9d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.67ac42fc89d5c984.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.67ac42fc89d5c984.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.83317f3b3977639c.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.83317f3b3977639c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.b5b55f9072af7a5d.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.b5b55f9072af7a5d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.859e58b02983b520.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.859e58b02983b520.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.478f7d5866f2865d.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.478f7d5866f2865d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.7494238f7c6ad706.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.7494238f7c6ad706.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.199e2ba708699dcb.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.199e2ba708699dcb.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.98e2ba9a44a80b8d.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.98e2ba9a44a80b8d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.36058e7553ffa345.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.36058e7553ffa345.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.48de1152e01ba572.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.48de1152e01ba572.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.7a521a109d6461ca.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.7a521a109d6461ca.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.c091a192bf82f926.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.c091a192bf82f926.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.badf407c7a6f2db0.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.badf407c7a6f2db0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.213c3d6af366a76e.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.213c3d6af366a76e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.93772d4fe83877f5.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.93772d4fe83877f5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.3a384d03bec6f703.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.3a384d03bec6f703.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.9cdb03119b332984.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.9cdb03119b332984.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.e79ec6009494dfce.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.e79ec6009494dfce.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.7766acfcd5f91811.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.7766acfcd5f91811.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.e0ae21e641671328.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.e0ae21e641671328.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.26d85ff3fe699cbb.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.26d85ff3fe699cbb.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.f36a4d3fb726f719.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.f36a4d3fb726f719.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.fcda67b8e3d7ff14.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.fcda67b8e3d7ff14.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.72882aebe76845de.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.72882aebe76845de.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.2e295de118cafdef.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.2e295de118cafdef.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.e1cdb5c5cec33e2e.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.e1cdb5c5cec33e2e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.7e7c3d8167ac74f6.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.7e7c3d8167ac74f6.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.790c6f46fa4e9d8b.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.790c6f46fa4e9d8b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.1f694c1ce3fcc4d1.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.1f694c1ce3fcc4d1.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.3aa230ff56d754c5.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.3aa230ff56d754c5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.ae739446f2d00124.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.ae739446f2d00124.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.e221063f635f2e9f.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.e221063f635f2e9f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.e3b79e7ad6d1e67b.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.e3b79e7ad6d1e67b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.67dc98b63dd3081e.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.67dc98b63dd3081e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.49c692f8bc2d227f.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.49c692f8bc2d227f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.60d8ff3f62a0dde3.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.60d8ff3f62a0dde3.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.241341676d07c7c5.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.241341676d07c7c5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.edc1a3543d37dac7.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.edc1a3543d37dac7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.2ae7f1f871d749d9.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.2ae7f1f871d749d9.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.11864bd2178e2c08.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.11864bd2178e2c08.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.cf7ba940ae593d96.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.cf7ba940ae593d96.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.d61bc93d9240911c.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.d61bc93d9240911c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.7dc2e8495b82afa0.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.7dc2e8495b82afa0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.cc6c20111eef392b.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.cc6c20111eef392b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.28dda31a087b27dc.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.28dda31a087b27dc.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.2a65ffecac1e4433.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.2a65ffecac1e4433.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.f3ac4fdc10100a71.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.f3ac4fdc10100a71.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.e5cbb81e295d94aa.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.e5cbb81e295d94aa.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.8fd37bd46bcdef8e.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.8fd37bd46bcdef8e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.021da63363b275e2.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.021da63363b275e2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.7047500798cae5bd.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.7047500798cae5bd.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.37b21bb61cb7da6e.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.37b21bb61cb7da6e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.987edd5fb1761cdf.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.987edd5fb1761cdf.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.f4f05ad29882de17.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.f4f05ad29882de17.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.74a04f9bd98b3d92.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.74a04f9bd98b3d92.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.63c6b3c7dbad89c3.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.63c6b3c7dbad89c3.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.a961a8a3e36733d2.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.a961a8a3e36733d2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.5c35ca803e68095b.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.5c35ca803e68095b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.b314e238d6967a8f.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.b314e238d6967a8f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.1d0f9c7b17d4bc2b.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.1d0f9c7b17d4bc2b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.790da421b54213dd.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.790da421b54213dd.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.a9cf0d3dab52d046.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.a9cf0d3dab52d046.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.8efe0bec8cec6f08.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.8efe0bec8cec6f08.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.cfc4809f40a5b725.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.cfc4809f40a5b725.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2127ec25c75e4984.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2127ec25c75e4984.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.62a04a024d699193.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.62a04a024d699193.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.f45aa85f3888e4f5.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.f45aa85f3888e4f5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.a26c328f4cf8b171.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.a26c328f4cf8b171.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.ea05c1dd27403a55.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.ea05c1dd27403a55.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.d6af4f6428d66d9a.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.d6af4f6428d66d9a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.74e478ac085e3404.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.74e478ac085e3404.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.92e6c66e598bc5b0.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.92e6c66e598bc5b0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.5be2e1ec1d76cc74.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.5be2e1ec1d76cc74.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.aa5faeff88cffc63.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.aa5faeff88cffc63.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.97f81f55c7dda273.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.97f81f55c7dda273.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.2eea9520afb8e6ea.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.2eea9520afb8e6ea.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.df4e0a4839a040a1.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.df4e0a4839a040a1.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.e1a7f78fb87ff37c.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.e1a7f78fb87ff37c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.4ddc9ac973a0065e.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.4ddc9ac973a0065e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/chunks/webpack-4ca33bb86fc5510e.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/chunks/webpack-4ca33bb86fc5510e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/group/[groupName].html` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/admin/group/[groupName].html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/admin/group/%5BgroupName%5D-4ba8b6abfb4b13ca.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-569252d467889e35.js" defer=""></script><script src="/_next/static/chunks/pages/admin/group/%5BgroupName%5D-4ba8b6abfb4b13ca.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_buildManifest.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/group/[groupName]","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/group/[groupName]","query":{},"buildId":"tU2e0PPhQ-QR0Wjh2ilIZ","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/groups.html` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/[type]/[entity].html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-569252d467889e35.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D/%5Bentity%5D-2f83fe1ff7f9d94c.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_buildManifest.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/groups","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]/[entity]","query":{},"buildId":"tU2e0PPhQ-QR0Wjh2ilIZ","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/role/[roleName].html` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/404.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/admin/role/%5BroleName%5D-a4f4cefefad41418.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-569252d467889e35.js" defer=""></script><script src="/_next/static/chunks/pages/404-8d282ae638ce5722.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_buildManifest.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/role/[roleName]","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/404","query":{},"buildId":"tU2e0PPhQ-QR0Wjh2ilIZ","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/roles.html` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/tasks.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/admin/roles-a560426c6514c003.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-569252d467889e35.js" defer=""></script><script src="/_next/static/chunks/pages/tasks-70243ca2c0452223.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_buildManifest.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/roles","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/tasks","query":{},"buildId":"tU2e0PPhQ-QR0Wjh2ilIZ","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/user/[userName].html` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/search.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/admin/user/%5BuserName%5D-5a66d4c05c9e7453.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-569252d467889e35.js" defer=""></script><script src="/_next/static/chunks/pages/search-abfa6bb494904a10.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_buildManifest.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/user/[userName]","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/search","query":{},"buildId":"tU2e0PPhQ-QR0Wjh2ilIZ","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/admin/users.html` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/[type].html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-569252d467889e35.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D-7bfcb609b1affd61.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_buildManifest.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/users","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]","query":{},"buildId":"tU2e0PPhQ-QR0Wjh2ilIZ","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/connections.html` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/admin/groups.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/connections-f98076127418a04b.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-569252d467889e35.js" defer=""></script><script src="/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_buildManifest.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/connections","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/groups","query":{},"buildId":"tU2e0PPhQ-QR0Wjh2ilIZ","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/index.html` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/admin/roles.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/index-142e8557e4889163.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-569252d467889e35.js" defer=""></script><script src="/_next/static/chunks/pages/admin/roles-a560426c6514c003.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_buildManifest.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/roles","query":{},"buildId":"tU2e0PPhQ-QR0Wjh2ilIZ","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/query.html` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/query.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/query-5a171bd499b8d4eb.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-569252d467889e35.js" defer=""></script><script src="/_next/static/chunks/pages/query-5a171bd499b8d4eb.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_buildManifest.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/query","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/query","query":{},"buildId":"tU2e0PPhQ-QR0Wjh2ilIZ","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/search.html` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/admin/user/[userName].html`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/search-abfa6bb494904a10.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-569252d467889e35.js" defer=""></script><script src="/_next/static/chunks/pages/admin/user/%5BuserName%5D-5a66d4c05c9e7453.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_buildManifest.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/search","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/user/[userName]","query":{},"buildId":"tU2e0PPhQ-QR0Wjh2ilIZ","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Apache_Spark_logo.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/Apache_Spark_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Capital_One_logo.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/Capital_One_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_White.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_White.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Featureform_logo_pink.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/Featureform_logo_pink.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Kubernetes_logo.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/Kubernetes_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Postgresql_elephant.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/Postgresql_elephant.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Redis_Logo.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/Redis_Logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/Snowflake_Logo.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/Snowflake_Logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/amazon_dynamoDB.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/amazon_dynamoDB.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/amazon_redshift.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/amazon_redshift.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/amazon_s3.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/amazon_s3.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/apache_cassandra.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/apache_cassandra.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/apache_hadoop.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/apache_hadoop.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/apple-touch-icon.png` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/azure_storage_accounts.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/azure_storage_accounts.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/base_logo.png` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/base_logo.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/clearIcon.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/clearIcon.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/clickhouse-logo.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/clickhouse-logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/creature.png` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/creature.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/favicon.ico` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/google_bigquery.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/google_bigquery.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/google_cloud_storage.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/google_cloud_storage.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/google_firestore.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/google_firestore.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/logo192.png` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/logo192.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/logo512.png` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/logo512.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/mongoDB.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/mongoDB.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/offline_store.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/offline_store.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/safari-pinned-tab.svg` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/static/welcomebackground.png` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/static/welcomebackground.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/dashboard/out/tasks.html` & `featureform_enterprise-0.14.4/src/featureform/dashboard/out/admin/role/[roleName].html`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-574fe43e4223620b.js" defer=""></script><script src="/_next/static/chunks/pages/tasks-70243ca2c0452223.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js" defer=""></script><script src="/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-569252d467889e35.js" defer=""></script><script src="/_next/static/chunks/pages/admin/role/%5BroleName%5D-a4f4cefefad41418.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_buildManifest.js" defer=""></script><script src="/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   height: 100vh;
   background-image: linear-gradient(180deg, #0A0909 23%, #7A15E5);
 }
 .jss12 {
   top: 150px;
   width: 100%;
   position: absolute;
@@ -79,8 +79,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 100px;
   left: 275px;
   width: 80%;
   position: absolute;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/tasks","query":{},"buildId":"yVmVSX0ksIXzzxWh3Ff_1","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><style data-emotion="css df4if1">.css-df4if1{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><style data-emotion="css mtj2fr">.css-mtj2fr{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;background-color:#161419;visibility:hidden;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss2 css-mtj2fr"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss5 css-i6s8oy"><div class="jss6 MuiBox-root css-0"><style data-emotion="css 10nbb9v">.css-10nbb9v{height:50px;margin-top:8px;margin-left:-8px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-10nbb9v{display:none;}}@media (min-width:600px){.css-10nbb9v{display:block;}}</style><img class="MuiBox-root css-10nbb9v" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss8 MuiBox-root css-0"><div class="MuiBox-root css-0"></div></div></div></header></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/role/[roleName]","query":{},"buildId":"tU2e0PPhQ-QR0Wjh2ilIZ","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/deploy.py` & `featureform_enterprise-0.14.4/src/featureform/deploy.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/enums.py` & `featureform_enterprise-0.14.4/src/featureform/enums.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/exceptions.py` & `featureform_enterprise-0.14.4/src/featureform/exceptions.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/format.py` & `featureform_enterprise-0.14.4/src/featureform/format.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/get.py` & `featureform_enterprise-0.14.4/src/featureform/get.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/grpc_client.py` & `featureform_enterprise-0.14.4/src/featureform/grpc_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import contextlib
 import logging
 import sys
+import time
 from dataclasses import dataclass, field
 from typing import Dict, Optional
 
 import grpc
 from google.rpc import error_details_pb2, status_pb2
 from .lib import auth
 
-logging.basicConfig(level=logging.DEBUG, filename="grpc_debug.log")
+logging.basicConfig(
+    level=logging.DEBUG,
+    format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
+    datefmt='%Y-%m-%dT%H:%M:%S'
+)
 
 
 @dataclass
 class FFGrpcErrorDetails:
     """
     FFGrpcErrorDetails is a dataclass that represents the details of an error returned by the Featureform gRPC server.
     """
@@ -68,49 +73,61 @@
             self.handle_grpc_error(e)
 
     @staticmethod
     def _merge_auth_metadata(original_metadata, auth_metadata):
         if original_metadata is None:
             return auth_metadata
         # Remove existing authorization header if present
+        exclude_list = ["authorization", "refresh-token", "subject"]
         merged_metadata = [
-            item for item in original_metadata if item[0].lower() != "authorization"
+            item for item in original_metadata if item[0].lower() not in exclude_list
         ]
         # Append the new authorization header
         merged_metadata.extend(auth_metadata)
         return merged_metadata
 
     @staticmethod
     def is_streaming_response(obj):
         return hasattr(obj, "__iter__") and not isinstance(
             obj, (str, bytes, dict, list)
         )
 
     def __getattr__(self, name):
         attr = getattr(self._grpc_stub, name)
         if name != "GetAuthConfig" and callable(attr):
-
             def wrapper(*args, **kwargs):
                 try:
-                    token = auth.singleton.get_access_token_or_authenticate(
+                    logging.debug(f"Calling {name} with args: {args} and kwargs: {kwargs}")
+                    start = time.perf_counter()
+                    resultDict = auth.singleton.get_access_token_or_authenticate(
                         self._insecure, self._host
                     )
-                    if token is not None:
+                    if resultDict["token"] is not None:
                         kwargs["metadata"] = self._merge_auth_metadata(
                             kwargs.get("metadata"),
-                            [("authorization", "Bearer " + token)],
+                            [
+                                ("authorization", "Bearer " + resultDict["token"]),
+                                ("refresh-token", resultDict["refreshToken"]),
+                                ("subject", resultDict["subject"]),
+                            ],
                         )
+                    start_call = time.perf_counter()
                     # Use the stored metadata for the call
                     result = attr(*args, **kwargs)
                     # If result is a streaming call, wrap it.
                     if self.is_streaming_response(result):
                         return self.streaming_wrapper(result)
+                    end_call = time.perf_counter()
+                    logging.debug(f"grpc call to {name} took {end_call - start_call:.4f} seconds")
                     return result
                 except grpc.RpcError as e:
                     self.handle_grpc_error(e)
+                finally:
+                    end = time.perf_counter()
+                    logging.debug(f"Total Call to {name} took {end - start:.4f} seconds")
 
             return wrapper
         else:
             return attr
 
     def handle_grpc_error(self, e: grpc.RpcError) -> None:
         ex = e if self.debug else None
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/lib/auth.py` & `featureform_enterprise-0.14.4/src/featureform/lib/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import base64
 import hashlib
 import os
 import threading
 from abc import ABC, abstractmethod
-from typing import Optional
+from typing import Optional, Tuple
 
 import featureform as ff
 import requests
 from flask import Flask, request
 from typeguard import typechecked
 from werkzeug.serving import make_server
 import yaml
@@ -162,15 +162,15 @@
             if json_resp:
                 self._access_token = json_resp.get("access_token")
                 self._refresh_token = json_resp.get("refresh_token")
                 self._access_token_expires = int(time.time()) + int(
                     json_resp.get("expires_in")
                 )
         else:
-            print(f"PKCE failed to get refresh_token() {response.status_code}")
+            print(f"PKCE failed to get refresh_token: {response.status_code}")
             self._access_token = None
             self._refresh_token = None
             self._access_token_expires = None
 
         return self._access_token
 
     def clear_access_token(self) -> None:
@@ -310,15 +310,20 @@
             if json_resp:
                 self._access_token = json_resp.get("access_token")
                 self._refresh_token = json_resp.get("refresh_token")
                 self._access_token_expires = int(time.time()) + int(
                     json_resp.get("expires_in")
                 )
         else:
-            print(f"Native failed to get refresh_token() {response.status_code}")
+            print(f"Native failed to get access_token: {response.status_code}")
+            try:
+                json_resp = response.json()
+                print(json_resp)
+            except ValueError:
+                print("Failed to parse JSON response.")
             self._access_token = None
             self._refresh_token = None
             self._access_token_expires = None
 
         return self._access_token
 
     def _request_refresh_token(self, refresh_token) -> Optional[str]:
@@ -342,14 +347,20 @@
             if json_resp:
                 self._access_token = json_resp.get("access_token")
                 self._refresh_token = json_resp.get("refresh_token")
                 self._access_token_expires = int(time.time()) + int(
                     json_resp.get("expires_in")
                 )
         else:
+            print(f"Native failed to get refresh_token: {response.status_code}")
+            try:
+                json_resp = response.json()
+                print(json_resp)
+            except ValueError:
+                print("Failed to parse JSON response.")
             self._refresh_token = None
             self._access_token_expires = None
 
         return self._access_token
 
     def _pull_file_creds(self) -> Optional[dict]:
         featureform_path = os.environ.get("FEATUREFORM_DIR", ".featureform")
@@ -409,15 +420,15 @@
 
         token_filepath = os.path.join(
             auth_dir, AuthenticationManagerImpl.TOKEN_FILENAME
         )
         if os.path.exists(token_filepath):
             os.remove(token_filepath)
 
-    def get_access_token_or_authenticate(self, insecure, host) -> Optional[str]:
+    def get_access_token_or_authenticate(self, insecure, host) -> Optional[dict]:
         token_dict = self._read_token_dict_from_file()
         if token_dict:
             self._access_token = token_dict.get("access_token")
             self._refresh_token = token_dict.get("refresh_token")
             self._access_token_expires = token_dict.get("access_token_expires")
 
         if self._access_token:
@@ -456,29 +467,43 @@
                 if token_dict and token_dict.get("access_token"):
                     self._access_token = token_dict.get("access_token")
                     self._refresh_token = token_dict.get("refresh_token")
                     self._access_token_expires = token_dict.get("access_token_expires")
                     self._write_token_dict_to_file(token_dict)
                     break
 
-        return self._access_token
+        resultDict = {
+            "token": None,
+            "refreshToken": None,
+            "subject": None,
+        }
+        if self._access_token:
+            parsed_token = JWTUtils.parse_token(self._access_token)
+            if len(parsed_token) != 4:
+                raise Exception("Invalid access token, cannot parse the sub property!")
+            payload = parsed_token[1]
+            resultDict["token"] = self._access_token
+            resultDict["refreshToken"] = self._refresh_token
+            resultDict["subject"] = payload.get("sub")
+
+        return resultDict
 
     def get_subject(self, config, insecure, host) -> Optional[str]:
         self._auth_config = self._init_auth_config(config)
         self._add_services()
 
         if len(self._services) == 1 and isinstance(
             self._services[0], PassThroughService
         ):
             return "default_user"
         else:
             sub = None
-            access_token = self.get_access_token_or_authenticate(insecure, host)
-            if access_token is not None:
-                parsed_token = JWTUtils.parse_token(access_token)
+            resultDict = self.get_access_token_or_authenticate(insecure, host)
+            if resultDict["token"] is not None:
+                parsed_token = JWTUtils.parse_token(resultDict["token"])
                 if len(parsed_token) != 4:
                     raise Exception("Invalid access token")
                 payload = parsed_token[1]
                 sub = payload.get("sub")
             return sub
 
     def _load_auth_config(self, insecure, host) -> Optional[OktaAuthConfig]:
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/list.py` & `featureform_enterprise-0.14.4/src/featureform/list.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/proto/metadata.proto` & `featureform_enterprise-0.14.4/src/featureform/proto/metadata.proto`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/proto/metadata_pb2.py` & `featureform_enterprise-0.14.4/src/featureform/proto/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/proto/metadata_pb2.pyi` & `featureform_enterprise-0.14.4/src/featureform/proto/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/proto/metadata_pb2_grpc.py` & `featureform_enterprise-0.14.4/src/featureform/proto/metadata_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/proto/serving.proto` & `featureform_enterprise-0.14.4/src/featureform/proto/serving.proto`

 * *Files 7% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 syntax = "proto3";
 
 option go_package = "github.com/featureform/proto";
 
 package featureform.serving.proto;
 
 service Feature {
-  rpc TrainingData(TrainingDataRequest) returns (stream TrainingDataRow) {}
+  rpc TrainingData(TrainingDataRequest) returns (stream TrainingDataRows) {}
   rpc TrainTestSplit(stream TrainTestSplitRequest) returns (stream BatchTrainTestSplitResponse) {}
   rpc TrainingDataColumns(TrainingDataColumnsRequest) returns (TrainingColumns) {}
   rpc FeatureServe(FeatureServeRequest) returns (FeatureRow) {}
-  rpc SourceData(SourceDataRequest) returns (stream SourceDataRow) {}
+  rpc SourceData(SourceDataRequest) returns (stream SourceDataRows) {}
   rpc SourceColumns(SourceColumnRequest) returns (SourceDataColumns) {}
   rpc Nearest(NearestRequest) returns (NearestResponse) {}
-  rpc BatchFeatureServe(BatchFeatureServeRequest) returns (stream BatchFeatureRow) {}
+  rpc BatchFeatureServe(BatchFeatureServeRequest) returns (stream BatchFeatureRows) {}
   rpc GetResourceLocation(ResourceIdRequest) returns (ResourceLocation) {}
 }
 
 message Model {
   string name = 1;
 }
 
@@ -30,14 +30,18 @@
 }
 
 message TrainingDataID {
   string name = 1;
   string version = 2;
 }
 
+message TrainingDataRows {
+  repeated TrainingDataRow rows = 1;
+}
+
 message TrainingDataRow {
   repeated Value features = 1;
   Value label = 2;
 }
 
 message FeatureServeRequest {
   repeated FeatureID features = 1;
@@ -56,14 +60,18 @@
   repeated Value values = 1;
 }
 
 message BatchFeatureServeRequest {
   repeated FeatureID features = 1;
 }
 
+message BatchFeatureRows {
+  repeated BatchFeatureRow rows = 1;
+}
+
 message BatchFeatureRow {
   Value entity = 1;
   repeated Value features = 2;
 }
 
 message FeatureID {
   string name = 1;
@@ -105,14 +113,18 @@
   int64 limit = 2;
 }
 
 message SourceColumnRequest {
   SourceID id = 1;
 }
 
+message SourceDataRows {
+  repeated SourceDataRow rows = 1;
+}
+
 message SourceDataRow {
   repeated Value rows = 1;
 }
 
 message SourceDataColumns {
   repeated string columns = 1;
 }
@@ -171,11 +183,7 @@
   RequestType request_type = 1;
   bool iterator_done = 2;
   oneof result {
     bool initialized = 3;
     TrainingDataRows data = 4;
   }
 }
-
-message TrainingDataRows {
-  repeated TrainingDataRow rows = 1;
-}
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/proto/serving_pb2.py` & `featureform_enterprise-0.14.4/src/featureform/proto/serving_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,78 +10,82 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x66\x65\x61tureform/proto/serving.proto\x12\x19\x66\x65\x61tureform.serving.proto\"\x15\n\x05Model\x12\x0c\n\x04name\x18\x01 \x01(\t\"}\n\x13TrainingDataRequest\x12\x35\n\x02id\x18\x01 \x01(\x0b\x32).featureform.serving.proto.TrainingDataID\x12/\n\x05model\x18\x02 \x01(\x0b\x32 .featureform.serving.proto.Model\"/\n\x0eTrainingDataID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"v\n\x0fTrainingDataRow\x12\x32\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32 .featureform.serving.proto.Value\x12/\n\x05label\x18\x02 \x01(\x0b\x32 .featureform.serving.proto.Value\"\xb3\x01\n\x13\x46\x65\x61tureServeRequest\x12\x36\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32$.featureform.serving.proto.FeatureID\x12\x33\n\x08\x65ntities\x18\x02 \x03(\x0b\x32!.featureform.serving.proto.Entity\x12/\n\x05model\x18\x03 \x01(\x0b\x32 .featureform.serving.proto.Model\"}\n\nFeatureRow\x12\x34\n\x06values\x18\x01 \x03(\x0b\x32 .featureform.serving.proto.ValueB\x02\x18\x01\x12\x39\n\x0bvalue_lists\x18\x02 \x03(\x0b\x32$.featureform.serving.proto.ValueList\"=\n\tValueList\x12\x30\n\x06values\x18\x01 \x03(\x0b\x32 .featureform.serving.proto.Value\"R\n\x18\x42\x61tchFeatureServeRequest\x12\x36\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32$.featureform.serving.proto.FeatureID\"w\n\x0f\x42\x61tchFeatureRow\x12\x30\n\x06\x65ntity\x18\x01 \x01(\x0b\x32 .featureform.serving.proto.Value\x12\x32\n\x08\x66\x65\x61tures\x18\x02 \x03(\x0b\x32 .featureform.serving.proto.Value\"*\n\tFeatureID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"9\n\x06\x45ntity\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\x05value\x18\x02 \x01(\tB\x02\x18\x01\x12\x0e\n\x06values\x18\x03 \x03(\t\"\xba\x02\n\x05Value\x12\x13\n\tstr_value\x18\x01 \x01(\tH\x00\x12\x13\n\tint_value\x18\x02 \x01(\x05H\x00\x12\x15\n\x0b\x66loat_value\x18\x03 \x01(\x02H\x00\x12\x16\n\x0c\x64ouble_value\x18\x04 \x01(\x01H\x00\x12\x15\n\x0bint64_value\x18\x05 \x01(\x03H\x00\x12\x15\n\x0bint32_value\x18\x06 \x01(\x05H\x00\x12\x14\n\nbool_value\x18\x07 \x01(\x08H\x00\x12\x1c\n\x12on_demand_function\x18\x08 \x01(\x0cH\x00\x12=\n\x0evector32_value\x18\t \x01(\x0b\x32#.featureform.serving.proto.Vector32H\x00\x12\x16\n\x0cuint32_value\x18\n \x01(\rH\x00\x12\x16\n\x0cuint64_value\x18\x0b \x01(\x04H\x00\x42\x07\n\x05value\")\n\x08SourceID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"S\n\x11SourceDataRequest\x12/\n\x02id\x18\x01 \x01(\x0b\x32#.featureform.serving.proto.SourceID\x12\r\n\x05limit\x18\x02 \x01(\x03\"F\n\x13SourceColumnRequest\x12/\n\x02id\x18\x01 \x01(\x0b\x32#.featureform.serving.proto.SourceID\"?\n\rSourceDataRow\x12.\n\x04rows\x18\x01 \x03(\x0b\x32 .featureform.serving.proto.Value\"$\n\x11SourceDataColumns\x12\x0f\n\x07\x63olumns\x18\x01 \x03(\t\"S\n\x1aTrainingDataColumnsRequest\x12\x35\n\x02id\x18\x01 \x01(\x0b\x32).featureform.serving.proto.TrainingDataID\"2\n\x0fTrainingColumns\x12\x10\n\x08\x66\x65\x61tures\x18\x01 \x03(\t\x12\r\n\x05label\x18\x02 \x01(\t\"\x19\n\x08Vector32\x12\r\n\x05value\x18\x01 \x03(\x02\"\x82\x01\n\x0eNearestRequest\x12\x30\n\x02id\x18\x01 \x01(\x0b\x32$.featureform.serving.proto.FeatureID\x12\x33\n\x06vector\x18\x02 \x01(\x0b\x32#.featureform.serving.proto.Vector32\x12\t\n\x01k\x18\x03 \x01(\x05\"#\n\x0fNearestResponse\x12\x10\n\x08\x65ntities\x18\x01 \x03(\t\"@\n\x11ResourceIdRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\x05\"$\n\x10ResourceLocation\x12\x10\n\x08location\x18\x01 \x01(\t\"\x9f\x02\n\x15TrainTestSplitRequest\x12\x35\n\x02id\x18\x01 \x01(\x0b\x32).featureform.serving.proto.TrainingDataID\x12/\n\x05model\x18\x02 \x01(\x0b\x32 .featureform.serving.proto.Model\x12\x11\n\ttest_size\x18\x03 \x01(\x02\x12\x12\n\ntrain_size\x18\x04 \x01(\x02\x12\x0f\n\x07shuffle\x18\x05 \x01(\x08\x12\x14\n\x0crandom_state\x18\x06 \x01(\x05\x12<\n\x0crequest_type\x18\x07 \x01(\x0e\x32&.featureform.serving.proto.RequestType\x12\x12\n\nbatch_size\x18\x08 \x01(\x05\"\xd0\x01\n\x1b\x42\x61tchTrainTestSplitResponse\x12<\n\x0crequest_type\x18\x01 \x01(\x0e\x32&.featureform.serving.proto.RequestType\x12\x15\n\riterator_done\x18\x02 \x01(\x08\x12\x15\n\x0binitialized\x18\x03 \x01(\x08H\x00\x12;\n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32+.featureform.serving.proto.TrainingDataRowsH\x00\x42\x08\n\x06result\"L\n\x10TrainingDataRows\x12\x38\n\x04rows\x18\x01 \x03(\x0b\x32*.featureform.serving.proto.TrainingDataRow*5\n\x0bRequestType\x12\x0e\n\nINITIALIZE\x10\x00\x12\x0c\n\x08TRAINING\x10\x01\x12\x08\n\x04TEST\x10\x02\x32\x8e\x08\n\x07\x46\x65\x61ture\x12n\n\x0cTrainingData\x12..featureform.serving.proto.TrainingDataRequest\x1a*.featureform.serving.proto.TrainingDataRow\"\x00\x30\x01\x12\x80\x01\n\x0eTrainTestSplit\x12\x30.featureform.serving.proto.TrainTestSplitRequest\x1a\x36.featureform.serving.proto.BatchTrainTestSplitResponse\"\x00(\x01\x30\x01\x12z\n\x13TrainingDataColumns\x12\x35.featureform.serving.proto.TrainingDataColumnsRequest\x1a*.featureform.serving.proto.TrainingColumns\"\x00\x12g\n\x0c\x46\x65\x61tureServe\x12..featureform.serving.proto.FeatureServeRequest\x1a%.featureform.serving.proto.FeatureRow\"\x00\x12h\n\nSourceData\x12,.featureform.serving.proto.SourceDataRequest\x1a(.featureform.serving.proto.SourceDataRow\"\x00\x30\x01\x12o\n\rSourceColumns\x12..featureform.serving.proto.SourceColumnRequest\x1a,.featureform.serving.proto.SourceDataColumns\"\x00\x12\x62\n\x07Nearest\x12).featureform.serving.proto.NearestRequest\x1a*.featureform.serving.proto.NearestResponse\"\x00\x12x\n\x11\x42\x61tchFeatureServe\x12\x33.featureform.serving.proto.BatchFeatureServeRequest\x1a*.featureform.serving.proto.BatchFeatureRow\"\x00\x30\x01\x12r\n\x13GetResourceLocation\x12,.featureform.serving.proto.ResourceIdRequest\x1a+.featureform.serving.proto.ResourceLocation\"\x00\x42\x1eZ\x1cgithub.com/featureform/protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x66\x65\x61tureform/proto/serving.proto\x12\x19\x66\x65\x61tureform.serving.proto\"\x15\n\x05Model\x12\x0c\n\x04name\x18\x01 \x01(\t\"}\n\x13TrainingDataRequest\x12\x35\n\x02id\x18\x01 \x01(\x0b\x32).featureform.serving.proto.TrainingDataID\x12/\n\x05model\x18\x02 \x01(\x0b\x32 .featureform.serving.proto.Model\"/\n\x0eTrainingDataID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"L\n\x10TrainingDataRows\x12\x38\n\x04rows\x18\x01 \x03(\x0b\x32*.featureform.serving.proto.TrainingDataRow\"v\n\x0fTrainingDataRow\x12\x32\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32 .featureform.serving.proto.Value\x12/\n\x05label\x18\x02 \x01(\x0b\x32 .featureform.serving.proto.Value\"\xb3\x01\n\x13\x46\x65\x61tureServeRequest\x12\x36\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32$.featureform.serving.proto.FeatureID\x12\x33\n\x08\x65ntities\x18\x02 \x03(\x0b\x32!.featureform.serving.proto.Entity\x12/\n\x05model\x18\x03 \x01(\x0b\x32 .featureform.serving.proto.Model\"}\n\nFeatureRow\x12\x34\n\x06values\x18\x01 \x03(\x0b\x32 .featureform.serving.proto.ValueB\x02\x18\x01\x12\x39\n\x0bvalue_lists\x18\x02 \x03(\x0b\x32$.featureform.serving.proto.ValueList\"=\n\tValueList\x12\x30\n\x06values\x18\x01 \x03(\x0b\x32 .featureform.serving.proto.Value\"R\n\x18\x42\x61tchFeatureServeRequest\x12\x36\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32$.featureform.serving.proto.FeatureID\"L\n\x10\x42\x61tchFeatureRows\x12\x38\n\x04rows\x18\x01 \x03(\x0b\x32*.featureform.serving.proto.BatchFeatureRow\"w\n\x0f\x42\x61tchFeatureRow\x12\x30\n\x06\x65ntity\x18\x01 \x01(\x0b\x32 .featureform.serving.proto.Value\x12\x32\n\x08\x66\x65\x61tures\x18\x02 \x03(\x0b\x32 .featureform.serving.proto.Value\"*\n\tFeatureID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"9\n\x06\x45ntity\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\x05value\x18\x02 \x01(\tB\x02\x18\x01\x12\x0e\n\x06values\x18\x03 \x03(\t\"\xba\x02\n\x05Value\x12\x13\n\tstr_value\x18\x01 \x01(\tH\x00\x12\x13\n\tint_value\x18\x02 \x01(\x05H\x00\x12\x15\n\x0b\x66loat_value\x18\x03 \x01(\x02H\x00\x12\x16\n\x0c\x64ouble_value\x18\x04 \x01(\x01H\x00\x12\x15\n\x0bint64_value\x18\x05 \x01(\x03H\x00\x12\x15\n\x0bint32_value\x18\x06 \x01(\x05H\x00\x12\x14\n\nbool_value\x18\x07 \x01(\x08H\x00\x12\x1c\n\x12on_demand_function\x18\x08 \x01(\x0cH\x00\x12=\n\x0evector32_value\x18\t \x01(\x0b\x32#.featureform.serving.proto.Vector32H\x00\x12\x16\n\x0cuint32_value\x18\n \x01(\rH\x00\x12\x16\n\x0cuint64_value\x18\x0b \x01(\x04H\x00\x42\x07\n\x05value\")\n\x08SourceID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"S\n\x11SourceDataRequest\x12/\n\x02id\x18\x01 \x01(\x0b\x32#.featureform.serving.proto.SourceID\x12\r\n\x05limit\x18\x02 \x01(\x03\"F\n\x13SourceColumnRequest\x12/\n\x02id\x18\x01 \x01(\x0b\x32#.featureform.serving.proto.SourceID\"H\n\x0eSourceDataRows\x12\x36\n\x04rows\x18\x01 \x03(\x0b\x32(.featureform.serving.proto.SourceDataRow\"?\n\rSourceDataRow\x12.\n\x04rows\x18\x01 \x03(\x0b\x32 .featureform.serving.proto.Value\"$\n\x11SourceDataColumns\x12\x0f\n\x07\x63olumns\x18\x01 \x03(\t\"S\n\x1aTrainingDataColumnsRequest\x12\x35\n\x02id\x18\x01 \x01(\x0b\x32).featureform.serving.proto.TrainingDataID\"2\n\x0fTrainingColumns\x12\x10\n\x08\x66\x65\x61tures\x18\x01 \x03(\t\x12\r\n\x05label\x18\x02 \x01(\t\"\x19\n\x08Vector32\x12\r\n\x05value\x18\x01 \x03(\x02\"\x82\x01\n\x0eNearestRequest\x12\x30\n\x02id\x18\x01 \x01(\x0b\x32$.featureform.serving.proto.FeatureID\x12\x33\n\x06vector\x18\x02 \x01(\x0b\x32#.featureform.serving.proto.Vector32\x12\t\n\x01k\x18\x03 \x01(\x05\"#\n\x0fNearestResponse\x12\x10\n\x08\x65ntities\x18\x01 \x03(\t\"@\n\x11ResourceIdRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\x05\"$\n\x10ResourceLocation\x12\x10\n\x08location\x18\x01 \x01(\t\"\x9f\x02\n\x15TrainTestSplitRequest\x12\x35\n\x02id\x18\x01 \x01(\x0b\x32).featureform.serving.proto.TrainingDataID\x12/\n\x05model\x18\x02 \x01(\x0b\x32 .featureform.serving.proto.Model\x12\x11\n\ttest_size\x18\x03 \x01(\x02\x12\x12\n\ntrain_size\x18\x04 \x01(\x02\x12\x0f\n\x07shuffle\x18\x05 \x01(\x08\x12\x14\n\x0crandom_state\x18\x06 \x01(\x05\x12<\n\x0crequest_type\x18\x07 \x01(\x0e\x32&.featureform.serving.proto.RequestType\x12\x12\n\nbatch_size\x18\x08 \x01(\x05\"\xd0\x01\n\x1b\x42\x61tchTrainTestSplitResponse\x12<\n\x0crequest_type\x18\x01 \x01(\x0e\x32&.featureform.serving.proto.RequestType\x12\x15\n\riterator_done\x18\x02 \x01(\x08\x12\x15\n\x0binitialized\x18\x03 \x01(\x08H\x00\x12;\n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32+.featureform.serving.proto.TrainingDataRowsH\x00\x42\x08\n\x06result*5\n\x0bRequestType\x12\x0e\n\nINITIALIZE\x10\x00\x12\x0c\n\x08TRAINING\x10\x01\x12\x08\n\x04TEST\x10\x02\x32\x91\x08\n\x07\x46\x65\x61ture\x12o\n\x0cTrainingData\x12..featureform.serving.proto.TrainingDataRequest\x1a+.featureform.serving.proto.TrainingDataRows\"\x00\x30\x01\x12\x80\x01\n\x0eTrainTestSplit\x12\x30.featureform.serving.proto.TrainTestSplitRequest\x1a\x36.featureform.serving.proto.BatchTrainTestSplitResponse\"\x00(\x01\x30\x01\x12z\n\x13TrainingDataColumns\x12\x35.featureform.serving.proto.TrainingDataColumnsRequest\x1a*.featureform.serving.proto.TrainingColumns\"\x00\x12g\n\x0c\x46\x65\x61tureServe\x12..featureform.serving.proto.FeatureServeRequest\x1a%.featureform.serving.proto.FeatureRow\"\x00\x12i\n\nSourceData\x12,.featureform.serving.proto.SourceDataRequest\x1a).featureform.serving.proto.SourceDataRows\"\x00\x30\x01\x12o\n\rSourceColumns\x12..featureform.serving.proto.SourceColumnRequest\x1a,.featureform.serving.proto.SourceDataColumns\"\x00\x12\x62\n\x07Nearest\x12).featureform.serving.proto.NearestRequest\x1a*.featureform.serving.proto.NearestResponse\"\x00\x12y\n\x11\x42\x61tchFeatureServe\x12\x33.featureform.serving.proto.BatchFeatureServeRequest\x1a+.featureform.serving.proto.BatchFeatureRows\"\x00\x30\x01\x12r\n\x13GetResourceLocation\x12,.featureform.serving.proto.ResourceIdRequest\x1a+.featureform.serving.proto.ResourceLocation\"\x00\x42\x1eZ\x1cgithub.com/featureform/protob\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'featureform.proto.serving_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'Z\034github.com/featureform/proto'
   _globals['_FEATUREROW'].fields_by_name['values']._options = None
   _globals['_FEATUREROW'].fields_by_name['values']._serialized_options = b'\030\001'
   _globals['_ENTITY'].fields_by_name['value']._options = None
   _globals['_ENTITY'].fields_by_name['value']._serialized_options = b'\030\001'
-  _globals['_REQUESTTYPE']._serialized_start=2698
-  _globals['_REQUESTTYPE']._serialized_end=2751
+  _globals['_REQUESTTYPE']._serialized_start=2850
+  _globals['_REQUESTTYPE']._serialized_end=2903
   _globals['_MODEL']._serialized_start=62
   _globals['_MODEL']._serialized_end=83
   _globals['_TRAININGDATAREQUEST']._serialized_start=85
   _globals['_TRAININGDATAREQUEST']._serialized_end=210
   _globals['_TRAININGDATAID']._serialized_start=212
   _globals['_TRAININGDATAID']._serialized_end=259
-  _globals['_TRAININGDATAROW']._serialized_start=261
-  _globals['_TRAININGDATAROW']._serialized_end=379
-  _globals['_FEATURESERVEREQUEST']._serialized_start=382
-  _globals['_FEATURESERVEREQUEST']._serialized_end=561
-  _globals['_FEATUREROW']._serialized_start=563
-  _globals['_FEATUREROW']._serialized_end=688
-  _globals['_VALUELIST']._serialized_start=690
-  _globals['_VALUELIST']._serialized_end=751
-  _globals['_BATCHFEATURESERVEREQUEST']._serialized_start=753
-  _globals['_BATCHFEATURESERVEREQUEST']._serialized_end=835
-  _globals['_BATCHFEATUREROW']._serialized_start=837
-  _globals['_BATCHFEATUREROW']._serialized_end=956
-  _globals['_FEATUREID']._serialized_start=958
-  _globals['_FEATUREID']._serialized_end=1000
-  _globals['_ENTITY']._serialized_start=1002
-  _globals['_ENTITY']._serialized_end=1059
-  _globals['_VALUE']._serialized_start=1062
-  _globals['_VALUE']._serialized_end=1376
-  _globals['_SOURCEID']._serialized_start=1378
-  _globals['_SOURCEID']._serialized_end=1419
-  _globals['_SOURCEDATAREQUEST']._serialized_start=1421
-  _globals['_SOURCEDATAREQUEST']._serialized_end=1504
-  _globals['_SOURCECOLUMNREQUEST']._serialized_start=1506
-  _globals['_SOURCECOLUMNREQUEST']._serialized_end=1576
-  _globals['_SOURCEDATAROW']._serialized_start=1578
-  _globals['_SOURCEDATAROW']._serialized_end=1641
-  _globals['_SOURCEDATACOLUMNS']._serialized_start=1643
-  _globals['_SOURCEDATACOLUMNS']._serialized_end=1679
-  _globals['_TRAININGDATACOLUMNSREQUEST']._serialized_start=1681
-  _globals['_TRAININGDATACOLUMNSREQUEST']._serialized_end=1764
-  _globals['_TRAININGCOLUMNS']._serialized_start=1766
-  _globals['_TRAININGCOLUMNS']._serialized_end=1816
-  _globals['_VECTOR32']._serialized_start=1818
-  _globals['_VECTOR32']._serialized_end=1843
-  _globals['_NEARESTREQUEST']._serialized_start=1846
-  _globals['_NEARESTREQUEST']._serialized_end=1976
-  _globals['_NEARESTRESPONSE']._serialized_start=1978
-  _globals['_NEARESTRESPONSE']._serialized_end=2013
-  _globals['_RESOURCEIDREQUEST']._serialized_start=2015
-  _globals['_RESOURCEIDREQUEST']._serialized_end=2079
-  _globals['_RESOURCELOCATION']._serialized_start=2081
-  _globals['_RESOURCELOCATION']._serialized_end=2117
-  _globals['_TRAINTESTSPLITREQUEST']._serialized_start=2120
-  _globals['_TRAINTESTSPLITREQUEST']._serialized_end=2407
-  _globals['_BATCHTRAINTESTSPLITRESPONSE']._serialized_start=2410
-  _globals['_BATCHTRAINTESTSPLITRESPONSE']._serialized_end=2618
-  _globals['_TRAININGDATAROWS']._serialized_start=2620
-  _globals['_TRAININGDATAROWS']._serialized_end=2696
-  _globals['_FEATURE']._serialized_start=2754
-  _globals['_FEATURE']._serialized_end=3792
+  _globals['_TRAININGDATAROWS']._serialized_start=261
+  _globals['_TRAININGDATAROWS']._serialized_end=337
+  _globals['_TRAININGDATAROW']._serialized_start=339
+  _globals['_TRAININGDATAROW']._serialized_end=457
+  _globals['_FEATURESERVEREQUEST']._serialized_start=460
+  _globals['_FEATURESERVEREQUEST']._serialized_end=639
+  _globals['_FEATUREROW']._serialized_start=641
+  _globals['_FEATUREROW']._serialized_end=766
+  _globals['_VALUELIST']._serialized_start=768
+  _globals['_VALUELIST']._serialized_end=829
+  _globals['_BATCHFEATURESERVEREQUEST']._serialized_start=831
+  _globals['_BATCHFEATURESERVEREQUEST']._serialized_end=913
+  _globals['_BATCHFEATUREROWS']._serialized_start=915
+  _globals['_BATCHFEATUREROWS']._serialized_end=991
+  _globals['_BATCHFEATUREROW']._serialized_start=993
+  _globals['_BATCHFEATUREROW']._serialized_end=1112
+  _globals['_FEATUREID']._serialized_start=1114
+  _globals['_FEATUREID']._serialized_end=1156
+  _globals['_ENTITY']._serialized_start=1158
+  _globals['_ENTITY']._serialized_end=1215
+  _globals['_VALUE']._serialized_start=1218
+  _globals['_VALUE']._serialized_end=1532
+  _globals['_SOURCEID']._serialized_start=1534
+  _globals['_SOURCEID']._serialized_end=1575
+  _globals['_SOURCEDATAREQUEST']._serialized_start=1577
+  _globals['_SOURCEDATAREQUEST']._serialized_end=1660
+  _globals['_SOURCECOLUMNREQUEST']._serialized_start=1662
+  _globals['_SOURCECOLUMNREQUEST']._serialized_end=1732
+  _globals['_SOURCEDATAROWS']._serialized_start=1734
+  _globals['_SOURCEDATAROWS']._serialized_end=1806
+  _globals['_SOURCEDATAROW']._serialized_start=1808
+  _globals['_SOURCEDATAROW']._serialized_end=1871
+  _globals['_SOURCEDATACOLUMNS']._serialized_start=1873
+  _globals['_SOURCEDATACOLUMNS']._serialized_end=1909
+  _globals['_TRAININGDATACOLUMNSREQUEST']._serialized_start=1911
+  _globals['_TRAININGDATACOLUMNSREQUEST']._serialized_end=1994
+  _globals['_TRAININGCOLUMNS']._serialized_start=1996
+  _globals['_TRAININGCOLUMNS']._serialized_end=2046
+  _globals['_VECTOR32']._serialized_start=2048
+  _globals['_VECTOR32']._serialized_end=2073
+  _globals['_NEARESTREQUEST']._serialized_start=2076
+  _globals['_NEARESTREQUEST']._serialized_end=2206
+  _globals['_NEARESTRESPONSE']._serialized_start=2208
+  _globals['_NEARESTRESPONSE']._serialized_end=2243
+  _globals['_RESOURCEIDREQUEST']._serialized_start=2245
+  _globals['_RESOURCEIDREQUEST']._serialized_end=2309
+  _globals['_RESOURCELOCATION']._serialized_start=2311
+  _globals['_RESOURCELOCATION']._serialized_end=2347
+  _globals['_TRAINTESTSPLITREQUEST']._serialized_start=2350
+  _globals['_TRAINTESTSPLITREQUEST']._serialized_end=2637
+  _globals['_BATCHTRAINTESTSPLITRESPONSE']._serialized_start=2640
+  _globals['_BATCHTRAINTESTSPLITRESPONSE']._serialized_end=2848
+  _globals['_FEATURE']._serialized_start=2906
+  _globals['_FEATURE']._serialized_end=3947
 # @@protoc_insertion_point(module_scope)
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/proto/serving_pb2.pyi` & `featureform_enterprise-0.14.4/src/featureform/proto/serving_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,30 @@
         version: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing.Literal["name", b"name", "version", b"version"]) -> None: ...
 
 global___TrainingDataID = TrainingDataID
 
 @typing.final
+class TrainingDataRows(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    ROWS_FIELD_NUMBER: builtins.int
+    @property
+    def rows(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TrainingDataRow]: ...
+    def __init__(
+        self,
+        *,
+        rows: collections.abc.Iterable[global___TrainingDataRow] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing.Literal["rows", b"rows"]) -> None: ...
+
+global___TrainingDataRows = TrainingDataRows
+
+@typing.final
 class TrainingDataRow(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FEATURES_FIELD_NUMBER: builtins.int
     LABEL_FIELD_NUMBER: builtins.int
     @property
     def features(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Value]: ...
@@ -194,14 +210,30 @@
         features: collections.abc.Iterable[global___FeatureID] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing.Literal["features", b"features"]) -> None: ...
 
 global___BatchFeatureServeRequest = BatchFeatureServeRequest
 
 @typing.final
+class BatchFeatureRows(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    ROWS_FIELD_NUMBER: builtins.int
+    @property
+    def rows(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___BatchFeatureRow]: ...
+    def __init__(
+        self,
+        *,
+        rows: collections.abc.Iterable[global___BatchFeatureRow] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing.Literal["rows", b"rows"]) -> None: ...
+
+global___BatchFeatureRows = BatchFeatureRows
+
+@typing.final
 class BatchFeatureRow(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ENTITY_FIELD_NUMBER: builtins.int
     FEATURES_FIELD_NUMBER: builtins.int
     @property
     def entity(self) -> global___Value: ...
@@ -359,14 +391,30 @@
     ) -> None: ...
     def HasField(self, field_name: typing.Literal["id", b"id"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing.Literal["id", b"id"]) -> None: ...
 
 global___SourceColumnRequest = SourceColumnRequest
 
 @typing.final
+class SourceDataRows(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    ROWS_FIELD_NUMBER: builtins.int
+    @property
+    def rows(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SourceDataRow]: ...
+    def __init__(
+        self,
+        *,
+        rows: collections.abc.Iterable[global___SourceDataRow] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing.Literal["rows", b"rows"]) -> None: ...
+
+global___SourceDataRows = SourceDataRows
+
+@typing.final
 class SourceDataRow(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ROWS_FIELD_NUMBER: builtins.int
     @property
     def rows(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Value]: ...
     def __init__(
@@ -583,23 +631,7 @@
         data: global___TrainingDataRows | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing.Literal["data", b"data", "initialized", b"initialized", "result", b"result"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing.Literal["data", b"data", "initialized", b"initialized", "iterator_done", b"iterator_done", "request_type", b"request_type", "result", b"result"]) -> None: ...
     def WhichOneof(self, oneof_group: typing.Literal["result", b"result"]) -> typing.Literal["initialized", "data"] | None: ...
 
 global___BatchTrainTestSplitResponse = BatchTrainTestSplitResponse
-
-@typing.final
-class TrainingDataRows(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    ROWS_FIELD_NUMBER: builtins.int
-    @property
-    def rows(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TrainingDataRow]: ...
-    def __init__(
-        self,
-        *,
-        rows: collections.abc.Iterable[global___TrainingDataRow] | None = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing.Literal["rows", b"rows"]) -> None: ...
-
-global___TrainingDataRows = TrainingDataRows
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/proto/serving_pb2_grpc.py` & `featureform_enterprise-0.14.4/src/featureform/proto/serving_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         Args:
             channel: A grpc.Channel.
         """
         self.TrainingData = channel.unary_stream(
                 '/featureform.serving.proto.Feature/TrainingData',
                 request_serializer=featureform_dot_proto_dot_serving__pb2.TrainingDataRequest.SerializeToString,
-                response_deserializer=featureform_dot_proto_dot_serving__pb2.TrainingDataRow.FromString,
+                response_deserializer=featureform_dot_proto_dot_serving__pb2.TrainingDataRows.FromString,
                 )
         self.TrainTestSplit = channel.stream_stream(
                 '/featureform.serving.proto.Feature/TrainTestSplit',
                 request_serializer=featureform_dot_proto_dot_serving__pb2.TrainTestSplitRequest.SerializeToString,
                 response_deserializer=featureform_dot_proto_dot_serving__pb2.BatchTrainTestSplitResponse.FromString,
                 )
         self.TrainingDataColumns = channel.unary_unary(
@@ -33,30 +33,30 @@
                 '/featureform.serving.proto.Feature/FeatureServe',
                 request_serializer=featureform_dot_proto_dot_serving__pb2.FeatureServeRequest.SerializeToString,
                 response_deserializer=featureform_dot_proto_dot_serving__pb2.FeatureRow.FromString,
                 )
         self.SourceData = channel.unary_stream(
                 '/featureform.serving.proto.Feature/SourceData',
                 request_serializer=featureform_dot_proto_dot_serving__pb2.SourceDataRequest.SerializeToString,
-                response_deserializer=featureform_dot_proto_dot_serving__pb2.SourceDataRow.FromString,
+                response_deserializer=featureform_dot_proto_dot_serving__pb2.SourceDataRows.FromString,
                 )
         self.SourceColumns = channel.unary_unary(
                 '/featureform.serving.proto.Feature/SourceColumns',
                 request_serializer=featureform_dot_proto_dot_serving__pb2.SourceColumnRequest.SerializeToString,
                 response_deserializer=featureform_dot_proto_dot_serving__pb2.SourceDataColumns.FromString,
                 )
         self.Nearest = channel.unary_unary(
                 '/featureform.serving.proto.Feature/Nearest',
                 request_serializer=featureform_dot_proto_dot_serving__pb2.NearestRequest.SerializeToString,
                 response_deserializer=featureform_dot_proto_dot_serving__pb2.NearestResponse.FromString,
                 )
         self.BatchFeatureServe = channel.unary_stream(
                 '/featureform.serving.proto.Feature/BatchFeatureServe',
                 request_serializer=featureform_dot_proto_dot_serving__pb2.BatchFeatureServeRequest.SerializeToString,
-                response_deserializer=featureform_dot_proto_dot_serving__pb2.BatchFeatureRow.FromString,
+                response_deserializer=featureform_dot_proto_dot_serving__pb2.BatchFeatureRows.FromString,
                 )
         self.GetResourceLocation = channel.unary_unary(
                 '/featureform.serving.proto.Feature/GetResourceLocation',
                 request_serializer=featureform_dot_proto_dot_serving__pb2.ResourceIdRequest.SerializeToString,
                 response_deserializer=featureform_dot_proto_dot_serving__pb2.ResourceLocation.FromString,
                 )
 
@@ -120,15 +120,15 @@
 
 
 def add_FeatureServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'TrainingData': grpc.unary_stream_rpc_method_handler(
                     servicer.TrainingData,
                     request_deserializer=featureform_dot_proto_dot_serving__pb2.TrainingDataRequest.FromString,
-                    response_serializer=featureform_dot_proto_dot_serving__pb2.TrainingDataRow.SerializeToString,
+                    response_serializer=featureform_dot_proto_dot_serving__pb2.TrainingDataRows.SerializeToString,
             ),
             'TrainTestSplit': grpc.stream_stream_rpc_method_handler(
                     servicer.TrainTestSplit,
                     request_deserializer=featureform_dot_proto_dot_serving__pb2.TrainTestSplitRequest.FromString,
                     response_serializer=featureform_dot_proto_dot_serving__pb2.BatchTrainTestSplitResponse.SerializeToString,
             ),
             'TrainingDataColumns': grpc.unary_unary_rpc_method_handler(
@@ -140,30 +140,30 @@
                     servicer.FeatureServe,
                     request_deserializer=featureform_dot_proto_dot_serving__pb2.FeatureServeRequest.FromString,
                     response_serializer=featureform_dot_proto_dot_serving__pb2.FeatureRow.SerializeToString,
             ),
             'SourceData': grpc.unary_stream_rpc_method_handler(
                     servicer.SourceData,
                     request_deserializer=featureform_dot_proto_dot_serving__pb2.SourceDataRequest.FromString,
-                    response_serializer=featureform_dot_proto_dot_serving__pb2.SourceDataRow.SerializeToString,
+                    response_serializer=featureform_dot_proto_dot_serving__pb2.SourceDataRows.SerializeToString,
             ),
             'SourceColumns': grpc.unary_unary_rpc_method_handler(
                     servicer.SourceColumns,
                     request_deserializer=featureform_dot_proto_dot_serving__pb2.SourceColumnRequest.FromString,
                     response_serializer=featureform_dot_proto_dot_serving__pb2.SourceDataColumns.SerializeToString,
             ),
             'Nearest': grpc.unary_unary_rpc_method_handler(
                     servicer.Nearest,
                     request_deserializer=featureform_dot_proto_dot_serving__pb2.NearestRequest.FromString,
                     response_serializer=featureform_dot_proto_dot_serving__pb2.NearestResponse.SerializeToString,
             ),
             'BatchFeatureServe': grpc.unary_stream_rpc_method_handler(
                     servicer.BatchFeatureServe,
                     request_deserializer=featureform_dot_proto_dot_serving__pb2.BatchFeatureServeRequest.FromString,
-                    response_serializer=featureform_dot_proto_dot_serving__pb2.BatchFeatureRow.SerializeToString,
+                    response_serializer=featureform_dot_proto_dot_serving__pb2.BatchFeatureRows.SerializeToString,
             ),
             'GetResourceLocation': grpc.unary_unary_rpc_method_handler(
                     servicer.GetResourceLocation,
                     request_deserializer=featureform_dot_proto_dot_serving__pb2.ResourceIdRequest.FromString,
                     response_serializer=featureform_dot_proto_dot_serving__pb2.ResourceLocation.SerializeToString,
             ),
     }
@@ -185,15 +185,15 @@
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_stream(request, target, '/featureform.serving.proto.Feature/TrainingData',
             featureform_dot_proto_dot_serving__pb2.TrainingDataRequest.SerializeToString,
-            featureform_dot_proto_dot_serving__pb2.TrainingDataRow.FromString,
+            featureform_dot_proto_dot_serving__pb2.TrainingDataRows.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def TrainTestSplit(request_iterator,
             target,
             options=(),
@@ -253,15 +253,15 @@
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_stream(request, target, '/featureform.serving.proto.Feature/SourceData',
             featureform_dot_proto_dot_serving__pb2.SourceDataRequest.SerializeToString,
-            featureform_dot_proto_dot_serving__pb2.SourceDataRow.FromString,
+            featureform_dot_proto_dot_serving__pb2.SourceDataRows.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def SourceColumns(request,
             target,
             options=(),
@@ -304,15 +304,15 @@
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_stream(request, target, '/featureform.serving.proto.Feature/BatchFeatureServe',
             featureform_dot_proto_dot_serving__pb2.BatchFeatureServeRequest.SerializeToString,
-            featureform_dot_proto_dot_serving__pb2.BatchFeatureRow.FromString,
+            featureform_dot_proto_dot_serving__pb2.BatchFeatureRows.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def GetResourceLocation(request,
             target,
             options=(),
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/register.py` & `featureform_enterprise-0.14.4/src/featureform/register.py`

 * *Files 0% similar despite different names*

```diff
@@ -1969,14 +1969,18 @@
 
         Args:
             name (str): Name of Redis provider to be retrieved
 
         Returns:
             redis (OnlineProvider): Provider
         """
+        warnings.warn(
+                "Use client.get_redis instead",
+                DeprecationWarning,
+            )
         mock_config = RedisConfig(host="", port=123, password="", db=123)
         mock_provider = Provider(
             name=name, function="ONLINE", description="", team="", config=mock_config
         )
         return OnlineProvider(self, mock_provider)
 
     def get_dynamodb(self, name: str):
@@ -1997,14 +2001,18 @@
 
         Args:
             name (str): Name of DynamoDB provider to be retrieved
 
         Returns:
             dynamodb (OnlineProvider): Provider
         """
+        warnings.warn(
+                "Use client.get_dynamodb instead",
+                DeprecationWarning,
+            )
         mock_config = DynamodbConfig(
             region="", access_key="", secret_key="", should_import_from_s3=False
         )
         mock_provider = Provider(
             name=name, function="ONLINE", description="", team="", config=mock_config
         )
         return OnlineProvider(self, mock_provider)
@@ -2028,14 +2036,18 @@
 
         Args:
             name (str): Name of MongoDB provider to be retrieved
 
         Returns:
             mongodb (OnlineProvider): Provider
         """
+        warnings.warn(
+                "Use client.get_mongodb instead",
+                DeprecationWarning,
+            )
         mock_config = MongoDBConfig(
             username="", password="", host="", port="", database="", throughput=1
         )
         mock_provider = Provider(
             name=name, function="ONLINE", description="", team="", config=mock_config
         )
         return OnlineProvider(self, mock_provider)
@@ -2059,14 +2071,18 @@
 
         Args:
             name (str): Name of Azure blob provider to be retrieved
 
         Returns:
             azure_blob (FileStoreProvider): Provider
         """
+        warnings.warn(
+                "Use client.get_blob_store instead",
+                DeprecationWarning,
+            )
         fake_azure_config = AzureFileStoreConfig(
             account_name="", account_key="", container_name="", root_path=""
         )
         fake_config = OnlineBlobConfig(
             store_type="AZURE", store_config=fake_azure_config.config()
         )
         mock_provider = Provider(
@@ -2090,14 +2106,18 @@
 
         Args:
             name (str): Name of Postgres provider to be retrieved
 
         Returns:
             postgres (OfflineSQLProvider): Provider
         """
+        warnings.warn(
+                "Use client.get_postgres instead",
+                DeprecationWarning,
+            )
         mock_config = PostgresConfig(
             host="",
             port="",
             database="",
             user="",
             password="",
             sslmode="",
@@ -2123,14 +2143,18 @@
 
         Args:
             name (str): Name of ClickHouse provider to be retrieved
 
         Returns:
             clickhouse (OfflineSQLProvider): Provider
         """
+        warnings.warn(
+                "Use client.get_clickhouse instead",
+                DeprecationWarning,
+            )
         mock_config = ClickHouseConfig(
             host="",
             port=9000,
             database="",
             user="",
             password="",
             ssl=False,
@@ -2156,14 +2180,18 @@
 
         Args:
             name (str): Name of Snowflake provider to be retrieved
 
         Returns:
             snowflake (OfflineSQLProvider): Provider
         """
+        warnings.warn(
+                "Use client.get_snowflake instead",
+                DeprecationWarning,
+            )
         mock_config = SnowflakeConfig(
             account="ff_fake",
             database="ff_fake",
             organization="ff_fake",
             username="ff_fake",
             password="ff_fake",
             schema="ff_fake",
@@ -2189,14 +2217,18 @@
 
         Args:
             name (str): Name of Snowflake provider to be retrieved
 
         Returns:
             snowflake_legacy (OfflineSQLProvider): Provider
         """
+        warnings.warn(
+                "Use client.get_snowflake_legacy instead",
+                DeprecationWarning,
+            )
         mock_config = SnowflakeConfig(
             account_locator="ff_fake",
             database="ff_fake",
             username="ff_fake",
             password="ff_fake",
             schema="ff_fake",
             warehouse="ff_fake",
@@ -2223,14 +2255,18 @@
 
         Args:
             name (str): Name of Redshift provider to be retrieved
 
         Returns:
             redshift (OfflineSQLProvider): Provider
         """
+        warnings.warn(
+                "Use client.get_redshift instead",
+                DeprecationWarning,
+            )
         mock_config = RedshiftConfig(
             host="", port="5439", database="", user="", password="", sslmode=""
         )
         mock_provider = Provider(
             name=name, function="OFFLINE", description="", team="", config=mock_config
         )
         return OfflineSQLProvider(self, mock_provider)
@@ -2251,14 +2287,18 @@
 
         Args:
             name (str): Name of BigQuery provider to be retrieved
 
         Returns:
             bigquery (OfflineSQLProvider): Provider
         """
+        warnings.warn(
+                "Use client.get_bigquery instead",
+                DeprecationWarning,
+            )
         mock_config = BigQueryConfig(
             project_id="mock_project",
             dataset_id="mock_dataset",
             credentials=GCPCredentials(
                 project_id="mock_project",
                 credentials_path="client/tests/test_files/bigquery_dummy_credentials.json",
             ),
@@ -2284,14 +2324,18 @@
 
         Args:
             name (str): Name of Spark provider to be retrieved
 
         Returns:
             spark (OfflineSQLProvider): Provider
         """
+        warnings.warn(
+                "Use client.get_spark instead",
+                DeprecationWarning,
+            )
         mock_config = SparkConfig(
             executor_type="", executor_config={}, store_type="", store_config={}
         )
         mock_provider = Provider(
             name=name, function="OFFLINE", description="", team="", config=mock_config
         )
         return OfflineSparkProvider(self, mock_provider)
@@ -2314,14 +2358,18 @@
 
         Args:
             name (str): Name of k8s provider to be retrieved
 
         Returns:
             k8s (OfflineK8sProvider): Provider
         """
+        warnings.warn(
+                "Use client.get_kubernetes instead",
+                DeprecationWarning,
+            )
         mock_config = K8sConfig(store_type="", store_config={})
         mock_provider = Provider(
             name=name, function="OFFLINE", description="", team="", config=mock_config
         )
         return OfflineK8sProvider(self, mock_provider)
 
     def get_s3(self, name):
@@ -2344,14 +2392,18 @@
 
         Args:
             name (str): Name of S3 to be retrieved
 
         Returns:
             s3 (FileStore): Provider
         """
+        warnings.warn(
+                "Use client.get_s3 instead",
+                DeprecationWarning,
+            )
         provider = Provider(
             name=name,
             function="OFFLINE",
             description="description",
             team="team",
             config=s3_config,
         )
@@ -2359,14 +2411,18 @@
             registrar=self,
             provider=provider,
             config=s3_config,
             store_type=s3_config.type(),
         )
 
     def get_gcs(self, name):
+        warnings.warn(
+                "Use client.get_gcs instead",
+                DeprecationWarning,
+            )
         filePath = "provider/connection/mock_credentials.json"
         fake_creds = GCPCredentials(project_id="id", credentials_path=filePath)
         mock_config = GCSFileStoreConfig(
             bucket_name="", bucket_path="", credentials=fake_creds
         )
         mock_provider = Provider(
             name=name, function="OFFLINE", description="", team="", config=mock_config
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/resources.py` & `featureform_enterprise-0.14.4/src/featureform/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from datetime import timedelta
 import json
 import os
 import re
 import sys
 import uuid
+import logging
 from abc import ABC, abstractmethod
 from dataclasses import field
 from typing import List, Tuple, Union, Optional, Any, Dict
 
 import dill
 import grpc
 from google.protobuf.duration_pb2 import Duration
@@ -20,14 +21,16 @@
 
 from . import feature_flag
 from .types import VectorType, type_from_proto
 from .enums import *
 from .exceptions import *
 from .version import check_up_to_date
 
+logger = logging.getLogger(__name__)
+
 NameVariant = Tuple[str, str]
 
 # Constants for Pyspark Versions
 MAJOR_VERSION = "3"
 MINOR_VERSIONS = ["7", "8", "9", "10", "11"]
 
 
@@ -1647,16 +1650,17 @@
             provider=self.provider,
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
             status=pb.ResourceStatus(status=pb.ResourceStatus.NO_STATUS),
             max_job_duration=duration,
             **defArgs,
         )
-        _get_and_set_equivalent_variant(req_id, serialized, "source_variant", stub)
-        stub.CreateSourceVariant(serialized)
+        existing_variant = _get_and_set_equivalent_variant(req_id, serialized, "source_variant", stub)
+        if existing_variant is None:
+            stub.CreateSourceVariant(serialized)
         return serialized.variant
 
     def get_status(self):
         return ResourceStatus(self.status)
 
     def is_transformation_type(self):
         return isinstance(self.definition, Transformation)
@@ -1843,16 +1847,17 @@
             columns=self.location.proto(),
             mode=ComputationMode.PRECOMPUTED.proto(),
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
             status=pb.ResourceStatus(status=pb.ResourceStatus.NO_STATUS),
             additional_parameters=None,
         )
-        _get_and_set_equivalent_variant(req_id, serialized, "feature_variant", stub)
-        stub.CreateFeatureVariant(serialized)
+        existing_variant = _get_and_set_equivalent_variant(req_id, serialized, "feature_variant", stub)
+        if existing_variant is None:
+            stub.CreateFeatureVariant(serialized)
         return serialized.variant
 
     def get_status(self):
         return ResourceStatus(self.status)
 
     def is_ready(self):
         return self.status == ResourceStatus.READY.value
@@ -2071,16 +2076,17 @@
             function=pb.PythonFunction(query=self.query),
             mode=ComputationMode.CLIENT_COMPUTED.proto(),
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
             status=pb.ResourceStatus(status=pb.ResourceStatus.READY),
             additional_parameters=self.additional_parameters.proto(),
         )
-        _get_and_set_equivalent_variant(req_id, serialized, "feature_variant", stub)
-        stub.CreateFeatureVariant(serialized)
+        existing_variant = _get_and_set_equivalent_variant(req_id, serialized, "feature_variant", stub)
+        if existing_variant is None:
+            stub.CreateFeatureVariant(serialized)
         return serialized.variant
 
     def get(self, stub) -> "OnDemandFeatureVariant":
         name_variant = pb.NameVariant(name=self.name, variant=self.variant)
         ondemand_feature = next(stub.GetFeatureVariants(iter([name_variant])))
         additional_Parameters = self._get_additional_parameters(ondemand_feature)
 
@@ -2191,16 +2197,17 @@
             owner=self.owner,
             description=self.description,
             columns=self.location.proto(),
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
             status=pb.ResourceStatus(status=pb.ResourceStatus.NO_STATUS),
         )
-        _get_and_set_equivalent_variant(req_id, serialized, "label_variant", stub)
-        stub.CreateLabelVariant(serialized)
+        existing_variant = _get_and_set_equivalent_variant(req_id, serialized, "label_variant", stub)
+        if existing_variant is None:
+            stub.CreateLabelVariant(serialized)
         return serialized.variant
 
     def get_status(self):
         return ResourceStatus(self.status)
 
     def is_ready(self):
         return self.status == ResourceStatus.READY.value
@@ -2401,16 +2408,17 @@
             label=pb.NameVariant(name=self.label[0], variant=self.label[1]),
             feature_lags=feature_lags,
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
             status=pb.ResourceStatus(status=pb.ResourceStatus.NO_STATUS),
             provider=self.provider,
         )
-        _get_and_set_equivalent_variant(req_id, serialized, "training_set_variant", stub)
-        stub.CreateTrainingSetVariant(serialized)
+        existing_variant = _get_and_set_equivalent_variant(req_id, serialized, "training_set_variant", stub)
+        if existing_variant is None:
+            stub.CreateTrainingSetVariant(serialized)
         return serialized.variant
 
     def get_status(self):
         return ResourceStatus(self.status)
 
     def is_ready(self):
         return self.status == ResourceStatus.READY.value
@@ -2851,21 +2859,23 @@
 # and sets the serialized to it.
 #
 # i.e. for a source variant, looks for a source variant with the same name and definition
 def _get_and_set_equivalent_variant(
     req_id, resource_variant_proto, variant_field, stub
 ) -> Optional[str]:
     if feature_flag.is_enabled("FF_GET_EQUIVALENT_VARIANTS", True):
+        logger.info("Starting to get equivalent")
         # Get equivalent from stub
         equivalent = stub.GetEquivalent(
             pb.GetEquivalentRequest(
                 request_id=str(req_id),
                 variant=pb.ResourceVariant(**{variant_field: resource_variant_proto}),
             )
         )
+        logger.info("Finished get equivalent")
 
         # grpc call returns the default ResourceVariant proto when equivalent doesn't exist which explains the below check
         if equivalent != pb.ResourceVariant():
             variant_value = getattr(getattr(equivalent, variant_field), "variant")
             print(
                 f"Looks like an equivalent {variant_field.replace('_', ' ')} already exists, going to use its variant: ",
                 variant_value,
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/search.py` & `featureform_enterprise-0.14.4/src/featureform/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-import os
 import requests
 from .format import *
 
 
 def search(phrase, host):
     response = requests.get(f"http://{host}/data/search?q={phrase}")
 
-    if response.status_code is not 200:
+    if response.status_code != 200:
         print(
             f"Search request for {phrase} resulted in HTTP status {response.status_code}"
         )
         return
 
     results = response.json()
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/serving.py` & `featureform_enterprise-0.14.4/src/featureform/serving.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,17 +260,18 @@
         return pd.DataFrame(data=data, columns=columns)
 
     def _get_source_data(self, name, variant, limit):
         id = serving_pb2.SourceID(name=name, version=variant)
         req = serving_pb2.SourceDataRequest(id=id, limit=limit)
         resp = self._stub.SourceData(req)
         data = []
-        for rows in resp:
-            row = [getattr(r, r.WhichOneof("value")) for r in rows.rows]
-            data.append(row)
+        for batch in resp:
+            for rows in batch.rows:
+                row = [getattr(r, r.WhichOneof("value")) for r in rows.rows]
+                data.append(row)
         return data
 
     def _get_source_columns(self, name, variant):
         id = serving_pb2.SourceID(name=name, version=variant)
         req = serving_pb2.SourceDataRequest(id=id)
         resp = self._stub.SourceColumns(req)
         # The Python type of resp.columns is <class 'google._upb._message.RepeatedScalarContainer'>
@@ -308,20 +309,28 @@
         if model is not None:
             req.model.name = model if isinstance(model, str) else model.name
         self.name = name
         self.version = version
         self._stub = stub
         self._req = req
         self._iter = stub.TrainingData(req)
+        self._buf = []
+        self._index = 0
 
     def __iter__(self):
         return self
 
     def __next__(self):
-        return Row(next(self._iter))
+        if self._index >= len(self._buf):
+            self._buf = next(self._iter).rows
+            self._index = 0
+
+        row = Row(self._buf[self._index])
+        self._index += 1
+        return row
 
     def restart(self):
         self._iter = self._stub.TrainingData(self._req)
 
 
 class LocalStream:
     def __init__(self, datalist, include_label_timestamp):
@@ -872,20 +881,28 @@
         for name, variant in features:
             feature_id = req.features.add()
             feature_id.name = name
             feature_id.version = variant
         self._stub = stub
         self._req = req
         self._iter = stub.BatchFeatureServe(req)
+        self._buf = []
+        self._index = 0
 
     def __iter__(self):
         return self
 
     def __next__(self):
-        return FeatureSetRow(next(self._iter)).to_tuple()
+        if self._index >= len(self._buf):
+            self._buf = next(self._iter).rows
+            self._index = 0
+
+        row = FeatureSetRow(self._buf[self._index]).to_tuple()
+        self._index += 1
+        return row
 
     def restart(self):
         self._iter = self._stub.BatchFeatureServe(self._req)
 
 
 class FeatureSetRow:
     def __init__(self, proto_row):
```

### Comparing `featureform_enterprise-0.13.9/src/featureform/status_display.py` & `featureform_enterprise-0.14.4/src/featureform/status_display.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/tls.py` & `featureform_enterprise-0.14.4/src/featureform/tls.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/train_test_split.py` & `featureform_enterprise-0.14.4/src/featureform/train_test_split.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/type_objects.py` & `featureform_enterprise-0.14.4/src/featureform/type_objects.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/types.py` & `featureform_enterprise-0.14.4/src/featureform/types.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/variant_names_generator.py` & `featureform_enterprise-0.14.4/src/featureform/variant_names_generator.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/src/featureform/version.py` & `featureform_enterprise-0.14.4/src/featureform/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-import pkg_resources
-import requests
 import threading
 
+import importlib_metadata
+import requests
+
 version_check_url = "https://version.featureform.com"
 
 
 def get_package_version():
-    return pkg_resources.get_distribution("featureform-enterprise").version
+    return importlib_metadata.distribution("featureform-enterprise").version
 
 
 def check_up_to_date(local, client):
     download_thread = threading.Thread(
         target=run_version_check, name="Downloader", args=(local, client)
     )
     download_thread.start()
 
 
 def run_version_check(local, client):
     try:
         version = get_package_version()
-        requests.get(
-            version_check_url,
-            params={"local": local, "client": client, "version": version},
-        )
+        # requests.get(
+        #     version_check_url,
+        #     params={"local": local, "client": client, "version": version},
+        # )
     except:
         pass
```

### Comparing `featureform_enterprise-0.13.9/src/featureform_enterprise.egg-info/PKG-INFO` & `featureform_enterprise-0.14.4/src/featureform_enterprise.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featureform-enterprise
-Version: 0.13.9
+Version: 0.14.4
 Summary: Package for the Featureform Enterprise Feature Store
 Home-page: https://featureform.com
 Author: FeatureForm, Inc.
 Author-email: hello@featureform.com
 Project-URL: Bug Tracker, https://github.com/featureform/featureform/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -34,14 +34,15 @@
 Requires-Dist: fastparquet
 Requires-Dist: pinecone-client
 Requires-Dist: weaviate-client
 Requires-Dist: docker
 Requires-Dist: okta-jwt-verifier
 Requires-Dist: googleapis-common-protos
 Requires-Dist: uuid
+Requires-Dist: importlib-metadata
 
 # Featureform Python Client
 
 ## Overview
 
 Featureform’s Python client is a SDK for defining, managing and serving resources (e.g. infrastructure providers, data sources, transformations, etc.). At a high level, the API is divided into two parts:
```

### Comparing `featureform_enterprise-0.13.9/src/featureform_enterprise.egg-info/SOURCES.txt` & `featureform_enterprise-0.14.4/src/featureform_enterprise.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.df4e0a4839a040a1.js
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.e1a7f78fb87ff37c.js
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yang.758f2e9ec02ed81c.js
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.4ddc9ac973a0065e.js
 src/featureform/dashboard/out/_next/static/chunks/webpack-4ca33bb86fc5510e.js
 src/featureform/dashboard/out/_next/static/chunks/pages/404-8d282ae638ce5722.js
 src/featureform/dashboard/out/_next/static/chunks/pages/[type]-7bfcb609b1affd61.js
-src/featureform/dashboard/out/_next/static/chunks/pages/_app-574fe43e4223620b.js
+src/featureform/dashboard/out/_next/static/chunks/pages/_app-569252d467889e35.js
 src/featureform/dashboard/out/_next/static/chunks/pages/_error-e18771d792fd8fe7.js
 src/featureform/dashboard/out/_next/static/chunks/pages/connections-f98076127418a04b.js
 src/featureform/dashboard/out/_next/static/chunks/pages/index-142e8557e4889163.js
 src/featureform/dashboard/out/_next/static/chunks/pages/query-5a171bd499b8d4eb.js
 src/featureform/dashboard/out/_next/static/chunks/pages/search-abfa6bb494904a10.js
 src/featureform/dashboard/out/_next/static/chunks/pages/tasks-70243ca2c0452223.js
 src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-2f83fe1ff7f9d94c.js
@@ -287,20 +287,20 @@
 src/featureform/dashboard/out/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js
 src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/[groupName]-4ba8b6abfb4b13ca.js
 src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/[roleName]-a4f4cefefad41418.js
 src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/[userName]-5a66d4c05c9e7453.js
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.9d4c892d6ec3e998.js
 src/featureform/dashboard/out/_next/static/css/85a2addfd2efc882.css
 src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf
+src/featureform/dashboard/out/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_buildManifest.js
+src/featureform/dashboard/out/_next/static/tU2e0PPhQ-QR0Wjh2ilIZ/_ssgManifest.js
 src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js
 src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_ssgManifest.js
 src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js
 src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_ssgManifest.js
-src/featureform/dashboard/out/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_buildManifest.js
-src/featureform/dashboard/out/_next/static/yVmVSX0ksIXzzxWh3Ff_1/_ssgManifest.js
 src/featureform/dashboard/out/admin/groups.html
 src/featureform/dashboard/out/admin/roles.html
 src/featureform/dashboard/out/admin/users.html
 src/featureform/dashboard/out/admin/group/[groupName].html
 src/featureform/dashboard/out/admin/role/[roleName].html
 src/featureform/dashboard/out/admin/user/[userName].html
 src/featureform/dashboard/out/static/Apache_Spark_logo.svg
```

### Comparing `featureform_enterprise-0.13.9/tests/test_auth.py` & `featureform_enterprise-0.14.4/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/tests/test_autogenerated_variants.py` & `featureform_enterprise-0.14.4/tests/test_autogenerated_variants.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/tests/test_class_api.py` & `featureform_enterprise-0.14.4/tests/test_class_api.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/tests/test_cli.py` & `featureform_enterprise-0.14.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/tests/test_client.py` & `featureform_enterprise-0.14.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/tests/test_deploy.py` & `featureform_enterprise-0.14.4/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/tests/test_enums.py` & `featureform_enterprise-0.14.4/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/tests/test_executor_resources.py` & `featureform_enterprise-0.14.4/tests/test_executor_resources.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/tests/test_getting_model.py` & `featureform_enterprise-0.14.4/tests/test_getting_model.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/tests/test_multi_feature.py` & `featureform_enterprise-0.14.4/tests/test_multi_feature.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/tests/test_ondemand_features.py` & `featureform_enterprise-0.14.4/tests/test_ondemand_features.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/tests/test_parse.py` & `featureform_enterprise-0.14.4/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/tests/test_resource_registration.py` & `featureform_enterprise-0.14.4/tests/test_resource_registration.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/tests/test_search.py` & `featureform_enterprise-0.14.4/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/tests/test_serving_model.py` & `featureform_enterprise-0.14.4/tests/test_serving_model.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/tests/test_source_columns.py` & `featureform_enterprise-0.14.4/tests/test_source_columns.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/tests/test_source_dataframe.py` & `featureform_enterprise-0.14.4/tests/test_source_dataframe.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/tests/test_spark_provider.py` & `featureform_enterprise-0.14.4/tests/test_spark_provider.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/tests/test_tags_and_properties.py` & `featureform_enterprise-0.14.4/tests/test_tags_and_properties.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/tests/test_train_test_split.py` & `featureform_enterprise-0.14.4/tests/test_train_test_split.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/tests/test_training_set_dataframe.py` & `featureform_enterprise-0.14.4/tests/test_training_set_dataframe.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.9/tests/test_updating_provider.py` & `featureform_enterprise-0.14.4/tests/test_updating_provider.py`

 * *Files identical despite different names*


# Comparing `tmp/ltbams-0.9.6.tar.gz` & `tmp/ltbams-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltbams-0.9.6.tar", last modified: Sun Apr 21 21:18:22 2024, max compression
+gzip compressed data, was "ltbams-0.9.7.tar", last modified: Fri May 24 19:47:47 2024, max compression
```

## Comparing `ltbams-0.9.6.tar` & `ltbams-0.9.7.tar`

### file list

```diff
@@ -1,208 +1,213 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.208616 ltbams-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-21 21:15:52.000000 ltbams-0.9.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35918 2024-04-21 21:15:52.000000 ltbams-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-21 21:15:52.000000 ltbams-0.9.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-04-21 21:18:22.208616 ltbams-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-04-21 21:15:52.000000 ltbams-0.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.208616 ltbams-0.9.6/ams/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-21 21:18:22.208616 ltbams-0.9.6/ams/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.176617 ltbams-0.9.6/ams/cases/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.184617 ltbams-0.9.6/ams/cases/5bus/
--rw-r--r--   0 runner    (1001) docker     (127)    27546 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/5bus/pjm5bus_demo.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    18258 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/5bus/pjm5bus_uced.json
--rw-r--r--   0 runner    (1001) docker     (127)    28206 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/5bus/pjm5bus_uced.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    28070 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/5bus/pjm5bus_uced_esd1.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.184617 ltbams-0.9.6/ams/cases/ieee123/
--rw-r--r--   0 runner    (1001) docker     (127)    39223 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/ieee123/ieee123.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    41678 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/ieee123/ieee123_regcv1.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.184617 ltbams-0.9.6/ams/cases/ieee14/
--rw-r--r--   0 runner    (1001) docker     (127)    21400 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/ieee14/ieee14.json
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/ieee14/ieee14.raw
--rw-r--r--   0 runner    (1001) docker     (127)    33054 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/ieee14/ieee14_uced.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.184617 ltbams-0.9.6/ams/cases/ieee39/
--rw-r--r--   0 runner    (1001) docker     (127)    29475 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/ieee39/ieee39.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    41664 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/ieee39/ieee39_uced.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    40803 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/ieee39/ieee39_uced_esd1.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    40751 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/ieee39/ieee39_uced_pvd1.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    44914 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/ieee39/ieee39_uced_vis.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.188617 ltbams-0.9.6/ams/cases/matpower/
--rwxr-xr-x   0 runner    (1001) docker     (127)    33696 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/matpower/case118.m
--rwxr-xr-x   0 runner    (1001) docker     (127)     4597 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/matpower/case14.m
--rwxr-xr-x   0 runner    (1001) docker     (127)    65678 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/matpower/case300.m
--rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/matpower/case39.m
--rwxr-xr-x   0 runner    (1001) docker     (127)     1921 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/matpower/case5.m
--rw-r--r--   0 runner    (1001) docker     (127)   659546 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/matpower/case_ACTIVSg2000.m
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.188617 ltbams-0.9.6/ams/cases/npcc/
--rwxr-xr-x   0 runner    (1001) docker     (127)    26342 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/npcc/npcc.m
--rw-r--r--   0 runner    (1001) docker     (127)    86582 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/npcc/npcc_uced.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.188617 ltbams-0.9.6/ams/cases/pglib/
--rw-r--r--   0 runner    (1001) docker     (127)    16351 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/pglib/pglib_opf_case39_epri__api.m
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.188617 ltbams-0.9.6/ams/cases/wecc/
--rwxr-xr-x   0 runner    (1001) docker     (127)    30498 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/wecc/wecc.m
--rw-r--r--   0 runner    (1001) docker     (127)    94790 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cases/wecc/wecc_uced.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.188617 ltbams-0.9.6/ams/core/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20251 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/core/documenter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15939 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/core/matprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/core/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9529 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/core/param.py
--rw-r--r--   0 runner    (1001) docker     (127)    26910 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/core/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/core/symprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/core/var.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.188617 ltbams-0.9.6/ams/interop/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/interop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41574 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/interop/andes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.192617 ltbams-0.9.6/ams/io/
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/io/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    13887 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/io/matpower.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/io/psse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/io/pypower.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/io/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (127)    21786 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.192617 ltbams-0.9.6/ams/models/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/models/area.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/models/bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/models/cost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.192617 ltbams-0.9.6/ams/models/distributed/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/models/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/models/distributed/esd1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/models/distributed/pvd1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/models/group.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/models/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/models/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/models/region.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.192617 ltbams-0.9.6/ams/models/renewable/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/models/renewable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/models/renewable/regc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/models/reserve.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/models/shunt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.192617 ltbams-0.9.6/ams/models/static/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/models/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/models/static/gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/models/static/pq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/models/timeslot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.192617 ltbams-0.9.6/ams/opt/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29652 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/opt/omodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.192617 ltbams-0.9.6/ams/pypower/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/pypower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/pypower/_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.196617 ltbams-0.9.6/ams/pypower/core/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/pypower/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32783 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/pypower/core/pips.py
--rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/pypower/core/ppoption.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/pypower/core/ppver.py
--rw-r--r--   0 runner    (1001) docker     (127)    85083 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/pypower/core/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/pypower/eps.py
--rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/pypower/idx.py
--rw-r--r--   0 runner    (1001) docker     (127)    26368 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/pypower/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.196617 ltbams-0.9.6/ams/pypower/make/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/pypower/make/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23753 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/pypower/make/matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)    18623 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/pypower/make/pdv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.196617 ltbams-0.9.6/ams/pypower/routines/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/pypower/routines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17441 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/pypower/routines/cpf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/pypower/routines/cpf_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    73444 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/pypower/routines/opf.py
--rw-r--r--   0 runner    (1001) docker     (127)    78183 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/pypower/routines/opffcns.py
--rw-r--r--   0 runner    (1001) docker     (127)    30954 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/pypower/routines/pflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    50142 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/pypower/toggle.py
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/pypower/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.196617 ltbams-0.9.6/ams/routines/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/routines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/routines/acopf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/routines/cpf.py
--rw-r--r--   0 runner    (1001) docker     (127)    15971 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/routines/dcopf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/routines/dcpf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/routines/dopf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/routines/ed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/routines/pflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    31954 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/routines/routine.py
--rw-r--r--   0 runner    (1001) docker     (127)    24714 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/routines/rted.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/routines/type.py
--rw-r--r--   0 runner    (1001) docker     (127)    15429 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/routines/uc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)    22858 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.196617 ltbams-0.9.6/ams/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-21 21:15:52.000000 ltbams-0.9.6/ams/utils/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.196617 ltbams-0.9.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.200616 ltbams-0.9.6/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.180616 ltbams-0.9.6/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.200616 ltbams-0.9.6/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/_templates/autosummary/module_toctree.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.200616 ltbams-0.9.6/docs/source/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/examples/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.200616 ltbams-0.9.6/docs/source/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/getting_started/copyright.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.200616 ltbams-0.9.6/docs/source/getting_started/formats/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/getting_started/formats/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17425 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/getting_started/formats/matpower.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/getting_started/formats/psse.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/getting_started/formats/pypower.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)   171220 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/getting_started/formats/xlsx.png
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/getting_started/formats/xlsx.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/getting_started/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/getting_started/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/getting_started/testcase.rst
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/getting_started/verification.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.200616 ltbams-0.9.6/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (127)    52102 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/images/dcopf_time.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.204616 ltbams-0.9.6/docs/source/images/sponsors/
--rw-r--r--   0 runner    (1001) docker     (127)    87680 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/images/sponsors/CURENT_Logo_NameOnTrans.png
--rw-r--r--   0 runner    (1001) docker     (127)    59336 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/images/sponsors/CURENT_Logo_Transparent.png
--rw-r--r--   0 runner    (1001) docker     (127)   837476 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/images/sponsors/CURENT_Logo_Transparent_Name.png
--rw-r--r--   0 runner    (1001) docker     (127)    26131 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/images/sponsors/doe.png
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.204616 ltbams-0.9.6/docs/source/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/modeling/example.rst
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/modeling/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/modeling/model.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/modeling/routine.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/modeling/system.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-21 21:15:52.000000 ltbams-0.9.6/docs/source/release-notes.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.204616 ltbams-0.9.6/ltbams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-04-21 21:18:22.000000 ltbams-0.9.6/ltbams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-21 21:18:22.000000 ltbams-0.9.6/ltbams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 21:18:22.000000 ltbams-0.9.6/ltbams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 21:18:22.000000 ltbams-0.9.6/ltbams.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-21 21:18:22.000000 ltbams-0.9.6/ltbams.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 21:18:22.000000 ltbams-0.9.6/ltbams.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-21 21:15:52.000000 ltbams-0.9.6/requirements-extra.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-21 21:15:52.000000 ltbams-0.9.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-21 21:18:22.208616 ltbams-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-21 21:15:52.000000 ltbams-0.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:18:22.208616 ltbams-0.9.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 21:15:52.000000 ltbams-0.9.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-21 21:15:52.000000 ltbams-0.9.6/tests/test_1st_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-21 21:15:52.000000 ltbams-0.9.6/tests/test_addressing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8156 2024-04-21 21:15:52.000000 ltbams-0.9.6/tests/test_andes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7778 2024-04-21 21:15:52.000000 ltbams-0.9.6/tests/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-21 21:15:52.000000 ltbams-0.9.6/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-21 21:15:52.000000 ltbams-0.9.6/tests/test_dctypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-21 21:15:52.000000 ltbams-0.9.6/tests/test_export_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-21 21:15:52.000000 ltbams-0.9.6/tests/test_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-21 21:15:52.000000 ltbams-0.9.6/tests/test_known_good.py
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-21 21:15:52.000000 ltbams-0.9.6/tests/test_mats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-21 21:15:52.000000 ltbams-0.9.6/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-21 21:15:52.000000 ltbams-0.9.6/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-21 21:15:52.000000 ltbams-0.9.6/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-21 21:15:52.000000 ltbams-0.9.6/tests/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-04-21 21:15:52.000000 ltbams-0.9.6/tests/test_routine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-21 21:15:52.000000 ltbams-0.9.6/tests/test_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    81189 2024-04-21 21:15:52.000000 ltbams-0.9.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.715768 ltbams-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-24 19:45:15.000000 ltbams-0.9.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35922 2024-05-24 19:45:15.000000 ltbams-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-24 19:45:15.000000 ltbams-0.9.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-05-24 19:47:47.715768 ltbams-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-05-24 19:45:15.000000 ltbams-0.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.715768 ltbams-0.9.7/ams/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-24 19:47:47.715768 ltbams-0.9.7/ams/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.687768 ltbams-0.9.7/ams/cases/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.691768 ltbams-0.9.7/ams/cases/5bus/
+-rw-r--r--   0 runner    (1001) docker     (127)    27546 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/5bus/pjm5bus_demo.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    18258 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/5bus/pjm5bus_uced.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28206 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/5bus/pjm5bus_uced.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    28070 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/5bus/pjm5bus_uced_esd1.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    29722 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/5bus/pjm5bus_uced_ev.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.691768 ltbams-0.9.7/ams/cases/ieee123/
+-rw-r--r--   0 runner    (1001) docker     (127)    39223 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/ieee123/ieee123.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    41678 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/ieee123/ieee123_regcv1.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.691768 ltbams-0.9.7/ams/cases/ieee14/
+-rw-r--r--   0 runner    (1001) docker     (127)    21400 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/ieee14/ieee14.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/ieee14/ieee14.raw
+-rw-r--r--   0 runner    (1001) docker     (127)    33054 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/ieee14/ieee14_uced.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.695767 ltbams-0.9.7/ams/cases/ieee39/
+-rw-r--r--   0 runner    (1001) docker     (127)    29475 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/ieee39/ieee39.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    41664 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/ieee39/ieee39_uced.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    40803 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/ieee39/ieee39_uced_esd1.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    40751 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/ieee39/ieee39_uced_pvd1.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    44914 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/ieee39/ieee39_uced_vis.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.695767 ltbams-0.9.7/ams/cases/matpower/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    33696 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/matpower/case118.m
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4597 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/matpower/case14.m
+-rwxr-xr-x   0 runner    (1001) docker     (127)    65678 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/matpower/case300.m
+-rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/matpower/case39.m
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1921 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/matpower/case5.m
+-rw-r--r--   0 runner    (1001) docker     (127)   659546 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/matpower/case_ACTIVSg2000.m
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.695767 ltbams-0.9.7/ams/cases/npcc/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26342 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/npcc/npcc.m
+-rw-r--r--   0 runner    (1001) docker     (127)    86582 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/npcc/npcc_uced.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.695767 ltbams-0.9.7/ams/cases/pglib/
+-rw-r--r--   0 runner    (1001) docker     (127)    16351 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/pglib/pglib_opf_case39_epri__api.m
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.695767 ltbams-0.9.7/ams/cases/wecc/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30498 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/wecc/wecc.m
+-rw-r--r--   0 runner    (1001) docker     (127)    94790 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cases/wecc/wecc_uced.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.699768 ltbams-0.9.7/ams/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20251 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/core/documenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/core/matprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9529 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/core/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26912 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/core/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/core/symprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/core/var.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.699768 ltbams-0.9.7/ams/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16342 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/extension/eva.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.699768 ltbams-0.9.7/ams/interop/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/interop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41573 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/interop/andes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.699768 ltbams-0.9.7/ams/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14257 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/io/matpower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/io/psse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/io/pypower.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/io/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21786 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.699768 ltbams-0.9.7/ams/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/models/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/models/bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/models/cost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.699768 ltbams-0.9.7/ams/models/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/models/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/models/distributed/esd1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/models/distributed/ev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/models/distributed/pvd1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/models/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/models/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/models/region.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.699768 ltbams-0.9.7/ams/models/renewable/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/models/renewable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/models/renewable/regc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/models/reserve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/models/shunt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.699768 ltbams-0.9.7/ams/models/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/models/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/models/static/gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/models/static/pq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/models/timeslot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.703768 ltbams-0.9.7/ams/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29652 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/opt/omodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.703768 ltbams-0.9.7/ams/pypower/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/pypower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/pypower/_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.703768 ltbams-0.9.7/ams/pypower/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/pypower/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32783 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/pypower/core/pips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/pypower/core/ppoption.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/pypower/core/ppver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85083 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/pypower/core/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/pypower/eps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/pypower/idx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26368 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/pypower/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.703768 ltbams-0.9.7/ams/pypower/make/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/pypower/make/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23753 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/pypower/make/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18623 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/pypower/make/pdv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.703768 ltbams-0.9.7/ams/pypower/routines/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/pypower/routines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17441 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/pypower/routines/cpf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/pypower/routines/cpf_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73444 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/pypower/routines/opf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78183 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/pypower/routines/opffcns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30818 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/pypower/routines/pflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50142 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/pypower/toggle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/pypower/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.707768 ltbams-0.9.7/ams/routines/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/routines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/routines/acopf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/routines/cpf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15971 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/routines/dcopf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/routines/dcpf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/routines/dopf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11591 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/routines/ed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/routines/pflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31956 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/routines/routine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24716 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/routines/rted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/routines/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15433 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/routines/uc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23243 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.707768 ltbams-0.9.7/ams/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-05-24 19:45:15.000000 ltbams-0.9.7/ams/utils/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.707768 ltbams-0.9.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.707768 ltbams-0.9.7/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.687768 ltbams-0.9.7/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.707768 ltbams-0.9.7/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/_templates/autosummary/module_toctree.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.707768 ltbams-0.9.7/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/examples/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.707768 ltbams-0.9.7/docs/source/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/getting_started/copyright.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.711768 ltbams-0.9.7/docs/source/getting_started/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/getting_started/formats/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17425 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/getting_started/formats/matpower.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/getting_started/formats/psse.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8986 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/getting_started/formats/pypower.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)   171220 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/getting_started/formats/xlsx.png
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/getting_started/formats/xlsx.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/getting_started/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/getting_started/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/getting_started/testcase.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/getting_started/verification.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.711768 ltbams-0.9.7/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    52102 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/images/dcopf_time.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.711768 ltbams-0.9.7/docs/source/images/sponsors/
+-rw-r--r--   0 runner    (1001) docker     (127)    87680 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/images/sponsors/CURENT_Logo_NameOnTrans.png
+-rw-r--r--   0 runner    (1001) docker     (127)    59336 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/images/sponsors/CURENT_Logo_Transparent.png
+-rw-r--r--   0 runner    (1001) docker     (127)   837476 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/images/sponsors/CURENT_Logo_Transparent_Name.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26131 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/images/sponsors/doe.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.711768 ltbams-0.9.7/docs/source/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/modeling/example.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/modeling/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/modeling/model.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/modeling/routine.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/modeling/system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-05-24 19:45:15.000000 ltbams-0.9.7/docs/source/release-notes.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.711768 ltbams-0.9.7/ltbams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-05-24 19:47:47.000000 ltbams-0.9.7/ltbams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-24 19:47:47.000000 ltbams-0.9.7/ltbams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 19:47:47.000000 ltbams-0.9.7/ltbams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 19:47:47.000000 ltbams-0.9.7/ltbams.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-24 19:47:47.000000 ltbams-0.9.7/ltbams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 19:47:47.000000 ltbams-0.9.7/ltbams.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-24 19:45:15.000000 ltbams-0.9.7/requirements-extra.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-24 19:45:15.000000 ltbams-0.9.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-24 19:47:47.715768 ltbams-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-24 19:45:15.000000 ltbams-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:47:47.715768 ltbams-0.9.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:45:15.000000 ltbams-0.9.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-24 19:45:15.000000 ltbams-0.9.7/tests/test_1st_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-24 19:45:15.000000 ltbams-0.9.7/tests/test_addressing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8156 2024-05-24 19:45:15.000000 ltbams-0.9.7/tests/test_andes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7778 2024-05-24 19:45:15.000000 ltbams-0.9.7/tests/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-24 19:45:15.000000 ltbams-0.9.7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-24 19:45:15.000000 ltbams-0.9.7/tests/test_dctypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-24 19:45:15.000000 ltbams-0.9.7/tests/test_export_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-24 19:45:15.000000 ltbams-0.9.7/tests/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-24 19:45:15.000000 ltbams-0.9.7/tests/test_known_good.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6021 2024-05-24 19:45:15.000000 ltbams-0.9.7/tests/test_mats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-24 19:45:15.000000 ltbams-0.9.7/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-24 19:45:15.000000 ltbams-0.9.7/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-24 19:45:15.000000 ltbams-0.9.7/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-24 19:45:15.000000 ltbams-0.9.7/tests/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-05-24 19:45:15.000000 ltbams-0.9.7/tests/test_routine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-24 19:45:15.000000 ltbams-0.9.7/tests/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81189 2024-05-24 19:45:15.000000 ltbams-0.9.7/versioneer.py
```

### Comparing `ltbams-0.9.6/CONTRIBUTING.rst` & `ltbams-0.9.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/LICENSE` & `ltbams-0.9.7/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-AMS: Python Software for Dispatch Modeling and Co-Simulation with Dynanic
+AMS: Python Software for Scheduling Modeling and Co-Simulation with Dynanic
 
 Copyright (c) 2023-2024 Jinning Wang
 
 This program is free software; you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation; either version 3 of the License, or
 (at your option) any later version.
@@ -645,15 +645,15 @@
 free software which everyone can redistribute and change under these terms.
 
   To do so, attach the following notices to the program.  It is safest
 to attach them to the start of each source file to most effectively
 state the exclusion of warranty; and each file should have at least
 the "copyright" line and a pointer to where the full notice is found.
 
-    AMS, a python software for dispatch modeling and co-simulation with dynanic
+    AMS, a python software for scheduling modeling and co-simulation with dynanic
     Copyright (C) 2023 Jinning Wang
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
```

### Comparing `ltbams-0.9.6/PKG-INFO` & `ltbams-0.9.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ltbams
-Version: 0.9.6
-Summary: Python software for dispatch modeling and co-simulation with dynanic.
+Version: 0.9.7
+Summary: Python software for scheduling modeling and co-simulation with dynanics.
 Home-page: https://github.com/CURENT/ams
 Author: Jinning Wang
 Author-email: jinninggm@gmail.com
 License: GNU Public License v3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
@@ -29,15 +29,15 @@
 Provides-Extra: sphinx 
 Provides-Extra: sphinx-copybutton 
 Provides-Extra: sphinx-panels 
 License-File: LICENSE
 
 # LTB AMS
 
-Python Software for Power System Dispatch Modeling and Co-Simulation with Dynanic, serving as the market simulator for the [CURENT Largescale Testbed][LTB Repository].
+Python Software for Power System Scheduling Modeling and Co-Simulation with Dynanic, serving as the market simulator for the [CURENT Largescale Testbed][LTB Repository].
 
 [![License: GPL-3.0](https://img.shields.io/badge/License-GPL--3.0-blue.svg)](https://github.com/CURENT/ams/blob/master/LICENSE)
 ![platforms](https://anaconda.org/conda-forge/ltbams/badges/platforms.svg)
 [![Python Versions](https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)](https://www.python.org/)
 ![Repo Size](https://img.shields.io/github/repo-size/CURENT/ams)
 [![GitHub last commit (master)](https://img.shields.io/github/last-commit/CURENT/ams/master?label=last%20commit%20to%20master)](https://github.com/CURENT/ams/commits/master/)
 [![GitHub last commit (develop)](https://img.shields.io/github/last-commit/CURENT/ams/develop?label=last%20commit%20to%20develop)](https://github.com/CURENT/ams/commits/develop/)
@@ -60,15 +60,15 @@
 | Build Status  | [![GitHub Action Status](https://github.com/CURENT/ams/workflows/Python%20application/badge.svg)](https://github.com/curent/ams/actions)  | [![Build Status](https://dev.azure.com/curentltb/ams/_apis/build/status%2FCURENT.ams?branchName=master)](https://dev.azure.com/curentltb/ams/_build/latest?definitionId=2&branchName=master) |
 
 
 # Why AMS
 
 With the built-in interface with dynamic simulation engine, ANDES, AMS enables Dynamics Interfaced Stability Constrained Production Cost and Market Operation Modeling.
 
-AMS produces credible dispatch results and competitive performance.
+AMS produces credible scheduling results and competitive performance.
 The following results show the comparison of DCOPF between AMS and other tools.
 
 | Cost [\$]       |      AMS       |  MATPOWER   | pandapower |
 |----------------:|--------------:|------------:|-----------:|
 | PEGASE 1354-Bus |  1,173,590.63  |  1,173,590.63 |  1,173,590.63 |
 | PEGASE 2869-Bus |  2,338,915.61  |  2,338,915.61 |  2,338,915.61 |
 | GOC 4020-Bus    |    793,634.11  |    793,634.11 |    793,634.11 |
@@ -108,15 +108,15 @@
 Install from GitHub source:
 
 ```bash
 pip install git+https://github.com/CURENT/ams.git
 ```
 
 # Sponsors and Contributors
-AMS is the dispatch simulation engine for the CURENT Largescale Testbed (LTB).
+AMS is the scheduling simulation engine for the CURENT Largescale Testbed (LTB).
 More information about CURENT LTB can be found at the [LTB Repository][LTB Repository].
 
 This work was supported in part by the Engineering Research Center Program of the National Science Foundation and the Department of Energy
 under NSF Award Number EEC-1041877 and the CURENT Industry Partnership Program.
 
 This work was supported in part by the Advanced Grid Research and Development Program in the Office of Electricity at the U.S. Department of Energy.
```

### Comparing `ltbams-0.9.6/README.md` & `ltbams-0.9.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # LTB AMS
 
-Python Software for Power System Dispatch Modeling and Co-Simulation with Dynanic, serving as the market simulator for the [CURENT Largescale Testbed][LTB Repository].
+Python Software for Power System Scheduling Modeling and Co-Simulation with Dynanic, serving as the market simulator for the [CURENT Largescale Testbed][LTB Repository].
 
 [![License: GPL-3.0](https://img.shields.io/badge/License-GPL--3.0-blue.svg)](https://github.com/CURENT/ams/blob/master/LICENSE)
 ![platforms](https://anaconda.org/conda-forge/ltbams/badges/platforms.svg)
 [![Python Versions](https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)](https://www.python.org/)
 ![Repo Size](https://img.shields.io/github/repo-size/CURENT/ams)
 [![GitHub last commit (master)](https://img.shields.io/github/last-commit/CURENT/ams/master?label=last%20commit%20to%20master)](https://github.com/CURENT/ams/commits/master/)
 [![GitHub last commit (develop)](https://img.shields.io/github/last-commit/CURENT/ams/develop?label=last%20commit%20to%20develop)](https://github.com/CURENT/ams/commits/develop/)
@@ -27,15 +27,15 @@
 | Build Status  | [![GitHub Action Status](https://github.com/CURENT/ams/workflows/Python%20application/badge.svg)](https://github.com/curent/ams/actions)  | [![Build Status](https://dev.azure.com/curentltb/ams/_apis/build/status%2FCURENT.ams?branchName=master)](https://dev.azure.com/curentltb/ams/_build/latest?definitionId=2&branchName=master) |
 
 
 # Why AMS
 
 With the built-in interface with dynamic simulation engine, ANDES, AMS enables Dynamics Interfaced Stability Constrained Production Cost and Market Operation Modeling.
 
-AMS produces credible dispatch results and competitive performance.
+AMS produces credible scheduling results and competitive performance.
 The following results show the comparison of DCOPF between AMS and other tools.
 
 | Cost [\$]       |      AMS       |  MATPOWER   | pandapower |
 |----------------:|--------------:|------------:|-----------:|
 | PEGASE 1354-Bus |  1,173,590.63  |  1,173,590.63 |  1,173,590.63 |
 | PEGASE 2869-Bus |  2,338,915.61  |  2,338,915.61 |  2,338,915.61 |
 | GOC 4020-Bus    |    793,634.11  |    793,634.11 |    793,634.11 |
@@ -75,15 +75,15 @@
 Install from GitHub source:
 
 ```bash
 pip install git+https://github.com/CURENT/ams.git
 ```
 
 # Sponsors and Contributors
-AMS is the dispatch simulation engine for the CURENT Largescale Testbed (LTB).
+AMS is the scheduling simulation engine for the CURENT Largescale Testbed (LTB).
 More information about CURENT LTB can be found at the [LTB Repository][LTB Repository].
 
 This work was supported in part by the Engineering Research Center Program of the National Science Foundation and the Department of Energy
 under NSF Award Number EEC-1041877 and the CURENT Industry Partnership Program.
 
 This work was supported in part by the Advanced Grid Research and Development Program in the Office of Electricity at the U.S. Department of Energy.
```

### Comparing `ltbams-0.9.6/ams/__init__.py` & `ltbams-0.9.7/ams/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from ams import utils  # NOQA
 from ams import models     # NOQA
 from ams import system    # NOQA
 from ams import routines  # NOQA
 from ams import opt       # NOQA
 from ams import pypower  # NOQA
 from ams import report  # NOQA
+from ams import extension  # NOQA
 
 from ams.main import config_logger, load, run  # NOQA
 from ams.utils.paths import get_case  # NOQA
 from ams.shared import ppc2df  # NOQA
 
 __author__ = 'Jining Wang'
 
-__all__ = ['io', 'utils', 'models', 'system']
+__all__ = ['io', 'utils', 'models', 'system', 'extension']
```

### Comparing `ltbams-0.9.6/ams/cases/5bus/pjm5bus_demo.xlsx` & `ltbams-0.9.7/ams/cases/5bus/pjm5bus_demo.xlsx`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/5bus/pjm5bus_uced.json` & `ltbams-0.9.7/ams/cases/5bus/pjm5bus_uced.json`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/5bus/pjm5bus_uced.xlsx` & `ltbams-0.9.7/ams/cases/5bus/pjm5bus_uced.xlsx`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/5bus/pjm5bus_uced_esd1.xlsx` & `ltbams-0.9.7/ams/cases/5bus/pjm5bus_uced_esd1.xlsx`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/ieee123/ieee123.xlsx` & `ltbams-0.9.7/ams/cases/ieee123/ieee123.xlsx`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/ieee123/ieee123_regcv1.xlsx` & `ltbams-0.9.7/ams/cases/ieee123/ieee123_regcv1.xlsx`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/ieee14/ieee14.json` & `ltbams-0.9.7/ams/cases/ieee14/ieee14.json`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/ieee14/ieee14.raw` & `ltbams-0.9.7/ams/cases/ieee14/ieee14.raw`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/ieee14/ieee14_uced.xlsx` & `ltbams-0.9.7/ams/cases/ieee14/ieee14_uced.xlsx`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/ieee39/ieee39.xlsx` & `ltbams-0.9.7/ams/cases/ieee39/ieee39.xlsx`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/ieee39/ieee39_uced.xlsx` & `ltbams-0.9.7/ams/cases/ieee39/ieee39_uced.xlsx`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/ieee39/ieee39_uced_esd1.xlsx` & `ltbams-0.9.7/ams/cases/ieee39/ieee39_uced_esd1.xlsx`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/ieee39/ieee39_uced_pvd1.xlsx` & `ltbams-0.9.7/ams/cases/ieee39/ieee39_uced_pvd1.xlsx`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/ieee39/ieee39_uced_vis.xlsx` & `ltbams-0.9.7/ams/cases/ieee39/ieee39_uced_vis.xlsx`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/matpower/case118.m` & `ltbams-0.9.7/ams/cases/matpower/case118.m`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/matpower/case14.m` & `ltbams-0.9.7/ams/cases/matpower/case14.m`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/matpower/case300.m` & `ltbams-0.9.7/ams/cases/matpower/case300.m`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/matpower/case39.m` & `ltbams-0.9.7/ams/cases/matpower/case39.m`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/matpower/case5.m` & `ltbams-0.9.7/ams/cases/matpower/case5.m`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/matpower/case_ACTIVSg2000.m` & `ltbams-0.9.7/ams/cases/matpower/case_ACTIVSg2000.m`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/npcc/npcc.m` & `ltbams-0.9.7/ams/cases/npcc/npcc.m`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/npcc/npcc_uced.xlsx` & `ltbams-0.9.7/ams/cases/npcc/npcc_uced.xlsx`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/pglib/pglib_opf_case39_epri__api.m` & `ltbams-0.9.7/ams/cases/pglib/pglib_opf_case39_epri__api.m`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/wecc/wecc.m` & `ltbams-0.9.7/ams/cases/wecc/wecc.m`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cases/wecc/wecc_uced.xlsx` & `ltbams-0.9.7/ams/cases/wecc/wecc_uced.xlsx`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/cli.py` & `ltbams-0.9.7/ams/cli.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/core/documenter.py` & `ltbams-0.9.7/ams/core/documenter.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/core/matprocessor.py` & `ltbams-0.9.7/ams/core/matprocessor.py`

 * *Files 8% similar despite different names*

```diff
@@ -388,131 +388,152 @@
         tap = np.ones(nl)
         i = np.flatnonzero(tap0)
         tap[i] = tap0[i]  # assign non-zero tap ratios
         b = b / tap  # adjusted series susceptance
 
         return b
 
-    def build_ptdf(self):
+    def build_ptdf(self, dtype='float64', no_store=False):
         """
         Build the DC PTDF matrix and store it in the MParam `PTDF`.
 
         `PTDF[m, n]` means the increased line flow on line `m` when there is
         1 p.u. power injection at bus `n`.
 
         It requires DC Bbus and Bf.
 
         Note that there is discrepency between the PTDF-based line flow and
         DCOPF calcualted line flow. The gap is ignorable for small cases.
 
+        Try to use 'float32' for dtype if memory is a concern.
+
+        Parameters
+        ----------
+        dtype : str, optional
+            Data type of the PTDF matrix. Default is 'float64'.
+        no_store : bool, optional
+            If True, the PTDF will not be stored into `MatProcessor.PTDF._v`.
+
         Returns
         -------
         PTDF : np.ndarray
             Power transfer distribution factor.
         """
         system = self.system
 
-        # common variables
-        nb = system.Bus.n
-        nl = system.Line.n
-
         # use first slack bus as reference slack bus
         slack = system.Slack.bus.v[0]
 
         # use first bus for voltage angle reference
         noref_idx = system.Bus.idx.v[1:]
         noref = system.Bus.idx2uid(noref_idx)
 
         noslack = [system.Bus.idx2uid(bus) for bus in system.Bus.idx.v if bus != slack]
 
         # build other matrices if not built
         if not self.initialized:
             logger.debug("System matrices are not built. Building now.")
             self.build()
+
         # use dense representation
-        Bbus, Bf = self.Bbus.v, self.Bf.v
+        Bbus = self.Bbus._v.todense().astype(dtype)
+        Bf = self.Bf._v.todense().astype(dtype)
 
         # initialize PTDF matrix
-        H = np.zeros((nl, nb))
+        H = np.zeros((system.Line.n, system.Bus.n), dtype=dtype)
         # calculate PTDF
         H[:, noslack] = np.linalg.solve(Bbus[np.ix_(noslack, noref)].T, Bf[:, noref].T).T
-        # store PTDF
-        self.PTDF._v = H
 
-        return self.PTDF._v
+        if not no_store:
+            self.PTDF._v = H
 
-    def build_lodf(self):
+        return H
+
+    def build_lodf(self, dtype='float64', no_store=False):
         """
         Build the DC LODF matrix and store it in the MParam `LODF`.
 
         `LODF[m, n]` means the increased line flow on line `m` when there is
         1 p.u. line flow decrease on line `n` due to line `n` outage.
 
         It requires DC PTDF and Cft.
 
+        Try to use 'float32' for dtype if memory is a concern.
+
+        Parameters
+        ----------
+        dtype : str, optional
+            Data type of the LODF matrix. Default is 'float64'.
+        no_store : bool, optional
+            If True, the LODF will not be stored into `MatProcessor.LODF._v`.
+
         Returns
         -------
         LODF : np.ndarray
             Line outage distribution factor.
         """
-        system = self.system
-
-        # common variables
-        nl = system.Line.n
+        nl = self.system.Line.n
 
         # build PTDF if not built
         if self.PTDF._v is None:
-            self.build_ptdf()
+            ptdf = self.build_ptdf(dtype=dtype, no_store=True)
+        else:
+            ptdf = self.PTDF._v
 
-        H = self.PTDF._v * self.Cft._v
+        H = ptdf * self.Cft._v
         h = np.diag(H, 0)
         LODF = safe_div(H, np.ones((nl, nl)) - np.ones((nl, 1)) * h.T)
         LODF = LODF - np.diag(np.diag(LODF)) - np.eye(nl, nl)
 
-        self.LODF._v = LODF
-        return self.LODF._v
+        if not no_store:
+            self.LODF._v = LODF.astype(dtype)
+        return LODF.astype(dtype)
 
-    def build_otdf(self, line=None):
+    def build_otdf(self, line=None, dtype='float64'):
         """
-        Build the DC OTDF matrix.
+        Build the DC OTDF matrix for line outage:
+        :math:`OTDF_k = PTDF + LODF[:, k] @ PTDF[k, ]`,
+        where k is the outage line locations.
+
+        OTDF_k[m, n] means the increased line flow on line `m` when there is
+        1 p.u. line flow decrease on line `k` due to line `k` outage.
 
-        `OTDF_k[m, n]` means the PTDF[m, n] with line `k` outage.
+        Note that the OTDF is not stored in the MatProcessor.
 
-        It requires ... ...
+        Try to use 'float32' for dtype if memory is a concern.
 
         Parameters
         ----------
-        line : int, str, optional
-            Outage line idx to build the OTDF. If not provided, use the
-            first line `System.Line.idx.v[0]`.
+        line : int, str, list, optional
+            Lines index for which the OTDF is calculated. It takes both single
+            or multiple line indices.
+            If not given, the first line is used by default.
+        dtype : str, optional
+            Data type of the OTDF matrix. Default is 'float64'.
 
         Returns
         -------
         OTDF : np.ndarray
             Line outage distribution factor.
         """
-        system = self.system
-
-        if line is None:
-            line = system.Line.idx.v[0]
-        elif isinstance(line, list):
-            logger.warning("Multiple line is given, only the first one is used.")
-            line = line[0]
-        line_uid = system.Line.idx2uid(line)
+        if self.PTDF._v is None:
+            ptdf = self.build_ptdf(dtype=dtype, no_store=True)
+        else:
+            ptdf = self.PTDF._v
 
-        # build LODF if not built
         if self.LODF._v is None:
-            self.build_lodf()
-
-        # common variables
-        nb = system.Bus.n
-        nl = system.Line.n
-
-        # initialize OTDF matrix
-        OTDF = np.zeros((nl, nb))
+            lodf = self.build_lodf(dtype=dtype, no_store=True)
+        else:
+            lodf = self.LODF._v
 
-        line_lodf = self.LODF._v[:, line_uid]  # LODF for the outage line
-        line_ptdf = self.PTDF._v[line_uid, :]  # PTDF for the outage line
-        OTDF += self.PTDF._v  # Add PTDF to OTDF
-        OTDF += line_lodf[:, np.newaxis] * line_ptdf  # Add LODF * PTDF for the outage line
+        if line is None:
+            luid = [0]
+        elif isinstance(line, (int, str)):
+            try:
+                luid = [self.system.Line.idx2uid(line)]
+            except ValueError:
+                raise ValueError(f"Line {line} not found.")
+        elif isinstance(line, list):
+            luid = self.system.Line.idx2uid(line)
 
-        return OTDF
+        otdf = ptdf + lodf[:, luid] @ ptdf[luid, :]
+        return otdf.astype(dtype)
```

### Comparing `ltbams-0.9.6/ams/core/model.py` & `ltbams-0.9.7/ams/core/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from ams.core.var import Algeb
 
 logger = logging.getLogger(__name__)
 
 
 class Model:
     """
-    Base class for power system dispatch models.
+    Base class for power system scheduling models.
 
     This class is revised from ``andes.core.model.Model``.
     """
 
     def __init__(self, system=None, config=None):
 
         # --- Model ---
```

### Comparing `ltbams-0.9.6/ams/core/param.py` & `ltbams-0.9.7/ams/core/param.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/core/service.py` & `ltbams-0.9.7/ams/core/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -493,15 +493,15 @@
             logger.error(msg)
 
     @property
     def v(self):
         n_gen = self.u.n
         n_ts = self.u.horizon.n
         tout = np.zeros((n_gen, n_ts))
-        t = self.rtn.config.t  # dispatch interval
+        t = self.rtn.config.t  # scheduling interval
 
         # minimum online/offline duration
         td = np.ceil(self.u2.v/t).astype(int)
 
         # Create index arrays for generators and time periods
         i, t = np.meshgrid(np.arange(n_gen), np.arange(n_ts), indexing='ij')
         # Create a mask for valid time periods based on minimum duration
```

### Comparing `ltbams-0.9.6/ams/core/symprocessor.py` & `ltbams-0.9.7/ams/core/symprocessor.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/core/var.py` & `ltbams-0.9.7/ams/core/var.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/interop/andes.py` & `ltbams-0.9.7/ams/interop/andes.py`

 * *Files 1% similar despite different names*

```diff
@@ -512,15 +512,15 @@
         if not adsys.is_setup:
             adsys.setup()
         if amsys.dyn.link is None:
             amsys.dyn.link = make_link_table(adsys=adsys)
 
     def send(self, adsys=None, routine=None):
         """
-        Send results of the recent sovled AMS dispatch (``sp.recent``) to the
+        Send results of the recent sovled AMS routine (``sp.recent``) to the
         target ANDES system.
 
         Note that converged AC conversion DOES NOT guarantee successful dynamic
         initialization ``TDS.init()``.
         Failed initialization is usually caused by limiter violation.
 
         Parameters
```

### Comparing `ltbams-0.9.6/ams/io/__init__.py` & `ltbams-0.9.7/ams/io/__init__.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/io/json.py` & `ltbams-0.9.7/ams/io/json.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/io/matpower.py` & `ltbams-0.9.7/ams/io/matpower.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,16 @@
         baseKV = data[9]
         if baseKV == 0:
             baseKV = 110
         zone = data[10]
         vmax = data[11]
         vmin = data[12]
 
-        system.add('Bus', idx=idx, name='Bus ' + str(idx), Vn=baseKV,
+        system.add('Bus', idx=idx, name='Bus ' + str(idx),
+                   type=ty, Vn=baseKV,
                    v0=vmag, a0=vang,
                    vmax=vmax, vmin=vmin,
                    area=area, zone=zone)
         if pd != 0 or qd != 0:
             system.add('PQ', bus=idx, name='PQ ' + str(idx), Vn=baseKV, p0=pd, q0=qd)
         if gs or bs:
             system.add('Shunt', bus=idx, name='Shunt ' + str(idx), Vn=baseKV, g=gs, b=bs)
@@ -196,36 +197,43 @@
                    trans=tf, tap=ratio, phi=angle,
                    rate_a=rate_a, rate_b=rate_b, rate_c=rate_c,
                    amin=amin, amax=amax)
 
     if ('bus_name' in mpc) and (len(mpc['bus_name']) == len(system.Bus.name.v)):
         system.Bus.name.v[:] = mpc['bus_name']
 
-    gcost_idx = 0
-    gen_idx = np.arange(mpc['gen'].shape[0]) + 1
-    for data, gen in zip(mpc['gencost'], gen_idx):
-        # NOTE: only type 2 costs are supported for now
-        # type  startup shutdown	n	c2  c1  c0
-        # 0     1       2           3   4   5   6
-        if data[0] != 2:
-            raise ValueError('Only MODEL 2 costs are supported')
-        gcost_idx += 1
-        gctype = int(data[0])
-        startup = data[1]
-        shutdown = data[2]
-        c2 = data[4] * base_mva ** 2
-        c1 = data[5] * base_mva
-        c0 = data[6]
-        system.add('GCost', gen=int(gen),
-                   u=1, type=gctype,
-                   idx=gcost_idx,
-                   name=f'GCost {gcost_idx}',
-                   csu=startup, csd=shutdown,
-                   c2=c2, c1=c1, c0=c0
-                   )
+    # --- gencost ---
+    if 'gencost' in mpc:
+        gcost_idx = 0
+        gen_idx = np.arange(mpc['gen'].shape[0]) + 1
+        mpc_cost = np.zeros((mpc['gen'].shape[0], 7))
+        if mpc['gencost'].shape[1] < 7:
+            mpc_cost[:, :mpc['gencost'].shape[1]] = mpc['gencost']
+        else:
+            mpc_cost = mpc['gencost']
+        for data, gen in zip(mpc_cost, gen_idx):
+            # NOTE: only type 2 costs are supported for now
+            # type  startup shutdown	n	c2  c1  c0
+            # 0     1       2           3   4   5   6
+            if data[0] != 2:
+                raise ValueError('Only MODEL 2 costs are supported')
+            gcost_idx += 1
+            gctype = int(data[0])
+            startup = data[1]
+            shutdown = data[2]
+            c2 = data[4] * base_mva ** 2
+            c1 = data[5] * base_mva
+            c0 = data[6]
+            system.add('GCost', gen=int(gen),
+                       u=1, type=gctype,
+                       idx=gcost_idx,
+                       name=f'GCost {gcost_idx}',
+                       csu=startup, csd=shutdown,
+                       c2=c2, c1=c1, c0=c0
+                       )
 
     # --- region ---
     zone_id = np.unique(system.Bus.zone.v).astype(int)
     for zone in zone_id:
         zone_idx = f'ZONE_{zone}'
         system.add('Region', idx=zone_idx, name=zone_idx)
     bus_zone = system.Bus.zone.v
```

### Comparing `ltbams-0.9.6/ams/io/pypower.py` & `ltbams-0.9.7/ams/io/pypower.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/io/xlsx.py` & `ltbams-0.9.7/ams/io/xlsx.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/main.py` & `ltbams-0.9.7/ams/main.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/models/__init__.py` & `ltbams-0.9.7/ams/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
-The package for models used in dispatch modeling.
+The package for models used in scheduling modeling.
 
 The file_classes includes the list of file classes and their corresponding classes.
 """
 
 
 ams_file_classes = list([
     ('info', ['Summary']),
     ('bus', ['Bus']),
     ('static', ['PQ', 'Slack', 'PV']),
     ('shunt', ['Shunt']),
     ('line', ['Line']),
-    ('distributed', ['PVD1', 'ESD1']),
+    ('distributed', ['PVD1', 'ESD1', 'EV1', 'EV2']),
     ('renewable', ['REGCA1', 'REGCV1', 'REGCV2']),
     ('area', ['Area']),
     ('region', ['Region']),
     ('reserve', ['SFR', 'SR', 'NSR', 'VSGR']),
     ('cost', ['GCost', 'SFRCost', 'SRCost', 'NSRCost', 'VSGCost']),
     ('cost', ['DCost']),
     ('timeslot', ['TimeSlot', 'EDTSlot', 'UCTSlot']),
```

### Comparing `ltbams-0.9.6/ams/models/area.py` & `ltbams-0.9.7/ams/models/area.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/models/bus.py` & `ltbams-0.9.7/ams/models/bus.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 
 import numpy as np
 
+from andes.core.param import NumParam
 from andes.models.bus import BusData
 
 from ams.core.var import Algeb
 from ams.core.model import Model
 
 logger = logging.getLogger(__name__)
 
@@ -21,14 +22,20 @@
 
         self.group = 'ACTopology'
         # NOTE: in ANDES, self.zone is defined to trace a non-existing model "Region"
         # in AMS, model "Zone" is developed,
         # so we need to change the model name of IdxParam self.zone
         self.zone.model = 'Region'
 
+        self.type = NumParam(name='type',
+                             info='bus type, 1=PQ, 2=PV, 3=ref, 4=isolated (place holder)',
+                             default=1,
+                             vtype=int,
+                             )
+
         self.a = Algeb(name='a',
                        tex_name=r'\theta',
                        info='voltage angle',
                        unit='rad',
                        )
         self.v = Algeb(name='v',
                        tex_name='V',
```

### Comparing `ltbams-0.9.6/ams/models/cost.py` & `ltbams-0.9.7/ams/models/cost.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/models/distributed/esd1.py` & `ltbams-0.9.7/ams/models/distributed/esd1.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                              vrange=(0, 1),
                              )
 
 
 class ESD1(ESD1Data, Model):
     """
     Distributed energy storage model, revised from ANDES ``ESD1`` model for
-    dispatch.
+    scheduling.
 
     Following parameters are omitted from the original dynamic model:
     ``fn``, ``busf``, ``xc``, ``pqflag``, ``igreg``, ``v0``, ``v1``,
     ``dqdv``, ``fdbd``, ``ddn``, ``ialim``, ``vt0``, ``vt1``, ``vt2``,
     ``vt3``, ``vrflag``, ``ft0``, ``ft1``, ``ft2``, ``ft3``, ``frflag``,
     ``tip``, ``tiq``, ``recflag``.
```

### Comparing `ltbams-0.9.6/ams/models/distributed/pvd1.py` & `ltbams-0.9.7/ams/models/distributed/pvd1.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                                vrange='(0, 1]',
                                )
 
 
 class PVD1(PVD1Data, Model):
     """
     Distributed PV model, revised from ANDES ``PVD1`` model for
-    dispatch.
+    scheduling.
 
     Following parameters are omitted from the original dynamic model:
     ``fn``, ``busf``, ``xc``, ``pqflag``, ``igreg``, ``v0``, ``v1``,
     ``dqdv``, ``fdbd``, ``ddn``, ``ialim``, ``vt0``, ``vt1``, ``vt2``,
     ``vt3``, ``vrflag``, ``ft0``, ``ft1``, ``ft2``, ``ft3``, ``frflag``,
     ``tip``, ``tiq``, ``recflag``.
```

### Comparing `ltbams-0.9.6/ams/models/group.py` & `ltbams-0.9.7/ams/models/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         self.common_vars.extend(('Pe', 'Qe'))
 
 
 class VSG(GroupBase):
     """
     Renewable generator with virtual synchronous generator (VSG) control group.
 
-    Note that this is a group separate from ``RenGen`` for VSG dispatch study.
+    Note that this is a group separate from ``RenGen`` for VSG scheduling study.
     """
 
     def __init__(self):
         super().__init__()
         self.common_params.extend(('bus', 'gen', 'Sn'))
         self.common_vars.extend(('Pe', 'Qe'))
```

### Comparing `ltbams-0.9.6/ams/models/info.py` & `ltbams-0.9.7/ams/models/info.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/models/line.py` & `ltbams-0.9.7/ams/models/line.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/models/region.py` & `ltbams-0.9.7/ams/models/region.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/models/renewable/regc.py` & `ltbams-0.9.7/ams/models/renewable/regc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
-RenGen dispatch model.
+RenGen scheduling model.
 """
 
 from andes.core.param import NumParam, IdxParam, ExtParam
 from andes.core.model import ModelData
 from ams.core.model import Model
 
 
 class REGCData(ModelData):
     """
-    Data container for RenGen dispatch model.
+    Data container for RenGen scheduling model.
     """
 
     def __init__(self):
         ModelData.__init__(self)
         self.bus = IdxParam(model='Bus',
                             info="interface bus idx",
                             mandatory=True,
@@ -33,15 +33,15 @@
                                info="Q ratio of linked static gen",
                                tex_name=r'\gamma_Q'
                                )
 
 
 class REGCA1(REGCData, Model):
     """
-    Renewable generator dispatch model.
+    Renewable generator scheduling model.
 
     Reference:
 
     [1] ANDES Documentation, REGCA1
 
     Available:
     https://docs.andes.app/en/latest/groupdoc/RenGen.html#regca1
@@ -100,15 +100,15 @@
                              info='Maximum damping emulation',
                              unit='p.u.',
                              power=True,)
 
 
 class REGCV2(REGCV1):
     """
-    Voltage-controlled VSC.
+    Voltage-controlled VSC, identical to :ref:`REGCV1`.
 
     Reference:
 
     [1] ANDES Documentation, REGCV2
 
     Available:
```

### Comparing `ltbams-0.9.6/ams/models/reserve.py` & `ltbams-0.9.7/ams/models/reserve.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/models/static/gen.py` & `ltbams-0.9.7/ams/models/static/gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                               err_tol=r"\epsilon_{tol}"
                               )
 
         self.zone = ExtParam(model='Bus', src='zone', indexer=self.bus, export=False,
                              info='Retrieved zone idx', vtype=str, default=None,
                              )
 
-        self.ud = Algeb(info='connection status decision',
+        self.ud = Algeb(info='commitment decision',
                         unit='bool',
                         tex_name=r'u_d',
                         name='ud',
                         )
         self.p = Algeb(info='active power generation',
                        unit='p.u.',
                        tex_name='p',
```

### Comparing `ltbams-0.9.6/ams/models/static/pq.py` & `ltbams-0.9.7/ams/models/static/pq.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/models/timeslot.py` & `ltbams-0.9.7/ams/models/timeslot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Model for rolling horizon used in dispatch.
+Model for rolling horizon used in scheduling.
 """
 
 from andes.core import ModelData, NumParam
 from andes.models.timeseries import str_list_iconv
 from ams.core.model import Model
```

### Comparing `ltbams-0.9.6/ams/opt/omodel.py` & `ltbams-0.9.7/ams/opt/omodel.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/pypower/core/pips.py` & `ltbams-0.9.7/ams/pypower/core/pips.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/pypower/core/ppoption.py` & `ltbams-0.9.7/ams/pypower/core/ppoption.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/pypower/core/solver.py` & `ltbams-0.9.7/ams/pypower/core/solver.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/pypower/idx.py` & `ltbams-0.9.7/ams/pypower/idx.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/pypower/io.py` & `ltbams-0.9.7/ams/pypower/io.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/pypower/make/matrices.py` & `ltbams-0.9.7/ams/pypower/make/matrices.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/pypower/make/pdv.py` & `ltbams-0.9.7/ams/pypower/make/pdv.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/pypower/routines/cpf.py` & `ltbams-0.9.7/ams/pypower/routines/cpf.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/pypower/routines/cpf_callbacks.py` & `ltbams-0.9.7/ams/pypower/routines/cpf_callbacks.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/pypower/routines/opf.py` & `ltbams-0.9.7/ams/pypower/routines/opf.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/pypower/routines/opffcns.py` & `ltbams-0.9.7/ams/pypower/routines/opffcns.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/pypower/routines/pflow.py` & `ltbams-0.9.7/ams/pypower/routines/pflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,18 +48,16 @@
         PYPOWER options vector. It can be used to specify the solution algorithm
         and output options among other things. Default is None.
 
     Returns
     -------
     results : dict or None
         Solved power flow results. None if the power flow did not converge.
-    success : bool
-        True if the algorithm successfully found a solution, False otherwise.
-    et : float
-        Elapsed time in seconds for running the power flow.
+    sstats : dict
+        Solver statistics.
 
     Notes
     -----
     If the ENFORCE_Q_LIMS option is set to True (default is False), then if any
     generator reactive power limit is violated after running the AC power flow,
     the corresponding bus is converted to a IDX.bus.PQ bus, with Qg at the limit, and
     the case is re-run. The voltage magnitude at the bus will deviate from the
@@ -299,15 +297,15 @@
             np.ix_(
                 results["order"]["branch"]["status"]["off"],
                 [IDX.branch.PF,
                  IDX.branch.QF,
                  IDX.branch.PT,
                  IDX.branch.QT])] = 0
 
-    return results, success, sstats
+    return results, sstats
 
 
 def dcpf(B, Pbus, Va0, ref, pv, pq):
     """
     Solves a DC power flow.
 
     Solves for the bus voltage angles at all but the reference bus, given the
```

### Comparing `ltbams-0.9.6/ams/pypower/toggle.py` & `ltbams-0.9.7/ams/pypower/toggle.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/pypower/utils.py` & `ltbams-0.9.7/ams/pypower/utils.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/report.py` & `ltbams-0.9.7/ams/report.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/routines/__init__.py` & `ltbams-0.9.7/ams/routines/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Dispatch routines.
+Scheduling routines.
 """
 
 from collections import OrderedDict
 from andes.utils.func import list_flatten
 from ams.routines.routine import RoutineBase  # NOQA
 
 all_routines = OrderedDict([
```

### Comparing `ltbams-0.9.6/ams/routines/acopf.py` & `ltbams-0.9.7/ams/routines/acopf.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,16 +87,15 @@
     def solve(self, method=None, **kwargs):
         """
         Solve ACOPF using PYPOWER with PIPS.
         """
         ppc = system2ppc(self.system)
         ppopt = ppoption()
         res, sstats = runopf(casedata=ppc, ppopt=ppopt, **kwargs)
-        self.converged = res['success']
-        return res, self.converged, sstats
+        return res, sstats
 
     def run(self, force_init=False, no_code=True,
             method=None, **kwargs):
         """
         Run ACOPF using PYPOWER with PIPS.
 
         Examples
```

### Comparing `ltbams-0.9.6/ams/routines/cpf.py` & `ltbams-0.9.7/ams/routines/cpf.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/routines/dcopf.py` & `ltbams-0.9.7/ams/routines/dcopf.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/routines/dcpf.py` & `ltbams-0.9.7/ams/routines/dcpf.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,17 +120,16 @@
     def solve(self, method=None):
         """
         Solve DC power flow using PYPOWER.
         """
         ppc = system2ppc(self.system)
         ppopt = ppoption(PF_DC=True)
 
-        res, success, sstats = runpf(casedata=ppc, ppopt=ppopt)
-        self.converged = bool(success)
-        return res, self.converged, sstats
+        res, sstats = runpf(casedata=ppc, ppopt=ppopt)
+        return res, sstats
 
     def run(self, force_init=False, no_code=True,
             method=None, **kwargs):
         """
         Run DC pwoer flow.
 
         Examples
@@ -151,25 +150,30 @@
         -------
         exit_code : int
             Exit code of the routine.
         """
         if not self.initialized:
             self.init(force=force_init, no_code=no_code)
         t0, _ = elapsed()
-        res, success, sstats = self.solve(method=method)
-        self.exit_code = 0 if success else 1
+        res, sstats = self.solve(method=method)
+        self.converged = res['success']
+        self.exit_code = 0 if res['success'] else 1
         _, s = elapsed(t0)
         self.exec_time = float(s.split(' ')[0])
         n_iter = int(sstats['num_iters'])
         n_iter_str = f"{n_iter} iterations " if n_iter > 1 else f"{n_iter} iteration "
         if self.exit_code == 0:
             msg = f"<{self.class_name}> solved in {s}, converged in "
             msg += n_iter_str + f"with {sstats['solver_name']}."
             logger.info(msg)
-            self.unpack(res)
+            try:
+                self.unpack(res)
+            except Exception:
+                logger.warning(f"Failed to unpack results from {self.class_name}.")
+                return False
             return True
         else:
             msg = f"{self.class_name} failed in "
             msg += f"{int(sstats['num_iters'])} iterations with "
             msg += f"{sstats['solver_name']}!"
             logger.warning(msg)
             return False
```

### Comparing `ltbams-0.9.6/ams/routines/dopf.py` & `ltbams-0.9.7/ams/routines/dopf.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/routines/ed.py` & `ltbams-0.9.7/ams/routines/ed.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,24 +40,24 @@
                                name='dsrpz', tex_name=r'd_{s,r, p, z}',
                                info='zonal spinning reserve requirement in percentage',)
         self.dsr = NumOpDual(u=self.dsrpz, u2=self.sd, fun=np.multiply,
                              rfun=np.transpose,
                              name='dsr', tex_name=r'd_{s,r,z}',
                              info='zonal spinning reserve requirement',)
 
-        # NOTE: define e_str in dispatch model
+        # NOTE: define e_str in the scheduling model
         self.prsb = Constraint(info='spinning reserve balance',
                                name='prsb', is_eq=True,)
         self.rsr = Constraint(info='spinning reserve requirement',
                               name='rsr', is_eq=False,)
 
 
 class MPBase:
     """
-    Base class for multi-period dispatch.
+    Base class for multi-period scheduling.
     """
 
     def __init__(self) -> None:
         # NOTE: Setting `ED.scale.owner` to `Horizon` will cause an error when calling `ED.scale.v`.
         # This is because `Horizon` is a group that only contains the model `TimeSlot`.
         # The `get` method of `Horizon` calls `andes.models.group.GroupBase.get` and results in an error.
         self.sd = RParam(info='zonal load factor for ED',
@@ -216,21 +216,21 @@
         cost += '+ t dot sum(c1 @ pg + csr @ prs)'
         cost += '+ sum(mul(ugt, mul(c0, tlv)))'
         self.obj.e_str = cost
 
     def dc2ac(self, **kwargs):
         """
         AC conversion ``dc2ac`` is not implemented yet for
-        multi-period dispatch.
+        multi-period scheduling.
         """
         return NotImplementedError
 
     def unpack(self, **kwargs):
         """
-        Multi-period dispatch will not unpack results from
+        Multi-period scheduling will not unpack results from
         solver into devices.
 
         # TODO: unpack first period results, and allow input
         # to specify which period to unpack.
         """
         return None
 
@@ -243,26 +243,26 @@
     EDES should be used instead, otherwise there is no SOC.
     """
 
     def __init__(self, system, config):
         ED.__init__(self, system, config)
         DGBase.__init__(self)
 
-        self.config.t = 1  # dispatch interval in hour
+        self.config.t = 1  # scheduling interval in hour
 
         self.info = 'Economic dispatch with distributed generation'
         self.type = 'DCED'
 
         # NOTE: extend vars to 2D
         self.pgdg.horizon = self.timeslot
 
 
 class ESD1MPBase(ESD1Base):
     """
-    Extended base class for energy storage in multi-period dispatch.
+    Extended base class for energy storage in multi-period scheduling.
     """
 
     def __init__(self):
         ESD1Base.__init__(self)
 
         self.Mre = RampSub(u=self.SOC, name='Mre', tex_name=r'M_{r,ES}',
                            info='Subtraction matrix for SOC',
@@ -297,15 +297,15 @@
     The bilinear term in the formulation is linearized with big-M method.
     """
 
     def __init__(self, system, config):
         ED.__init__(self, system, config)
         ESD1MPBase.__init__(self)
 
-        self.config.t = 1  # dispatch interval in hour
+        self.config.t = 1  # scheduling interval in hour
 
         self.info = 'Economic dispatch with energy storage'
         self.type = 'DCED'
 
         # NOTE: extend vars to 2D
         self.pgdg.horizon = self.timeslot
         self.SOC.horizon = self.timeslot
```

### Comparing `ltbams-0.9.6/ams/routines/pflow.py` & `ltbams-0.9.7/ams/routines/pflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,16 @@
             msg = "Gauss method is not fully tested yet, not recommended!"
             logger.warning(msg)
         if alg is None:
             msg = f"Invalid method `{method}` for PFlow."
             raise ValueError(msg)
         ppopt = ppoption(PF_ALG=alg, ENFORCE_Q_LIMS=self.config.qlim)
 
-        res, success, sstats = runpf(casedata=ppc, ppopt=ppopt)
-        return res, success, sstats
+        res, sstats = runpf(casedata=ppc, ppopt=ppopt)
+        return res, sstats
 
     def run(self, force_init=False, no_code=True, method="newton", **kwargs):
         """
         Run AC power flow using PYPOWER.
 
         Currently, four methods are supported: 'newton', 'fdxb', 'fdbx', 'gauss',
         for Newton's method, fast-decoupled, XB, fast-decoupled, BX, and Gauss-Seidel,
```

### Comparing `ltbams-0.9.6/ams/routines/routine.py` & `ltbams-0.9.7/ams/routines/routine.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,15 +352,15 @@
             msg = f"{self.class_name} failed as {status} in "
             msg += n_iter_str + f"with {sstats.solver_name}!"
             logger.warning(msg)
             return False
 
     def export_csv(self, path=None):
         """
-        Export dispatch results to a csv file.
+        Export scheduling results to a csv file.
         For multi-period routines, the column "Time" is the time index of
         ``timeslot.v``, which usually comes from ``EDTSlot`` or ``UCTSlot``.
         The rest columns are the variables registered in ``vars``.
 
         For single-period routines, the column "Time" have a pseduo value of "T1".
 
         Parameters
```

### Comparing `ltbams-0.9.6/ams/routines/rted.py` & `ltbams-0.9.7/ams/routines/rted.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         # --- SFR ---
         self.pru = Var(info='RegUp reserve',
                        unit='p.u.', name='pru', tex_name=r'p_{r,u}',
                        model='StaticGen', nonneg=True,)
         self.prd = Var(info='RegDn reserve',
                        unit='p.u.', name='prd', tex_name=r'p_{r,d}',
                        model='StaticGen', nonneg=True,)
-        # NOTE: define e_str in dispatch routine
+        # NOTE: define e_str in scheduling routine
         self.rbu = Constraint(name='rbu', is_eq=True,
                               info='RegUp reserve balance',)
         self.rbd = Constraint(name='rbd', is_eq=True,
                               info='RegDn reserve balance',)
         self.rru = Constraint(name='rru', is_eq=False,
                               info='RegUp reserve source',)
         self.rrd = Constraint(name='rrd', is_eq=False,
```

### Comparing `ltbams-0.9.6/ams/routines/type.py` & `ltbams-0.9.7/ams/routines/type.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/routines/uc.py` & `ltbams-0.9.7/ams/routines/uc.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,21 +311,21 @@
     def init(self, force=False, no_code=True, **kwargs):
         self._initial_guess()
         return super().init(force=force, no_code=no_code, **kwargs)
 
     def dc2ac(self, **kwargs):
         """
         AC conversion ``dc2ac`` is not implemented yet for
-        multi-period dispatch.
+        multi-period scheduling.
         """
         return NotImplementedError
 
     def unpack(self, **kwargs):
         """
-        Multi-period dispatch will not unpack results from
+        Multi-period scheduling will not unpack results from
         solver into devices.
 
         # TODO: unpack first period results, and allow input
         # to specify which period to unpack.
         """
         return None
```

### Comparing `ltbams-0.9.6/ams/shared.py` & `ltbams-0.9.7/ams/shared.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ams/system.py` & `ltbams-0.9.7/ams/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     for method in methods:
         setattr(System, method, disable_method(getattr(System, method)))
 
 
 class System(andes_System):
     """
     A subclass of ``andes.system.System``, this class encapsulates data, models,
-    and routines for dispatch modeling and analysis in power systems.
+    and routines for scheduling modeling and analysis in power systems.
     Some methods  inherited from the parent class are intentionally disabled.
 
     Parameters
     ----------
     case : str, optional
         The path to the case file.
     name : str, optional
@@ -430,14 +430,21 @@
                 a0 += algeb.owner.n
 
         # NOTE: this is a temporary solution for building Y matrix
         # consider refator this part if any other similar cases occur in the future
         self.Line.a1a = self.Bus.get(src='a', attr='a', idx=self.Line.bus1.v)
         self.Line.a2a = self.Bus.get(src='a', attr='a', idx=self.Line.bus2.v)
 
+        # assign bus type as placeholder; 1=PQ, 2=PV, 3=ref, 4=isolated
+        if self.Bus.type.v.sum() == self.Bus.n:  # if all type are PQ
+            self.Bus.set(src='type', attr='v', idx=self.PV.bus.v,
+                         value=np.ones(self.PV.n))
+            self.Bus.set(src='type', attr='v', idx=self.Slack.bus.v,
+                         value=np.ones(self.Slack.n))
+
         _, s = elapsed(t0)
         logger.info('System set up in %s.', s)
 
         return ret
 
     # FIXME: remove unused methods
     # # Disable methods not supported in AMS
```

### Comparing `ltbams-0.9.6/ams/utils/paths.py` & `ltbams-0.9.7/ams/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/docs/Makefile` & `ltbams-0.9.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/docs/make.bat` & `ltbams-0.9.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/docs/source/_templates/autosummary/class.rst` & `ltbams-0.9.7/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/docs/source/_templates/autosummary/module.rst` & `ltbams-0.9.7/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/docs/source/_templates/autosummary/module_toctree.rst` & `ltbams-0.9.7/docs/source/_templates/autosummary/module_toctree.rst`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/docs/source/api.rst` & `ltbams-0.9.7/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/docs/source/conf.py` & `ltbams-0.9.7/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (master_doc, 'ams', 'AMS Manual',
-     author, 'ams', 'Python Software for Dispatch Modeling and Co-Simulation with Dynanic',
+     author, 'ams', 'Python Software for Scheduling Modeling and Co-Simulation with Dynanic',
      'Miscellaneous'),
 ]
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3/', None),
     'numpy': ('https://numpy.org/doc/stable/', None),  # Updated URL for numpy
```

### Comparing `ltbams-0.9.6/docs/source/examples/index.rst` & `ltbams-0.9.7/docs/source/examples/index.rst`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/docs/source/getting_started/copyright.rst` & `ltbams-0.9.7/docs/source/getting_started/copyright.rst`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/docs/source/getting_started/formats/matpower.rst` & `ltbams-0.9.7/docs/source/getting_started/formats/matpower.rst`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/docs/source/getting_started/formats/psse.rst` & `ltbams-0.9.7/docs/source/getting_started/formats/psse.rst`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/docs/source/getting_started/formats/pypower.rst` & `ltbams-0.9.7/docs/source/getting_started/formats/pypower.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. _input-pypower:
 
 PYPOWER
 --------
 
 AMS includes `PYPOWER cases <https://github.com/CURENT/ams/tree/develop/ams/cases/pypower>`_
-in version 2 for dispatch modeling and analysis. PYPOWER cases follow the same format as MATPOWER.
+in version 2 for scheduling modeling and analysis. PYPOWER cases follow the same format as MATPOWER.
 
 The PYPOWER case is defined as a Python dictionary that includes ``bus``, ``gen``, ``branch``,
 ``areas``, and ``gencost``.
 Defines the PYPOWER case file format.
 
 A PYPOWER case file is a Python file or MAT-file that defines or returns a dict named ``ppc``, referred to
 as a "PYPOWER case dict". The keys of this dict are ``bus``, ``gen``, ``branch``, ``areas``, and
```

### Comparing `ltbams-0.9.6/docs/source/getting_started/formats/xlsx.png` & `ltbams-0.9.7/docs/source/getting_started/formats/xlsx.png`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/docs/source/getting_started/formats/xlsx.rst` & `ltbams-0.9.7/docs/source/getting_started/formats/xlsx.rst`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/docs/source/getting_started/index.rst` & `ltbams-0.9.7/docs/source/getting_started/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
    <embed>
    <h1 style="letter-spacing: 0.4em; font-size: 2.5em !important;
    margin-bottom: 0; padding-bottom: 0"> AMS </h1>
 
    <p style="color: #00746F; font-variant: small-caps; font-weight: bold;
    margin-bottom: 2em">
-   Python Library for Flexible Dispatch Modeling and Dispatch-Dynamic Co-Simulation</p>
+   Python Library for Flexible Scheduling Modeling and Co-Simulation with Dynamics</p>
    </embed>
 
 .. _getting-started:
 
 ===============
 Getting started
 ===============
```

### Comparing `ltbams-0.9.6/docs/source/getting_started/install.rst` & `ltbams-0.9.7/docs/source/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/docs/source/getting_started/overview.rst` & `ltbams-0.9.7/docs/source/getting_started/overview.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. _package-overview:
 
 ================
 Package Overview
 ================
 
-AMS is an open-source packages for flexible dispatch modeling and co-simulation with
+AMS is an open-source packages for flexible scheduling modeling and co-simulation with
 the in-house dynanic simulation engine `ANDES <https://github.com/curent/andes>`_.
 
 AMS is currently under active development. To get involved,
 
 * Report issues in the
   `GitHub issues page <https://github.com/CURENT/ams/issues>`_
 * Learn version control with
```

### Comparing `ltbams-0.9.6/docs/source/getting_started/testcase.rst` & `ltbams-0.9.7/docs/source/getting_started/testcase.rst`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/docs/source/images/dcopf_time.png` & `ltbams-0.9.7/docs/source/images/dcopf_time.png`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/docs/source/images/sponsors/CURENT_Logo_NameOnTrans.png` & `ltbams-0.9.7/docs/source/images/sponsors/CURENT_Logo_NameOnTrans.png`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/docs/source/images/sponsors/CURENT_Logo_Transparent.png` & `ltbams-0.9.7/docs/source/images/sponsors/CURENT_Logo_Transparent.png`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/docs/source/images/sponsors/CURENT_Logo_Transparent_Name.png` & `ltbams-0.9.7/docs/source/images/sponsors/CURENT_Logo_Transparent_Name.png`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/docs/source/images/sponsors/doe.png` & `ltbams-0.9.7/docs/source/images/sponsors/doe.png`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/docs/source/index.rst` & `ltbams-0.9.7/docs/source/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 .. _`Source Repository`: https://github.com/CURENT/ams
 .. _`Report Issues`: https://github.com/CURENT/ams/issues
 .. _`Q&A`: https://github.com/CURENT/ams/discussions
 .. _`ANDES Repository`: https://github.com/CURENT/andes
 .. _`LTB Repository`: https://github.com/CURENT/
 
-LTB AMS is an open-source packages for dispatch modeling, serving as the market
+LTB AMS is an open-source packages for scheduling modeling, serving as the market
 simulator for the CURENT Large scale Testbed (LTB).
 
-AMS enables **flexible** dispatch modeling and **interoprability** with the in-house
+AMS enables **flexible** scheduling modeling and **interoprability** with the in-house
 dynamic simulator ANDES.
 
 .. panels::
     :card: + intro-card text-center
     :column: col-lg-6 col-md-6 col-sm-6 col-xs-12 d-flex
 
     ---
@@ -40,29 +40,29 @@
             :classes: btn-block btn-secondary stretched-link
 
     ---
 
     Examples
     ^^^^^^^^
 
-    The examples of using AMS for power system dispatch study.
+    The examples of using AMS for power system scheduling study.
 
     +++
 
     .. link-button:: scripting_examples
             :type: ref
             :text: To the examples
             :classes: btn-block btn-secondary stretched-link
 
     ---
 
     Model development guide
     ^^^^^^^^^^^^^^^^^^^^^^^
 
-    New dispatch modeling in AMS.
+    New scheduling modeling in AMS.
 
     +++
 
     .. link-button:: development
             :type: ref
             :text: To the development guide
             :classes: btn-block btn-secondary stretched-link
```

### Comparing `ltbams-0.9.6/docs/source/modeling/example.rst` & `ltbams-0.9.7/docs/source/modeling/example.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Examples
 ========
 
-One example is provided to demonstrate descriptive dispatch modeling.
+One example is provided to demonstrate descriptive scheduling modeling.
 
 DCOPF
 ----------
 
 
 DC optimal power flow (DCOPF) is a fundamental routine used in power system analysis.
 In this example, we demonstrate how to implement a DCOPF routine in a descriptive
```

### Comparing `ltbams-0.9.6/docs/source/modeling/model.rst` & `ltbams-0.9.7/docs/source/modeling/model.rst`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/docs/source/modeling/routine.rst` & `ltbams-0.9.7/docs/source/modeling/routine.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Routine
 ===========
 
-Routine refers to dispatch-level model, and it includes two sectinos, namely,
+Routine refers to scheduling-level model, and it includes two sectinos, namely,
 Data Section and Model Section.
 
 Data Section
 ------------------
 
 A simplified code snippet for RTED is shown below as an example.
 
@@ -46,15 +46,15 @@
 Later, in the constraint, ``gs`` is multiplied to the reserve variable ``pru``.
 
 Model Section
 -----------------
 
 Descriptive Formulation
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-Dispatch routine is the descriptive model of the optimization problem.
+Scheduling routine is the descriptive model of the optimization problem.
 
 Further, to facilitate the routine definition, AMS developed a class
 :py:mod:`ams.core.param.RParam` to pass the model data to multiple routine modeling.
 
 .. autoclass:: ams.core.param.RParam
     :noindex:
 
@@ -89,28 +89,28 @@
 The interoperation with dynamic simulator invovles both file conversion and data exchange.
 In AMS, the built-in interface with ANDES is implemented in :py:mod:`ams.interop.andes`.
 
 
 File Format Converter
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Power flow data is the bridge between dispatch study and dynamic study,
+Power flow data is the bridge between scheduling study and dynamics study,
 where it defines grid topology and power flow.
 An AMS case can be converted to an ANDES case, with the option to supply additional dynamic
 data.
 
 .. autofunction:: ams.interop.andes.to_andes
     :noindex:
 
 
 Data Exchange in Simulation
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-To achieve dispatch-dynamic cosimulation, it requires bi-directional data exchange between
-dispatch and dynamic study.
+To achieve scheduling-dynamics cosimulation, it requires bi-directional data exchange between
+scheduling and dynamics study.
 From the perspective of AMS, two functions, ``send`` and ``receive``, are developed.
 The maping relationship for a specific routine is defined in the routine class as ``map1`` and
 ``map2``.
 Additionally, a link table for the ANDES case is used for the controller connections.
 
 Module :py:mod:`ams.interop.andes.Dynamic`, contains the necessary functions and classes for
 file conversion and data exchange.
```

### Comparing `ltbams-0.9.6/docs/source/modeling/system.rst` & `ltbams-0.9.7/docs/source/modeling/system.rst`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/ltbams.egg-info/PKG-INFO` & `ltbams-0.9.7/ltbams.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ltbams
-Version: 0.9.6
-Summary: Python software for dispatch modeling and co-simulation with dynanic.
+Version: 0.9.7
+Summary: Python software for scheduling modeling and co-simulation with dynanics.
 Home-page: https://github.com/CURENT/ams
 Author: Jinning Wang
 Author-email: jinninggm@gmail.com
 License: GNU Public License v3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
@@ -29,15 +29,15 @@
 Provides-Extra: sphinx 
 Provides-Extra: sphinx-copybutton 
 Provides-Extra: sphinx-panels 
 License-File: LICENSE
 
 # LTB AMS
 
-Python Software for Power System Dispatch Modeling and Co-Simulation with Dynanic, serving as the market simulator for the [CURENT Largescale Testbed][LTB Repository].
+Python Software for Power System Scheduling Modeling and Co-Simulation with Dynanic, serving as the market simulator for the [CURENT Largescale Testbed][LTB Repository].
 
 [![License: GPL-3.0](https://img.shields.io/badge/License-GPL--3.0-blue.svg)](https://github.com/CURENT/ams/blob/master/LICENSE)
 ![platforms](https://anaconda.org/conda-forge/ltbams/badges/platforms.svg)
 [![Python Versions](https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)](https://www.python.org/)
 ![Repo Size](https://img.shields.io/github/repo-size/CURENT/ams)
 [![GitHub last commit (master)](https://img.shields.io/github/last-commit/CURENT/ams/master?label=last%20commit%20to%20master)](https://github.com/CURENT/ams/commits/master/)
 [![GitHub last commit (develop)](https://img.shields.io/github/last-commit/CURENT/ams/develop?label=last%20commit%20to%20develop)](https://github.com/CURENT/ams/commits/develop/)
@@ -60,15 +60,15 @@
 | Build Status  | [![GitHub Action Status](https://github.com/CURENT/ams/workflows/Python%20application/badge.svg)](https://github.com/curent/ams/actions)  | [![Build Status](https://dev.azure.com/curentltb/ams/_apis/build/status%2FCURENT.ams?branchName=master)](https://dev.azure.com/curentltb/ams/_build/latest?definitionId=2&branchName=master) |
 
 
 # Why AMS
 
 With the built-in interface with dynamic simulation engine, ANDES, AMS enables Dynamics Interfaced Stability Constrained Production Cost and Market Operation Modeling.
 
-AMS produces credible dispatch results and competitive performance.
+AMS produces credible scheduling results and competitive performance.
 The following results show the comparison of DCOPF between AMS and other tools.
 
 | Cost [\$]       |      AMS       |  MATPOWER   | pandapower |
 |----------------:|--------------:|------------:|-----------:|
 | PEGASE 1354-Bus |  1,173,590.63  |  1,173,590.63 |  1,173,590.63 |
 | PEGASE 2869-Bus |  2,338,915.61  |  2,338,915.61 |  2,338,915.61 |
 | GOC 4020-Bus    |    793,634.11  |    793,634.11 |    793,634.11 |
@@ -108,15 +108,15 @@
 Install from GitHub source:
 
 ```bash
 pip install git+https://github.com/CURENT/ams.git
 ```
 
 # Sponsors and Contributors
-AMS is the dispatch simulation engine for the CURENT Largescale Testbed (LTB).
+AMS is the scheduling simulation engine for the CURENT Largescale Testbed (LTB).
 More information about CURENT LTB can be found at the [LTB Repository][LTB Repository].
 
 This work was supported in part by the Engineering Research Center Program of the National Science Foundation and the Department of Energy
 under NSF Award Number EEC-1041877 and the CURENT Industry Partnership Program.
 
 This work was supported in part by the Advanced Grid Research and Development Program in the Office of Electricity at the U.S. Department of Energy.
```

### Comparing `ltbams-0.9.6/ltbams.egg-info/SOURCES.txt` & `ltbams-0.9.7/ltbams.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 ams/report.py
 ams/shared.py
 ams/system.py
 ams/cases/5bus/pjm5bus_demo.xlsx
 ams/cases/5bus/pjm5bus_uced.json
 ams/cases/5bus/pjm5bus_uced.xlsx
 ams/cases/5bus/pjm5bus_uced_esd1.xlsx
+ams/cases/5bus/pjm5bus_uced_ev.xlsx
 ams/cases/ieee123/ieee123.xlsx
 ams/cases/ieee123/ieee123_regcv1.xlsx
 ams/cases/ieee14/ieee14.json
 ams/cases/ieee14/ieee14.raw
 ams/cases/ieee14/ieee14_uced.xlsx
 ams/cases/ieee39/ieee39.xlsx
 ams/cases/ieee39/ieee39_uced.xlsx
@@ -44,14 +45,16 @@
 ams/core/documenter.py
 ams/core/matprocessor.py
 ams/core/model.py
 ams/core/param.py
 ams/core/service.py
 ams/core/symprocessor.py
 ams/core/var.py
+ams/extension/__init__.py
+ams/extension/eva.py
 ams/interop/__init__.py
 ams/interop/andes.py
 ams/io/__init__.py
 ams/io/json.py
 ams/io/matpower.py
 ams/io/psse.py
 ams/io/pypower.py
@@ -65,14 +68,15 @@
 ams/models/line.py
 ams/models/region.py
 ams/models/reserve.py
 ams/models/shunt.py
 ams/models/timeslot.py
 ams/models/distributed/__init__.py
 ams/models/distributed/esd1.py
+ams/models/distributed/ev.py
 ams/models/distributed/pvd1.py
 ams/models/renewable/__init__.py
 ams/models/renewable/regc.py
 ams/models/static/__init__.py
 ams/models/static/gen.py
 ams/models/static/pq.py
 ams/opt/__init__.py
```

### Comparing `ltbams-0.9.6/ltbams.egg-info/requires.txt` & `ltbams-0.9.7/ltbams.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 andes>=1.8.7
 cvxpy
-kvxopt>=1.3.2.0
+kvxopt>=1.3.2.1
 matplotlib
 numpy
 openpyxl
 pandas
 psutil
 pybind11
 scipy
```

### Comparing `ltbams-0.9.6/requirements-extra.txt` & `ltbams-0.9.7/requirements-extra.txt`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/setup.py` & `ltbams-0.9.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 # --- update `extras_conda` to include packages only available in PyPI ---
 
 setup(
     name='ltbams',
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
-    description="Python software for dispatch modeling and co-simulation with dynanic.",
+    description="Python software for scheduling modeling and co-simulation with dynanics.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Jinning Wang",
     author_email='jinninggm@gmail.com',
     url='https://github.com/CURENT/ams',
     packages=find_packages(exclude=[]),
     entry_points={
```

### Comparing `ltbams-0.9.6/tests/test_1st_system.py` & `ltbams-0.9.7/tests/test_1st_system.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/tests/test_addressing.py` & `ltbams-0.9.7/tests/test_addressing.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/tests/test_andes.py` & `ltbams-0.9.7/tests/test_andes.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/tests/test_case.py` & `ltbams-0.9.7/tests/test_case.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/tests/test_dctypes.py` & `ltbams-0.9.7/tests/test_dctypes.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/tests/test_export_csv.py` & `ltbams-0.9.7/tests/test_export_csv.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/tests/test_group.py` & `ltbams-0.9.7/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/tests/test_known_good.py` & `ltbams-0.9.7/tests/test_known_good.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/tests/test_mats.py` & `ltbams-0.9.7/tests/test_mats.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,24 +4,20 @@
 from scipy.sparse import csr_matrix as c_sparse
 from scipy.sparse import lil_matrix as l_sparse
 
 import ams
 from ams.core.matprocessor import MatProcessor, MParam
 
 
-class TestMatProcessor(unittest.TestCase):
+class TestMatProcessorBasic(unittest.TestCase):
     """
-    Test functionality of MatProcessor.
+    Test basic functionality of MatProcessor.
     """
 
     def setUp(self) -> None:
-        # cases is for testing PTDF, LODF, etc.
-        self.cases = ['matpower/case14.m',
-                      'matpower/case39.m',
-                      'matpower/case118.m']
         self.ss = ams.load(ams.get_case("matpower/case300.m"),
                            default_config=True, no_output=True)
         self.nR = self.ss.Region.n
         self.nb = self.ss.Bus.n
         self.nl = self.ss.Line.n
         self.ng = self.ss.StaticGen.n
         self.nsh = self.ss.Shunt.n
@@ -36,45 +32,37 @@
         """
         one_vec = MParam(v=c_sparse(np.ones(self.ss.Bus.n)))
         # check if `_v` is `c_sparse` instance
         self.assertIsInstance(one_vec._v, c_sparse)
         # check if `v` is 1D-array
         self.assertEqual(one_vec.v.shape, (self.ss.Bus.n,))
 
-    def test_cg(self):
+    def test_c(self):
         """
-        Test `Cg`.
+        Test connectivity matrices.
         """
+        # Test `Cg`
         self.assertIsInstance(self.mats.Cg._v, (c_sparse, l_sparse))
         self.assertIsInstance(self.mats.Cg.v, np.ndarray)
         self.assertEqual(self.mats.Cg._v.max(), 1)
         np.testing.assert_equal(self.mats.Cg._v.sum(axis=0), np.ones((1, self.ng)))
 
-    def test_cl(self):
-        """
-        Test `Cl`.
-        """
+        # Test `Cl`
         self.assertIsInstance(self.mats.Cl._v, (c_sparse, l_sparse))
         self.assertIsInstance(self.mats.Cl.v, np.ndarray)
         self.assertEqual(self.mats.Cl._v.max(), 1)
         np.testing.assert_equal(self.mats.Cl._v.sum(axis=0), np.ones((1, self.nD)))
 
-    def test_csh(self):
-        """
-        Test `Csh`.
-        """
+        # Test `Csh`
         self.assertIsInstance(self.mats.Csh._v, (c_sparse, l_sparse))
         self.assertIsInstance(self.mats.Csh.v, np.ndarray)
         self.assertEqual(self.mats.Csh._v.max(), 1)
         np.testing.assert_equal(self.mats.Csh._v.sum(axis=0), np.ones((1, self.nsh)))
 
-    def test_cft(self):
-        """
-        Test `Cft`.
-        """
+        # Test `Cft`
         self.assertIsInstance(self.mats.Cft._v, (c_sparse, l_sparse))
         self.assertIsInstance(self.mats.Cft.v, np.ndarray)
         self.assertEqual(self.mats.Cft._v.max(), 1)
         np.testing.assert_equal(self.mats.Cft._v.sum(axis=0), np.zeros((1, self.nl)))
 
     def test_b_calc(self):
         """
@@ -108,76 +96,85 @@
     def test_pbusinj(self):
         """
         Test `Pbusinj`.
         """
         self.assertIsInstance(self.mats.Pbusinj._v, np.ndarray)
         np.testing.assert_equal(self.mats.Pbusinj._v.shape, (self.nb,))
 
-    def test_ptdf(self):
+
+class TestMatProcessorTDFs(unittest.TestCase):
+    """
+    Test PTDF, LODF, OTDF.
+    """
+
+    def setUp(self) -> None:
+        self.cases = ['matpower/case14.m',
+                      'matpower/case39.m',
+                      'matpower/case118.m']
+
+    def test_ptdf_before_mat_init(self):
         """
-        Test `PTDF`.
+        Test `PTDF` before MatProcessor initialization.
         """
 
         for case in self.cases:
             ss = ams.load(ams.get_case(case),
                           setup=True, default_config=True, no_output=True)
-            ss.DCOPF.run(solver='ECOS')
 
-            ptdf = ss.mats.build_ptdf()
+            _ = ss.mats.build_ptdf(no_store=True)
+            self.assertIsNone(ss.mats.PTDF._v)
+
+            _ = ss.mats.build_ptdf(dtype='float64', no_store=False)
+            self.assertEqual(ss.mats.PTDF._v.shape, (ss.Line.n, ss.Bus.n))
+            self.assertEqual(ss.mats.PTDF._v.dtype, np.float64)
 
-            plf = ss.DCOPF.plf.v
-            plfc = ptdf@(ss.mats.Cg._v@ss.DCOPF.pg.v - ss.mats.Cl._v@ss.DCOPF.pd.v)
-            np.testing.assert_allclose(plf, plfc, atol=1e-2)
+            ptdf = ss.mats.build_ptdf(dtype='float32', no_store=True)
+            self.assertEqual(ptdf.dtype, np.float32)
 
-    def test_lodf(self):
+    def test_lodf_before_ptdf(self):
         """
-        Test `LODF`.
+        Test `LODF` before `PTDF`.
         """
+
         for case in self.cases:
             ss = ams.load(ams.get_case(case),
                           setup=True, default_config=True, no_output=True)
-            # build matrices
-            ss.mats.build()
-            _ = ss.mats.build_ptdf()
-            lodf = ss.mats.build_lodf()
 
-            # outage line
-            oline_idx = ss.Line.idx.v[1]
-            oline = ss.Line.idx2uid(oline_idx)
+            _ = ss.mats.build_lodf(no_store=True)
+            self.assertIsNone(ss.mats.LODF._v)
 
-            # pre-outage
-            ss.DCPF.run()
-            plf0 = ss.DCPF.plf.v.copy()
+            _ = ss.mats.build_lodf(dtype='float64', no_store=False)
+            self.assertEqual(ss.mats.LODF._v.dtype, np.float64)
 
-            # post-outage
-            ss.Line.set(src='u', attr='v', idx=oline_idx, value=0)
-            ss.DCPF.update()
-            ss.DCPF.run()
-            plf1 = ss.DCPF.plf.v.copy()
+            lodf = ss.mats.build_lodf(dtype='float32', no_store=True)
+            self.assertEqual(lodf.dtype, np.float32)
 
-            dplf = plf1 - plf0
-            dplfc = -lodf[:, oline] * dplf[oline]
-
-            np.testing.assert_allclose(dplf, dplfc, atol=1e-7)
-
-    def test_otdf(self):
+    def test_otdf_before_lodf(self):
         """
         Test `OTDF`.
         """
 
         for case in self.cases:
             ss = ams.load(ams.get_case(case),
                           setup=True, default_config=True, no_output=True)
             # build matrices
             ss.mats.build()
 
-            oline_idx = ss.Line.idx.v[1]
+            otdf64 = ss.mats.build_otdf(dtype='float64')
+            self.assertEqual(otdf64.dtype, np.float64)
+
+            otdf32 = ss.mats.build_otdf(dtype='float32')
+            self.assertEqual(otdf32.dtype, np.float32)
 
-            otdf = ss.mats.build_otdf(line=oline_idx)
+            np.testing.assert_allclose(otdf64, otdf32, atol=1e-3)
 
-            ss.Line.set(src='u', attr='v', idx=oline_idx, value=0)
-            ss.DCPF.run()
+            # input str
+            otdf_l2 = ss.mats.build_otdf(line=ss.Line.idx.v[2])
+            self.assertEqual(otdf_l2.shape, (ss.Line.n, ss.Bus.n))
 
-            plf = ss.DCPF.plf.v
-            plfc = otdf@(ss.mats.Cg._v@ss.DCPF.pg.v - ss.mats.Cl._v@ss.DCPF.pd.v)
+            # input list with single element
+            otdf_l2 = ss.mats.build_otdf(line=ss.Line.idx.v[2:3])
+            self.assertEqual(otdf_l2.shape, (ss.Line.n, ss.Bus.n))
 
-            np.testing.assert_allclose(plf, plfc, atol=1e-7)
+            # input list with multiple elements
+            otdf_l23 = ss.mats.build_otdf(line=ss.Line.idx.v[2:5])
+            self.assertEqual(otdf_l23.shape, (ss.Line.n, ss.Bus.n))
```

### Comparing `ltbams-0.9.6/tests/test_model.py` & `ltbams-0.9.7/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/tests/test_paths.py` & `ltbams-0.9.7/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/tests/test_report.py` & `ltbams-0.9.7/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/tests/test_repr.py` & `ltbams-0.9.7/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/tests/test_routine.py` & `ltbams-0.9.7/tests/test_routine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import unittest
 import numpy as np
 
+from andes.shared import pd
+
 import ams
 
 
 class TestRoutineMethods(unittest.TestCase):
     """
     Test methods of `Routine`.
     """
@@ -48,14 +50,17 @@
 
         # get an unpacked var value
         self.ss.DCOPF.run(solver='ECOS')
         self.assertEqual(self.ss.DCOPF.exit_code, 0, "Exit code is not 0.")
         np.testing.assert_equal(self.ss.DCOPF.get('pg', 'PV_30', 'v'),
                                 self.ss.StaticGen.get('p', 'PV_30', 'v'))
 
+        # test input type
+        self.assertIsInstance(self.ss.DCOPF.get('pg', pd.Series(['PV_30']), 'v'), np.ndarray)
+
         # test return type
         self.assertIsInstance(self.ss.DCOPF.get('pg', 'PV_30', 'v'), float)
         self.assertIsInstance(self.ss.DCOPF.get('pg', ['PV_30'], 'v'), np.ndarray)
 
         # --- multi period routine ---
         self.ss.ED.run(solver='ECOS')
         self.assertEqual(self.ss.ED.exit_code, 0, "Exit code is not 0.")
```

### Comparing `ltbams-0.9.6/tests/test_service.py` & `ltbams-0.9.7/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `ltbams-0.9.6/versioneer.py` & `ltbams-0.9.7/versioneer.py`

 * *Files identical despite different names*


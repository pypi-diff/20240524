# Comparing `tmp/jaeger-1.7.1.tar.gz` & `tmp/jaeger-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaeger-1.7.1.tar", max compression
+gzip compressed data, was "jaeger-1.7.2.tar", max compression
```

## Comparing `jaeger-1.7.1.tar` & `jaeger-1.7.2.tar`

### file list

```diff
@@ -1,76 +1,77 @@
--rw-r--r--   0        0        0     1504 2024-05-08 15:20:54.176815 jaeger-1.7.1/LICENSE.md
--rw-r--r--   0        0        0     2393 2024-05-08 15:20:54.176815 jaeger-1.7.1/README.md
--rw-r--r--   0        0        0     3613 2024-05-08 15:20:54.180815 jaeger-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     1764 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/__init__.py
--rw-r--r--   0        0        0    20331 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/__main__.py
--rw-r--r--   0        0        0       61 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/__init__.py
--rw-r--r--   0        0        0     5033 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/actor.py
--rw-r--r--   0        0        0      816 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/__init__.py
--rw-r--r--   0        0        0     1029 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/alerts.py
--rw-r--r--   0        0        0     1182 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/can.py
--rw-r--r--   0        0        0     3381 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/chiller.py
--rw-r--r--   0        0        0    35363 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/configuration.py
--rw-r--r--   0        0        0      722 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/debug.py
--rw-r--r--   0        0        0     2690 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/disable.py
--rw-r--r--   0        0        0    15119 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/fvc.py
--rw-r--r--   0        0        0    11373 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/home.py
--rw-r--r--   0        0        0     5314 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/ieb.py
--rw-r--r--   0        0        0     1410 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/pollers.py
--rw-r--r--   0        0        0    16070 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/positioner.py
--rw-r--r--   0        0        0     9994 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/power.py
--rw-r--r--   0        0        0      990 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/snapshot.py
--rw-r--r--   0        0        0     1397 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/talk.py
--rw-r--r--   0        0        0     1034 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/testing.py
--rw-r--r--   0        0        0     3579 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/unwind.py
--rw-r--r--   0        0        0      949 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/version.py
--rw-r--r--   0        0        0    14035 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/alerts.py
--rw-r--r--   0        0        0    21709 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/can.py
--rw-r--r--   0        0        0     5257 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/chiller.py
--rw-r--r--   0        0        0     4054 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/commands/__init__.py
--rw-r--r--   0        0        0    22135 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/commands/base.py
--rw-r--r--   0        0        0     9010 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/commands/bootloader.py
--rw-r--r--   0        0        0    12181 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/commands/calibration.py
--rw-r--r--   0        0        0    10788 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/commands/goto.py
--rw-r--r--   0        0        0     6013 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/commands/status.py
--rw-r--r--   0        0        0    26797 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/commands/trajectory.py
--rw-r--r--   0        0        0    10030 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/chiller_APO.yaml
--rw-r--r--   0        0        0     7487 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/chiller_APO_variables.csv
--rw-r--r--   0        0        0     1317 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/fvc.yaml
--rw-r--r--   0        0        0    10541 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/ieb_APO.yaml
--rw-r--r--   0        0        0    10539 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/ieb_LCO.yaml
--rw-r--r--   0        0        0     3329 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/jaeger_APO.yml
--rw-r--r--   0        0        0     3302 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/jaeger_LCO.yml
--rw-r--r--   0        0        0     8711 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/schema.json
--rw-r--r--   0        0        0     1815 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/sextants/epfl.yaml
--rw-r--r--   0        0        0     2367 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/sextants/osu.yaml
--rw-r--r--   0        0        0     1512 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/sextants/schema.json
--rw-r--r--   0        0        0     2364 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/sextants/uw.yaml
--rw-r--r--   0        0        0     3545 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/exceptions.py
--rw-r--r--   0        0        0    52574 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/fps.py
--rw-r--r--   0        0        0    42572 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/fvc.py
--rw-r--r--   0        0        0     4518 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/ieb.py
--rw-r--r--   0        0        0      162 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/interfaces/__init__.py
--rw-r--r--   0        0        0     1142 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/interfaces/bus.py
--rw-r--r--   0        0        0     6759 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/interfaces/cannet.py
--rw-r--r--   0        0        0    12892 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/interfaces/message.py
--rw-r--r--   0        0        0     1874 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/interfaces/notifier.py
--rw-r--r--   0        0        0     1199 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/interfaces/virtual.py
--rw-r--r--   0        0        0    20177 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/kaiju.py
--rw-r--r--   0        0        0     8034 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/maskbits.py
--rw-r--r--   0        0        0     7797 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/plotting.py
--rw-r--r--   0        0        0    18121 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/positioner.py
--rw-r--r--   0        0        0        0 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/scripts/__init__.py
--rw-r--r--   0        0        0     1851 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/scripts/generate_chiller_yaml.py
--rw-r--r--   0        0        0      346 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/target/__init__.py
--rw-r--r--   0        0        0    18703 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/target/assignment.py
--rw-r--r--   0        0        0    40466 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/target/configuration.py
--rw-r--r--   0        0        0    17185 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/target/coordinates.py
--rw-r--r--   0        0        0    10095 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/target/design.py
--rw-r--r--   0        0        0     5476 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/target/schemas.py
--rw-r--r--   0        0        0    15992 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/target/tools.py
--rw-r--r--   0        0        0    15709 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/testing.py
--rw-r--r--   0        0        0       60 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/utils/__init__.py
--rw-r--r--   0        0        0     9610 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/utils/database.py
--rw-r--r--   0        0        0    14611 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/utils/helpers.py
--rw-r--r--   0        0        0     9549 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/utils/utils.py
--rw-r--r--   0        0        0     4060 1970-01-01 00:00:00.000000 jaeger-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-05-24 18:30:47.797006 jaeger-1.7.2/LICENSE.md
+-rw-r--r--   0        0        0     2393 2024-05-24 18:30:47.797006 jaeger-1.7.2/README.md
+-rw-r--r--   0        0        0     3613 2024-05-24 18:30:47.801006 jaeger-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0     1764 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/__init__.py
+-rw-r--r--   0        0        0    20331 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/__main__.py
+-rw-r--r--   0        0        0       61 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/__init__.py
+-rw-r--r--   0        0        0     5033 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/actor.py
+-rw-r--r--   0        0        0      816 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1029 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/alerts.py
+-rw-r--r--   0        0        0     1182 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/can.py
+-rw-r--r--   0        0        0     3381 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/chiller.py
+-rw-r--r--   0        0        0    35429 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/configuration.py
+-rw-r--r--   0        0        0      722 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/debug.py
+-rw-r--r--   0        0        0     2690 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/disable.py
+-rw-r--r--   0        0        0    15129 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/fvc.py
+-rw-r--r--   0        0        0    11373 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/home.py
+-rw-r--r--   0        0        0     5314 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/ieb.py
+-rw-r--r--   0        0        0     1410 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/pollers.py
+-rw-r--r--   0        0        0    16070 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/positioner.py
+-rw-r--r--   0        0        0     9994 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/power.py
+-rw-r--r--   0        0        0      990 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/snapshot.py
+-rw-r--r--   0        0        0     1397 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/talk.py
+-rw-r--r--   0        0        0     1034 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/testing.py
+-rw-r--r--   0        0        0     3579 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/unwind.py
+-rw-r--r--   0        0        0      949 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/version.py
+-rw-r--r--   0        0        0    14035 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/alerts.py
+-rw-r--r--   0        0        0    21709 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/can.py
+-rw-r--r--   0        0        0     5257 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/chiller.py
+-rw-r--r--   0        0        0     4054 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/commands/__init__.py
+-rw-r--r--   0        0        0    22135 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/commands/base.py
+-rw-r--r--   0        0        0     9010 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/commands/bootloader.py
+-rw-r--r--   0        0        0    12181 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/commands/calibration.py
+-rw-r--r--   0        0        0    10788 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/commands/goto.py
+-rw-r--r--   0        0        0     6013 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/commands/status.py
+-rw-r--r--   0        0        0    26797 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/commands/trajectory.py
+-rw-r--r--   0        0        0    10030 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/etc/chiller_APO.yaml
+-rw-r--r--   0        0        0     7487 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/etc/chiller_APO_variables.csv
+-rw-r--r--   0        0        0     1317 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/etc/fvc.yaml
+-rw-r--r--   0        0        0    10541 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/etc/ieb_APO.yaml
+-rw-r--r--   0        0        0    10539 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/etc/ieb_LCO.yaml
+-rw-r--r--   0        0        0     3597 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/etc/jaeger_APO.yml
+-rw-r--r--   0        0        0     3347 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/etc/jaeger_LCO.yml
+-rw-r--r--   0        0        0     8711 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/etc/schema.json
+-rw-r--r--   0        0        0     1815 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/etc/sextants/epfl.yaml
+-rw-r--r--   0        0        0     2367 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/etc/sextants/osu.yaml
+-rw-r--r--   0        0        0     1512 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/etc/sextants/schema.json
+-rw-r--r--   0        0        0     2364 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/etc/sextants/uw.yaml
+-rw-r--r--   0        0        0     3545 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/exceptions.py
+-rw-r--r--   0        0        0    52574 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/fps.py
+-rw-r--r--   0        0        0    42576 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/fvc.py
+-rw-r--r--   0        0        0     4518 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/ieb.py
+-rw-r--r--   0        0        0      162 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/interfaces/__init__.py
+-rw-r--r--   0        0        0     1142 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/interfaces/bus.py
+-rw-r--r--   0        0        0     6759 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/interfaces/cannet.py
+-rw-r--r--   0        0        0    12892 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/interfaces/message.py
+-rw-r--r--   0        0        0     1874 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/interfaces/notifier.py
+-rw-r--r--   0        0        0     1199 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/interfaces/virtual.py
+-rw-r--r--   0        0        0    20177 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/kaiju.py
+-rw-r--r--   0        0        0     8034 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/maskbits.py
+-rw-r--r--   0        0        0     7797 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/plotting.py
+-rw-r--r--   0        0        0    18121 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/positioner.py
+-rw-r--r--   0        0        0        0 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/scripts/__init__.py
+-rw-r--r--   0        0        0     1851 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/scripts/generate_chiller_yaml.py
+-rw-r--r--   0        0        0      346 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/target/__init__.py
+-rw-r--r--   0        0        0    19651 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/target/assignment.py
+-rw-r--r--   0        0        0    41675 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/target/configuration.py
+-rw-r--r--   0        0        0    19864 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/target/coordinates.py
+-rw-r--r--   0        0        0    12248 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/target/design.py
+-rw-r--r--   0        0        0     6580 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/target/schemas.py
+-rw-r--r--   0        0        0    11232 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/target/too.py
+-rw-r--r--   0        0        0    16554 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/target/tools.py
+-rw-r--r--   0        0        0    15709 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/testing.py
+-rw-r--r--   0        0        0       60 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/utils/__init__.py
+-rw-r--r--   0        0        0     9610 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/utils/database.py
+-rw-r--r--   0        0        0    14611 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/utils/helpers.py
+-rw-r--r--   0        0        0     9164 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/utils/utils.py
+-rw-r--r--   0        0        0     4060 1970-01-01 00:00:00.000000 jaeger-1.7.2/PKG-INFO
```

### Comparing `jaeger-1.7.1/LICENSE.md` & `jaeger-1.7.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/README.md` & `jaeger-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/pyproject.toml` & `jaeger-1.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jaeger"
-version = "1.7.1"
+version = "1.7.2"
 description = "Controllers for the SDSS-V FPS"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/jaeger"
 repository = "https://github.com/sdss/jaeger"
 documentation = "https://sdss-jaeger.readthedocs.io/en/latest/"
@@ -25,15 +25,15 @@
 [tool.poetry.dependencies]
 python = "^3.10,<3.13"
 sdss-drift = "^1.0.0"
 sdss-clu = "^2.0.0"
 sdsstools = "^1.6.0"
 sdssdb = "^0.11.3"
 sdss-kaiju =  [
-    {version="^1.4.0b1", python=">=3.11"},
+    {version="^1.4.0b5", python=">=3.11"},
     {version="^1.3.0,<1.4.0", python=">=3.10,<3.11"}
 ]
 sdss-coordio = "^1.11.0"
 click_default_group = ">=1.2.2"
 "zc.lockfile" = "^2.0"
 polars = "^0.20.9"
 adbc-driver-postgresql = ">=0.9.0"
```

### Comparing `jaeger-1.7.1/src/jaeger/__init__.py` & `jaeger-1.7.2/src/jaeger/__init__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/__main__.py` & `jaeger-1.7.2/src/jaeger/__main__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/actor/actor.py` & `jaeger-1.7.2/src/jaeger/actor/actor.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/actor/commands/__init__.py` & `jaeger-1.7.2/src/jaeger/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/actor/commands/alerts.py` & `jaeger-1.7.2/src/jaeger/actor/commands/alerts.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/actor/commands/can.py` & `jaeger-1.7.2/src/jaeger/actor/commands/can.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/actor/commands/chiller.py` & `jaeger-1.7.2/src/jaeger/actor/commands/chiller.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/actor/commands/configuration.py` & `jaeger-1.7.2/src/jaeger/actor/commands/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,14 +203,16 @@
         try:
             command.debug(text=f"Epoch delay: {round(epoch_delay, 1)} seconds.")
 
             if epoch is None:
                 epoch = float(Time.now().jd)
             epoch += epoch_delay / 86400.0
 
+            command.debug(text=f"Effective epoch: {epoch:.6f}.")
+
             design = await Design.create_async(
                 design_id,
                 epoch=epoch,
                 scale=scale,
                 safety_factor=safety_factor,
                 offset_min_skybrightness=offset_min_skybrightness,
                 boss_wavelength=boss_wavelength,
```

### Comparing `jaeger-1.7.1/src/jaeger/actor/commands/debug.py` & `jaeger-1.7.2/src/jaeger/actor/commands/debug.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/actor/commands/disable.py` & `jaeger-1.7.2/src/jaeger/actor/commands/disable.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/actor/commands/fvc.py` & `jaeger-1.7.2/src/jaeger/actor/commands/fvc.py`

 * *Files 1% similar despite different names*

```diff
@@ -434,15 +434,15 @@
 
             command.info(fvc_rms=new_rms)
 
             if current_rms is None:
                 pass
             else:
                 delta_rms = current_rms - new_rms
-                command.info(fvc_deltarms=delta_rms)
+                command.info(fvc_deltarms=round(delta_rms, 2))
             current_rms = new_rms
 
             command.info(fvc_perc_90=round(fvc.perc_90 * 1000.0, 2))
             command.info(fvc_percent_reached=round(fvc.fvc_percent_reached, 1))
 
             # 4. Check if we have reached the distance criterion.
             if target_90_percentile and fvc.perc_90 * 1000.0 <= target_90_percentile:
```

### Comparing `jaeger-1.7.1/src/jaeger/actor/commands/home.py` & `jaeger-1.7.2/src/jaeger/actor/commands/home.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/actor/commands/ieb.py` & `jaeger-1.7.2/src/jaeger/actor/commands/ieb.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/actor/commands/pollers.py` & `jaeger-1.7.2/src/jaeger/actor/commands/pollers.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/actor/commands/positioner.py` & `jaeger-1.7.2/src/jaeger/actor/commands/positioner.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/actor/commands/power.py` & `jaeger-1.7.2/src/jaeger/actor/commands/power.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/actor/commands/snapshot.py` & `jaeger-1.7.2/src/jaeger/actor/commands/snapshot.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/actor/commands/talk.py` & `jaeger-1.7.2/src/jaeger/actor/commands/talk.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/actor/commands/testing.py` & `jaeger-1.7.2/src/jaeger/actor/commands/testing.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/actor/commands/unwind.py` & `jaeger-1.7.2/src/jaeger/actor/commands/unwind.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/actor/commands/version.py` & `jaeger-1.7.2/src/jaeger/actor/commands/version.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/alerts.py` & `jaeger-1.7.2/src/jaeger/alerts.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/can.py` & `jaeger-1.7.2/src/jaeger/can.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/chiller.py` & `jaeger-1.7.2/src/jaeger/chiller.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/commands/__init__.py` & `jaeger-1.7.2/src/jaeger/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/commands/base.py` & `jaeger-1.7.2/src/jaeger/commands/base.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/commands/bootloader.py` & `jaeger-1.7.2/src/jaeger/commands/bootloader.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/commands/calibration.py` & `jaeger-1.7.2/src/jaeger/commands/calibration.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/commands/goto.py` & `jaeger-1.7.2/src/jaeger/commands/goto.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/commands/status.py` & `jaeger-1.7.2/src/jaeger/commands/status.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/commands/trajectory.py` & `jaeger-1.7.2/src/jaeger/commands/trajectory.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/etc/chiller_APO.yaml` & `jaeger-1.7.2/src/jaeger/etc/chiller_APO.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/etc/chiller_APO_variables.csv` & `jaeger-1.7.2/src/jaeger/etc/chiller_APO_variables.csv`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/etc/fvc.yaml` & `jaeger-1.7.2/src/jaeger/etc/fvc.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/etc/ieb_APO.yaml` & `jaeger-1.7.2/src/jaeger/etc/ieb_APO.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/etc/ieb_LCO.yaml` & `jaeger-1.7.2/src/jaeger/etc/ieb_LCO.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/etc/jaeger_APO.yml` & `jaeger-1.7.2/src/jaeger/etc/jaeger_LCO.yml`

 * *Files 3% similar despite different names*

```diff
@@ -42,37 +42,38 @@
 fps:
   use_database: true
   allow_unknown: true
   initialise_timeouts: 0.5
   start_pollers: false
   status_poller_delay: 5
   position_poller_delay: 5
-  disabled_positioners: []
+  disabled_positioners: [1074, 759, 1286]
   offline_positioners: null
   disable_collision_detection_positioners: []
   open_loop_positioners: []
   use_sync_line: false
   snapshot_path: /data/logs/jaeger/snapshots/
   configuration_snapshot_path: /data/logs/jaeger/configuration_snapshots/
+  robot_grid_dumps: /data/logs/jaeger/grids/
   use_lock: True
 
 ieb:
-  config: etc/ieb_APO.yaml
+  config: etc/ieb_LCO.yaml
   disabled_devices: []
 
 positioner:
   reduction_ratio: 1024
   motor_steps: 1073741824
   time_step: 0.0005
   motor_speed: 2000
   initialise_datums_timeout: 300
   disable_precise_moves: true
   uid_bits: 6
-  trajectory_data_n_points: 3
-  firmware_messages_per_positioner: 16
+  trajectory_data_n_points: 10
+  firmware_messages_per_positioner: 8
   trajectory_dump_path: /data/logs/jaeger/trajectories/
 
 kaiju:
   speed: 2
   ang_step: 0.1
   collision_buffer: 2.0
   smooth_points: 21
@@ -81,49 +82,47 @@
   epsilon_factor: 2
   lattice_position: [10., 170.]
   default_path_generator: mdp
   greed: 0.7
   phobia: 0.6
 
 configuration:
-  default_focal_scale: 1
-  scale_temperature_coeffs: [1.01810522e-05, 9.99758691e-01]
+  default_focal_scale: 1.0003
+  scale_temperature_coeffs: null
   use_guider_scale: true
   guider_max_scale_age: 3600
-  clip_scale: 500
-  scale_fudge_factor: 0.99988
+  clip_scale: 3000
+  scale_fudge_factor: 0.9986
   max_cloned_time: 4500
   max_designs_epoch: 4
 
 fvc:
   config: etc/fvc.yaml
   exposure_time: 5.
-  fbi_level: 4.
-  dark_image: /data/fcam/calib/60062/fimg-fvc1n-0011.fits
-  polids: null
+  fbi_level: 9.
+  dark_image: /data/fcam/calib/60062/fimg-fvc1s-0001.fits
+  polids: [0, 1, 2, 3, 4, 5, 6, 9, 20, 27, 28, 29, 30]
   target_90_percentile: 30.0
   target_distance: 5
   max_fvc_iterations: 2
-  centroid_method: zbplus2
-  check_rotator: true
+  centroid_method: null
+  check_rotator: false
   k: 1.0
   max_correction: 15
   ieb_keys:
     TEMPRTD2: rtd2
     TEMPRTD3: rtd3
     TEMPT3: t3
     LED1: led1
     LED2: led2
     LED3: led3
     LED4: led4
 
 chiller:
-  config: etc/chiller_APO.yaml
-  temperature: auto
-  flow: 6
+  config: null
 
 files:
   log_dir: /data/logs/jaeger
 
 low_temperature:
   sensor: RTD2
   cold_threshold: 0
@@ -144,15 +143,15 @@
   dbname: sdss5db
   user: sdss_user
   host: sdss5-db
   port: 5432
 
 alerts:
   interval: 60
-  enabled: ['gfa', 'ieb', 'robot', 'flow', 'temperature', 'chiller']
+  enabled: ['gfa', 'ieb', 'robot', 'flow', 'temperature']
   gfa:
     warning: 30
     critical: 35
     shutdown: true
   ieb:
     sensor: RTD1
     warning: 35
```

### Comparing `jaeger-1.7.1/src/jaeger/etc/jaeger_LCO.yml` & `jaeger-1.7.2/src/jaeger/etc/jaeger_APO.yml`

 * *Files 6% similar despite different names*

```diff
@@ -42,37 +42,38 @@
 fps:
   use_database: true
   allow_unknown: true
   initialise_timeouts: 0.5
   start_pollers: false
   status_poller_delay: 5
   position_poller_delay: 5
-  disabled_positioners: [1074, 759, 1286]
+  disabled_positioners: []
   offline_positioners: null
   disable_collision_detection_positioners: []
   open_loop_positioners: []
   use_sync_line: false
   snapshot_path: /data/logs/jaeger/snapshots/
   configuration_snapshot_path: /data/logs/jaeger/configuration_snapshots/
+  robot_grid_dumps: /data/logs/jaeger/grids/
   use_lock: True
 
 ieb:
-  config: etc/ieb_LCO.yaml
+  config: etc/ieb_APO.yaml
   disabled_devices: []
 
 positioner:
   reduction_ratio: 1024
   motor_steps: 1073741824
   time_step: 0.0005
   motor_speed: 2000
   initialise_datums_timeout: 300
   disable_precise_moves: true
   uid_bits: 6
-  trajectory_data_n_points: 10
-  firmware_messages_per_positioner: 8
+  trajectory_data_n_points: 3
+  firmware_messages_per_positioner: 16
   trajectory_dump_path: /data/logs/jaeger/trajectories/
 
 kaiju:
   speed: 2
   ang_step: 0.1
   collision_buffer: 2.0
   smooth_points: 21
@@ -81,47 +82,56 @@
   epsilon_factor: 2
   lattice_position: [10., 170.]
   default_path_generator: mdp
   greed: 0.7
   phobia: 0.6
 
 configuration:
-  default_focal_scale: 1.0003
-  scale_temperature_coeffs: null
+  default_focal_scale: 1
+  scale_temperature_coeffs: [1.01810522e-05, 9.99758691e-01]
   use_guider_scale: true
   guider_max_scale_age: 3600
-  clip_scale: 3000
-  scale_fudge_factor: 0.9986
+  clip_scale: 500
+  scale_fudge_factor: 0.99988
   max_cloned_time: 4500
   max_designs_epoch: 4
+  targets_of_opportunity:
+    replace: false
+    path: $TOO_DATA_DIR/current
+    exclude_design_modes: ['^.+?_eng$', '^.+?_rm_?.*$']
+    max_replacements: 2
+    categories: ['science']
+    minimum_priority: [6000, 3000, 0]
 
 fvc:
   config: etc/fvc.yaml
   exposure_time: 5.
-  fbi_level: 9.
-  dark_image: /data/fcam/calib/60062/fimg-fvc1s-0001.fits
-  polids: [0, 1, 2, 3, 4, 5, 6, 9, 20, 27, 28, 29, 30]
+  fbi_level: 4.
+  dark_image: /data/fcam/calib/60062/fimg-fvc1n-0011.fits
+  polids: null
   target_90_percentile: 30.0
   target_distance: 5
   max_fvc_iterations: 2
-  centroid_method: null
-  check_rotator: false
+  centroid_method: zbplus2
+  check_rotator: true
   k: 1.0
   max_correction: 15
   ieb_keys:
     TEMPRTD2: rtd2
     TEMPRTD3: rtd3
     TEMPT3: t3
     LED1: led1
     LED2: led2
     LED3: led3
     LED4: led4
 
 chiller:
-  config: null
+  config: etc/chiller_APO.yaml
+  temperature: auto
+  flow: 6
 
 files:
   log_dir: /data/logs/jaeger
 
 low_temperature:
   sensor: RTD2
   cold_threshold: 0
@@ -142,15 +152,15 @@
   dbname: sdss5db
   user: sdss_user
   host: sdss5-db
   port: 5432
 
 alerts:
   interval: 60
-  enabled: ['gfa', 'ieb', 'robot', 'flow', 'temperature']
+  enabled: ['gfa', 'ieb', 'robot', 'flow', 'temperature', 'chiller']
   gfa:
     warning: 30
     critical: 35
     shutdown: true
   ieb:
     sensor: RTD1
     warning: 35
```

### Comparing `jaeger-1.7.1/src/jaeger/etc/schema.json` & `jaeger-1.7.2/src/jaeger/etc/schema.json`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/etc/sextants/epfl.yaml` & `jaeger-1.7.2/src/jaeger/etc/sextants/epfl.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/etc/sextants/osu.yaml` & `jaeger-1.7.2/src/jaeger/etc/sextants/osu.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/etc/sextants/schema.json` & `jaeger-1.7.2/src/jaeger/etc/sextants/schema.json`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/etc/sextants/uw.yaml` & `jaeger-1.7.2/src/jaeger/etc/sextants/uw.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/exceptions.py` & `jaeger-1.7.2/src/jaeger/exceptions.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/fps.py` & `jaeger-1.7.2/src/jaeger/fps.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/fvc.py` & `jaeger-1.7.2/src/jaeger/fvc.py`

 * *Files 1% similar despite different names*

```diff
@@ -923,15 +923,15 @@
             robot.setDestinationAlphaBeta(positioner.alpha, positioner.beta)
 
             offset_data = offsets.filter(polars.col.positioner_id == robot.id)
 
             if len(offset_data) == 0 or len(offset_data) > 1:
                 raise ValueError(f"Invalid offset data for positioner {robot.id}.")
 
-            if offset_data[0, "transformation_valid"]:
+            if not offset_data[0, "transformation_valid"]:
                 continue
 
             new = offset_data[["alpha_new", "beta_new"]]
             dist = offset_data[["xwok_distance", "ywok_distance"]] * 1000.0
 
             meas_distance = numpy.hypot(dist["xwok_distance"], dist["ywok_distance"])[0]
             if meas_distance > target_distance:
```

### Comparing `jaeger-1.7.1/src/jaeger/ieb.py` & `jaeger-1.7.2/src/jaeger/ieb.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/interfaces/bus.py` & `jaeger-1.7.2/src/jaeger/interfaces/bus.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/interfaces/cannet.py` & `jaeger-1.7.2/src/jaeger/interfaces/cannet.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/interfaces/message.py` & `jaeger-1.7.2/src/jaeger/interfaces/message.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/interfaces/notifier.py` & `jaeger-1.7.2/src/jaeger/interfaces/notifier.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/interfaces/virtual.py` & `jaeger-1.7.2/src/jaeger/interfaces/virtual.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/kaiju.py` & `jaeger-1.7.2/src/jaeger/kaiju.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/maskbits.py` & `jaeger-1.7.2/src/jaeger/maskbits.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/plotting.py` & `jaeger-1.7.2/src/jaeger/plotting.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/positioner.py` & `jaeger-1.7.2/src/jaeger/positioner.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/scripts/generate_chiller_yaml.py` & `jaeger-1.7.2/src/jaeger/scripts/generate_chiller_yaml.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/target/assignment.py` & `jaeger-1.7.2/src/jaeger/target/assignment.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 from jaeger import config, log
 from jaeger.target.coordinates import (
     icrs_from_positioner_dataframe,
     positioner_from_icrs_dataframe,
 )
 from jaeger.target.schemas import FIBRE_DATA_SCHEMA
+from jaeger.utils import Timer
 
 from .tools import get_wok_data
 
 
 if TYPE_CHECKING:
     from .configuration import Configuration, DitheredConfiguration, ManualConfiguration
 
@@ -79,20 +80,22 @@
 
         self.wok_data = get_wok_data(self.observatory)
 
         if self.design:
             self.target_data = self.design.target_data
             self.position_angle = self.design.field.position_angle
         else:
-            self.target_data = {}
+            self.target_data = None
             self.position_angle = 0.0
 
         self.boresight: Observed | None = None
 
-        self.fibre_data = self.create_fibre_data()
+        with Timer() as timer:
+            self.fibre_data = self.create_fibre_data()
+        log.debug(f"Created fibre data in {timer.elapsed:.2f} s.")
 
     def __repr__(self):
         return f"<{self.__class__.__name__} (design_id={self.design_id})>"
 
     @property
     def epoch(self):
         """Returns the configuratione epoch."""
@@ -158,32 +161,43 @@
                     "pmra": None,
                     "pmdec": None,
                     "parallax": None,
                     "coord_epoch": None,
                     "delta_ra": None,
                     "delta_dec": None,
                     "assigned": False,
+                    "too": False,
                 }
 
-                if hole_id in tdata and tdata[hole_id]["fibre_type"] == fibre_type:
-                    hole_data.update(
-                        {
-                            "catalogid": tdata[hole_id]["catalogid"],
-                            "ra_icrs": tdata[hole_id]["ra"],
-                            "dec_icrs": tdata[hole_id]["dec"],
-                            "pmra": tdata[hole_id]["pmra"],
-                            "pmdec": tdata[hole_id]["pmdec"],
-                            "parallax": tdata[hole_id]["parallax"],
-                            "coord_epoch": tdata[hole_id]["epoch"],
-                            "delta_ra": tdata[hole_id]["delta_ra"],
-                            "delta_dec": tdata[hole_id]["delta_dec"],
-                            "assigned": True,
-                        }
+                if tdata is not None:
+                    # Get the target data row for this hole and fibre.
+                    tdata_row = tdata.filter(
+                        polars.col.hole_id == hole_id,
+                        polars.col.fibre_type == fibre_type,
                     )
 
+                    if len(tdata_row) == 1:
+                        tdata_row_dict = tdata_row.rows(named=True)[0]
+
+                        hole_data.update(
+                            {
+                                "catalogid": tdata_row_dict["catalogid"],
+                                "ra_icrs": tdata_row_dict["ra"],
+                                "dec_icrs": tdata_row_dict["dec"],
+                                "pmra": tdata_row_dict["pmra"],
+                                "pmdec": tdata_row_dict["pmdec"],
+                                "parallax": tdata_row_dict["parallax"],
+                                "coord_epoch": tdata_row_dict["epoch"],
+                                "delta_ra": tdata_row_dict["delta_ra"],
+                                "delta_dec": tdata_row_dict["delta_dec"],
+                                "assigned": True,
+                                "too": tdata_row_dict["is_too"],
+                            }
+                        )
+
                 fibre_tdata.append(hole_data)
 
         # Create initial DF from wok_data. This contains 1500 columns, one per fibre.
         fibre_data = polars.DataFrame(fibre_tdata)
 
         # Add empty columns for the rest of the schema. Negate boolean columns.
         fibre_data = (
@@ -321,15 +335,18 @@
             configuration,
             scale=scale,
             boss_wavelength=boss_wavelength,
             apogee_wavelength=apogee_wavelength,
         )
 
         if compute_coordinates:
-            self.compute_coordinates(epoch)
+            log.debug("Computing coordinates for assignment.")
+            with Timer() as timer:
+                self.compute_coordinates(epoch)
+            log.debug(f"Computed coordinates in {timer.elapsed:.2f} s.")
 
     def compute_coordinates(self, epoch: Optional[float] = None):
         """Computes coordinates in different systems.
 
         Parameters
         ----------
         epoch
@@ -358,42 +375,42 @@
         fibre_data_icrs = self.fibre_data.filter(
             polars.col("ra_icrs").is_not_null(),
             polars.col("dec_icrs").is_not_null(),
         )
 
         # Get the positioner data for the targets with ICRS. The returned
         # dataframe has the same height and all the same columns, but populated.
-        pos_data = positioner_from_icrs_dataframe(
+        assigned = positioner_from_icrs_dataframe(
             fibre_data_icrs,
             self.boresight,
             self.site,
             epoch=epoch,
             position_angle=self.design.field.position_angle,
             focal_plane_scale=self.scale,
         )
 
         # A couple sanity checks.
-        assert pos_data.height == fibre_data_icrs.height
-        assert pos_data.columns == fibre_data_icrs.columns
+        assert assigned.height == fibre_data_icrs.height
+        assert assigned.columns == fibre_data_icrs.columns
 
         # We mark these fibres as "assigned".
-        pos_data = pos_data.with_columns(assigned=True, on_target=True)
+        assigned = assigned.with_columns(assigned=True, on_target=True)
 
         # Now get a data frame with the fibres that are not assigned.
         unassigned = self.fibre_data.filter(
             polars.col("index").is_in(fibre_data_icrs["index"]).not_()
         )
 
         # For these the positioner alpha/beta coordinates are the same as for the
-        # positioner with the same positioner_id in pos_data. We create lists
+        # positioner with the same positioner_id in assigned. We create lists
         # of the same height as unassinged and then add them.
         alpha_unassigned: list[float] = []
         beta_unassigned: list[float] = []
         for row in unassigned.iter_rows(named=True):
-            pid_data = pos_data.filter(polars.col.positioner_id == row["positioner_id"])
+            pid_data = assigned.filter(polars.col.positioner_id == row["positioner_id"])
             if pid_data.height == 0:
                 alpha_unassigned.append(numpy.nan)
                 beta_unassigned.append(numpy.nan)
             else:
                 alpha_unassigned.append(pid_data["alpha"][0])
                 beta_unassigned.append(pid_data["beta"][0])
 
@@ -419,15 +436,15 @@
             position_angle=self.design.field.position_angle,
             focal_plane_scale=self.scale,
         )
         icrs_unassigned = icrs_unassigned.with_columns(assigned=False, on_target=False)
 
         # Join the two dataframes. Recast and resort.
         fibre_data = (
-            polars.concat([pos_data, icrs_unassigned])
+            polars.concat([assigned, icrs_unassigned])
             .sort("index")
             .cast(FIBRE_DATA_SCHEMA)
         )
 
         self.fibre_data = fibre_data
 
         # Mark all the fibres as valid for now. .validate() will set them to False
@@ -536,14 +553,18 @@
 
         fdata = fdata.with_columns(
             alpha=polars.Series(alphas),
             beta=polars.Series(betas),
             valid=True,
         )
 
+        # Artificially assign all the BOSS fibres.
+        boss_idx = (fdata["fibre_type"] == "BOSS").arg_true()
+        fdata[boss_idx, "assigned"] = True
+
         fdata = (
             icrs_from_positioner_dataframe(
                 fdata,
                 self.site,
                 boresight=self.boresight,
                 epoch=self.site.time.jd,
                 position_angle=self.position_angle,
```

### Comparing `jaeger-1.7.1/src/jaeger/target/configuration.py` & `jaeger-1.7.2/src/jaeger/target/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # @Author: José Sánchez-Gallego (gallegoj@uw.edu)
 # @Date: 2021-11-10
 # @Filename: configuration.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 from __future__ import annotations
 
+import json
 import logging
 import os
 import pathlib
 import shutil
 from copy import deepcopy
 from time import time
 
@@ -50,14 +51,15 @@
     get_robot_grid,
     get_snapshot_async,
     load_robot_grid,
     warn,
 )
 from jaeger.target.assignment import Assignment, BaseAssignment, ManualAssignment
 from jaeger.target.tools import copy_summary_file, get_fibermap_table, get_wok_data
+from jaeger.utils import Timer
 from jaeger.utils.database import connect_database
 from jaeger.utils.helpers import run_in_executor
 
 
 if TYPE_CHECKING:
     from clu import Command
 
@@ -110,15 +112,18 @@
 
         self.design: Design | None = None
         self.design_id: int | None = None
 
         self.extra_summary_data = {}
 
         self.fps = fps
-        self.robot_grid = self._initialise_grid()
+
+        with Timer() as timer:
+            self.robot_grid = self._initialise_grid()
+        log.debug(f"Initialised robot grid in {timer.elapsed:.2f} seconds.")
 
         self.command: Command[JaegerActor] | None = None
 
         self._decollided: list[int] = []
 
         self.to_destination: TrajectoryType = None
         self.from_destination: TrajectoryType = None
@@ -399,14 +404,30 @@
 
                 self.update_coordinates_from_robot_grid(positioner_ids=decollided)
 
             # Final check for collisions.
             if len(self.robot_grid.getCollidedRobotList()) > 0:
                 raise TrajectoryError("The robot grid remains collided.")
 
+        # Save the grid before trying to generate paths. Mostly for debugging
+        # if something fails.
+        now = Time.now()
+        grid_dump = dump_robot_grid(self.robot_grid)
+        grid_dump_path = os.path.join(
+            config["fps"]["robot_grid_dumps"],
+            str(get_sjd(self.assignment.observatory.upper())),
+            f"grid_dump_{now.isot}.json",
+        )
+
+        try:
+            os.makedirs(os.path.dirname(grid_dump_path), exist_ok=True)
+            json.dump(grid_dump, open(grid_dump_path, "w"))
+        except Exception as ee:
+            self.log(f"Error saving grid dump: {ee}", level=logging.ERROR)
+
         # Fix deadlocks (this sets the trajectories in the instance).
         self.log("Generating path pair.")
         n_retries = n_deadlock_retries if resolve_deadlocks else -1
         unlocked = await self._resolve_deadlocks(
             n_retries=n_retries,
             path_generation_mode=path_generation_mode,
             force=force,
@@ -683,41 +704,44 @@
                 self.configuration_id = None
 
                 return self.write_to_database(replace=False)
 
         a_data = self.fibre_data.clone()
         a_data = a_data.with_columns(cs.ends_with("focal").fill_nan(None))
 
+        target_data_hole = self.design.get_target_data_dict() if self.design else None
+
         focals = []
         for row in a_data.iter_rows(named=True):
             pid = row["positioner_id"]
             hole_id = row["hole_id"]
             assigned = row["assigned"]
 
             if row["valid"]:
                 xfocal = row["xfocal"]
                 yfocal = row["yfocal"]
             else:
                 xfocal = yfocal = None
 
-            if self.design and hole_id in self.design.target_data and assigned:
-                assignment_pk = self.design.target_data[hole_id]["assignment_pk"]
+            if target_data_hole and hole_id in target_data_hole and assigned:
+                assignment_pk = target_data_hole[hole_id]["assignment_pk"]
             else:
                 assignment_pk = None
 
             focals.append(
                 dict(
                     assignment_pk=assignment_pk,
                     xfocal=xfocal,
                     yfocal=yfocal,
                     positioner_id=pid,
                     fiber_type=row["fibre_type"].lower(),
                     configuration_id=self.configuration_id,
                     catalogid=row["catalogid"],
                     assigned=assigned,
+                    replaced=row["too"],
                 )
             )
 
         with opsdb.database.atomic():
             opsdb.AssignmentToFocal.insert_many(focals).execute(opsdb.database)
 
     @staticmethod
@@ -768,14 +792,15 @@
 
         adata = self.assignment
 
         fdata = fibre_data if fibre_data is not None else self.fibre_data.clone()
         fdata = fdata.with_columns(cs.numeric().fill_null(-999).fill_nan(-999))
 
         design = self.design
+        target_data_hole = design.get_target_data_dict() if design else None
 
         header = {
             "configuration_id": self.configuration_id,
             "robostrategy_run": "NA",
             "fps_calibrations_version": calibration.fps_calibs_version,
             "jaeger_version": jaeger_version,
             "coordio_version": coordio_version,
@@ -835,14 +860,15 @@
             row.update(
                 {
                     "positionerId": pid,
                     "holeId": hole_id,
                     "fiberType": fibre_type.upper(),
                     "assigned": int(row_data["assigned"]),
                     "valid": int(row_data["valid"]),
+                    "too": int(row_data["too"]),
                     "on_target": int(row_data["on_target"]),
                     "xwok": row_data["xwok"],
                     "ywok": row_data["ywok"],
                     "zwok": row_data["zwok"],
                     "xFocal": row_data["xfocal"],
                     "yFocal": row_data["yfocal"],
                     "alpha": row_data["alpha"],
@@ -856,16 +882,16 @@
                     "spectrographId": spec_id,
                     "fiberId": row_data["fibre_id"],
                     "lambda_eff": row_data["wavelength"],
                 }
             )
 
             # And now only the one that is associated with a target.
-            if row_data["assigned"] and design and hole_id in design.target_data:
-                target = design.target_data[hole_id]
+            if row_data["assigned"] and target_data_hole:
+                target = target_data_hole[hole_id]
                 row.update(
                     {
                         "racat": target["ra"],
                         "deccat": target["dec"],
                         "pmra": target["pmra"] or -999.0,
                         "pmdec": target["pmdec"] or -999.0,
                         "parallax": target["parallax"] or -999.0,
@@ -959,21 +985,25 @@
         boss_wavelength: float | None = None,
         apogee_wavelength: float | None = None,
     ):
         super().__init__(fps=fps, scale=scale)
 
         self.design = design
         self.design_id = design.design_id
-        self.assignment = Assignment(
-            self,
-            epoch=epoch,
-            scale=scale,
-            boss_wavelength=boss_wavelength,
-            apogee_wavelength=apogee_wavelength,
-        )
+
+        log.info("Creating assignment instance.")
+        with Timer() as timer:
+            self.assignment = Assignment(
+                self,
+                epoch=epoch,
+                scale=scale,
+                boss_wavelength=boss_wavelength,
+                apogee_wavelength=apogee_wavelength,
+            )
+        log.debug(f"Assignment instance created in {timer.elapsed:.2f} seconds.")
 
         assert self.assignment.site.time
 
         self.epoch = self.assignment.site.time.jd
         self.scale = scale
 
     def __repr__(self):
```

### Comparing `jaeger-1.7.1/src/jaeger/target/coordinates.py` & `jaeger-1.7.2/src/jaeger/target/coordinates.py`

 * *Files 10% similar despite different names*

```diff
@@ -382,16 +382,19 @@
     if boresight is not None:
         field = Field(focal, field_center=boresight)
         obs = Observed(field, site=site, wavelength=wavelength)
         icrs = ICRS(obs)
     else:
         field = obs = icrs = None
 
-    # Add focal coordinates. These always exist.
+    # Add wok and focal coordinates. These always exist.
     data = data.with_columns(
+        xwok=polars.Series(xwok),
+        ywok=polars.Series(ywok),
+        zwok=polars.Series(zwok),
         xfocal=polars.Series(focal[:, 0]),
         yfocal=polars.Series(focal[:, 1]),
     )
 
     # The field, observed, ICRS coordinates depend on whether there is a boresight.
     if icrs is not None and obs is not None and field is not None:
         data = data.with_columns(
@@ -544,7 +547,87 @@
         dx=positioner_data[0, "dx"],
         dy=positioner_data[0, "dy"],
     )
 
     wok_coords = numpy.array(wok)
 
     return wok_coords, numpy.array([tangent[0], tangent[1], 0])
+
+
+def apply_proper_motions(data: polars.DataFrame, epoch: float | None = None):
+    """Propagates ICRs coordinates to a given epoch handling missing values.
+
+    Parameters
+    ----------
+    data
+        A data frame with at least columns ``ra`` and ``dec`` which must be
+        ICRS coordinates in degrees. Optionally the data frame can have columns
+        ``pmra``, ``pmdec``, and ``epoch`` in ``mas/yr`` and ``JD`` respectively.
+        ``epoch`` is the epoch of the input coordinates.
+    epoch
+        The epoch, in Julian year, to which to propagate the input coordinates.
+        Defaults to the current time.
+
+    Returns
+    -------
+    data_epoch
+        A data frame with columns ``ra``, ``dec``, and ``epoch`` with the ICRS
+        coordinates of each target at ``epoch``.
+
+    """
+
+    data = data.clone()
+
+    now = Time.now().jd
+    epoch = epoch or now
+
+    # Add missing columns.
+    if "pmra" not in data.columns:
+        data = data.with_columns(pmra=polars.lit(0.0, dtype=polars.Float32))
+
+    if "pmdec" not in data.columns:
+        data = data.with_columns(pmdec=polars.lit(0.0, dtype=polars.Float32))
+
+    # If the epoch column is missing the pmra and pmdec columns are irrelevant.
+    if "epoch" not in data.columns:
+        data = data.with_columns(
+            pmra=polars.lit(0.0, dtype=polars.Float32),
+            pmdec=polars.lit(0.0, dtype=polars.Float32),
+            epoch=polars.lit(epoch, dtype=polars.Float32),
+        )
+
+    # Find rows with missing proper motions and set them to zero.
+    invalid_data = data.select(
+        (
+            polars.col.ra.is_null()
+            | polars.col.ra.is_nan()
+            | polars.col.dec.is_null()
+            | polars.col.dec.is_nan()
+            | polars.col.epoch.is_null()
+            | polars.col.epoch.is_nan()
+        )
+        .arg_true()
+        .alias("index")
+    )
+
+    data[invalid_data["index"], "pmra"] = 0.0
+    data[invalid_data["index"], "pmdec"] = 0.0
+    data[invalid_data["index"], "epoch"] = epoch
+
+    # Propagate coordinates.
+    icrs = ICRS(
+        numpy.array([data["ra"].to_numpy(), data["dec"].to_numpy()]).T,
+        pmra=data["pmra"].to_numpy(),
+        pmdec=data["pmdec"].to_numpy(),
+        epoch=Time(data["epoch"].to_numpy(), format="jyear").jd,
+    )
+    icrs_epoch = icrs.to_epoch(epoch)
+
+    data_epoch = polars.DataFrame(
+        {
+            "ra": polars.Series(icrs_epoch[:, 0], dtype=polars.Float64),
+            "dec": polars.Series(icrs_epoch[:, 1], dtype=polars.Float64),
+            "epoch": epoch,
+        }
+    )
+
+    return data_epoch
```

### Comparing `jaeger-1.7.1/src/jaeger/target/design.py` & `jaeger-1.7.2/src/jaeger/target/design.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,26 +6,31 @@
 # @Filename: design.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 
+from typing import Any
+
 import numpy
 import peewee
 import polars
 
 from coordio.defaults import calibration
 from coordio.utils import object_offset
 from sdssdb.peewee.sdss5db import targetdb
 
 from jaeger import config, log
 from jaeger.fps import FPS
+from jaeger.target.schemas import TARGET_DATA_SCHEMA
+from jaeger.target.too import add_targets_of_opportunity_to_design
 from jaeger.utils.database import connect_database
 from jaeger.utils.helpers import run_in_executor
+from jaeger.utils.utils import Timer
 
 from .configuration import Configuration
 
 
 __all__ = ["Design"]
 
 
@@ -59,59 +64,80 @@
         `None`, uses the current time.
     scale
         Focal plane scale factor to apply. Defaults to coordio's internal value.
     safety_factor
         For offset calculation. Factor to add to ``mag_limit``. See ``object_offset``.
     offset_min_skybrightness
         Minimum sky brightness for the offset. See ``object_offset``.
+    use_targets_of_opportunity
+        Whether to replace targets with targets of opportunity accoding to the
+        parameters in ``configuration.targets_of_opportunity``.
 
     """
 
     def __init__(
         self,
         design_id: int,
         fps: FPS | None = None,
         create_configuration: bool = True,
         epoch: float | None = None,
         scale: float | None = None,
         safety_factor: float = 0.1,
         offset_min_skybrightness: float = 0.5,
+        use_targets_of_opportunity: bool = True,
     ):
         if calibration.wokCoords is None:
             raise RuntimeError("Cannot retrieve wok calibration. Is $WOKCALIB_DIR set?")
 
+        log.info(f"Creating Design instance for design_id={design_id}.")
+
         self.fps = fps or FPS.get_instance()
         self.design_id = design_id
 
         if connect_database(targetdb.database) is False:
             raise RuntimeError("Cannot connect to database.")
 
-        try:
-            self.design = targetdb.Design.get(design_id=design_id)
-        except peewee.DoesNotExist:
-            raise ValueError(f"design_id {design_id} does not exist in the database.")
+        with Timer() as timer:
+            try:
+                self.design = targetdb.Design.get(design_id=design_id)
+            except peewee.DoesNotExist:
+                raise ValueError(f"design_id {design_id} does not exist in DB.")
+
+        log.debug(f"Design data retrieved from DB in {timer.elapsed:.2f} s.")
 
         self.field = FieldData(
             field_id=self.design.field.field_id,
             rs_run=self.design.field.version.plan if self.design else "NA",
             observatory=self.design.field.observatory.label,
             racen=self.design.field.racen,
             deccen=self.design.field.deccen,
             position_angle=self.design.field.position_angle,
         )
 
         self.safety_factor = safety_factor
         self.offset_min_skybrightness = offset_min_skybrightness
-        self.target_data: dict[str, dict] = self.get_target_data()
+
+        log.debug("Loading target data and calculating offsets.")
+        with Timer() as timer:
+            self.target_data: polars.DataFrame = self.get_target_data()
+        log.debug(f"Loaded target data in {timer.elapsed:.2f} s.")
+
+        self.replaced_target_data: polars.DataFrame | None = None
+
+        if use_targets_of_opportunity:
+            with Timer() as timer:
+                add_targets_of_opportunity_to_design(self)
+            log.debug(f"Added targets of opportunity in {timer.elapsed:.2f} s.")
 
         self.configuration: Configuration
         if create_configuration:
+            log.info(f"Creating configuration for design_id={design_id}.")
             self.configuration = Configuration(self, fps=fps, epoch=epoch, scale=scale)
 
-    def get_target_data(self) -> dict[str, dict]:
+    def get_target_data(self) -> polars.DataFrame:
         """Retrieves target data as a dictionary."""
 
         # TODO: this is all synchronous which is probably ok because this
         # query should run in < 1s, but at some point maybe we can change
         # this to use async-peewee and aiopg.
 
         if connect_database(targetdb.database) is False:
@@ -121,23 +147,41 @@
             targetdb.Design.select(
                 targetdb.Assignment.pk.alias("assignment_pk"),
                 targetdb.CartonToTarget.pk.alias("carton_to_target_pk"),
                 targetdb.CartonToTarget.lambda_eff,
                 targetdb.CartonToTarget.delta_ra,
                 targetdb.CartonToTarget.delta_dec,
                 targetdb.CartonToTarget.can_offset,
-                targetdb.Target,
-                targetdb.Magnitude,
-                targetdb.Hole.holeid,
+                targetdb.CartonToTarget.priority,
+                targetdb.Target.catalogid,
+                targetdb.Target.ra,
+                targetdb.Target.dec,
+                targetdb.Target.epoch,
+                targetdb.Target.pmra,
+                targetdb.Target.pmdec,
+                targetdb.Target.parallax,
+                targetdb.Magnitude.bp,
+                targetdb.Magnitude.g,
+                targetdb.Magnitude.h,
+                targetdb.Magnitude.i,
+                targetdb.Magnitude.z,
+                targetdb.Magnitude.r,
+                targetdb.Magnitude.rp,
+                targetdb.Magnitude.gaia_g,
+                targetdb.Magnitude.j,
+                targetdb.Magnitude.k,
+                targetdb.Magnitude.optical_prov,
+                targetdb.Hole.holeid.alias("hole_id"),
                 targetdb.Instrument.label.alias("fibre_type"),
                 targetdb.Cadence.label.alias("cadence"),
                 targetdb.Carton.carton,
                 targetdb.Category.label.alias("category"),
                 targetdb.Carton.program,
                 targetdb.Design.design_mode,
+                peewee.SQL("false").alias("is_too"),
             )
             .join(targetdb.Assignment)
             .join(targetdb.CartonToTarget)
             .join(targetdb.Target)
             .switch(targetdb.CartonToTarget)
             .join(targetdb.Carton)
             .join(targetdb.Category, peewee.JOIN.LEFT_OUTER)
@@ -149,19 +193,21 @@
             .join(targetdb.Hole)
             .switch(targetdb.Assignment)
             .join(targetdb.Instrument)
             .where(targetdb.Design.design_id == self.design_id)
             .dicts()
         )
 
+        target_data = polars.DataFrame(list(target_data), schema=TARGET_DATA_SCHEMA)
+
         target_data = self.calculate_offsets(target_data)
 
-        return {data["holeid"]: data for data in list(target_data)}
+        return target_data
 
-    def calculate_offsets(self, target_data: list[dict]):
+    def calculate_offsets(self, target_data: polars.DataFrame):
         """Determines the target offsets."""
 
         def _offset(group: polars.DataFrame):
             design_mode = group[0, "design_mode"]
             fibre_type = group[0, "fibre_type"]
 
             design_mode_rec = targetdb.DesignMode.get(label=design_mode)
@@ -199,15 +245,15 @@
             if can_offset.any():
                 # TODO: this should not be necessary but right now there's a bug in
                 # object_offset that will return delta_ra=-1 when the design_mode
                 # doesn't have any magnitude limits defined.
 
                 delta_ra, delta_dec, _ = object_offset(
                     mag,
-                    mag_lim,
+                    numpy.array(mag_lim),
                     lunation,
                     fibre_type.capitalize(),
                     config["observatory"].upper(),
                     can_offset=can_offset,
                     skybrightness=skybrightness,
                     safety_factor=self.safety_factor,
                     offset_min_skybrightness=self.offset_min_skybrightness,
@@ -223,21 +269,19 @@
                 delta_ra=polars.Series(values=delta_ra, dtype=polars.Float32),
                 delta_dec=polars.Series(values=delta_dec, dtype=polars.Float32),
             )
 
         log.debug(f"offset_min_skybrightness={self.offset_min_skybrightness}")
         log.debug(f"safety_factor={self.safety_factor}")
 
-        # Convert to data frame to group by fibre type (no need to group by design
-        # mode since a design can only have one design mode).
-        df = polars.DataFrame(list(target_data), infer_schema_length=None)
-        df = df.groupby("fibre_type").apply(_offset)
+        # Group by fibre type and apply the offset calculation. delta_ra and delta_dec
+        # are modified and target_data is updated.
+        target_data = target_data.groupby("fibre_type").apply(_offset)
 
-        # Return as a list of dicts again.
-        return df.rows(named=True)
+        return target_data
 
     @classmethod
     def check_design(cls, design_id: int, site: str):
         """Checks if a design exists and is for the current observatory."""
 
         if connect_database(targetdb.database) is False:
             raise RuntimeError("Database is not connected.")
@@ -273,14 +317,15 @@
         apogee_wavelength: float | None = None,
         **kwargs,
     ):
         """Returns a design while creating the configuration in an executor."""
 
         self = cls(design_id, fps=fps, create_configuration=False, **kwargs)
 
+        log.info(f"Creating configuration for design_id={self.design_id}.")
         configuration = await run_in_executor(
             Configuration,
             self,
             fps=fps,
             epoch=epoch,
             scale=scale,
             boss_wavelength=boss_wavelength,
@@ -288,7 +333,14 @@
         )
         self.configuration = configuration
 
         return self
 
     def __repr__(self):
         return f"<Design (design_id={self.design_id})>"
+
+    def get_target_data_dict(self) -> dict[str, dict[str, Any]]:
+        """Returns a dictionary of the target data keyed by ``hole_id``."""
+
+        td_dicts = self.target_data.to_dicts()
+
+        return {td["hole_id"]: td for td in td_dicts}
```

### Comparing `jaeger-1.7.1/src/jaeger/target/schemas.py` & `jaeger-1.7.2/src/jaeger/target/schemas.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,25 +11,31 @@
 from typing import Mapping
 
 import numpy
 import polars
 import polars.type_aliases
 
 
-__all__ = ["CONFSUMMARY_FIBER_MAP_SCHEMA", "FIBRE_DATA_SCHEMA", "CONFIGURATION_SCHEMA"]
+__all__ = [
+    "CONFSUMMARY_FIBER_MAP_SCHEMA",
+    "FIBRE_DATA_SCHEMA",
+    "CONFIGURATION_SCHEMA",
+    "TARGET_DATA_SCHEMA",
+]
 
 
 CONFSUMMARY_FIBER_MAP_SCHEMA = [
     ("positionerId", numpy.int16, -999),
     ("holeId", "U7", ""),
     ("fiberType", "U10", ""),
     ("assigned", numpy.int16, 0),
     ("on_target", numpy.int16, 0),
     ("valid", numpy.int16, 0),
     ("decollided", numpy.int16, 0),
+    ("too", numpy.int16, 0),
     ("xwok", numpy.float64, -999.0),
     ("ywok", numpy.float64, -999.0),
     ("zwok", numpy.float64, -999.0),
     ("xFocal", numpy.float64, -999.0),
     ("yFocal", numpy.float64, -999.0),
     ("alpha", numpy.float32, -999.0),
     ("beta", numpy.float32, -999.0),
@@ -78,14 +84,15 @@
     "fibre_type": polars.String,
     "hole_id": polars.String,
     "fibre_id": polars.Int32,
     "site": polars.String,
     "assigned": polars.Boolean,
     "reassigned": polars.Boolean,
     "valid": polars.Boolean,
+    "too": polars.Boolean,
     "on_target": polars.Boolean,
     "disabled": polars.Boolean,
     "offline": polars.Boolean,
     "deadlocked": polars.Boolean,
     "decollided": polars.Boolean,
     "dubious": polars.Boolean,
     "wavelength": polars.Float32,
@@ -161,7 +168,44 @@
         "optical_prov": polars.String,
         "gaia_bp_mag": polars.Float32,
         "gaia_rp_mag": polars.Float32,
         "gaia_g_mag": polars.Float32,
         "tmass_h_mag": polars.Float32,
     }
 )
+
+
+TARGET_DATA_SCHEMA = {
+    "assignment_pk": polars.Int64,
+    "carton_to_target_pk": polars.Int64,
+    "lambda_eff": polars.Float32,
+    "delta_ra": polars.Float32,
+    "delta_dec": polars.Float32,
+    "can_offset": polars.Boolean,
+    "priority": polars.Int32,
+    "catalogid": polars.Int64,
+    "dec": polars.Float64,
+    "epoch": polars.Float32,
+    "pmdec": polars.Float32,
+    "pmra": polars.Float32,
+    "ra": polars.Float64,
+    "parallax": polars.Float32,
+    "bp": polars.Float32,
+    "g": polars.Float32,
+    "h": polars.Float32,
+    "i": polars.Float32,
+    "z": polars.Float32,
+    "r": polars.Float32,
+    "rp": polars.Float32,
+    "gaia_g": polars.Float32,
+    "j": polars.Float32,
+    "k": polars.Float32,
+    "optical_prov": polars.String,
+    "hole_id": polars.String,
+    "fibre_type": polars.String,
+    "cadence": polars.String,
+    "carton": polars.String,
+    "category": polars.String,
+    "program": polars.String,
+    "design_mode": polars.String,
+    "is_too": polars.Boolean,
+}
```

### Comparing `jaeger-1.7.1/src/jaeger/target/tools.py` & `jaeger-1.7.2/src/jaeger/target/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import numpy
 import polars
 from astropy.time import Time
 
 from coordio import __version__ as coordio_version
 from coordio.defaults import calibration
 from kaiju import __version__ as kaiju_version
+from sdssdb.peewee.sdss5db import database
 from sdsstools import yanny
 from sdsstools.time import get_sjd
 
 import jaeger.target
 from jaeger import __version__ as jaeger_version
 from jaeger import config, log
 from jaeger.exceptions import JaegerError
@@ -434,17 +435,16 @@
             robostategy_run=polars.lit(design.field.rs_run),
             field_if=design.field.field_id,
             ra_cen=design.field.racen,
             dec_cen=design.field.deccen,
             pa=design.field.position_angle,
         )
 
-    # Additional target information.
-    if configuration.assignment.target_data != {}:
-        target_data: dict[str, dict[str, Any]] = configuration.assignment.target_data
+        # Additional target information.
+        target_data = configuration.design.get_target_data_dict()
 
         # Iterate over each target and update the relevant columns.
         for irow, row in enumerate(data.iter_rows(named=True)):
             hole_id = row["hole_id"]
             assigned = row["assigned"]
 
             if not assigned or hole_id not in target_data:
@@ -454,14 +454,15 @@
 
             data[irow, "lambda_design"] = target["lambda_eff"]
             data[irow, "carton_to_target_pk"] = target["carton_to_target_pk"]
             data[irow, "cadence"] = target["cadence"]
             data[irow, "firstcarton"] = target["carton"]
             data[irow, "program"] = target["program"]
             data[irow, "category"] = target["category"]
+            data[irow, "too"] = target["is_too"]
 
             data[irow, "sloan_g_mag"] = target["g"]
             data[irow, "sloan_r_mag"] = target["r"]
             data[irow, "sloan_i_mag"] = target["i"]
             data[irow, "sloan_z_mag"] = target["z"]
             data[irow, "gaia_bp_mag"] = target["bp"]
             data[irow, "gaia_rp_mag"] = target["rp"]
@@ -500,7 +501,27 @@
             write_path = summary_dir / f"configuration-{configuration_id}.parquet"
 
         write_path = pathlib.Path(write_path)
         write_path.parent.mkdir(parents=True, exist_ok=True)
         data.write_parquet(write_path)
 
     return data
+
+
+def get_tonight_targets():
+    """Returns a list of ``catalogids`` observed tonight."""
+
+    observatory = config["observatory"]
+    mjd = get_sjd(observatory)
+
+    opsdb = f"opsdb_{observatory}"
+    df = polars.read_database(
+        f"""
+        SELECT a2f.catalogid from {opsdb}.assignment_to_focal a2f
+            JOIN {opsdb}.configuration c USING (configuration_id)
+            JOIN {opsdb}.design_to_status d2s USING (design_id)
+        WHERE mjd IS NOT NULL AND mjd >= {mjd}
+        """,
+        database,
+    )
+
+    return df
```

### Comparing `jaeger-1.7.1/src/jaeger/testing.py` & `jaeger-1.7.2/src/jaeger/testing.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/utils/database.py` & `jaeger-1.7.2/src/jaeger/utils/database.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/utils/helpers.py` & `jaeger-1.7.2/src/jaeger/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.1/src/jaeger/utils/utils.py` & `jaeger-1.7.2/src/jaeger/utils/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,35 +4,33 @@
 # @Author: José Sánchez-Gallego (gallegoj@uw.edu)
 # @Date: 2018-09-11
 # @Filename: utils.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 from __future__ import annotations
 
-import os
+import time
 
-from typing import Optional, Tuple
+from typing import Tuple
 
 import numpy
-from astropy.time import Time
 
 from jaeger import config
-from jaeger.exceptions import JaegerError
 from jaeger.maskbits import ResponseCode
 
 
 __all__ = [
     "get_dtype_str",
     "int_to_bytes",
     "bytes_to_int",
     "get_identifier",
     "parse_identifier",
     "motor_steps_to_angle",
     "get_goto_move_time",
-    "get_sjd",
+    "Timer",
 ]
 
 
 MOTOR_STEPS = config["positioner"]["motor_steps"]
 
 
 def get_dtype_str(dtype, byteorder="little"):
@@ -310,34 +308,30 @@
     """
 
     speed = speed or config["positioner"]["motor_speed"]
 
     return move * config["positioner"]["reduction_ratio"] / (6.0 * speed) + 0.25
 
 
-def get_sjd(observatory: Optional[str] = None) -> int:
-    """Returns the SDSS Julian Date as an integer based on the observatory.
+class Timer:
+    """Convenience context manager to time events.
 
-    Parameters
-    ----------
-    observatory
-        The current observatory, either APO or LCO. If `None`, uses ``$OBSERVATORY``.
+    Modified from https://bit.ly/3ebdp3y.
 
     """
 
-    if observatory is None:
-        try:
-            observatory = os.environ["OBSERVATORY"]
-        except KeyError:
-            raise JaegerError("Observatory not passed and $OBSERVATORY is not set.")
-
-    observatory = observatory.upper()
-    if observatory not in ["APO", "LCO"]:
-        raise JaegerError(f"Invalid observatory {observatory}.")
+    def __enter__(self):
+        self.start = time.time()
+        self.end = None
+        return self
+
+    def __exit__(self, *args):
+        self.end = time.time()
+        self.interval = self.end - self.start
 
-    time = Time.now()
-    mjd = time.mjd
+    @property
+    def elapsed(self):
 
-    if observatory == "APO":
-        return int(mjd + 0.3)
-    else:
-        return int(mjd + 0.4)
+        if self.end:
+            return self.interval
+
+        return time.time() - self.start
```

### Comparing `jaeger-1.7.1/PKG-INFO` & `jaeger-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaeger
-Version: 1.7.1
+Version: 1.7.2
 Summary: Controllers for the SDSS-V FPS
 Home-page: https://github.com/sdss/jaeger
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.10,<3.13
@@ -24,15 +24,15 @@
 Requires-Dist: nptyping (>=2.5.0,<3.0.0)
 Requires-Dist: polars (>=0.20.9,<0.21.0)
 Requires-Dist: pyarrow (>=15.0.0)
 Requires-Dist: sdss-clu (>=2.0.0,<3.0.0)
 Requires-Dist: sdss-coordio (>=1.11.0,<2.0.0)
 Requires-Dist: sdss-drift (>=1.0.0,<2.0.0)
 Requires-Dist: sdss-kaiju (>=1.3.0,<1.4.0) ; python_version >= "3.10" and python_version < "3.11"
-Requires-Dist: sdss-kaiju (>=1.4.0b1,<2.0.0) ; python_version >= "3.11"
+Requires-Dist: sdss-kaiju (>=1.4.0b5,<2.0.0) ; python_version >= "3.11"
 Requires-Dist: sdssdb (>=0.11.3,<0.12.0)
 Requires-Dist: sdsstools (>=1.6.0,<2.0.0)
 Requires-Dist: tables (>=3.9.2,<4.0.0)
 Requires-Dist: zc.lockfile (>=2.0,<3.0)
 Project-URL: Documentation, https://sdss-jaeger.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/sdss/jaeger
 Description-Content-Type: text/markdown
```


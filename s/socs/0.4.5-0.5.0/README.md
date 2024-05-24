# Comparing `tmp/socs-0.4.5.tar.gz` & `tmp/socs-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socs-0.4.5.tar", last modified: Mon Jan  8 20:43:00 2024, max compression
+gzip compressed data, was "socs-0.5.0.tar", last modified: Fri May 24 20:12:44 2024, max compression
```

## Comparing `socs-0.4.5.tar` & `socs-0.5.0.tar`

### file list

```diff
@@ -1,226 +1,232 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.493485 socs-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-01-08 20:42:49.000000 socs-0.4.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-08 20:42:49.000000 socs-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-01-08 20:43:00.493485 socs-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-01-08 20:42:49.000000 socs-0.4.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-08 20:42:49.000000 socs-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-01-08 20:43:00.493485 socs-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-01-08 20:42:49.000000 socs-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.493485 socs-0.4.5/socs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.465485 socs-0.4.5/socs/Lakeshore/
--rw-r--r--   0 runner    (1001) docker     (127)    15686 2024-01-08 20:42:49.000000 socs-0.4.5/socs/Lakeshore/Lakeshore240.py
--rw-r--r--   0 runner    (1001) docker     (127)    40327 2024-01-08 20:42:49.000000 socs-0.4.5/socs/Lakeshore/Lakeshore336.py
--rw-r--r--   0 runner    (1001) docker     (127)    56866 2024-01-08 20:42:49.000000 socs-0.4.5/socs/Lakeshore/Lakeshore370.py
--rw-r--r--   0 runner    (1001) docker     (127)    57740 2024-01-08 20:42:49.000000 socs-0.4.5/socs/Lakeshore/Lakeshore372.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1444 2024-01-08 20:42:49.000000 socs-0.4.5/socs/Lakeshore/Lakeshore425.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/Lakeshore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-01-08 20:42:49.000000 socs-0.4.5/socs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-08 20:43:00.493485 socs-0.4.5/socs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.465485 socs-0.4.5/socs/agents/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.465485 socs-0.4.5/socs/agents/acti_camera/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/acti_camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/acti_camera/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.465485 socs-0.4.5/socs/agents/acu/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/acu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   109979 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/acu/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    25342 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/acu/avoidance.py
--rw-r--r--   0 runner    (1001) docker     (127)    21718 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/acu/drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/acu/exercisor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.465485 socs-0.4.5/socs/agents/bluefors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/bluefors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/bluefors/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.465485 socs-0.4.5/socs/agents/cryomech_cpa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/cryomech_cpa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14370 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/cryomech_cpa/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.465485 socs-0.4.5/socs/agents/fts_aerotech/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/fts_aerotech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12424 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/fts_aerotech/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.465485 socs-0.4.5/socs/agents/generator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17702 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/generator/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.465485 socs-0.4.5/socs/agents/holo_fpga/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/holo_fpga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/holo_fpga/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.469485 socs-0.4.5/socs/agents/holo_synth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/holo_synth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/holo_synth/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.469485 socs-0.4.5/socs/agents/hwp_encoder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29446 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_encoder/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.469485 socs-0.4.5/socs/agents/hwp_gripper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_gripper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27795 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_gripper/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.469485 socs-0.4.5/socs/agents/hwp_gripper/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_gripper/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_gripper/drivers/gripper_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.469485 socs-0.4.5/socs/agents/hwp_pcu/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_pcu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_pcu/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.469485 socs-0.4.5/socs/agents/hwp_pcu/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_pcu/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_pcu/drivers/hwp_pcu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.469485 socs-0.4.5/socs/agents/hwp_picoscope/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_picoscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_picoscope/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.469485 socs-0.4.5/socs/agents/hwp_picoscope/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_picoscope/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_picoscope/drivers/class_ps3000a.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.469485 socs-0.4.5/socs/agents/hwp_pid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_pid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13968 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_pid/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.469485 socs-0.4.5/socs/agents/hwp_pid/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_pid/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11003 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_pid/drivers/pid_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.473485 socs-0.4.5/socs/agents/hwp_pmx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_pmx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_pmx/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.473485 socs-0.4.5/socs/agents/hwp_pmx/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_pmx/drivers/PMX_ethernet.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_pmx/drivers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.473485 socs-0.4.5/socs/agents/hwp_supervisor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_supervisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38272 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/hwp_supervisor/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.473485 socs-0.4.5/socs/agents/ibootbar/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/ibootbar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18557 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/ibootbar/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.473485 socs-0.4.5/socs/agents/ifm_sbn246_flowmeter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/ifm_sbn246_flowmeter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/ifm_sbn246_flowmeter/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.473485 socs-0.4.5/socs/agents/labjack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/labjack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20965 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/labjack/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.473485 socs-0.4.5/socs/agents/labjack/cal_curves/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/labjack/cal_curves/GA10K4D25_cal_curve.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.473485 socs-0.4.5/socs/agents/lakeshore240/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/lakeshore240/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12026 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/lakeshore240/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.473485 socs-0.4.5/socs/agents/lakeshore336/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/lakeshore336/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48306 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/lakeshore336/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.473485 socs-0.4.5/socs/agents/lakeshore370/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/lakeshore370/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36049 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/lakeshore370/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.473485 socs-0.4.5/socs/agents/lakeshore372/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/lakeshore372/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    66303 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/lakeshore372/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.477485 socs-0.4.5/socs/agents/lakeshore425/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/lakeshore425/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9229 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/lakeshore425/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.477485 socs-0.4.5/socs/agents/magpie/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/magpie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37829 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/magpie/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.477485 socs-0.4.5/socs/agents/meinberg_m1000/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/meinberg_m1000/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/meinberg_m1000/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/ocs_plugin_so.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.477485 socs-0.4.5/socs/agents/pfeiffer_tc400/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/pfeiffer_tc400/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/pfeiffer_tc400/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/pfeiffer_tc400/drivers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.477485 socs-0.4.5/socs/agents/pfeiffer_tpg366/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/pfeiffer_tpg366/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/pfeiffer_tpg366/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.477485 socs-0.4.5/socs/agents/pysmurf_controller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/pysmurf_controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39828 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/pysmurf_controller/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.477485 socs-0.4.5/socs/agents/pysmurf_monitor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/pysmurf_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9920 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/pysmurf_monitor/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.477485 socs-0.4.5/socs/agents/scpi_psu/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/scpi_psu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/scpi_psu/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/scpi_psu/drivers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.477485 socs-0.4.5/socs/agents/smurf_crate_monitor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/smurf_crate_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11231 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/smurf_crate_monitor/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.481485 socs-0.4.5/socs/agents/smurf_file_emulator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/smurf_file_emulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27858 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/smurf_file_emulator/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)   105526 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/smurf_file_emulator/status_sample.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.481485 socs-0.4.5/socs/agents/smurf_stream_simulator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/smurf_stream_simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/smurf_stream_simulator/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.481485 socs-0.4.5/socs/agents/smurf_timing_card/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/smurf_timing_card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/smurf_timing_card/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.481485 socs-0.4.5/socs/agents/suprsync/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/suprsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/suprsync/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.481485 socs-0.4.5/socs/agents/synacc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/synacc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/synacc/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.481485 socs-0.4.5/socs/agents/tektronix3021c/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/tektronix3021c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/tektronix3021c/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/tektronix3021c/drivers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.481485 socs-0.4.5/socs/agents/thorlabs_mc2000b/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/thorlabs_mc2000b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/thorlabs_mc2000b/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.481485 socs-0.4.5/socs/agents/ucsc_radiometer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/ucsc_radiometer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/ucsc_radiometer/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.481485 socs-0.4.5/socs/agents/ups/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/ups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17876 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/ups/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.481485 socs-0.4.5/socs/agents/vantagepro2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/vantagepro2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/vantagepro2/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    14136 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/vantagepro2/drivers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.485485 socs-0.4.5/socs/agents/wiregrid_actuator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/wiregrid_actuator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37235 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/wiregrid_actuator/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.485485 socs-0.4.5/socs/agents/wiregrid_actuator/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)    14540 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/wiregrid_actuator/drivers/Actuator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/wiregrid_actuator/drivers/DigitalIO.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/wiregrid_actuator/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/wiregrid_actuator/limitswitch_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/wiregrid_actuator/stopper_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.485485 socs-0.4.5/socs/agents/wiregrid_encoder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/wiregrid_encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14735 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/wiregrid_encoder/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     9427 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/wiregrid_encoder/drivers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.485485 socs-0.4.5/socs/agents/wiregrid_kikusui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/wiregrid_kikusui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24167 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/wiregrid_kikusui/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.485485 socs-0.4.5/socs/agents/wiregrid_kikusui/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/wiregrid_kikusui/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/wiregrid_kikusui/drivers/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.485485 socs-0.4.5/socs/agents/xy_stage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/xy_stage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-01-08 20:42:49.000000 socs-0.4.5/socs/agents/xy_stage/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.485485 socs-0.4.5/socs/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-01-08 20:42:49.000000 socs-0.4.5/socs/common/moxa_serial.py
--rw-r--r--   0 runner    (1001) docker     (127)    17376 2024-01-08 20:42:49.000000 socs-0.4.5/socs/common/pmx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-01-08 20:42:49.000000 socs-0.4.5/socs/common/prologix_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.489485 socs-0.4.5/socs/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25728 2024-01-08 20:42:49.000000 socs-0.4.5/socs/db/suprsync.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4832 2024-01-08 20:42:49.000000 socs-0.4.5/socs/db/suprsync_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.489485 socs-0.4.5/socs/mibs/
--rw-r--r--   0 runner    (1001) docker     (127)    17434 2024-01-08 20:42:49.000000 socs-0.4.5/socs/mibs/IBOOTPDU-MIB.py
--rw-r--r--   0 runner    (1001) docker     (127)   143372 2024-01-08 20:42:49.000000 socs-0.4.5/socs/mibs/MBG-SNMP-LTNG-MIB.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-01-08 20:42:49.000000 socs-0.4.5/socs/mibs/MBG-SNMP-ROOT-MIB.py
--rw-r--r--   0 runner    (1001) docker     (127)    16838 2024-01-08 20:42:49.000000 socs-0.4.5/socs/mibs/SNMPv2-MIB.py
--rw-r--r--   0 runner    (1001) docker     (127)    38813 2024-01-08 20:42:49.000000 socs-0.4.5/socs/mibs/UPS-MIB.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/mibs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-01-08 20:42:49.000000 socs-0.4.5/socs/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7993 2024-01-08 20:42:49.000000 socs-0.4.5/socs/snmp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.489485 socs-0.4.5/socs/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 20:42:49.000000 socs-0.4.5/socs/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-01-08 20:42:49.000000 socs-0.4.5/socs/testing/device_emulator.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-08 20:42:49.000000 socs-0.4.5/socs/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.489485 socs-0.4.5/socs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-01-08 20:43:00.000000 socs-0.4.5/socs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-01-08 20:43:00.000000 socs-0.4.5/socs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 20:43:00.000000 socs-0.4.5/socs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-08 20:43:00.000000 socs-0.4.5/socs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-01-08 20:43:00.000000 socs-0.4.5/socs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-08 20:43:00.000000 socs-0.4.5/socs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 20:43:00.489485 socs-0.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-01-08 20:42:49.000000 socs-0.4.5/tests/test_device_emulator.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-08 20:42:49.000000 socs-0.4.5/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-08 20:42:49.000000 socs-0.4.5/tests/test_snmp.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-08 20:42:49.000000 socs-0.4.5/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    69022 2024-01-08 20:42:49.000000 socs-0.4.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.746967 socs-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-24 20:12:32.000000 socs-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-24 20:12:32.000000 socs-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-24 20:12:44.746967 socs-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-05-24 20:12:32.000000 socs-0.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-24 20:12:32.000000 socs-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-24 20:12:44.746967 socs-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-24 20:12:32.000000 socs-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.746967 socs-0.5.0/socs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.718968 socs-0.5.0/socs/Lakeshore/
+-rw-r--r--   0 runner    (1001) docker     (127)    15686 2024-05-24 20:12:32.000000 socs-0.5.0/socs/Lakeshore/Lakeshore240.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40327 2024-05-24 20:12:32.000000 socs-0.5.0/socs/Lakeshore/Lakeshore336.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56866 2024-05-24 20:12:32.000000 socs-0.5.0/socs/Lakeshore/Lakeshore370.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57740 2024-05-24 20:12:32.000000 socs-0.5.0/socs/Lakeshore/Lakeshore372.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1444 2024-05-24 20:12:32.000000 socs-0.5.0/socs/Lakeshore/Lakeshore425.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/Lakeshore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-24 20:12:32.000000 socs-0.5.0/socs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-24 20:12:44.746967 socs-0.5.0/socs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.718968 socs-0.5.0/socs/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.718968 socs-0.5.0/socs/agents/acti_camera/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/acti_camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/acti_camera/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.718968 socs-0.5.0/socs/agents/acu/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/acu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   114372 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/acu/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25342 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/acu/avoidance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21718 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/acu/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/acu/exercisor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.718968 socs-0.5.0/socs/agents/bluefors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/bluefors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19214 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/bluefors/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.718968 socs-0.5.0/socs/agents/cryomech_cpa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/cryomech_cpa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14241 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/cryomech_cpa/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.718968 socs-0.5.0/socs/agents/fts_aerotech/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/fts_aerotech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/fts_aerotech/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.718968 socs-0.5.0/socs/agents/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17615 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/generator/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.722967 socs-0.5.0/socs/agents/holo_fpga/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/holo_fpga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/holo_fpga/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.722967 socs-0.5.0/socs/agents/holo_synth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/holo_synth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/holo_synth/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.722967 socs-0.5.0/socs/agents/hwp_encoder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29403 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_encoder/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.722967 socs-0.5.0/socs/agents/hwp_gripper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_gripper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35200 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_gripper/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.722967 socs-0.5.0/socs/agents/hwp_gripper/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_gripper/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_gripper/drivers/gripper_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.722967 socs-0.5.0/socs/agents/hwp_pcu/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_pcu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_pcu/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.722967 socs-0.5.0/socs/agents/hwp_pcu/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_pcu/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_pcu/drivers/hwp_pcu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.722967 socs-0.5.0/socs/agents/hwp_picoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_picoscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_picoscope/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.722967 socs-0.5.0/socs/agents/hwp_picoscope/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_picoscope/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_picoscope/drivers/class_ps3000a.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.722967 socs-0.5.0/socs/agents/hwp_pid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_pid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_pid/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.722967 socs-0.5.0/socs/agents/hwp_pid/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_pid/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17239 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_pid/drivers/pid_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.726967 socs-0.5.0/socs/agents/hwp_pmx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_pmx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16403 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_pmx/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.726967 socs-0.5.0/socs/agents/hwp_pmx/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_pmx/drivers/PMX_ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_pmx/drivers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.726967 socs-0.5.0/socs/agents/hwp_supervisor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_supervisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53348 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/hwp_supervisor/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.726967 socs-0.5.0/socs/agents/ibootbar/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/ibootbar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18519 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/ibootbar/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.726967 socs-0.5.0/socs/agents/ifm_sbn246_flowmeter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/ifm_sbn246_flowmeter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/ifm_sbn246_flowmeter/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.726967 socs-0.5.0/socs/agents/labjack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/labjack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20838 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/labjack/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.726967 socs-0.5.0/socs/agents/labjack/cal_curves/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/labjack/cal_curves/GA10K4D25_cal_curve.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.726967 socs-0.5.0/socs/agents/lakeshore240/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/lakeshore240/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11939 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/lakeshore240/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.726967 socs-0.5.0/socs/agents/lakeshore336/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/lakeshore336/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47661 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/lakeshore336/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.726967 socs-0.5.0/socs/agents/lakeshore370/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/lakeshore370/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35448 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/lakeshore370/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.726967 socs-0.5.0/socs/agents/lakeshore372/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/lakeshore372/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65222 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/lakeshore372/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.726967 socs-0.5.0/socs/agents/lakeshore425/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/lakeshore425/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9142 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/lakeshore425/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.730967 socs-0.5.0/socs/agents/magpie/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/magpie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37753 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/magpie/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.730967 socs-0.5.0/socs/agents/meinberg_m1000/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/meinberg_m1000/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17785 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/meinberg_m1000/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.730967 socs-0.5.0/socs/agents/meinberg_syncbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/meinberg_syncbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18023 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/meinberg_syncbox/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/ocs_plugin_so.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.730967 socs-0.5.0/socs/agents/pfeiffer_tc400/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/pfeiffer_tc400/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/pfeiffer_tc400/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/pfeiffer_tc400/drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.730967 socs-0.5.0/socs/agents/pfeiffer_tpg366/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/pfeiffer_tpg366/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/pfeiffer_tpg366/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.730967 socs-0.5.0/socs/agents/pysmurf_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/pysmurf_controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44402 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/pysmurf_controller/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/pysmurf_controller/smurf_subprocess_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.730967 socs-0.5.0/socs/agents/pysmurf_monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/pysmurf_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/pysmurf_monitor/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.730967 socs-0.5.0/socs/agents/scpi_psu/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/scpi_psu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/scpi_psu/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/scpi_psu/drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.730967 socs-0.5.0/socs/agents/smurf_crate_monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/smurf_crate_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11231 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/smurf_crate_monitor/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.734968 socs-0.5.0/socs/agents/smurf_file_emulator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/smurf_file_emulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27781 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/smurf_file_emulator/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105526 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/smurf_file_emulator/status_sample.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.734968 socs-0.5.0/socs/agents/smurf_stream_simulator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/smurf_stream_simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/smurf_stream_simulator/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.734968 socs-0.5.0/socs/agents/smurf_timing_card/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/smurf_timing_card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/smurf_timing_card/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.734968 socs-0.5.0/socs/agents/suprsync/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/suprsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10523 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/suprsync/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.734968 socs-0.5.0/socs/agents/synacc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/synacc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9533 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/synacc/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.734968 socs-0.5.0/socs/agents/tektronix3021c/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/tektronix3021c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/tektronix3021c/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/tektronix3021c/drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.734968 socs-0.5.0/socs/agents/thorlabs_mc2000b/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/thorlabs_mc2000b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/thorlabs_mc2000b/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.734968 socs-0.5.0/socs/agents/ucsc_radiometer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/ucsc_radiometer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/ucsc_radiometer/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.734968 socs-0.5.0/socs/agents/ups/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/ups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17838 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/ups/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.734968 socs-0.5.0/socs/agents/vantagepro2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/vantagepro2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/vantagepro2/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14819 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/vantagepro2/drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.738968 socs-0.5.0/socs/agents/wiregrid_actuator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/wiregrid_actuator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37192 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/wiregrid_actuator/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.738968 socs-0.5.0/socs/agents/wiregrid_actuator/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)    14540 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/wiregrid_actuator/drivers/Actuator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/wiregrid_actuator/drivers/DigitalIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/wiregrid_actuator/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/wiregrid_actuator/limitswitch_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/wiregrid_actuator/stopper_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.738968 socs-0.5.0/socs/agents/wiregrid_encoder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/wiregrid_encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14696 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/wiregrid_encoder/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9427 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/wiregrid_encoder/drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.738968 socs-0.5.0/socs/agents/wiregrid_kikusui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/wiregrid_kikusui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23974 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/wiregrid_kikusui/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.738968 socs-0.5.0/socs/agents/wiregrid_kikusui/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/wiregrid_kikusui/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/wiregrid_kikusui/drivers/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.738968 socs-0.5.0/socs/agents/xy_stage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/xy_stage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9856 2024-05-24 20:12:32.000000 socs-0.5.0/socs/agents/xy_stage/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.738968 socs-0.5.0/socs/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-05-24 20:12:32.000000 socs-0.5.0/socs/common/moxa_serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17459 2024-05-24 20:12:32.000000 socs-0.5.0/socs/common/pmx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-24 20:12:32.000000 socs-0.5.0/socs/common/prologix_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.738968 socs-0.5.0/socs/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25728 2024-05-24 20:12:32.000000 socs-0.5.0/socs/db/suprsync.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4832 2024-05-24 20:12:32.000000 socs-0.5.0/socs/db/suprsync_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.742967 socs-0.5.0/socs/mibs/
+-rw-r--r--   0 runner    (1001) docker     (127)    17434 2024-05-24 20:12:32.000000 socs-0.5.0/socs/mibs/IBOOTPDU-MIB.py
+-rw-r--r--   0 runner    (1001) docker     (127)   143372 2024-05-24 20:12:32.000000 socs-0.5.0/socs/mibs/MBG-SNMP-LTNG-MIB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-24 20:12:32.000000 socs-0.5.0/socs/mibs/MBG-SNMP-ROOT-MIB.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19714 2024-05-24 20:12:32.000000 socs-0.5.0/socs/mibs/MBG-SYNCBOX-N2X-MIB.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16838 2024-05-24 20:12:32.000000 socs-0.5.0/socs/mibs/SNMPv2-MIB.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38813 2024-05-24 20:12:32.000000 socs-0.5.0/socs/mibs/UPS-MIB.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/mibs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-24 20:12:32.000000 socs-0.5.0/socs/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7993 2024-05-24 20:12:32.000000 socs-0.5.0/socs/snmp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.742967 socs-0.5.0/socs/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:32.000000 socs-0.5.0/socs/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13788 2024-05-24 20:12:32.000000 socs-0.5.0/socs/testing/device_emulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-05-24 20:12:32.000000 socs-0.5.0/socs/testing/hwp_emulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-24 20:12:32.000000 socs-0.5.0/socs/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.742967 socs-0.5.0/socs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-24 20:12:44.000000 socs-0.5.0/socs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-05-24 20:12:44.000000 socs-0.5.0/socs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 20:12:44.000000 socs-0.5.0/socs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-24 20:12:44.000000 socs-0.5.0/socs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-24 20:12:44.000000 socs-0.5.0/socs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-24 20:12:44.000000 socs-0.5.0/socs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:12:44.742967 socs-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-24 20:12:32.000000 socs-0.5.0/tests/test_device_emulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-24 20:12:32.000000 socs-0.5.0/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-24 20:12:32.000000 socs-0.5.0/tests/test_snmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-24 20:12:32.000000 socs-0.5.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-05-24 20:12:32.000000 socs-0.5.0/versioneer.py
```

### Comparing `socs-0.4.5/LICENSE.txt` & `socs-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/PKG-INFO` & `socs-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: socs
-Version: 0.4.5
+Version: 0.5.0
 Summary: Simons Observatory Control System
 Home-page: https://github.com/simonsobs/socs
 Project-URL: Source Code, https://github.com/simonsobs/ocs
 Project-URL: Documentation, https://ocs.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/simonsobs/ocs/issues
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Framework :: Twisted
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
@@ -24,21 +29,21 @@
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: sqlalchemy>=1.4
 Requires-Dist: twisted
 Requires-Dist: pyasn1==0.4.8
 Provides-Extra: all
 Requires-Dist: labjack-ljm; extra == "all"
-Requires-Dist: pyepics; extra == "all"
+Requires-Dist: pixell; extra == "all"
+Requires-Dist: pandas; extra == "all"
 Requires-Dist: pfeiffer-vacuum-protocol==0.4; extra == "all"
-Requires-Dist: scipy; extra == "all"
+Requires-Dist: pyepics; extra == "all"
 Requires-Dist: numexpr; extra == "all"
 Requires-Dist: so3g; extra == "all"
-Requires-Dist: pixell; extra == "all"
-Requires-Dist: pandas; extra == "all"
+Requires-Dist: scipy; extra == "all"
 Provides-Extra: acu
 Requires-Dist: pixell; extra == "acu"
 Requires-Dist: so3g; extra == "acu"
 Provides-Extra: labjack
 Requires-Dist: labjack-ljm; extra == "labjack"
 Requires-Dist: numexpr; extra == "labjack"
 Requires-Dist: scipy; extra == "labjack"
@@ -55,35 +60,16 @@
 Provides-Extra: timing-master
 Requires-Dist: pyepics; extra == "timing-master"
 
 ========================================
 SOCS - Simons Observatory Control System
 ========================================
 
-.. image:: https://img.shields.io/github/actions/workflow/status/simonsobs/socs/develop.yml?branch=main
-    :target: https://github.com/simonsobs/socs/actions?query=workflow%3A%22Build+Test+Images%22
-    :alt: GitHub Workflow Status
-
-.. image:: https://readthedocs.org/projects/socs/badge/?version=main
-    :target: https://socs.readthedocs.io/en/main/?badge=main
-    :alt: Documentation Status
-
-.. image:: https://coveralls.io/repos/github/simonsobs/socs/badge.svg
-    :target: https://coveralls.io/github/simonsobs/socs
-
-.. image:: https://img.shields.io/badge/dockerhub-latest-blue
-    :target: https://hub.docker.com/r/simonsobs/socs
-
-.. image:: https://img.shields.io/pypi/v/socs
-   :target: https://pypi.org/project/socs/
-   :alt: PyPI Package
-
-.. image:: https://results.pre-commit.ci/badge/github/simonsobs/socs/main.svg
-   :target: https://results.pre-commit.ci/latest/github/simonsobs/socs/main
-   :alt: pre-commit.ci status
+| |pypi| |versions| |docker| |license|
+| |tests| |pre-commit| |coverage| |docs|
 
 Overview
 --------
 
 This repository, `SOCS`_, contains hardware control code for the
 Simons Observatory.  This code operates within the framework provided
 by `OCS`_.
@@ -195,7 +181,37 @@
 
 License
 --------
 This project is licensed under the BSD 2-Clause License - see the
 `LICENSE.txt`_ file for details.
 
 .. _LICENSE.txt: https://github.com/simonsobs/socs/blob/main/LICENSE.txt
+
+
+.. |coverage| image:: https://coveralls.io/repos/github/simonsobs/socs/badge.svg
+    :target: https://coveralls.io/github/simonsobs/socs
+
+.. |docker| image:: https://img.shields.io/badge/dockerhub-latest-blue
+    :target: https://hub.docker.com/r/simonsobs/socs
+
+.. |docs| image:: https://readthedocs.org/projects/socs/badge/?version=main
+    :target: https://socs.readthedocs.io/en/main/?badge=main
+    :alt: Documentation Status
+
+.. |license| image:: https://img.shields.io/pypi/l/socs
+    :target: LICENSE.txt
+    :alt: PyPI - License
+
+.. |pre-commit| image:: https://results.pre-commit.ci/badge/github/simonsobs/socs/main.svg
+   :target: https://results.pre-commit.ci/latest/github/simonsobs/socs/main
+   :alt: pre-commit.ci status
+
+.. |pypi| image:: https://img.shields.io/pypi/v/socs
+   :target: https://pypi.org/project/socs/
+   :alt: PyPI Package
+
+.. |tests| image:: https://github.com/simonsobs/socs/actions/workflows/develop.yml/badge.svg?branch=main
+    :target: https://github.com/simonsobs/socs/actions/workflows/develop.yml
+    :alt: GitHub Workflow Status
+
+.. |versions| image:: https://img.shields.io/pypi/pyversions/socs
+    :alt: PyPI - Python Version
```

### Comparing `socs-0.4.5/README.rst` & `socs-0.5.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,13 @@
 ========================================
 SOCS - Simons Observatory Control System
 ========================================
 
-.. image:: https://img.shields.io/github/actions/workflow/status/simonsobs/socs/develop.yml?branch=main
-    :target: https://github.com/simonsobs/socs/actions?query=workflow%3A%22Build+Test+Images%22
-    :alt: GitHub Workflow Status
-
-.. image:: https://readthedocs.org/projects/socs/badge/?version=main
-    :target: https://socs.readthedocs.io/en/main/?badge=main
-    :alt: Documentation Status
-
-.. image:: https://coveralls.io/repos/github/simonsobs/socs/badge.svg
-    :target: https://coveralls.io/github/simonsobs/socs
-
-.. image:: https://img.shields.io/badge/dockerhub-latest-blue
-    :target: https://hub.docker.com/r/simonsobs/socs
-
-.. image:: https://img.shields.io/pypi/v/socs
-   :target: https://pypi.org/project/socs/
-   :alt: PyPI Package
-
-.. image:: https://results.pre-commit.ci/badge/github/simonsobs/socs/main.svg
-   :target: https://results.pre-commit.ci/latest/github/simonsobs/socs/main
-   :alt: pre-commit.ci status
+| |pypi| |versions| |docker| |license|
+| |tests| |pre-commit| |coverage| |docs|
 
 Overview
 --------
 
 This repository, `SOCS`_, contains hardware control code for the
 Simons Observatory.  This code operates within the framework provided
 by `OCS`_.
@@ -138,7 +119,37 @@
 
 License
 --------
 This project is licensed under the BSD 2-Clause License - see the
 `LICENSE.txt`_ file for details.
 
 .. _LICENSE.txt: https://github.com/simonsobs/socs/blob/main/LICENSE.txt
+
+
+.. |coverage| image:: https://coveralls.io/repos/github/simonsobs/socs/badge.svg
+    :target: https://coveralls.io/github/simonsobs/socs
+
+.. |docker| image:: https://img.shields.io/badge/dockerhub-latest-blue
+    :target: https://hub.docker.com/r/simonsobs/socs
+
+.. |docs| image:: https://readthedocs.org/projects/socs/badge/?version=main
+    :target: https://socs.readthedocs.io/en/main/?badge=main
+    :alt: Documentation Status
+
+.. |license| image:: https://img.shields.io/pypi/l/socs
+    :target: LICENSE.txt
+    :alt: PyPI - License
+
+.. |pre-commit| image:: https://results.pre-commit.ci/badge/github/simonsobs/socs/main.svg
+   :target: https://results.pre-commit.ci/latest/github/simonsobs/socs/main
+   :alt: pre-commit.ci status
+
+.. |pypi| image:: https://img.shields.io/pypi/v/socs
+   :target: https://pypi.org/project/socs/
+   :alt: PyPI Package
+
+.. |tests| image:: https://github.com/simonsobs/socs/actions/workflows/develop.yml/badge.svg?branch=main
+    :target: https://github.com/simonsobs/socs/actions/workflows/develop.yml
+    :alt: GitHub Workflow Status
+
+.. |versions| image:: https://img.shields.io/pypi/pyversions/socs
+    :alt: PyPI - Python Version
```

### Comparing `socs-0.4.5/setup.py` & `socs-0.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,14 +87,19 @@
     project_urls={
         "Source Code": "https://github.com/simonsobs/ocs",
         "Documentation": "https://ocs.readthedocs.io/",
         "Bug Tracker": "https://github.com/simonsobs/ocs/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: BSD License",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Astronomy",
         "Framework :: Twisted",
     ],
     python_requires=">=3.7",
     install_requires=[
```

### Comparing `socs-0.4.5/socs/Lakeshore/Lakeshore240.py` & `socs-0.5.0/socs/Lakeshore/Lakeshore240.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/Lakeshore/Lakeshore336.py` & `socs-0.5.0/socs/Lakeshore/Lakeshore336.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/Lakeshore/Lakeshore370.py` & `socs-0.5.0/socs/Lakeshore/Lakeshore370.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/Lakeshore/Lakeshore372.py` & `socs-0.5.0/socs/Lakeshore/Lakeshore372.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/Lakeshore/Lakeshore425.py` & `socs-0.5.0/socs/Lakeshore/Lakeshore425.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/acti_camera/agent.py` & `socs-0.5.0/socs/agents/acti_camera/agent.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,24 +34,33 @@
     is_streaming : bool
         Tracks whether or not the agent is actively issuing requests to grab
         screenshots from cameras. Setting to false stops sending commands.
     log : txaio.tx.Logger
         txaio logger object, created by the OCSAgent
     """
 
-    def __init__(self, agent, camera_addresses, locations, user, password):
+    def __init__(self, agent, camera_addresses, locations, user, password, resolutions=None):
         self.agent = agent
         self.is_streaming = False
         self.log = self.agent.log
         self.lock = TimeoutLock()
 
+        # Default resolution if none provided
+        if resolutions is None:
+            resolutions = ['N640x480,100'] * len(camera_addresses)
+        else:
+            for i in range(len(camera_addresses)):
+                if len(resolutions) <= i:
+                    resolutions.append('N640x480,100')
+
         self.cameras = []
-        for (location, address) in (zip(locations, camera_addresses)):
+        for (location, address, resolution) in (zip(locations, camera_addresses, resolutions)):
             self.cameras.append({'location': location,
                                  'address': address,
+                                 'resolution': resolution,
                                  'connected': True})
         self.user = user
         self.password = password
 
         agg_params = {
             'frame_length': 10 * 60  # [sec]
         }
@@ -84,27 +93,26 @@
                          'connected': True,
                          'address': '10.10.10.41'},
              'location2': ...
             }
         """
         pm = Pacemaker(1 / 60, quantize=False)
 
-        session.set_status('running')
         self.is_streaming = True
         while self.is_streaming:
             # Use UTC
             timestamp = time.time()
             data = {}
 
             for camera in self.cameras:
                 data[camera['location']] = {'location': camera['location']}
                 self.log.info(f"Grabbing screenshot from {camera['location']}")
                 payload = {'USER': self.user,
                            'PWD': self.password,
-                           'SNAPSHOT': 'N640x480,100'}
+                           'SNAPSHOT': camera['resolution']}
                 url = f"http://{camera['address']}/cgi-bin/encoder"
 
                 # Format directory and filename
                 ctime = int(timestamp)
                 ctime_dir = int(str(timestamp)[:5])
                 Path(f"screenshots/{camera['location']}/{ctime_dir}").mkdir(parents=True, exist_ok=True)
                 filename = f"screenshots/{camera['location']}/{ctime_dir}/{ctime}.jpg"
@@ -175,14 +183,16 @@
     """
     if parser is None:
         parser = argparse.ArgumentParser()
 
     pgroup = parser.add_argument_group("Agent Options")
     pgroup.add_argument("--camera-addresses", nargs='+', type=str, help="List of camera IP addresses.")
     pgroup.add_argument("--locations", nargs='+', type=str, help="List of camera locations.")
+    pgroup.add_argument("--resolutions", nargs='+', type=str,
+                        help="List of resolution and quality. Ex: N640x480,100 where 100 is quality %.")
     pgroup.add_argument("--user", help="Username of camera.")
     pgroup.add_argument("--password", help="Password of camera.")
     pgroup.add_argument("--mode", choices=['acq', 'test'])
 
     return parser
 
 
@@ -200,14 +210,15 @@
     elif args.mode == 'test':
         init_params = False
 
     agent, runner = ocs_agent.init_site_agent(args)
     p = ACTiCameraAgent(agent,
                         camera_addresses=args.camera_addresses,
                         locations=args.locations,
+                        resolutions=args.resolutions,
                         user=args.user,
                         password=args.password)
 
     agent.register_process("acq",
                            p.acq,
                            p._stop_acq,
                            startup=init_params)
```

### Comparing `socs-0.4.5/socs/agents/acu/agent.py` & `socs-0.5.0/socs/agents/acu/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,15 +349,14 @@
         **Process** - To prevent LAT from going into Survival mode,
         do something on the command interface every so often.  (The
         default inactivity timeout is 1 minute.)
 
         """
         IDLE_RESET_TIMEOUT = 60  # The watchdog timeout in ACU
 
-        session.set_status('running')
         next_action = 0
 
         while session.status in ['starting', 'running']:
             if time.time() < next_action:
                 yield dsleep(IDLE_RESET_TIMEOUT / 10)
                 continue
             success = True
@@ -429,16 +428,14 @@
         In the case of an SATP, the Status3rdAxis is not populated
         (the Boresight info can be found in StatusDetailed).  In the
         case of the LAT, the corotator info is queried separately and
         stored under Status3rdAxis.
 
         """
 
-        session.set_status('running')
-
         # Note that session.data will get scanned, to assign data to
         # feed blocks.  We make an explicit list of items to ignore
         # during that scan (not_data_keys).
         session.data = {'PlatformType': self.acu_config['platform'],
                         'DefaultScanParams': self.scan_params,
                         'StatusResponseRate': 0.,
                         'IgnoredAxes': self.ignore_axes,
@@ -802,15 +799,14 @@
               "Az_Vel_Des": 0,
               "Az_Vffw": 0,
               "Az_Pos_Des": -20.00112176010607,
               "Az_Pos_Err": 0
             }
 
         """
-        session.set_status('running')
         FMT = self.udp_schema['format']
         FMT_LEN = struct.calcsize(FMT)
         UDP_PORT = self.udp['port']
 
         # The udp_data list is used as a queue; it contains
         # struct-unpacked samples from the UDP stream in the form
         # (time_received, data).
@@ -1000,14 +996,21 @@
           target (float): target position.
 
         Returns:
           ok (bool): True if the motion completed successfully and
             arrived at target position.
           msg (str): success/error message.
 
+        Notes:
+          This has various checks to ensure the movement executes as
+          expected and in a timely fashion.  In the case that the
+          warning horn sounds, this function should block until that
+          completes, even if the requested position has been achieved
+          (i.e. no actual motion was needed).
+
         """
         # Step time in event loop.
         TICK_TIME = 0.1
 
         # Time for which to sample distance for "still" and "moving"
         # conditions.
         PROFILE_TIME = 1.
@@ -1022,17 +1025,31 @@
 
         # How long to wait after initiation for signs of motion,
         # before giving up.  This is normally within 2 or 3 seconds
         # (SATP), but in "cold" cases where siren needs to sound, this
         # can be as long as 12 seconds.
         MAX_STARTUP_TIME = 13.
 
-        # Velocity to assume when computing maximum time a move should take (to bail
-        # out in unforeseen circumstances).
-        UNREASONABLE_VEL = 0.5
+        # How long does it take to sound the warning horn?  It takes
+        # 10 seconds.  Don't wait longer than this.
+        WARNING_HORN_TOO_LONG = 15.
+
+        # How long after mode change to Preset should we expect to see
+        # brakes released, except in case that warning horn is
+        # sounding?  3 seconds should be enough.
+        WARNING_HORN_DETECT = 3.
+
+        # Velocity to assume when computing maximum time a move should
+        # take (to bail out in unforeseen circumstances).  There are
+        # other checks in place to catch when the platform has not
+        # started moving or has stopped at the wrong place.  So the
+        # timeout computed from this should only activate in cases
+        # where some other commander has taken over and then kept the
+        # platform moving around.
+        UNREASONABLE_VEL = 0.1
 
         # Positive acknowledgment of AcuControl.go_to
         OK_RESPONSE = b'OK, Command executed.'
 
         # Enum for the motion states
         State = Enum(f'{axis}State',
                      ['INIT', 'WAIT_MOVING', 'WAIT_STILL', 'FAIL', 'DONE'])
@@ -1056,14 +1073,19 @@
 
             def get_mode(_self):
                 return self.data['status']['summary'][f'{axis}_mode']
 
             def get_vel(_self):
                 return self.data['status']['summary'][f'{axis}_current_velocity']
 
+            def get_active(_self):
+                return bool(
+                    self.data['status']['axis_state'][f'{axis}_brakes_released']
+                    and not self.data['status']['axis_state'][f'{axis}_axis_stop'])
+
         class AzAxis(AxisControl):
             @inlineCallbacks
             def goto(_self, target):
                 result = yield self.acu_control.go_to(az=target)
                 return result
 
         class ElAxis(AxisControl):
@@ -1117,14 +1139,15 @@
         state = State.INIT
         start_time = None
         motion_aborted = False
         assumption_fail = False
         motion_completed = False
         give_up_time = None
         has_never_moved = True
+        warning_horn = False
 
         while session.status in ['starting', 'running', 'stopping']:
             # Time ...
             now = time.time()
             if start_time is None:
                 start_time = now
             time_since_start = now - start_time
@@ -1132,30 +1155,32 @@
 
             # Space ...
             current_pos, current_vel = ctrl.get_pos(), ctrl.get_vel()
             distance = abs(target - current_pos)
             history.append(distance)
             if give_up_time is None:
                 give_up_time = now + distance / UNREASONABLE_VEL \
-                    + MAX_STARTUP_TIME + 2 * PROFILE_TIME
+                    + MAX_STARTUP_TIME + 2 * PROFILE_TIME \
+                    + WARNING_HORN_TOO_LONG
 
             # Do we seem to be moving / not moving?
             ok, _d = get_history(PROFILE_TIME)
             still = ok and (np.std(_d) < 0.01)
             moving = ok and (np.std(_d) >= 0.01)
             has_never_moved = (has_never_moved and not moving)
 
             near_destination = distance < THERE_YET
             mode_ok = (ctrl.get_mode() == 'Preset')
+            active_now = ctrl.get_active()
 
             # Log only on state changes
             if state != last_state:
                 _state = f'{axis}.state={state.name}'
                 self.log.info(
-                    f'{_state:<30} dt={now-start_time:7.3f} dist={distance:8.3f}')
+                    f'{_state:<30} dt={now - start_time:7.3f} dist={distance:8.3f}')
                 last_state = state
 
             # Handle task abort
             if session.status == 'stopping' and not motion_aborted:
                 target = limit_func(current_pos + current_vel * ABORT_TIME)
                 state = State.INIT
                 motion_aborted = True
@@ -1179,15 +1204,22 @@
                 history = []
                 start_time = time.time()
 
             elif state == State.WAIT_MOVING:
                 # Position and mode change requested, now wait for
                 # either mode change or clear failure of motion.
                 if mode_ok:
-                    state = state.WAIT_STILL
+                    if active_now:
+                        state = state.WAIT_STILL
+                    elif time_since_start > WARNING_HORN_TOO_LONG:
+                        self.log.error('Warning horn too long!')
+                        state = state.FAIL
+                    elif time_since_start > WARNING_HORN_DETECT and not warning_horn:
+                        warning_horn = True
+                        self.log.info('Warning horn is probably sounding.')
                 elif still and motion_expected:
                     self.log.error(f'Motion did not start within {MAX_STARTUP_TIME:.1f} s.')
                     state = state.FAIL
 
             elif state == State.WAIT_STILL:
                 # Once moving, watch for end of motion.
                 if not mode_ok:
@@ -1321,15 +1353,14 @@
                 limit_func, limits = self._get_limit_func(axis)
                 if target != limit_func(target):
                     raise ocs_agent.ParamError(
                         f'{axis}={target} not in accepted range, '
                         f'[{limits[0]}, {limits[1]}].')
 
             self.log.info(f'Requested position: az={target_az}, el={target_el}')
-            session.set_status('running')
 
             legs, msg = yield self._get_sunsafe_moves(target_az, target_el,
                                                       zero_legs_ok=False)
             if msg is not None:
                 self.log.error(msg)
                 return False, msg
 
@@ -1377,15 +1408,14 @@
                 limit_func, limits = self._get_limit_func(axis)
                 if target != limit_func(target):
                     raise ocs_agent.ParamError(
                         f'{axis}={target} not in accepted range, '
                         f'[{limits[0]}, {limits[1]}].')
 
             self.log.info(f'Commanded position: boresight={target}')
-            session.set_status('running')
 
             ok, msg = yield self._go_to_axis(session, 'Boresight', target)
 
             if ok and params['end_stop']:
                 yield self._set_modes(third='Stop')
 
         return ok, msg
@@ -1404,16 +1434,14 @@
           end_stop (bool): put axes in Stop mode after motion
 
         """
         target = self.named_positions.get(params['target'])
         if target is None:
             return False, 'Position "%s" is not configured.' % params['target']
 
-        session.set_status('running')
-
         ok, msg, _session = self.agent.start('go_to', {'az': target[0], 'el': target[1],
                                                        'end_stop': params['end_stop']})
         if ok == ocs.ERROR:
             return False, 'Failed to start go_to task.'
         ok, msg, _session = yield self.agent.wait('go_to')
         return (ok == ocs.OK), msg
 
@@ -1489,15 +1517,14 @@
     def clear_faults(self, session, params):
         """clear_faults()
 
         **Task** - Clear any axis faults.
 
         """
 
-        session.set_status('running')
         yield self.acu_control.clear_faults()
         session.set_status('stopping')
         return True, 'Job completed.'
 
     @ocs_agent.param('all_axes', default=False, type=bool)
     @inlineCallbacks
     def stop_and_clear(self, session, params):
@@ -1516,15 +1543,14 @@
                      self.data['status']['summary']['Elevation_mode']]
             if self.acu_config['platform'] == 'satp':
                 modes.append(self.data['status']['summary']['Boresight_mode'])
             elif self.acu_config['platform'] in ['ccat', 'lat']:
                 modes.append(self.data['status']['corotator']['Corotator_mode'])
             return modes
 
-        session.set_status('running')
         for i in range(6):
             for short_name, mode in zip(['az', 'el', 'third'],
                                         _read_modes()):
                 if (params['all_axes'] or short_name not in self.ignore_axes) and mode != 'Stop':
                     break
             else:
                 self.log.info('All axes in Stop mode')
@@ -1588,15 +1614,14 @@
             - 3: az_vel, in deg/s.
             - 4: el_vel, in deg/s.
             - 5: az_flags (2 if last point in a leg; 1 otherwise.)
             - 6: el_flags (2 if last point in a leg; 1 otherwise.)
 
             It is acceptable to omit columns 5 and 6.
         """
-        session.set_status('running')
 
         times, azs, els, vas, ves, azflags, elflags = sh.from_file(params['filename'])
         if min(azs) <= self.motion_limits['azimuth']['lower'] \
            or max(azs) >= self.motion_limits['azimuth']['upper']:
             return False, 'Azimuth location out of range!'
         if min(els) <= self.motion_limits['elevation']['lower'] \
            or max(els) >= self.motion_limits['elevation']['upper']:
@@ -1763,15 +1788,14 @@
             scan_params['wait_to_start'] = plan['wait_to_start']
 
         step_time = scan_params['step_time']
         point_batch_count = None
         if scan_upload_len:
             point_batch_count = scan_upload_len / step_time
 
-        session.set_status('running')
         self.log.info('The plan: {plan}', plan=plan)
         self.log.info('The scan_params: {scan_params}', scan_params=scan_params)
 
         # Before any motion, check for sun safety.
         ok, msg = self._check_scan_sunsafe(az_endpoint1, az_endpoint2, el_endpoint1,
                                            az_speed, az_accel)
         if ok:
@@ -1786,18 +1810,22 @@
         yield dsleep(1)
 
         # Verify we're good to move
         ok, msg = yield self._check_ready_motion(session)
         if not ok:
             return False, msg
 
-        # Seek to starting position
+        # Seek to starting position.  Note we ask for at least one leg
+        # here, because go_to_axes knows how to wait for the warning
+        # horn to finish before returning, which relieves us from
+        # handling that delay in the (already onerous) scan point
+        # timing.
         self.log.info(f'Moving to start position, az={plan["init_az"]}, el={init_el}')
         legs, msg = yield self._get_sunsafe_moves(plan['init_az'], init_el,
-                                                  zero_legs_ok=True)
+                                                  zero_legs_ok=False)
         if msg is not None:
             self.log.error(msg)
             return False, msg
         for leg_az, leg_el in legs:
             ok, msg = yield self._go_to_axes(session, az=leg_az, el=leg_el)
             if not ok:
                 return False, f'Start position seek failed with message: {msg}'
@@ -1837,14 +1865,17 @@
         Returns:
           Tuple (success, msg) where success is a bool.
 
         """
         # The approximate loop time
         LOOP_STEP = 0.1  # seconds
 
+        # Time to allow for initial ProgramTrack transition.
+        MAX_PROGTRACK_SET_TIME = 5.
+
         # Minimum number of points to have in the stack.  While the
         # docs strictly require 4, this number should be at least 1
         # more than that to allow for rounding when we are setting the
         # refill threshold.
         MIN_STACK_POP = 6  # points
 
         if point_batch_count is None:
@@ -1868,70 +1899,97 @@
             if not acquired:
                 return False, f"Operation failed: {self.azel_lock.job} is running."
             if session.status not in ['starting', 'running']:
                 return False, "Operation aborted before motion began."
 
             yield self.acu_control.http.Command('DataSets.CmdTimePositionTransfer',
                                                 'Clear Stack')
-            yield dsleep(0.2)
+            yield dsleep(0.5)
 
             if azonly:
                 yield self._set_modes(az='ProgramTrack')
             else:
                 yield self._set_modes(az='ProgramTrack', el='ProgramTrack')
 
-            yield dsleep(0.5)
+            yield dsleep(0.1)
 
             # Values for mode are:
             # - 'go' -- keep uploading points (unless there are no more to upload).
             # - 'stop' -- do not request more points from generator; finish the ones you have.
             # - 'abort' -- do not upload more points; exit loop and clear stack.
             mode = 'go'
 
             lines = []
             last_mode = None
             was_graceful_exit = True
+            start_time = time.time()
+            got_progtrack = False
             faults = {}
+            got_points_in = False
+            first_upload_time = None
 
             while True:
+                now = time.time()
                 current_modes = {'Az': self.data['status']['summary']['Azimuth_mode'],
                                  'El': self.data['status']['summary']['Elevation_mode'],
                                  'Remote': self.data['status']['platform_status']['Remote_mode']}
                 free_positions = self.data['status']['summary']['Free_upload_positions']
 
+                # Use this var to detect case where we're uploading
+                # points but ACU is quietly dumping them because the
+                # vel is too high.
+                got_points_in = got_points_in \
+                    or (got_progtrack and free_positions < FULL_STACK)
+
                 if last_mode != mode:
                     self.log.info(f'scan mode={mode}, line_buffer={len(lines)}, track_free={free_positions}')
                     last_mode = mode
 
                 for k in PTRACK_FAULT_KEYS:
                     if k not in faults and self.data['status']['ACU_failures_errors'].get(k):
                         self.log.info('Fault during track: "{k}"', k=k)
                         faults[k] = True
 
                 if mode != 'abort':
                     # Reasons we might decide to abort ...
-                    if current_modes['Az'] != 'ProgramTrack':
-                        self.log.warn('Unexpected mode transition!')
+                    if current_modes['Az'] == 'ProgramTrack':
+                        got_progtrack = True
+                    else:
+                        if got_progtrack:
+                            self.log.warn('Unexpected exit from ProgramTrack mode!')
+                            mode = 'abort'
+                            was_graceful_exit = False
+                        elif now - start_time > MAX_PROGTRACK_SET_TIME:
+                            self.log.warn('Failed to set ProgramTrack mode in a timely fashion.')
+                            mode = 'abort'
+                            was_graceful_exit = False
+                    if not got_points_in and (first_upload_time is not None) \
+                       and (now - first_upload_time > 10):
+                        self.log.warn('ACU seems to be dumping our track. Vel too high?')
                         mode = 'abort'
-                        was_graceful_exit = False
                     if current_modes['Remote'] == 0:
                         self.log.warn('ACU no longer in remote mode!')
                         mode = 'abort'
                         was_graceful_exit = False
                     if session.status == 'stopping':
                         mode = 'abort'
 
                 if mode == 'abort':
                     lines = []
 
                 # Is it time to upload more lines?
                 if free_positions >= STACK_REFILL_THRESHOLD:
                     new_line_target = max(int(free_positions - STACK_TARGET), 1)
 
-                    while mode == 'go' and (len(lines) < new_line_target or lines[-1][0] != 0):
+                    # Make sure that you get one more line than you
+                    # need (len(lines) > new_line_target), so that
+                    # after "grabbing the minimum batch", below, there
+                    # is still >= 1 line left.  The lines-is-empty
+                    # check is used to decide we're done.
+                    while mode == 'go' and (len(lines) <= new_line_target or lines[-1][0] != 0):
                         try:
                             lines.extend(next(point_gen))
                         except StopIteration:
                             mode = 'stop'
 
                     # Grab the minimum batch
                     upload_lines, lines = lines[:new_line_target], lines[new_line_target:]
@@ -1939,15 +1997,19 @@
                     # If the last line has a "group" flag, keep transferring lines.
                     while len(lines) and len(upload_lines) and upload_lines[-1][0] != 0:
                         upload_lines.append(lines.pop(0))
 
                     if len(upload_lines):
                         # Discard the group flag and upload all.
                         text = ''.join([line for _flag, line in upload_lines])
+                        # This seems to return b'Ok.' no matter ~what,
+                        # so not much point checking it.
                         yield self.acu_control.http.UploadPtStack(text)
+                        if first_upload_time is None:
+                            first_upload_time = time.time()
 
                 if len(lines) == 0 and free_positions >= FULL_STACK - 1:
                     break
 
                 yield dsleep(LOOP_STEP)
 
             # Go to Stop mode?
@@ -2102,15 +2164,16 @@
             "avoidance": {
               "safety_unknown": false,
               "warning_zone": false,
               "danger_zone": false,
               "escape_triggered": false,
               "escape_active": false,
               "last_escape_time": 0,
-              "sun_is_real": true
+              "sun_is_real": true,
+              "platform_is_moveable": true
             }
           }
 
         In debugging, the Sun position might be falsified.  In that
         case the "sun_pos" subtree will contain an entry like this::
 
           "WARNING": "Fake Sun Position is in use!",
@@ -2159,15 +2222,14 @@
         feed_pacer = Pacemaker(.1)
 
         req_out = False
         self.sun = None
         last_panic = 0
 
         session.data = {}
-        session.set_status('running')
 
         while session.status in ['starting', 'running']:
             new_data = {
                 'timestamp': time.time(),
             }
             new_data.update(self.sun_params)
 
@@ -2175,14 +2237,21 @@
                 az, el = [self.data['status']['summary'][f'{ax}_current_position']
                           for ax in ['Azimuth', 'Elevation']]
                 if az is None or el is None:
                     raise KeyError
             except KeyError:
                 az, el = None, None
 
+            try:
+                moveable = [bool(self.data['status']['platform_status'][k])
+                            for k in ['Safe_mode', 'Remote_mode']]
+                moveable = (not moveable[0]) and moveable[1]
+            except KeyError:
+                moveable = False
+
             no_map = self.sun is None
             old_map = (not no_map
                        and self.sun._now() - self.sun.base_time > SUN_MAP_REFRESH)
             do_recompute = (
                 not req_out
                 and (no_map or old_map or self.sun_params['recompute_req'])
             )
@@ -2198,29 +2267,28 @@
                     'map_exists': not no_map,
                     'map_is_old': old_map,
                     'map_ref_time': None if no_map else self.sun.base_time,
                     'platform_azel': (az, el),
                 },
             })
 
-            sun_is_real = True  # flags time shift during debugging.
+            # Flags for unsafe position.
+            safety_known, danger_zone, warning_zone = False, False, False
+            # Flag for time shift during debugging.
+            sun_is_real = True
             if self.sun is not None:
                 info = self.sun.get_sun_pos(az, el)
                 sun_is_real = ('WARNING' not in info)
                 new_data['sun_pos'].update(info)
                 if az is not None:
                     t = self.sun.check_trajectory([az], [el])['sun_time']
                     new_data['sun_pos']['sun_safe_time'] = t if t > 0 else 0
-
-            # Are we currently in safe position?
-            safety_known, danger_zone, warning_zone = False, False, False
-            if self.sun is not None:
-                safety_known = True
-                danger_zone = (t < self.sun_params['policy']['min_sun_time'])
-                warning_zone = (t < self.sun_params['policy']['response_time'])
+                    safety_known = True
+                    danger_zone = (t < self.sun_params['policy']['min_sun_time'])
+                    warning_zone = (t < self.sun_params['policy']['response_time'])
 
             # Has a drill been requested?
             drill_req = (self.sun_params['next_drill'] is not None
                          and self.sun_params['next_drill'] <= time.time())
 
             # Should we be doing a escape_sun_now?
             panic_for_real = safety_known and danger_zone and self._get_sun_policy('escape_enabled')
@@ -2237,21 +2305,34 @@
                 'safety_unknown': not safety_known,
                 'warning_zone': warning_zone,
                 'danger_zone': danger_zone,
                 'escape_triggered': panic_for_real,
                 'escape_active': escape_in_progress,
                 'last_escape_time': last_panic,
                 'sun_is_real': sun_is_real,
+                'platform_is_moveable': moveable,
             }
 
-            if (panic_for_real or panic_for_fun) and (time.time() - last_panic > 60.):
-                self.log.warn('monitor_sun is requesting escape_sun_now.')
+            if (panic_for_real or panic_for_fun):
+                now = time.time()
+                # Different retry conditions for moveable / not moveable
+                if moveable and (now - last_panic > 60.):
+                    # When moveable, only attempt escape every 1 minute.
+                    self.log.warn('monitor_sun is requesting escape_sun_now.')
+                    self.agent.start('escape_sun_now')
+                    last_panic = now
+                elif not moveable and (now - last_panic > 600.):
+                    # When not moveable, only print complaint message every 10 minutes.
+                    self.log.warn('monitor_sun cannot request escape_sun_now, '
+                                  'because platform not moveable by remote!')
+                    last_panic = now
+
+                # Regardless, clear the drill indicator -- we don't
+                # want that to occur randomly later.
                 self.sun_params['next_drill'] = None
-                self.agent.start('escape_sun_now')
-                last_panic = time.time()
 
             # Update session.
             session.data.update(new_data)
 
             # Publish -- only if we have the sun pos though..
             if sun_is_real and safety_known and feed_pacer.next_sample <= time.time():
                 feed_pacer.sleep()  # should be instantaneous, just update counters
@@ -2344,15 +2425,14 @@
 
         """
         state = 'init'
         last_state = state
 
         session.data = {'state': state,
                         'timestamp': time.time()}
-        session.set_status('running')
 
         while session.status in ['starting', 'running'] and state not in ['escape-done']:
             az, el = [self.data['status']['summary'][f'{ax}_current_position']
                       for ax in ['Azimuth', 'Elevation']]
 
             if state == 'init':
                 state = 'escape-abort'
@@ -2524,15 +2604,14 @@
 
         session.data = {
             'timestamp': time.time(),
             'iterations': 0,
             'attempts': 0,
             'errors': 0,
         }
-        session.set_status('running')
 
         def _publish_activity(activity):
             msg = {
                 'block_name': 'A',
                 'timestamp': time.time(),
                 'data': {'activity': activity},
             }
```

### Comparing `socs-0.4.5/socs/agents/acu/avoidance.py` & `socs-0.5.0/socs/agents/acu/avoidance.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/acu/drivers.py` & `socs-0.5.0/socs/agents/acu/drivers.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/acu/exercisor.py` & `socs-0.5.0/socs/agents/acu/exercisor.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/bluefors/agent.py` & `socs-0.5.0/socs/agents/bluefors/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -462,16 +462,14 @@
 
         """
 
         ok, msg = self.try_set_job('acq')
         if not ok:
             return ok, msg
 
-        session.set_status('running')
-
         # Create file objects for all logs in today's directory
         self.log_tracker.open_all_logs()
 
         # Determine parser configuration
         stale_time = os.environ.get("STALE_TIME", 2)
         mode = os.environ.get("MODE", "follow")
```

### Comparing `socs-0.4.5/socs/agents/cryomech_cpa/agent.py` & `socs-0.5.0/socs/agents/cryomech_cpa/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,16 +244,14 @@
 
         with self.lock.acquire_timeout(0, job='init') as acquired:
             if not acquired:
                 self.log.warn("Could not start init because "
                               "{} is already running".format(self.lock.job))
                 return False, "Could not acquire lock."
 
-            session.set_status('running')
-
             # Establish connection to ptc
             self.ptc = PTC(self.ip_address, port=self.port,
                            fake_errors=self.fake_errors)
 
             # Test connection and display identifying info
             self.ptc.get_data()
             print("PTC Model:", self.ptc.model)
@@ -283,16 +281,14 @@
         """
         with self.lock.acquire_timeout(3, job='power_ptc') as acquired:
             if not acquired:
                 self.log.warn("Could not start task because {} is already "
                               "running".format(self.lock.job))
                 return False, "Could not acquire lock."
 
-            session.set_status('running')
-
             self.ptc.power(params['state'])
 
         return True, "PTC powered {}".format(params['state'])
 
     @ocs_agent.param('test_mode', default=False, type=bool)
     def acq(self, session, params):
         """acq()
@@ -306,16 +302,14 @@
         """
         with self.lock.acquire_timeout(0, job='acq') as acquired:
             if not acquired:
                 self.log.warn("Could not start acq because {} is already"
                               "running".format(self.lock.job))
                 return False, "Could not acquire lock."
 
-            session.set_status('running')
-
             last_release = time.time()
 
             self.take_data = True
 
             while self.take_data:
                 # Relinquish sampling lock occasionally
                 if time.time() - last_release > 1.:
```

### Comparing `socs-0.4.5/socs/agents/fts_aerotech/agent.py` & `socs-0.5.0/socs/agents/fts_aerotech/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,15 +264,14 @@
             if not acquired:
                 self.log.warn(f"Could not start acq because {self.lock.job} "
                               "is already running")
                 return False, "Could not acquire lock."
 
             self.log.info("Starting Data Acquisition for FTS Mirror at"
                           f"{f_sample} Hz")
-            session.set_status('running')
             self.take_data = True
             last_release = time.time()
 
             while self.take_data:
                 if time.time() - last_release > 1.:
                     if not self.lock.release_and_acquire(timeout=20):
                         self.log.warn("Could not re-acquire lock now held by"
```

### Comparing `socs-0.4.5/socs/agents/generator/agent.py` & `socs-0.5.0/socs/agents/generator/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,16 +325,14 @@
 
         with self.lock.acquire_timeout(3, job='init') as acquired:
             if not acquired:
                 self.log.warn("Could not start init because "
                               "{} is already running".format(self.lock.job))
                 return False, "Could not acquire lock."
 
-            session.set_status('starting')
-
             self._connect()
             if not self.initialized:
                 return False, 'Could not connect to generator'
 
         # Start data acquisition if requested
         if params['auto_acquire']:
             self.agent.start('acq')
@@ -372,16 +370,14 @@
 
         with self.lock.acquire_timeout(0, job='acq') as acquired:
             if not acquired:
                 self.log.warn("Could not start acq because {} is already running"
                               .format(self.lock.job))
                 return False, "Could not acquire lock."
 
-            session.set_status('running')
-
             self.take_data = True
 
             session.data = {"fields": {}}
 
             pm = Pacemaker(self.pacemaker_freq)
             while self.take_data:
                 pm.sleep()
```

### Comparing `socs-0.4.5/socs/agents/holo_fpga/agent.py` & `socs-0.5.0/socs/agents/holo_fpga/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/holo_synth/agent.py` & `socs-0.5.0/socs/agents/holo_synth/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/hwp_encoder/agent.py` & `socs-0.5.0/socs/agents/hwp_encoder/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -524,16 +524,14 @@
 
         with self.lock.acquire_timeout(timeout=0, job='acq') as acquired:
             if not acquired:
                 self.log.warn('Could not start acq because {} is already running'
                               .format(self.lock.job))
                 return False, 'Could not acquire lock.'
 
-            session.set_status('running')
-
             self.take_data = True
 
             # Prepare data_cache for session.data
             self.hwp_freq = -1
             self.ct = time.time()
             data_cache = {
                 'approx_hwp_freq': self.hwp_freq,
```

### Comparing `socs-0.4.5/socs/agents/hwp_gripper/agent.py` & `socs-0.5.0/socs/agents/hwp_gripper/agent.py`

 * *Files 27% similar despite different names*

```diff
@@ -29,14 +29,16 @@
         self.agent = agent
         self.log = agent.log
         self.client_lock = TimeoutLock()
 
         self._initialized = False
         self.mcu_ip = args.mcu_ip
         self.control_port = args.control_port
+        self.warm_grip_distance = args.warm_grip_distance
+        self.adjustment_distance = args.adjustment_distance
 
         self.shutdown_mode = False
         self.supervisor_id = args.supervisor_id
 
         self.client: Optional[cli.GripperClient] = None
 
         agg_params = {'frame_length': 60}
@@ -166,15 +168,15 @@
             self.client.brake, params['state'], params['actuator'], job='brake'
         )
         session.data['response'] = return_dict
         return return_dict['result'], f"Success: {return_dict['result']}"
 
     @ocs_agent.param('mode', default='push', type=str, choices=['push', 'pos'])
     @ocs_agent.param('actuator', default=1, type=int, check=lambda x: 1 <= x <= 3)
-    @ocs_agent.param('distance', default=0, type=float, check=lambda x: -10. <= x <= 10.)
+    @ocs_agent.param('distance', default=0, type=float)
     def move(self, session, params=None):
         """move(mode='push', actuator=1, distance=0)
 
         **Task** - Move an actuator a specific distance. If the HWP is spinning,
         this task will not run.
 
         Parameters:
@@ -199,15 +201,15 @@
                 >>> response.session['response']
                 {'result': True,
                  'log': ["Control.STEP() operation finished for step 1",
                          "MOVE in Gripper.MOVE() completed successfully"]}
         """
 
         if self._get_hwp_freq() > 0.1:
-            self.log.warning("Not moving actuators while HWP is spinning")
+            self.log.warn("Not moving actuators while HWP is spinning")
             return False, "HWP is spinning, not moving actuators"
 
         return_dict = self._run_client_func(
             self.client.move, params['mode'], params['actuator'],
             params['distance'], job='move'
         )
         session.data['response'] = return_dict
@@ -311,22 +313,24 @@
         session.data['response'] = return_dict
         return return_dict['result'], f"Success: {return_dict['result']}"
 
     @ocs_agent.param('value', type=bool)
     def is_cold(self, session, params=None):
         """is_cold(value=False)
 
-        **Task** - Set the code to operate in warm/cold grip configuration
+        **Task** - Set the limit switches to warm/cold grip configuration
 
         Parameters:
             value (bool): Set to warm grip (False) or cold grip (True)
 
         Notes:
-            Configures the software to query the correct set of limit switches. The
-            maximum extension of the actuators depends on the cryostat temperature.
+            Configures the software to query the correct set of limit switches.
+            Warm grip configuration enables both warm and cold limit switches.
+            Cold grip configuration enables only cold limit switches. The maximum
+            extension of the actuators depends on the cryostat temperature.
 
             The most recent data collected is stored in session data in the
             structure:
 
                 >>> response.session['response']
                 {'result': True,
                  'log': ["Received request to change is_cold to True",
@@ -380,101 +384,250 @@
                       "operations from being performed")
         self.shutdown_mode = True
         return True, 'Shutdown completed'
 
     def grip(self, session, params=None):
         """grip()
 
-        **Task** - Series of commands to automatically grip the HWP.
-        This will return grippers to their home position, then move them each
-        inwards incrementally. If the HWP is spinning, this will not run.
-        """
-        if self._get_hwp_freq() > 0.1:
-            return False, "Not gripping HWP because HWP is spinning"
-
-        self._grip_hwp(session, check_shutdown=True)
-        return True, "Finished gripping procedure"
-
-    def _grip_hwp(self, session, check_shutdown=True):
-        """
-        Helper function to grip the HWP that can be called by the grip_hwp
-        task or by the shutdown procedure.  This will return grippers to their
-        home position, then move them each inwards incrementally.
-
-        Args
-        ------
-        session (OpSession):
-            Session object for current operation. This function will add to
-            session data.
+        **Task** - Series of commands to automatically warm grip the HWP. This
+        assumes that HWP is cold. This will return grippers to their home position,
+        then move them each inwards incrementally until warm limit switches are
+        tiggered. If the HWP is spinning, this will not run. If this fails to grip
+        hwp, this will return grippers to their home position.
 
         Notes:
             The most recent data collected is stored in session data in the
             structure:
 
                 >>> response.session['responses']
                 [{'result': True, 'log': [.., .., etc]},
                                     ..
                  {'result': True, 'log': [.., .., etc]}]
         """
+        if self._get_hwp_freq() > 0.1:
+            return False, "Not gripping HWP because HWP is spinning"
+
+        result, session.data = self._grip_hwp(check_shutdown=True)
+        return result, "Finished gripping procedure"
+
+    def _grip_hwp(self, check_shutdown=True):
+        """
+        Helper function to grip the HWP that can be called by the grip_hwp
+        task or by the shutdown procedure.  This will return grippers to their
+        home position, then move them each inwards incrementally.
+        """
         data = {
             'responses': [],
         }
-        session.data = data
 
         def run_and_append(func, *args, **kwargs):
             return_dict = self._run_client_func(func, *args, **kwargs)
             data['responses'].append(return_dict)
             return return_dict
 
+        # We should check if hwp is already gripper or not
+        return_dict = run_and_append(self.client.get_state, job='grip',
+                                     check_shutdown=check_shutdown)
+        act_results = return_dict['result']['actuators']
+        limit_switch_state = act_results[0]['limits']['warm_grip']['state'] | \
+            act_results[1]['limits']['warm_grip']['state'] | \
+            act_results[2]['limits']['warm_grip']['state']
+        if limit_switch_state:
+            self.log.warn("HWP is already gripped. Do nothing.")
+            return True, data
+
+        # Reset alarms
+        run_and_append(self.client.reset, job='grip', check_shutdown=check_shutdown)
+        time.sleep(1)
+
         # Enable power to actuators
         run_and_append(self.client.power, True, job='grip', check_shutdown=check_shutdown)
+        time.sleep(1)
 
+        # Disable brake
         run_and_append(self.client.brake, False, job='grip', check_shutdown=check_shutdown)
+        time.sleep(1)
+
+        # Ignore limit switches to move grippers backwards
+        run_and_append(self.client.force, True, job='grip', check_shutdown=check_shutdown)
+
+        # Ensure that the limit switches are in warm configuration
+        run_and_append(self.client.is_cold, False, job='grip', check_shutdown=check_shutdown)
 
         # Send grippers to their home position
         run_and_append(self.client.home, job='grip', check_shutdown=check_shutdown)
 
+        # Ensure that we do not ignore limit switches
+        run_and_append(self.client.force, False, job='grip', check_shutdown=check_shutdown)
+
         finished = [False, False, False]
-        for actuator, _ in enumerate(finished):
-            while not finished[actuator]:
-                # Move actuator inwards until warm-limit is hit
-                run_and_append(self.client.move, 'POS', actuator + 1, 0.2,
-                               job='grip', check_shutdown=check_shutdown)
 
-                # Reset alarms. If the warm-limit is hit, the alarm will be triggered
-                # and return_dict['result'] will be True
-                return_dict = run_and_append(self.client.reset, job='grip',
-                                             check_shutdown=check_shutdown)
+        # Move to the warm_grip_distance - 5 mm.
+        for actuator in range(3):
+            distance = self.warm_grip_distance[actuator] - 5.
+            return_dict = run_and_append(self.client.move, 'POS', actuator + 1, distance,
+                                         job='grip', check_shutdown=check_shutdown)
+            time.sleep(1)
+
+        # Move actator inwards by 0.1 mm step, warm_grip_distance + 1 is absolute maximum
+        for i in range(60):
+            if all(finished):
+                break
+            for actuator, _ in enumerate(finished):
+                if finished[actuator]:
+                    continue
+
+                # Move actuator inwards until warm-limit is hit
+                # If the warm limit is hit, return_dict['result'] will be False
+                return_dict = run_and_append(self.client.move, 'POS', actuator + 1, 0.1,
+                                             job='grip', check_shutdown=check_shutdown)
+
+                if not return_dict['result']:
+                    # Reset alarms.
+                    run_and_append(self.client.reset, job='grip',
+                                   check_shutdown=check_shutdown)
+                    time.sleep(1)
 
-                if return_dict['result']:
-                    # If the warm-limit is hit, move the actuator outwards bit
+                    # If the warm-limit is hit, move the actuator outwards by 0.5 mm
+                    # to un-trigger the warm-limit. This is because gripper sligthly
+                    # overshoot the limit switches. The outward movement compensates
+                    # for the overshoot and hysteresys of the limit switches.
                     run_and_append(self.client.is_cold, True, job='grip',
                                    check_shutdown=check_shutdown)
                     time.sleep(1)
 
                     run_and_append(self.client.move, 'POS', actuator + 1, -0.5,
                                    job='grip', check_shutdown=check_shutdown)
 
                     run_and_append(self.client.is_cold, False, job='grip',
                                    check_shutdown=check_shutdown)
                     time.sleep(1)
 
                     finished[actuator] = True
 
+        # Return grippers back to home is something is wrong
+        if not all(finished):
+            self.log.error('Failed to grip HWP. Retract grippers.')
+            run_and_append(self.client.force, True, job='grip',
+                           check_shutdown=check_shutdown)
+            time.sleep(1)
+
+            run_and_append(self.client.home, job='grip',
+                           check_shutdown=check_shutdown)
+            time.sleep(1)
+
+            run_and_append(self.client.force, False, job='grip',
+                           check_shutdown=check_shutdown)
+
+        # Adjust gripper position if you need
+        else:
+            run_and_append(self.client.is_cold, True, job='grip',
+                           check_shutdown=check_shutdown)
+            time.sleep(1)
+
+            for actuator in range(3):
+                run_and_append(self.client.move, 'POS', actuator + 1,
+                               self.adjustment_distance[actuator],
+                               job='grip', check_shutdown=check_shutdown)
+
+            run_and_append(self.client.is_cold, False, job='grip',
+                           check_shutdown=check_shutdown)
+            time.sleep(1)
+
         # Enable breaks
         run_and_append(self.client.brake, True, job='grip',
                        check_shutdown=check_shutdown)
         time.sleep(1)
 
         # Disable power to actuators
         run_and_append(self.client.power, False, job='grip',
                        check_shutdown=check_shutdown)
         time.sleep(1)
 
-        return data
+        # We should stop schedule if we have an error in this task
+        if not all(finished):
+            self.log.error('Failed to grip HWP. Grippers are retracted.')
+            return False, data
+
+        return True, data
+
+    def ungrip(self, session, params=None):
+        """ungrip()
+
+        **Task** - Series of commands to automatically ungrip the HWP.
+        This will return grippers to their home position, and retract
+        grippers as much as possible.
+
+        Notes:
+            The most recent data collected is stored in session data in the
+            structure:
+
+                >>> response.session['responses']
+                [{'result': True, 'log': [.., .., etc]},
+                                    ..
+                 {'result': True, 'log': [.., .., etc]}]
+        """
+
+        result, session.data = self._ungrip_hwp(check_shutdown=True)
+        return result, "Finished ungripping procedure"
+
+    def _ungrip_hwp(self, check_shutdown=True):
+        """
+        Helper function to ungrip the HWP that can be called by the ungrip_hwp
+        task or by the shutdown procedure.  This will return grippers to their
+        home position, and retract as much as possible.
+        """
+        data = {
+            'responses': [],
+        }
+
+        def run_and_append(func, *args, **kwargs):
+            return_dict = self._run_client_func(func, *args, **kwargs)
+            data['responses'].append(return_dict)
+            return return_dict
+
+        run_and_append(self.client.reset, job='ungrip', check_shutdown=check_shutdown)
+        # Enable power to actuators
+        run_and_append(self.client.power, True, job='ungrip', check_shutdown=check_shutdown)
+        # Disable breaks
+        run_and_append(self.client.brake, False, job='ungrip', check_shutdown=check_shutdown)
+        # Ignore limit switches
+        run_and_append(self.client.force, True, job='ungrip', check_shutdown=check_shutdown)
+
+        # Send grippers to their home position
+        run_and_append(self.client.home, job='ungrip', check_shutdown=check_shutdown)
+
+        # Move actuator outwards as much as possible
+        for actuator in range(1, 4):
+            run_and_append(self.client.move, 'POS', actuator, -1.9,
+                           job='ungrip', check_shutdown=check_shutdown)
+        time.sleep(1)
+
+        # Enable brake
+        run_and_append(self.client.brake, True, job='ungrip', check_shutdown=check_shutdown)
+        # Power off actuators
+        run_and_append(self.client.power, False, job='ungrip', check_shutdown=check_shutdown)
+        # Enable limit switches
+        run_and_append(self.client.force, False, job='ungrip', check_shutdown=check_shutdown)
+        time.sleep(1)
+
+        # check limit switch state
+        return_dict = run_and_append(self.client.get_state, job='ungrip',
+                                     check_shutdown=check_shutdown)
+        act_results = return_dict['result']['actuators']
+        limit_switch_state = act_results[0]['limits']['warm_grip']['state'] | \
+            act_results[1]['limits']['warm_grip']['state'] | \
+            act_results[2]['limits']['warm_grip']['state']
+
+        # Stop schedule if the limit switch state is wrong
+        if limit_switch_state:
+            self.log.error("Failed to ungrip HWP. Limit switch state is not as expected.")
+            return False, data
+
+        return True, data
 
     def cancel_shutdown(self, session, params=None):
         """cancel_shutdown()
 
         **Task** - Take the gripper agent out of shutdown mode
         """
         self.shutdown_mode = False
@@ -502,15 +655,14 @@
                            'jxc_out': 0,
                            'act{axis}_pos': 0,
                            'act{axis}_limit_warm_grip_state': False,
                            'act{axis}_limit_cold_grip_state': False,
                            'act{axis}_emg': False,
                            'act{axis}_brake': True}}
         """
-        session.set_status('running')
         sleep_time = 5
         while session.status in ['starting', 'running']:
             if self.client is None:
                 self.log.warn("Client not initialized")
                 time.sleep(1)
                 continue
 
@@ -588,15 +740,14 @@
             The most recent data collected is stored in session data in the
             structure:
 
                 >>> response.session
                 {'time': 1649085992.719602,
                  'gripper_action': 'ok'}
         """
-        session.set_status('running')
         last_ok_time = time.time()
 
         if self.supervisor_id is None:
             return False, 'No supervisor ID set'
 
         warning_issued = False
         while session.status in ['starting', 'running']:
@@ -612,24 +763,24 @@
             elif action == 'stop':
                 if not self.shutdown_mode:
                     self.agent.start('shutdown')
 
             time_since_ok = time.time() - last_ok_time
             if time_since_ok > params['no_data_warn_time'] and not warning_issued:
                 self.log.error(
-                    f"Have not received 'ok' in {time_since_ok/60:.2f} minutes."
+                    f"Have not received 'ok' in {time_since_ok / 60:.2f} minutes."
                     f"Will issue shutdown in "
-                    f"{params['no_data_shutdown_time']/60:.2f} minutes."
+                    f"{params['no_data_shutdown_time'] / 60:.2f} minutes."
                 )
                 warning_issued = True
 
             if time_since_ok > params['no_data_shutdown_time']:
                 self.log.error(
                     f"Have not received 'ok' in "
-                    f"{params['no_data_shutdown_time']/60:.2f} minutes. "
+                    f"{params['no_data_shutdown_time'] / 60:.2f} minutes. "
                     "Issuing shutdown"
                 )
                 self.agent.start('shutdown')
 
             data = {
                 'data': {'gripper_action': action},
                 'block_name': 'gripper_action',
@@ -655,14 +806,22 @@
         parser = argparse.ArgumentParser()
 
     pgroup = parser.add_argument_group('Agent Options')
     pgroup.add_argument('--mcu-ip', type=str,
                         help='IP of Gripper Beaglebone')
     pgroup.add_argument('--control-port', type=int, default=8041,
                         help='Port for actuator control as set by the Beaglebone code')
+    pgroup.add_argument('--warm-grip-distance', action='store', type=float, nargs=3,
+                        default=[10.0, 10.0, 10.0],
+                        help='Nominal distance for warm grip position (mm). This needs'
+                             'to be multiple of 0.1')
+    pgroup.add_argument('--adjustment-distance', action='store', type=float, nargs=3,
+                        default=[0, 0, 0],
+                        help='Adjustment distance to compensate the misalignment of '
+                             'limit switches (mm). This needs to be multiple of 0.1')
     pgroup.add_argument('--supervisor-id', type=str,
                         help='Instance ID for HWP Supervisor agent')
     pgroup.add_argument('--no-data-warn-time', type=float, default=60,
                         help='Time (seconds) since last supervisor-ok signal to '
                              'wait before issuing a warning')
     pgroup.add_argument('--no-data-shutdown-time', type=float, default=300,
                         help='Time (seconds) since last supervisor-ok signal to '
@@ -694,14 +853,15 @@
     agent.register_task('alarm', gripper_agent.alarm)
     agent.register_task('reset', gripper_agent.reset)
     agent.register_task('act', gripper_agent.act)
     agent.register_task('is_cold', gripper_agent.is_cold)
     agent.register_task('force', gripper_agent.force)
     agent.register_task('shutdown', gripper_agent.shutdown)
     agent.register_task('grip', gripper_agent.grip)
+    agent.register_task('ungrip', gripper_agent.ungrip)
     agent.register_task('cancel_shutdown', gripper_agent.cancel_shutdown)
 
     runner.run(agent, auto_reconnect=True)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `socs-0.4.5/socs/agents/hwp_gripper/drivers/gripper_client.py` & `socs-0.5.0/socs/agents/hwp_gripper/drivers/gripper_client.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/hwp_pcu/agent.py` & `socs-0.5.0/socs/agents/hwp_pcu/agent.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import time
 from dataclasses import dataclass
 from queue import Queue
 
 import txaio
-from twisted.internet import defer
+from twisted.internet import defer, reactor, threads
 
 txaio.use_twisted()
 
 from ocs import ocs_agent, site_config
 
 import socs.agents.hwp_pcu.drivers.hwp_pcu as pcu
 
@@ -23,38 +23,16 @@
     class SendCommand (BaseAction):
         command: str
 
 
 def process_action(action, PCU: pcu.PCU):
     """Process an action with PCU hardware"""
     if isinstance(action, Actions.SendCommand):
-        off_channel = []
-        on_channel = []
-        if action.command == 'off':
-            off_channel = [0, 1, 2, 5, 6, 7]
-            on_channel = []
-        elif action.command == 'on_1':
-            off_channel = [5, 6, 7]
-            on_channel = [0, 1, 2]
-        elif action.command == 'on_2':
-            on_channel = [0, 1, 2, 5, 6, 7]
-            off_channel = []
-        elif action.command == 'stop':
-            on_channel = [1, 2, 5]
-            off_channel = [0, 6, 7]
-
+        PCU.send_command(action.command)
         action.log.info(f"Command: {action.command}")
-        action.log.info(f"  Off channels: {off_channel}")
-        action.log.info(f"  On channels: {on_channel}")
-        for i in off_channel:
-            PCU.relay_off(i)
-        for i in on_channel:
-            PCU.relay_on(i)
-
-        return dict(off_channel=off_channel, on_channel=on_channel)
 
 
 class HWPPCUAgent:
     """Agent to phase compensation improve the CHWP motor efficiency
 
     Args:
         agent (ocs.ocs_agent.OCSAgent): Instantiated OCSAgent class for this agent
@@ -93,43 +71,62 @@
 
     def _process_actions(self, PCU: pcu.PCU):
         while not self.action_queue.empty():
             action = self.action_queue.get()
             try:
                 self.log.info(f"Running action {action}")
                 res = process_action(action, PCU)
-                action.deferred.callback(res)
+                reactor.callFromThread(action.deferred.callback, res)
             except Exception as e:
                 self.log.error(f"Error processing action: {action}")
-                action.deferred.errback(e)
+                reactor.callFromThread(action.deferred.errback, e)
 
     def _get_and_publish_data(self, PCU: pcu.PCU, session):
         now = time.time()
         data = {'timestamp': now,
                 'block_name': 'hwppcu',
                 'data': {}}
         status = PCU.get_status()
+
         data['data']['status'] = status
         self.agent.publish_to_feed('hwppcu', data)
         session.data = {'status': status, 'last_updated': now}
 
+        if status in ['failed', 'undefined']:
+            PCU.clear_buffer()
+            self.log.warn(f'Status is {status}, cleared buffer')
+
+    def _clear_queue(self):
+        while not self.action_queue.empty():
+            action = self.action_queue.get()
+            action.deferred.errback(Exception("Action cancelled"))
+
     def main(self, session, params):
         """
         **Process** - Main process for PCU agent.
         """
-        PCU = pcu.PCU(port=self.port)
-        self.log.info('Connected to PCU')
+        PCU = None
 
-        session.set_status('running')
-        while not self.action_queue.empty():
-            action = self.action_queue.get()
-            action.deferred.errback(Exception("Action cancelled"))
+        threads.blockingCallFromThread(reactor, self._clear_queue)
 
         last_daq = 0
         while session.status in ['starting', 'running']:
+            if PCU is None:
+                try:
+                    PCU = pcu.PCU(port=self.port)
+                    self.log.info('Connected to PCU')
+                    PCU.clear_buffer()
+                    self.log.info('Cleared buffer')
+                except ConnectionRefusedError:
+                    self.log.error(
+                        "Could not connect to PCU. "
+                        "Retrying after 30 sec..."
+                    )
+                    time.sleep(30)
+                    continue
             now = time.time()
             if now - last_daq > 5:
                 self._get_and_publish_data(PCU, session)
                 last_daq = now
 
             self._process_actions(PCU)
             time.sleep(0.1)
```

### Comparing `socs-0.4.5/socs/agents/hwp_picoscope/agent.py` & `socs-0.5.0/socs/agents/hwp_picoscope/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/hwp_picoscope/drivers/class_ps3000a.py` & `socs-0.5.0/socs/agents/hwp_picoscope/drivers/class_ps3000a.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/hwp_pid/agent.py` & `socs-0.5.0/socs/agents/lakeshore240/agent.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,387 +1,338 @@
 import argparse
+import os
 import time
+import warnings
+from typing import Optional
 
-from ocs import ocs_agent, site_config
-from ocs.ocs_twisted import TimeoutLock
-from twisted.internet import reactor
+import txaio
 
-import socs.agents.hwp_pid.drivers.pid_controller as pd
+from socs.Lakeshore.Lakeshore240 import Module
 
+on_rtd = os.environ.get('READTHEDOCS') == 'True'
+if not on_rtd:
+    from ocs import ocs_agent, site_config
+    from ocs.ocs_twisted import TimeoutLock
 
-class HWPPIDAgent:
-    """Agent to PID control the rotation speed of the CHWP
 
-    Args:
-        ip (str): IP address for the PID controller
-        port (str): Port for the PID controller
-        verbosity (str): Verbosity of PID controller output
+class LS240_Agent:
 
-    """
+    def __init__(self, agent, port="/dev/ttyUSB0", f_sample=2.5):
 
-    def __init__(self, agent, ip, port, verbosity):
-        self.agent = agent
+        self.agent: ocs_agent.OCSAgent = agent
         self.log = agent.log
         self.lock = TimeoutLock()
-        self._initialized = False
-        self.take_data = False
-        self.ip = ip
-        self.port = port
-        self._verbosity = verbosity > 0
-
-        agg_params = {'frame_length': 60}
-        self.agent.register_feed(
-            'hwppid', record=True, agg_params=agg_params)
-
-    @ocs_agent.param('auto_acquire', default=False, type=bool)
-    @ocs_agent.param('force', default=False, type=bool)
-    def init_connection(self, session, params):
-        """init_connection(auto_acquire=False, force=False)
-
-        **Task** - Initialize connection to PID
-        Controller.
-
-        Parameters:
-            auto_acquire (bool, optional): Default is False. Starts data
-                acquisition after initialization if True.
-            force (bool, optional): Force initialization, even if already
-                initialized. Defaults to False.
-
-        """
-        if self._initialized and not params['force']:
-            self.log.info("Connection already initialized. Returning...")
-            return True, "Connection already initialized"
 
-        with self.lock.acquire_timeout(10, job='init_connection') as acquired:
-            if not acquired:
-                self.log.warn(
-                    'Could not run init_connection because {} is already running'.format(self.lock.job))
-                return False, 'Could not acquire lock'
-
-            try:
-                self.pid = pd.PID(ip=self.ip, port=self.port,
-                                  verb=self._verbosity)
-                self.log.info('Connected to PID controller')
-            except BrokenPipeError:
-                self.log.error('Could not establish connection to PID controller')
-                reactor.callFromThread(reactor.stop)
-                return False, 'Unable to connect to PID controller'
-
-        self._initialized = True
-
-        # Start 'acq' Process if requested
-        if params['auto_acquire']:
-            self.agent.start('acq')
-
-        return True, 'Connection to PID controller established'
-
-    def tune_stop(self, session, params):
-        """tune_stop()
-
-        **Task** - Reverse the drive direction of the PID controller and
-        optimize the PID parameters for deceleration.
+        self.port = port
+        self.module: Optional[Module] = None
 
-        """
-        with self.lock.acquire_timeout(3, job='tune_stop') as acquired:
-            if not acquired:
-                self.log.warn(
-                    'Could not tune stop because {} is already running'.format(self.lock.job))
-                return False, 'Could not acquire lock'
+        self.f_sample = f_sample
 
-            self.pid.tune_stop()
+        self.initialized = False
+        self.take_data = False
 
-        return True, 'Reversing Direction'
+        # Registers Temperature and Voltage feeds
+        agg_params = {
+            'frame_length': 60,
+        }
+        self.agent.register_feed('temperatures',
+                                 record=True,
+                                 agg_params=agg_params,
+                                 buffer_time=1)
+
+    # Task functions.
+    def init_lakeshore(self, session, params=None):
+        """init_lakeshore(auto_acquire=False)
 
-    def tune_freq(self, session, params):
-        """tune_freq()
+        **Task** - Perform first time setup of the Lakeshore 240 Module.
 
-        **Task** - Tune the PID controller setpoint to the rotation frequency
-        and optimize the PID parameters for rotation.
+        Parameters:
+            auto_acquire (bool, optional): Starts data acquisition after
+                initialization if True. Defaults to False.
 
         """
-        with self.lock.acquire_timeout(3, job='tune_freq') as acquired:
-            if not acquired:
-                self.log.warn(
-                    'Could not tune freq because {} is already running'.format(self.lock.job))
-                return False, 'Could not acquire lock'
-
-            self.pid.tune_freq()
-
-        return True, 'Tuning to setpoint'
-
-    @ocs_agent.param('freq', default=0., check=lambda x: 0. <= x <= 3.0)
-    def declare_freq(self, session, params):
-        """declare_freq(freq=0)
+        if params is None:
+            params = {}
 
-        **Task** - Store the entered frequency as the PID setpoint when
-        ``tune_freq()`` is next called.
+        auto_acquire = params.get('auto_acquire', False)
 
-        Parameters:
-            freq (float): Desired HWP rotation frequency
+        if self.initialized:
+            return True, "Already Initialized Module"
 
-        """
-        with self.lock.acquire_timeout(3, job='declare_freq') as acquired:
+        with self.lock.acquire_timeout(0, job='init') as acquired:
             if not acquired:
-                self.log.warn(
-                    'Could not declare freq because {} is already running'.format(self.lock.job))
-                return False, 'Could not acquire lock'
-
-            self.pid.declare_freq(params['freq'])
-
-        return True, 'Setpoint at {} Hz'.format(params['freq'])
-
-    @ocs_agent.param('p', default=0.2, type=float, check=lambda x: 0. < x <= 8.)
-    @ocs_agent.param('i', default=63, type=int, check=lambda x: 0 <= x <= 200)
-    @ocs_agent.param('d', default=0., type=float, check=lambda x: 0. <= x < 10.)
-    def set_pid(self, session, params):
-        """set_pid(p=0.2, i=63, d=0.)
-
-        **Task** - Set the PID parameters. Note these changes are for the
-        current session only and will change whenever the agent container is
-        reloaded.
-
-        Parameters:
-            p (float): Proportional PID value
-            i (int): Integral PID value
-            d (float): Derivative PID value
+                self.log.warn("Could not start init because "
+                              "{} is already running".format(self.lock.job))
+                return False, "Could not acquire lock."
 
-        """
-        with self.lock.acquire_timeout(3, job='set_pid') as acquired:
-            if not acquired:
-                self.log.warn(
-                    'Could not set pid because {} is already running'.format(self.lock.job))
-                return False, 'Could not acquire lock'
+            self.module = Module(port=self.port)
+            print("Initialized Lakeshore module: {!s}".format(self.module))
+            session.add_message("Lakeshore initialized with ID: %s" % self.module.inst_sn)
 
-            self.pid.set_pid(
-                [params['p'], params['i'], params['d']])
+        self.initialized = True
 
-        return True, f"Set PID params to p: {params['p']}, i: {params['i']}, d: {params['d']}"
+        # Start data acquisition if requested
+        if auto_acquire:
+            self.agent.start('acq')
 
-    def get_freq(self, session, params):
-        """get_freq()
+        return True, 'Lakeshore module initialized.'
 
-        **Task** - Return the current HWP frequency as seen by the PID
-        controller.
+    def set_values(self, session, params=None):
+        """set_values(channel, sensor=None, auto_range=None, range=None,\
+                current_reversal=None, units=None, enabled=None, name=None)
+
+        **Task** - Set sensor parameters for a Lakeshore240 Channel.
+
+        Args:
+            channel (int):
+                Channel number to set. Valid choices are 1-8.
+            sensor (int, optional):
+                Specifies sensor type.  See
+                :func:`socs.Lakeshore.Lakeshore240.Channel.set_values` for
+                possible types.
+            auto_range (int, optional):
+                Specifies if channel should use autorange. Must be 0 or 1.
+            range (int, optional):
+                Specifies range if auto_range is false. Only settable for NTC
+                RTD.  See
+                :func:`socs.Lakeshore.Lakeshore240.Channel.set_values` for
+                possible ranges.
+            current_reversal (int, optional):
+                Specifies if input current reversal is on or off.
+                Always 0 if input is a diode.
+            units (int, optional):
+                Specifies preferred units parameter, and sets the units for
+                alarm settings.  See
+                :func:`socs.Lakeshore.Lakeshore240.Channel.set_values` for
+                possible units.
+            enabled (int, optional):
+                Sets if channel is enabled.
+            name (str, optional):
+                Sets name of channel.
+
+        """
+        if params is None:
+            params = {}
+
+        with self.lock.acquire_timeout(0, job='set_values') as acquired:
+            if not acquired:
+                self.log.warn("Could not start set_values because "
+                              "{} is already running".format(self.lock.job))
+                return False, "Could not acquire lock."
+
+            self.module.channels[params['channel'] - 1].set_values(
+                sensor=params.get('sensor'),
+                auto_range=params.get('auto_range'),
+                range=params.get('range'),
+                current_reversal=params.get('current_reversal'),
+                unit=params.get('unit'),
+                enabled=params.get('enabled'),
+                name=params.get('name'),
+            )
 
-        """
-        with self.lock.acquire_timeout(3, job='get_freq') as acquired:
-            if not acquired:
-                self.log.warn(
-                    'Could not get freq because {} is already running'.format(self.lock.job))
-                return False, 'Could not acquire lock'
-
-            freq = self.pid.get_freq()
-            session.data = {
-                'freq': freq,
-                'timestamp': time.time(),
-            }
+        return True, 'Set values for channel {}'.format(params['channel'])
 
-        return True, 'Current frequency = {}'.format(freq)
+    def upload_cal_curve(self, session, params=None):
+        """upload_cal_curve(channel, filename)
 
-    def get_target(self, session, params):
-        """get_target()
+        **Task** - Upload a calibration curve to a channel.
 
-        **Task** - Return the target HWP frequency of the PID
-        controller.
+        Parameters:
+            channel (int): Channel number, 1-8.
+            filename (str): Filename for calibration curve.
 
         """
-        with self.lock.acquire_timeout(3, job='get_target') as acquired:
-            if not acquired:
-                self.log.warn(
-                    'Could not get freq because {} is already running'.format(self.lock.job))
-                return False, 'Could not acquire lock'
-
-            freq = self.pid.get_target()
+        channel = params['channel']
+        filename = params['filename']
 
-        return True, 'Target frequency = {}'.format(freq)
-
-    def get_direction(self, session, params):
-        """get_direction()
-
-        **Task** - Return the current HWP tune direction as seen by the PID
-        controller.
-
-        """
-        with self.lock.acquire_timeout(3, job='get_direction') as acquired:
+        with self.lock.acquire_timeout(0, job='upload_cal_curve') as acquired:
             if not acquired:
-                self.log.warn(
-                    'Could not get freq because {} is already running'.format(self.lock.job))
-                return False, 'Could not acquire lock'
+                self.log.warn("Could not start set_values because "
+                              "{} is already running".format(self.lock.job))
+                return False, "Could not acquire lock."
 
-            direction = self.pid.get_direction()
-            session.data = {'direction': direction}
+            channel = self.module.channels[channel - 1]
+            self.log.info("Starting upload to channel {}...".format(channel))
+            channel.load_curve(filename)
+            self.log.info("Finished uploading.")
 
-        return True, 'Current direction = {}'.format(['Forward', 'Reverse'][direction])
+        return True, "Uploaded curve to channel {}".format(channel)
 
-    @ocs_agent.param('direction', type=str, default='0', choices=['0', '1'])
-    def set_direction(self, session, params):
-        """set_direction(direction='0')
+    def acq(self, session, params=None):
+        """acq(sampling_frequency=2.5)
 
-        **Task** - Set the HWP rotation direction.
+        **Process** - Start data acquisition.
 
         Parameters:
-            direction (str): '0' for forward and '1' for reverse.
+            sampling_frequency (float):
+                Sampling frequency for data collection. Defaults to 2.5 Hz
 
-        """
-        with self.lock.acquire_timeout(3, job='set_direction') as acquired:
-            if not acquired:
-                self.log.warn(
-                    'Could not set direction because {} is already running'.format(self.lock.job))
-                return False, 'Could not acquire lock'
 
-            self.pid.set_direction(params['direction'])
+        The most recent data collected is stored in session data in the
+        structure::
 
-        return True, 'Set direction'
+            >>> response.session['data']
+            {"fields":
+                {"Channel_1": {"T": 99.26, "V": 99.42},
+                 "Channel_2": {"T": 99.54, "V": 101.06},
+                 "Channel_3": {"T": 100.11, "V":100.79},
+                 "Channel_4": {"T": 98.49, "V": 100.77},
+                 "Channel_5": {"T": 97.75, "V": 101.45},
+                 "Channel_6": {"T": 99.58, "V": 101.75},
+                 "Channel_7": {"T": 98.03, "V": 100.82},
+                 "Channel_8": {"T": 101.14, "V":101.01}},
+             "timestamp":1601925677.6914878}
 
-    @ocs_agent.param('slope', default=1., type=float, check=lambda x: -10. < x < 10.)
-    @ocs_agent.param('offset', default=0.1, type=float, check=lambda x: -10. < x < 10.)
-    def set_scale(self, session, params):
-        """set_scale(slope=1, offset=0.1)
+        """
+        if params is None:
+            params = {}
 
-        **Task** - Set the PID's internal conversion from input voltage to
-        rotation frequency.
+        f_sample = params.get('sampling_frequency')
+        # If f_sample is None, use value passed to Agent init
+        if f_sample is None:
+            f_sample = self.f_sample
 
-        Parameters:
-            slope (float): Slope of the "rotation frequency vs input voltage"
-                relationship
-            offset (float): y-intercept of the "rotation frequency vs input
-                voltage" relationship
+        sleep_time = 1 / f_sample - 0.01
 
-        """
-        with self.lock.acquire_timeout(3, job='set_scale') as acquired:
+        with self.lock.acquire_timeout(0, job='acq') as acquired:
             if not acquired:
-                self.log.warn(
-                    'Could not set scale because {} is already running'.format(self.lock.job))
-                return False, 'Could not acquire lock'
+                self.log.warn("Could not start acq because {} is already running"
+                              .format(self.lock.job))
+                return False, "Could not acquire lock."
 
-            self.pid.set_scale(params['slope'], params['offset'])
+            self.take_data = True
 
-        return True, 'Set scale'
+            session.data = {"fields": {}}
 
-    def acq(self, session, params):
-        """acq()
+            while self.take_data:
+                current_time = time.time()
+                data = {
+                    'timestamp': current_time,
+                    'block_name': 'temps',
+                    'data': {}
+                }
 
-        **Process** - Start PID data acquisition.
+                for chan in self.module.channels:
+                    # Read sensor on channel
+                    chan_string = "Channel_{}".format(chan.channel_num)
+                    temp_reading = chan.get_reading(unit='K')
+                    sensor_reading = chan.get_reading(unit='S')
 
-        Notes:
-            The most recent data collected is stored in the session data in the
-            structure::
+                    # For data feed
+                    data['data'][chan_string + '_T'] = temp_reading
+                    data['data'][chan_string + '_V'] = sensor_reading
 
-                >>> response.session['data']
-                {'current_freq': 0,
-                 'target_freq': 0,
-                 'direction': 1,
-                 'last_updated': 1649085992.719602}
+                    # For session.data
+                    field_dict = {chan_string: {"T": temp_reading, "V": sensor_reading}}
+                    session.data['fields'].update(field_dict)
 
-        """
-        with self.lock.acquire_timeout(timeout=10, job='acq') as acquired:
-            if not acquired:
-                self.log.warn('Could not start iv acq because {} is already running'
-                              .format(self.lock.job))
-                return False, 'Could not acquire lock'
+                self.agent.publish_to_feed('temperatures', data)
 
-            session.set_status('running')
-            last_release = time.time()
-            self.take_data = True
+                session.data.update({'timestamp': current_time})
 
-            while self.take_data:
-                # Relinquish sampling lock occasionally.
-                if time.time() - last_release > 1.:
-                    last_release = time.time()
-                    if not self.lock.release_and_acquire(timeout=10):
-                        self.log.warn(f"Failed to re-acquire sampling lock, "
-                                      f"currently held by {self.lock.job}.")
-                        continue
-
-                data = {'timestamp': time.time(),
-                        'block_name': 'HWPPID', 'data': {}}
-
-                try:
-                    current_freq = self.pid.get_freq()
-                    target_freq = self.pid.get_target()
-                    direction = self.pid.get_direction()
-
-                    data['data']['current_freq'] = current_freq
-                    data['data']['target_freq'] = target_freq
-                    data['data']['direction'] = direction
-                except BaseException:
-                    time.sleep(1)
-                    continue
-
-                self.agent.publish_to_feed('hwppid', data)
-
-                session.data = {'current_freq': current_freq,
-                                'target_freq': target_freq,
-                                'direction': direction,
-                                'last_updated': time.time()}
+                time.sleep(sleep_time)
 
-                time.sleep(5)
+            self.agent.feeds['temperatures'].flush_buffer()
 
-        self.agent.feeds['hwppid'].flush_buffer()
-        return True, 'Acqusition exited cleanly'
+        return True, 'Acquisition exited cleanly.'
 
-    def _stop_acq(self, session, params):
+    def _stop_acq(self, session, params=None):
         """
-        Stop acq process.
+        Stops acq process.
         """
         if self.take_data:
             self.take_data = False
-            return True, 'requested to stop taking data'
-
-        return False, 'acq is not currently running'
+            return True, 'requested to stop taking data.'
+        else:
+            return False, 'acq is not currently running'
 
 
 def make_parser(parser=None):
-    """
-    Build the argument parser for the Agent. Allows sphinx to automatically build documentation
-    baised on this function
-    """
     if parser is None:
         parser = argparse.ArgumentParser()
 
-    # Add options specific to this agent
     pgroup = parser.add_argument_group('Agent Options')
-    pgroup.add_argument('--ip')
-    pgroup.add_argument('--port')
-    pgroup.add_argument('--verbose', '-v', action='count', default=0,
-                        help='PID Controller verbosity level.')
-    pgroup.add_argument('--mode', type=str, default='acq',
-                        choices=['init', 'acq'],
-                        help="Starting operation for the Agent.")
+    pgroup.add_argument('--serial-number', type=str,
+                        help="Serial number of your Lakeshore240 device")
+    pgroup.add_argument('--port', type=str,
+                        help="Path to USB node for the lakeshore")
+    pgroup.add_argument('--mode', type=str, choices=['idle', 'init', 'acq'],
+                        help="Starting action for the agent.")
+    pgroup.add_argument('--sampling-frequency', type=float,
+                        help="Sampling frequency for data acquisition")
+
     return parser
 
 
 def main(args=None):
+    # Start logging
+    txaio.start_logging(level=os.environ.get("LOGLEVEL", "info"))
+
     parser = make_parser()
-    args = site_config.parse_args(agent_class='HWPPIDAgent',
+
+    # Not used anymore, but we don't it to break the agent if these args are passed
+    parser.add_argument('--fake-data', help=argparse.SUPPRESS)
+    parser.add_argument('--num-channels', help=argparse.SUPPRESS)
+
+    # Interpret options in the context of site_config.
+    args = site_config.parse_args(agent_class='Lakeshore240Agent',
                                   parser=parser,
                                   args=args)
 
+    if args.fake_data is not None:
+        warnings.warn("WARNING: the --fake-data parameter is deprecated, please "
+                      "remove from your site-config file", DeprecationWarning)
+
+    if args.num_channels is not None:
+        warnings.warn("WARNING: the --num-channels parameter is deprecated, please "
+                      "remove from your site-config file", DeprecationWarning)
+
+    # Automatically acquire data if requested (default)
     init_params = False
     if args.mode == 'init':
         init_params = {'auto_acquire': False}
     elif args.mode == 'acq':
         init_params = {'auto_acquire': True}
 
+    device_port = None
+    if args.port is not None:
+        device_port = args.port
+    else:  # Tries to find correct USB port automatically
+
+        # This exists if udev rules are setup properly for the 240s
+        if os.path.exists('/dev/{}'.format(args.serial_number)):
+            device_port = "/dev/{}".format(args.serial_number)
+
+        elif os.path.exists('/dev/serial/by-id'):
+            ports = os.listdir('/dev/serial/by-id')
+            for port in ports:
+                if args.serial_number in port:
+                    device_port = "/dev/serial/by-id/{}".format(port)
+                    print("Found port {}".format(device_port))
+                    break
+
+    if device_port is None:
+        print("Could not find device port for {}".format(args.serial_number))
+        return
+
     agent, runner = ocs_agent.init_site_agent(args)
-    hwppid_agent = HWPPIDAgent(agent, ip=args.ip,
-                               port=args.port,
-                               verbosity=args.verbose)
-    agent.register_task('init_connection', hwppid_agent.init_connection,
+
+    kwargs = {
+        'port': device_port
+    }
+
+    if args.sampling_frequency is not None:
+        kwargs['f_sample'] = float(args.sampling_frequency)
+
+    therm = LS240_Agent(agent, **kwargs)
+
+    agent.register_task('init_lakeshore', therm.init_lakeshore,
                         startup=init_params)
-    agent.register_process('acq', hwppid_agent.acq,
-                           hwppid_agent._stop_acq)
-    agent.register_task('tune_stop', hwppid_agent.tune_stop)
-    agent.register_task('tune_freq', hwppid_agent.tune_freq)
-    agent.register_task('declare_freq', hwppid_agent.declare_freq)
-    agent.register_task('set_pid', hwppid_agent.set_pid)
-    agent.register_task('get_freq', hwppid_agent.get_freq)
-    agent.register_task('get_target', hwppid_agent.get_target)
-    agent.register_task('get_direction', hwppid_agent.get_direction)
-    agent.register_task('set_direction', hwppid_agent.set_direction)
-    agent.register_task('set_scale', hwppid_agent.set_scale)
+    agent.register_task('set_values', therm.set_values)
+    agent.register_task('upload_cal_curve', therm.upload_cal_curve)
+    agent.register_process('acq', therm.acq, therm._stop_acq)
 
     runner.run(agent, auto_reconnect=True)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `socs-0.4.5/socs/agents/hwp_pmx/agent.py` & `socs-0.5.0/socs/agents/hwp_pmx/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,15 @@
     def clear_alarm(self, session, params):
         """clear_alarm()
         **Task** - Clear alarm and exit protection mode.
         """
         action = Actions.ClearAlarm(**params)
         self.action_queue.put(action)
         session.data = yield action.deferred
+        self.prot = 0
         return True, 'Clear alarm'
 
     @defer.inlineCallbacks
     def use_ext(self, session, params):
         """use_ext()
         **Task** - Set the PMX Kikusui to use an external voltage control. Doing so
         enables PID control.
@@ -275,15 +276,14 @@
                 {'curr': 0,
                  'volt': 0,
                  'prot': 0,
                  'last_updated': 1649085992.719602}
 
         """
         PMX = None
-        session.set_status('running')
 
         threads.blockingCallFromThread(reactor, self._clear_queue)
 
         sleep_time = 1 / self.f_sample - 0.01
         last_daq = 0
         while session.status in ['starting', 'running']:
             if PMX is None:
@@ -380,15 +380,14 @@
         **Process** - This is a process that is constantly running to monitor the
         HWP supervisor and the recommended course of action
         course of action recommended by the HWP supervisor. If certain conditions
         are met, this will trigger a shutdown and force the power supply to
         power off.
         """
 
-        session.set_status('running')
         last_ok_time = time.time()
 
         if self.supervisor_id is None:
             return False, "No supervisor ID set"
 
         while session.status in ['starting', 'running']:
```

### Comparing `socs-0.4.5/socs/agents/hwp_pmx/drivers/PMX_ethernet.py` & `socs-0.5.0/socs/agents/hwp_pmx/drivers/PMX_ethernet.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/ibootbar/agent.py` & `socs-0.5.0/socs/agents/ibootbar/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,14 @@
              'address': '10.10.10.50'}
         """
         # Set initial default outlet names
         # Note outlets are numbered 1-8 physically on ibootbars, OIDs are numbered 0-7
         names = ['Outlet-1', 'Outlet-2', 'Outlet-3', 'Outlet-4',
                  'Outlet-5', 'Outlet-6', 'Outlet-7', 'Outlet-8']
 
-        session.set_status('running')
         self.is_streaming = True
         while self.is_streaming:
             yield dsleep(1)
             if not self.connected:
                 self.log.error('No SNMP response. Check your connection!')
                 self.log.info('Trying to reconnect.')
```

### Comparing `socs-0.4.5/socs/agents/ifm_sbn246_flowmeter/agent.py` & `socs-0.5.0/socs/agents/ifm_sbn246_flowmeter/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,24 +98,28 @@
              'fields':
                 {'flow': 42.4, 'temperature': 22.8}
             }
 
         """
         pm = Pacemaker(1, quantize=True)
         self.take_data = True
-        session.set_status('running')
 
         while self.take_data:
             pm.sleep()
 
             dp = int(self.daq_port)
             adr = "/iolinkmaster/port[{}]/iolinkdevice/pdin/getdata".format(dp)
             url = 'http://{}'.format(self.ip_address)
 
-            r = requests.post(url, json={"code": "request", "cid": -1, "adr": adr})
+            try:
+                r = requests.post(url, json={"code": "request", "cid": -1, "adr": adr})
+            except requests.exceptions.ConnectionError as e:
+                self.log.warn(f"Connection error occured: {e}")
+                continue
+
             value = r.json()['data']['value']
 
             flow_gpm, temp_f = extract(value)  # units [gallons/minute], [F]
             flow = flow_gpm * 3.785411784  # liters/minute
             flow = round(flow, 1)
             temp = (temp_f - 32) * (5 / 9)  # Celsius
             temp = round(temp, 1)
```

### Comparing `socs-0.4.5/socs/agents/labjack/agent.py` & `socs-0.5.0/socs/agents/labjack/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -242,15 +242,14 @@
 
         with self.lock.acquire_timeout(0, job='init') as acquired:
             if not acquired:
                 self.log.warn("Could not start init because "
                               "{} is already running".format(self.lock.job))
                 return False, "Could not acquire lock."
 
-            session.set_status('starting')
             # Connect with the labjack
             self.handle = ljm.openS("ANY", "ANY", self.ip_address)
             info = ljm.getHandleInfo(self.handle)
             self.log.info("\nOpened LabJack of type: %i, Connection type: %i,\n"
                           "Serial number: %i, IP address: %s, Port: %i" %
                           (info[0], info[1], info[2],
                            ljm.numberToIP(info[3]), info[4]))
@@ -310,15 +309,14 @@
 
         with self.lock.acquire_timeout(0, job='acq') as acquired:
             if not acquired:
                 self.log.warn("Could not start acq because "
                               "{} is already running".format(self.lock.job))
                 return False, "Could not acquire lock."
 
-            session.set_status('running')
             self.take_data = True
 
             # Start the data stream. Use the scan rate returned by the stream,
             # which should be the same as the input scan rate.
             try:
                 scan_rate = ljm.eStreamStart(self.handle, scans_per_read, num_chs,
                                              ch_addrs, scan_rate_input)
@@ -438,15 +436,14 @@
 
         with self.lock.acquire_timeout(0, job='acq_reg') as acquired:
             if not acquired:
                 self.log.warn("Could not start acq because "
                               "{} is already running".format(self.lock.job))
                 return False, "Could not acquire lock."
 
-            session.set_status('running')
             self.take_data = True
 
             while self.take_data:
                 data = {
                     'block_name': 'reg',
                     'data': {}
                 }
```

### Comparing `socs-0.4.5/socs/agents/labjack/cal_curves/GA10K4D25_cal_curve.txt` & `socs-0.5.0/socs/agents/labjack/cal_curves/GA10K4D25_cal_curve.txt`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/lakeshore336/agent.py` & `socs-0.5.0/socs/agents/lakeshore336/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,16 +122,14 @@
         with self._lock.acquire_timeout(job='init', timeout=0) as acquired:
             if not acquired:
                 print(
                     f"Lock could not be acquired because it is held by "
                     f"{self._lock.job}")
                 return False, 'Could not acquire lock'
 
-            session.set_status('running')
-
             # get lakeshore
             self.module = LS336(self.ip)
             session.add_message(
                 f'Lakeshore initialized with ID: {self.module.id}')
 
         self.initialized = True
 
@@ -186,16 +184,14 @@
         with self._lock.acquire_timeout(job='acq', timeout=3) as acquired:
             if not acquired:
                 print(
                     f"Lock could not be acquired because it is held by "
                     f"{self._lock.job}")
                 return False, 'Could not acquire lock'
 
-            session.set_status('running')
-
             # initialize recent temps array
             # shape is N_points x N_channels
             # N_points is 2 hour / t_sample rounded up
             # N_channels is 8 if the extra scanner is installed, 4 otherwise
             # t_sample can't be more than 2 hours
             N_channels = len(self.module.channels)
             self._recent_temps = np.full(
@@ -309,16 +305,14 @@
                                         timeout=3) as acquired:
             if not acquired:
                 print(
                     f"Lock could not be acquired because it is held by "
                     f"{self._lock.job}")
                 return False, 'Could not acquire lock'
 
-            session.set_status('running')
-
             # get heater
             heater_key = params.get('heater', '2')  # default to 50W output
             heater = self.module.heaters[heater_key]
 
             # set range
             current_range = heater.get_heater_range()
             if params['range'] == current_range:
@@ -355,16 +349,14 @@
         with self._lock.acquire_timeout(job='set_pid', timeout=3) as acquired:
             if not acquired:
                 print(
                     f"Lock could not be acquired because it is held by "
                     f"{self._lock.job}")
                 return False, 'Could not acquire lock'
 
-            session.set_status('running')
-
             # get heater
             heater_key = params.get('heater', '2')  # default to 50W output
             heater = self.module.heaters[heater_key]
 
             # set pid
             current_p, current_i, current_d = heater.get_pid()
             if (params['P'] == current_p
@@ -406,16 +398,14 @@
         with self._lock.acquire_timeout(job='set_mode', timeout=3) as acquired:
             if not acquired:
                 print(
                     f"Lock could not be acquired because it is held by "
                     f"{self._lock.job}")
                 return False, 'Could not acquire lock'
 
-            session.set_status('running')
-
             # get heater
             heater_key = params.get('heater', '2')  # default to 50W output
             heater = self.module.heaters[heater_key]
 
             # set mode
             current_mode = heater.get_mode()
             if params['mode'] == current_mode:
@@ -448,16 +438,14 @@
                                         timeout=3) as acquired:
             if not acquired:
                 print(
                     f"Lock could not be acquired because it is held by "
                     f"{self._lock.job}")
                 return False, 'Could not acquire lock'
 
-            session.set_status('running')
-
             # get heater
             heater_key = params.get('heater', '2')  # default to 50W output
             heater = self.module.heaters[heater_key]
 
             # set heater resistance
             _ = heater.get_heater_resistance_setting()
             if params['resistance'] == heater.resistance:
@@ -491,16 +479,14 @@
                                         timeout=3) as acquired:
             if not acquired:
                 print(
                     f"Lock could not be acquired because it is held by "
                     f"{self._lock.job}")
                 return False, 'Could not acquire lock'
 
-            session.set_status('running')
-
             # get heater
             heater_key = params.get('heater', '2')  # default to 50W output
             heater = self.module.heaters[heater_key]
 
             # set max current
             current_max_current = heater.get_max_current()
             if params['current'] == current_max_current:
@@ -536,16 +522,14 @@
                                         timeout=3) as acquired:
             if not acquired:
                 print(
                     f"Lock could not be acquired because it is held by "
                     f"{self._lock.job}")
                 return False, 'Could not acquire lock'
 
-            session.set_status('running')
-
             # get heater
             heater_key = params.get('heater', '2')  # default to 50W output
             heater = self.module.heaters[heater_key]
 
             # set manual out
             current_manual_out = heater.get_manual_out()
             if params['percent'] == current_manual_out:
@@ -582,16 +566,14 @@
                                         timeout=3) as acquired:
             if not acquired:
                 print(
                     f"Lock could not be acquired because it is held by "
                     f"{self._lock.job}")
                 return False, 'Could not acquire lock'
 
-            session.set_status('running')
-
             # get heater
             heater_key = params.get('heater', '2')  # default to 50W output
             heater = self.module.heaters[heater_key]
 
             # D1 is the same as D
             if params['input'] == 'D1':
                 params['input'] = 'D'
@@ -632,16 +614,14 @@
                                         timeout=3) as acquired:
             if not acquired:
                 print(
                     f"Lock could not be acquired because it is held by "
                     f"{self._lock.job}")
                 return False, 'Could not acquire lock'
 
-            session.set_status('running')
-
             # get heater
             heater_key = params.get('heater', '2')  # default to 50W output
             heater = self.module.heaters[heater_key]
 
             # set setpoint
             current_setpoint = heater.get_setpoint()
             if params['setpoint'] == current_setpoint:
@@ -684,16 +664,14 @@
                                         timeout=3) as acquired:
             if not acquired:
                 print(
                     f"Lock could not be acquired because it is held by "
                     f"{self._lock.job}")
                 return False, 'Could not acquire lock'
 
-            session.set_status('running')
-
             # get channel
             channel_key = params.get('channel', 'A')  # default to input A
             channel = self.module.channels[channel_key]
 
             # set T limit
             current_limit = channel.get_T_limit()
             if params['T_limit'] == current_limit:
@@ -763,16 +741,14 @@
                                         timeout=3) as acquired:
             if not acquired:
                 print(
                     f"Lock could not be acquired because it is held by "
                     f"{self._lock.job}")
                 return False, 'Could not acquire lock'
 
-            session.set_status('running')
-
             # get heater
             heater_key = params.get('heater', '2')  # default to 50W output
             heater = self.module.heaters[heater_key]
 
             # get current setpoint
             current_setpoint = heater.get_setpoint()
 
@@ -930,16 +906,14 @@
                                         timeout=3) as acquired:
             if not acquired:
                 print(
                     f"Lock could not be acquired because it is held by "
                     f"{self._lock.job}")
                 return False, 'Could not acquire lock'
 
-            session.set_status('running')
-
             # get heater
             heater_key = params.get('heater', '2')  # default to 50W output
             heater = self.module.heaters[heater_key]
 
             # get channel
             channel = heater.get_input_channel()
             channel_num = self.module.channels[channel].num
@@ -1001,16 +975,14 @@
                                         timeout=3) as acquired:
             if not acquired:
                 print(
                     f"Lock could not be acquired because it is held by "
                     f"{self._lock.job}")
                 return False, 'Could not acquire lock'
 
-            session.set_status('running')
-
             # get channel
             channel_key = params.get('channel', 'A')  # default to input A
             channel = self.module.channels[channel_key]
 
             # check that attribute is a valid channel method
             if getattr(channel, f"get_{params['attribute']}",
                        False) is not False:
@@ -1048,16 +1020,14 @@
                                         timeout=3) as acquired:
             if not acquired:
                 print(
                     f"Lock could not be acquired because it is held by "
                     f"{self._lock.job}")
                 return False, 'Could not acquire lock'
 
-            session.set_status('running')
-
             # get heater
             heater_key = params.get('heater', '2')  # default to 50W output
             heater = self.module.heaters[heater_key]
 
             # check that attribute is a valid heater method
             if getattr(heater, f"get_{params['attribute']}",
                        False) is not False:
```

### Comparing `socs-0.4.5/socs/agents/lakeshore370/agent.py` & `socs-0.5.0/socs/agents/lakeshore370/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,16 +145,14 @@
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
             if not acquired2:
                 self.log.warn(f"Could not start init because "
                               f"{self._acq_proc_lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             if self.fake_data:
                 self.res = random.randrange(1, 1000)
                 session.add_message("No initialization since faking data")
                 self.thermometers = ["thermA", "thermB"]
             else:
                 self.module = LS370(self.port)
                 print("Initialized Lakeshore module: {!s}".format(self.module))
@@ -186,15 +184,14 @@
                               f"{self._acq_proc_lock.job} is already running")
                 return False, "Could not acquire lock"
             if not acquired:
                 self.log.warn(f"Could not start Process because "
                               f"{self._lock.job} is holding the lock")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
             self.log.info("Starting data acquisition for {}".format(self.agent.agent_address))
             previous_channel = None
             last_release = time.time()
 
             self.take_data = True
             while self.take_data:
 
@@ -311,16 +308,14 @@
         """
         with self._lock.acquire_timeout(job='set_heater_range') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             heater_string = params.get('heater', 'sample')
             if heater_string.lower() == 'sample':
                 heater = self.module.sample_heater
             elif heater_string.lower() == 'still':  # TODO: add still heater class to driver
                 # heater = self.module.still_heater
                 self.log.warn(f"{heater_string} heater not yet implemented in this agent, please modify client")
 
@@ -350,16 +345,14 @@
         """
         with self._lock.acquire_timeout(job='set_excitation_mode') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             self.module.chan_num2channel(params['channel']).set_excitation_mode(params['mode'])
             session.add_message(f'post message in agent for Set channel {params["channel"]} excitation mode to {params["mode"]}')
             print(f'print statement in agent for Set channel {params["channel"]} excitation mode to {params["mode"]}')
 
         return True, f'return text for Set channel {params["channel"]} excitation mode to {params["mode"]}'
 
     @ocs_agent.param('channel', type=int, check=lambda x: 1 <= x <= 16)
@@ -380,16 +373,14 @@
         """
         with self._lock.acquire_timeout(job='set_excitation') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             current_excitation = self.module.chan_num2channel(params['channel']).get_excitation()
 
             if params['value'] == current_excitation:
                 print(f'Channel {params["channel"]} excitation already set to {params["value"]}')
             else:
                 self.module.chan_num2channel(params['channel']).set_excitation(params['value'])
                 session.add_message(f'Set channel {params["channel"]} excitation to {params["value"]}')
@@ -416,16 +407,14 @@
         """
         with self._lock.acquire_timeout(job='set_pid') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             self.module.sample_heater.set_pid(params["P"], params["I"], params["D"])
             session.add_message(f'post message text for Set PID to {params["P"]}, {params["I"]}, {params["D"]}')
             print(f'print text for Set PID to {params["P"]}, {params["I"]}, {params["D"]}')
 
         return True, f'return text for Set PID to {params["P"]}, {params["I"]}, {params["D"]}'
 
     @ocs_agent.param('channel', type=int)
@@ -440,16 +429,14 @@
         """
         with self._lock.acquire_timeout(job='set_active_channel') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             self.module.set_active_channel(params["channel"])
             session.add_message(f'post message text for set channel to {params["channel"]}')
             print(f'print text for set channel to {params["channel"]}')
 
         return True, f'return text for set channel to {params["channel"]}'
 
     @ocs_agent.param('autoscan', type=bool)
@@ -464,16 +451,14 @@
         """
         with self._lock.acquire_timeout(job='set_autoscan') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             if params['autoscan']:
                 self.module.enable_autoscan()
                 self.log.info('enabled autoscan')
             else:
                 self.module.disable_autoscan()
                 self.log.info('disabled autoscan')
 
@@ -494,16 +479,14 @@
         """
         with self._lock.acquire_timeout(job='servo_to_temperature') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             # Check we're in correct control mode for servo.
             if self.module.sample_heater.mode != 'Closed Loop':
                 session.add_message('Changing control to Closed Loop mode for servo.')
                 self.module.sample_heater.set_mode("Closed Loop")
 
             # Check we aren't autoscanning.
             if self.module.get_autoscan() is True:
@@ -549,16 +532,14 @@
         """
         with self._lock.acquire_timeout(job='check_temp_stability') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             setpoint = float(self.module.sample_heater.get_setpoint())
 
             if params is None:
                 params = {'measurements': 10, 'threshold': 0.5e-3}
 
             test_temps = []
 
@@ -599,16 +580,14 @@
         """
         with self._lock.acquire_timeout(job='set_output_mode') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             if params['heater'].lower() == 'still':
                 # self.module.still_heater.set_mode(params['mode']) #TODO: add still heater to driver
                 self.log.warn(f"{params['heater']} heater not yet implemented in this agent, please modify client")
             if params['heater'].lower() == 'sample':
                 self.module.sample_heater.set_mode(params['mode'])
             self.log.info("Set {} output mode to {}".format(params['heater'], params['mode']))
 
@@ -649,16 +628,14 @@
                 self.log.warn(f"{heater} heater not yet implemented in this agent, please modify client")
             if heater.lower() == 'sample':
                 self.log.info("display: {}\toutput: {}".format(display, output))
                 self.module.sample_heater.set_heater_output(output, display_type=display)
 
             self.log.info("Set {} heater display to {}, output to {}".format(heater, display, output))
 
-            session.set_status('running')
-
             data = {'timestamp': time.time(),
                     'block_name': '{}_heater_out'.format(heater),
                     'data': {'{}_heater_out'.format(heater): output}
                     }
             session.app.publish_to_feed('temperatures', data)
 
         return True, "Set {} display to {}, output to {}".format(heater, display, output)
@@ -697,16 +674,14 @@
 
         """
         with self._lock.acquire_timeout(job=f"get_{params['attribute']}", timeout=3) as acquired:
             if not acquired:
                 print(f"Lock could not be acquired because it is held by {self._lock.job}")
                 return False, 'Could not acquire lock'
 
-            session.set_status('running')
-
             # get channel
             channel_key = int(params.get('channel', 1))
             channel = self.module.chan_num2channel(channel_key)
 
             # check that attribute is a valid channel method
             if getattr(channel, f"get_{params['attribute']}", False) is not False:
                 query = getattr(channel, f"get_{params['attribute']}")
@@ -748,16 +723,14 @@
 
         """
         with self._lock.acquire_timeout(job=f"get_{params['attribute']}", timeout=3) as acquired:
             if not acquired:
                 print(f"Lock could not be acquired because it is held by {self._lock.job}")
                 return False, 'Could not acquire lock'
 
-            session.set_status('running')
-
             # get heater
             heater = self.module.sample_heater
 
             # check that attribute is a valid heater method
             if getattr(heater, f"get_{params['attribute']}", False) is not False:
                 query = getattr(heater, f"get_{params['attribute']}")
```

### Comparing `socs-0.4.5/socs/agents/lakeshore372/agent.py` & `socs-0.5.0/socs/agents/lakeshore372/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -190,16 +190,14 @@
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
             if not acquired2:
                 self.log.warn(f"Could not start init because "
                               f"{self._acq_proc_lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             if self.fake_data:
                 self.res = random.randrange(1, 1000)
                 session.add_message("No initialization since faking data")
                 self.thermometers = ["thermA", "thermB"]
             else:
                 try:
                     self.module = LS372(self.ip)
@@ -267,15 +265,14 @@
                               f"{self._acq_proc_lock.job} is already running")
                 return False, "Could not acquire lock"
             if not acquired:
                 self.log.warn(f"Could not start Process because "
                               f"{self._lock.job} is holding the lock")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
             self.log.info("Starting data acquisition for {}".format(self.agent.agent_address))
             previous_channel = None
             last_release = time.time()
 
             session.data = {"fields": {}}
 
             self.take_data = True
@@ -443,16 +440,14 @@
         """
         with self._lock.acquire_timeout(job='set_heater_range') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             heater_string = params.get('heater', 'sample')
             if heater_string.lower() == 'sample':
                 heater = self.module.sample_heater
             elif heater_string.lower() == 'still':
                 heater = self.module.still_heater
 
             current_range = heater.get_heater_range()
@@ -482,16 +477,14 @@
         """
         with self._lock.acquire_timeout(job='set_excitation_mode') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             self.module.channels[params['channel']].set_excitation_mode(params['mode'])
             session.add_message(f'post message in agent for Set channel {params["channel"]} excitation mode to {params["mode"]}')
             print(f'print statement in agent for Set channel {params["channel"]} excitation mode to {params["mode"]}')
 
         return True, f'return text for Set channel {params["channel"]} excitation mode to {params["mode"]}'
 
     @ocs_agent.param('channel', type=int, check=lambda x: 1 <= x <= 16)
@@ -512,16 +505,14 @@
         """
         with self._lock.acquire_timeout(job='set_excitation') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             current_excitation = self.module.channels[params['channel']].get_excitation()
             mode = self.module.channels[params["channel"]].get_excitation_mode()
             units = 'amps' if mode == 'current' else 'volts'
 
             if params['value'] == current_excitation:
                 session.add_message(f'Channel {params["channel"]} excitation {mode} already set to {params["value"]} {units}')
             else:
@@ -543,16 +534,14 @@
         """
         with self._lock.acquire_timeout(job='get_excitation') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             current_excitation = self.module.channels[params["channel"]].get_excitation()
             mode = self.module.channels[params["channel"]].get_excitation_mode()
             units = 'amps' if mode == 'current' else 'volts'
             session.add_message(f'Channel {params["channel"]} excitation {mode} is {current_excitation} {units}')
             session.data = {"excitation": current_excitation}
 
         return True, f'Channel {params["channel"]} excitation {mode} is {current_excitation} {units}'
@@ -578,16 +567,14 @@
         """
         with self._lock.acquire_timeout(job='set_resistance_range') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             current_resistance_range = self.module.channels[params['channel']].get_resistance_range()
 
             if params['resistance_range'] == current_resistance_range:
                 session.add_message(f'Channel {params["channel"]} resistance_range already set to {params["resistance_range"]}')
             else:
                 self.module.channels[params['channel']].set_resistance_range(params['resistance_range'])
                 session.add_message(f'Set channel {params["channel"]} resistance range to {params["resistance_range"]}')
@@ -606,16 +593,14 @@
         """
         with self._lock.acquire_timeout(job='get_resistance_range') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             current_resistance_range = self.module.channels[params['channel']].get_resistance_range()
             session.add_message(f'Channel {params["channel"]} resistance range is {current_resistance_range}')
             session.data = {"resistance_range": current_resistance_range}
 
         return True, f'Channel {params["channel"]} resistance range is {current_resistance_range}'
 
     @ocs_agent.param('channel', type=int, check=lambda x: 1 <= x <= 16)
@@ -633,16 +618,14 @@
         """
         with self._lock.acquire_timeout(job='set_dwell') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             self.module.channels[params["channel"]].set_dwell(params["dwell"])
             session.add_message(f'Set dwell to {params["dwell"]}')
 
         return True, f'Set channel {params["channel"]} dwell time to {params["dwell"]}'
 
     @ocs_agent.param('channel', type=int, check=lambda x: 1 <= x <= 16)
     def get_dwell(self, session, params):
@@ -656,16 +639,14 @@
         """
         with self._lock.acquire_timeout(job='set_dwell') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             current_dwell = self.module.channels[params["channel"]].get_dwell()
             session.add_message(f'Dwell time for channel {params["channel"]} is {current_dwell}')
             session.data = {"dwell_time": current_dwell}
 
         return True, f'Channel {params["channel"]} dwell time is {current_dwell}'
 
     @ocs_agent.param('P', type=int)
@@ -687,16 +668,14 @@
         """
         with self._lock.acquire_timeout(job='set_pid') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             self.module.sample_heater.set_pid(params["P"], params["I"], params["D"])
             session.add_message(f'post message text for Set PID to {params["P"]}, {params["I"]}, {params["D"]}')
             print(f'print text for Set PID to {params["P"]}, {params["I"]}, {params["D"]}')
 
         return True, f'return text for Set PID to {params["P"]}, {params["I"]}, {params["D"]}'
 
     @ocs_agent.param('channel', type=int)
@@ -711,16 +690,14 @@
         """
         with self._lock.acquire_timeout(job='set_active_channel') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             self.module.set_active_channel(params["channel"])
             session.add_message(f'post message text for set channel to {params["channel"]}')
             print(f'print text for set channel to {params["channel"]}')
 
         return True, f'return text for set channel to {params["channel"]}'
 
     @ocs_agent.param('autoscan', type=bool)
@@ -735,16 +712,14 @@
         """
         with self._lock.acquire_timeout(job='set_autoscan') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             if params['autoscan']:
                 self.module.enable_autoscan()
                 self.log.info('enabled autoscan')
             else:
                 self.module.disable_autoscan()
                 self.log.info('disabled autoscan')
 
@@ -762,16 +737,14 @@
         """
         with self._lock.acquire_timeout(job='servo_to_temperature') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             # Check we're in correct control mode for servo.
             if self.module.sample_heater.mode != 'Closed Loop':
                 session.add_message('Changing control to Closed Loop mode for servo.')
                 self.module.sample_heater.set_mode("Closed Loop")
 
             # Check we aren't autoscanning.
             if self.module.get_autoscan() is True:
@@ -809,16 +782,14 @@
         """
         with self._lock.acquire_timeout(job='engage_channel') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             channel = params['channel']
             state = params['state']
             if state == 'on':
                 self.module.channels[channel].enable_channel()
             else:
                 self.module.channels[channel].disable_channel()
 
@@ -837,16 +808,14 @@
         """
         with self._lock.acquire_timeout(job='engage_channel') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             channel = params['channel']
             state = params['state']
             if state == 'on':
                 self.module.channels[channel].enable_autorange()
             else:
                 self.module.channels[channel].disable_autorange()
 
@@ -867,16 +836,14 @@
         """
         with self._lock.acquire_timeout(job='set_calibration_curve') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             channel = params['channel']
             curve_number = params['curve_number']
             self.module.channels[channel].set_calibration_curve(curve_number)
 
         return True, f"Assigned channel {channel} to curve number {curve_number}."
 
     @ocs_agent.param('channel', type=int)
@@ -904,31 +871,29 @@
         """
         with self._lock.acquire_timeout(job='get_input_setup') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             channel = params['channel']
 
             ls_chann_setting = self.module.channels[channel]
             input_setup = ls_chann_setting.get_input_setup()
 
             session.data = {"mode": ls_chann_setting.mode,
                             "excitation": ls_chann_setting.excitation,
                             "excitation_units": ls_chann_setting.excitation_units,
                             "autorange": ls_chann_setting.autorange,
                             "range": ls_chann_setting.range,
                             "csshunt": ls_chann_setting.csshunt,
                             "units": ls_chann_setting.units}
 
         return True, f"Channel {channel} has measurement inputs {input_setup} = [mode," \
-                     "excitation, auto range, range, cs_shunt, units]"
+            "excitation, auto range, range, cs_shunt, units]"
 
     @ocs_agent.param('setpoint', type=float)
     @ocs_agent.param('heater', type=str)
     @ocs_agent.param('channel', type=int)
     @ocs_agent.param('P', type=float)
     @ocs_agent.param('I', type=float)
     @ocs_agent.param('update_time', type=float)
@@ -974,15 +939,14 @@
                               f"{self._acq_proc_lock.job} is already running")
                 return False, "Could not acquire lock"
             if not acquired:
                 self.log.warn(f"Could not start Process because "
                               f"{self._lock.job} is holding the lock")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
             session.data = {"fields": {}}
 
             setpoint = params['setpoint']
             heater = params['heater']
             ch = params['channel']
             P_val = params['P']
             I_val = params['I']
@@ -1124,16 +1088,14 @@
         """
         with self._lock.acquire_timeout(job='check_temp_stability') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             setpoint = float(self.module.sample_heater.get_setpoint())
 
             if params is None:
                 params = {'measurements': 10, 'threshold': 0.5e-3}
 
             test_temps = []
 
@@ -1174,16 +1136,14 @@
         """
         with self._lock.acquire_timeout(job='set_output_mode') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             if params['heater'].lower() == 'still':
                 self.module.still_heater.set_mode(params['mode'])
             if params['heater'].lower() == 'sample':
                 self.module.sample_heater.set_mode(params['mode'])
             self.log.info("Set {} output mode to {}".format(params['heater'], params['mode']))
 
         return True, "Set {} output mode to {}".format(params['heater'], params['mode'])
@@ -1227,16 +1187,14 @@
                 self.module.still_heater.set_heater_output(output, display_type=display)
             if heater.lower() == 'sample':
                 self.log.info("display: {}\toutput: {}".format(display, output))
                 self.module.sample_heater.set_heater_output(output, display_type=display)
 
             self.log.info("Set {} heater display to {}, output to {}".format(heater, display, output))
 
-            session.set_status('running')
-
             data = {'timestamp': time.time(),
                     'block_name': '{}_heater_out'.format(heater),
                     'data': {'{}_heater_out'.format(heater): output}
                     }
             session.app.publish_to_feed('temperatures', data)
 
         return True, "Set {} display to {}, output to {}".format(heater, display, output)
@@ -1262,16 +1220,14 @@
 
             output = params['output']
 
             self.module.still_heater.set_still_output(output)
 
             self.log.info("Set still output to {}".format(output))
 
-            session.set_status('running')
-
             data = {'timestamp': time.time(),
                     'block_name': 'still_heater_still_out',
                     'data': {'still_heater_still_out': output}
                     }
             session.app.publish_to_feed('temperatures', data)
 
         return True, "Set still output to {}".format(output)
@@ -1296,15 +1252,14 @@
                               f"{self._lock.job} is already running")
                 return False, "Could not acquire lock"
 
             still_output = self.module.still_heater.get_still_output()
 
             self.log.info("Current still output is {}".format(still_output))
 
-            session.set_status('running')
             session.data = {"still_heater_still_out": still_output}
 
         return True, "Current still output is {}".format(still_output)
 
     @ocs_agent.param('configfile', type=str)
     def input_configfile(self, session, params=None):
         """input_configfile(configfile)
@@ -1336,16 +1291,14 @@
 
             ls = self.module
             ls_serial = ls.id.split(',')[2]
 
             device_config = config[ls_serial]['device_settings']
             ls_chann_settings = config[ls_serial]['channel']
 
-            session.set_status('running')
-
             # enable/disable autoscan
             if device_config['autoscan'] == 'on':
                 ls.enable_autoscan()
                 self.log.info("autoscan enabled")
             elif device_config['autoscan'] == 'off':
                 ls.disable_autoscan()
                 self.log.info("autoscan disabled")
```

### Comparing `socs-0.4.5/socs/agents/lakeshore425/agent.py` & `socs-0.5.0/socs/agents/lakeshore425/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,14 @@
 
         with self.lock.acquire_timeout(0, job='init') as acquired:
             if not acquired:
                 self.log.warn("Could not start init because "
                               "{} is already running".format(self.lock.job))
                 return False, "Could not acquire lock."
 
-            session.set_status('starting')
-
             self.dev = ls.LakeShore425(self.port)
             self.log.info(self.dev.get_id())
             print("Initialized Lakeshore module: {!s}".format(self.dev))
 
         self.initialized = True
         # Start data acquisition if requested
         if auto_acquire:
@@ -115,16 +113,14 @@
 
         with self.lock.acquire_timeout(0, job='acq') as acquired:
             if not acquired:
                 self.log.warn("Could not start acq because {} is already running"
                               .format(self.lock.job))
                 return False, "Could not acquire lock."
 
-            session.set_status('running')
-
             self.take_data = True
 
             session.data = {"fields": {}}
 
             last_release = time.time()
             while self.take_data:
                 if time.time() - last_release > 1.:
```

### Comparing `socs-0.4.5/socs/agents/magpie/agent.py` & `socs-0.5.0/socs/agents/magpie/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -816,15 +816,14 @@
         location. The ``src`` param can also be a filepath or list of filepaths
         pointing to G3Files to be streamed. If a list of filenames is passed,
         once the first file is finished streaming, subsequent files will be
         streamed.
         """
 
         self._running = True
-        session.set_status('running')
 
         src_idx = 0
         if isinstance(params['src'], str):
             sources = [params['src']]
         else:
             sources = params['src']
 
@@ -946,15 +945,14 @@
         stream_start_time = None
 
         sender = core.G3NetworkSender(
             hostname='*', port=params['dest'], max_queue_size=1000
         )
 
         sender.Process(self.fp.config_frame())
-        session.set_status('running')
         while session.status in ['starting', 'running']:
             f = self.out_queue.get(block=True)
             t = f['timestamp'].time / core.G3Units.s
             now = time.time()
             if first_frame_time is None:
                 first_frame_time = t
                 stream_start_time = now
```

### Comparing `socs-0.4.5/socs/agents/meinberg_m1000/agent.py` & `socs-0.5.0/socs/agents/meinberg_m1000/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,15 +408,14 @@
             self.log.error('Either there is a network connection issue, '
                            + 'or maybe you are using the wrong SNMP '
                            + 'version. Either way, we are exiting.')
 
             reactor.callFromThread(reactor.stop)
             return False, 'acq process failed - No connection to M1000'
 
-        session.set_status('running')
         self.is_streaming = True
 
         while self.is_streaming:
             yield self.meinberg.run_snmp_get(session)
             self.log.debug("{data}", data=session.data)
             yield dsleep(1)
```

### Comparing `socs-0.4.5/socs/agents/ocs_plugin_so.py` & `socs-0.5.0/socs/agents/ocs_plugin_so.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         ('Lakeshore336Agent', 'lakeshore336/agent.py'),
         ('Lakeshore370Agent', 'lakeshore370/agent.py'),
         ('Lakeshore372Agent', 'lakeshore372/agent.py'),
         ('Lakeshore425Agent', 'lakeshore425/agent.py'),
         ('LATRtXYStageAgent', 'xy_stage/agent.py'),
         ('MagpieAgent', 'magpie/agent.py'),
         ('MeinbergM1000Agent', 'meinberg_m1000/agent.py'),
+        ('MeinbergSyncboxAgent', 'meinberg_syncbox/agent.py'),
         ('PfeifferAgent', 'pfeiffer_tpg366/agent.py'),
         ('PfeifferTC400Agent', 'pfeiffer_tc400/agent.py'),
         ('PysmurfController', 'pysmurf_controller/agent.py'),
         ('PysmurfMonitor', 'pysmurf_monitor/agent.py'),
         ('ScpiPsuAgent', 'scpi_psu/agent.py'),
         ('SmurfFileEmulator', 'smurf_file_emulator/agent.py'),
         ('SmurfStreamSimulator', 'smurf_stream_simulator/agent.py'),
```

### Comparing `socs-0.4.5/socs/agents/pfeiffer_tc400/agent.py` & `socs-0.5.0/socs/agents/pfeiffer_tc400/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/pfeiffer_tc400/drivers.py` & `socs-0.5.0/socs/agents/pfeiffer_tc400/drivers.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/pfeiffer_tpg366/agent.py` & `socs-0.5.0/socs/agents/pfeiffer_tpg366/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,16 +125,14 @@
 
         with self.lock.acquire_timeout(timeout=0, job='init') as acquired:
             # Locking mechanism stops code from proceeding if no lock acquired
             if not acquired:
                 self.log.warn("Could not start init because {} is already running".format(self.lock.job))
                 return False, "Could not acquire lock."
 
-            session.set_status('running')
-
             self.take_data = True
 
             while self.take_data:
                 data = {
                     'timestamp': time.time(),
                     'block_name': 'pressures',
                     'data': {}
```

### Comparing `socs-0.4.5/socs/agents/pysmurf_controller/agent.py` & `socs-0.5.0/socs/agents/pysmurf_controller/agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from dataclasses import asdict
+
 import matplotlib
 from autobahn.twisted.util import sleep as dsleep
 from twisted.internet import protocol, reactor, threads
 from twisted.internet.defer import Deferred, inlineCallbacks
 from twisted.logger import FileLogObserver, Logger
 from twisted.python.failure import Failure
 
@@ -15,18 +17,18 @@
 import epics
 import numpy as np
 import sodetlib as sdl
 from ocs import ocs_agent, site_config
 from ocs.ocs_agent import log_formatter
 from ocs.ocs_twisted import TimeoutLock
 from sodetlib.det_config import DetConfig
-from sodetlib.operations import (bias_dets, bias_steps, iv, uxm_relock,
-                                 uxm_setup)
+from sodetlib.operations import bias_dets
 
-NBIASLINES = 12
+from socs.agents.pysmurf_controller.smurf_subprocess_util import (
+    RunCfg, RunResult, run_smurf_func)
 
 
 class PysmurfScriptProtocol(protocol.ProcessProtocol):
     """
     The process protocol used to dispatch external Pysmurf scripts, and manage
     the stdin, stdout, and stderr pipelines.
 
@@ -73,14 +75,22 @@
         rc = status.value.exitCode
         if self.log is not None:
             self.log.info("Process ended with exit code {rc}", rc=rc)
 
         self.deferred.callback(rc)
 
 
+def set_session_data(session, result: RunResult):
+    """Sets session data based on a RunResult object"""
+    if result.return_val is not None:
+        if isinstance(result.return_val, dict):
+            session.data = result.return_val
+    session.data['result'] = asdict(result)
+
+
 class PysmurfController:
     """
     Controller object for running pysmurf scripts and functions.
 
     Args:
         agent (ocs.ocs_agent.OCSAgent):
             OCSAgent object which is running
@@ -297,15 +307,14 @@
                 'last_update':  Time that session-data was last updated,
                 'stream_id': Stream-id of the controlled smurf instance
             }
         """
         S, cfg = self._get_smurf_control(load_tune=False, no_dir=True)
         reg = sdl.Registers(S)
 
-        session.set_status('running')
         kw = {'retry_on_fail': False}
         while session.status in ['starting', 'running']:
             try:
                 d = dict(
                     channel_mask=S.get_channel_mask(**kw).tolist(),
                     downsample_factor=S.get_downsample_factor(**kw),
                     agg_time=reg.agg_time.get(**kw),
@@ -328,14 +337,34 @@
 
         return True, "Finished checking state"
 
     def _stop_check_state(self, session, params):
         """Stopper for check state process"""
         session.set_status('stopping')
 
+    def run_test_func(self, session, params):
+        """run_test_func()
+
+        **Task** - Task to test the subprocessing functionality without any
+        smurf hardware.
+        """
+        cfg = RunCfg(
+            func_name='test',
+        )
+        result = run_smurf_func(cfg)
+        if not result.success:
+            self.log.error("Subprocess errored out:\n{tb}", tb=result.traceback)
+
+        if isinstance(result.return_val, dict):
+            session.data = result.return_val
+        else:
+            session.data['data'] = result.return_val
+
+        return result.success, 'finished'
+
     @ocs_agent.param("duration", default=None, type=float)
     @ocs_agent.param('kwargs', default=None)
     @ocs_agent.param('load_tune', default=True, type=bool)
     @ocs_agent.param('stream_type', default='obs', choices=['obs', 'oper'])
     @ocs_agent.param('subtype', default=None)
     @ocs_agent.param('tag', default=None)
     @ocs_agent.param('test_mode', default=False, type=bool)
@@ -400,15 +429,14 @@
 
             stop_time = None
             if params['duration'] is not None:
                 stop_time = time.time() + params['duration']
 
             session.data['stream_id'] = cfg.stream_id
             session.data['sid'] = sdl.stream_g3_on(S, **params['kwargs'])
-            session.set_status('running')
             while session.status in ['starting', 'running']:
                 if stop_time is not None:
                     if time.time() > stop_time:
                         break
                 time.sleep(1)
 
                 if params['test_mode']:
@@ -419,16 +447,17 @@
 
     def _stream_stop(self, session, params=None):
         session.set_status('stopping')
         return True, "Requesting to end stream"
 
     @ocs_agent.param('bands', default=None)
     @ocs_agent.param('kwargs', default=None)
+    @ocs_agent.param('run_in_main_procsess', default=False)
     def uxm_setup(self, session, params):
-        """uxm_setup(bands=None, kwargs=None)
+        """uxm_setup(bands=None, kwargs=None, run_in_main_process=False)
 
         **Task** - Runs first-time setup procedure for a UXM. This will run the
         following operations:
 
             1. Setup Amps (~1 min)
             2. Estimate attens if attens are not already set in the device cfg
                (~1 min / band)
@@ -445,14 +474,17 @@
         Args
         -----
         bands : list, int
             Bands to set up. Defaults to all.
         kwargs : dict
             Dict containing additional keyword args to pass to the uxm_setup
             function.
+        run_in_main_process : bool
+            If true, run smurf-function in main process. Mainly for the purpose
+            of testing without the reactor running.
 
         Notes
         -------
         SODETLIB functions such as ``uxm_setup`` and any other functions called
         by ``uxm_setup`` will add relevant data to the ``session.data`` object
         to  a unique key. For example, if all is successful ``session.data``
         may look like::
@@ -479,31 +511,30 @@
         if params['kwargs'] is None:
             params['kwargs'] = {}
 
         with self.lock.acquire_timeout(0, job='uxm_setup') as acquired:
             if not acquired:
                 return False, f"Operation failed: {self.lock.job} is running."
 
-            S, cfg = self._get_smurf_control(session=session)
-            session.set_status('running')
-            self.log.info("Starting UXM setup")
-            success, summary = uxm_setup.uxm_setup(
-                S, cfg, bands=params['bands'], **params['kwargs']
+            cfg = RunCfg(
+                func_name='run_uxm_setup',
+                kwargs={'bands': params['bands'], 'kwargs': params['kwargs']},
+                run_in_main_process=params['run_in_main_process'],
             )
-
-            if not success:
-                final_step = session.data['timestamps'][-1][0]
-                return False, f"Failed on step {final_step}"
-            else:
-                return True, "Completed full UXM-Setup procedure"
+            result = run_smurf_func(cfg)
+            set_session_data(session, result)
+            if result.traceback is not None:
+                self.log.error("Error occurred:\n{tb}", tb=result.traceback)
+            return result.success, "Finished UXM Setup"
 
     @ocs_agent.param('bands', default=None)
     @ocs_agent.param('kwargs', default=None)
+    @ocs_agent.param('run_in_main_process', default=False, type=bool)
     def uxm_relock(self, session, params):
-        """uxm_relock(bands=None, kwargs=None)
+        """uxm_relock(bands=None, kwargs=None, run_in_main_process=False)
 
         **Task** - Relocks detectors to existing tune if setup has already been
         run. Runs the following operations:
 
             1. Setup Amps (~1 min)
             2. Relocks detectors, setup notches (if requested), and serial
                gradient descent / eta scan (~5 min / band)
@@ -518,14 +549,17 @@
         Args
         -----
         bands : list, int
             Bands to set up. Defaults to all.
         kwargs : dict
             Dict containing additional keyword args to pass to the uxm_relock
             function.
+        run_in_main_process : bool
+            If true, run smurf-function in main process. Mainly for the purpose
+            of testing without the reactor running.
 
         Notes
         -------
         SODETLIB functions such as ``uxm_relock`` and any other functions called
         will add relevant data to the ``session.data`` object to  a unique key.
         For example, if all is successful ``session.data`` may look like::
 
@@ -547,26 +581,32 @@
         if params['kwargs'] is None:
             params['kwargs'] = {}
 
         with self.lock.acquire_timeout(0, job='uxm_relock') as acquired:
             if not acquired:
                 return False, f"Operation failed: {self.lock.job} is running."
 
-            session.set_status('running')
-            S, cfg = self._get_smurf_control(session=session)
-            success, summary = uxm_relock.uxm_relock(
-                S, cfg, bands=params['bands'], **params['kwargs']
+            cfg = RunCfg(
+                func_name='run_uxm_relock',
+                kwargs={'bands': params['bands'], 'kwargs': params['kwargs']},
+                run_in_main_process=params['run_in_main_process'],
             )
-            return success, "Finished UXM Relock"
+            result = run_smurf_func(cfg)
+            set_session_data(session, result)
+            if result.traceback is not None:
+                self.log.error("Error occurred:\n{tb}", tb=result.traceback)
+
+            return result.success, "Finished UXM Setup"
 
     @ocs_agent.param('duration', default=30., type=float)
     @ocs_agent.param('kwargs', default=None)
     @ocs_agent.param('tag', default=None)
+    @ocs_agent.param('run_in_main_process', default=False, type=bool)
     def take_noise(self, session, params):
-        """take_noise(duration=30., kwargs=None, tag=None)
+        """take_noise(duration=30., kwargs=None, tag=None, run_in_main_process=False)
 
         **Task** - Takes a short timestream and calculates noise statistics.
         Median white noise level for each band will be stored in the session
         data. See the `sodetlib noise docs
         <https://simons1.princeton.edu/docs/sodetlib/noise.html>`_ for more
         information on the noise function and possible keyword arguments.
 
@@ -576,15 +616,17 @@
             Duration of timestream to take for noise calculation.
         kwargs : dict
             Dict containing additional keyword args to pass to the take_noise
             function.
         tag : string, optional
             Tag (or comma-separated list of tags) to attach to the G3 stream.
             This has precedence over the `tag` key in the kwargs dict.
-
+        run_in_main_process : bool
+            If true, run smurf-function in main process. Mainly for the purpose
+            of testing without the reactor running.
 
         Notes
         -------
         Median white noise levels for each band will be stored in the
         session.data object, for example::
 
             >> response.session['data']
@@ -600,23 +642,30 @@
         if params['tag'] is not None:
             params['kwargs']['g3_tag'] = params['tag']
 
         with self.lock.acquire_timeout(0, job='take_noise') as acquired:
             if not acquired:
                 return False, f"Operation failed: {self.lock.job} is running."
 
-            session.set_status('running')
-            S, cfg = self._get_smurf_control(session=session)
-            sdl.noise.take_noise(S, cfg, params['duration'], **params['kwargs'])
-            return True, "Finished taking noise"
+            cfg = RunCfg(
+                func_name='take_noise',
+                args=[params['duration']],
+                kwargs={'kwargs': params['kwargs']},
+                run_in_main_process=params['run_in_main_process'],
+            )
+
+            result = run_smurf_func(cfg)
+            set_session_data(session, result)
+            return result.success, "Finished taking noise"
 
     @ocs_agent.param('kwargs', default=None)
     @ocs_agent.param('tag', default=None)
+    @ocs_agent.param('run_in_main_process', default=False, type=bool)
     def take_bgmap(self, session, params):
-        """take_bgmap(kwargs=None, tag=None)
+        """take_bgmap(kwargs=None, tag=None, run_in_main_process=False)
 
         **Task** - Takes a bias-group map. This will calculate the number of
         channels assigned to each bias group and put that into the session data
         object along with the filepath to the analyzed bias-step output. See
         the `bias steps docs page <https://simons1.princeton.edu/docs/sodetlib/operations/bias_steps.html>`_
         for more information on what additional keyword arguments can be
         passed.
@@ -624,14 +673,17 @@
         Args
         ----
         kwargs : dict
             Additional kwargs to pass to take_bgmap function.
         tag : Optional[str]
             String containing a tag or comma-separated list of tags to attach
             to the g3 stream.
+        run_in_main_process : bool
+            If true, run smurf-function in main process. Mainly for the purpose
+            of testing without the reactor running.
 
         Notes
         ------
         The filepath of the BiasStepAnalysis object and the number of channels
         assigned to each bias group will be written to the session.data
         object::
 
@@ -648,37 +700,32 @@
         if params['tag'] is not None:
             params['kwargs']['g3_tag'] = params['tag']
 
         with self.lock.acquire_timeout(0, job='take_bgmap') as acquired:
             if not acquired:
                 return False, f"Operation failed: {self.lock.job} is running."
 
-            session.set_status('running')
-            S, cfg = self._get_smurf_control(session=session)
-
             kwargs = {
                 'show_plots': False,
             }
             kwargs.update(params['kwargs'])
-            bsa = bias_steps.take_bgmap(S, cfg, **kwargs)
-            nchans_per_bg = [0 for _ in range(NBIASLINES + 1)]
-            for bg in range(NBIASLINES):
-                nchans_per_bg[bg] = int(np.sum(bsa.bgmap == bg))
-            nchans_per_bg[-1] = int(np.sum(bsa.bgmap == -1))
-
-            session.data = {
-                'nchans_per_bg': nchans_per_bg,
-                'filepath': bsa.filepath,
-            }
-            return True, "Finished taking bgmap"
+            cfg = RunCfg(
+                func_name='take_bgmap',
+                kwargs={'kwargs': kwargs},
+                run_in_main_process=params['run_in_main_process'],
+            )
+            result = run_smurf_func(cfg)
+            set_session_data(session, result)
+            return result.success, "Finished taking bgmap"
 
     @ocs_agent.param('kwargs', default=None)
     @ocs_agent.param('tag', default=None)
+    @ocs_agent.param('run_in_main_process', default=False, type=bool)
     def take_iv(self, session, params):
-        """take_iv(kwargs=None, tag=None)
+        """take_iv(kwargs=None, tag=None, run_in_main_process=False)
 
         **Task** - Takes an IV. This will add the normal resistance array and
         channel info to the session data object along with the analyzed IV
         filepath. See the `sodetlib IV docs page
         <https://simons1.princeton.edu/docs/sodetlib/operations/iv.html>`_
         for more information on what additional keyword arguments can be passed
         in.
@@ -686,14 +733,17 @@
         Args
         ----
         kwargs : dict
             Additional kwargs to pass to the ``take_iv`` function.
         tag : Optional[str]
             String containing a tag or comma-separated list of tags to attach
             to the g3 stream.
+        run_in_main_process : bool
+            If true, run smurf-function in main process. Mainly for the purpose
+            of testing without the reactor running.
 
         Notes
         ------
         The following data will be written to the session.data object::
 
             >> response.session['data']
             {
@@ -709,32 +759,29 @@
 
         if params['tag'] is not None:
             params['kwargs']['g3_tag'] = params['tag']
 
         with self.lock.acquire_timeout(0, job='take_iv') as acquired:
             if not acquired:
                 return False, f"Operation failed: {self.lock.job} is running."
-
-            session.set_status('starting')
-            S, cfg = self._get_smurf_control(session=session)
-            iva = iv.take_iv(S, cfg, **params['kwargs'])
-            session.data = {
-                'bands': iva.bands.tolist(),
-                'channels': iva.channels.tolist(),
-                'bgmap': iva.bgmap.tolist(),
-                'R_n': iva.R_n.tolist(),
-                'filepath': iva.filepath,
-            }
-            return True, "Finished taking IV"
+            cfg = RunCfg(
+                func_name='take_iv',
+                kwargs={'iv_kwargs': params['kwargs']},
+                run_in_main_process=params['run_in_main_process'],
+            )
+            result = run_smurf_func(cfg)
+            set_session_data(session, result)
+            return result.success, "Finished taking IV"
 
     @ocs_agent.param('kwargs', default=None)
     @ocs_agent.param('rfrac_range', default=(0.2, 0.9))
     @ocs_agent.param('tag', default=None)
+    @ocs_agent.param('run_in_main_process', default=False, type=bool)
     def take_bias_steps(self, session, params):
-        """take_bias_steps(kwargs=None, rfrac_range=(0.2, 0.9), tag=None)
+        """take_bias_steps(kwargs=None, rfrac_range=(0.2, 0.9), tag=None, run_in_main_process=False)
 
         **Task** - Takes bias_steps and saves the output filepath to the
         session data object. See the `sodetlib bias step docs page
         <https://simons1.princeton.edu/docs/sodetlib/operations/bias_steps.html>`_
         for more information on bias steps and what kwargs can be passed in.
 
         Args
@@ -743,14 +790,17 @@
             Additional kwargs to pass to ``take_bais_steps`` function.
         rfrac_range : tuple
             Range of valid rfracs to check against when determining the number
             of good detectors.
         tag : Optional[str]
             String containing a tag or comma-separated list of tags to attach
             to the g3 stream.
+        run_in_main_process : bool
+            If true, run smurf-function in main process. Mainly for the purpose
+            of testing without the reactor running.
 
         Notes
         ------
         The following data will be written to the session.data object::
 
             >> response.session['data']
             {
@@ -774,66 +824,111 @@
         if params['tag'] is not None:
             params['kwargs']['g3_tag'] = params['tag']
 
         with self.lock.acquire_timeout(0, job='bias_steps') as acquired:
             if not acquired:
                 return False, f"Operation failed: {self.lock.job} is running."
 
-            session.set_status('starting')
-            S, cfg = self._get_smurf_control(session=session)
-            bsa = bias_steps.take_bias_steps(
-                S, cfg, **params['kwargs']
+            cfg = RunCfg(
+                func_name='take_bias_steps',
+                kwargs={
+                    'kwargs': params['kwargs'], 'rfrac_range': params['rfrac_range'],
+                },
+                run_in_main_process=params['run_in_main_process'],
             )
+            result = run_smurf_func(cfg)
+            set_session_data(session, result)
+            if result.success:  # Publish quantile results
+                for name, d in result.return_val['quantiles'].items():
+                    block = dict(zip(d['labels'], d['values']))
+                    block[f'{name}_count'] = d['count']
+                    pub_data = {
+                        'timestamp': time.time(),
+                        'block_name': f'{name}_quantile',
+                        'data': block
+                    }
+                    self.agent.publish_to_feed('bias_step_quantiles', pub_data)
 
-            biased = np.logical_and.reduce([
-                params['rfrac_range'][0] < bsa.Rfrac,
-                params['rfrac_range'][1] > bsa.Rfrac
-            ])
-            session.data = {
-                'filepath': bsa.filepath,
-                'biased_total': int(np.sum(biased)),
-                'biased_per_bg': [
-                    int(np.sum(biased[bsa.bgmap == bg])) for bg in range(12)
-                ],
-            }
-            quantiles = np.array([15, 25, 50, 75, 85])
+            return result.success, "Finished taking bias steps"
 
-            def publish_quantile_block(arr, name):
-                if np.isnan(arr).all():
-                    return None
-                labels = [f'{name}_q{q}' for q in quantiles]
-                qs = [float(np.nanquantile(arr, q / 100)) for q in quantiles]
-                block = {
-                    k: q
-                    for k, q in zip(labels, qs)
-                }
-                count = int(np.sum(~np.isnan(arr)))
-                block[f'{name}_count'] = count
+    @ocs_agent.param('bgs', default=None)
+    @ocs_agent.param('kwargs', default=None)
+    @ocs_agent.param('tag', default=None)
+    @ocs_agent.param('run_in_main_process', default=False, type=bool)
+    def take_bias_waves(self, session, params):
+        """take_bias_waves(kwargs=None, rfrac_range=(0.2, 0.9), tag=None, run_in_main_process=False)
 
-                session.data[f'{name}_quantiles'] = {
-                    name: qs,
-                    'quantiles': labels,
-                    'count': count,
-                }
+        **Task** - Takes bias_wave and saves the output filepath to the
+        session data object.
+
+        Args
+        ----
+        kwargs : dict
+            Additional kwargs to pass to ``take_bias_wave`` function.
+        rfrac_range : tuple
+            Range of valid rfracs to check against when determining the number
+            of good detectors.
+        tag : Optional[str]
+            String containing a tag or comma-separated list of tags to attach
+            to the g3 stream.
+        run_in_main_process : bool
+            If true, run smurf-function in main process. Mainly for the purpose
+            of testing without the reactor running.
 
-                d = {
-                    'timestamp': time.time(),
-                    'block_name': f'{name}_quantile',
-                    'data': block
+        Notes
+        ------
+        The following data will be written to the session.data object::
+
+            >> response.session['data']
+            {
+                'filepath': Filepath of saved BiasWaveAnalysis object
+                'biased_total': Total number of detectors biased into rfrac_range
+                'biased_per_bg': List containing number of biased detectors on each bias line
+                'Rtes_quantiles': {
+                    'Rtes': List of 15%, 25%, 50%, 75%, 85% Rtes quantiles,
+                    'quantiles': List of quantile labels
+                    'count': Total count of the distribution
                 }
+                'responsivity_quantiles': Same as above for responsivity
+                'Rfrac_quantiles': Same as above for Rfrac
+
+            }
+        """
+
+        if params['kwargs'] is None:
+            params['kwargs'] = {}
 
-                self.agent.publish_to_feed('bias_step_quantiles', d)
-                return d
+        if params['tag'] is not None:
+            params['kwargs']['g3_tag'] = params['tag']
 
-            # Resistance quantiles
-            publish_quantile_block(bsa.R0, 'Rtes')
-            publish_quantile_block(bsa.Si, 'resposnivity')
-            publish_quantile_block(bsa.Rfrac, 'Rfrac')
+        with self.lock.acquire_timeout(0, job='bias_wave') as acquired:
+            if not acquired:
+                return False, f"Operation failed: {self.lock.job} is running."
+
+            cfg = RunCfg(
+                func_name='take_bias_waves',
+                kwargs={
+                    'kwargs': params['kwargs'], 'rfrac_range': params['rfrac_range'],
+                },
+                run_in_main_process=params['run_in_main_process'],
+            )
+            result = run_smurf_func(cfg)
+            set_session_data(session, result)
+            if result.success:  # Publish quantile results
+                for name, d in result.return_val['quantiles'].items():
+                    block = dict(zip(d['labels'], d['values']))
+                    block[f'{name}_count'] = d['count']
+                    pub_data = {
+                        'timestamp': time.time(),
+                        'block_name': f'{name}_quantile',
+                        'data': block
+                    }
+                    self.agent.publish_to_feed('bias_wave_quantiles', pub_data)
 
-            return True, "Finished taking bias steps"
+            return result.success, "Finished taking bias steps"
 
     @ocs_agent.param('bgs', default=None)
     @ocs_agent.param('kwargs', default=None)
     def overbias_tes(self, session, params):
         """overbias_tes(bgs=None, kwargs=None)
 
         **Task** - Overbiases detectors using S.overbias_tes_all.
@@ -850,15 +945,14 @@
         if params['kwargs'] is not None:
             kw.update(params['kwargs'])
 
         with self.lock.acquire_timeout(0, job='overbias_tes') as acquired:
             if not acquired:
                 return False, f"Operation failed: {self.lock.job} is running."
 
-            session.set_status('running')
             S, cfg = self._get_smurf_control(session=session)
             sdl.overbias_dets(S, cfg, **kw)
 
         return True, "Finished Overbiasing TES"
 
     @ocs_agent.param('bgs', default=None)
     @ocs_agent.param('bias')
@@ -888,15 +982,14 @@
                 return False, "Number of biases must match number of bgs"
             biases = params['bias']
 
         with self.lock.acquire_timeout(0, job='set_biases') as acquired:
             if not acquired:
                 return False, f"Operation failed: {self.lock.job} is running."
 
-            session.set_status('running')
             S, _ = self._get_smurf_control(session=session)
 
             for bg, bias in zip(bgs, biases):
                 S.set_tes_bias_bipolar(bg, bias)
 
             return True, f"Finished setting biases to {params['bias']}"
 
@@ -953,15 +1046,14 @@
         if params['kwargs'] is None:
             params['kwargs'] = {}
 
         with self.lock.acquire_timeout(0, job='bias_steps') as acquired:
             if not acquired:
                 return False, f"Operation failed: {self.lock.job} is running."
 
-            session.set_status('running')
             S, cfg = self._get_smurf_control(session=session)
             if isinstance(params['rfrac'], (int, float)):
                 biases = bias_dets.bias_to_rfrac(
                     S, cfg, rfrac=params['rfrac'], **params['kwargs']
                 )
             else:
                 biases = bias_dets.bias_to_rfrac_range(
@@ -986,15 +1078,14 @@
         disable_tones: bool
             If True, will turn off RF tones and flux-ramp signal
         """
         with self.lock.acquire_timeout(0, job='all_off') as acquired:
             if not acquired:
                 return False, f"Operation failed: {self.lock.job} is running."
 
-            session.set_status('running')
             S, cfg = self._get_smurf_control(session=session)
             if params['disable_tones']:
                 S.all_off()
             if params['disable_amps']:
                 S.C.write_ps_en(0)
 
             return True, "Everything off"
@@ -1042,19 +1133,21 @@
     )
     agent.register_task('uxm_setup', controller.uxm_setup)
     agent.register_task('uxm_relock', controller.uxm_relock)
     agent.register_task('take_bgmap', controller.take_bgmap)
     agent.register_task('bias_dets', controller.bias_dets)
     agent.register_task('take_iv', controller.take_iv)
     agent.register_task('take_bias_steps', controller.take_bias_steps)
+    agent.register_task('take_bias_waves', controller.take_bias_waves)
     agent.register_task('overbias_tes', controller.overbias_tes)
     agent.register_task('take_noise', controller.take_noise)
     agent.register_task('bias_dets', controller.bias_dets)
     agent.register_task('all_off', controller.all_off)
     agent.register_task('set_biases', controller.set_biases)
     agent.register_task('zero_biases', controller.zero_biases)
+    agent.register_task('run_test_func', controller.run_test_func)
 
     runner.run(agent, auto_reconnect=True)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `socs-0.4.5/socs/agents/pysmurf_monitor/agent.py` & `socs-0.5.0/socs/agents/pysmurf_monitor/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,14 @@
                 Stop the Process loop after processing any file(s).
                 This is meant only for testing. Default is False.
 
         """
         srfm = SupRsyncFilesManager(self.db_path, create_all=True, echo=self.echo_sql)
 
         self.running = True
-        session.set_status('running')
         while self.running:
             files = []
             while not self.file_queue.empty():
                 meta = self.file_queue.get()
                 # Archive name defaults to pysmurf because that is currently
                 # the only archive. The smurf-streamer will set the
                 # archive_name to "timestreams"
```

### Comparing `socs-0.4.5/socs/agents/scpi_psu/agent.py` & `socs-0.5.0/socs/agents/scpi_psu/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,14 @@
                 [seconds].
             channels (list[int], optional): Channels to monitor. [1, 2, 3] by
                 default.
             test_mode (bool, optional): Exit process after single loop if True.
                 Defaults to False.
 
         """
-        session.set_status('running')
         self.monitor = True
 
         while self.monitor:
             with self.lock.acquire_timeout(1) as acquired:
                 if acquired:
                     data = {
                         'timestamp': time.time(),
```

### Comparing `socs-0.4.5/socs/agents/scpi_psu/drivers.py` & `socs-0.5.0/socs/agents/scpi_psu/drivers.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/smurf_crate_monitor/agent.py` & `socs-0.5.0/socs/agents/smurf_crate_monitor/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/smurf_file_emulator/agent.py` & `socs-0.5.0/socs/agents/smurf_file_emulator/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -685,15 +685,14 @@
             start_offset (float, optional):
                 If set, this will add an offset to the start time passed to the
                 `stream_between` function, allowing you to create offsets between
                 streams taken at the same time.
             tag (str, optional):
                 User tag to add to the g3 stream.
         """
-        session.set_status('starting')
 
         if self.tune is None:
             raise ValueError("No tune loaded!")
 
         # Write initial smurf metadata
         if 'duration' in params:
             action = 'take_g3_data'
@@ -710,15 +709,14 @@
         if params.get('duration') is not None:
             end_time = start_time + params['duration']
 
         tag = 'obs,cmb'
         if params.get('tag') is not None:
             tag += f',{params["tag"]}'
 
-        session.set_status('running')
         streamer = self._new_streamer(action=action, action_time=action_time, tag='obs,cmb')
         session.data['session_id'] = streamer.session_id
         session.data['g3_files'] = streamer.file_list
 
         if params['use_stream_between']:
             streamer.stream_between(start_time, end_time)
             return True, "Finished Stream"
```

### Comparing `socs-0.4.5/socs/agents/smurf_file_emulator/status_sample.yaml` & `socs-0.5.0/socs/agents/smurf_file_emulator/status_sample.yaml`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/smurf_stream_simulator/agent.py` & `socs-0.5.0/socs/agents/smurf_stream_simulator/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/smurf_timing_card/agent.py` & `socs-0.5.0/socs/agents/smurf_timing_card/agent.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,15 +51,14 @@
                     'COUNTTXCLK': 1461994265,
                     'DELTATXCLK': 15416942,
                     'RATETXCLK': 123.33553599999999,
                     'timestamp': 1678983237.832111}
 
         """
         pacemaker = Pacemaker(1. / self.sleep_time)
-        session.set_status('running')
         while session.status in ['starting', 'running']:
             data = {}
             for name, pv in self.pvs.items():
                 res = pv.get(timeout=self.timeout, use_monitor=self.use_monitor)
                 if res is None:
                     self.log.error("Timeout for PV: {name}", name=name)
                     break
```

### Comparing `socs-0.4.5/socs/agents/suprsync/agent.py` & `socs-0.5.0/socs/agents/suprsync/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,14 @@
             srfm, self.archive_name, self.remote_basedir, ssh_host=self.ssh_host,
             ssh_key=self.ssh_key, cmd_timeout=self.cmd_timeout,
             copy_timeout=self.copy_timeout, compression=self.compression,
             bwlimit=self.bwlimit
         )
 
         self.running = True
-        session.set_status('running')
 
         # Note this will also be stored directly in session.data
         counters = {
             'iterations': 0,
             'copies': 0,
             'errors_timeout': 0,
             'errors_nonzero': 0,
```

### Comparing `socs-0.4.5/socs/agents/synacc/agent.py` & `socs-0.5.0/socs/agents/synacc/agent.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,24 +11,37 @@
     """
     Agent to control and monitor Synaccess Networks PDUs.
 
     Args:
         ip_address(str): IP address for the device.
         username(str): Username credential to login to device.
         password(str): Password credential to login to device.
+        outlet_names(list of str): List of outlet names.
+        num_outlets(int): Number of outlets for device.
     """
 
-    def __init__(self, agent, ip_address, username, password):
+    def __init__(self, agent, ip_address, username, password, outlet_names=None, num_outlets=5):
         self.agent = agent
         self.log = agent.log
         self.lock = TimeoutLock()
         self.ip_address = ip_address
         self.user = username
         self.passw = password
 
+        if outlet_names is None:
+            outlet_names = []
+            for i in range(num_outlets):
+                outlet_names.append('outlet%i' % (i + 1))
+            self.outlet_names = outlet_names
+        else:
+            for i in range(num_outlets):
+                if len(outlet_names) <= i:
+                    outlet_names.append('outlet%i' % (i + 1))
+            self.outlet_names = outlet_names
+
         agg_params = {'frame_length': 60}
         self.agent.register_feed(
             'synaccess', record=True, agg_params=agg_params)
 
     def __get_status(self):
         req = "http://" + self.user + ":" + self.passw + "@" +\
             self.ip_address + "/cmd.cgi?$A5"
@@ -122,47 +135,48 @@
                     self.ip_address + "/cmd.cgi?$A7" + " " + on
                 requests.get(req)
                 return True, 'Set all outlets to {}'.format(params['on'])
             else:
                 return False, "Could not acquire lock"
 
     @ocs_agent.param('_')
-    def status_acq(self, session, params=None):
-        """status_acq()
+    def acq(self, session, params=None):
+        """acq()
 
         **Process** - Start data acquisition.
 
         Notes:
             The most recent data collected is stored in session.data in the
             structure::
 
                 >>> response.session['data']
                 {"fields":
-                    {synaccess:
-                        {0: 0 or 1, (0: OFF, 1:ON)
-                         1: 0 or 1, (0: OFF, 1:ON)
-                         2: 0 or 1, (0: OFF, 1:ON)
-                         3: 0 or 1, (0: OFF, 1:ON)
-                         4: 0 or 1, (0: OFF, 1:ON)
-                        }
+                    {"0": {"status": 0 or 1, (0: OFF, 1:ON)
+                           "name": "outlet1"},
+                     "1": {"status": 0 or 1, (0: OFF, 1:ON)
+                           "name": "outlet2"},
+                     "2": {"status": 0 or 1, (0: OFF, 1:ON)
+                           "name": "outlet3"},
+                     "3": {"status": 0 or 1, (0: OFF, 1:ON)
+                           "name": "outlet4"},
+                     "4": {"status": 0 or 1, (0: OFF, 1:ON)
+                           "name": "outlet5"},
                     }
                 }
 
         """
 
-        with self.lock.acquire_timeout(timeout=3, job='status_acq')\
+        with self.lock.acquire_timeout(timeout=3, job='acq')\
                 as acquired:
             if not acquired:
                 self.log.warn(
                     'Could not start status acq because {} is already running'
                     .format(self.lock.job))
                 return False, 'Could not acquire lock'
 
-            session.set_status('running')
-
             self.take_data = True
             last_release = time.time()
             session.data = {'fields': {}}
             while self.take_data:
                 if time.time() - last_release > 1.:
                     last_release = time.time()
                     if not self.lock.release_and_acquire(timeout=10):
@@ -180,27 +194,27 @@
                 resp = self.__get_status()
                 for i, x in enumerate(resp):
                     if x == '1':
                         status = 1
                     else:
                         status = 0
                     data['data']['synaccess_%d' % i] = status
-                    status_dict['%d' % i] = status
+                    status_dict['%d' % i] = {'status': status}
+                    status_dict['%d' % i]['name'] = self.outlet_names[i]
                 self.agent.publish_to_feed('synaccess', data)
-                field_dict = {'synaccess': status_dict}
                 session.data['timestamp'] = current_time
-                session.data['fields'] = field_dict
+                session.data['fields'] = status_dict
 
                 time.sleep(1)  # DAQ interval
                 # End of while loop
 
         self.agent.feeds['synaccess'].flush_buffer()
         return True, 'Acqusition exited cleanly'
 
-    def stop_status_acq(self, session, params=None):
+    def stop_acq(self, session, params=None):
         if self.take_data:
             self.take_data = False
             return True, 'requested to stop taking data'
 
         return False, 'acq is not currently running'
 
 
@@ -213,31 +227,36 @@
         parser = argparse.ArgumentParser()
 
     # Add options specific to this agent.
     pgroup = parser.add_argument_group('Agent Options')
     pgroup.add_argument('--ip-address', help='IP address for the device.')
     pgroup.add_argument('--username', help='Username credential to login to device.')
     pgroup.add_argument('--password', help='Password credential to login to device.')
+    pgroup.add_argument('--outlet-names', nargs='+', type=str,
+                        help="List of outlet names.")
+    pgroup.add_argument('--num-outlets', default=5, help='Number of outlets for the device.')
     return parser
 
 
 def main(args=None):
     parser = make_parser()
     args = site_config.parse_args(agent_class='SynaccessAgent',
                                   parser=parser,
                                   args=args)
 
     agent, runner = ocs_agent.init_site_agent(args)
 
     p = SynaccessAgent(agent,
                        ip_address=args.ip_address,
                        username=args.username,
-                       password=args.password)
-    agent.register_process('status_acq', p.status_acq,
-                           p.stop_status_acq, startup=True)
+                       password=args.password,
+                       outlet_names=args.outlet_names,
+                       num_outlets=args.num_outlets)
+    agent.register_process('acq', p.acq,
+                           p.stop_acq, startup=True)
     agent.register_task('get_status', p.get_status, startup={})
     agent.register_task('reboot', p.reboot)
     agent.register_task('set_outlet', p.set_outlet)
     agent.register_task('set_all', p.set_all)
 
     runner.run(agent, auto_reconnect=True)
```

### Comparing `socs-0.4.5/socs/agents/tektronix3021c/agent.py` & `socs-0.5.0/socs/agents/tektronix3021c/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/thorlabs_mc2000b/agent.py` & `socs-0.5.0/socs/agents/thorlabs_mc2000b/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,16 +98,14 @@
 
         with self.lock.acquire_timeout(job='init_chopper') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self.lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             # Establish connection to the chopper controller
             self.hdl = MC2000BOpen(self.comport, self.nbaud, self.timeout)
 
         if (self.hdl == 0):
             self.initialized = True
             self.log.info("Chopper connected")
         else:
@@ -134,16 +132,14 @@
         """
         with self.lock.acquire_timeout(timeout=3, job='set_frequency') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self.lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             MC2000BSetFrequency(self.hdl, params['freq'])
 
         return True, "Chopper frequency set to {} Hz".format(params['freq'])
 
     @ocs_agent.param('bladetype', type=str, default='MC1F2')
     def set_bladetype(self, session, params):
         """set_bladetype(bladetype=None)
@@ -159,16 +155,14 @@
         """
         with self.lock.acquire_timeout(timeout=3, job='set_bladetype') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self.lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             bladetype = bladetype_keys[params['bladetype']]
             MC2000BSetBladeType(self.hdl, bladetype)
 
         return True, "Chopper bladetype set to {}".format(params['bladetype'])
 
     @ocs_agent.param('output_mode', type=str, choices=['actual', 'target'], default='target')
     def set_reference_output_mode(self, session, params):
@@ -186,16 +180,14 @@
         """
         with self.lock.acquire_timeout(timeout=3, job='set_reference_output_mode') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self.lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             mode = params['output_mode']
             mode_int = outputmode_keys[mode]
             MC2000BSetReferenceOutput(self.hdl, mode_int)
 
         return True, "Chopper output mode set to {}".format(params['output_mode'])
 
     @ocs_agent.param('reference', type=str, default='internalinner')
@@ -214,16 +206,14 @@
         """
         with self.lock.acquire_timeout(timeout=3, job='set_blade_reference') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start Task because "
                               f"{self.lock.job} is already running")
                 return False, "Could not acquire lock"
 
-            session.set_status('running')
-
             reference = params['reference']
 
             if reference in ('external', 'internal'):
                 ref = reference_mode_keys[reference]
             else:
                 ref = reference_high_prec_mode[reference]
 
@@ -239,16 +229,14 @@
         """
         with self.lock.acquire_timeout(timeout=0, job='acq') as acquired:
             if not acquired:
                 self.log.warn(f"Could not start acq because {self.lock.job} "
                               "is already running")
                 return False, "Could not acquire lock."
 
-            session.set_status('running')
-
             last_release = time.time()
 
             self.take_data = True
 
             self.log.info("Starting data acquisition for {}".format(self.agent.agent_address))
 
             while self.take_data:
```

### Comparing `socs-0.4.5/socs/agents/ucsc_radiometer/agent.py` & `socs-0.5.0/socs/agents/ucsc_radiometer/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,14 @@
             {'timestamp': 1678820419.0,
              'pwv': 0.49253026985972237}
 
         """
         pm = Pacemaker(1 / 60, quantize=False)
 
         self.take_data = True
-        session.set_status('running')
 
         while self.take_data:
             try:
                 r = requests.get(self.url, timeout=60)
             except ValueError:
                 pm.sleep()
                 continue
```

### Comparing `socs-0.4.5/socs/agents/ups/agent.py` & `socs-0.5.0/socs/agents/ups/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,15 +304,14 @@
                 Units:: RMS Volts
             upsInputCurrent::
                 Units:: 0.1 RMS Amp
             upsInputTruePower::
                 Units:: Watts
         """
 
-        session.set_status('running')
         self.is_streaming = True
         timeout = time.time() + 60 * self.restart  # exit loop after self.restart minutes
         while self.is_streaming:
             if ((self.restart != 0) and (time.time() > timeout)):
                 break
             yield dsleep(1)
             if not self.connected:
```

### Comparing `socs-0.4.5/socs/agents/vantagepro2/agent.py` & `socs-0.5.0/socs/agents/vantagepro2/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,14 @@
 
         with self.lock.acquire_timeout(0, job='init') as acquired:
             if not acquired:
                 self.log.warn("Could not start init because "
                               "{} is already running".format(self.lock.job))
                 return False, "Could not acquire lock."
 
-            session.set_status('starting')
-
             self._initialize_module()
 
         # Start data acquisition if requested
         if params['auto_acquire']:
             self.agent.start('acq')
 
         time.sleep(2)
@@ -111,15 +109,14 @@
         with self.lock.acquire_timeout(0, job='acq') as acquired:
             if not acquired:
                 self.log.warn("""Could not start acq because {} is
                 already running"""
                               .format(self.lock.job))
                 return False, "Could not acquire lock."
 
-            session.set_status('running')
             # use pacemaker class to take data at regular intervals
             if sample_freq % 1 == 0:
                 pm = Pacemaker(sample_freq, True)
             else:
                 pm = Pacemaker(sample_freq)
 
             self.take_data = True
```

### Comparing `socs-0.4.5/socs/agents/vantagepro2/drivers.py` & `socs-0.5.0/socs/agents/vantagepro2/drivers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import array as arr
 import struct
 import time
 
+import numpy as np
 from serial import Serial
 
 # some commands require a CRC code (cyclic redundancy check) -
 # these require the provided CRC table
 crc_table = arr.array('H', [
     0x0, 0x1021, 0x2042, 0x3063, 0x4084, 0x50a5, 0x60c6, 0x70e7,
     0x8108, 0x9129, 0xa14a, 0xb16b, 0xc18c, 0xd1ad, 0xe1ce, 0xf1ef,
@@ -54,14 +55,30 @@
 
 def F_to_C(temp):
     """Function to convert fahrenheit measurement to celsius"""
 
     return (temp - 32) * (5 / 9)
 
 
+def wind_chill(temp, wind):
+    """Function to calculate wind chill temperature. Only valid if temp < 50F.
+    Taken from https://www.calculator.net/wind-chill-calculator.html
+    If temp > 50F, need to use heat index instead...
+
+        Temp: Temperature in Fahrenheit
+        wind: Speed in miles per hour
+    """
+    # Calculation not valid above 50 F
+    if temp > 50:
+        return temp
+
+    chill = 35.75 + 0.6215 * temp - 35.75 * np.power(wind, 0.16) + 0.4275 * temp * np.power(wind, 0.16)
+    return chill
+
+
 class VantagePro2:
     """Allows communication to Vantage Pro 2 Weather Monitor Module.
     Contains commands to be issued and member variables that store
     collected data.
     """
 
     def __init__(self, path, baud=19200, timeout=1):
@@ -314,19 +331,23 @@
         loop_data['transmitter_battery_status'] = byte_data[71]
         loop_data['console_battery_voltage'] = ((byte_data[72] * 300) / 512) / 100.0
         loop_data['forecast_icons'] = byte_data[73]
         loop_data['forecast_rule_num'] = byte_data[74]
         loop_data['time_sunrise'] = byte_data[75]
         loop_data['time_sunset'] = byte_data[76]
 
-        # Correct UV Index by a factor of 10 and fix overflow
+        # Add wind chill temperature to observation data
+        temp = byte_data[9] / 10.0
+        wind_speed = byte_data[10]
+        loop_data['wind_chill_temp'] = F_to_C(wind_chill(temp, wind_speed))
+
+        # Fix overflow
         uvi = loop_data['UV']
         if uvi < 0:
             uvi += 2**8
-        uvi /= 10
         loop_data['UV'] = uvi
 
         # CRC check, data must be sent byte by byte
         pure_data = struct.unpack('=99b', info)
         self.crc_check(pure_data)
 
         return loop_data
```

### Comparing `socs-0.4.5/socs/agents/wiregrid_actuator/agent.py` & `socs-0.5.0/socs/agents/wiregrid_actuator/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -793,16 +793,14 @@
                 self.log.warn(
                     'acq(): '
                     'Lock could not be acquired because it is held by {}.'
                     .format(self.lock.job))
                 return False, 'acq(): Could not acquire lock.'
             self.log.info('acq(): Got the lock')
 
-            session.set_status('running')
-
             self.run_acq = True
             last_release = time.time()
             session.data = {'fields': {}}
             while self.run_acq:
                 if time.time() - last_release > 1.:
                     last_release = time.time()
                     if not self.lock.release_and_acquire(timeout=180):
```

### Comparing `socs-0.4.5/socs/agents/wiregrid_actuator/drivers/Actuator.py` & `socs-0.5.0/socs/agents/wiregrid_actuator/drivers/Actuator.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/wiregrid_actuator/drivers/DigitalIO.py` & `socs-0.5.0/socs/agents/wiregrid_actuator/drivers/DigitalIO.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/wiregrid_actuator/limitswitch_config.py` & `socs-0.5.0/socs/agents/wiregrid_actuator/limitswitch_config.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/wiregrid_encoder/agent.py` & `socs-0.5.0/socs/agents/wiregrid_encoder/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,16 +110,14 @@
         with self.lock.acquire_timeout(timeout=0, job='acq') as acquired:
             if not acquired:
                 self.log.warn(
                     'Could not start acq because {} is already running'
                     .format(self.lock.job))
                 return False, 'Could not acquire lock.'
 
-            session.set_status('running')
-
             self.take_data = True
             # Initialize data containers
             session.data = {'fields': {'irig_data': {}, 'encoder_data': {},
                             'timestamp': 0}}
             irig_rdata = {'timestamp': 0,
                           'block_name': 'wgencoder_irig',
                           'data': {
@@ -312,15 +310,15 @@
                     'pru_clock': enc_rdata['data']['pru_clock'],
                     'reference_degree':
                         enc_rdata['data']['reference_degree'],
                     'error': enc_rdata['data']['error']
                 }
                 session.data['timestamp'] = current_time
                 session.data['fields']['irig_data'] = irig_field_dict
-                session.data['fields']['enc_data'] = enc_field_dict
+                session.data['fields']['encoder_data'] = enc_field_dict
                 # End of loop
             # End of lock acquiring
 
         self.agent.feeds['wgencoder_rough'].flush_buffer()
         # This buffer (full data) has huge data size.
         self.agent.feeds['wgencoder_full'].flush_buffer()
```

### Comparing `socs-0.4.5/socs/agents/wiregrid_encoder/drivers.py` & `socs-0.5.0/socs/agents/wiregrid_encoder/drivers.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/wiregrid_kikusui/agent.py` & `socs-0.5.0/socs/agents/wiregrid_kikusui/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
         self.take_data = False
         self.kikusui_ip = kikusui_ip
         self.kikusui_port = int(kikusui_port)
         self.encoder_agent = encoder_agent
         self.debug = debug
 
-        self.position_path = '/data/wg-data/position.log'
         self.debug_log_path = '/data/wg-data/action/'
 
         self.open_trial = 10
         self.Deg = 360 / 52000
         # self.feedback_time = [0.151, 0.241, 0.271, 0.301, 0.331]
         self.feedback_time = [0.151, 0.241, 0.271, 0.361, 0.451]
         self.feedback_cut = [1., 2., 3., 5.0, 8.0]
@@ -165,15 +164,15 @@
                     'Failed to get encoder position | '
                     '{}'.format(e)
                 )
                 return -1.
 
         try:
             position = (float)(
-                response.session['data']['fields']['enc_data']['reference_degree'][-1])
+                response.session['data']['fields']['encoder_data']['reference_degree'][-1])
         except Exception as e:
             self.log.warn(
                 'Failed to get encoder position | '
                 '{}'.format(e)
             )
 
         return position
@@ -383,34 +382,30 @@
             if angle < 0.:
                 return False, \
                     'Could not get the angle of the wire-grid rotation.'
 
             return True, \
                 'Get wire-grid rotation angle = {} deg'.format(angle)
 
-    @ocs_agent.param('storepath', default='/data/wg-data/action/', type=str)
-    def calibrate_wg(self, session, params):
-        """calibrate_wg(storepath='/data/wg-data/action/')
+    def calibrate_wg(self, session, params=None):
+        """calibrate_wg()
 
         **Task** - Run rotation-motor calibration for wire-grid.
 
-        Parameters:
-            storepath (str): Path for log file.
         """
-        storepath = params.get('storepath')
 
         with self.lock.acquire_timeout(timeout=5, job='calibrate_wg')\
                 as acquired:
             if not acquired:
                 self.log.warn('Could not run calibrate_wg() '
                               'because {} is already running'
                               .format(self.lock.job))
                 return False, 'Could not acquire lock'
 
-            logfile = openlog(storepath)
+            logfile = openlog(self.debug_log_path)
 
             cycle = 1
             for i in range(11):
                 tperiod = 0.10 + 0.02 * i
                 for j in range(100):
                     if j % 20 == 0:
                         self.log.warn(f'this is {cycle}th time action')
@@ -464,22 +459,26 @@
 
             self.feedback_steps = params.get('feedback_steps', 8)
             self.num_laps = params.get('num_laps', 1)
             self.stopped_time = params.get('stopped_time', 10)
             self.feedback_time = params.get(
                 'feedback_time', [0.181, 0.221, 0.251, 0.281, 0.301])
 
-            logfile = openlog(self.debug_log_path)
+            if self.debug:
+                logfile = openlog(self.debug_log_path)
+            else:
+                logfile = None
 
             for i in range(int(self.num_laps * 16.)):
                 self._move_next(
                     logfile, self.feedback_steps, self.feedback_time)
                 time.sleep(self.stopped_time)
 
-            logfile.close()
+            if self.debug:
+                logfile.close()
 
             return True, 'Step-wise rotation finished'
 
     def IV_acq(self, session, params=None):
         """IV_acq()
 
         **Process** - Run data acquisition.
@@ -508,16 +507,14 @@
         with self.lock.acquire_timeout(timeout=1000, job='IV_acq') as acquired:
             if not acquired:
                 self.log.warn('Could not run IV_acq '
                               'because {} is already running'
                               .format(self.lock.job))
                 return False, 'Could not acquire lock'
 
-            session.set_status('running')
-
             self.take_data = True
             last_release = time.time()
             session.data = {'fields': {}}
             while self.take_data:
                 if time.time() - last_release > 1.:
                     last_release = time.time()
                     if not self.lock.release_and_acquire(timeout=1000):
```

### Comparing `socs-0.4.5/socs/agents/wiregrid_kikusui/drivers/common.py` & `socs-0.5.0/socs/agents/wiregrid_kikusui/drivers/common.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/agents/xy_stage/agent.py` & `socs-0.5.0/socs/agents/xy_stage/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,14 @@
 
         with self.lock.acquire_timeout(timeout=0, job='acq') as acquired:
             if not acquired:
                 self.log.warn("Could not start acq because {} is already running".format(self.lock.job))
                 return False, "Could not acquire lock."
 
             self.log.info(f"Starting Data Acquisition for XY Stages at {f_sample} Hz")
-            session.set_status('running')
             self.take_data = True
             last_release = time.time()
 
             while self.take_data:
                 if time.time() - last_release > 1.:
                     if not self.lock.release_and_acquire(timeout=10):
                         self.log.warn(f"Could not re-acquire lock now held by {self.lock.job}.")
```

### Comparing `socs-0.4.5/socs/common/moxa_serial.py` & `socs-0.5.0/socs/common/moxa_serial.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/common/pmx.py` & `socs-0.5.0/socs/common/pmx.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,22 +75,24 @@
 
     def check_current(self):
         """Check the current."""
         self.clean_serial()
         self.ser.write("MEAS:CURR?\n\r")
         self.wait()
         try:
-            val = float(self.ser.readline())
-            msg = "Measured current = %.3f A" % (val)
+            val = self.ser.readline()
+            curr = float(val)
+            msg = "Measured current = %.3f A" % (curr)
             # print(msg)
         except ValueError:
-            val = -999.
+            print(f"Could not convert '{val}' to float")
+            curr = -999.
             msg = 'WARNING! Could not get correct current value! | Response = "%s"' % (val)
             print(msg)
-        return msg, val
+        return msg, curr
 
     def check_voltage_current(self):
         """Check both the voltage and current."""
         self.clean_serial()
         voltage = self.check_voltage()[1]
         current = self.check_current()[1]
         # msg = (
```

### Comparing `socs-0.4.5/socs/common/prologix_interface.py` & `socs-0.5.0/socs/common/prologix_interface.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/db/suprsync.py` & `socs-0.5.0/socs/db/suprsync.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/db/suprsync_cli.py` & `socs-0.5.0/socs/db/suprsync_cli.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/mibs/IBOOTPDU-MIB.py` & `socs-0.5.0/socs/mibs/IBOOTPDU-MIB.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/mibs/MBG-SNMP-LTNG-MIB.py` & `socs-0.5.0/socs/mibs/MBG-SNMP-LTNG-MIB.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/mibs/MBG-SNMP-ROOT-MIB.py` & `socs-0.5.0/socs/mibs/MBG-SNMP-ROOT-MIB.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/mibs/SNMPv2-MIB.py` & `socs-0.5.0/socs/mibs/SNMPv2-MIB.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/mibs/UPS-MIB.py` & `socs-0.5.0/socs/mibs/UPS-MIB.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/plugin.py` & `socs-0.5.0/socs/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     'BlueforsAgent': {'module': 'socs.agents.bluefors.agent', 'entry_point': 'main'},
     'CrateAgent': {'module': 'socs.agents.smurf_crate_monitor.agent', 'entry_point': 'main'},
     'CryomechCPAAgent': {'module': 'socs.agents.cryomech_cpa.agent', 'entry_point': 'main'},
     'FPGAAgent': {'module': 'socs.agents.holo_fpga.agent', 'entry_point': 'main'},
     'FlowmeterAgent': {'module': 'socs.agents.ifm_sbn246_flowmeter.agent', 'entry_point': 'main'},
     'FTSAerotechAgent': {'module': 'socs.agents.fts_aerotech.agent', 'entry_point': 'main'},
     'GeneratorAgent': {'module': 'socs.agents.generator.agent', 'entry_point': 'main'},
+    'Hi6200Agent': {'module': 'socs.agents.hi6200.agent', 'entry_point': 'main'},
     'HWPBBBAgent': {'module': 'socs.agents.hwp_encoder.agent', 'entry_point': 'main'},
     'HWPGripperAgent': {'module': 'socs.agents.hwp_gripper.agent', 'entry_point': 'main'},
     'HWPPCUAgent': {'module': 'socs.agents.hwp_pcu.agent', 'entry_point': 'main'},
     'HWPPicoscopeAgent': {'module': 'socs.agents.hwp_picoscope.agent', 'entry_point': 'main'},
     'HWPPIDAgent': {'module': 'socs.agents.hwp_pid.agent', 'entry_point': 'main'},
     'HWPPMXAgent': {'module': 'socs.agents.hwp_pmx.agent', 'entry_point': 'main'},
     'HWPSupervisor': {'module': 'socs.agents.hwp_supervisor.agent', 'entry_point': 'main'},
@@ -22,14 +23,15 @@
     'Lakeshore336Agent': {'module': 'socs.agents.lakeshore336.agent', 'entry_point': 'main'},
     'Lakeshore370Agent': {'module': 'socs.agents.lakeshore370.agent', 'entry_point': 'main'},
     'Lakeshore372Agent': {'module': 'socs.agents.lakeshore372.agent', 'entry_point': 'main'},
     'Lakeshore425Agent': {'module': 'socs.agents.lakeshore425.agent', 'entry_point': 'main'},
     'LATRtXYStageAgent': {'module': 'socs.agents.xy_stage.agent', 'entry_point': 'main'},
     'MagpieAgent': {'module': 'socs.agents.magpie.agent', 'entry_point': 'main'},
     'MeinbergM1000Agent': {'module': 'socs.agents.meinberg_m1000.agent', 'entry_point': 'main'},
+    'MeinbergSyncboxAgent': {'module': 'socs.agents.meinberg_syncbox.agent', 'entry_point': 'main'},
     'PfeifferAgent': {'module': 'socs.agents.pfeiffer_tpg366.agent', 'entry_point': 'main'},
     'PfeifferTC400Agent': {'module': 'socs.agents.pfeiffer_tc400.agent', 'entry_point': 'main'},
     'PysmurfController': {'module': 'socs.agents.pysmurf_controller.agent', 'entry_point': 'main'},
     'PysmurfMonitor': {'module': 'socs.agents.pysmurf_monitor.agent', 'entry_point': 'main'},
     'ScpiPsuAgent': {'module': 'socs.agents.scpi_psu.agent', 'entry_point': 'main'},
     'SmurfFileEmulator': {'module': 'socs.agents.smurf_file_emulator.agent', 'entry_point': 'main'},
     'SmurfStreamSimulator': {'module': 'socs.agents.smurf_stream_simulator.agent', 'entry_point': 'main'},
```

### Comparing `socs-0.4.5/socs/snmp.py` & `socs-0.5.0/socs/snmp.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/socs/testing/device_emulator.py` & `socs-0.5.0/socs/testing/device_emulator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,53 @@
+import logging
 import shutil
 import socket
 import subprocess
 import threading
 import time
+import traceback as tb
+from copy import deepcopy
+from typing import Dict
 
 import pytest
 import serial
 
 
-def create_device_emulator(responses, relay_type, port=9001, encoding='utf-8'):
+def create_device_emulator(responses, relay_type, port=9001, encoding='utf-8',
+                           reconnect=False):
     """Create a device emulator fixture.
 
     This provides a device emulator that can be used to mock a device during
     testing.
 
     Args:
         responses (dict): Dictionary with commands as keys, and responses as
             values. See :class:`.DeviceEmulator` for details.
         relay_type (str): Communication relay type. Either 'serial' or 'tcp'.
         port (int): Port for the TCP relay to listen for connections on.
             Defaults to 9001. Only used if relay_type is 'tcp'.
         encoding (str): Encoding for the messages and responses. See
             :func:`socs.testing.device_emulator.DeviceEmulator` for more
             details.
+        reconnect (bool): If True, on TCP client disconnect, the emulator will
+            listen for new incoming connections instead of quitting
 
     Returns:
         function:
             A pytest fixture that creates a Device emulator of the specified
             type.
 
     """
     if relay_type not in ['serial', 'tcp']:
         raise NotImplementedError(f"relay_type '{relay_type}' is not"
                                   + "implemented or is an invalid type")
 
     @pytest.fixture()
     def create_device():
-        device = DeviceEmulator(responses, encoding)
+        device = DeviceEmulator(responses, encoding, reconnect=reconnect)
 
         if relay_type == 'serial':
             device.create_serial_relay()
         elif relay_type == 'tcp':
             device.create_tcp_relay(port)
 
         yield device
@@ -58,14 +65,16 @@
         responses (dict): Initial responses, any response required by Agent
             startup, if any.
         encoding (str): Encoding for the messages and responses.
             DeviceEmulator will try to encode and decode messages with the
             given encoding. No encoding is used if set to None. That can be
             useful if you need to use raw data from your hardware. Defaults
             to 'utf-8'.
+        reconnect (bool): If True, on TCP client disconnect, the emulator will
+            listen for new incoming connections instead of quitting
 
     Attributes:
         responses (dict): Current set of responses the DeviceEmulator would
             give. Should all be strings, not bytes-like.
         default_response (str): Default response to send if a command is
             unrecognized. No response is sent and an error message is logged if
             a command is unrecognized and the default response is set to None.
@@ -75,22 +84,31 @@
         _type (str): Relay type, either 'serial' or 'tcp'.
         _read (bool): Used to stop the background reading of data recieved on
             the relay.
         _conn (socket.socket): TCP connection for use in 'tcp' relay.
 
     """
 
-    def __init__(self, responses, encoding='utf-8'):
-        self.responses = responses
+    def __init__(self, responses, encoding='utf-8', reconnect=False):
+        self.responses = deepcopy(responses)
         self.default_response = None
         self.encoding = encoding
+        self.reconnect = reconnect
         self._type = None
         self._read = True
         self._conn = None
 
+        self.logger = logging.getLogger(self.__class__.__name__)
+        self.logger.setLevel(logging.DEBUG)
+        if len(self.logger.handlers) == 0:
+            formatter = logging.Formatter("%(asctime)s - %(name)s: %(message)s")
+            handler = logging.StreamHandler()
+            handler.setFormatter(formatter)
+            self.logger.addHandler(handler)
+
     @staticmethod
     def _setup_socat():
         """Setup a data relay with socat.
 
         The "./responder" link is the external end of the relay, which the Agent
         should connect to. "./internal" is used within the DeviceEmulator object to accept
         commands and to respond to the Agent.
@@ -128,15 +146,15 @@
             baudrate=57600,
             timeout=5,
         )
         bkg_read = threading.Thread(name='background',
                                     target=self._read_serial)
         bkg_read.start()
 
-    def _get_response(self, msg):
+    def get_response(self, msg):
         """Determine the response to a given message.
 
         Args:
             msg (str): Command string to get the response for.
 
         Returns:
             str: Response string. Will return None if a valid response is not
@@ -151,15 +169,17 @@
 
         try:
             if isinstance(self.responses[msg], list):
                 response = self.responses[msg].pop(0)
             else:
                 response = self.responses[msg]
         except Exception as e:
-            print(f"encountered error {e}")
+            self.logger.info(f"Responses: {self.responses}")
+            self.logger.info(f"encountered error {e}")
+            self.logger.info(tb.format_exc())
             response = None
 
         return response
 
     def _read_serial(self):
         """Loop until shutdown, reading any commands sent over the relay.
         Respond immediately to a command with the response in self.responses.
@@ -168,26 +188,26 @@
         self._read = True
 
         while self._read:
             if self.ser.in_waiting > 0:
                 msg = self.ser.readline()
                 if self.encoding:
                     msg = msg.strip().decode(self.encoding)
-                print(f"msg='{msg}'")
+                self.logger.debug(f"msg='{msg}'")
 
-                response = self._get_response(msg)
+                response = self.get_response(msg)
 
                 # Avoid user providing bytes-like response
                 if isinstance(response, bytes) and self.encoding is not None:
                     response = response.decode()
 
                 if response is None:
                     continue
 
-                print(f"response='{response}'")
+                self.logger.debug(f"response='{response}'")
                 if self.encoding:
                     response = (response + '\r\n').encode(self.encoding)
                 self.ser.write(response)
 
             time.sleep(0.01)
 
     def __del__(self):
@@ -226,43 +246,55 @@
         # Listen for connections
         self._sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         while not self._sock_bound:
             try:
                 self._sock.bind(('127.0.0.1', port))
                 self._sock_bound = True
             except OSError:
-                print(f"Failed to bind to port {port}, trying again...")
+                self.logger.error(f"Failed to bind to port {port}, trying again...")
                 time.sleep(1)
         self._sock.listen(1)
-        print("Device emulator waiting for tcp client connection")
+        self.logger.info("Device emulator waiting for tcp client connection")
         self._conn, client_address = self._sock.accept()
-        print(f"Client connection made from {client_address}")
+        self.logger.info(f"Client connection made from {client_address}")
 
         while self._read:
             try:
                 msg = self._conn.recv(4096)
+                if not msg:
+                    self.logger.info("Client disconnected")
+                    if self.reconnect:
+                        self.logger.info("Waiting for new connection")
+                        # attempt to reconnect
+                        self._conn, client_address = self._sock.accept()
+                        self.logger.info(f"Client connection made from {client_address}")
+                        continue
+                    else:
+                        self.logger.info("Shutting down")
+                        break
+
             # Was seeing this on tests in the cryomech agent
             except ConnectionResetError:
-                print('Caught connection reset on Agent clean up')
+                self.logger.info('Caught connection reset on Agent clean up')
                 break
             if self.encoding:
                 msg = msg.strip().decode(self.encoding)
             if msg:
-                print(f"msg='{msg}'")
+                self.logger.debug(f"msg='{msg}'")
 
-                response = self._get_response(msg)
+                response = self.get_response(msg)
 
                 # Avoid user providing bytes-like response
                 if isinstance(response, bytes) and self.encoding is not None:
                     response = response.decode()
 
                 if response is None:
                     continue
 
-                print(f"response='{response}'")
+                self.logger.debug(f"response='{response}'")
                 if self.encoding:
                     response = response.encode(self.encoding)
                 self._conn.sendall(response)
 
             time.sleep(0.01)
 
         self._conn.close()
@@ -294,14 +326,26 @@
                                     kwargs={'port': port})
         bkg_read.start()
 
         # wait for socket to bind properly before returning
         while not self._sock_bound:
             time.sleep(0.1)
 
+    def update_responses(self, responses: Dict):
+        """
+        Updates the current responses. See ``define_responses`` for more detail.
+
+        Args
+        ------
+        responses: dict
+            Dict of commands to use to update the current responses.
+        """
+        self.responses.update(responses)
+        self.logger.info(f"responses set to {self.responses}")
+
     def define_responses(self, responses, default_response=None):
         """Define what responses are available to reply with on the configured
         communication relay.
 
         Args:
             responses (dict): Dictionary of commands: response. Values can be a
                 list, in which case the responses in the list are popped and
@@ -320,11 +364,11 @@
 
         Notes:
             The DeviceEmulator will handle encoding/decoding. The responses
             defined should all be strings, not bytes-like, unless you set
             ``encoding=None``.
 
         """
-        print(f"responses set to {responses}")
-        self.responses = responses
-        print(f"default response set to '{default_response}'")
+        self.logger.info(f"responses set to {responses}")
+        self.responses = deepcopy(responses)
+        self.logger.info(f"default response set to '{default_response}'")
         self.default_response = default_response
```

### Comparing `socs-0.4.5/socs.egg-info/PKG-INFO` & `socs-0.5.0/socs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: socs
-Version: 0.4.5
+Version: 0.5.0
 Summary: Simons Observatory Control System
 Home-page: https://github.com/simonsobs/socs
 Project-URL: Source Code, https://github.com/simonsobs/ocs
 Project-URL: Documentation, https://ocs.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/simonsobs/ocs/issues
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Framework :: Twisted
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
@@ -24,21 +29,21 @@
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: sqlalchemy>=1.4
 Requires-Dist: twisted
 Requires-Dist: pyasn1==0.4.8
 Provides-Extra: all
 Requires-Dist: labjack-ljm; extra == "all"
-Requires-Dist: pyepics; extra == "all"
+Requires-Dist: pixell; extra == "all"
+Requires-Dist: pandas; extra == "all"
 Requires-Dist: pfeiffer-vacuum-protocol==0.4; extra == "all"
-Requires-Dist: scipy; extra == "all"
+Requires-Dist: pyepics; extra == "all"
 Requires-Dist: numexpr; extra == "all"
 Requires-Dist: so3g; extra == "all"
-Requires-Dist: pixell; extra == "all"
-Requires-Dist: pandas; extra == "all"
+Requires-Dist: scipy; extra == "all"
 Provides-Extra: acu
 Requires-Dist: pixell; extra == "acu"
 Requires-Dist: so3g; extra == "acu"
 Provides-Extra: labjack
 Requires-Dist: labjack-ljm; extra == "labjack"
 Requires-Dist: numexpr; extra == "labjack"
 Requires-Dist: scipy; extra == "labjack"
@@ -55,35 +60,16 @@
 Provides-Extra: timing-master
 Requires-Dist: pyepics; extra == "timing-master"
 
 ========================================
 SOCS - Simons Observatory Control System
 ========================================
 
-.. image:: https://img.shields.io/github/actions/workflow/status/simonsobs/socs/develop.yml?branch=main
-    :target: https://github.com/simonsobs/socs/actions?query=workflow%3A%22Build+Test+Images%22
-    :alt: GitHub Workflow Status
-
-.. image:: https://readthedocs.org/projects/socs/badge/?version=main
-    :target: https://socs.readthedocs.io/en/main/?badge=main
-    :alt: Documentation Status
-
-.. image:: https://coveralls.io/repos/github/simonsobs/socs/badge.svg
-    :target: https://coveralls.io/github/simonsobs/socs
-
-.. image:: https://img.shields.io/badge/dockerhub-latest-blue
-    :target: https://hub.docker.com/r/simonsobs/socs
-
-.. image:: https://img.shields.io/pypi/v/socs
-   :target: https://pypi.org/project/socs/
-   :alt: PyPI Package
-
-.. image:: https://results.pre-commit.ci/badge/github/simonsobs/socs/main.svg
-   :target: https://results.pre-commit.ci/latest/github/simonsobs/socs/main
-   :alt: pre-commit.ci status
+| |pypi| |versions| |docker| |license|
+| |tests| |pre-commit| |coverage| |docs|
 
 Overview
 --------
 
 This repository, `SOCS`_, contains hardware control code for the
 Simons Observatory.  This code operates within the framework provided
 by `OCS`_.
@@ -195,7 +181,37 @@
 
 License
 --------
 This project is licensed under the BSD 2-Clause License - see the
 `LICENSE.txt`_ file for details.
 
 .. _LICENSE.txt: https://github.com/simonsobs/socs/blob/main/LICENSE.txt
+
+
+.. |coverage| image:: https://coveralls.io/repos/github/simonsobs/socs/badge.svg
+    :target: https://coveralls.io/github/simonsobs/socs
+
+.. |docker| image:: https://img.shields.io/badge/dockerhub-latest-blue
+    :target: https://hub.docker.com/r/simonsobs/socs
+
+.. |docs| image:: https://readthedocs.org/projects/socs/badge/?version=main
+    :target: https://socs.readthedocs.io/en/main/?badge=main
+    :alt: Documentation Status
+
+.. |license| image:: https://img.shields.io/pypi/l/socs
+    :target: LICENSE.txt
+    :alt: PyPI - License
+
+.. |pre-commit| image:: https://results.pre-commit.ci/badge/github/simonsobs/socs/main.svg
+   :target: https://results.pre-commit.ci/latest/github/simonsobs/socs/main
+   :alt: pre-commit.ci status
+
+.. |pypi| image:: https://img.shields.io/pypi/v/socs
+   :target: https://pypi.org/project/socs/
+   :alt: PyPI Package
+
+.. |tests| image:: https://github.com/simonsobs/socs/actions/workflows/develop.yml/badge.svg?branch=main
+    :target: https://github.com/simonsobs/socs/actions/workflows/develop.yml
+    :alt: GitHub Workflow Status
+
+.. |versions| image:: https://img.shields.io/pypi/pyversions/socs
+    :alt: PyPI - Python Version
```

### Comparing `socs-0.4.5/socs.egg-info/SOURCES.txt` & `socs-0.5.0/socs.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -84,21 +84,24 @@
 socs/agents/lakeshore372/agent.py
 socs/agents/lakeshore425/__init__.py
 socs/agents/lakeshore425/agent.py
 socs/agents/magpie/__init__.py
 socs/agents/magpie/agent.py
 socs/agents/meinberg_m1000/__init__.py
 socs/agents/meinberg_m1000/agent.py
+socs/agents/meinberg_syncbox/__init__.py
+socs/agents/meinberg_syncbox/agent.py
 socs/agents/pfeiffer_tc400/__init__.py
 socs/agents/pfeiffer_tc400/agent.py
 socs/agents/pfeiffer_tc400/drivers.py
 socs/agents/pfeiffer_tpg366/__init__.py
 socs/agents/pfeiffer_tpg366/agent.py
 socs/agents/pysmurf_controller/__init__.py
 socs/agents/pysmurf_controller/agent.py
+socs/agents/pysmurf_controller/smurf_subprocess_util.py
 socs/agents/pysmurf_monitor/__init__.py
 socs/agents/pysmurf_monitor/agent.py
 socs/agents/scpi_psu/__init__.py
 socs/agents/scpi_psu/agent.py
 socs/agents/scpi_psu/drivers.py
 socs/agents/smurf_crate_monitor/__init__.py
 socs/agents/smurf_crate_monitor/agent.py
@@ -147,16 +150,18 @@
 socs/common/prologix_interface.py
 socs/db/__init__.py
 socs/db/suprsync.py
 socs/db/suprsync_cli.py
 socs/mibs/IBOOTPDU-MIB.py
 socs/mibs/MBG-SNMP-LTNG-MIB.py
 socs/mibs/MBG-SNMP-ROOT-MIB.py
+socs/mibs/MBG-SYNCBOX-N2X-MIB.py
 socs/mibs/SNMPv2-MIB.py
 socs/mibs/UPS-MIB.py
 socs/mibs/__init__.py
 socs/testing/__init__.py
 socs/testing/device_emulator.py
+socs/testing/hwp_emulator.py
 tests/test_device_emulator.py
 tests/test_plugin.py
 tests/test_snmp.py
 tests/test_util.py
```

### Comparing `socs-0.4.5/tests/test_device_emulator.py` & `socs-0.5.0/tests/test_device_emulator.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.5/versioneer.py` & `socs-0.5.0/versioneer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,64 @@
 
-# Version: 0.18
+# Version: 0.29
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
-* https://github.com/warner/python-versioneer
+* https://github.com/python-versioneer/python-versioneer
 * Brian Warner
-* License: Public Domain
-* Compatible With: python2.6, 2.7, 3.2, 3.3, 3.4, 3.5, 3.6, and pypy
+* License: Public Domain (Unlicense)
+* Compatible with: Python 3.7, 3.8, 3.9, 3.10, 3.11 and pypy3
 * [![Latest Version][pypi-image]][pypi-url]
 * [![Build Status][travis-image]][travis-url]
 
-This is a tool for managing a recorded version number in distutils-based
+This is a tool for managing a recorded version number in setuptools-based
 python projects. The goal is to remove the tedious and error-prone "update
 the embedded version string" step from your release process. Making a new
 release should be as easy as recording a new tag in your version-control
 system, and maybe making new tarballs.
 
 
 ## Quick Install
 
-* `pip install versioneer` to somewhere to your $PATH
-* add a `[versioneer]` section to your setup.cfg (see below)
-* run `versioneer install` in your source tree, commit the results
+Versioneer provides two installation modes. The "classic" vendored mode installs
+a copy of versioneer into your repository. The experimental build-time dependency mode
+is intended to allow you to skip this step and simplify the process of upgrading.
+
+### Vendored mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+   * Note that you will need to add `tomli; python_version < "3.11"` to your
+     build-time dependencies if you use `pyproject.toml`
+* run `versioneer install --vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
+
+### Build-time dependency mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+* add `versioneer` (with `[toml]` extra, if configuring in `pyproject.toml`)
+  to the `requires` key of the `build-system` table in `pyproject.toml`:
+  ```toml
+  [build-system]
+  requires = ["setuptools", "versioneer[toml]"]
+  build-backend = "setuptools.build_meta"
+  ```
+* run `versioneer install --no-vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
 
 ## Version Identifiers
 
 Source trees come from a variety of places:
 
 * a version-control system checkout (mostly used by developers)
 * a nightly tarball, produced by build automation
@@ -53,15 +82,15 @@
 unreleased software (between tags), the version identifier should provide
 enough information to help developers recreate the same tree, while also
 giving them an idea of roughly how old the tree is (after version 1.2, before
 version 1.3). Many VCS systems can report a description that captures this,
 for example `git describe --tags --dirty --always` reports things like
 "0.7-1-g574ab98-dirty" to indicate that the checkout is one revision past the
 0.7 tag, has a unique revision id of "574ab98", and is "dirty" (it has
-uncommitted changes.
+uncommitted changes).
 
 The version identifier is used for multiple purposes:
 
 * to allow the module to self-identify its version: `myproject.__version__`
 * to choose a name and prefix for a 'setup.py sdist' tarball
 
 ## Theory of Operation
@@ -158,15 +187,15 @@
 display the full contents of `get_versions()` (including the `error` string,
 which may help identify what went wrong).
 
 ## Known Limitations
 
 Some situations are known to cause problems for Versioneer. This details the
 most significant ones. More can be found on Github
-[issues page](https://github.com/warner/python-versioneer/issues).
+[issues page](https://github.com/python-versioneer/python-versioneer/issues).
 
 ### Subprojects
 
 Versioneer has limited support for source trees in which `setup.py` is not in
 the root directory (e.g. `setup.py` and `.git/` are *not* siblings). The are
 two common reasons why `setup.py` might not be in the root:
 
@@ -186,17 +215,17 @@
 
 `pip install --editable .` should work correctly. `setup.py install` might
 work too.
 
 Pip-8.1.1 is known to have this problem, but hopefully it will get fixed in
 some later version.
 
-[Bug #38](https://github.com/warner/python-versioneer/issues/38) is tracking
+[Bug #38](https://github.com/python-versioneer/python-versioneer/issues/38) is tracking
 this issue. The discussion in
-[PR #61](https://github.com/warner/python-versioneer/pull/61) describes the
+[PR #61](https://github.com/python-versioneer/python-versioneer/pull/61) describes the
 issue from the Versioneer side in more detail.
 [pip PR#3176](https://github.com/pypa/pip/pull/3176) and
 [pip PR#3615](https://github.com/pypa/pip/pull/3615) contain work to improve
 pip to let Versioneer work correctly.
 
 Versioneer-0.16 and earlier only looked for a `.git` directory next to the
 `setup.cfg`, so subprojects were completely unsupported with those releases.
@@ -216,39 +245,28 @@
 `pkg_resources.DistributionNotFound` errors when running the entrypoint
 script, which must be resolved by re-installing the package. This happens
 when the install happens with one version, then the egg_info data is
 regenerated while a different version is checked out. Many setup.py commands
 cause egg_info to be rebuilt (including `sdist`, `wheel`, and installing into
 a different virtualenv), so this can be surprising.
 
-[Bug #83](https://github.com/warner/python-versioneer/issues/83) describes
+[Bug #83](https://github.com/python-versioneer/python-versioneer/issues/83) describes
 this one, but upgrading to a newer version of setuptools should probably
 resolve it.
 
-### Unicode version strings
-
-While Versioneer works (and is continually tested) with both Python 2 and
-Python 3, it is not entirely consistent with bytes-vs-unicode distinctions.
-Newer releases probably generate unicode version strings on py2. It's not
-clear that this is wrong, but it may be surprising for applications when then
-write these strings to a network connection or include them in bytes-oriented
-APIs like cryptographic checksums.
-
-[Bug #71](https://github.com/warner/python-versioneer/issues/71) investigates
-this question.
-
 
 ## Updating Versioneer
 
 To upgrade your project to a new release of Versioneer, do the following:
 
 * install the new Versioneer (`pip install -U versioneer` or equivalent)
-* edit `setup.cfg`, if necessary, to include any new configuration settings
-  indicated by the release notes. See [UPGRADING](./UPGRADING.md) for details.
-* re-run `versioneer install` in your source tree, to replace
+* edit `setup.cfg` and `pyproject.toml`, if necessary,
+  to include any new configuration settings indicated by the release notes.
+  See [UPGRADING](./UPGRADING.md) for details.
+* re-run `versioneer install --[no-]vendor` in your source tree, to replace
   `SRC/_version.py`
 * commit any changed files
 
 ## Future Directions
 
 This tool is designed to make it easily extended to other version-control
 systems: all VCS-specific components are in separate directories like
@@ -257,195 +275,263 @@
 will take a VCS name as an argument, and will construct a version of
 `versioneer.py` that is specific to the given VCS. It might also take the
 configuration arguments that are currently provided manually during
 installation by editing setup.py . Alternatively, it might go the other
 direction and include code from all supported VCS systems, reducing the
 number of intermediate scripts.
 
+## Similar projects
+
+* [setuptools_scm](https://github.com/pypa/setuptools_scm/) - a non-vendored build-time
+  dependency
+* [minver](https://github.com/jbweston/miniver) - a lightweight reimplementation of
+  versioneer
+* [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
+  plugin
 
 ## License
 
 To make Versioneer easier to embed, all its code is dedicated to the public
 domain. The `_version.py` that it creates is also in the public domain.
-Specifically, both are released under the Creative Commons "Public Domain
-Dedication" license (CC0-1.0), as described in
-https://creativecommons.org/publicdomain/zero/1.0/ .
+Specifically, both are released under the "Unlicense", as described in
+https://unlicense.org/.
 
 [pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
 [pypi-url]: https://pypi.python.org/pypi/versioneer/
 [travis-image]:
-https://img.shields.io/travis/warner/python-versioneer/master.svg
-[travis-url]: https://travis-ci.org/warner/python-versioneer
+https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
+[travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
 
 """
+# pylint:disable=invalid-name,import-outside-toplevel,missing-function-docstring
+# pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
+# pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
+# pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
+# pylint:disable=attribute-defined-outside-init,too-many-arguments
 
-from __future__ import print_function
-
-try:
-    import configparser
-except ImportError:
-    import ConfigParser as configparser
-
+import configparser
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
+from pathlib import Path
+from typing import Any, Callable, cast, Dict, List, Optional, Tuple, Union
+from typing import NoReturn
+import functools
+
+have_tomllib = True
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    try:
+        import tomli as tomllib
+    except ImportError:
+        have_tomllib = False
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
+    VCS: str
+    style: str
+    tag_prefix: str
+    versionfile_source: str
+    versionfile_build: Optional[str]
+    parentdir_prefix: Optional[str]
+    verbose: Optional[bool]
+
 
-def get_root():
+def get_root() -> str:
     """Get the project root directory.
 
     We require that all commands are run from the project root, i.e. the
     directory that contains setup.py, setup.cfg, and versioneer.py .
     """
     root = os.path.realpath(os.path.abspath(os.getcwd()))
     setup_py = os.path.join(root, "setup.py")
+    pyproject_toml = os.path.join(root, "pyproject.toml")
     versioneer_py = os.path.join(root, "versioneer.py")
-    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
+    if not (
+        os.path.exists(setup_py)
+        or os.path.exists(pyproject_toml)
+        or os.path.exists(versioneer_py)
+    ):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
+        pyproject_toml = os.path.join(root, "pyproject.toml")
         versioneer_py = os.path.join(root, "versioneer.py")
-    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
+    if not (
+        os.path.exists(setup_py)
+        or os.path.exists(pyproject_toml)
+        or os.path.exists(versioneer_py)
+    ):
         err = ("Versioneer was unable to run the project root directory. "
                "Versioneer requires setup.py to be executed from "
                "its immediate directory (like 'python setup.py COMMAND'), "
                "or in a way that lets it use sys.argv[0] to find the root "
                "(like 'python path/to/setup.py COMMAND').")
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
-        me = os.path.realpath(os.path.abspath(__file__))
-        me_dir = os.path.normcase(os.path.splitext(me)[0])
+        my_path = os.path.realpath(os.path.abspath(__file__))
+        me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
-        if me_dir != vsr_dir:
+        if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
             print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(me), versioneer_py))
+                  % (os.path.dirname(my_path), versioneer_py))
     except NameError:
         pass
     return root
 
 
-def get_config_from_root(root):
+def get_config_from_root(root: str) -> VersioneerConfig:
     """Read the project setup.cfg file to determine Versioneer config."""
-    # This might raise EnvironmentError (if setup.cfg is missing), or
+    # This might raise OSError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
-    setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.SafeConfigParser()
-    with open(setup_cfg, "r") as f:
-        parser.readfp(f)
-    VCS = parser.get("versioneer", "VCS")  # mandatory
-
-    def get(parser, name):
-        if parser.has_option("versioneer", name):
-            return parser.get("versioneer", name)
-        return None
+    root_pth = Path(root)
+    pyproject_toml = root_pth / "pyproject.toml"
+    setup_cfg = root_pth / "setup.cfg"
+    section: Union[Dict[str, Any], configparser.SectionProxy, None] = None
+    if pyproject_toml.exists() and have_tomllib:
+        try:
+            with open(pyproject_toml, 'rb') as fobj:
+                pp = tomllib.load(fobj)
+            section = pp['tool']['versioneer']
+        except (tomllib.TOMLDecodeError, KeyError) as e:
+            print(f"Failed to load config from {pyproject_toml}: {e}")
+            print("Try to load it from setup.cfg")
+    if not section:
+        parser = configparser.ConfigParser()
+        with open(setup_cfg) as cfg_file:
+            parser.read_file(cfg_file)
+        parser.get("versioneer", "VCS")  # raise error if missing
+
+        section = parser["versioneer"]
+
+    # `cast`` really shouldn't be used, but its simplest for the
+    # common VersioneerConfig users at the moment. We verify against
+    # `None` values elsewhere where it matters
+
     cfg = VersioneerConfig()
-    cfg.VCS = VCS
-    cfg.style = get(parser, "style") or ""
-    cfg.versionfile_source = get(parser, "versionfile_source")
-    cfg.versionfile_build = get(parser, "versionfile_build")
-    cfg.tag_prefix = get(parser, "tag_prefix")
-    if cfg.tag_prefix in ("''", '""'):
+    cfg.VCS = section['VCS']
+    cfg.style = section.get("style", "")
+    cfg.versionfile_source = cast(str, section.get("versionfile_source"))
+    cfg.versionfile_build = section.get("versionfile_build")
+    cfg.tag_prefix = cast(str, section.get("tag_prefix"))
+    if cfg.tag_prefix in ("''", '""', None):
         cfg.tag_prefix = ""
-    cfg.parentdir_prefix = get(parser, "parentdir_prefix")
-    cfg.verbose = get(parser, "verbose")
+    cfg.parentdir_prefix = section.get("parentdir_prefix")
+    if isinstance(section, configparser.SectionProxy):
+        # Make sure configparser translates to bool
+        cfg.verbose = section.getboolean("verbose")
+    else:
+        cfg.verbose = section.get("verbose")
+
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
 # these dictionaries contain VCS-specific tools
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
-def register_vcs_handler(vcs, method):  # decorator
+def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
-    def decorate(f):
+    def decorate(f: Callable) -> Callable:
         """Store f in HANDLERS[vcs][method]."""
-        if vcs not in HANDLERS:
-            HANDLERS[vcs] = {}
-        HANDLERS[vcs][method] = f
+        HANDLERS.setdefault(vcs, {})[method] = f
         return f
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(
+    commands: List[str],
+    args: List[str],
+    cwd: Optional[str] = None,
+    verbose: bool = False,
+    hide_stderr: bool = False,
+    env: Optional[Dict[str, str]] = None,
+) -> Tuple[Optional[str], Optional[int]]:
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs: Dict[str, Any] = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
+                                       stdout=subprocess.PIPE,
+                                       stderr=(subprocess.PIPE if hide_stderr
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
-            e = sys.exc_info()[1]
+        except OSError as e:
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %s" % (commands,))
         return None, None
-    stdout = p.communicate()[0].strip()
-    if sys.version_info[0] >= 3:
-        stdout = stdout.decode()
-    if p.returncode != 0:
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
-        return None, p.returncode
-    return stdout, p.returncode
+        return None, process.returncode
+    return stdout, process.returncode
 
 
-LONG_VERSION_PY['git'] = '''
+LONG_VERSION_PY['git'] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain. Generated by
-# versioneer-0.18 (https://github.com/warner/python-versioneer)
+# This file is released into the public domain.
+# Generated by versioneer-0.29
+# https://github.com/python-versioneer/python-versioneer
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
 import sys
+from typing import Any, Callable, Dict, List, Optional, Tuple
+import functools
 
 
-def get_keywords():
+def get_keywords() -> Dict[str, str]:
     """Get the keywords needed to look up the version information."""
     # these strings will be replaced by git during git-archive.
     # setup.py/versioneer.py will grep for the variable names, so they must
     # each be defined on a line of their own. _version.py will just call
     # get_keywords().
     git_refnames = "%(DOLLAR)sFormat:%%d%(DOLLAR)s"
     git_full = "%(DOLLAR)sFormat:%%H%(DOLLAR)s"
@@ -453,16 +539,23 @@
     keywords = {"refnames": git_refnames, "full": git_full, "date": git_date}
     return keywords
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
+    VCS: str
+    style: str
+    tag_prefix: str
+    parentdir_prefix: str
+    versionfile_source: str
+    verbose: bool
+
 
-def get_config():
+def get_config() -> VersioneerConfig:
     """Create, populate and return the VersioneerConfig() object."""
     # these strings are filled in when 'setup.py versioneer' creates
     # _version.py
     cfg = VersioneerConfig()
     cfg.VCS = "git"
     cfg.style = "%(STYLE)s"
     cfg.tag_prefix = "%(TAG_PREFIX)s"
@@ -472,161 +565,187 @@
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
-def register_vcs_handler(vcs, method):  # decorator
+def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
-    def decorate(f):
+    def decorate(f: Callable) -> Callable:
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(
+    commands: List[str],
+    args: List[str],
+    cwd: Optional[str] = None,
+    verbose: bool = False,
+    hide_stderr: bool = False,
+    env: Optional[Dict[str, str]] = None,
+) -> Tuple[Optional[str], Optional[int]]:
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs: Dict[str, Any] = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
+                                       stdout=subprocess.PIPE,
+                                       stderr=(subprocess.PIPE if hide_stderr
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
-            e = sys.exc_info()[1]
+        except OSError as e:
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %%s" %% dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %%s" %% (commands,))
         return None, None
-    stdout = p.communicate()[0].strip()
-    if sys.version_info[0] >= 3:
-        stdout = stdout.decode()
-    if p.returncode != 0:
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
         if verbose:
             print("unable to run %%s (error)" %% dispcmd)
             print("stdout was %%s" %% stdout)
-        return None, p.returncode
-    return stdout, p.returncode
+        return None, process.returncode
+    return stdout, process.returncode
 
 
-def versions_from_parentdir(parentdir_prefix, root, verbose):
+def versions_from_parentdir(
+    parentdir_prefix: str,
+    root: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for i in range(3):
+    for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        else:
-            rootdirs.append(root)
-            root = os.path.dirname(root)  # up a level
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %%s but none started with prefix %%s" %%
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs):
+def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords = {}
+    keywords: Dict[str, str] = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-            if line.strip().startswith("git_date ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["date"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(keywords, tag_prefix, verbose):
+def git_versions_from_keywords(
+    keywords: Dict[str, str],
+    tag_prefix: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
         # git-2.2.0 added "%%cI", which expands to an ISO-8601 -compliant
         # datestamp. However we prefer "%%ci" (which expands to an "ISO-8601
         # -like" string, which we must then edit to make compliant), because
         # it's been around since git-1.5.3, and it's too difficult to
         # discover which version we're using, or to work around using an
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %%d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = {r for r in refs if re.search(r'\d', r)}
         if verbose:
             print("discarding '%%s', no digits" %% ",".join(refs - tags))
     if verbose:
         print("likely tags: %%s" %% ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r'\d', r):
+                continue
             if verbose:
                 print("picking %%s" %% r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -634,52 +753,97 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(
+    tag_prefix: str,
+    root: str,
+    verbose: bool,
+    runner: Callable = run_command
+) -> Dict[str, Any]:
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %%s not under git control" %% root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%%s*" %% tag_prefix],
-                                   cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces = {}
+    pieces: Dict[str, Any] = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+                             cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -688,15 +852,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%%s'"
                                %% describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -713,34 +877,35 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def plus_or_dot(pieces):
+def plus_or_dot(pieces: Dict[str, Any]) -> str:
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces):
+def render_pep440(pieces: Dict[str, Any]) -> str:
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -757,31 +922,79 @@
         rendered = "0+untagged.%%d.g%%s" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%%d.g%%s" %% (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%%d.g%%s" %% (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces: Dict[str, Any]) -> str:
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post.dev%%d" %% pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%%d.dev%%d" %% (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%%d" %% (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
-        rendered = "0.post.dev%%d" %% pieces["distance"]
+        rendered = "0.post0.dev%%d" %% pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces):
+def render_pep440_post(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -800,15 +1013,44 @@
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%%s" %% pieces["short"]
     return rendered
 
 
-def render_pep440_old(pieces):
+def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%%d" %% pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%%s" %% pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%%d" %% pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%%s" %% pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def render_pep440_old(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
@@ -822,15 +1064,15 @@
         # exception #1
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces):
+def render_git_describe(pieces: Dict[str, Any]) -> str:
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -842,15 +1084,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces):
+def render_git_describe_long(pieces: Dict[str, Any]) -> str:
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -862,47 +1104,51 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces, style):
+def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {"version": "unknown",
                 "full-revisionid": pieces.get("long"),
                 "dirty": None,
                 "error": pieces["error"],
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%%s'" %% style)
 
     return {"version": rendered, "full-revisionid": pieces["long"],
             "dirty": pieces["dirty"], "error": None,
             "date": pieces.get("date")}
 
 
-def get_versions():
+def get_versions() -> Dict[str, Any]:
     """Get version information or return default if unable to do so."""
     # I am in _version.py, which lives at ROOT/VERSIONFILE_SOURCE. If we have
     # __file__, we can work backwards from there to the root. Some
     # py2exe/bbfreeze/non-CPython implementations don't do __file__, in which
     # case we can only use expanded keywords.
 
     cfg = get_config()
@@ -915,15 +1161,15 @@
         pass
 
     try:
         root = os.path.realpath(__file__)
         # versionfile_source is the relative path from the top of the source
         # tree (where the .git directory might live) to this file. Invert
         # this to find the root from __file__.
-        for i in cfg.versionfile_source.split('/'):
+        for _ in cfg.versionfile_source.split('/'):
             root = os.path.dirname(root)
     except NameError:
         return {"version": "0+unknown", "full-revisionid": None,
                 "dirty": None,
                 "error": "unable to find root of source tree",
                 "date": None}
 
@@ -942,83 +1188,95 @@
     return {"version": "0+unknown", "full-revisionid": None,
             "dirty": None,
             "error": "unable to compute version", "date": None}
 '''
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs):
+def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords = {}
+    keywords: Dict[str, str] = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-            if line.strip().startswith("git_date ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["date"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(keywords, tag_prefix, verbose):
+def git_versions_from_keywords(
+    keywords: Dict[str, str],
+    tag_prefix: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
         # git-2.2.0 added "%cI", which expands to an ISO-8601 -compliant
         # datestamp. However we prefer "%ci" (which expands to an "ISO-8601
         # -like" string, which we must then edit to make compliant), because
         # it's been around since git-1.5.3, and it's too difficult to
         # discover which version we're using, or to work around using an
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = {r for r in refs if re.search(r'\d', r)}
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r'\d', r):
+                continue
             if verbose:
                 print("picking %s" % r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -1026,52 +1284,97 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(
+    tag_prefix: str,
+    root: str,
+    verbose: bool,
+    runner: Callable = run_command
+) -> Dict[str, Any]:
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%s*" % tag_prefix],
-                                   cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces = {}
+    pieces: Dict[str, Any] = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+                             cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -1080,15 +1383,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%s'"
                                % describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -1105,144 +1408,146 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def do_vcs_install(manifest_in, versionfile_source, ipy):
+def do_vcs_install(versionfile_source: str, ipy: Optional[str]) -> None:
     """Git-specific installation logic for Versioneer.
 
     For Git, this means creating/changing .gitattributes to mark _version.py
     for export-subst keyword substitution.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-    files = [manifest_in, versionfile_source]
+    files = [versionfile_source]
     if ipy:
         files.append(ipy)
-    try:
-        me = __file__
-        if me.endswith(".pyc") or me.endswith(".pyo"):
-            me = os.path.splitext(me)[0] + ".py"
-        versioneer_file = os.path.relpath(me)
-    except NameError:
-        versioneer_file = "versioneer.py"
-    files.append(versioneer_file)
+    if "VERSIONEER_PEP518" not in globals():
+        try:
+            my_path = __file__
+            if my_path.endswith((".pyc", ".pyo")):
+                my_path = os.path.splitext(my_path)[0] + ".py"
+            versioneer_file = os.path.relpath(my_path)
+        except NameError:
+            versioneer_file = "versioneer.py"
+        files.append(versioneer_file)
     present = False
     try:
-        f = open(".gitattributes", "r")
-        for line in f.readlines():
-            if line.strip().startswith(versionfile_source):
-                if "export-subst" in line.strip().split()[1:]:
-                    present = True
-        f.close()
-    except EnvironmentError:
+        with open(".gitattributes", "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith(versionfile_source):
+                    if "export-subst" in line.strip().split()[1:]:
+                        present = True
+                        break
+    except OSError:
         pass
     if not present:
-        f = open(".gitattributes", "a+")
-        f.write("%s export-subst\n" % versionfile_source)
-        f.close()
+        with open(".gitattributes", "a+") as fobj:
+            fobj.write(f"{versionfile_source} export-subst\n")
         files.append(".gitattributes")
     run_command(GITS, ["add", "--"] + files)
 
 
-def versions_from_parentdir(parentdir_prefix, root, verbose):
+def versions_from_parentdir(
+    parentdir_prefix: str,
+    root: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for i in range(3):
+    for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        else:
-            rootdirs.append(root)
-            root = os.path.dirname(root)  # up a level
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %s but none started with prefix %s" %
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.18) from
+# This file was generated by 'versioneer.py' (0.29) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
-from __future__ import absolute_import
 import json
 
 version_json = '''
 %s
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
 """
 
 
-def versions_from_file(filename):
+def versions_from_file(filename: str) -> Dict[str, Any]:
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
-    except EnvironmentError:
+    except OSError:
         raise NotThisMethod("unable to read _version.py")
     mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
                    contents, re.M | re.S)
     if not mo:
         mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
                        contents, re.M | re.S)
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
-def write_to_version_file(filename, versions):
+def write_to_version_file(filename: str, versions: Dict[str, Any]) -> None:
     """Write the given version number to the given _version.py file."""
-    os.unlink(filename)
     contents = json.dumps(versions, sort_keys=True,
                           indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
-def plus_or_dot(pieces):
+def plus_or_dot(pieces: Dict[str, Any]) -> str:
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces):
+def render_pep440(pieces: Dict[str, Any]) -> str:
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -1259,31 +1564,79 @@
         rendered = "0+untagged.%d.g%s" % (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%d.g%s" % (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces: Dict[str, Any]) -> str:
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post.dev%d" % pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%d" % (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
-        rendered = "0.post.dev%d" % pieces["distance"]
+        rendered = "0.post0.dev%d" % pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces):
+def render_pep440_post(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -1302,15 +1655,44 @@
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%s" % pieces["short"]
     return rendered
 
 
-def render_pep440_old(pieces):
+def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%d" % pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%s" % pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%d" % pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%s" % pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def render_pep440_old(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
@@ -1324,15 +1706,15 @@
         # exception #1
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces):
+def render_git_describe(pieces: Dict[str, Any]) -> str:
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -1344,15 +1726,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces):
+def render_git_describe_long(pieces: Dict[str, Any]) -> str:
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -1364,32 +1746,36 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces, style):
+def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {"version": "unknown",
                 "full-revisionid": pieces.get("long"),
                 "dirty": None,
                 "error": pieces["error"],
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
@@ -1400,30 +1786,30 @@
             "date": pieces.get("date")}
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
-def get_versions(verbose=False):
+def get_versions(verbose: bool = False) -> Dict[str, Any]:
     """Get the project version from whatever source is available.
 
     Returns dict with two keys: 'version' and 'full'.
     """
     if "versioneer" in sys.modules:
         # see the discussion in cmdclass.py:get_cmdclass()
         del sys.modules["versioneer"]
 
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
-    verbose = verbose or cfg.verbose
+    verbose = verbose or bool(cfg.verbose)  # `bool()` used to avoid `None`
     assert cfg.versionfile_source is not None, \
         "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
@@ -1476,21 +1862,21 @@
         print("unable to compute version")
 
     return {"version": "0+unknown", "full-revisionid": None,
             "dirty": None, "error": "unable to compute version",
             "date": None}
 
 
-def get_version():
+def get_version() -> str:
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
-def get_cmdclass(cmdclass=None):
-    """Get the custom setuptools/distutils subclasses used by Versioneer.
+def get_cmdclass(cmdclass: Optional[Dict[str, Any]] = None):
+    """Get the custom setuptools subclasses used by Versioneer.
 
     If the package uses a different cmdclass (e.g. one from numpy), it
     should be provide as an argument.
     """
     if "versioneer" in sys.modules:
         del sys.modules["versioneer"]
         # this fixes the "python setup.py develop" case (also 'install' and
@@ -1500,92 +1886,128 @@
         # of Versioneer. A's setup.py imports A's Versioneer, leaving it in
         # sys.modules by the time B's setup.py is executed, causing B to run
         # with the wrong versioneer. Setuptools wraps the sub-dep builds in a
         # sandbox that restores sys.modules to it's pre-build state, so the
         # parent is protected against the child's "import versioneer". By
         # removing ourselves from sys.modules here, before the child build
         # happens, we protect the child from the parent's versioneer too.
-        # Also see https://github.com/warner/python-versioneer/issues/52
+        # Also see https://github.com/python-versioneer/python-versioneer/issues/52
 
     cmds = {} if cmdclass is None else cmdclass.copy()
 
-    # we add "version" to both distutils and setuptools
-    from distutils.core import Command
+    # we add "version" to setuptools
+    from setuptools import Command
 
     class cmd_version(Command):
         description = "report generated version string"
-        user_options = []
-        boolean_options = []
+        user_options: List[Tuple[str, str, str]] = []
+        boolean_options: List[str] = []
 
-        def initialize_options(self):
+        def initialize_options(self) -> None:
             pass
 
-        def finalize_options(self):
+        def finalize_options(self) -> None:
             pass
 
-        def run(self):
+        def run(self) -> None:
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
     cmds["version"] = cmd_version
 
-    # we override "build_py" in both distutils and setuptools
+    # we override "build_py" in setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
     #  setuptools/bdist_wheel -> distutils/install ->..
     #  setuptools/bdist_egg -> distutils/install_lib -> build_py
     #  setuptools/install -> bdist_egg ->..
     #  setuptools/develop -> ?
     #  pip install:
     #   copies source tree to a tempdir before running egg_info/etc
     #   if .git isn't copied too, 'git describe' will fail
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
+    # pip install -e . and setuptool/editable_wheel will invoke build_py
+    # but the build_py command is not expected to copy any files.
+
     # we override different "build_py" commands for both environments
     if 'build_py' in cmds:
-        _build_py = cmds['build_py']
-    elif "setuptools" in sys.modules:
-        from setuptools.command.build_py import build_py as _build_py
+        _build_py: Any = cmds['build_py']
     else:
-        from distutils.command.build_py import build_py as _build_py
+        from setuptools.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
-        def run(self):
+        def run(self) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
+            if getattr(self, "editable_mode", False):
+                # During editable installs `.py` and data files are
+                # not copied to build_lib
+                return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
                 target_versionfile = os.path.join(self.build_lib,
                                                   cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
     cmds["build_py"] = cmd_build_py
 
-    if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
-        from cx_Freeze.dist import build_exe as _build_exe
+    if 'build_ext' in cmds:
+        _build_ext: Any = cmds['build_ext']
+    else:
+        from setuptools.command.build_ext import build_ext as _build_ext
+
+    class cmd_build_ext(_build_ext):
+        def run(self) -> None:
+            root = get_root()
+            cfg = get_config_from_root(root)
+            versions = get_versions()
+            _build_ext.run(self)
+            if self.inplace:
+                # build_ext --inplace will only build extensions in
+                # build/lib<..> dir with no _version.py to write to.
+                # As in place builds will already have a _version.py
+                # in the module dir, we do not need to write one.
+                return
+            # now locate _version.py in the new build/ directory and replace
+            # it with an updated value
+            if not cfg.versionfile_build:
+                return
+            target_versionfile = os.path.join(self.build_lib,
+                                              cfg.versionfile_build)
+            if not os.path.exists(target_versionfile):
+                print(f"Warning: {target_versionfile} does not exist, skipping "
+                      "version update. This can happen if you are running build_ext "
+                      "without first running build_py.")
+                return
+            print("UPDATING %s" % target_versionfile)
+            write_to_version_file(target_versionfile, versions)
+    cmds["build_ext"] = cmd_build_ext
 
+    if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
+        from cx_Freeze.dist import build_exe as _build_exe  # type: ignore
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
         class cmd_build_exe(_build_exe):
-            def run(self):
+            def run(self) -> None:
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
@@ -1601,20 +2023,20 @@
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
     if 'py2exe' in sys.modules:  # py2exe enabled?
         try:
-            from py2exe.distutils_buildexe import py2exe as _py2exe  # py3
+            from py2exe.setuptools_buildexe import py2exe as _py2exe  # type: ignore
         except ImportError:
-            from py2exe.build_exe import py2exe as _py2exe  # py2
+            from py2exe.distutils_buildexe import py2exe as _py2exe  # type: ignore
 
         class cmd_py2exe(_py2exe):
-            def run(self):
+            def run(self) -> None:
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
@@ -1627,32 +2049,67 @@
                              "STYLE": cfg.style,
                              "TAG_PREFIX": cfg.tag_prefix,
                              "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["py2exe"] = cmd_py2exe
 
+    # sdist farms its file list building out to egg_info
+    if 'egg_info' in cmds:
+        _egg_info: Any = cmds['egg_info']
+    else:
+        from setuptools.command.egg_info import egg_info as _egg_info
+
+    class cmd_egg_info(_egg_info):
+        def find_sources(self) -> None:
+            # egg_info.find_sources builds the manifest list and writes it
+            # in one shot
+            super().find_sources()
+
+            # Modify the filelist and normalize it
+            root = get_root()
+            cfg = get_config_from_root(root)
+            self.filelist.append('versioneer.py')
+            if cfg.versionfile_source:
+                # There are rare cases where versionfile_source might not be
+                # included by default, so we must be explicit
+                self.filelist.append(cfg.versionfile_source)
+            self.filelist.sort()
+            self.filelist.remove_duplicates()
+
+            # The write method is hidden in the manifest_maker instance that
+            # generated the filelist and was thrown away
+            # We will instead replicate their final normalization (to unicode,
+            # and POSIX-style paths)
+            from setuptools import unicode_utils
+            normalized = [unicode_utils.filesys_decode(f).replace(os.sep, '/')
+                          for f in self.filelist.files]
+
+            manifest_filename = os.path.join(self.egg_info, 'SOURCES.txt')
+            with open(manifest_filename, 'w') as fobj:
+                fobj.write('\n'.join(normalized))
+
+    cmds['egg_info'] = cmd_egg_info
+
     # we override different "sdist" commands for both environments
     if 'sdist' in cmds:
-        _sdist = cmds['sdist']
-    elif "setuptools" in sys.modules:
-        from setuptools.command.sdist import sdist as _sdist
+        _sdist: Any = cmds['sdist']
     else:
-        from distutils.command.sdist import sdist as _sdist
+        from setuptools.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
-        def run(self):
+        def run(self) -> None:
             versions = get_versions()
             self._versioneer_generated_versions = versions
             # unless we update this, the command will keep using the old
             # version
             self.distribution.metadata.version = versions["version"]
             return _sdist.run(self)
 
-        def make_release_tree(self, base_dir, files):
+        def make_release_tree(self, base_dir: str, files: List[str]) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
@@ -1697,29 +2154,34 @@
 #versionfile_source =
 #versionfile_build =
 #tag_prefix =
 #parentdir_prefix =
 
 """
 
-INIT_PY_SNIPPET = """
+OLD_SNIPPET = """
 from ._version import get_versions
 __version__ = get_versions()['version']
 del get_versions
 """
 
+INIT_PY_SNIPPET = """
+from . import {0}
+__version__ = {0}.get_versions()['version']
+"""
 
-def do_setup():
+
+def do_setup() -> int:
     """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (EnvironmentError, configparser.NoSectionError,
+    except (OSError, configparser.NoSectionError,
             configparser.NoOptionError) as e:
-        if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
+        if isinstance(e, (OSError, configparser.NoSectionError)):
             print("Adding sample versioneer config to setup.cfg",
                   file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
@@ -1731,70 +2193,45 @@
                         "TAG_PREFIX": cfg.tag_prefix,
                         "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                         "VERSIONFILE_SOURCE": cfg.versionfile_source,
                         })
 
     ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
                        "__init__.py")
+    maybe_ipy: Optional[str] = ipy
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
-        except EnvironmentError:
+        except OSError:
             old = ""
-        if INIT_PY_SNIPPET not in old:
+        module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
+        snippet = INIT_PY_SNIPPET.format(module)
+        if OLD_SNIPPET in old:
+            print(" replacing boilerplate in %s" % ipy)
+            with open(ipy, "w") as f:
+                f.write(old.replace(OLD_SNIPPET, snippet))
+        elif snippet not in old:
             print(" appending to %s" % ipy)
             with open(ipy, "a") as f:
-                f.write(INIT_PY_SNIPPET)
+                f.write(snippet)
         else:
             print(" %s unmodified" % ipy)
     else:
         print(" %s doesn't exist, ok" % ipy)
-        ipy = None
-
-    # Make sure both the top-level "versioneer.py" and versionfile_source
-    # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
-    # they'll be copied into source distributions. Pip won't be able to
-    # install the package without this.
-    manifest_in = os.path.join(root, "MANIFEST.in")
-    simple_includes = set()
-    try:
-        with open(manifest_in, "r") as f:
-            for line in f:
-                if line.startswith("include "):
-                    for include in line.split()[1:]:
-                        simple_includes.add(include)
-    except EnvironmentError:
-        pass
-    # That doesn't cover everything MANIFEST.in can do
-    # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
-    # it might give some false negatives. Appending redundant 'include'
-    # lines is safe, though.
-    if "versioneer.py" not in simple_includes:
-        print(" appending 'versioneer.py' to MANIFEST.in")
-        with open(manifest_in, "a") as f:
-            f.write("include versioneer.py\n")
-    else:
-        print(" 'versioneer.py' already in MANIFEST.in")
-    if cfg.versionfile_source not in simple_includes:
-        print(" appending versionfile_source ('%s') to MANIFEST.in" %
-              cfg.versionfile_source)
-        with open(manifest_in, "a") as f:
-            f.write("include %s\n" % cfg.versionfile_source)
-    else:
-        print(" versionfile_source already in MANIFEST.in")
+        maybe_ipy = None
 
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
     # substitution.
-    do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
+    do_vcs_install(cfg.versionfile_source, maybe_ipy)
     return 0
 
 
-def scan_setup_py():
+def scan_setup_py() -> int:
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
     errors = 0
     with open("setup.py", "r") as f:
         for line in f.readlines():
             if "import versioneer" in line:
@@ -1823,14 +2260,18 @@
         print("'versioneer.versionfile_source = ' . This configuration")
         print("now lives in setup.cfg, and should be removed from setup.py")
         print("")
         errors += 1
     return errors
 
 
+def setup_command() -> NoReturn:
+    """Set up Versioneer and exit with appropriate error code."""
+    errors = do_setup()
+    errors += scan_setup_py()
+    sys.exit(1 if errors else 0)
+
+
 if __name__ == "__main__":
     cmd = sys.argv[1]
     if cmd == "setup":
-        errors = do_setup()
-        errors += scan_setup_py()
-        if errors:
-            sys.exit(1)
+        setup_command()
```


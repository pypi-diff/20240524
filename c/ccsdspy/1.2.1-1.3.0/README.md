# Comparing `tmp/ccsdspy-1.2.1.tar.gz` & `tmp/ccsdspy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccsdspy-1.2.1.tar", last modified: Sun Nov 26 10:25:28 2023, max compression
+gzip compressed data, was "ccsdspy-1.3.0.tar", last modified: Fri May 24 05:19:51 2024, max compression
```

## Comparing `ccsdspy-1.2.1.tar` & `ccsdspy-1.3.0.tar`

### file list

```diff
@@ -1,200 +1,241 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:28.535902 ccsdspy-1.2.1/
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:27.304902 ccsdspy-1.2.1/.github/
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:27.340903 ccsdspy-1.2.1/.github/workflows/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1077 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/.github/workflows/ccsdspy-ci.yml
--rw-r--r--   0 daniel    (1000) daniel    (1000)      803 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/.github/workflows/doc-build.yml
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1237 2023-02-04 03:42:21.000000 ccsdspy-1.2.1/.gitignore
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3585 2023-11-26 10:19:19.000000 ccsdspy-1.2.1/CHANGELOG.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1490 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/LICENSE.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7083 2023-11-26 10:25:28.535902 ccsdspy-1.2.1/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4005 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/README.rst
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:27.408904 ccsdspy-1.2.1/ccsdspy/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      526 2023-03-18 05:21:40.000000 ccsdspy-1.2.1/ccsdspy/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1703 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/__main__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      411 2023-11-26 10:25:27.000000 ccsdspy-1.2.1/ccsdspy/_version.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      166 2023-03-17 22:28:24.000000 ccsdspy-1.2.1/ccsdspy/constants.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    12846 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/ccsdspy/converters.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    20866 2023-11-23 22:57:30.000000 ccsdspy-1.2.1/ccsdspy/decode.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6541 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/ccsdspy/packet_fields.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    24280 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/ccsdspy/packet_types.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:27.500905 ccsdspy-1.2.1/ccsdspy/tests/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/__init__.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:27.309903 ccsdspy-1.2.1/ccsdspy/tests/data/
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:27.518902 ccsdspy-1.2.1/ccsdspy/tests/data/csa/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   502824 2023-11-23 14:46:10.000000 ccsdspy-1.2.1/ccsdspy/tests/data/csa/apid00400.tlm
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:27.593906 ccsdspy-1.2.1/ccsdspy/tests/data/europa_clipper/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   154816 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/ccsdspy/tests/data/europa_clipper/apid01216.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)      128 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/ccsdspy/tests/data/europa_clipper/apid01217.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)    33176 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/ccsdspy/tests/data/europa_clipper/apid01219.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)    33176 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/ccsdspy/tests/data/europa_clipper/apid01223.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)    33176 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/ccsdspy/tests/data/europa_clipper/apid01227.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)      540 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/ccsdspy/tests/data/europa_clipper/apid01232.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)   255012 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/ccsdspy/tests/data/europa_clipper/ecm_raw2.bin
--rw-r--r--   0 daniel    (1000) daniel    (1000)    33176 2023-11-23 22:05:09.000000 ccsdspy-1.2.1/ccsdspy/tests/data/europa_clipper/expanding_footer_packet.bin
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:27.599902 ccsdspy-1.2.1/ccsdspy/tests/data/hs/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      232 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/hs/README.rst
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:27.631902 ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid001/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    73848 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid001/SSAT1_2015-180-00-00-00_2015-180-01-59-58_1_1_sim.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)      727 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid001/defs.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:27.644906 ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid010/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   179163 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid010/SSAT1_2015-180-00-00-00_2015-180-00-59-59_10_1_sim.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1524 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid010/defs.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:27.660905 ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid035/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   367200 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid035/SSAT1_2015-180-00-00-00_2015-180-01-59-59_35_1_sim.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1159 2023-03-17 22:28:24.000000 ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid035/defs.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:27.675902 ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid130/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   559689 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid130/SSAT1_2015-180-00-00-00_2015-180-01-59-35_130_1_sim.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)      390 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid130/defs.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:27.691906 ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid251/
--rw-r--r--   0 daniel    (1000) daniel    (1000)  1008000 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid251/SSAT1_2015-180-00-00-00_2015-180-01-59-59_251_1_sim.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)      422 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid251/defs.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:27.714907 ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid895/
--rw-r--r--   0 daniel    (1000) daniel    (1000)  2446980 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid895/SSAT1_2015-180-00-00-00_2015-180-01-59-56_895_1_sim.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)      440 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid895/defs.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:27.729903 ccsdspy-1.2.1/ccsdspy/tests/data/hs/attic/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    17668 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/hs/attic/SSAT_Mnemonics.csv
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2116 2023-03-17 22:28:25.000000 ccsdspy-1.2.1/ccsdspy/tests/data/hs/attic/_expand_mnemnonics.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:27.752904 ccsdspy-1.2.1/ccsdspy/tests/data/packet_def/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      111 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/packet_def/simple_csv_3col.csv
--rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/packet_def/simple_csv_3col_with_array.csv
--rw-r--r--   0 daniel    (1000) daniel    (1000)      142 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/packet_def/simple_csv_4col.csv
--rw-r--r--   0 daniel    (1000) daniel    (1000)      149 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/packet_def/simple_csv_4col_with_array.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:27.808906 ccsdspy-1.2.1/ccsdspy/tests/data/split/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    14820 2023-03-17 22:28:25.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/CYGNSS_F7_L0_2022_086_10_15_V01_F__first101pkts.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1040 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/apid00384.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)      416 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/apid00386.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1680 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/apid00391.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)      672 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/apid00392.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5600 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/apid00393.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2964 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/apid00394.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2448 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/apid01313.tlm
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:28.271904 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1443 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/Conventions.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2025 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_INP.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2024 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_OUT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2028 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_TLM.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2334 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_ACK.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3181 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_AD_RESP.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2954 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_AUTOLOAD.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3169 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_ERASEFLASH.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3264 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_DUMP.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3193 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_LOAD.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11574 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_PWR.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4383 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_TRACK_STAT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4673 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_COMM_DIAG.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11049 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_CYGNSS_PKT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4339 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_DATA_LOGGER_STAT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11742 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_FRONT_END_STAT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3521 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_NAV_INFO.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     5569 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_OP_SETTINGS.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3874 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_ORBITAL_ELEMENTS.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3373 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_PPS_TABLE.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     8213 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_PROCESSED_DATA.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11728 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_PVT_INFO.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9803 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_RAW_DATA.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6597 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_CHAN_STAT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9974 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_LIST.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3052 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_STAT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2812 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4689 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM_TH.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3067 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_STATUS.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3875 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_STREAM_ROUTER_STAT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1672 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_ECHO.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2233 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_MAG_RAW.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    13104 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_NST_RAW.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     8921 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_RWA_RAW.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    14772 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_ADCS.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    10135 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_ADCSIO.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)   150107 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_BOOT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4122 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_DDMI.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1935 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_DNLD.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1662 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_DNLD_FAT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    42952 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_DNLD_FPT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9093 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_ERREVT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1562 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_FILL.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    12767 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_HI.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    28801 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_LOW.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    31990 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_LZ.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    17290 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_PASS.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3652 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_PVT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     8744 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_SSV.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)       45 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/LIMITS.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9201 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/Overview.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    24277 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/Revision History.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6540 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/SCI_DDM_BB_X8.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4905 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/SCI_DDM_X10.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     5124 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/SCI_DDM_X11.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6725 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/SCI_DDM_X8.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6856 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/SCI_FULL.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     5878 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/SCI_META.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6120 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/SCI_META_V2.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2016 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/SCI_RAW.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1384 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/SUPER_NOM.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:28.314906 ccsdspy-1.2.1/ccsdspy/tests/data/var_length/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      634 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/var_length/README.md
--rw-r--r--   0 daniel    (1000) daniel    (1000)      318 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/var_length/var_length_packets.bin
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1213 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/var_length/var_length_packets.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2015 2023-03-17 22:28:24.000000 ccsdspy-1.2.1/ccsdspy/tests/data/var_length/var_length_packets_double_varfield.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      590 2023-03-17 22:28:24.000000 ccsdspy-1.2.1/ccsdspy/tests/data/var_length/var_length_packets_double_varfield_with_footer.bin
--rw-r--r--   0 daniel    (1000) daniel    (1000)      338 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/ccsdspy/tests/data/var_length/var_length_packets_with_footer.bin
--rw-r--r--   0 daniel    (1000) daniel    (1000)    19374 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/ccsdspy/tests/test_converters.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4837 2023-03-17 22:28:24.000000 ccsdspy-1.2.1/ccsdspy/tests/test_hs.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3103 2023-02-21 04:48:16.000000 ccsdspy-1.2.1/ccsdspy/tests/test_packet_fields.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7600 2023-03-17 22:28:24.000000 ccsdspy-1.2.1/ccsdspy/tests/test_packet_types.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8837 2023-03-18 05:21:40.000000 ccsdspy-1.2.1/ccsdspy/tests/test_primary_header.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     9618 2023-11-26 10:11:30.000000 ccsdspy-1.2.1/ccsdspy/tests/test_regression.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4480 2023-03-17 22:28:24.000000 ccsdspy-1.2.1/ccsdspy/tests/test_split.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4756 2023-11-23 21:58:39.000000 ccsdspy-1.2.1/ccsdspy/tests/test_utils.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4182 2023-03-17 22:28:24.000000 ccsdspy-1.2.1/ccsdspy/tests/test_var_length.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7887 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/ccsdspy/utils.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:28.532902 ccsdspy-1.2.1/ccsdspy.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7083 2023-11-26 10:25:27.000000 ccsdspy-1.2.1/ccsdspy.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7077 2023-11-26 10:25:27.000000 ccsdspy-1.2.1/ccsdspy.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-11-26 10:25:27.000000 ccsdspy-1.2.1/ccsdspy.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)      194 2023-11-26 10:25:27.000000 ccsdspy-1.2.1/ccsdspy.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        8 2023-11-26 10:25:27.000000 ccsdspy-1.2.1/ccsdspy.egg-info/top_level.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:28.369902 ccsdspy-1.2.1/docs/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8399 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/docs/Makefile
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:28.370903 ccsdspy-1.2.1/docs/_static/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    36033 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/docs/_static/logo.png
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:28.414902 ccsdspy-1.2.1/docs/_static/used-by/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)   281290 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/docs/_static/used-by/elfin.jpg
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)  1343999 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/docs/_static/used-by/goes-r.png
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    74095 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/docs/_static/used-by/hermes.png
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)   240058 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/docs/_static/used-by/mms.jpg
--rw-r--r--   0 daniel    (1000) daniel    (1000)   644732 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/docs/_static/used-by/padre.png
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)   152642 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/docs/_static/used-by/punch.png
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)      106 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/docs/_static/used-by/resize.sh
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:28.439904 ccsdspy-1.2.1/docs/_static/used-by/small/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    16916 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/docs/_static/used-by/small/elfin.jpg
--rw-r--r--   0 daniel    (1000) daniel    (1000)    20111 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/docs/_static/used-by/small/goes-r.png
--rw-r--r--   0 daniel    (1000) daniel    (1000)    14174 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/docs/_static/used-by/small/hermes.png
--rw-r--r--   0 daniel    (1000) daniel    (1000)    41871 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/docs/_static/used-by/small/mms.jpg
--rw-r--r--   0 daniel    (1000) daniel    (1000)    14542 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/docs/_static/used-by/small/padre.png
--rw-r--r--   0 daniel    (1000) daniel    (1000)    13675 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/docs/_static/used-by/small/punch.png
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10829 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/docs/_static/used-by/small/spherex.png
--rw-r--r--   0 daniel    (1000) daniel    (1000)   102429 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/docs/_static/used-by/spherex.png
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:28.454902 ccsdspy-1.2.1/docs/_templates/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      463 2023-03-18 05:21:40.000000 ccsdspy-1.2.1/docs/_templates/github.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)       80 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/docs/_templates/logo.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      134 2023-03-18 05:21:40.000000 ccsdspy-1.2.1/docs/api.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7670 2023-03-18 05:21:40.000000 ccsdspy-1.2.1/docs/conf.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:28.463904 ccsdspy-1.2.1/docs/dev-guide/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7279 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/docs/dev-guide/index.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3247 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/docs/index.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7768 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/docs/make.bat
--rw-r--r--   0 daniel    (1000) daniel    (1000)       34 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/docs/requirements.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:28.519904 ccsdspy-1.2.1/docs/user-guide/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3409 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/docs/user-guide/ccsds.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4247 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/docs/user-guide/converters.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3253 2023-03-17 22:28:24.000000 ccsdspy-1.2.1/docs/user-guide/fixedlength.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)      243 2023-03-18 05:21:40.000000 ccsdspy-1.2.1/docs/user-guide/index.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1853 2023-03-17 22:28:24.000000 ccsdspy-1.2.1/docs/user-guide/packetfields.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4671 2023-11-23 21:58:59.000000 ccsdspy-1.2.1/docs/user-guide/utils.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3777 2023-03-17 22:28:24.000000 ccsdspy-1.2.1/docs/user-guide/variablelength.rst
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-26 10:25:28.530905 ccsdspy-1.2.1/docs/whatsnew/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       95 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/docs/whatsnew/changelog.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)      110 2023-03-18 03:52:05.000000 ccsdspy-1.2.1/docs/whatsnew/index.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2716 2023-03-17 22:28:24.000000 ccsdspy-1.2.1/pyproject.toml
--rw-r--r--   0 daniel    (1000) daniel    (1000)      542 2023-02-04 02:00:23.000000 ccsdspy-1.2.1/readthedocs.yml
--rw-r--r--   0 daniel    (1000) daniel    (1000)      162 2023-11-26 10:25:28.536903 ccsdspy-1.2.1/setup.cfg
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.906944 ccsdspy-1.3.0/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.476945 ccsdspy-1.3.0/.github/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.496443 ccsdspy-1.3.0/.github/workflows/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1077 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/.github/workflows/ccsdspy-ci.yml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      803 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/.github/workflows/doc-build.yml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1237 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/.gitignore
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4409 2024-05-24 05:16:37.000000 ccsdspy-1.3.0/CHANGELOG.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1490 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/LICENSE.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7554 2024-05-24 05:19:51.906444 ccsdspy-1.3.0/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4469 2024-05-24 05:11:16.000000 ccsdspy-1.3.0/README.rst
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.508444 ccsdspy-1.3.0/ccsdspy/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      526 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1703 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/__main__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      411 2024-05-24 05:19:50.000000 ccsdspy-1.3.0/ccsdspy/_version.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      166 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/constants.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    12846 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/converters.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    20891 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/decode.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7184 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/packet_fields.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    30012 2024-05-24 05:11:16.000000 ccsdspy-1.3.0/ccsdspy/packet_types.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.530944 ccsdspy-1.3.0/ccsdspy/tests/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/__init__.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.483944 ccsdspy-1.3.0/ccsdspy/tests/data/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.590446 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2016 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byte_order_packets.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      860 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_1.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2848 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_1.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1660 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_12.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4660 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_12.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2460 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_123.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6663 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_123.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3260 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_1234.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8619 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_1234.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4860 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_123456.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    12470 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_123456.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5660 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_1234567.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    14266 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_1234567.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6460 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_12345678.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    16334 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_12345678.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1660 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_21.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4664 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_21.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3260 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_2143.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8596 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_2143.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2460 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_321.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6647 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_321.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3260 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_3412.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8608 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_3412.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3260 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_4321.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8582 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_4321.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6460 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_78563412.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    16288 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_78563412.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6460 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_87654321.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    16316 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/data/byte_order/byteorder_87654321.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.592443 ccsdspy-1.3.0/ccsdspy/tests/data/csa/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   502824 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/csa/apid00400.tlm
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.617447 ccsdspy-1.3.0/ccsdspy/tests/data/europa_clipper/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   154816 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/europa_clipper/apid01216.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      128 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/europa_clipper/apid01217.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    33176 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/europa_clipper/apid01219.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    33176 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/europa_clipper/apid01223.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    33176 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/europa_clipper/apid01227.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      540 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/europa_clipper/apid01232.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   255012 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/europa_clipper/ecm_raw2.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    33176 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/europa_clipper/expanding_footer_packet.bin
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.619946 ccsdspy-1.3.0/ccsdspy/tests/data/hs/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      232 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/hs/README.rst
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.624446 ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid001/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    73848 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid001/SSAT1_2015-180-00-00-00_2015-180-01-59-58_1_1_sim.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      727 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid001/defs.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.631945 ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid010/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   179163 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid010/SSAT1_2015-180-00-00-00_2015-180-00-59-59_10_1_sim.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1524 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid010/defs.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.641945 ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid035/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   367200 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid035/SSAT1_2015-180-00-00-00_2015-180-01-59-59_35_1_sim.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1159 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid035/defs.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.648945 ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid130/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   559689 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid130/SSAT1_2015-180-00-00-00_2015-180-01-59-35_130_1_sim.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      390 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid130/defs.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.658445 ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid251/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)  1008000 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid251/SSAT1_2015-180-00-00-00_2015-180-01-59-59_251_1_sim.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      422 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid251/defs.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.672444 ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid895/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)  2446980 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid895/SSAT1_2015-180-00-00-00_2015-180-01-59-56_895_1_sim.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      440 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid895/defs.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.675943 ccsdspy-1.3.0/ccsdspy/tests/data/hs/attic/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    17668 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/hs/attic/SSAT_Mnemonics.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2117 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/hs/attic/_expand_mnemnonics.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.684944 ccsdspy-1.3.0/ccsdspy/tests/data/packet_def/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      111 2024-05-24 05:11:16.000000 ccsdspy-1.3.0/ccsdspy/tests/data/packet_def/basic_csv_3col.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      141 2024-05-24 05:11:16.000000 ccsdspy-1.3.0/ccsdspy/tests/data/packet_def/basic_csv_3col_with_all.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2024-05-24 05:11:16.000000 ccsdspy-1.3.0/ccsdspy/tests/data/packet_def/basic_csv_3col_with_array.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      122 2024-05-24 05:11:16.000000 ccsdspy-1.3.0/ccsdspy/tests/data/packet_def/basic_csv_3col_with_expand.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      122 2024-05-24 05:11:16.000000 ccsdspy-1.3.0/ccsdspy/tests/data/packet_def/basic_csv_3col_with_reference.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      142 2024-05-24 05:11:16.000000 ccsdspy-1.3.0/ccsdspy/tests/data/packet_def/extended_csv_4col.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      149 2024-05-24 05:11:16.000000 ccsdspy-1.3.0/ccsdspy/tests/data/packet_def/extended_csv_4col_with_array.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.697944 ccsdspy-1.3.0/ccsdspy/tests/data/split/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    14820 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/CYGNSS_F7_L0_2022_086_10_15_V01_F__first101pkts.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1040 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/apid00384.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      416 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/apid00386.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1680 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/apid00391.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      672 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/apid00392.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5600 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/apid00393.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2964 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/apid00394.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2448 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/apid01313.tlm
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.813943 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1443 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/Conventions.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2025 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_INP.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2024 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_OUT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2028 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_TLM.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2334 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_ACK.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3181 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_AD_RESP.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2954 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_AUTOLOAD.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3169 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_ERASEFLASH.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3264 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_DUMP.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3193 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_LOAD.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11574 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_PWR.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4383 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_TRACK_STAT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4673 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_COMM_DIAG.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11049 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CYGNSS_PKT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4339 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_DATA_LOGGER_STAT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11742 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_FRONT_END_STAT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3521 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_NAV_INFO.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     5569 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_OP_SETTINGS.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3874 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_ORBITAL_ELEMENTS.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3373 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PPS_TABLE.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     8213 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PROCESSED_DATA.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11728 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PVT_INFO.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9803 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_RAW_DATA.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6597 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_CHAN_STAT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9974 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_LIST.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3052 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_STAT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2812 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4689 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM_TH.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3067 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_STATUS.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3875 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_STREAM_ROUTER_STAT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1672 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_ECHO.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2233 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_MAG_RAW.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    13104 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_NST_RAW.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     8921 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_RWA_RAW.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    14772 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_ADCS.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    10135 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_ADCSIO.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)   150107 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_BOOT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4122 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_DDMI.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1935 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_DNLD.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1662 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_DNLD_FAT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    42952 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_DNLD_FPT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9093 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_ERREVT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1562 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_FILL.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    12767 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_HI.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    28801 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_LOW.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    31990 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_LZ.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    17290 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_PASS.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3652 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_PVT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     8744 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_SSV.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)       45 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/LIMITS.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9201 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/Overview.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    24277 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/Revision History.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6540 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/SCI_DDM_BB_X8.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4905 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/SCI_DDM_X10.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     5124 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/SCI_DDM_X11.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6725 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/SCI_DDM_X8.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6856 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/SCI_FULL.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     5878 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/SCI_META.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6120 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/SCI_META_V2.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2016 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/SCI_RAW.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1384 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/SUPER_NOM.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.823946 ccsdspy-1.3.0/ccsdspy/tests/data/var_length/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      634 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/var_length/README.md
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      318 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/var_length/var_length_packets.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1214 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/var_length/var_length_packets.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2016 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/var_length/var_length_packets_double_varfield.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      590 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/var_length/var_length_packets_double_varfield_with_footer.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      338 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/data/var_length/var_length_packets_with_footer.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3487 2024-02-26 07:06:13.000000 ccsdspy-1.3.0/ccsdspy/tests/test_byte_order.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    19378 2024-02-13 06:57:00.000000 ccsdspy-1.3.0/ccsdspy/tests/test_converters.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4838 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/test_hs.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3103 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/test_packet_fields.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     9316 2024-05-24 05:11:16.000000 ccsdspy-1.3.0/ccsdspy/tests/test_packet_types.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8837 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/test_primary_header.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     9618 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/test_regression.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4480 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/test_split.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4757 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/test_utils.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4182 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/tests/test_var_length.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7887 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/ccsdspy/utils.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.903944 ccsdspy-1.3.0/ccsdspy.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7554 2024-05-24 05:19:50.000000 ccsdspy-1.3.0/ccsdspy.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8980 2024-05-24 05:19:51.000000 ccsdspy-1.3.0/ccsdspy.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2024-05-24 05:19:50.000000 ccsdspy-1.3.0/ccsdspy.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      201 2024-05-24 05:19:50.000000 ccsdspy-1.3.0/ccsdspy.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        8 2024-05-24 05:19:50.000000 ccsdspy-1.3.0/ccsdspy.egg-info/top_level.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.832443 ccsdspy-1.3.0/docs/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8399 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/Makefile
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.833943 ccsdspy-1.3.0/docs/_static/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    36033 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/_static/logo.png
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.871944 ccsdspy-1.3.0/docs/_static/used-by/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)   324142 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/_static/used-by/csa.png
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)   281290 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/_static/used-by/elfin.jpg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   508291 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/_static/used-by/europa-clipper.png
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)  1343999 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/_static/used-by/goes-r.png
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    74095 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/_static/used-by/hermes.png
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)   240058 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/_static/used-by/mms.jpg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)  1671745 2024-02-13 06:52:11.000000 ccsdspy-1.3.0/docs/_static/used-by/pace.png
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   644732 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/_static/used-by/padre.png
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)   152642 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/_static/used-by/punch.png
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)      106 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/_static/used-by/resize.sh
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.884944 ccsdspy-1.3.0/docs/_static/used-by/small/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    19888 2024-02-13 06:46:54.000000 ccsdspy-1.3.0/docs/_static/used-by/small/csa.png
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    16916 2024-02-13 06:46:54.000000 ccsdspy-1.3.0/docs/_static/used-by/small/elfin.jpg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    17632 2024-02-13 06:46:54.000000 ccsdspy-1.3.0/docs/_static/used-by/small/europa-clipper.png
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    20111 2024-02-13 06:46:54.000000 ccsdspy-1.3.0/docs/_static/used-by/small/goes-r.png
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    14174 2024-02-13 06:46:54.000000 ccsdspy-1.3.0/docs/_static/used-by/small/hermes.png
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    41871 2024-02-13 06:46:54.000000 ccsdspy-1.3.0/docs/_static/used-by/small/mms.jpg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     9213 2024-02-13 06:52:11.000000 ccsdspy-1.3.0/docs/_static/used-by/small/pace.png
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    14542 2024-02-13 06:46:54.000000 ccsdspy-1.3.0/docs/_static/used-by/small/padre.png
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    13675 2024-02-13 06:46:54.000000 ccsdspy-1.3.0/docs/_static/used-by/small/punch.png
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    10829 2024-02-13 06:46:54.000000 ccsdspy-1.3.0/docs/_static/used-by/small/spherex.png
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   102429 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/_static/used-by/spherex.png
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.888448 ccsdspy-1.3.0/docs/_templates/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      463 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/_templates/github.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       80 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/_templates/logo.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      134 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/api.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7671 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/conf.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.890443 ccsdspy-1.3.0/docs/dev-guide/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7279 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/dev-guide/index.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3524 2024-02-13 06:52:11.000000 ccsdspy-1.3.0/docs/index.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7768 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/make.bat
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       34 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/requirements.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.899444 ccsdspy-1.3.0/docs/user-guide/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3409 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/user-guide/ccsds.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4247 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/user-guide/converters.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3072 2024-05-24 05:11:16.000000 ccsdspy-1.3.0/docs/user-guide/fixedlength.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      255 2024-05-24 05:11:16.000000 ccsdspy-1.3.0/docs/user-guide/index.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3976 2024-05-24 05:11:16.000000 ccsdspy-1.3.0/docs/user-guide/loadfile.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1853 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/user-guide/packetfields.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4671 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/user-guide/utils.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3963 2024-05-24 05:11:16.000000 ccsdspy-1.3.0/docs/user-guide/variablelength.rst
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-24 05:19:51.901945 ccsdspy-1.3.0/docs/whatsnew/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       95 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/whatsnew/changelog.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      110 2024-02-11 01:40:22.000000 ccsdspy-1.3.0/docs/whatsnew/index.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2725 2024-05-24 05:11:16.000000 ccsdspy-1.3.0/pyproject.toml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      597 2024-05-24 05:11:16.000000 ccsdspy-1.3.0/readthedocs.yml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      162 2024-05-24 05:19:51.907945 ccsdspy-1.3.0/setup.cfg
```

### Comparing `ccsdspy-1.2.1/.github/workflows/ccsdspy-ci.yml` & `ccsdspy-1.3.0/.github/workflows/ccsdspy-ci.yml`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/.github/workflows/doc-build.yml` & `ccsdspy-1.3.0/.github/workflows/doc-build.yml`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/.gitignore` & `ccsdspy-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/CHANGELOG.rst` & `ccsdspy-1.3.0/CHANGELOG.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Notable changes to this project will be documented in this file.
 The format is based on `Keep a Changelog <https://keepachangelog.com/en/1.0.0/>`__.
 
+
+Version 1.3.0 - 2024-05-24
+============================
+  * Added support for custom byte orderings in  `ccsdspy.PacketField` and `ccsdspy.PacketArray`. You can now pass strings like `byte_order="3412"` in addition to `byte_order="big"` and `byte_order="little"`. (Discussion `#110 <https://github.com/CCSDSPy/ccsdspy/discussions/110>`_)
+
+  * Implement loading variable length packets from CSV (`Issue #115 <https://github.com/CCSDSPy/ccsdspy/issues/115>`_)
+  * Add documentation page: :doc:`/user-guide/loadfile`
+  * Accept CCSDS header fields as converter inputs (`PR #118 <https://github.com/CCSDSPy/ccsdspy/pull/118>`_)
+  * Add support `pkt.load(fh, reset_file_obj=True)` keyword argument which resets file handle to original position before loading (`Issue #111 <https://github.com/CCSDSPy/ccsdspy/issues/111>`_)
+    
 Version 1.2.1 - 2023-11-26
 ==========================
   * Fixed bug/regression introduced in 1.2.0 from signed integer patch (Discussion `#101 <https://github.com/CCSDSPy/ccsdspy/discussions/101>`_)
   * Fixed bug with expanding fields that occur in the middle of the packet (Discussion `#102 <https://github.com/CCSDSPy/ccsdspy/discussions/102>`_)
 
 Version 1.2.0 - 2023-09-27
 ==========================
```

### Comparing `ccsdspy-1.2.1/LICENSE.rst` & `ccsdspy-1.3.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/PKG-INFO` & `ccsdspy-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccsdspy
-Version: 1.2.1
+Version: 1.3.0
 Summary: IO Interface for Reading CCSDS Data in Python.
 Author-email: Daniel da Silva <mail@danieldasilva.org>, Steven Christe <steven.d.christe@nasa.gov>
 License: Copyright (c) 2018, Daniel da Silva
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -41,18 +41,18 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 Requires-Dist: numpy>=1.8.0
 Provides-Extra: dev
 Requires-Dist: coverage>=6.5.0; extra == "dev"
-Requires-Dist: pytest>=7.1.3; extra == "dev"
+Requires-Dist: pytest<8.1.0,>=7.1.3; extra == "dev"
 Requires-Dist: pytest-astropy; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: black>=22.10.0; extra == "dev"
+Requires-Dist: black==22.10.0; extra == "dev"
 Requires-Dist: flake8>=5.0.4; extra == "dev"
 Requires-Dist: coverage[toml]; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx>=5.2.3; extra == "docs"
 Requires-Dist: sphinx-automodapi>=0.14.1; extra == "docs"
 Requires-Dist: graphviz>=0.20.1; extra == "docs"
 Requires-Dist: numpydoc; extra == "docs"
@@ -76,20 +76,26 @@
 	  
 This community-developed package provides a Python interface for reading tightly packed bits in the `Consultative Committee for Space Data Systems (CCSDS) <https://public.ccsds.org/default.aspx>`__ format used by many NASA and ESA missions. The library is developed with requirements sourced from the community and extensive automated testing.
 
 Used By
 -------
 .. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/goes-r.png
     :target: https://www.goes-r.gov/
+.. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/europa-clipper.png
+    :target: https://europa.nasa.gov/	     
+.. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/mms.jpg
+    :target: https://mms.gsfc.nasa.gov/
+.. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/pace.png
+    :target: https://pace.gsfc.nasa.gov/
 .. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/hermes.png
     :target: https://science.nasa.gov/missions/hermes
+.. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/csa.png
+    :target: https://www.asc-csa.gc.ca/eng/	     
 .. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/punch.png
     :target: https://punch.space.swri.edu/
-.. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/mms.jpg
-    :target: https://mms.gsfc.nasa.gov/
 .. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/spherex.png
     :target: https://www.jpl.nasa.gov/missions/spherex
 .. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/elfin.jpg
     :target: https://elfin.igpp.ucla.edu/
 .. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/padre.png
     :target: https://padre.ssl.berkeley.edu
 
@@ -116,21 +122,21 @@
    
    pkt = ccsdspy.FixedLength([
         PacketField(name='SHCOARSE', data_type='uint', bit_length=32),
         PacketField(name='SHFINE',   data_type='uint', bit_length=20),
         PacketField(name='OPMODE',   data_type='uint', bit_length=3),
         PacketField(name='SPACER',   data_type='fill', bit_length=1),
         PacketField(name='VOLTAGE',  data_type='int',  bit_length=8),
-	PacketArray(
+        PacketArray(
             name='SENSOR_GRID',
             data_type='uint',
             bit_length=16,
             array_shape=(32, 32),
             array_order='C'
-	),
+        ),
    ])
    
    result = pkt.load('mypackets.bin')
 
 Documentation
 =============
 Our documentation is hosted on readthedocs and can be found `here <https://ccsdspy.readthedocs.io/en/latest/>`__.
```

### Comparing `ccsdspy-1.2.1/README.rst` & `ccsdspy-1.3.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -17,20 +17,26 @@
 	  
 This community-developed package provides a Python interface for reading tightly packed bits in the `Consultative Committee for Space Data Systems (CCSDS) <https://public.ccsds.org/default.aspx>`__ format used by many NASA and ESA missions. The library is developed with requirements sourced from the community and extensive automated testing.
 
 Used By
 -------
 .. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/goes-r.png
     :target: https://www.goes-r.gov/
+.. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/europa-clipper.png
+    :target: https://europa.nasa.gov/	     
+.. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/mms.jpg
+    :target: https://mms.gsfc.nasa.gov/
+.. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/pace.png
+    :target: https://pace.gsfc.nasa.gov/
 .. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/hermes.png
     :target: https://science.nasa.gov/missions/hermes
+.. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/csa.png
+    :target: https://www.asc-csa.gc.ca/eng/	     
 .. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/punch.png
     :target: https://punch.space.swri.edu/
-.. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/mms.jpg
-    :target: https://mms.gsfc.nasa.gov/
 .. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/spherex.png
     :target: https://www.jpl.nasa.gov/missions/spherex
 .. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/elfin.jpg
     :target: https://elfin.igpp.ucla.edu/
 .. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/padre.png
     :target: https://padre.ssl.berkeley.edu
 
@@ -57,21 +63,21 @@
    
    pkt = ccsdspy.FixedLength([
         PacketField(name='SHCOARSE', data_type='uint', bit_length=32),
         PacketField(name='SHFINE',   data_type='uint', bit_length=20),
         PacketField(name='OPMODE',   data_type='uint', bit_length=3),
         PacketField(name='SPACER',   data_type='fill', bit_length=1),
         PacketField(name='VOLTAGE',  data_type='int',  bit_length=8),
-	PacketArray(
+        PacketArray(
             name='SENSOR_GRID',
             data_type='uint',
             bit_length=16,
             array_shape=(32, 32),
             array_order='C'
-	),
+        ),
    ])
    
    result = pkt.load('mypackets.bin')
 
 Documentation
 =============
 Our documentation is hosted on readthedocs and can be found `here <https://ccsdspy.readthedocs.io/en/latest/>`__.
```

### Comparing `ccsdspy-1.2.1/ccsdspy/__init__.py` & `ccsdspy-1.3.0/ccsdspy/__init__.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/__main__.py` & `ccsdspy-1.3.0/ccsdspy/__main__.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/converters.py` & `ccsdspy-1.3.0/ccsdspy/converters.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/decode.py` & `ccsdspy-1.3.0/ccsdspy/decode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Internal decoding routines."""
+
 from __future__ import division
 from collections import namedtuple
 import math
 import warnings
 
 import numpy as np
 
@@ -167,15 +168,15 @@
         nbytes_final = {3: 4, 5: 8, 6: 8, 7: 8}.get(nbytes_file, nbytes_file)
         start_byte_file = bit_offset[field._name] // BITS_PER_BYTE
 
         # byte_order_symbol is only used to control float types here.
         #  - uint and int byte order are handled with byteswap later
         #  - fill is independent of byte order (all 1's)
         #  - byte order is not applicable to str types
-        byte_order_symbol = "<" if field._byte_order == "little" else ">"
+        byte_order_symbol = "<" if field._byte_order_parse == "little" else ">"
         np_dtype = {
             "uint": ">u%d" % nbytes_final,
             "int": ">i%d" % nbytes_final,
             "fill": "S%d" % nbytes_final,
             "float": "%sf%d" % (byte_order_symbol, nbytes_final),
             "str": "S%d" % nbytes_final,
         }[field._data_type]
@@ -241,15 +242,15 @@
             bitmask |= (1 << int(BITS_PER_BYTE * meta.nbytes_final - bitmask_left)) - 1
             tmp = np.left_shift([1], bitmask_right)
             bitmask &= np.bitwise_not(tmp[0] - 1).astype(arr.dtype)
 
             arr &= bitmask
             arr >>= bitmask_right
 
-            if field._byte_order == "little":
+            if field._byte_order_parse == "little":
                 arr.byteswap(inplace=True)
 
             if field._data_type == "int":
                 arr.dtype = meta.np_dtype
                 sign_bit = (arr >> (field._bit_length - 1)) & 1
 
                 # Set bits between start_bit and stop_bit to 1
@@ -396,15 +397,15 @@
                             "1" * ((nbytes_file * BITS_PER_BYTE) - left_bits_before_shift), 2
                         )
                         field_raw_data &= mask
 
                     if right_shift > 0:
                         field_raw_data >>= right_shift
 
-                if field._byte_order == "little":
+                if field._byte_order_parse == "little":
                     field_raw_data.byteswap(inplace=True)
 
                 if field._data_type == "int":
                     field_raw_data.dtype = numpy_dtypes[field._name]
                     sign_bit = (field_raw_data >> (field._bit_length - 1)) & 1
 
                     if sign_bit:
@@ -510,15 +511,15 @@
             nbytes_file[field._name], nbytes_file[field._name]
         )
 
         # byte_order_symbol is only used to control float types here.
         #  - uint and int byte order are handled with byteswap later
         #  - fill is independent of byte order (all 1's)
         #  - byte order is not applicable to str types
-        byte_order_symbol = "<" if field._byte_order == "little" else ">"
+        byte_order_symbol = "<" if field._byte_order_parse == "little" else ">"
         np_dtype = {
             "uint": ">u%d" % nbytes_final,
             "int": ">i%d" % nbytes_final,
             "fill": "S%d" % nbytes_final,
             "float": "%sf%d" % (byte_order_symbol, nbytes_final),
             "str": "S%d" % nbytes_final,
         }[field._data_type]
```

### Comparing `ccsdspy-1.2.1/ccsdspy/packet_fields.py` & `ccsdspy-1.3.0/ccsdspy/packet_fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 See also:
 - packet_types.FixedLength
 - packet_types.VariableLength
 """
 
 __author__ = "Daniel da Silva <mail@danieldasilva.org>"
 
+import string
+
 import numpy as np
 
 from .converters import Converter
 
 
 class PacketField:
     """A field contained in a packet."""
@@ -26,16 +28,17 @@
             Data type of the field.
         bit_length : int
             Number of bits contained in the field.
         bit_offset : int, optional
             Bit offset into packet, including the primary header which is 48 bits long.
             If this is not specified, than the bit offset will the be calculated automatically
             from its position inside the packet definition.
-        byte_order : {'big', 'little'}, optional
-            Byte order of the field. Defaults to big endian.
+        byte_order : {'big', 'little'}, or custom string of digits like "4321"
+            Byte order of the field. Can be "big", "little", or an arbitrary ordering
+            Specified as a string of digits like "2341". Defaults to big endian.
 
         Raises
         ------
         TypeError
              If one of the arguments is not of the correct type.
         ValueError
              data_type or byte_order is invalid
@@ -49,24 +52,35 @@
         if not (bit_offset is None or isinstance(bit_offset, (int, np.integer))):
             raise TypeError("bit_offset parameter must be an int")
 
         valid_data_types = ("uint", "int", "float", "str", "fill")
         if data_type not in valid_data_types:
             raise ValueError(f"data_type must be one of {valid_data_types}")
 
-        valid_byte_orders = ("big", "little")
-        if byte_order not in valid_byte_orders:
-            raise ValueError(f"byte_order must be one of {valid_byte_orders}")
+        valid_default_byte_orders = ("big", "little")
+        valid_custom_byte_order = all(char in string.digits for char in byte_order)
+        if byte_order in valid_default_byte_orders:
+            byte_order_parse = byte_order
+            byte_order_post = None
+        elif valid_custom_byte_order:
+            byte_order_parse = "big"
+            byte_order_post = byte_order
+        else:
+            raise ValueError(
+                f"byte_order must be one of {valid_default_byte_orders} or "
+                "a string like '1234' or '3412'."
+            )
 
         self._name = name
         self._data_type = data_type
         self._bit_length = bit_length
         self._bit_offset = bit_offset
         self._byte_order = byte_order
-
+        self._byte_order_parse = byte_order_parse
+        self._byte_order_post = byte_order_post
         self._field_type = "element"
         self._array_shape = None
         self._array_order = None
 
     def __repr__(self):
         values = {k: repr(v) for (k, v) in self.__dict__.items()}
         values["cls_name"] = self.__class__.__name__
```

### Comparing `ccsdspy-1.2.1/ccsdspy/packet_types.py` & `ccsdspy-1.3.0/ccsdspy/packet_types.py`

 * *Files 23% similar despite different names*

```diff
@@ -38,16 +38,16 @@
     def from_file(cls, file):
         """
         Parameters
         ----------
         file : str
            Path to file on the local file system that defines the packet fields.
            Currently only supports csv files.
-           See :download:`simple_csv_3col.csv <../../ccsdspy/tests/data/packet_def/simple_csv_3col.csv>`  # noqa: E501
-           and :download:`simple_csv_4col.csv <../../ccsdspy/tests/data/packet_def/simple_csv_4col.csv>`  # noqa: E501
+           See :download:`basic_csv_3col.csv <../../ccsdspy/tests/data/packet_def/basic_csv_3col.csv>`  # noqa: E501
+           and :download:`extended_csv_4col.csv <../../ccsdspy/tests/data/packet_def/extended_csv_4col.csv>`  # noqa: E501
 
         Returns
         -------
         An instance of FixedLength.
         """
         file_extension = os.path.splitext(file)
         if file_extension[1] == ".csv":
@@ -95,15 +95,21 @@
         else:
             raise TypeError("input_field_name must be either str, list, or tuple")
 
         del input_field_name  # don't use the variable again in this function
 
         # Check that each of the input field names exists in the packet, and report
         # the missing fields if not
-        fields_in_packet_set = {field._name for field in self._fields}
+        # Collect valid names of fields, which include primary header fields as well
+        # as fields defined in the packet.
+        fields_in_packet_set = set()
+
+        for field in _prepend_primary_header_fields(self._fields):
+            fields_in_packet_set.add(field._name)
+
         input_field_names_set = set(input_field_names)
         all_fields_present = input_field_names_set <= fields_in_packet_set  # subset
 
         if not all_fields_present:
             missing_fields = input_field_names_set - fields_in_packet_set  # set op A \ B
             raise ValueError(
                 "Some fields specified as inputs to converters were missing: "
@@ -137,23 +143,30 @@
             raise ValueError(
                 "The FixedLength class does not support variable fields. "
                 "Instead, use the VariableLength class."
             )
 
         self._init(fields)
 
-    def load(self, file, include_primary_header=False):
+    def load(self, file, include_primary_header=False, reset_file_obj=False):
         """Decode a file-like object containing a sequence of these packets.
 
         Parameters
         ----------
         file : str
            Path to file on the local file system, or file-like object
         include_primary_header : bool
-           If True, provides the primary header in the output
+           If True, provides the primary header in the output. The names of the
+           fields are: `CCSDS_VERSION_NUMBER`, `CCSDS_PACKET_TYPE`,
+           `CCSDS_SECONDARY_FLAG`, `CCSDS_SEQUENCE_FLAG`, `CCSDS_APID`,
+           `CCSDS_SEQUENCE_COUNT`, and `CCSDS_PACKET_LENGTH`
+        reset_file_obj : bool
+           If True, leave the file object, when it is file buffer, where it was before load is called.
+           Otherwise, (default), leave the file stream pos after the read packets.
+           Does not apply when file is a string.
 
         Returns
         -------
         field_arrays : dict, string to NumPy array
             dictionary mapping field names to NumPy arrays, with key order matching
             the order of fields in the packet.
 
@@ -168,14 +181,15 @@
         """
         packet_arrays = _load(
             file,
             self._fields,
             self._converters,
             "fixed_length",
             include_primary_header=True,
+            reset_file_obj=reset_file_obj,
         )
 
         # inspect the primary header and issue warning if appropriate
         _inspect_primary_header_fields(packet_arrays)
 
         if not include_primary_header:
             _delete_primary_header_fields(packet_arrays)
@@ -255,23 +269,30 @@
                 "The VariableLength class does not support explicit bit "
                 "offsets. You must specify the entire packet so they can be "
                 "determined automatically."
             )
 
         self._init(fields)
 
-    def load(self, file, include_primary_header=False):
+    def load(self, file, include_primary_header=False, reset_file_obj=False):
         """Decode a file-like object containing a sequence of these packets.
 
         Parameters
         ----------
         file : str
            Path to file on the local file system, or file-like object
         include_primary_header : bool
-           If True, provides the primary header in the output
+           If True, provides the primary header in the output. The names of the
+           fields are: `CCSDS_VERSION_NUMBER`, `CCSDS_PACKET_TYPE`,
+           `CCSDS_SECONDARY_FLAG`, `CCSDS_SEQUENCE_FLAG`, `CCSDS_APID`,
+           `CCSDS_SEQUENCE_COUNT`, and `CCSDS_PACKET_LENGTH`
+        reset_file_obj : bool
+           If True, leave the file object, when it is file buffer, where it was before load is called.
+           Otherwise, (default), leave the file stream pos after the read packets.
+           Does not apply when file is a string.
 
         Returns
         -------
         field_arrays : dict, string to NumPy array
             dictionary mapping field names to NumPy arrays, with key order matching
             the order of fields in the packet.
 
@@ -284,15 +305,20 @@
         UserWarning
             If there are more than one APID
         """
         # The variable length decoder requires the full packet definition, so if
         # they didn't want the primary header fields, we parse for them and then
         # remove them after.
         packet_arrays = _load(
-            file, self._fields, self._converters, "variable_length", include_primary_header=True
+            file,
+            self._fields,
+            self._converters,
+            "variable_length",
+            include_primary_header=True,
+            reset_file_obj=reset_file_obj,
         )
 
         # inspect the primary header and issue warning if appropriate
         _inspect_primary_header_fields(packet_arrays)
 
         if not include_primary_header:
             _delete_primary_header_fields(packet_arrays)
@@ -430,17 +456,22 @@
     for array_name, array_details in expand_history.items():
         array_shape = (npackets,) + array_details["shape"]
         array_dtype = field_arrays[list(array_details["fields"].keys())[0]].dtype
         array = np.zeros(array_shape, dtype=array_dtype)
 
         for element_name, indices in array_details["fields"].items():
             array.__setitem__((slice(None),) + indices, field_arrays[element_name])
+            # get index of the position where the array field was
+            pos = list(return_field_arrays.keys()).index(element_name)
             del return_field_arrays[element_name]
 
-        return_field_arrays[array_name] = array
+        # do the following trick to insert the unexpanded array where the expanded arrays fields were.
+        return_field_items = list(return_field_arrays.items())
+        return_field_items.insert(pos, (array_name, array))
+        return_field_arrays = dict(return_field_items)
 
     return return_field_arrays
 
 
 def _prepend_primary_header_fields(existing_fields):
     """Helper function that prepends primary header fields to a list of packet
     fields, to support load(include_primary_header=True)
@@ -495,14 +526,42 @@
     ]
 
     return_fields.extend(existing_fields)
 
     return return_fields
 
 
+def _parse_csv_array_shape(data_type_str):
+    """Parse a data type string from a CSV to determine the array shape.
+
+    Parameters
+    ----------
+    data_type_str : str
+        Full string specifying the data type, e.g. `uint(1, 2)`
+
+    Returns
+    -------
+    array_shape : str, int, tuple of int
+       Parsed array shape to be used in loading CSV.
+    """
+    array_shape_str = data_type_str[data_type_str.find("(") + 1 : data_type_str.find(")")]
+    if array_shape_str == "expand":
+        array_shape = "expand"
+    elif "," in array_shape_str:
+        try:
+            array_shape = tuple(map(int, array_shape_str.split(", ")))
+        except ValueError:
+            raise ValueError(
+                "Array shape must be `expand`, the name of another field, or a tuple of ints."
+            )
+    else:  # string is either another field for reference or a single integer for a one dimensional array shape
+        array_shape = int(array_shape_str) if array_shape_str.isnumeric() else array_shape_str
+    return array_shape
+
+
 def _get_fields_csv_file(csv_file):
     """Parse a simple comma-delimited file that defines a packet.
 
     Should not include the CCSDS header. The minimum set of columns are (name,
     data_type, bit_length). An optional bit_offset can also be provided.
 
     Parameters
@@ -525,45 +584,39 @@
         if headers is None:
             raise RuntimeError("CSV file must not be empty")
 
         if not all((req_col in headers) for req_col in req_columns):
             raise ValueError(f"Minimum required columns are {req_columns}.")
 
         for row in reader:  # skip the header row
-            if "bit_offset" not in headers:  # 3 col csv file
+            if "bit_offset" not in headers:  # basic 3 col csv file
                 if (row["data_type"].count("(") == 1) and (row["data_type"].count(")") == 1):
                     data_type = row["data_type"].split("(")[0]
-                    array_shape_str = row["data_type"][
-                        row["data_type"].find("(") + 1 : row["data_type"].find(")")
-                    ]
-                    array_shape = tuple(map(int, array_shape_str.split(", ")))
+                    array_shape = _parse_csv_array_shape(row["data_type"])
                     fields.append(
                         PacketArray(
                             name=row["name"],
                             data_type=data_type,
                             bit_length=int(row["bit_length"]),
-                            array_shape=(array_shape),
+                            array_shape=array_shape,
                         )
                     )
                 else:
                     fields.append(
                         PacketField(
                             name=row["name"],
                             data_type=row["data_type"],
                             bit_length=int(row["bit_length"]),
                         )
                     )
-            if "bit_offset" in headers:  # 4 col csv file provides bit offsets
+            if "bit_offset" in headers:  # extended 4 col csv file provides bit offsets
                 # TODO: Check the consistency of bit_offsets versus previous bit_lengths
                 if (row["data_type"].count("(") == 1) and (row["data_type"].count(")") == 1):
                     data_type = row["data_type"].split("(")[0]
-                    array_shape_str = row["data_type"][
-                        row["data_type"].find("(") + 1 : row["data_type"].find(")")
-                    ]
-                    array_shape = tuple(map(int, array_shape_str.split(", ")))
+                    array_shape = _parse_csv_array_shape(row["data_type"])
                     fields.append(
                         PacketArray(
                             name=row["name"],
                             data_type=data_type,
                             bit_length=int(row["bit_length"]),
                             bit_offset=int(row["bit_offset"]),
                             array_shape=array_shape,
@@ -578,15 +631,17 @@
                             bit_offset=int(row["bit_offset"]),
                         )
                     )
 
     return fields
 
 
-def _load(file, fields, converters, decoder_name, include_primary_header=False):
+def _load(
+    file, fields, converters, decoder_name, include_primary_header=False, reset_file_obj=False
+):
     """Decode a file-like object containing a sequence of these packets.
 
     Parameters
     ----------
     file: str
        Path to file on the local file system, or file-like object
     fields : list of `ccsdspy.PacketField`
@@ -594,30 +649,37 @@
     converters : dict, str to tuple (str, Converter)
        Dictionary of post-processing conversions. keys are input field names,
        values are tuples of (output_field_name, Converter instance)
     decoder_name: {'fixed_length', 'variable_length'}
        String identifying which decoder to use.
     include_primary_header: bool
        If True, provides the primary header in the output
+    reset_file_obj : bool
+           If True, leave the file object, when it is a file buffer, where it was before _load is called.
+           Otherwise, (default), leave the file stream pos after the read packets.
+           Does not apply when file is a string.
 
     Returns
     -------
     dictionary mapping field names to NumPy arrays, with key order matching
     the order fields in the packet.
 
     Raises
     ------
     ValueError
       the decoder_name is not one of the allowed values
     """
     if hasattr(file, "read"):
+        file_pos = file.tell()
         file_bytes = np.frombuffer(file.read(), "u1")
     else:
         file_bytes = np.fromfile(file, "u1")
 
+    orig_fields = fields
+
     if include_primary_header:
         fields = _prepend_primary_header_fields(fields)
 
     fields, expand_history = _expand_array_fields(fields)
 
     if decoder_name == "fixed_length":
         field_arrays = _decode_fixed_length(file_bytes, fields)
@@ -626,16 +688,19 @@
     else:
         raise ValueError(
             f"Invalid decoder_name 'f{decoder_name}' specified. Must be "
             "either 'fixed_length', or 'variable_length'"
         )
 
     field_arrays = _unexpand_field_arrays(field_arrays, expand_history)
+    field_arrays = _apply_post_byte_reoderings(field_arrays, orig_fields)
     field_arrays = _apply_converters(field_arrays, converters)
 
+    if hasattr(file, "read") and reset_file_obj:
+        file.seek(file_pos)
     return field_arrays
 
 
 def _apply_converters(field_arrays, converters):
     """Apply post-processing converters in place to a dictionary of field
     arrays.
 
@@ -662,7 +727,95 @@
         for input_field_name in input_field_names:
             input_arrays.append(field_arrays[input_field_name])
 
         # Call converter function
         converted[output_field_name] = converter.convert(*input_arrays)
 
     return converted
+
+
+def _apply_post_byte_reoderings(field_arrays, orig_fields):
+    """Step of load procedure to apply post-processing byte reorderings.
+
+    A field gets post-processing byte reordering if the attribute
+      `field._byte_order_post` is not None.
+
+    Parameters
+    ----------
+    field_arrays : dict of string to NumPy arrays
+       The decoded packet field arrays without any post-processing applied
+    orig_fields : List of PacketField
+       Original fields as specified in the packet, before any replacements
+       which occur in the processing step.
+
+    Returns
+    -------
+    Reference to argument field_arrays (object was mutuated).
+    """
+    for field in orig_fields:
+        if field._byte_order_post is None:
+            continue
+
+        byte_order_string = field._byte_order_post
+        byte_order_ints = [int(digit) for digit in byte_order_string]
+        is_obj_array = field_arrays[field._name].dtype == object
+
+        if is_obj_array:
+            new_packet_arrays = []
+
+            for i, packet_array in enumerate(field_arrays[field._name]):
+                field_arrays[field._name][i] = _do_array_byte_reordering(
+                    packet_array, byte_order_ints
+                )
+        else:
+            field_arrays[field._name] = _do_array_byte_reordering(
+                field_arrays[field._name], byte_order_ints
+            )
+
+    return field_arrays
+
+
+def _do_array_byte_reordering(array, byte_order_ints):
+    """Reorder the bytes of an array.
+
+    Parameters
+    ----------
+    array : NumPy array
+      May be multidimensional. Dtype of array must not be object.
+    byte_order_ints : list of int
+      Inceces of the bytes in order, e.g., 2314.
+
+    Returns
+    -------
+    Array with bytes reordered according to the passed order.
+    """
+    assert array.dtype != object, "Error in byte reordering, please report a bug:.{array.dtype}"
+
+    parsed_byte_length = array.itemsize
+    native_byte_length = max(byte_order_ints)
+
+    array_bytes = array.copy()
+    array_bytes.dtype = np.uint8
+    array_bytes = array_bytes.reshape((array.size, parsed_byte_length))
+
+    digits_zero_idx = [digit - 1 for digit in reversed(byte_order_ints)]
+    select_indeces = []
+    select_indeces.extend(digits_zero_idx)
+    select_indeces.extend(sorted(set(range(array.itemsize)) - set(digits_zero_idx)))
+
+    padding = array.itemsize - len(byte_order_ints)
+    reordered = np.zeros_like(array_bytes)
+
+    for i in range(reordered.shape[0]):
+        reordered[i, :] = array_bytes[i, ::-1][select_indeces]
+
+    shifted = np.zeros_like(reordered)
+
+    if padding > 0:
+        shifted[:, padding:] = reordered[:, :-padding]
+    else:
+        shifted[:] = reordered
+
+    shifted.dtype = array.dtype
+    shifted = shifted.reshape(array.shape)
+
+    return shifted
```

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/csa/apid00400.tlm` & `ccsdspy-1.3.0/ccsdspy/tests/data/csa/apid00400.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/europa_clipper/apid01216.tlm` & `ccsdspy-1.3.0/ccsdspy/tests/data/europa_clipper/apid01216.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/europa_clipper/apid01219.tlm` & `ccsdspy-1.3.0/ccsdspy/tests/data/europa_clipper/apid01219.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/europa_clipper/apid01223.tlm` & `ccsdspy-1.3.0/ccsdspy/tests/data/europa_clipper/apid01223.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/europa_clipper/apid01227.tlm` & `ccsdspy-1.3.0/ccsdspy/tests/data/europa_clipper/apid01227.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/europa_clipper/apid01232.tlm` & `ccsdspy-1.3.0/ccsdspy/tests/data/europa_clipper/apid01232.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/europa_clipper/ecm_raw2.bin` & `ccsdspy-1.3.0/ccsdspy/tests/data/europa_clipper/ecm_raw2.bin`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/europa_clipper/expanding_footer_packet.bin` & `ccsdspy-1.3.0/ccsdspy/tests/data/europa_clipper/expanding_footer_packet.bin`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid001/SSAT1_2015-180-00-00-00_2015-180-01-59-58_1_1_sim.tlm` & `ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid001/SSAT1_2015-180-00-00-00_2015-180-01-59-58_1_1_sim.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid001/defs.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid001/defs.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid010/SSAT1_2015-180-00-00-00_2015-180-00-59-59_10_1_sim.tlm` & `ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid010/SSAT1_2015-180-00-00-00_2015-180-00-59-59_10_1_sim.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid010/defs.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid010/defs.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid035/SSAT1_2015-180-00-00-00_2015-180-01-59-59_35_1_sim.tlm` & `ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid035/SSAT1_2015-180-00-00-00_2015-180-01-59-59_35_1_sim.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid035/defs.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid035/defs.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid130/SSAT1_2015-180-00-00-00_2015-180-01-59-35_130_1_sim.tlm` & `ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid130/SSAT1_2015-180-00-00-00_2015-180-01-59-35_130_1_sim.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid251/SSAT1_2015-180-00-00-00_2015-180-01-59-59_251_1_sim.tlm` & `ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid251/SSAT1_2015-180-00-00-00_2015-180-01-59-59_251_1_sim.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/hs/apid895/SSAT1_2015-180-00-00-00_2015-180-01-59-56_895_1_sim.tlm` & `ccsdspy-1.3.0/ccsdspy/tests/data/hs/apid895/SSAT1_2015-180-00-00-00_2015-180-01-59-56_895_1_sim.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/hs/attic/SSAT_Mnemonics.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/hs/attic/SSAT_Mnemonics.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/hs/attic/_expand_mnemnonics.py` & `ccsdspy-1.3.0/ccsdspy/tests/data/hs/attic/_expand_mnemnonics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This was a data cleaning script."""
+
 import pandas as pd
 from collections import OrderedDict
 
 if __name__ == "__main__":
     df = pd.read_csv("SSAT_Mnemonics.csv")
     apids = set(df["packet_display_name"])
```

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/CYGNSS_F7_L0_2022_086_10_15_V01_F__first101pkts.tlm` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/CYGNSS_F7_L0_2022_086_10_15_V01_F__first101pkts.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/apid00384.tlm` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/apid00384.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/apid00392.tlm` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/apid00392.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/apid00393.tlm` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/apid00393.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/apid00394.tlm` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/apid00394.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/apid01313.tlm` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/apid01313.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/Conventions.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/Conventions.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_INP.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_INP.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_OUT.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_OUT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_TLM.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_TLM.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_ACK.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_ACK.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_AD_RESP.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_AD_RESP.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_AUTOLOAD.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_AUTOLOAD.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_ERASEFLASH.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_ERASEFLASH.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_DUMP.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_DUMP.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_LOAD.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_LOAD.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_PWR.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_PWR.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_TRACK_STAT.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_TRACK_STAT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_COMM_DIAG.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_COMM_DIAG.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_CYGNSS_PKT.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CYGNSS_PKT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_DATA_LOGGER_STAT.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_DATA_LOGGER_STAT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_FRONT_END_STAT.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_FRONT_END_STAT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_NAV_INFO.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_NAV_INFO.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_OP_SETTINGS.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_OP_SETTINGS.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_ORBITAL_ELEMENTS.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_ORBITAL_ELEMENTS.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_PPS_TABLE.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PPS_TABLE.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_PROCESSED_DATA.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PROCESSED_DATA.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_PVT_INFO.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PVT_INFO.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_RAW_DATA.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_RAW_DATA.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_CHAN_STAT.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_CHAN_STAT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_LIST.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_LIST.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_STAT.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_STAT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM_TH.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM_TH.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_STATUS.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_STATUS.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_STREAM_ROUTER_STAT.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_STREAM_ROUTER_STAT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_ECHO.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_ECHO.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_MAG_RAW.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_MAG_RAW.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_NST_RAW.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_NST_RAW.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/DIAG_RWA_RAW.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/DIAG_RWA_RAW.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_ADCS.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_ADCS.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_ADCSIO.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_ADCSIO.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_BOOT.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_BOOT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_DDMI.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_DDMI.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_DNLD.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_DNLD.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_DNLD_FAT.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_DNLD_FAT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_DNLD_FPT.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_DNLD_FPT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_ERREVT.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_ERREVT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_FILL.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_FILL.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_HI.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_HI.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_LOW.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_LOW.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_LZ.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_LZ.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_PASS.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_PASS.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_PVT.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_PVT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/ENG_SSV.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/ENG_SSV.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/Overview.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/Overview.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/Revision History.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/Revision History.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/SCI_DDM_BB_X8.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/SCI_DDM_BB_X8.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/SCI_DDM_X10.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/SCI_DDM_X10.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/SCI_DDM_X11.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/SCI_DDM_X11.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/SCI_DDM_X8.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/SCI_DDM_X8.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/SCI_FULL.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/SCI_FULL.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/SCI_META.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/SCI_META.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/SCI_META_V2.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/SCI_META_V2.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/SCI_RAW.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/SCI_RAW.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/split/defs/SUPER_NOM.csv` & `ccsdspy-1.3.0/ccsdspy/tests/data/split/defs/SUPER_NOM.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/var_length/README.md` & `ccsdspy-1.3.0/ccsdspy/tests/data/var_length/README.md`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/var_length/var_length_packets.py` & `ccsdspy-1.3.0/ccsdspy/tests/data/var_length/var_length_packets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Create simple packets with variable lengths"""
+
 import struct
 
 import numpy as np
 
 out_name = "var_length_packets_with_footer.bin"
 include_footer = True
 num_packets = 10
```

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/var_length/var_length_packets_double_varfield.py` & `ccsdspy-1.3.0/ccsdspy/tests/data/var_length/var_length_packets_double_varfield.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Create simple packets with variable lengths"""
+
 import struct
 
 import numpy as np
 
 out_name = "var_length_packets_double_varfield_with_footer.bin"
 include_footer = True
 num_packets = 10
```

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/data/var_length/var_length_packets_double_varfield_with_footer.bin` & `ccsdspy-1.3.0/ccsdspy/tests/data/var_length/var_length_packets_double_varfield_with_footer.bin`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/test_converters.py` & `ccsdspy-1.3.0/ccsdspy/tests/test_converters.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,15 @@
         dtype=object,
     )
 
     converter = converters.StringifyBytesConverter(format=format)
     result = converter.convert(field_array)
 
     assert isinstance(result, np.ndarray)
-    assert np.issubdtype(result.dtype, object)
+    assert np.issubdtype(result.dtype, np.generic)
 
     if format == "bin":
         expected = np.array(
             [
                 np.array(
                     [
                         "0b0",  #   0
```

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/test_hs.py` & `ccsdspy-1.3.0/ccsdspy/tests/test_hs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Run end-to-end test of decoding fixed-length packets
 using the test data in the data/hs directory.
 """
+
 import csv
 import glob
 import os
 import numpy as np
 
 import pytest
```

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/test_packet_fields.py` & `ccsdspy-1.3.0/ccsdspy/tests/test_packet_fields.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/test_packet_types.py` & `ccsdspy-1.3.0/ccsdspy/tests/test_packet_types.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,22 +7,31 @@
 import struct
 
 import numpy as np
 import pytest
 
 from .. import FixedLength, VariableLength, PacketField, PacketArray
 from ..constants import BITS_PER_BYTE
-from ..packet_types import _get_fields_csv_file
+from ..packet_types import _get_fields_csv_file, _parse_csv_array_shape
 
 dir_path = os.path.dirname(os.path.realpath(__file__))
 packet_def_dir = os.path.join(dir_path, "data", "packet_def")
-csv_file_4col = os.path.join(packet_def_dir, "simple_csv_4col.csv")
-csv_file_3col = os.path.join(packet_def_dir, "simple_csv_3col.csv")
-csv_file_4col_with_array = os.path.join(packet_def_dir, "simple_csv_4col_with_array.csv")
-csv_file_3col_with_array = os.path.join(packet_def_dir, "simple_csv_3col_with_array.csv")
+csv_file_4col = os.path.join(packet_def_dir, "extended_csv_4col.csv")
+csv_file_3col = os.path.join(packet_def_dir, "basic_csv_3col.csv")
+csv_file_4col_with_array = os.path.join(packet_def_dir, "extended_csv_4col_with_array.csv")
+csv_file_3col_with_array = os.path.join(packet_def_dir, "basic_csv_3col_with_array.csv")
+csv_file_3col_with_expand = os.path.join(packet_def_dir, "basic_csv_3col_with_expand.csv")
+csv_file_3col_with_reference = os.path.join(packet_def_dir, "basic_csv_3col_with_reference.csv")
+csv_file_3col_with_all = os.path.join(packet_def_dir, "basic_csv_3col_with_all.csv")
+
+hs_packet_dir = os.path.join(dir_path, "data", "hs")
+random_binary_file = os.path.join(
+    hs_packet_dir, "apid001", "SSAT1_2015-180-00-00-00_2015-180-01-59-58_1_1_sim.tlm"
+)
+random_packet_def = os.path.join(hs_packet_dir, "apid001", "defs.csv")
 
 
 def test_FixedLength_initializer_copies_field_list():
     """Tests that the FixedLengthPacket initializer stores a copy of the
     provided fields list.
     """
     fields = [PacketField(name="mnemonic", data_type="uint", bit_length=BITS_PER_BYTE)]
@@ -93,14 +102,39 @@
 def test_FixedLength_from_file_not_supported(filename):
     """Test that if given an unsupported filetype raises an error"""
     with pytest.raises(ValueError):
         FixedLength.from_file(filename)
 
 
 @pytest.mark.parametrize(
+    "shape_str, expected_value",
+    [
+        ("uint(4)", 4),
+        ("uint(1, 2)", (1, 2)),
+        ("uint(expand)", "expand"),
+        ("uint(OPMODE)", "OPMODE"),
+    ],
+)
+def test_parse_csv_array_shape(shape_str, expected_value):
+    assert _parse_csv_array_shape(shape_str) == expected_value
+
+
+def test_parse_csv_array_shape_fails_on_invalid_shape_str():
+    with pytest.raises(ValueError):
+        _parse_csv_array_shape("uint(4, FIELD)")
+
+
+def test_VariableLength_from_file():
+    """Test that from_file returns a VariableLength instance"""
+    assert isinstance(VariableLength.from_file(csv_file_3col_with_expand), VariableLength)
+    assert isinstance(VariableLength.from_file(csv_file_3col_with_reference), VariableLength)
+    assert isinstance(VariableLength.from_file(csv_file_3col_with_all), VariableLength)
+
+
+@pytest.mark.parametrize(
     "cls,numpy_dtype,ccsdspy_data_type,ccsdspy_bit_length,array_order,include_bit_offset",
     [
         (FixedLength, ">f4", "float", 32, "C", False),
         (FixedLength, ">f4", "float", 32, "F", False),
         (FixedLength, ">u2", "uint", 16, "C", False),
         (FixedLength, ">u2", "uint", 16, "F", False),
         (FixedLength, ">u8", "uint", 64, "C", False),
@@ -225,7 +259,16 @@
                     array_shape="expand",
                     data_type="uint",
                     bit_length=BITS_PER_BYTE,
                     bit_offset=32,
                 ),
             ]
         )
+
+
+def test_load_without_moving_file_buffer_pos():
+    """Tests that load(..., reset_file_obj=True) works as intended."""
+    pkts = FixedLength.from_file(random_packet_def)
+    with open(random_binary_file, "rb") as fp:
+        pos = fp.tell()
+        pkts.load(fp, reset_file_obj=True)
+        assert pos == fp.tell()
```

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/test_primary_header.py` & `ccsdspy-1.3.0/ccsdspy/tests/test_primary_header.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/test_regression.py` & `ccsdspy-1.3.0/ccsdspy/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/test_split.py` & `ccsdspy-1.3.0/ccsdspy/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/test_utils.py` & `ccsdspy-1.3.0/ccsdspy/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Tests for the ccsdspy.utils packate
 
 Tests for utils.split_by_apid() can be found in test_split.py
 """
+
 import glob
 import io
 import os
 
 import numpy as np
 import pytest
```

### Comparing `ccsdspy-1.2.1/ccsdspy/tests/test_var_length.py` & `ccsdspy-1.3.0/ccsdspy/tests/test_var_length.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy/utils.py` & `ccsdspy-1.3.0/ccsdspy/utils.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/ccsdspy.egg-info/PKG-INFO` & `ccsdspy-1.3.0/ccsdspy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccsdspy
-Version: 1.2.1
+Version: 1.3.0
 Summary: IO Interface for Reading CCSDS Data in Python.
 Author-email: Daniel da Silva <mail@danieldasilva.org>, Steven Christe <steven.d.christe@nasa.gov>
 License: Copyright (c) 2018, Daniel da Silva
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -41,18 +41,18 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 Requires-Dist: numpy>=1.8.0
 Provides-Extra: dev
 Requires-Dist: coverage>=6.5.0; extra == "dev"
-Requires-Dist: pytest>=7.1.3; extra == "dev"
+Requires-Dist: pytest<8.1.0,>=7.1.3; extra == "dev"
 Requires-Dist: pytest-astropy; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: black>=22.10.0; extra == "dev"
+Requires-Dist: black==22.10.0; extra == "dev"
 Requires-Dist: flake8>=5.0.4; extra == "dev"
 Requires-Dist: coverage[toml]; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx>=5.2.3; extra == "docs"
 Requires-Dist: sphinx-automodapi>=0.14.1; extra == "docs"
 Requires-Dist: graphviz>=0.20.1; extra == "docs"
 Requires-Dist: numpydoc; extra == "docs"
@@ -76,20 +76,26 @@
 	  
 This community-developed package provides a Python interface for reading tightly packed bits in the `Consultative Committee for Space Data Systems (CCSDS) <https://public.ccsds.org/default.aspx>`__ format used by many NASA and ESA missions. The library is developed with requirements sourced from the community and extensive automated testing.
 
 Used By
 -------
 .. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/goes-r.png
     :target: https://www.goes-r.gov/
+.. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/europa-clipper.png
+    :target: https://europa.nasa.gov/	     
+.. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/mms.jpg
+    :target: https://mms.gsfc.nasa.gov/
+.. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/pace.png
+    :target: https://pace.gsfc.nasa.gov/
 .. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/hermes.png
     :target: https://science.nasa.gov/missions/hermes
+.. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/csa.png
+    :target: https://www.asc-csa.gc.ca/eng/	     
 .. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/punch.png
     :target: https://punch.space.swri.edu/
-.. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/mms.jpg
-    :target: https://mms.gsfc.nasa.gov/
 .. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/spherex.png
     :target: https://www.jpl.nasa.gov/missions/spherex
 .. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/elfin.jpg
     :target: https://elfin.igpp.ucla.edu/
 .. image:: https://raw.githubusercontent.com/ccsdspy/ccsdspy/main/docs/_static/used-by/small/padre.png
     :target: https://padre.ssl.berkeley.edu
 
@@ -116,21 +122,21 @@
    
    pkt = ccsdspy.FixedLength([
         PacketField(name='SHCOARSE', data_type='uint', bit_length=32),
         PacketField(name='SHFINE',   data_type='uint', bit_length=20),
         PacketField(name='OPMODE',   data_type='uint', bit_length=3),
         PacketField(name='SPACER',   data_type='fill', bit_length=1),
         PacketField(name='VOLTAGE',  data_type='int',  bit_length=8),
-	PacketArray(
+        PacketArray(
             name='SENSOR_GRID',
             data_type='uint',
             bit_length=16,
             array_shape=(32, 32),
             array_order='C'
-	),
+        ),
    ])
    
    result = pkt.load('mypackets.bin')
 
 Documentation
 =============
 Our documentation is hosted on readthedocs and can be found `here <https://ccsdspy.readthedocs.io/en/latest/>`__.
```

### Comparing `ccsdspy-1.2.1/ccsdspy.egg-info/SOURCES.txt` & `ccsdspy-1.3.0/ccsdspy.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -18,23 +18,53 @@
 ccsdspy/utils.py
 ccsdspy.egg-info/PKG-INFO
 ccsdspy.egg-info/SOURCES.txt
 ccsdspy.egg-info/dependency_links.txt
 ccsdspy.egg-info/requires.txt
 ccsdspy.egg-info/top_level.txt
 ccsdspy/tests/__init__.py
+ccsdspy/tests/test_byte_order.py
 ccsdspy/tests/test_converters.py
 ccsdspy/tests/test_hs.py
 ccsdspy/tests/test_packet_fields.py
 ccsdspy/tests/test_packet_types.py
 ccsdspy/tests/test_primary_header.py
 ccsdspy/tests/test_regression.py
 ccsdspy/tests/test_split.py
 ccsdspy/tests/test_utils.py
 ccsdspy/tests/test_var_length.py
+ccsdspy/tests/data/byte_order/byte_order_packets.py
+ccsdspy/tests/data/byte_order/byteorder_1.bin
+ccsdspy/tests/data/byte_order/byteorder_1.csv
+ccsdspy/tests/data/byte_order/byteorder_12.bin
+ccsdspy/tests/data/byte_order/byteorder_12.csv
+ccsdspy/tests/data/byte_order/byteorder_123.bin
+ccsdspy/tests/data/byte_order/byteorder_123.csv
+ccsdspy/tests/data/byte_order/byteorder_1234.bin
+ccsdspy/tests/data/byte_order/byteorder_1234.csv
+ccsdspy/tests/data/byte_order/byteorder_123456.bin
+ccsdspy/tests/data/byte_order/byteorder_123456.csv
+ccsdspy/tests/data/byte_order/byteorder_1234567.bin
+ccsdspy/tests/data/byte_order/byteorder_1234567.csv
+ccsdspy/tests/data/byte_order/byteorder_12345678.bin
+ccsdspy/tests/data/byte_order/byteorder_12345678.csv
+ccsdspy/tests/data/byte_order/byteorder_21.bin
+ccsdspy/tests/data/byte_order/byteorder_21.csv
+ccsdspy/tests/data/byte_order/byteorder_2143.bin
+ccsdspy/tests/data/byte_order/byteorder_2143.csv
+ccsdspy/tests/data/byte_order/byteorder_321.bin
+ccsdspy/tests/data/byte_order/byteorder_321.csv
+ccsdspy/tests/data/byte_order/byteorder_3412.bin
+ccsdspy/tests/data/byte_order/byteorder_3412.csv
+ccsdspy/tests/data/byte_order/byteorder_4321.bin
+ccsdspy/tests/data/byte_order/byteorder_4321.csv
+ccsdspy/tests/data/byte_order/byteorder_78563412.bin
+ccsdspy/tests/data/byte_order/byteorder_78563412.csv
+ccsdspy/tests/data/byte_order/byteorder_87654321.bin
+ccsdspy/tests/data/byte_order/byteorder_87654321.csv
 ccsdspy/tests/data/csa/apid00400.tlm
 ccsdspy/tests/data/europa_clipper/apid01216.tlm
 ccsdspy/tests/data/europa_clipper/apid01217.tlm
 ccsdspy/tests/data/europa_clipper/apid01219.tlm
 ccsdspy/tests/data/europa_clipper/apid01223.tlm
 ccsdspy/tests/data/europa_clipper/apid01227.tlm
 ccsdspy/tests/data/europa_clipper/apid01232.tlm
@@ -51,18 +81,21 @@
 ccsdspy/tests/data/hs/apid130/defs.csv
 ccsdspy/tests/data/hs/apid251/SSAT1_2015-180-00-00-00_2015-180-01-59-59_251_1_sim.tlm
 ccsdspy/tests/data/hs/apid251/defs.csv
 ccsdspy/tests/data/hs/apid895/SSAT1_2015-180-00-00-00_2015-180-01-59-56_895_1_sim.tlm
 ccsdspy/tests/data/hs/apid895/defs.csv
 ccsdspy/tests/data/hs/attic/SSAT_Mnemonics.csv
 ccsdspy/tests/data/hs/attic/_expand_mnemnonics.py
-ccsdspy/tests/data/packet_def/simple_csv_3col.csv
-ccsdspy/tests/data/packet_def/simple_csv_3col_with_array.csv
-ccsdspy/tests/data/packet_def/simple_csv_4col.csv
-ccsdspy/tests/data/packet_def/simple_csv_4col_with_array.csv
+ccsdspy/tests/data/packet_def/basic_csv_3col.csv
+ccsdspy/tests/data/packet_def/basic_csv_3col_with_all.csv
+ccsdspy/tests/data/packet_def/basic_csv_3col_with_array.csv
+ccsdspy/tests/data/packet_def/basic_csv_3col_with_expand.csv
+ccsdspy/tests/data/packet_def/basic_csv_3col_with_reference.csv
+ccsdspy/tests/data/packet_def/extended_csv_4col.csv
+ccsdspy/tests/data/packet_def/extended_csv_4col_with_array.csv
 ccsdspy/tests/data/split/CYGNSS_F7_L0_2022_086_10_15_V01_F__first101pkts.tlm
 ccsdspy/tests/data/split/apid00384.tlm
 ccsdspy/tests/data/split/apid00386.tlm
 ccsdspy/tests/data/split/apid00391.tlm
 ccsdspy/tests/data/split/apid00392.tlm
 ccsdspy/tests/data/split/apid00393.tlm
 ccsdspy/tests/data/split/apid00394.tlm
@@ -137,34 +170,41 @@
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/requirements.txt
 docs/_static/logo.png
+docs/_static/used-by/csa.png
 docs/_static/used-by/elfin.jpg
+docs/_static/used-by/europa-clipper.png
 docs/_static/used-by/goes-r.png
 docs/_static/used-by/hermes.png
 docs/_static/used-by/mms.jpg
+docs/_static/used-by/pace.png
 docs/_static/used-by/padre.png
 docs/_static/used-by/punch.png
 docs/_static/used-by/resize.sh
 docs/_static/used-by/spherex.png
+docs/_static/used-by/small/csa.png
 docs/_static/used-by/small/elfin.jpg
+docs/_static/used-by/small/europa-clipper.png
 docs/_static/used-by/small/goes-r.png
 docs/_static/used-by/small/hermes.png
 docs/_static/used-by/small/mms.jpg
+docs/_static/used-by/small/pace.png
 docs/_static/used-by/small/padre.png
 docs/_static/used-by/small/punch.png
 docs/_static/used-by/small/spherex.png
 docs/_templates/github.html
 docs/_templates/logo.html
 docs/dev-guide/index.rst
 docs/user-guide/ccsds.rst
 docs/user-guide/converters.rst
 docs/user-guide/fixedlength.rst
 docs/user-guide/index.rst
+docs/user-guide/loadfile.rst
 docs/user-guide/packetfields.rst
 docs/user-guide/utils.rst
 docs/user-guide/variablelength.rst
 docs/whatsnew/changelog.rst
 docs/whatsnew/index.rst
```

### Comparing `ccsdspy-1.2.1/docs/Makefile` & `ccsdspy-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/_static/logo.png` & `ccsdspy-1.3.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/_static/used-by/elfin.jpg` & `ccsdspy-1.3.0/docs/_static/used-by/elfin.jpg`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/_static/used-by/goes-r.png` & `ccsdspy-1.3.0/docs/_static/used-by/goes-r.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/_static/used-by/hermes.png` & `ccsdspy-1.3.0/docs/_static/used-by/hermes.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/_static/used-by/mms.jpg` & `ccsdspy-1.3.0/docs/_static/used-by/mms.jpg`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/_static/used-by/padre.png` & `ccsdspy-1.3.0/docs/_static/used-by/padre.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/_static/used-by/punch.png` & `ccsdspy-1.3.0/docs/_static/used-by/punch.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/_static/used-by/small/elfin.jpg` & `ccsdspy-1.3.0/docs/_static/used-by/small/elfin.jpg`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/_static/used-by/small/goes-r.png` & `ccsdspy-1.3.0/docs/_static/used-by/small/goes-r.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/_static/used-by/small/hermes.png` & `ccsdspy-1.3.0/docs/_static/used-by/small/hermes.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/_static/used-by/small/mms.jpg` & `ccsdspy-1.3.0/docs/_static/used-by/small/mms.jpg`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/_static/used-by/small/padre.png` & `ccsdspy-1.3.0/docs/_static/used-by/small/padre.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/_static/used-by/small/punch.png` & `ccsdspy-1.3.0/docs/_static/used-by/small/punch.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/_static/used-by/small/spherex.png` & `ccsdspy-1.3.0/docs/_static/used-by/small/spherex.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/_static/used-by/spherex.png` & `ccsdspy-1.3.0/docs/_static/used-by/spherex.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/conf.py` & `ccsdspy-1.3.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 html_theme_options = {
     "description": "A Python package for reading CCSDS packet data.",
     "show_related": True,
-    "github_banner": True,
+    "github_banner": False,
     "github_button": False,
     "github_user": "ccsdspy",
     "github_repo": "ccsdspy",
     "extra_nav_links": {"CCSDS Blue Books": "https://public.ccsds.org/publications/bluebooks.aspx"},
 }
 
 # Add any paths that contain custom static files (such as style sheets) here,
```

### Comparing `ccsdspy-1.2.1/docs/dev-guide/index.rst` & `ccsdspy-1.3.0/docs/dev-guide/index.rst`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/index.rst` & `ccsdspy-1.3.0/docs/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -30,27 +30,34 @@
    dev-guide/index
    api
 
 Used By
 -------
 .. image:: _static/used-by/small/goes-r.png
     :target: https://www.goes-r.gov/
+.. image:: _static/used-by/small/europa-clipper.png
+    :target: https://europa.nasa.gov/
+.. image:: _static/used-by/small/mms.jpg
+    :target: https://mms.gsfc.nasa.gov/
+.. image:: _static/used-by/small/pace.png
+    :target: https://pace.gsfc.nasa.gov/
 .. image:: _static/used-by/small/hermes.png
     :target: https://science.nasa.gov/missions/hermes
+.. image:: _static/used-by/small/csa.png
+    :target: https://www.asc-csa.gc.ca/eng/
 .. image:: _static/used-by/small/punch.png
-    :target: https://punch.space.swri.edu/
-.. image:: _static/used-by/small/mms.jpg
-    :target: https://mms.gsfc.nasa.gov/
+    :target: https://punch.space.swri.edu/	     
 .. image:: _static/used-by/small/spherex.png
     :target: https://www.jpl.nasa.gov/missions/spherex
 .. image:: _static/used-by/small/elfin.jpg
     :target: https://elfin.igpp.ucla.edu/
 .. image:: _static/used-by/small/padre.png
     :target: https://padre.ssl.berkeley.edu
-
+	     
+	     
 Do you know of other missions that use CCSDSPy? Let us know `through a github issue`_!
 
 .. _through a github issue: https://github.com/ccsdspy/ccsdspy/issues/new
 
 Install ccsdspy
 ---------------
 To install ccsdspy from source, you can use
```

### Comparing `ccsdspy-1.2.1/docs/make.bat` & `ccsdspy-1.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/user-guide/ccsds.rst` & `ccsdspy-1.3.0/docs/user-guide/ccsds.rst`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/user-guide/converters.rst` & `ccsdspy-1.3.0/docs/user-guide/converters.rst`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/user-guide/fixedlength.rst` & `ccsdspy-1.3.0/docs/user-guide/fixedlength.rst`

 * *Files 14% similar despite different names*

```diff
@@ -29,24 +29,16 @@
         PacketField(name='SHFINE',   data_type='uint', bit_length=20),
         PacketField(name='OPMODE',   data_type='uint', bit_length=3),
         PacketField(name='SPACER',   data_type='fill', bit_length=1),
         PacketField(name='VOLTAGE',  data_type='int',  bit_length=8)
    ])
 
 Note that the CCSDS header need not be included as it is included by default.
-A packet need not be defined in code.
-It can also be defined in a text file.
-For example,
 
-With this file, it is then possible to define the packet object with
-
-.. code-block:: python
-
-   import ccsdspy
-   pkt = ccsdspy.FixedLength.from_file('packet_definition.csv')
+Alternatively, fixed length packets can be :ref:`loaded from a CSV file <loadfile>`.
 
 Parsing a file
 ==============
 Once a `~ccsdspy.FixedLength` object is defined, it can be used to read a binary file containing those packets.
 
 .. code-block:: python
```

### Comparing `ccsdspy-1.2.1/docs/user-guide/packetfields.rst` & `ccsdspy-1.3.0/docs/user-guide/packetfields.rst`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/user-guide/utils.rst` & `ccsdspy-1.3.0/docs/user-guide/utils.rst`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.2.1/docs/user-guide/variablelength.rst` & `ccsdspy-1.3.0/docs/user-guide/variablelength.rst`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 
     result = pkt.load('MyCCSDS.bin')
 
 The result will be a dictionary with the names as the keys.
 The values are arrays with the `~ccsdspy.PacketArray` field providing arrays with variable sizes.
 It is also possible to get access to the packet primary header. See :ref:`getting-header`.
 
+.. warning::
+    `bit_offset` cannot be specified for variable length packets. Instead, the packet definition must define all packets, and the bit offsets are calculated automatically.
+
 .. contents::
    :depth: 2
 
 Reference-based Variable Length Field
 =====================================
 An example of using a reference-based variable length field called `data1` which gets the number of elements from another field called `data1_len` is below, and similar for `data2` and `data2_len`. There is not a limit to the number of reference-based variable length fields in a packet definition.
```

### Comparing `ccsdspy-1.2.1/pyproject.toml` & `ccsdspy-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 dependencies = [
   'numpy>=1.8.0',
 ]
 
 [project.optional-dependencies]
 dev = [
   'coverage>=6.5.0',
-  'pytest>=7.1.3',
+  'pytest>=7.1.3, <8.1.0',
   'pytest-astropy',
   'pytest-cov',
-  'black>=22.10.0',
+  'black==22.10.0',
   'flake8>=5.0.4',
   'coverage[toml]'
 ]
 
 docs = [
   'sphinx>=5.2.3',
   'sphinx-automodapi>=0.14.1',
@@ -57,15 +57,15 @@
 [tool.setuptools_scm]
 write_to = "ccsdspy/_version.py"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = ["ccsdspy/tests", "docs"]
 norecursedirs = ["build", "docs/_build", "docs/generated", "*.egg-info", "attic"]
-doctest_plus = "enabled"
+#doctest_plus = "enabled"
 text_file_format = "rst"
 addopts = "--doctest-modules"
 collect_ignore_glob= ['_*.py']
 filterwarnings = [
   "ignore::UserWarning",
   "ignore::DeprecationWarning",
   # This is due to dependencies building with a numpy version different from
```


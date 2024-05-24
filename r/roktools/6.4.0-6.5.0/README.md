# Comparing `tmp/roktools-6.4.0.tar.gz` & `tmp/roktools-6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roktools-6.4.0.tar", max compression
+gzip compressed data, was "roktools-6.5.0.tar", max compression
```

## Comparing `roktools-6.4.0.tar` & `roktools-6.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1067 2024-05-17 06:27:00.966726 roktools-6.4.0/LICENSE
--rw-r--r--   0        0        0     1665 2024-05-17 06:27:00.966726 roktools-6.4.0/README.md
--rw-r--r--   0        0        0     1162 2024-05-17 06:27:00.966726 roktools-6.4.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-17 06:27:00.966726 roktools-6.4.0/roktools/__init__.py
--rw-r--r--   0        0        0     4509 2024-05-17 06:27:00.966726 roktools-6.4.0/roktools/cl.py
--rw-r--r--   0        0        0      133 2024-05-17 06:27:00.966726 roktools-6.4.0/roktools/constants.py
--rw-r--r--   0        0        0      491 2024-05-17 06:27:00.966726 roktools-6.4.0/roktools/decorator.py
--rw-r--r--   0        0        0      933 2024-05-17 06:27:00.966726 roktools-6.4.0/roktools/file.py
--rw-r--r--   0        0        0    33628 2024-05-17 06:27:00.966726 roktools-6.4.0/roktools/geodetic.py
--rw-r--r--   0        0        0        0 2024-05-17 06:27:01.018726 roktools-6.4.0/roktools/gnss/__init__.py
--rw-r--r--   0        0        0     1884 2024-05-17 06:27:00.966726 roktools-6.4.0/roktools/gnss/edit.py
--rw-r--r--   0        0        0     1644 2024-05-17 06:27:00.966726 roktools-6.4.0/roktools/gnss/observables.py
--rw-r--r--   0        0        0     1244 2024-05-17 06:27:00.966726 roktools-6.4.0/roktools/gnss/residuals.py
--rw-r--r--   0        0        0     9572 2024-05-17 06:27:00.966726 roktools-6.4.0/roktools/gnss/types.py
--rw-r--r--   0        0        0     1479 2024-05-17 06:27:00.966726 roktools-6.4.0/roktools/logger.py
--rw-r--r--   0        0        0        0 2024-05-17 06:27:01.018726 roktools-6.4.0/roktools/orbit/__init__.py
--rw-r--r--   0        0        0     1745 2024-05-17 06:27:00.970727 roktools-6.4.0/roktools/orbit/kepler.py
--rw-r--r--   0        0        0     5905 2024-05-17 06:27:00.970727 roktools-6.4.0/roktools/orbit/tle.py
--rw-r--r--   0        0        0        0 2024-05-17 06:27:01.018726 roktools-6.4.0/roktools/parsers/rtklib/__init__,py
--rw-r--r--   0        0        0     5459 2024-05-17 06:27:00.970727 roktools-6.4.0/roktools/parsers/rtklib/stats.py
--rw-r--r--   0        0        0    61455 2024-05-17 06:27:00.970727 roktools-6.4.0/roktools/rinex.py
--rw-r--r--   0        0        0     3057 2024-05-17 06:27:00.970727 roktools-6.4.0/roktools/sinex.py
--rwxr-xr-x   0        0        0     1084 2024-05-17 06:27:00.970727 roktools-6.4.0/roktools/stats.py
--rwxr-xr-x   0        0        0     1598 2024-05-17 06:27:00.970727 roktools-6.4.0/roktools/tensorial.py
--rw-r--r--   0        0        0    11178 2024-05-17 06:27:00.970727 roktools-6.4.0/roktools/time.py
--rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 roktools-6.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-24 17:00:52.576516 roktools-6.5.0/LICENSE
+-rw-r--r--   0        0        0     1665 2024-05-24 17:00:52.576516 roktools-6.5.0/README.md
+-rw-r--r--   0        0        0     1162 2024-05-24 17:00:52.576516 roktools-6.5.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-24 17:00:52.576516 roktools-6.5.0/roktools/__init__.py
+-rw-r--r--   0        0        0     4509 2024-05-24 17:00:52.576516 roktools-6.5.0/roktools/cl.py
+-rw-r--r--   0        0        0      133 2024-05-24 17:00:52.576516 roktools-6.5.0/roktools/constants.py
+-rw-r--r--   0        0        0      491 2024-05-24 17:00:52.576516 roktools-6.5.0/roktools/decorator.py
+-rw-r--r--   0        0        0      933 2024-05-24 17:00:52.576516 roktools-6.5.0/roktools/file.py
+-rw-r--r--   0        0        0    33628 2024-05-24 17:00:52.576516 roktools-6.5.0/roktools/geodetic.py
+-rw-r--r--   0        0        0        0 2024-05-24 17:00:52.628515 roktools-6.5.0/roktools/gnss/__init__.py
+-rw-r--r--   0        0        0     1884 2024-05-24 17:00:52.580515 roktools-6.5.0/roktools/gnss/edit.py
+-rw-r--r--   0        0        0     1644 2024-05-24 17:00:52.580515 roktools-6.5.0/roktools/gnss/observables.py
+-rw-r--r--   0        0        0     1244 2024-05-24 17:00:52.580515 roktools-6.5.0/roktools/gnss/residuals.py
+-rw-r--r--   0        0        0     9572 2024-05-24 17:00:52.580515 roktools-6.5.0/roktools/gnss/types.py
+-rw-r--r--   0        0        0     1479 2024-05-24 17:00:52.580515 roktools-6.5.0/roktools/logger.py
+-rw-r--r--   0        0        0        0 2024-05-24 17:00:52.628515 roktools-6.5.0/roktools/orbit/__init__.py
+-rw-r--r--   0        0        0     1745 2024-05-24 17:00:52.580515 roktools-6.5.0/roktools/orbit/kepler.py
+-rw-r--r--   0        0        0     5905 2024-05-24 17:00:52.580515 roktools-6.5.0/roktools/orbit/tle.py
+-rw-r--r--   0        0        0        0 2024-05-24 17:00:52.628515 roktools-6.5.0/roktools/parsers/rtklib/__init__,py
+-rw-r--r--   0        0        0     5459 2024-05-24 17:00:52.580515 roktools-6.5.0/roktools/parsers/rtklib/stats.py
+-rw-r--r--   0        0        0    66936 2024-05-24 17:00:52.580515 roktools-6.5.0/roktools/rinex.py
+-rw-r--r--   0        0        0     3057 2024-05-24 17:00:52.580515 roktools-6.5.0/roktools/sinex.py
+-rwxr-xr-x   0        0        0     1084 2024-05-24 17:00:52.580515 roktools-6.5.0/roktools/stats.py
+-rwxr-xr-x   0        0        0     1598 2024-05-24 17:00:52.580515 roktools-6.5.0/roktools/tensorial.py
+-rw-r--r--   0        0        0    11178 2024-05-24 17:00:52.580515 roktools-6.5.0/roktools/time.py
+-rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 roktools-6.5.0/PKG-INFO
```

### Comparing `roktools-6.4.0/LICENSE` & `roktools-6.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `roktools-6.4.0/README.md` & `roktools-6.5.0/README.md`

 * *Files identical despite different names*

### Comparing `roktools-6.4.0/pyproject.toml` & `roktools-6.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "roktools"
-version = "6.4.0"
+version = "6.5.0"
 description = "Package with utilities and tools for GNSS data processing"
 authors = ["Rokubun <info@rokubun.cat>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.26.4"
```

### Comparing `roktools-6.4.0/roktools/cl.py` & `roktools-6.5.0/roktools/cl.py`

 * *Files identical despite different names*

### Comparing `roktools-6.4.0/roktools/file.py` & `roktools-6.5.0/roktools/file.py`

 * *Files identical despite different names*

### Comparing `roktools-6.4.0/roktools/geodetic.py` & `roktools-6.5.0/roktools/geodetic.py`

 * *Files identical despite different names*

### Comparing `roktools-6.4.0/roktools/gnss/edit.py` & `roktools-6.5.0/roktools/gnss/edit.py`

 * *Files identical despite different names*

### Comparing `roktools-6.4.0/roktools/gnss/observables.py` & `roktools-6.5.0/roktools/gnss/observables.py`

 * *Files identical despite different names*

### Comparing `roktools-6.4.0/roktools/gnss/residuals.py` & `roktools-6.5.0/roktools/gnss/residuals.py`

 * *Files identical despite different names*

### Comparing `roktools-6.4.0/roktools/gnss/types.py` & `roktools-6.5.0/roktools/gnss/types.py`

 * *Files identical despite different names*

### Comparing `roktools-6.4.0/roktools/logger.py` & `roktools-6.5.0/roktools/logger.py`

 * *Files identical despite different names*

### Comparing `roktools-6.4.0/roktools/orbit/kepler.py` & `roktools-6.5.0/roktools/orbit/kepler.py`

 * *Files identical despite different names*

### Comparing `roktools-6.4.0/roktools/orbit/tle.py` & `roktools-6.5.0/roktools/orbit/tle.py`

 * *Files identical despite different names*

### Comparing `roktools-6.4.0/roktools/parsers/rtklib/stats.py` & `roktools-6.5.0/roktools/parsers/rtklib/stats.py`

 * *Files identical despite different names*

### Comparing `roktools-6.4.0/roktools/rinex.py` & `roktools-6.5.0/roktools/rinex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, fields, asdict
 import datetime
 import enum
 import math
+import numpy as np
 import pandas as pd
 import re
 from typing import Dict, List, Tuple, Union, IO
 import sys
 
 from . import logger
 from . import time
@@ -16,14 +17,26 @@
 from .gnss.types import ConstellationId, Band, TrackingChannel, Satellite
 
 from .orbit.tle import TLE, read_celestrak
 from .orbit.kepler import Kepler
 
 RINEX_LINE_SYS_OBS_TYPES = "SYS / # / OBS TYPES"
 
+RANDOM_STR = 'random'
+ZERO_STR = 'zero'
+
+SAT_STR = 'sat'
+EPOCH_STR = 'epoch'
+A_M_STR = 'a_m'
+ECCENTRICITY_STR = 'eccentricity'
+INCLINATION_DEG_STR = 'inclination_deg'
+RIGHT_ASCENSION_DEG_STR = 'raan_deg'
+ARG_PERIGEE_DEG_STR = 'arg_perigee_deg'
+TRUE_ANOMALY_DEG_STR = 'true_anomaly_deg'
+
 RINEX_BAND_MAP = {
     ConstellationId.GPS: {
         '1': Band.L1,
         '2': Band.L2,
         '5': Band.L5
     },
     ConstellationId.GLONASS: {
@@ -166,14 +179,124 @@
 
 @dataclass
 class Clock(object):
     bias_s: float
     drift_s_per_s: float
     drift_rate_s_per_s2: float
 
+    ref_epoch: datetime = None
+
+
+class ClockModel(ABC):
+    """
+    This abstract class provides with an interface to provide with a Clock model
+    """
+
+    @abstractmethod
+    def get_clock(self, satellite: Satellite, epoch: datetime.datetime) -> Clock:
+        """
+        Get the clock for a satellite and an epoch
+        """
+        pass
+
+
+class ZeroClockModel(ClockModel):
+    """
+    Clock model with 0 bias and drift
+    """
+
+    def get_clock(self, satellite: Satellite, epoch: datetime.datetime) -> Clock:
+        return Clock(0, 0, 0)
+
+
+class GnssRandomClock(ClockModel):
+    """
+    Generate a clock model with random realizations for the clock bias and
+    drift.
+    """
+
+    def __init__(self, bias_max_s: float = 0.0005, drift_max_s_per_s: float = 1.0e-11):
+        """
+        Initialize the object with the threshold values for the bias and drift.
+        In certain works, the typical values of bias and drift for GPS, Galileo
+        and Beidou are usually contained between -/+0.5ms and-/+1e-11 respectively
+        """
+        self.bias_max_s = bias_max_s
+        self.drift_max_s_per_s = drift_max_s_per_s
+
+        # Internal memory to store the state of the previous clock
+        self.clocks = {}
+
+    def get_clock(self, satellite: Satellite, epoch: datetime.datetime) -> Clock:
+
+        clock = self.clocks.get(satellite, None)
+
+        if clock is None:
+            bias_s = np.random.uniform(low=-self.bias_max_s, high=self.bias_max_s)
+            drift_s_per_s = np.random.uniform(low=-self.drift_max_s_per_s, high=self.drift_max_s_per_s)
+
+            clock = Clock(bias_s, drift_s_per_s, 0.0, ref_epoch=epoch)
+
+            self.clocks[satellite] = clock
+
+        # Compute the bias for the updated clock
+        dt = (epoch - clock.ref_epoch).total_seconds() if clock.ref_epoch else 0.0
+        clock = Clock(clock.bias_s + clock.drift_s_per_s * dt, clock.drift_s_per_s, 0.0)
+
+        return clock
+
+
+@dataclass
+class CodeBiases(ABC):
+    """
+    This abstract class provides with an interface to provide with the code biases
+    """
+
+    @abstractmethod
+    def get_base_tgd(self) -> float:
+        """
+        Get the base group delay
+        """
+        return 0.0
+
+    @abstractmethod
+    def get_code_bias(self, channel: TrackingChannel) -> float:
+        """
+        Get the code bias for the given channel
+        """
+        return 0.0
+
+
+class ZeroCodeBiases(CodeBiases):
+
+    def get_base_tgd(self) -> float:
+        return super().get_base_tgd()
+
+    def get_code_bias(self, channel: TrackingChannel) -> float:
+        return super().get_code_bias(channel)
+
+@dataclass
+class LEOCodeBiases(CodeBiases):
+    """
+    Class to handle the code biases for the generic LEO constellation
+    """
+    tgd_s: float
+    isc_s9c_s: float
+
+    def get_base_tgd(self) -> float:
+        return self.tgd_s
+
+    @abstractmethod
+    def get_code_bias(self, channel: TrackingChannel) -> float:
+
+        if channel == TrackingChannel.from_string('9C'):
+            return self.isc_s9c_s
+
+        raise ValueError(f'Tracking channel [ {channel} ] not supported by LEO constellations')
+
 
 @dataclass
 class Record(object):
     epoch: datetime.datetime
     sat: Satellite
     channel: TrackingChannel
     range: float
@@ -1345,15 +1468,15 @@
 
 
 class Nav(object):
     """
     Class that holds Rinex Navigation data
     """
 
-    RINEX4_EPH_BLOCK_LINES_LEO = 6
+    RINEX4_EPH_BLOCK_LINES_LEO = 8
 
     RINEX4_EPH_BLOCK_LINES = {
         EphType.GPS_LNAV: 8,
         EphType.GPS_CNAV: 9,
         EphType.GPS_CNV2: 10,
         EphType.GAL_INAV: 8,
         EphType.GAL_FNAV: 8,
@@ -1508,29 +1631,29 @@
         out = "     4.99           NAVIGATION DATA     M                   RINEX VERSION / TYPE\n"
         out = out + f"{pgm.ljust(20)}rokubun             {epoch_str}PGM / RUN BY / DATE\n"
         out = out + "    18                                                      LEAP SECONDS\n"
         out = out + "                                                            END OF HEADER\n"
         return out
 
     @staticmethod
-    def create_navblock(satellite: Satellite, orbit: Kepler, sat_clock: Clock) -> RawNavBlock:
+    def create_navblock(satellite: Satellite, orbit: Kepler, sat_clock: Clock, code_biases: CodeBiases) -> RawNavBlock:
 
         WRITERS = {
             ConstellationId.STARLINK: Nav.create_leo_navblock,
             ConstellationId.SPIRE: Nav.create_leo_navblock,
             ConstellationId.LEO: Nav.create_leo_navblock,
             ConstellationId.ONEWEB: Nav.create_leo_navblock
         }
 
         writer = WRITERS.get(satellite.constellation, None)
         if writer:
-            return writer(satellite, orbit, sat_clock)
+            return writer(satellite, orbit, sat_clock, code_biases)
 
     @staticmethod
-    def create_leo_navblock(satellite: Satellite, orbit: Kepler, sat_clock: Clock) -> RawNavBlock:
+    def create_leo_navblock(satellite: Satellite, orbit: Kepler, sat_clock: Clock, biases: CodeBiases) -> RawNavBlock:
         """
         Output a RINEX4 navigation block from a set of orbit and clock parameters
         """
 
         lines = []
 
         # Header line
@@ -1577,57 +1700,76 @@
 
         # ORBIT - 5
         void = 0.0
         idot = 0.0
         delta_n_dot = orbit.delta_n_dot_rad_per_s
         lines.append(Nav._write_orbit_line(idot, delta_n_dot, weektow.week, void))
 
+        # ORBIT - 6
+        lines.append(Nav._write_orbit_line(void, void, biases.get_base_tgd(), void))
+
+        # ORBIT - 7
+        channel = TrackingChannel.from_string('9C')  # May depend on the LEO constellation
+        lines.append(Nav._write_orbit_line(biases.get_code_bias(channel), void, void, void))
+
         return RawNavBlock(satellite, orbit.toe, lines)
 
     @staticmethod
     @process_filename_or_file_handler('w')
-    def write_from_tle(output, tle_list: List[TLE], rinex2=False) -> None:
+    def write_from_tle(output, tle_list: List[TLE], rinex2=False, sat_clock_model=ZeroClockModel(), code_biases=ZeroCodeBiases()) -> None:
 
         output.write(Nav.create_header(pgm='rinex_from_file'))
 
         for tle in tle_list:
 
-            # Find the clock if available
-            sat_clock = Clock(0, 0, 0)
             try:
                 satellite = tle.get_satellite()
                 orbit = tle.to_kepler()
-                nav_block = Nav.create_navblock(satellite, orbit, sat_clock)
+                sat_clock = sat_clock_model.get_clock(satellite, tle.toe)
+                nav_block = Nav.create_navblock(satellite, orbit, sat_clock, code_biases)
 
                 output.write(nav_block.to_rinex2() if rinex2 else str(nav_block))
                 output.write('\n')
             except ValueError as e:
                 logger.warning(e)
                 continue
 
     @staticmethod
     @process_filename_or_file_handler('w')
-    def write_from_dataframe(output, df: pd.DataFrame, rinex2=False) -> None:
+    def write_from_dataframe(output, df: pd.DataFrame, rinex2=False, sat_clock_model=ZeroClockModel(), clock_biases=ZeroCodeBiases()) -> None:
+        f"""
+        Write a RINEX file from the orbital parameters contained in a DataFrame,
+        which should have the following fields
+        - {EPOCH_STR}, with the reference epoch (will be parsed to a datetime)
+        - {SAT_STR}, with the satellite identifier
+        - {A_M_STR}, with the semimajor axis
+        - {ECCENTRICITY_STR} Eccentricity of the orbit (adimensional)
+        - {INCLINATION_DEG_STR} Inclination of the orbit (degrees)
+        - {RIGHT_ASCENSION_DEG_STR} Right ascension of the ascending node (degrees)
+        - {ARG_PERIGEE_DEG_STR} Argument of the perigee (degrees)
+        - {TRUE_ANOMALY_DEG_STR} True anomaly (degrees)
+
+        """
 
         output.write(Nav.create_header(pgm='rinex_from_file'))
 
         df = df.sort_values(by=['epoch', 'sat'], ascending=[True, True])
 
         for _, row in df.iterrows():
 
             try:
                 constellation = ConstellationId.from_string(row.sat[0])
                 prn = int(row.sat[1:])
                 satellite = Satellite(constellation=constellation, prn=prn)
-                sat_clock = Clock(0, 0, 0)
+                sat_clock = sat_clock_model.get_clock(satellite, row.epoch)
                 orbit = Kepler(
                     row.epoch, row.a_m, row.eccentricity,
                     math.radians(row.inclination_deg), math.radians(row.raan_deg),
                     math.radians(row.arg_perigee_deg), math.radians(row.true_anomaly_deg))
-                nav_block = Nav.create_navblock(satellite, orbit, sat_clock)
+                nav_block = Nav.create_navblock(satellite, orbit, sat_clock, clock_biases)
 
                 output.write(nav_block.to_rinex2() if rinex2 else str(nav_block))
                 output.write('\n')
             except Exception as e:
                 logger.warning(e)
                 continue
 
@@ -1720,27 +1862,43 @@
     input_options.add_argument('--celestrak_file', metavar='<filename>', type=str,
                                help='File from Celestrak with the TLE elements to convert to RINEX.' +
                                     'Based on https://arxiv.org/abs/2401.17767')
 
     input_options.add_argument('--csv', metavar='<filename>', type=str,
                                help='CSV file with the description of ')
 
+    parser.add_argument('--clock-model', '-c', choices=[ZERO_STR, RANDOM_STR], required=False,
+                        help="Choose the clock model to be applied to satellites where clock \
+                            bias and drift has not been provided. Defaults to '{ZERO_STR}'")
+
     parser.add_argument('--rinex2', action='store_true',
-                        help='Output the format in Rinex 2 GPS format. Will skip satellites with PRN larger than 99')
+                        help='Output the format in Rinex 2 GPS format. Will skip satellites \
+                            with PRN larger than 99')
 
     # Parse the command-line arguments
     args = parser.parse_args()
 
+    sat_clock_model = ZeroClockModel()
+    if args.clock_model == RANDOM_STR:
+        sat_clock_model = GnssRandomClock()
+
+    code_biases = ZeroCodeBiases()
+    if args.code_biases == RANDOM_STR:
+        TGD_MAX_S = 10.0e-9
+        tgd_s = np.random.uniform(low=-TGD_MAX_S, high=TGD_MAX_S)
+        isc_s9c_s = np.random.uniform(low=-TGD_MAX_S, high=TGD_MAX_S)
+        code_biases = LEOCodeBiases(tgd_s, isc_s9c_s)
+
     if args.celestrak_file:
         tle_list = read_celestrak(args.celestrak_file)
-        Nav.write_from_tle(sys.stdout, tle_list, rinex2=args.rinex2)
+        Nav.write_from_tle(sys.stdout, tle_list, rinex2=args.rinex2, sat_clock_model=sat_clock_model, code_biases=code_biases)
 
     elif args.csv:
         df = pd.read_csv(args.csv, parse_dates=['epoch'])
-        Nav.write_from_dataframe(sys.stdout, df, rinex2=args.rinex2)
+        Nav.write_from_dataframe(sys.stdout, df, rinex2=args.rinex2, sat_clock_model=sat_clock_model, code_biases=code_biases)
 
 
 _ACCURACY_STR = "accuracy"
 _ADOT_STR = "Adot[m/s]"
 _AODC_STR = "aodc"
 _AODE_STR = "aode"
 _B1C_INTEGRITY_FLAGS_STR = "b1c_integrity_flags"
```

### Comparing `roktools-6.4.0/roktools/sinex.py` & `roktools-6.5.0/roktools/sinex.py`

 * *Files identical despite different names*

### Comparing `roktools-6.4.0/roktools/stats.py` & `roktools-6.5.0/roktools/stats.py`

 * *Files identical despite different names*

### Comparing `roktools-6.4.0/roktools/tensorial.py` & `roktools-6.5.0/roktools/tensorial.py`

 * *Files identical despite different names*

### Comparing `roktools-6.4.0/roktools/time.py` & `roktools-6.5.0/roktools/time.py`

 * *Files identical despite different names*

### Comparing `roktools-6.4.0/PKG-INFO` & `roktools-6.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roktools
-Version: 6.4.0
+Version: 6.5.0
 Summary: Package with utilities and tools for GNSS data processing
 Author: Rokubun
 Author-email: info@rokubun.cat
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


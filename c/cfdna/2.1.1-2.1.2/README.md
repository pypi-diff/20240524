# Comparing `tmp/cfdna-2.1.1.tar.gz` & `tmp/cfdna-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfdna-2.1.1.tar", max compression
+gzip compressed data, was "cfdna-2.1.2.tar", max compression
```

## Comparing `cfdna-2.1.1.tar` & `cfdna-2.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rwxr-xr-x   0        0        0    17895 2022-07-20 16:09:08.000000 cfdna-2.1.1/LICENSE.md
--rwxr-xr-x   0        0        0     1341 2023-11-21 14:09:42.209706 cfdna-2.1.1/README.md
--rw-r--r--   0        0        0     8196 2024-05-14 15:11:34.093762 cfdna-2.1.1/cfdna/.DS_Store
--rwxr-xr-x   0        0        0      638 2024-05-15 18:27:16.441217 cfdna-2.1.1/cfdna/__init__.py
--rwxr-xr-x   0        0        0     4486 2024-04-16 02:05:12.659608 cfdna-2.1.1/cfdna/__main__.py
--rwxr-xr-x   0        0        0       69 2022-07-20 16:09:08.000000 cfdna-2.1.1/cfdna/commandline/__init__.py
--rwxr-xr-x   0        0        0     8733 2024-05-15 18:27:00.233103 cfdna-2.1.1/cfdna/commandline/commands.py
--rwxr-xr-x   0        0        0       64 2022-08-30 19:13:58.000000 cfdna-2.1.1/cfdna/core/__init__.py
--rwxr-xr-x   0        0        0     2918 2023-11-06 18:52:38.951861 cfdna-2.1.1/cfdna/core/core.py
--rw-r--r--   0        0        0     6148 2023-11-06 14:19:28.230169 cfdna-2.1.1/cfdna/io/.DS_Store
--rwxr-xr-x   0        0        0      281 2022-07-20 16:09:09.000000 cfdna-2.1.1/cfdna/io/__init__.py
--rwxr-xr-x   0        0        0      184 2022-07-20 16:09:09.000000 cfdna-2.1.1/cfdna/io/read/__init__.py
--rwxr-xr-x   0        0        0     1762 2023-02-03 15:34:27.663648 cfdna-2.1.1/cfdna/io/read/read_bam.py
--rwxr-xr-x   0        0        0      491 2023-11-06 18:42:33.912191 cfdna-2.1.1/cfdna/io/read/read_h5.py
--rwxr-xr-x   0        0        0      190 2022-07-20 16:09:09.000000 cfdna-2.1.1/cfdna/io/write/__init__.py
--rwxr-xr-x   0        0        0      511 2023-11-06 18:43:44.583371 cfdna-2.1.1/cfdna/io/write/write_h5.py
--rwxr-xr-x   0        0        0      849 2022-07-20 16:09:09.000000 cfdna-2.1.1/cfdna/io/write/write_text.py
--rwxr-xr-x   0        0        0       67 2022-07-20 16:09:08.000000 cfdna-2.1.1/cfdna/plot/__init__.py
--rwxr-xr-x   0        0        0     7663 2022-07-20 16:09:09.000000 cfdna-2.1.1/cfdna/plot/plot_bokeh.py
--rwxr-xr-x   0        0        0      990 2023-11-07 16:01:23.498388 cfdna-2.1.1/cfdna/plot/plot_plt.py
--rwxr-xr-x   0        0        0      391 2022-10-05 14:16:05.000000 cfdna-2.1.1/cfdna/tools/__init__.py
--rwxr-xr-x   0        0        0      167 2023-11-06 18:36:25.971444 cfdna-2.1.1/cfdna/tools/cnv/__init__.py
--rwxr-xr-x   0        0        0     3563 2023-11-06 18:44:12.544286 cfdna-2.1.1/cfdna/tools/cnv/segmentation.py
--rw-r--r--   0        0        0     1334 2024-03-21 21:01:17.622900 cfdna-2.1.1/cfdna/tools/coverage/gene_activity.py
--rwxr-xr-x   0        0        0      165 2022-07-20 16:09:08.000000 cfdna-2.1.1/cfdna/tools/fragmentation/__init__.py
--rwxr-xr-x   0        0        0     2418 2022-08-30 16:29:27.000000 cfdna-2.1.1/cfdna/tools/fragmentation/frag_pattern.py
--rwxr-xr-x   0        0        0      175 2022-07-20 16:09:08.000000 cfdna-2.1.1/cfdna/tools/nucleosome/__init__.py
--rw-r--r--   0        0        0     4281 2022-10-20 20:27:47.000000 cfdna-2.1.1/cfdna/tools/nucleosome/gene_activity.py
--rwxr-xr-x   0        0        0     8696 2022-08-30 16:32:05.000000 cfdna-2.1.1/cfdna/tools/nucleosome/nfr.py
--rw-r--r--   0        0        0     5375 2022-10-21 19:39:37.000000 cfdna-2.1.1/cfdna/tools/nucleosome/relative_window.py
--rwxr-xr-x   0        0        0     8490 2024-05-09 17:45:05.523659 cfdna-2.1.1/cfdna/tools/nucleosome/wps.py
--rw-r--r--   0        0        0     7053 2022-10-05 14:45:53.000000 cfdna-2.1.1/cfdna/tools/nucleosome/wps_functions.py
--rwxr-xr-x   0        0        0      162 2022-07-20 16:09:08.000000 cfdna-2.1.1/cfdna/tools/summarize/__init__.py
--rw-r--r--   0        0        0     3551 2022-08-30 19:26:15.000000 cfdna-2.1.1/cfdna/tools/summarize/multi_sample.py
--rwxr-xr-x   0        0        0     3417 2023-11-06 18:46:14.639312 cfdna-2.1.1/cfdna/tools/summarize/summarize.py
--rwxr-xr-x   0        0        0      143 2022-07-20 16:09:09.000000 cfdna-2.1.1/cfdna/utilities/__init__.py
--rwxr-xr-x   0        0        0     4289 2022-08-30 19:22:16.000000 cfdna-2.1.1/cfdna/utilities/h5_utilities.py
--rw-r--r--   0        0        0     2474 2024-05-15 18:27:26.456858 cfdna-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     3553 1970-01-01 00:00:00.000000 cfdna-2.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0    17895 2022-07-20 16:09:08.000000 cfdna-2.1.2/LICENSE.md
+-rwxr-xr-x   0        0        0     1341 2023-11-21 14:09:42.209706 cfdna-2.1.2/README.md
+-rw-r--r--   0        0        0     8196 2024-05-24 18:42:49.301777 cfdna-2.1.2/cfdna/.DS_Store
+-rwxr-xr-x   0        0        0      638 2024-05-24 18:50:22.005758 cfdna-2.1.2/cfdna/__init__.py
+-rwxr-xr-x   0        0        0     4486 2024-04-16 02:05:12.659608 cfdna-2.1.2/cfdna/__main__.py
+-rwxr-xr-x   0        0        0       69 2022-07-20 16:09:08.000000 cfdna-2.1.2/cfdna/commandline/__init__.py
+-rwxr-xr-x   0        0        0     8797 2024-05-24 18:46:16.594987 cfdna-2.1.2/cfdna/commandline/commands.py
+-rwxr-xr-x   0        0        0       64 2022-08-30 19:13:58.000000 cfdna-2.1.2/cfdna/core/__init__.py
+-rwxr-xr-x   0        0        0     2918 2023-11-06 18:52:38.951861 cfdna-2.1.2/cfdna/core/core.py
+-rw-r--r--   0        0        0     6148 2023-11-06 14:19:28.230169 cfdna-2.1.2/cfdna/io/.DS_Store
+-rwxr-xr-x   0        0        0      281 2022-07-20 16:09:09.000000 cfdna-2.1.2/cfdna/io/__init__.py
+-rwxr-xr-x   0        0        0      184 2022-07-20 16:09:09.000000 cfdna-2.1.2/cfdna/io/read/__init__.py
+-rwxr-xr-x   0        0        0     1762 2023-02-03 15:34:27.663648 cfdna-2.1.2/cfdna/io/read/read_bam.py
+-rwxr-xr-x   0        0        0      491 2023-11-06 18:42:33.912191 cfdna-2.1.2/cfdna/io/read/read_h5.py
+-rwxr-xr-x   0        0        0      190 2022-07-20 16:09:09.000000 cfdna-2.1.2/cfdna/io/write/__init__.py
+-rwxr-xr-x   0        0        0      511 2023-11-06 18:43:44.583371 cfdna-2.1.2/cfdna/io/write/write_h5.py
+-rwxr-xr-x   0        0        0      849 2022-07-20 16:09:09.000000 cfdna-2.1.2/cfdna/io/write/write_text.py
+-rwxr-xr-x   0        0        0       67 2022-07-20 16:09:08.000000 cfdna-2.1.2/cfdna/plot/__init__.py
+-rwxr-xr-x   0        0        0     7663 2022-07-20 16:09:09.000000 cfdna-2.1.2/cfdna/plot/plot_bokeh.py
+-rwxr-xr-x   0        0        0      990 2023-11-07 16:01:23.498388 cfdna-2.1.2/cfdna/plot/plot_plt.py
+-rwxr-xr-x   0        0        0      391 2022-10-05 14:16:05.000000 cfdna-2.1.2/cfdna/tools/__init__.py
+-rwxr-xr-x   0        0        0      167 2023-11-06 18:36:25.971444 cfdna-2.1.2/cfdna/tools/cnv/__init__.py
+-rwxr-xr-x   0        0        0     3563 2023-11-06 18:44:12.544286 cfdna-2.1.2/cfdna/tools/cnv/segmentation.py
+-rw-r--r--   0        0        0     1334 2024-03-21 21:01:17.622900 cfdna-2.1.2/cfdna/tools/coverage/gene_activity.py
+-rwxr-xr-x   0        0        0      165 2022-07-20 16:09:08.000000 cfdna-2.1.2/cfdna/tools/fragmentation/__init__.py
+-rwxr-xr-x   0        0        0     2418 2022-08-30 16:29:27.000000 cfdna-2.1.2/cfdna/tools/fragmentation/frag_pattern.py
+-rwxr-xr-x   0        0        0      175 2022-07-20 16:09:08.000000 cfdna-2.1.2/cfdna/tools/nucleosome/__init__.py
+-rw-r--r--   0        0        0     4281 2022-10-20 20:27:47.000000 cfdna-2.1.2/cfdna/tools/nucleosome/gene_activity.py
+-rwxr-xr-x   0        0        0     8696 2022-08-30 16:32:05.000000 cfdna-2.1.2/cfdna/tools/nucleosome/nfr.py
+-rw-r--r--   0        0        0     5375 2022-10-21 19:39:37.000000 cfdna-2.1.2/cfdna/tools/nucleosome/relative_window.py
+-rwxr-xr-x   0        0        0    10395 2024-05-23 22:40:55.579719 cfdna-2.1.2/cfdna/tools/nucleosome/wps.py
+-rw-r--r--   0        0        0     7053 2022-10-05 14:45:53.000000 cfdna-2.1.2/cfdna/tools/nucleosome/wps_functions.py
+-rwxr-xr-x   0        0        0      162 2022-07-20 16:09:08.000000 cfdna-2.1.2/cfdna/tools/summarize/__init__.py
+-rw-r--r--   0        0        0     3551 2022-08-30 19:26:15.000000 cfdna-2.1.2/cfdna/tools/summarize/multi_sample.py
+-rwxr-xr-x   0        0        0     3417 2023-11-06 18:46:14.639312 cfdna-2.1.2/cfdna/tools/summarize/summarize.py
+-rwxr-xr-x   0        0        0      143 2022-07-20 16:09:09.000000 cfdna-2.1.2/cfdna/utilities/__init__.py
+-rwxr-xr-x   0        0        0     4289 2022-08-30 19:22:16.000000 cfdna-2.1.2/cfdna/utilities/h5_utilities.py
+-rw-r--r--   0        0        0     2474 2024-05-24 18:54:08.656977 cfdna-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3553 1970-01-01 00:00:00.000000 cfdna-2.1.2/PKG-INFO
```

### Comparing `cfdna-2.1.1/LICENSE.md` & `cfdna-2.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.1/README.md` & `cfdna-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.1/cfdna/.DS_Store` & `cfdna-2.1.2/cfdna/.DS_Store`

 * *Files 8% similar despite different names*

```diff
@@ -260,15 +260,15 @@
 00001030: 00b8 6270 6c69 7374 3030 d601 0203 0405  ..bplist00......
 00001040: 0607 0807 080b 085d 5368 6f77 5374 6174  .......]ShowStat
 00001050: 7573 4261 725b 5368 6f77 546f 6f6c 6261  usBar[ShowToolba
 00001060: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
 00001070: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
 00001080: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
 00001090: 735b 5368 6f77 5369 6465 6261 7208 0908  s[ShowSidebar...
-000010a0: 095f 1018 7b7b 3237 302c 2034 3339 7d2c  ._..{{270, 439},
+000010a0: 095f 1018 7b7b 3231 392c 2033 3035 7d2c  ._..{{219, 305},
 000010b0: 207b 3932 302c 2034 3336 7d7d 0908 1523   {920, 436}}...#
 000010c0: 2f3b 525f 6b6c 6d6e 6f8a 0000 0000 0000  /;R_klmno.......
 000010d0: 0101 0000 0000 0000 000d 0000 0000 0000  ................
 000010e0: 0000 0000 0000 0000 008b 0000 000b 0063  ...............c
 000010f0: 006f 006d 006d 0061 006e 0064 006c 0069  .o.m.m.a.n.d.l.i
 00001100: 006e 0065 7653 726e 6c6f 6e67 0000 0001  .n.evSrnlong....
 00001110: 0000 0004 0063 006f 0072 0065 6277 7370  .....c.o.r.ebwsp
@@ -318,16 +318,16 @@
 000013d0: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
 000013e0: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
 000013f0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00001400: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
 00001410: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
 00001420: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
 00001430: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-00001440: 6261 7208 0908 095f 1018 7b7b 3235 302c  bar...._..{{250,
-00001450: 2033 3336 7d2c 207b 3932 302c 2034 3336   336}, {920, 436
+00001440: 6261 7208 0908 095f 1018 7b7b 3232 302c  bar...._..{{220,
+00001450: 2033 3035 7d2c 207b 3932 302c 2034 3336   305}, {920, 436
 00001460: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
 00001470: 0000 0000 0000 0101 0000 0000 0000 000d  ................
 00001480: 0000 0000 0000 0000 0000 0000 0000 008b  ................
 00001490: 0000 0005 0074 006f 006f 006c 0073 7653  .....t.o.o.l.svS
 000014a0: 726e 6c6f 6e67 0000 0001 0000 0009 0075  rnlong.........u
 000014b0: 0074 0069 006c 0069 0074 0069 0065 0073  .t.i.l.i.t.i.e.s
 000014c0: 6277 7370 626c 6f62 0000 00b7 6270 6c69  bwspblob....bpli
```

### Comparing `cfdna-2.1.1/cfdna/__init__.py` & `cfdna-2.1.2/cfdna/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from . import commandline as cmd
 from . import tools as tl
 
 from ngsfragments import Fragments
 
 
 # This is extracted automatically by the top-level setup.py.
-__version__ = '2.1.1'
+__version__ = '2.1.2'
 
 __author__ = "Kyle S. Smith"
 
 __doc__ = """\
 
 API
 ======
```

### Comparing `cfdna-2.1.1/cfdna/__main__.py` & `cfdna-2.1.2/cfdna/__main__.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.1/cfdna/commandline/commands.py` & `cfdna-2.1.2/cfdna/commandline/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,17 +115,17 @@
         if args.anno_segs:
             sample = os.path.split(prefix)[-1]
             df = cfdna_object.obs_intervals[sample]["cnv_segments"].df
             df.loc[:,"chrom"] = cfdna_object.obs_intervals[sample]["cnv_segments"].index.labels
             df.loc[:,"start"] = cfdna_object.obs_intervals[sample]["cnv_segments"].index.starts
             df.loc[:,"end"] = cfdna_object.obs_intervals[sample]["cnv_segments"].index.ends
             df.loc[:,"sample"] = sample
-            df.loc[:,"bin_size"] = args.bin_size
+            df.loc[:,"n_bins"] = ((df.loc[:,"end"].values - df.loc[:,"start"].values) / args.bin_size).astype(int)
             df = df.loc[:,['sample', 'chrom', 'start', 'end', 'copy_number', 'event', 'subclone_status',
-                           'logR_Copy_Number', 'Corrected_Copy_Number', 'Corrected_Call', 'var', 'bin_size', 'median']]
+                           'logR_Copy_Number', 'Corrected_Copy_Number', 'Corrected_Call', 'var', 'n_bins', 'median']]
             df.to_csv(prefix+"_seg_annotations.seg", header=True, index=False, sep="\t")
 
             # Drop columns
             df.drop(columns=["chrom", "start", "end"], inplace=True)
 
 
 def GeneActivity(args):
```

### Comparing `cfdna-2.1.1/cfdna/core/core.py` & `cfdna-2.1.2/cfdna/core/core.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.1/cfdna/io/.DS_Store` & `cfdna-2.1.2/cfdna/io/.DS_Store`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.1/cfdna/io/read/read_bam.py` & `cfdna-2.1.2/cfdna/io/read/read_bam.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.1/cfdna/io/write/write_text.py` & `cfdna-2.1.2/cfdna/io/write/write_text.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.1/cfdna/plot/plot_bokeh.py` & `cfdna-2.1.2/cfdna/plot/plot_bokeh.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.1/cfdna/plot/plot_plt.py` & `cfdna-2.1.2/cfdna/plot/plot_plt.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.1/cfdna/tools/cnv/segmentation.py` & `cfdna-2.1.2/cfdna/tools/cnv/segmentation.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.1/cfdna/tools/coverage/gene_activity.py` & `cfdna-2.1.2/cfdna/tools/coverage/gene_activity.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.1/cfdna/tools/fragmentation/frag_pattern.py` & `cfdna-2.1.2/cfdna/tools/fragmentation/frag_pattern.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.1/cfdna/tools/nucleosome/gene_activity.py` & `cfdna-2.1.2/cfdna/tools/nucleosome/gene_activity.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.1/cfdna/tools/nucleosome/nfr.py` & `cfdna-2.1.2/cfdna/tools/nucleosome/nfr.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.1/cfdna/tools/nucleosome/relative_window.py` & `cfdna-2.1.2/cfdna/tools/nucleosome/relative_window.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.1/cfdna/tools/nucleosome/wps.py` & `cfdna-2.1.2/cfdna/tools/nucleosome/wps.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import ngsfragments as ngs
 import numpy as np
 import pandas as pd
 from ailist import LabeledIntervalArray
 import scipy
+from scipy.signal import lfilter
+from scipy.stats import trim_mean
+from scipy.signal import periodogram, welch
+from scipy.interpolate import Rbf
 
 
 def wps(frags, chrom=None, protection=120, min_length=120, max_length=210, normalize=True, norm_method="mean"):
     """
     Calculate Window Protection Score (WPS)
 
     Parameters
@@ -224,61 +228,94 @@
 
     # Remove those greater than max_distance
     p_dist = p_dist.iloc[p_dist.df.loc[:,"mean_dist"].values < max_distance, :]
 
     return p_dist
 
 
+def spec_pgram(x, smoothed=False):
+    """
+    """
+    
+    # Compute the periodogram
+    frequencies, power_spectrum = periodogram(x,
+                                              window="hann",
+                                              nfft=None,
+                                              return_onesided=True,
+                                              scaling="density",
+                                              detrend="linear")
+    if smoothed:
+        # Smooth the periodogram using Welch's method
+        frequencies, power_spectrum = welch(x,
+                                          window="hann",
+                                          nperseg=None,
+                                          noverlap=None,
+                                          detrend="linear",
+                                          scaling="density",
+                                          return_onesided=True)
+    return frequencies, power_spectrum
+
+
 def wps_gene_fft(fragments,
                  genome_version = "hg38",
                  protection = 120,
 				 min_length = 120,
                  max_length = 500,
+                 scale = True,
+                 feature = "gene",
                  verbose = False):
     """
     """
 
     import genome_info
 
     genome = genome_info.GenomeInfo(genome_version)
-    genes = genome.get_intervals("tss", downstream=10000, filter_column="gene_type", filter_selection="protein_coding")
+    #genes = genome.get_intervals("tss", downstream=10000, filter_column="gene_type", filter_selection="protein_coding")
+    if feature == "gene":
+        genes = genome.get_intervals("gene", filter_column="gene_type", filter_selection="protein_coding")
+    elif feature == "tss":
+        genes = genome.get_intervals("tss", upstream=5000, downstream=5000, filter_column="gene_type", filter_selection="protein_coding")
+    elif feature == "gene_body":
+        genes = genome.get_intervals("gene", upstream=5000, filter_column="gene_type", filter_selection="protein_coding")
 
     # Iterate over chromosomes
     chroms = fragments.frags.unique_labels
 
     # Initialize scores
-    scores = pd.DataFrame(np.zeros((genes.shape[0], 1000)), index=genes.loc[:,"gene_name"].values)
+    scores = pd.DataFrame(np.zeros((genes.shape[0], 280-120)), index=genes.loc[:,"gene_name"].values)
+    #scores = {}
+    b = np.array([1])
+    a = np.append(1, -(1 / np.arange(5, 100, 4)))
 
     # Iterate over chromosomes
     k = 0
     for chrom in chroms:
         if verbose: print(chrom, flush=True)
         wps = fragments.frags.wps(protection, chrom, min_length, max_length)
         wps[chrom].values[:] = ngs.peak_calling.CallPeaks.normalize_signal(wps[chrom].values)
 
         chrom_genes = genes.loc[chrom,:]
 
         for i in range(chrom_genes.shape[0]):
             interval = chrom_genes.index[i]
-            if len(wps[chrom].loc[interval.start:interval.end-2].values) == 10000:
-                values = wps[chrom].loc[interval.start:interval.end-2].values
-                values = ngs.correct.correction.gaussian_smooth(values, 10)
-                values = values - np.mean(values)
-                values = scipy.signal.detrend(values)
-                #sos = scipy.signal.butter(5,100, btype="highpass", fs=10000, output="sos")
-                #values = scipy.signal.sosfilt(sos, values)
-                values = scipy.fftpack.fft(values)
-                scores.iloc[k,:] = np.abs(values)[:1000]
-            k += 1
-
-
-    #scores.values[chrom_genes.loc[:,"Strand"].values == "-",:] = scores.values[chrom_genes.loc[:,"Strand"].values == "-",:][:,::-1]
-
-    #n = ((scores.T - scores.min(axis=1).values) / (scores.max(axis=1).values - scores.min(axis=1).values)).T
-    #n = n.loc[np.sum(pd.isnull(n), axis=1).values == 0,:]
-
-    #x = np.fft.fft2(n.values)
-    #x = np.fft.fftshift(x)
-
-    #expr = pd.Series(x[:,193:200].mean(axis=1).astype(float), scores.index.values)
+            tdataA1 = wps[chrom].loc[interval.start:interval.end].values
+            x = np.append(tdataA1[:300], tdataA1)
+            tdataA1 = lfilter(b, a, x)[300:]
+            tdataA1 = tdataA1 - trim_mean(tdataA1, 0.1)
+            resA1 = spec_pgram(tdataA1, smoothed=False)
+            freq = 1 / resA1[0][1:]
+            chosen = np.logical_and(freq >= 120, freq <= 280)
+            if chosen.sum() < 5:
+                continue
+            freq = np.round(freq[chosen])
+            fft_values = pd.Series(resA1[1][1:][chosen], index=freq)
+            fft_values = fft_values.groupby(by=fft_values.index.values.astype(int)).mean()
+            #print(fft_values, fft_values.shape, chosen, chosen.sum(), flush=True)
+            interp_func = Rbf(fft_values.index, fft_values.values, smooth=0.1)
+            fft_values = pd.Series(interp_func(np.arange(120-5, 280+5)), index = np.arange(120-5, 280+5))
+            fft_values = fft_values.rolling(window=5, center=True).mean()
+            fft_values = fft_values.loc[np.arange(120, 280)]
+            if scale:
+                fft_values = (fft_values - fft_values.min()) / (fft_values.max() - fft_values.min())
+            scores.loc[chrom_genes.df.loc[:,"gene_name"].values[i],:] = fft_values.values
 
     return scores
```

### Comparing `cfdna-2.1.1/cfdna/tools/nucleosome/wps_functions.py` & `cfdna-2.1.2/cfdna/tools/nucleosome/wps_functions.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.1/cfdna/tools/summarize/multi_sample.py` & `cfdna-2.1.2/cfdna/tools/summarize/multi_sample.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.1/cfdna/tools/summarize/summarize.py` & `cfdna-2.1.2/cfdna/tools/summarize/summarize.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.1/cfdna/utilities/h5_utilities.py` & `cfdna-2.1.2/cfdna/utilities/h5_utilities.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.1/pyproject.toml` & `cfdna-2.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cfdna"
-version = "2.1.1"
+version = "2.1.2"
 description = "Python package for fragment manipulation for cfDNA"
 authors = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 maintainers = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 repository = "https://github.com/kylessmith/cfdna"
 documentation = "https://www.biosciencestack.com/static/cfdna/docs/index.html"
 keywords = ["cython", "interval", "cfdna", "c"]
 readme = 'README.md'
@@ -39,15 +39,15 @@
 bokeh = "^3.1.0"
 scipy = "^1.9.1"
 statsmodels = "^0.13.5"
 seaborn = "^0.12.2"
 projectframe = "^1.0.0"
 hmmCNV = "^1.0.1"
 scikit-learn = "^1.2.2"
-ngsfragments = "^2.1.8"
+ngsfragments = "^2.2.0"
 genome_info = "^1.0.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0",
@@ -55,15 +55,15 @@
             "numpy>=1.23.5",
             "pandas>=2.0.0",
             "setuptools>=65.5.0",
             "ailist>=2.1.3",
             "pysam>=0.21.0",
             "genome_info>=1.0.4",
             "intervalframe>=1.1.5",
-            "ngsfragments>=2.1.8"]
+            "ngsfragments>=2.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.build]
 generate-setup-file = false
 #script = "build.py"
 
 [tool.cibuildwheel]
```

### Comparing `cfdna-2.1.1/PKG-INFO` & `cfdna-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfdna
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python package for fragment manipulation for cfDNA
 Home-page: https://github.com/kylessmith/cfdna
 License: GPL-2.0-or-later
 Keywords: cython,interval,cfdna,c
 Author: Kyle S. Smith
 Author-email: kyle.smith@stjude.org
 Maintainer: Kyle S. Smith
@@ -32,15 +32,15 @@
 Requires-Dist: bokeh (>=3.1.0,<4.0.0)
 Requires-Dist: cython (>=3.0.0,<4.0.0)
 Requires-Dist: genome_info (>=1.0.4,<2.0.0)
 Requires-Dist: hmmCNV (>=1.0.1,<2.0.0)
 Requires-Dist: intervalframe (>=1.1.5,<2.0.0)
 Requires-Dist: linear_segment (>=1.1.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: ngsfragments (>=2.1.8,<3.0.0)
+Requires-Dist: ngsfragments (>=2.2.0,<3.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: projectframe (>=1.0.0,<2.0.0)
 Requires-Dist: pysam (>=0.21.0,<0.22.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.9.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
```


# Comparing `tmp/libtsm-1.1.0.tar.gz` & `tmp/libtsm-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libtsm-1.1.0.tar", last modified: Tue Aug  3 12:54:07 2021, max compression
+gzip compressed data, was "libtsm-1.1.1.tar", last modified: Thu May 23 11:57:27 2024, max compression
```

## Comparing `libtsm-1.1.0.tar` & `libtsm-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 rosenzweig   (503) staff       (20)        0 2021-08-03 12:54:07.326720 libtsm-1.1.0/
--rw-r--r--   0 rosenzweig   (503) staff       (20)     1514 2021-07-15 08:19:33.000000 libtsm-1.1.0/LICENSE
--rw-r--r--   0 rosenzweig   (503) staff       (20)     3931 2021-08-03 12:54:07.326152 libtsm-1.1.0/PKG-INFO
--rw-r--r--   0 rosenzweig   (503) staff       (20)     3024 2021-07-19 13:16:51.000000 libtsm-1.1.0/README.md
-drwxr-xr-x   0 rosenzweig   (503) staff       (20)        0 2021-08-03 12:54:07.309487 libtsm-1.1.0/libtsm/
--rw-r--r--   0 rosenzweig   (503) staff       (20)       66 2021-07-15 08:19:33.000000 libtsm-1.1.0/libtsm/__init__.py
--rw-r--r--   0 rosenzweig   (503) staff       (20)     5733 2021-08-03 10:18:34.000000 libtsm-1.1.0/libtsm/pitchshift.py
--rw-r--r--   0 rosenzweig   (503) staff       (20)    18188 2021-07-15 08:19:33.000000 libtsm-1.1.0/libtsm/tsm.py
--rw-r--r--   0 rosenzweig   (503) staff       (20)    18746 2021-07-15 08:19:33.000000 libtsm-1.1.0/libtsm/utils.py
-drwxr-xr-x   0 rosenzweig   (503) staff       (20)        0 2021-08-03 12:54:07.318989 libtsm-1.1.0/libtsm.egg-info/
--rw-r--r--   0 rosenzweig   (503) staff       (20)     3931 2021-08-03 12:54:07.000000 libtsm-1.1.0/libtsm.egg-info/PKG-INFO
--rw-r--r--   0 rosenzweig   (503) staff       (20)      296 2021-08-03 12:54:07.000000 libtsm-1.1.0/libtsm.egg-info/SOURCES.txt
--rw-r--r--   0 rosenzweig   (503) staff       (20)        1 2021-08-03 12:54:07.000000 libtsm-1.1.0/libtsm.egg-info/dependency_links.txt
--rw-r--r--   0 rosenzweig   (503) staff       (20)      266 2021-08-03 12:54:07.000000 libtsm-1.1.0/libtsm.egg-info/requires.txt
--rw-r--r--   0 rosenzweig   (503) staff       (20)        7 2021-08-03 12:54:07.000000 libtsm-1.1.0/libtsm.egg-info/top_level.txt
--rw-r--r--   0 rosenzweig   (503) staff       (20)       38 2021-08-03 12:54:07.330383 libtsm-1.1.0/setup.cfg
--rw-r--r--   0 rosenzweig   (503) staff       (20)     1663 2021-08-03 11:35:02.000000 libtsm-1.1.0/setup.py
-drwxr-xr-x   0 rosenzweig   (503) staff       (20)        0 2021-08-03 12:54:07.322134 libtsm-1.1.0/test/
--rw-r--r--   0 rosenzweig   (503) staff       (20)     4321 2021-07-15 08:19:33.000000 libtsm-1.1.0/test/test_numerical.py
--rw-r--r--   0 rosenzweig   (503) staff       (20)     2828 2021-08-03 10:20:08.000000 libtsm-1.1.0/test/test_pitch_shifting.py
+drwxr-xr-x   0 typo       (501) staff       (20)        0 2024-05-23 11:57:27.025683 libtsm-1.1.1/
+-rw-r--r--   0 typo       (501) staff       (20)     1514 2024-05-03 13:02:08.000000 libtsm-1.1.1/LICENSE
+-rw-r--r--   0 typo       (501) staff       (20)     4368 2024-05-23 11:57:27.025460 libtsm-1.1.1/PKG-INFO
+-rw-r--r--   0 typo       (501) staff       (20)     3024 2024-05-03 13:02:08.000000 libtsm-1.1.1/README.md
+drwxr-xr-x   0 typo       (501) staff       (20)        0 2024-05-23 11:57:27.023311 libtsm-1.1.1/libtsm/
+-rw-r--r--   0 typo       (501) staff       (20)       66 2024-05-03 13:02:08.000000 libtsm-1.1.1/libtsm/__init__.py
+-rw-r--r--   0 typo       (501) staff       (20)     5628 2024-05-07 14:41:29.000000 libtsm-1.1.1/libtsm/pitchshift.py
+-rw-r--r--   0 typo       (501) staff       (20)    20000 2024-05-07 14:41:29.000000 libtsm-1.1.1/libtsm/tsm.py
+-rw-r--r--   0 typo       (501) staff       (20)    19863 2024-05-22 14:47:14.000000 libtsm-1.1.1/libtsm/utils.py
+drwxr-xr-x   0 typo       (501) staff       (20)        0 2024-05-23 11:57:27.024852 libtsm-1.1.1/libtsm.egg-info/
+-rw-r--r--   0 typo       (501) staff       (20)     4368 2024-05-23 11:57:26.000000 libtsm-1.1.1/libtsm.egg-info/PKG-INFO
+-rw-r--r--   0 typo       (501) staff       (20)      296 2024-05-23 11:57:27.000000 libtsm-1.1.1/libtsm.egg-info/SOURCES.txt
+-rw-r--r--   0 typo       (501) staff       (20)        1 2024-05-23 11:57:26.000000 libtsm-1.1.1/libtsm.egg-info/dependency_links.txt
+-rw-r--r--   0 typo       (501) staff       (20)      217 2024-05-23 11:57:26.000000 libtsm-1.1.1/libtsm.egg-info/requires.txt
+-rw-r--r--   0 typo       (501) staff       (20)        7 2024-05-23 11:57:26.000000 libtsm-1.1.1/libtsm.egg-info/top_level.txt
+-rw-r--r--   0 typo       (501) staff       (20)       38 2024-05-23 11:57:27.025729 libtsm-1.1.1/setup.cfg
+-rw-r--r--   0 typo       (501) staff       (20)     1600 2024-05-22 09:21:39.000000 libtsm-1.1.1/setup.py
+drwxr-xr-x   0 typo       (501) staff       (20)        0 2024-05-23 11:57:27.024588 libtsm-1.1.1/test/
+-rw-r--r--   0 typo       (501) staff       (20)     4321 2024-05-03 13:02:08.000000 libtsm-1.1.1/test/test_numerical.py
+-rw-r--r--   0 typo       (501) staff       (20)     2828 2024-05-03 13:02:08.000000 libtsm-1.1.1/test/test_pitch_shifting.py
```

### Comparing `libtsm-1.1.0/LICENSE` & `libtsm-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libtsm-1.1.0/PKG-INFO` & `libtsm-1.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 Metadata-Version: 2.1
 Name: libtsm
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python Package for Time-Scale Modification and Pitch-Shifting
 Home-page: https://www.audiolabs-erlangen.de/resources/MIR/2021-DAFX-AdaptivePitchShifting
+Download-URL: https://github.com/meinardmueller/libtsm/archive/refs/tags/v1.1.0.tar.gz
 Author: Sebastian Rosenzweig, Simon Schwär, Jonathan Driedger and Meinard Müller
 Author-email: sebastian.rosenzweig@audiolabs-erlangen.de
 License: MIT
-Download-URL: https://github.com/meinardmueller/libtsm/archive/refs/tags/v1.1.0.tar.gz
 Keywords: audio,music,tsm,pitch-shifting
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ipython>=7.8.0
+Requires-Dist: librosa>=0.8.0
+Requires-Dist: matplotlib>=3.1.0
+Requires-Dist: numba>=0.51.0
+Requires-Dist: numpy>=1.17.0
+Requires-Dist: pysoundfile>=0.9.0
+Requires-Dist: scipy>=1.3.0
 Provides-Extra: dev
+Requires-Dist: jupyter==1.0.*; extra == "dev"
+Requires-Dist: nbstripout==0.4.*; extra == "dev"
 Provides-Extra: tests
+Requires-Dist: pytest==6.2.*; extra == "tests"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: sphinx==4.0.*; extra == "docs"
+Requires-Dist: sphinx-rtd-theme==0.5.*; extra == "docs"
 
 # libtsm
 
 A Python toolbox for Time-Scale Modification (TSM) and Pitch-Shifting.
 
 Details and example application:
 
@@ -84,9 +95,7 @@
 pytest
 ```
 
 ## Acknowledgements
 
 This project is supported by the German Research Foundation (DFG MU 2686/12-1, MU 2686/13-1).
 The International Audio Laboratories Erlangen are a joint institution of the Friedrich-Alexander Universität Erlangen-Nürnberg (FAU) and Fraunhofer Institute for Integrated Circuits IIS. We thank Edgar Suarez, El Mehdi Lemnaouar and Miguel Gonzales for implementation support.
-
-
```

### Comparing `libtsm-1.1.0/README.md` & `libtsm-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `libtsm-1.1.0/libtsm/pitchshift.py` & `libtsm-1.1.1/libtsm/pitchshift.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,28 +126,28 @@
         # (Non-linear) Resampling
         fi = sc.interpolate.interp1d(tau[:, 0], tau[:, 1], kind='linear', fill_value="extrapolate")
         time_input = fi(t_x)
         fi = sc.interpolate.interp1d(time_input, x[:, 0], kind='cubic', fill_value="extrapolate")
         t_res = np.arange(0, tau[-1, 1] + 1 / Fs, 1 / Fs)
         y_ps = fi(t_res)
 
-        tau_inv = np.hstack((time_input.reshape(-1, 1), t_x.reshape(-1, 1)))
-        anchor_points = np.ceil(tau_inv * Fs).astype(int)
-        anchor_points = np.flip(anchor_points, axis=0)
-        anchor_points = anchor_points[np.unique(anchor_points[:, 0],
-                                                return_index=True)[1], :]  # only keep unique indices
+        # use inverse tau points as anchor points for TSM
+        anchor_points = np.ceil(tau * Fs).astype(int)
+        anchor_points = np.flip(anchor_points, axis=1)
+        # only keep unique indices
+        anchor_points = anchor_points[np.unique(anchor_points[:, 1], return_index=True)[1], :]
 
         # Time-Scale Modification
         y_ps = hps_tsm(y_ps, anchor_points, Fs=Fs, **kwargs)
 
     elif order == "tsm-res":
         # compute anchor points
         anchor_points = np.ceil(tau * Fs).astype(int)
-        anchor_points = anchor_points[np.unique(anchor_points[:, 1],
-                                                return_index=True)[1], :]  # only keep unique indices
+        # only keep unique indices
+        anchor_points = anchor_points[np.unique(anchor_points[:, 1], return_index=True)[1], :]
 
         # Time-Scale Modification
         y_tsm = hps_tsm(x, anchor_points, Fs=Fs, **kwargs)
 
         # (Non-linear) resampling
         time_output = np.linspace(0, (y_tsm.shape[0] - 1) / Fs, y_tsm.shape[0])
         fi = sc.interpolate.interp1d(tau[:, 1], tau[:, 0], kind='linear', fill_value="extrapolate")
```

### Comparing `libtsm-1.1.0/libtsm/tsm.py` & `libtsm-1.1.1/libtsm/tsm.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,25 +8,32 @@
 import numpy as np
 import scipy.interpolate
 from .utils import win, stft, istft, cross_corr, hps, find_peaks
 
 
 def pv_tsm(x, alpha, syn_hop=512, win_length=2048, win_beta=1, Fs=22050, zero_pad=0, restore_energy=False,
            fft_shift=False, phase_locking=False) -> np.ndarray:
-    """
-    Phase Vocoder Time scale modification algorithm, that rescales the time-axis of the input signal x
-    according to the time-stretch function s without altering the pitch of x.
+    """Time scale modification based on a phase vocoder
+
+    Rescales the time-axis of the input signal x according to the time-stretch function alpha
+    without altering the pitch of x.
 
     Parameters
     ----------
-    x : np.ndarray [shape=(N, )], real - valued
-        Signal to be transformed
+    x : np.ndarray [shape=(N, C)], real-valued
+        Signal to be transformed, second dimension is an optional channel dimension
 
     alpha : float or np.ndarray [shape=(S, 2)]
-        Time stretch function, given by a constant (float) or a set of S anchor points (int)
+        Time stretch function, given by a constant (float) or a set of S anchor points (int).
+        A valid anchor point sequence
+            (1) contains only non-negative values,
+            (2) both sequences along the first axis are strictly increasing,
+            (3) starts with position (m, 0), where m is an intereger >= 0.
+        These conditions will be checked and an error is thrown if they are not met.
+        See `libtsm.ensure_validity` for one way to ensure that condition (2) is fulfilled.
 
     syn_hop : int
         hop size of the synthesis window
 
     win_length : int
         length of analysis and synthesis window for STFT
 
@@ -76,14 +83,19 @@
     # in the output
 
     fi = scipy.interpolate.interp1d(anchor_points[:, 1], anchor_points[:, 0], kind='linear', fill_value='extrapolate')
     ana_win_pos = fi(syn_win_pos)
     ana_win_pos = np.round(ana_win_pos).astype(int)  # positions of the analysis windows in the input
     ana_hop = np.append([0], ana_win_pos[1:] - ana_win_pos[:-1])  # analysis hop sizes
 
+    # check conditions
+    assert anchor_points[0,1] == 0, "First sample for target sequence must be zero."
+    assert anchor_points[0,0] >= 0, "All anchor points must be non-negative."
+    assert np.all(ana_hop[1:] > 0), "The anchor point sequences must be stricly increasing for both source and target."
+
     # Phase Vocoder
     y = np.zeros((output_length, num_of_chan))  # initialize output
 
     for c in range(num_of_chan):  # loop over channels
 
         x_c = x[:, c]
 
@@ -114,30 +126,27 @@
 
             # We now compute a phasor that rotates the phase angles of the current input frame by angles theta such
             # that no phase discontinuities occur when re-synthesizing the resulting spectrogram with the synthesis
             # hopsize
             if not phase_locking:  # standard phase vocoder: the phase continuity of every bin is preserved separately
                 theta = ph_syn + ipa_hop - ph_curr  # phases of the last output frame Instantaneous phase advance
                 # Phases of the current input frame
-                phasor = np.exp(1j * theta)
 
             else:  # Phase vocoder with identity phase locking: the phase relationships from the input frame are
                 # partially preserved by 'locking' the phases of bins in the region of influence of a peak in the
                 # sprectrum to the phase of the peak's bin
                 p, irs, ire = find_peaks(X[:, i])  # Get the peaks in the spectrum together with their regions of
                 # influence
                 theta = np.zeros(Y[:, i].shape)
 
                 for n in range(0, len(p)):
                     theta[irs[n]:ire[n]] = ph_syn[p[n]] + ipa_hop[p[n]] - ph_curr[p[n]]  # Phases of the last
                     # output frame, Instantaneous phase advance, Phases of the current input frame
 
-                phasor = np.exp(1j * theta)
-
-            Y[:, i] = phasor * X[:, i]
+            Y[:, i] = np.exp(1j * theta) * X[:, i]
 
         # ISTFT
         y_c = istft(Y, syn_hop=syn_hop, win_length=win_length, win_beta=win_beta, zero_pad=zero_pad, num_of_iter=1,
                     orig_sig_len=output_length, restore_energy=restore_energy, fft_shift=fft_shift)
 
         y[:, c] = y_c[:, 0]
 
@@ -150,16 +159,22 @@
     according to the time-stretch function s without altering the pitch of x.
 
     Parameters
     ----------
     x : np.ndarray [shape=(N,num_of_chan)], real - valued
         Signal to be transformed
 
-    alpha : float or np.ndarray [shape=(S,2)]
-        Time stretch function, given by a constant (float) or a set of S anchor points (int)
+    alpha : float or np.ndarray [shape=(S, 2)]
+        Time stretch function, given by a constant (float) or a set of S anchor points (int).
+        A valid anchor point sequence
+            (1) contains only non-negative values,
+            (2) both sequences along the first axis are strictly increasing,
+            (3) starts with position (m, 0), where m is an intereger >= 0.
+        These conditions will be checked and an error is thrown if they are not met.
+        See `libtsm.ensure_validity` for one way to ensure that condition (2) is fulfilled.
 
     syn_hop : int
         hop size of the synthesis window
 
     win_length : int
         length of the analysis and synthesis window
 
@@ -194,20 +209,24 @@
     else:
         anchor_points = alpha.astype(int)
 
     output_length = anchor_points[-1, 1] + 1
     syn_win_pos = np.arange(0, output_length + win_len_half, syn_hop)  # positions of the synthesis winLenHalf
     # windows in the output
 
-    fi = scipy.interpolate.interp1d(anchor_points[:, 1], anchor_points[:, 0], kind='linear',
-                                 fill_value='extrapolate')
+    fi = scipy.interpolate.interp1d(anchor_points[:, 1], anchor_points[:, 0], kind='linear', fill_value='extrapolate')
     ana_win_pos = fi(syn_win_pos)
     ana_win_pos = np.round(ana_win_pos).astype(int)  # positions of the analysis windows in the input
     ana_hop = np.append([0], ana_win_pos[1:] - ana_win_pos[:-1])  # analysis hop sizes
 
+    # check conditions
+    assert anchor_points[0,1] == 0, "First sample for target sequence must be zero."
+    assert anchor_points[0,0] >= 0, "All anchor points must be non-negative."
+    assert np.all(ana_hop[1:] > 0), "The anchor point sequences must be stricly increasing for both source and target."
+
     # WSOLA
     y = np.zeros((output_length, num_of_chan))  # initialize output
     min_fac = np.min(syn_hop / ana_hop[1:])  # the minimal local stretching factor
     # to avoid that we access x outside its range, we need to zero pad it appropriately
     x = np.pad(x, [(win_len_half + tol, int(np.ceil(1 / min_fac)) * win_len + tol), (0, 0)])
     ana_win_pos += tol  # compensate for the extra 'tol' padded zeros at the beginning of x
 
@@ -265,16 +284,22 @@
     separately.
 
     Parameters
     ----------
     x : np.ndarray [shape=(N, )], real - valued
         Signal to be transformed
 
-    alpha : float or np.ndarray [shape=(S,2)]
-        Time stretch function, given by a constant (float) or a set of S anchor points (int)
+    alpha : float or np.ndarray [shape=(S, 2)]
+        Time stretch function, given by a constant (float) or a set of S anchor points (int).
+        A valid anchor point sequence
+            (1) contains only non-negative values,
+            (2) both sequences along the first axis are strictly increasing,
+            (3) starts with position (m, 0), where m is an intereger >= 0.
+        These conditions will be checked and an error is thrown if they are not met.
+        See `libtsm.ensure_validity` for one way to ensure that condition (2) is fulfilled.
 
     Fs : int
         Sampling rate
 
     hps_ana_hop : int
         hop size for HPS
```

### Comparing `libtsm-1.1.0/libtsm/utils.py` & `libtsm-1.1.1/libtsm/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,42 @@
 
 import numpy as np
 import scipy as sc
 import scipy.signal
 from typing import Tuple
 
 
+def ensure_validity(alpha, syn_hop=128):
+    """Remove points from a sequence of anchor points to ensure a valid TSM input
+
+    This function removes any anchor points that lead to a non-monotonous increase of the analysis window and
+    returns a new sequence of anchor points that is a valid TSM input.
+
+    Note that, depending on the data, this is not a sensible way to ensure a valid TSM input. Often, it may be
+    advisable to use coarser and semantically meaningful positions for the anchor points.
+
+    Parameters
+    ----------
+    alpha : float or np.ndarray [shape=(S, 2)]
+        Time stretch function, given by a set of S anchor points (int).
+
+    syn_hop : int
+        (smallest) hop size of the synthesis window (default: 128)
+    """
+    d_ana = np.diff(alpha[:,0])
+    d_syn = np.diff(alpha[:,1])
+    not_too_steep = np.pad(np.round(d_syn / d_ana) <= syn_hop, (1,0), constant_values=True)
+
+    # call recursively to remove consecutive points that are too steep
+    if not np.all(not_too_steep):
+        return ensure_validity(alpha[not_too_steep,:], syn_hop)
+    else:
+        return alpha
+
+
 def win(win_len, beta) -> np.ndarray:
     """
     Generates a sin^beta window.
 
     Parameters
     ----------
     win_len : int
@@ -89,15 +117,15 @@
     x_perc = np.zeros(x.shape)  # Initialize output
 
     for c in range(num_of_chan):  # loop over channels
         x_c = x[:, c]
 
         # stft
         spec, f, t = stft(x_c, ana_hop=ana_hop, win_length=win_length, win_beta=win_beta, Fs=Fs, num_of_frames=-1,
-                          fft_shift=False, zero_pad=0)
+                          fft_shift=False, zero_pad=zero_pad)
         mag_spec = np.abs(spec)
 
         # harmonic-percussive separation
         mag_spec_perc = median_filter(mag_spec, fil_len_perc, 0)
         mag_spec_harm = median_filter(mag_spec, fil_len_harm, 1)
 
         if masking_mode == 'binary':
```

### Comparing `libtsm-1.1.0/libtsm.egg-info/PKG-INFO` & `libtsm-1.1.1/libtsm.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 Metadata-Version: 2.1
 Name: libtsm
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python Package for Time-Scale Modification and Pitch-Shifting
 Home-page: https://www.audiolabs-erlangen.de/resources/MIR/2021-DAFX-AdaptivePitchShifting
+Download-URL: https://github.com/meinardmueller/libtsm/archive/refs/tags/v1.1.0.tar.gz
 Author: Sebastian Rosenzweig, Simon Schwär, Jonathan Driedger and Meinard Müller
 Author-email: sebastian.rosenzweig@audiolabs-erlangen.de
 License: MIT
-Download-URL: https://github.com/meinardmueller/libtsm/archive/refs/tags/v1.1.0.tar.gz
 Keywords: audio,music,tsm,pitch-shifting
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ipython>=7.8.0
+Requires-Dist: librosa>=0.8.0
+Requires-Dist: matplotlib>=3.1.0
+Requires-Dist: numba>=0.51.0
+Requires-Dist: numpy>=1.17.0
+Requires-Dist: pysoundfile>=0.9.0
+Requires-Dist: scipy>=1.3.0
 Provides-Extra: dev
+Requires-Dist: jupyter==1.0.*; extra == "dev"
+Requires-Dist: nbstripout==0.4.*; extra == "dev"
 Provides-Extra: tests
+Requires-Dist: pytest==6.2.*; extra == "tests"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: sphinx==4.0.*; extra == "docs"
+Requires-Dist: sphinx-rtd-theme==0.5.*; extra == "docs"
 
 # libtsm
 
 A Python toolbox for Time-Scale Modification (TSM) and Pitch-Shifting.
 
 Details and example application:
 
@@ -84,9 +95,7 @@
 pytest
 ```
 
 ## Acknowledgements
 
 This project is supported by the German Research Foundation (DFG MU 2686/12-1, MU 2686/13-1).
 The International Audio Laboratories Erlangen are a joint institution of the Friedrich-Alexander Universität Erlangen-Nürnberg (FAU) and Fraunhofer Institute for Integrated Circuits IIS. We thank Edgar Suarez, El Mehdi Lemnaouar and Miguel Gonzales for implementation support.
-
-
```

### Comparing `libtsm-1.1.0/setup.py` & `libtsm-1.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r') as fdesc:
     long_description = fdesc.read()
 
 setup(
     name='libtsm',
-    version='1.1.0',
+    version='1.1.1',
     description='Python Package for Time-Scale Modification and Pitch-Shifting',
     author='Sebastian Rosenzweig, Simon Schwär, Jonathan Driedger and Meinard Müller',
     author_email='sebastian.rosenzweig@audiolabs-erlangen.de',
     url='https://www.audiolabs-erlangen.de/resources/MIR/2021-DAFX-AdaptivePitchShifting',
     download_url='https://github.com/meinardmueller/libtsm/archive/refs/tags/v1.1.0.tar.gz',
     packages=find_packages(),
     long_description=long_description,
@@ -20,21 +20,21 @@
         "Programming Language :: Python",
         "Intended Audience :: Developers",
         "Topic :: Multimedia :: Sound/Audio :: Analysis",
         "Programming Language :: Python :: 3",
     ],
     keywords=['audio', 'music', 'tsm', 'pitch-shifting'],
     license='MIT',
-    install_requires=['ipython >= 7.8.0, < 8.0.0',
-                      'librosa >= 0.8.0, < 1.0.0',
-                      'matplotlib >= 3.1.0, < 4.0.0',
-                      'numba >= 0.51.0, < 1.0.0',
-                      'numpy >= 1.17.0, < 2.0.0',
-                      'pysoundfile >= 0.9.0, < 1.0.0',
-                      'scipy >= 1.3.0, < 2.0.0'],
+    install_requires=['ipython >= 7.8.0',
+                      'librosa >= 0.8.0',
+                      'matplotlib >= 3.1.0',
+                      'numba >= 0.51.0',
+                      'numpy >= 1.17.0',
+                      'pysoundfile >= 0.9.0',
+                      'scipy >= 1.3.0'],
     python_requires='>=3.6',
     extras_require={
         'dev': ['jupyter == 1.0.*',
                 'nbstripout == 0.4.*'],
         'tests': ['pytest == 6.2.*'],
         'docs': ['sphinx == 4.0.*',
                  'sphinx-rtd-theme == 0.5.*'],
```

### Comparing `libtsm-1.1.0/test/test_numerical.py` & `libtsm-1.1.1/test/test_numerical.py`

 * *Files identical despite different names*

### Comparing `libtsm-1.1.0/test/test_pitch_shifting.py` & `libtsm-1.1.1/test/test_pitch_shifting.py`

 * *Files identical despite different names*


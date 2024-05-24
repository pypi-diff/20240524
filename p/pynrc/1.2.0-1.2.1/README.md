# Comparing `tmp/pynrc-1.2.0.tar.gz` & `tmp/pynrc-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynrc-1.2.0.tar", last modified: Tue May 14 05:07:03 2024, max compression
+gzip compressed data, was "pynrc-1.2.1.tar", last modified: Fri May 24 18:46:08 2024, max compression
```

## Comparing `pynrc-1.2.0.tar` & `pynrc-1.2.1.tar`

### file list

```diff
@@ -1,468 +1,468 @@
-drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-14 05:07:03.762681 pynrc-1.2.0/
--rw-r--r--   0 jarron     (501) staff       (20)     5862 2024-05-14 04:44:59.000000 pynrc-1.2.0/CONTRIBUTING.rst
--rw-r--r--   0 jarron     (501) staff       (20)     4597 2024-05-14 05:01:21.000000 pynrc-1.2.0/HISTORY.rst
--rw-r--r--   0 jarron     (501) staff       (20)     1076 2023-06-14 14:36:11.000000 pynrc-1.2.0/LICENSE
--rw-r--r--   0 jarron     (501) staff       (20)      337 2023-06-14 14:36:11.000000 pynrc-1.2.0/MANIFEST.in
--rw-r--r--   0 jarron     (501) staff       (20)     9200 2024-05-14 05:07:03.762754 pynrc-1.2.0/PKG-INFO
--rw-r--r--   0 jarron     (501) staff       (20)     3954 2023-06-14 14:41:38.000000 pynrc-1.2.0/README.rst
-drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-14 05:07:03.706869 pynrc-1.2.0/docs/
--rw-r--r--   0 jarron     (501) staff       (20)      602 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/Makefile
-drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-14 05:07:03.703586 pynrc-1.2.0/docs/_build/
-drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-14 05:07:03.703506 pynrc-1.2.0/docs/_build/doctrees/
-drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-14 05:07:03.709365 pynrc-1.2.0/docs/_build/doctrees/nbsphinx/
--rw-r--r--   0 jarron     (501) staff       (20)    49182 2024-05-14 05:05:09.000000 pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Basic_Usage_14_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    19831 2024-05-14 05:05:09.000000 pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Basic_Usage_16_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    19084 2024-05-14 05:05:09.000000 pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Basic_Usage_27_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    24012 2024-05-14 05:05:10.000000 pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_20_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    59331 2024-05-14 05:05:10.000000 pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_26_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    59832 2024-05-14 05:05:10.000000 pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_29_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    61999 2024-05-14 05:05:10.000000 pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_32_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    12453 2024-05-14 05:05:10.000000 pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_40_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    32158 2024-05-14 05:05:10.000000 pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_8_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    29633 2024-05-14 05:05:11.000000 pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Wedges_10_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    25092 2024-05-14 05:05:11.000000 pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Wedges_20_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    78390 2024-05-14 05:05:11.000000 pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Wedges_24_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    47901 2024-05-14 05:05:11.000000 pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Wedges_26_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    42386 2024-05-14 05:05:11.000000 pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Wedges_9_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    40325 2024-05-14 05:05:11.000000 pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_HR8799_DMS_Level1b_11_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    50157 2024-05-14 05:05:12.000000 pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Ramp_Optimization_Examples_30_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    13328 2024-05-14 05:05:12.000000 pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Ramp_Optimization_Examples_32_1.png
--rw-r--r--   0 jarron     (501) staff       (20)    48589 2024-05-14 05:05:12.000000 pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Ramp_Optimization_Examples_35_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    21707 2024-05-14 05:05:12.000000 pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Ramp_Optimization_Examples_43_1.png
-drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-14 05:07:03.703703 pynrc-1.2.0/docs/_build/html/
-drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-14 05:07:03.712087 pynrc-1.2.0/docs/_build/html/_images/
--rw-r--r--   0 jarron     (501) staff       (20)    49182 2024-05-14 05:05:09.000000 pynrc-1.2.0/docs/_build/html/_images/tutorials_Basic_Usage_14_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    19831 2024-05-14 05:05:09.000000 pynrc-1.2.0/docs/_build/html/_images/tutorials_Basic_Usage_16_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    19084 2024-05-14 05:05:09.000000 pynrc-1.2.0/docs/_build/html/_images/tutorials_Basic_Usage_27_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    24012 2024-05-14 05:05:10.000000 pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Basics_20_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    59331 2024-05-14 05:05:10.000000 pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Basics_26_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    59832 2024-05-14 05:05:10.000000 pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Basics_29_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    61999 2024-05-14 05:05:10.000000 pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Basics_32_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    12453 2024-05-14 05:05:10.000000 pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Basics_40_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    32158 2024-05-14 05:05:10.000000 pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Basics_8_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    29633 2024-05-14 05:05:11.000000 pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Wedges_10_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    25092 2024-05-14 05:05:11.000000 pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Wedges_20_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    78390 2024-05-14 05:05:11.000000 pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Wedges_24_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    47901 2024-05-14 05:05:11.000000 pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Wedges_26_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    42386 2024-05-14 05:05:11.000000 pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Wedges_9_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    40325 2024-05-14 05:05:11.000000 pynrc-1.2.0/docs/_build/html/_images/tutorials_HR8799_DMS_Level1b_11_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    50157 2024-05-14 05:05:12.000000 pynrc-1.2.0/docs/_build/html/_images/tutorials_Ramp_Optimization_Examples_30_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    13328 2024-05-14 05:05:12.000000 pynrc-1.2.0/docs/_build/html/_images/tutorials_Ramp_Optimization_Examples_32_1.png
--rw-r--r--   0 jarron     (501) staff       (20)    48589 2024-05-14 05:05:12.000000 pynrc-1.2.0/docs/_build/html/_images/tutorials_Ramp_Optimization_Examples_35_0.png
--rw-r--r--   0 jarron     (501) staff       (20)    21707 2024-05-14 05:05:12.000000 pynrc-1.2.0/docs/_build/html/_images/tutorials_Ramp_Optimization_Examples_43_1.png
-drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-14 05:07:03.712497 pynrc-1.2.0/docs/_build/html/_static/
--rw-r--r--   0 jarron     (501) staff       (20)      286 2022-07-14 07:38:21.000000 pynrc-1.2.0/docs/_build/html/_static/file.png
--rw-r--r--   0 jarron     (501) staff       (20)       90 2022-07-14 07:38:21.000000 pynrc-1.2.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 jarron     (501) staff       (20)       90 2022-07-14 07:38:21.000000 pynrc-1.2.0/docs/_build/html/_static/plus.png
-drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-14 05:07:03.712825 pynrc-1.2.0/docs/_templates/
--rw-r--r--   0 jarron     (501) staff       (20)      106 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/_templates/base.rst
--rw-r--r--   0 jarron     (501) staff       (20)      611 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/_templates/custom-class-template.rst
--rw-r--r--   0 jarron     (501) staff       (20)     1219 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/_templates/custom-module-template.rst
-drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-14 05:07:03.713509 pynrc-1.2.0/docs/api/
-drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-14 05:07:03.756214 pynrc-1.2.0/docs/api/_autosummary/
--rw-r--r--   0 jarron     (501) staff       (20)     1492 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.DetectorOps.rst
--rw-r--r--   0 jarron     (501) staff       (20)     2855 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.NIRCam.rst
--rw-r--r--   0 jarron     (501) staff       (20)      104 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.detops.config2.rst
--rw-r--r--   0 jarron     (501) staff       (20)      124 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.detops.create_detops.rst
--rw-r--r--   0 jarron     (501) staff       (20)      115 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.detops.nrc_header.rst
--rw-r--r--   0 jarron     (501) staff       (20)      377 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.logging_utils.FilterLevelRange.rst
--rw-r--r--   0 jarron     (501) staff       (20)      150 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.logging_utils.restart_logging.rst
--rw-r--r--   0 jarron     (501) staff       (20)      383 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.logging_utils.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.logging_utils.setup_logging.rst
--rw-r--r--   0 jarron     (501) staff       (20)      136 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.maths.coords.Tel2Sci_info.rst
--rw-r--r--   0 jarron     (501) staff       (20)      132 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.maths.coords.det_to_sci.rst
--rw-r--r--   0 jarron     (501) staff       (20)      245 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.maths.coords.rst
--rw-r--r--   0 jarron     (501) staff       (20)      132 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.maths.coords.sci_to_det.rst
--rw-r--r--   0 jarron     (501) staff       (20)      153 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.maths.coords.siafap_sci_coords.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.maths.image_manip.align_LSQ.rst
--rw-r--r--   0 jarron     (501) staff       (20)      156 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.maths.image_manip.align_leastsq.rst
--rw-r--r--   0 jarron     (501) staff       (20)      147 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.maths.image_manip.crop_image.rst
--rw-r--r--   0 jarron     (501) staff       (20)      165 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.maths.image_manip.crop_observation.rst
--rw-r--r--   0 jarron     (501) staff       (20)      172 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.maths.image_manip.fix_nans_with_med.rst
--rw-r--r--   0 jarron     (501) staff       (20)      171 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.maths.image_manip.optimal_difference.rst
--rw-r--r--   0 jarron     (501) staff       (20)      406 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.maths.image_manip.rst
--rw-r--r--   0 jarron     (501) staff       (20)      164 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.maths.image_manip.scale_ref_image.rst
--rw-r--r--   0 jarron     (501) staff       (20)      159 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.maths.image_manip.shift_subtract.rst
--rw-r--r--   0 jarron     (501) staff       (20)      153 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.maths.image_manip.subtract_psf.rst
--rw-r--r--   0 jarron     (501) staff       (20)      629 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.multiaccum.rst
--rw-r--r--   0 jarron     (501) staff       (20)      132 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.average_slopes.rst
--rw-r--r--   0 jarron     (501) staff       (20)      134 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.disk_rim_model.rst
--rw-r--r--   0 jarron     (501) staff       (20)      123 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.do_contrast.rst
--rw-r--r--   0 jarron     (501) staff       (20)      125 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.do_gen_hdus.rst
--rw-r--r--   0 jarron     (501) staff       (20)      108 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.do_opt.rst
--rw-r--r--   0 jarron     (501) staff       (20)      143 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.do_plot_contrasts.rst
--rw-r--r--   0 jarron     (501) staff       (20)      146 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.do_plot_contrasts2.rst
--rw-r--r--   0 jarron     (501) staff       (20)      131 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.do_sat_levels.rst
--rw-r--r--   0 jarron     (501) staff       (20)      114 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.make_key.rst
--rw-r--r--   0 jarron     (501) staff       (20)      120 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.model_info.rst
--rw-r--r--   0 jarron     (501) staff       (20)      126 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.obs_optimize.rst
--rw-r--r--   0 jarron     (501) staff       (20)      111 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.obs_wfe.rst
--rw-r--r--   0 jarron     (501) staff       (20)      123 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.planet_mags.rst
--rw-r--r--   0 jarron     (501) staff       (20)      132 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.plot_contrasts.rst
--rw-r--r--   0 jarron     (501) staff       (20)      149 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.plot_contrasts_mjup.rst
--rw-r--r--   0 jarron     (501) staff       (20)      126 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.plot_hdulist.rst
--rw-r--r--   0 jarron     (501) staff       (20)      123 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.plot_images.rst
--rw-r--r--   0 jarron     (501) staff       (20)      140 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.plot_images_swlw.rst
--rw-r--r--   0 jarron     (501) staff       (20)      149 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.plot_planet_patches.rst
--rw-r--r--   0 jarron     (501) staff       (20)      129 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.plot_spectrum.rst
--rw-r--r--   0 jarron     (501) staff       (20)      608 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.rst
--rw-r--r--   0 jarron     (501) staff       (20)      129 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.update_yscale.rst
--rw-r--r--   0 jarron     (501) staff       (20)     3080 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_hci.rst
--rw-r--r--   0 jarron     (501) staff       (20)      154 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.bias_dark_high_temp.rst
--rw-r--r--   0 jarron     (501) staff       (20)      129 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.bin_spectrum.rst
--rw-r--r--   0 jarron     (501) staff       (20)      123 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.build_mask.rst
--rw-r--r--   0 jarron     (501) staff       (20)      143 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.build_mask_detid.rst
--rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.channel_select.rst
--rw-r--r--   0 jarron     (501) staff       (20)      134 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.coron_ap_locs.rst
--rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.coron_detector.rst
--rw-r--r--   0 jarron     (501) staff       (20)      126 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.coron_trans.rst
--rw-r--r--   0 jarron     (501) staff       (20)      134 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.dark_ramp_80K.rst
--rw-r--r--   0 jarron     (501) staff       (20)      152 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.do_charge_migration.rst
--rw-r--r--   0 jarron     (501) staff       (20)      111 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.do_fft.rst
--rw-r--r--   0 jarron     (501) staff       (20)      201 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.gen_unconvolved_point_source_image.rst
--rw-r--r--   0 jarron     (501) staff       (20)      126 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.get_detname.rst
--rw-r--r--   0 jarron     (501) staff       (20)      141 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.grism_background.rst
--rw-r--r--   0 jarron     (501) staff       (20)      155 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.grism_background_com.rst
--rw-r--r--   0 jarron     (501) staff       (20)      161 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.grism_background_image.rst
--rw-r--r--   0 jarron     (501) staff       (20)      143 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.make_grism_slope.rst
--rw-r--r--   0 jarron     (501) staff       (20)      149 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.nproc_use_convolve.rst
--rw-r--r--   0 jarron     (501) staff       (20)      123 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.offset_bar.rst
--rw-r--r--   0 jarron     (501) staff       (20)      132 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.pickoff_image.rst
--rw-r--r--   0 jarron     (501) staff       (20)      123 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.pickoff_xy.rst
--rw-r--r--   0 jarron     (501) staff       (20)      120 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.pix_noise.rst
--rw-r--r--   0 jarron     (501) staff       (20)      143 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.place_grism_spec.rst
--rw-r--r--   0 jarron     (501) staff       (20)      143 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.place_grismr_tso.rst
--rw-r--r--   0 jarron     (501) staff       (20)      662 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.rst
--rw-r--r--   0 jarron     (501) staff       (20)      146 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.segment_pupil_opd.rst
--rw-r--r--   0 jarron     (501) staff       (20)      131 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.var_ex_model.rst
--rw-r--r--   0 jarron     (501) staff       (20)      126 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.zodi_euclid.rst
--rw-r--r--   0 jarron     (501) staff       (20)      120 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.zodi_spec.rst
--rw-r--r--   0 jarron     (501) staff       (20)     3574 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.obs_hci.rst
--rw-r--r--   0 jarron     (501) staff       (20)      108 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.opds.rst
--rw-r--r--   0 jarron     (501) staff       (20)      145 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.apply_linearity.rst
--rw-r--r--   0 jarron     (501) staff       (20)      136 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.apply_nonlin.rst
--rw-r--r--   0 jarron     (501) staff       (20)      118 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.bp_fix.rst
--rw-r--r--   0 jarron     (501) staff       (20)      159 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.broken_pink_powspec.rst
--rw-r--r--   0 jarron     (501) staff       (20)      139 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.calc_cdsnoise.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.calc_eff_noise.rst
--rw-r--r--   0 jarron     (501) staff       (20)      124 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.calc_ktc.rst
--rw-r--r--   0 jarron     (501) staff       (20)      162 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.calc_linearity_coeff.rst
--rw-r--r--   0 jarron     (501) staff       (20)      153 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.calc_nonlin_coeff.rst
--rw-r--r--   0 jarron     (501) staff       (20)      130 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.chisqr_red.rst
--rw-r--r--   0 jarron     (501) staff       (20)      124 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.cube_fit.rst
--rw-r--r--   0 jarron     (501) staff       (20)      159 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.deconv_single_image.rst
--rw-r--r--   0 jarron     (501) staff       (20)      150 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.detname_to_scaid.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.find_group_sat.rst
--rw-r--r--   0 jarron     (501) staff       (20)      124 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.find_sat.rst
--rw-r--r--   0 jarron     (501) staff       (20)      150 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.fit_corr_powspec.rst
--rw-r--r--   0 jarron     (501) staff       (20)      149 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.fit_func_var_ex.rst
--rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.gen_cds_dict.rst
--rw-r--r--   0 jarron     (501) staff       (20)      156 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.gen_col_variations.rst
--rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.gen_ref_dict.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.gen_super_bias.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.gen_super_dark.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.gen_super_ramp.rst
--rw-r--r--   0 jarron     (501) staff       (20)      150 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.get_bias_offsets.rst
--rw-r--r--   0 jarron     (501) staff       (20)      141 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.get_fits_data.rst
--rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.get_flat_fields.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.get_freq_array.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.get_ipc_kernel.rst
--rw-r--r--   0 jarron     (501) staff       (20)      153 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.get_linear_coeffs.rst
--rw-r--r--   0 jarron     (501) staff       (20)      159 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.get_oddeven_offsets.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.get_power_spec.rst
--rw-r--r--   0 jarron     (501) staff       (20)      158 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.get_power_spec_all.rst
--rw-r--r--   0 jarron     (501) staff       (20)      159 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.get_ref_instability.rst
--rw-r--r--   0 jarron     (501) staff       (20)      142 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.ipc_deconvolve.rst
--rw-r--r--   0 jarron     (501) staff       (20)     2344 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.nircam_cal.rst
--rw-r--r--   0 jarron     (501) staff       (20)     2408 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.nircam_dark.rst
--rw-r--r--   0 jarron     (501) staff       (20)      165 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.pixel_linearity_gains.rst
--rw-r--r--   0 jarron     (501) staff       (20)      159 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.plot_dark_histogram.rst
--rw-r--r--   0 jarron     (501) staff       (20)      133 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.plot_kernel.rst
--rw-r--r--   0 jarron     (501) staff       (20)      141 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.pow_spec_ramp.rst
--rw-r--r--   0 jarron     (501) staff       (20)      155 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.pow_spec_ramp_pix.rst
--rw-r--r--   0 jarron     (501) staff       (20)      142 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.ppc_deconvolve.rst
--rw-r--r--   0 jarron     (501) staff       (20)      145 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.ramp_derivative.rst
--rw-r--r--   0 jarron     (501) staff       (20)      139 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.ramp_resample.rst
--rw-r--r--   0 jarron     (501) staff       (20)     1257 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.rst
--rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.time_to_sat.rst
--rw-r--r--   0 jarron     (501) staff       (20)      787 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.ref_pixels.NRC_refs.rst
--rw-r--r--   0 jarron     (501) staff       (20)      158 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.ref_pixels.calc_avg_amps.rst
--rw-r--r--   0 jarron     (501) staff       (20)      158 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.ref_pixels.calc_avg_cols.rst
--rw-r--r--   0 jarron     (501) staff       (20)      164 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.ref_pixels.calc_col_smooth.rst
--rw-r--r--   0 jarron     (501) staff       (20)      168 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.ref_pixels.channel_averaging.rst
--rw-r--r--   0 jarron     (501) staff       (20)      182 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.ref_pixels.channel_smooth_butter.rst
--rw-r--r--   0 jarron     (501) staff       (20)      173 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.ref_pixels.channel_smooth_fft.rst
--rw-r--r--   0 jarron     (501) staff       (20)      182 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.ref_pixels.channel_smooth_savgol.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.ref_pixels.chrem_med.rst
--rw-r--r--   0 jarron     (501) staff       (20)      150 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.ref_pixels.mask_helper.rst
--rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.ref_pixels.ref_filter.rst
--rw-r--r--   0 jarron     (501) staff       (20)      150 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.ref_pixels.reffix_amps.rst
--rw-r--r--   0 jarron     (501) staff       (20)      150 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.ref_pixels.reffix_hxrg.rst
--rw-r--r--   0 jarron     (501) staff       (20)      616 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.ref_pixels.rst
--rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.ref_pixels.smooth_fft.rst
--rw-r--r--   0 jarron     (501) staff       (20)      764 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.AptInput.rst
--rw-r--r--   0 jarron     (501) staff       (20)      570 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.DMS_input.rst
--rw-r--r--   0 jarron     (501) staff       (20)     1100 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.ReadAPTXML.rst
--rw-r--r--   0 jarron     (501) staff       (20)      152 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.build_dict_from_xml.rst
--rw-r--r--   0 jarron     (501) staff       (20)      141 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.create_det_class.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.create_obs_params.rst
--rw-r--r--   0 jarron     (501) staff       (20)      136 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.file_segmenting.rst
--rw-r--r--   0 jarron     (501) staff       (20)      149 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.gen_all_apt_visits.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.gen_jwst_pointing.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.gen_pointing_info.rst
--rw-r--r--   0 jarron     (501) staff       (20)      133 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.get_ditherinfo.rst
--rw-r--r--   0 jarron     (501) staff       (20)      129 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.get_exp_type.rst
--rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.get_filter_info.rst
--rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.get_orient_specreq.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.get_pointing_info.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.get_proposal_info.rst
--rw-r--r--   0 jarron     (501) staff       (20)      130 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.get_readmodes.rst
--rw-r--r--   0 jarron     (501) staff       (20)      132 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.get_roll_info.rst
--rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.get_siaf_detectors.rst
--rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.get_target_info.rst
--rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.get_tel_angles.rst
--rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.get_timing_info.rst
--rw-r--r--   0 jarron     (501) staff       (20)      132 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.pitch_vs_time.rst
--rw-r--r--   0 jarron     (501) staff       (20)      150 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.populate_obs_params.rst
--rw-r--r--   0 jarron     (501) staff       (20)      182 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.read_subarray_definition_file.rst
--rw-r--r--   0 jarron     (501) staff       (20)      924 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.rst
--rw-r--r--   0 jarron     (501) staff       (20)      153 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.update_eng_detectors.rst
--rw-r--r--   0 jarron     (501) staff       (20)      162 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.update_subarray_imaging.rst
--rw-r--r--   0 jarron     (501) staff       (20)      127 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.dms.DMS_filename.rst
--rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.dms.compute_local_roll.rst
--rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.dms.create_DMS_HDUList.rst
--rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.dms.create_group_entry.rst
--rw-r--r--   0 jarron     (501) staff       (20)      132 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.dms.dec_to_base36.rst
--rw-r--r--   0 jarron     (501) staff       (20)      150 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.dms.filename_visit_info.rst
--rw-r--r--   0 jarron     (501) staff       (20)      120 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.dms.jw_obs_id.rst
--rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.dms.level1b_data_model.rst
--rw-r--r--   0 jarron     (501) staff       (20)      153 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.dms.populate_group_table.rst
--rw-r--r--   0 jarron     (501) staff       (20)      482 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.dms.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.dms.save_level1b_fits.rst
--rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.dms.update_dms_headers.rst
--rw-r--r--   0 jarron     (501) staff       (20)      170 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.dms.update_headers_pynrc_info.rst
--rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.add_col_noise.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.add_cosmic_rays.rst
--rw-r--r--   0 jarron     (501) staff       (20)      118 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.add_ipc.rst
--rw-r--r--   0 jarron     (501) staff       (20)      118 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.add_ppc.rst
--rw-r--r--   0 jarron     (501) staff       (20)      124 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.add_xtalk.rst
--rw-r--r--   0 jarron     (501) staff       (20)      127 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.apply_flat.rst
--rw-r--r--   0 jarron     (501) staff       (20)      156 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.create_level1b_FITS.rst
--rw-r--r--   0 jarron     (501) staff       (20)      124 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.fft_noise.rst
--rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.gen_col_noise.rst
--rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.gen_dark_ramp.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.gen_ramp_biases.rst
--rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.gen_wfe_drift.rst
--rw-r--r--   0 jarron     (501) staff       (20)      167 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.make_gaia_source_table.rst
--rw-r--r--   0 jarron     (501) staff       (20)      150 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.make_ramp_poisson.rst
--rw-r--r--   0 jarron     (501) staff       (20)      173 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.make_simbad_source_table.rst
--rw-r--r--   0 jarron     (501) staff       (20)      127 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.pink_noise.rst
--rw-r--r--   0 jarron     (501) staff       (20)      728 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.rst
--rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.save_slope_image.rst
--rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.sim_dark_ramp.rst
--rw-r--r--   0 jarron     (501) staff       (20)      141 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.sim_image_ramp.rst
--rw-r--r--   0 jarron     (501) staff       (20)      141 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.sim_noise_data.rst
--rw-r--r--   0 jarron     (501) staff       (20)      165 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.simulate_detector_ramp.rst
--rw-r--r--   0 jarron     (501) staff       (20)      156 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.slope_to_fitswriter.rst
--rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.slope_to_level1b.rst
--rw-r--r--   0 jarron     (501) staff       (20)      153 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.sources_to_level1b.rst
--rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.sources_to_slope.rst
--rw-r--r--   0 jarron     (501) staff       (20)      130 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.xtalk_image.rst
--rw-r--r--   0 jarron     (501) staff       (20)      125 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.skyvec2ins.ad2lb.rst
--rw-r--r--   0 jarron     (501) staff       (20)      125 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.skyvec2ins.ei2lb.rst
--rw-r--r--   0 jarron     (501) staff       (20)      125 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.skyvec2ins.lb2ad.rst
--rw-r--r--   0 jarron     (501) staff       (20)      125 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.skyvec2ins.lb2ei.rst
--rw-r--r--   0 jarron     (501) staff       (20)      308 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.skyvec2ins.rst
--rw-r--r--   0 jarron     (501) staff       (20)      140 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.skyvec2ins.skyvec2ins.rst
--rw-r--r--   0 jarron     (501) staff       (20)      180 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.skyvec2ins.sun_ecliptic_longitude.rst
--rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.bp_2mass.rst
--rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.bp_gaia.rst
--rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.bp_igood.rst
--rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.bp_wise.rst
--rw-r--r--   0 jarron     (501) staff       (20)      150 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.filter_width.rst
--rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.miri_filter.rst
--rw-r--r--   0 jarron     (501) staff       (20)      155 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.nircam_com_nd.rst
--rw-r--r--   0 jarron     (501) staff       (20)      155 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.nircam_com_th.rst
--rw-r--r--   0 jarron     (501) staff       (20)      153 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.nircam_filter.rst
--rw-r--r--   0 jarron     (501) staff       (20)      164 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.nircam_grism_res.rst
--rw-r--r--   0 jarron     (501) staff       (20)      172 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.nircam_grism_si_ar.rst
--rw-r--r--   0 jarron     (501) staff       (20)      161 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.nircam_grism_th.rst
--rw-r--r--   0 jarron     (501) staff       (20)      167 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.nircam_grism_wref.rst
--rw-r--r--   0 jarron     (501) staff       (20)      158 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.nircam_lyot_th.rst
--rw-r--r--   0 jarron     (501) staff       (20)      164 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.niriss_grism_res.rst
--rw-r--r--   0 jarron     (501) staff       (20)      167 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.niriss_grism_wref.rst
--rw-r--r--   0 jarron     (501) staff       (20)      141 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.qe_nircam.rst
--rw-r--r--   0 jarron     (501) staff       (20)      164 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.qe_nircam_flight.rst
--rw-r--r--   0 jarron     (501) staff       (20)      173 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.qe_nircam_preflight.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.qe_nirspec.rst
--rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.read_filter.rst
--rw-r--r--   0 jarron     (501) staff       (20)      615 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.rst
--rw-r--r--   0 jarron     (501) staff       (20)      158 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.coords.NIRCam_V2V3_limits.rst
--rw-r--r--   0 jarron     (501) staff       (20)      126 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.coords.ap_radec.rst
--rw-r--r--   0 jarron     (501) staff       (20)      146 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.coords.convert_to_sky.rst
--rw-r--r--   0 jarron     (501) staff       (20)      132 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.coords.dist_image.rst
--rw-r--r--   0 jarron     (501) staff       (20)      149 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.coords.gen_sgd_offsets.rst
--rw-r--r--   0 jarron     (501) staff       (20)      163 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.coords.get_NRC_v2v3_limits.rst
--rw-r--r--   0 jarron     (501) staff       (20)      146 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.coords.get_idl_offset.rst
--rw-r--r--   0 jarron     (501) staff       (20)      149 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.coords.get_sgd_offsets.rst
--rw-r--r--   0 jarron     (501) staff       (20)      793 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.coords.jwst_point.rst
--rw-r--r--   0 jarron     (501) staff       (20)      124 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.coords.plotAxes.rst
--rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.coords.radec_offset.rst
--rw-r--r--   0 jarron     (501) staff       (20)      146 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.coords.radec_to_coord.rst
--rw-r--r--   0 jarron     (501) staff       (20)      143 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.coords.radec_to_v2v3.rst
--rw-r--r--   0 jarron     (501) staff       (20)      647 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.coords.rst
--rw-r--r--   0 jarron     (501) staff       (20)      140 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.coords.rtheta_to_xy.rst
--rw-r--r--   0 jarron     (501) staff       (20)      143 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.coords.v2v3_to_pixel.rst
--rw-r--r--   0 jarron     (501) staff       (20)      120 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.coords.xy_rot.rst
--rw-r--r--   0 jarron     (501) staff       (20)      140 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.coords.xy_to_rtheta.rst
--rw-r--r--   0 jarron     (501) staff       (20)      140 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.add_ipc.rst
--rw-r--r--   0 jarron     (501) staff       (20)      140 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.add_ppc.rst
--rw-r--r--   0 jarron     (501) staff       (20)      184 2024-05-14 05:05:00.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.apply_pixel_diffusion.rst
--rw-r--r--   0 jarron     (501) staff       (20)      137 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.bp_fix.rst
--rw-r--r--   0 jarron     (501) staff       (20)      161 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.convolve_image.rst
--rw-r--r--   0 jarron     (501) staff       (20)      149 2024-05-14 05:05:00.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.crop_image.rst
--rw-r--r--   0 jarron     (501) staff       (20)      167 2024-05-14 05:05:00.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.crop_observation.rst
--rw-r--r--   0 jarron     (501) staff       (20)      180 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.crop_zero_rows_cols.rst
--rw-r--r--   0 jarron     (501) staff       (20)      143 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.cv_shift.rst
--rw-r--r--   0 jarron     (501) staff       (20)      158 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.distort_image.rst
--rw-r--r--   0 jarron     (501) staff       (20)      152 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.expand_mask.rst
--rw-r--r--   0 jarron     (501) staff       (20)      164 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.fourier_imshift.rst
--rw-r--r--   0 jarron     (501) staff       (20)      187 2024-05-14 05:05:00.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.fractional_image_shift.rst
--rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.frebin.rst
--rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.fshift.rst
--rw-r--r--   0 jarron     (501) staff       (20)      151 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.get_im_cen.rst
--rw-r--r--   0 jarron     (501) staff       (20)      158 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.image_rescale.rst
--rw-r--r--   0 jarron     (501) staff       (20)      166 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.make_disk_image.rst
--rw-r--r--   0 jarron     (501) staff       (20)      169 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.model_to_hdulist.rst
--rw-r--r--   0 jarron     (501) staff       (20)      179 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.pad_or_cut_to_size.rst
--rw-r--r--   0 jarron     (501) staff       (20)      158 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.rotate_offset.rst
--rw-r--r--   0 jarron     (501) staff       (20)      175 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.rotate_shift_image.rst
--rw-r--r--   0 jarron     (501) staff       (20)      659 2024-05-14 05:05:00.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.rst
--rw-r--r--   0 jarron     (501) staff       (20)      397 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.logging_utils.FilterLevelRange.rst
--rw-r--r--   0 jarron     (501) staff       (20)      170 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.logging_utils.restart_logging.rst
--rw-r--r--   0 jarron     (501) staff       (20)      403 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.logging_utils.rst
--rw-r--r--   0 jarron     (501) staff       (20)      164 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.logging_utils.setup_logging.rst
--rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.maths.binned_statistic.rst
--rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.maths.find_closest.rst
--rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.maths.fit_bootstrap.rst
--rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.maths.hist_indices.rst
--rw-r--r--   0 jarron     (501) staff       (20)      120 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.maths.jl_poly.rst
--rw-r--r--   0 jarron     (501) staff       (20)      134 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.maths.jl_poly_fit.rst
--rw-r--r--   0 jarron     (501) staff       (20)      129 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.maths.radial_std.rst
--rw-r--r--   0 jarron     (501) staff       (20)      126 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.maths.round_int.rst
--rw-r--r--   0 jarron     (501) staff       (20)      347 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.maths.rst
--rw-r--r--   0 jarron     (501) staff       (20)      152 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.opds.OPDFile_to_HDUList.rst
--rw-r--r--   0 jarron     (501) staff       (20)     1961 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.opds.OTE_WFE_Drift_Model.rst
--rw-r--r--   0 jarron     (501) staff       (20)      117 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.opds.plot_im.rst
--rw-r--r--   0 jarron     (501) staff       (20)      120 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.opds.plot_opd.rst
--rw-r--r--   0 jarron     (501) staff       (20)      405 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.opds.rst
--rw-r--r--   0 jarron     (501) staff       (20)      123 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.opds.slew_time.rst
--rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.psfs.create_obslist.rst
--rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.psfs.create_waveset.rst
--rw-r--r--   0 jarron     (501) staff       (20)      146 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.psfs.field_coeff_func.rst
--rw-r--r--   0 jarron     (501) staff       (20)      160 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.psfs.gen_image_from_coeff.rst
--rw-r--r--   0 jarron     (501) staff       (20)      163 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.psfs.make_coeff_resid_grid.rst
--rw-r--r--   0 jarron     (501) staff       (20)      123 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.psfs.nproc_use.rst
--rw-r--r--   0 jarron     (501) staff       (20)      334 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.psfs.rst
--rw-r--r--   0 jarron     (501) staff       (20)      136 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.robust.biweightMean.rst
--rw-r--r--   0 jarron     (501) staff       (20)      124 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.robust.checkfit.rst
--rw-r--r--   0 jarron     (501) staff       (20)      121 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.robust.linefit.rst
--rw-r--r--   0 jarron     (501) staff       (20)      112 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.robust.mean.rst
--rw-r--r--   0 jarron     (501) staff       (20)      127 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.robust.medabsdev.rst
--rw-r--r--   0 jarron     (501) staff       (20)      112 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.robust.mode.rst
--rw-r--r--   0 jarron     (501) staff       (20)      121 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.robust.polyfit.rst
--rw-r--r--   0 jarron     (501) staff       (20)      314 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.robust.rst
--rw-r--r--   0 jarron     (501) staff       (20)      109 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.robust.std.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.spectra.BOSZ_filename.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.spectra.BOSZ_spectrum.rst
--rw-r--r--   0 jarron     (501) staff       (20)      141 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.spectra.bin_spectrum.rst
--rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.spectra.companion_spec.rst
--rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.spectra.cond_filter.rst
--rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.spectra.cond_table.rst
--rw-r--r--   0 jarron     (501) staff       (20)      173 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.spectra.download_BOSZ_spectrum.rst
--rw-r--r--   0 jarron     (501) staff       (20)      153 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.spectra.download_votable.rst
--rw-r--r--   0 jarron     (501) staff       (20)      141 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.spectra.jupiter_spec.rst
--rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.spectra.linder_filter.rst
--rw-r--r--   0 jarron     (501) staff       (20)      141 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.spectra.linder_table.rst
--rw-r--r--   0 jarron     (501) staff       (20)      146 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.spectra.mag_to_counts.rst
--rw-r--r--   0 jarron     (501) staff       (20)      173 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.spectra.mass_sensitivity_table.rst
--rw-r--r--   0 jarron     (501) staff       (20)      753 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.spectra.planets_sb12.rst
--rw-r--r--   0 jarron     (501) staff       (20)      670 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.spectra.rst
--rw-r--r--   0 jarron     (501) staff       (20)      543 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.spectra.source_spectrum.rst
--rw-r--r--   0 jarron     (501) staff       (20)      126 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.spectra.sp_accr.rst
--rw-r--r--   0 jarron     (501) staff       (20)      153 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.spectra.stellar_spectrum.rst
--rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.utils.check_fitsgz.rst
--rw-r--r--   0 jarron     (501) staff       (20)      132 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.utils.get_detname.rst
--rw-r--r--   0 jarron     (501) staff       (20)      137 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.utils.get_one_siaf.rst
--rw-r--r--   0 jarron     (501) staff       (20)      143 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.utils.load_plt_style.rst
--rw-r--r--   0 jarron     (501) staff       (20)      137 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.utils.pix_ang_size.rst
--rw-r--r--   0 jarron     (501) staff       (20)      297 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.utils.rst
--rw-r--r--   0 jarron     (501) staff       (20)     2060 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.webbpsf_ext_core.MIRI_ext.rst
--rw-r--r--   0 jarron     (501) staff       (20)     2596 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.webbpsf_ext_core.NIRCam_ext.rst
--rw-r--r--   0 jarron     (501) staff       (20)      166 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.webbpsf_ext_core.coron_grid.rst
--rw-r--r--   0 jarron     (501) staff       (20)      180 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.webbpsf_ext_core.nrc_mask_trans.rst
--rw-r--r--   0 jarron     (501) staff       (20)      419 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.webbpsf_ext_core.rst
--rw-r--r--   0 jarron     (501) staff       (20)      354 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/detector_classes.rst
--rw-r--r--   0 jarron     (501) staff       (20)      201 2023-06-14 14:41:38.000000 pynrc-1.2.0/docs/api/obs_classes.rst
--rw-r--r--   0 jarron     (501) staff       (20)      200 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/reduction.rst
--rw-r--r--   0 jarron     (501) staff       (20)      221 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/simul.rst
--rw-r--r--   0 jarron     (501) staff       (20)      246 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/utils.rst
--rw-r--r--   0 jarron     (501) staff       (20)      291 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api/webbpsf_ext.rst
--rw-r--r--   0 jarron     (501) staff       (20)      202 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/api.rst
--rw-r--r--   0 jarron     (501) staff       (20)       52 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/change_log.rst
--rw-r--r--   0 jarron     (501) staff       (20)     6101 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/conf.py
--rw-r--r--   0 jarron     (501) staff       (20)       33 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/contributing.rst
--rw-r--r--   0 jarron     (501) staff       (20)     2006 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/index.rst
--rw-r--r--   0 jarron     (501) staff       (20)    10026 2024-05-14 04:44:59.000000 pynrc-1.2.0/docs/install_clean.rst
--rw-r--r--   0 jarron     (501) staff       (20)     4056 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/installation.rst
--rw-r--r--   0 jarron     (501) staff       (20)     1202 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/license.rst
--rw-r--r--   0 jarron     (501) staff       (20)      809 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/make.bat
-drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-14 05:07:03.704068 pynrc-1.2.0/docs/paper/
-drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-14 05:07:03.756359 pynrc-1.2.0/docs/paper/pandexo_paper/
--rw-r--r--   0 jarron     (501) staff       (20)     3163 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/paper/pandexo_paper/Makefile
--rw-r--r--   0 jarron     (501) staff       (20)       27 2023-06-14 14:36:11.000000 pynrc-1.2.0/docs/readme.rst
-drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-14 05:07:03.758235 pynrc-1.2.0/pynrc/
--rw-r--r--   0 jarron     (501) staff       (20)     4222 2023-06-14 14:41:38.000000 pynrc-1.2.0/pynrc/__init__.py
--rw-r--r--   0 jarron     (501) staff       (20)    55121 2023-06-14 14:41:38.000000 pynrc-1.2.0/pynrc/detops.py
--rw-r--r--   0 jarron     (501) staff       (20)     5257 2023-06-14 14:41:38.000000 pynrc-1.2.0/pynrc/logging_utils.py
-drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-14 05:07:03.759818 pynrc-1.2.0/pynrc/maths/
--rw-r--r--   0 jarron     (501) staff       (20)       31 2023-06-14 14:36:13.000000 pynrc-1.2.0/pynrc/maths/__init__.py
--rw-r--r--   0 jarron     (501) staff       (20)    27869 2023-06-14 14:36:13.000000 pynrc-1.2.0/pynrc/maths/_robust.py
--rw-r--r--   0 jarron     (501) staff       (20)     5845 2024-05-14 04:44:59.000000 pynrc-1.2.0/pynrc/maths/coords.py
--rw-r--r--   0 jarron     (501) staff       (20)      213 2023-06-14 14:36:13.000000 pynrc-1.2.0/pynrc/maths/fast_poly.py
--rw-r--r--   0 jarron     (501) staff       (20)    21477 2024-05-14 04:44:59.000000 pynrc-1.2.0/pynrc/maths/image_manip.py
--rw-r--r--   0 jarron     (501) staff       (20)    60838 2024-05-14 04:44:59.000000 pynrc-1.2.0/pynrc/nb_funcs.py
--rw-r--r--   0 jarron     (501) staff       (20)    63124 2024-05-14 04:44:59.000000 pynrc-1.2.0/pynrc/nrc_utils.py
--rw-r--r--   0 jarron     (501) staff       (20)   116379 2024-05-14 04:44:59.000000 pynrc-1.2.0/pynrc/obs_nircam.py
--rw-r--r--   0 jarron     (501) staff       (20)     1149 2023-06-14 14:36:13.000000 pynrc-1.2.0/pynrc/opds.py
--rw-r--r--   0 jarron     (501) staff       (20)   138443 2024-05-14 04:44:59.000000 pynrc-1.2.0/pynrc/pynrc_core.py
-drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-14 05:07:03.761117 pynrc-1.2.0/pynrc/reduce/
--rw-r--r--   0 jarron     (501) staff       (20)        0 2023-06-14 14:36:13.000000 pynrc-1.2.0/pynrc/reduce/__init__.py
--rw-r--r--   0 jarron     (501) staff       (20)   113058 2024-05-14 04:44:59.000000 pynrc-1.2.0/pynrc/reduce/analysis.py
--rw-r--r--   0 jarron     (501) staff       (20)   204848 2023-06-14 14:41:38.000000 pynrc-1.2.0/pynrc/reduce/calib.py
--rw-r--r--   0 jarron     (501) staff       (20)    52586 2024-05-14 04:44:59.000000 pynrc-1.2.0/pynrc/reduce/nmf.py
--rw-r--r--   0 jarron     (501) staff       (20)    37560 2024-05-14 04:44:59.000000 pynrc-1.2.0/pynrc/reduce/pca.py
--rw-r--r--   0 jarron     (501) staff       (20)    49931 2023-06-14 14:41:38.000000 pynrc-1.2.0/pynrc/reduce/ref_pixels.py
-drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-14 05:07:03.762188 pynrc-1.2.0/pynrc/simul/
--rw-r--r--   0 jarron     (501) staff       (20)        0 2023-06-14 14:36:13.000000 pynrc-1.2.0/pynrc/simul/__init__.py
--rw-r--r--   0 jarron     (501) staff       (20)    42594 2023-06-14 14:36:13.000000 pynrc-1.2.0/pynrc/simul/_nghxrg.py
--rw-r--r--   0 jarron     (501) staff       (20)   294607 2023-06-14 14:41:38.000000 pynrc-1.2.0/pynrc/simul/apt.py
--rw-r--r--   0 jarron     (501) staff       (20)    37043 2023-06-14 14:41:38.000000 pynrc-1.2.0/pynrc/simul/dms.py
--rw-r--r--   0 jarron     (501) staff       (20)   121399 2024-05-14 04:44:59.000000 pynrc-1.2.0/pynrc/simul/ngNRC.py
--rw-r--r--   0 jarron     (501) staff       (20)    20489 2023-06-14 14:36:13.000000 pynrc-1.2.0/pynrc/simul/skyvec2ins.py
--rw-r--r--   0 jarron     (501) staff       (20)    34331 2024-05-14 04:44:59.000000 pynrc-1.2.0/pynrc/speckle_noise.py
--rw-r--r--   0 jarron     (501) staff       (20)     4424 2023-06-14 14:41:38.000000 pynrc-1.2.0/pynrc/testing.py
--rw-r--r--   0 jarron     (501) staff       (20)      150 2024-05-14 05:04:39.000000 pynrc-1.2.0/pynrc/version.py
-drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-14 05:07:03.759122 pynrc-1.2.0/pynrc.egg-info/
--rw-r--r--   0 jarron     (501) staff       (20)     9200 2024-05-14 05:07:03.000000 pynrc-1.2.0/pynrc.egg-info/PKG-INFO
--rw-r--r--   0 jarron     (501) staff       (20)    24006 2024-05-14 05:07:03.000000 pynrc-1.2.0/pynrc.egg-info/SOURCES.txt
--rw-r--r--   0 jarron     (501) staff       (20)        1 2024-05-14 05:07:03.000000 pynrc-1.2.0/pynrc.egg-info/dependency_links.txt
--rw-r--r--   0 jarron     (501) staff       (20)        1 2024-05-14 05:07:03.000000 pynrc-1.2.0/pynrc.egg-info/not-zip-safe
--rw-r--r--   0 jarron     (501) staff       (20)      114 2024-05-14 05:07:03.000000 pynrc-1.2.0/pynrc.egg-info/requires.txt
--rw-r--r--   0 jarron     (501) staff       (20)        6 2024-05-14 05:07:03.000000 pynrc-1.2.0/pynrc.egg-info/top_level.txt
--rw-r--r--   0 jarron     (501) staff       (20)      349 2024-05-14 05:07:03.763050 pynrc-1.2.0/setup.cfg
--rwxr-xr-x   0 jarron     (501) staff       (20)     5445 2024-05-14 05:02:07.000000 pynrc-1.2.0/setup.py
-drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-14 05:07:03.762546 pynrc-1.2.0/tests/
--rw-r--r--   0 jarron     (501) staff       (20)      407 2023-06-14 14:36:13.000000 pynrc-1.2.0/tests/cli.py.old.py
--rw-r--r--   0 jarron     (501) staff       (20)      255 2023-06-14 14:36:13.000000 pynrc-1.2.0/tests/test_pynrc.py
--rw-r--r--   0 jarron     (501) staff       (20)      982 2023-06-14 14:36:13.000000 pynrc-1.2.0/tests/test_pynrc.py.old
+drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-24 18:46:08.485890 pynrc-1.2.1/
+-rw-r--r--   0 jarron     (501) staff       (20)     5862 2024-05-14 05:27:40.000000 pynrc-1.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 jarron     (501) staff       (20)     4597 2024-05-14 05:27:40.000000 pynrc-1.2.1/HISTORY.rst
+-rw-r--r--   0 jarron     (501) staff       (20)     1076 2023-06-14 14:36:11.000000 pynrc-1.2.1/LICENSE
+-rw-r--r--   0 jarron     (501) staff       (20)      337 2023-06-14 14:36:11.000000 pynrc-1.2.1/MANIFEST.in
+-rw-r--r--   0 jarron     (501) staff       (20)     9360 2024-05-24 18:46:08.485982 pynrc-1.2.1/PKG-INFO
+-rw-r--r--   0 jarron     (501) staff       (20)     4114 2024-05-14 05:17:56.000000 pynrc-1.2.1/README.rst
+drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-24 18:46:08.423089 pynrc-1.2.1/docs/
+-rw-r--r--   0 jarron     (501) staff       (20)      602 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/Makefile
+drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-24 18:46:08.419662 pynrc-1.2.1/docs/_build/
+drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-24 18:46:08.419578 pynrc-1.2.1/docs/_build/doctrees/
+drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-24 18:46:08.426103 pynrc-1.2.1/docs/_build/doctrees/nbsphinx/
+-rw-r--r--   0 jarron     (501) staff       (20)    49182 2024-05-24 18:44:35.000000 pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Basic_Usage_14_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    19831 2024-05-24 18:44:35.000000 pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Basic_Usage_16_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    19084 2024-05-24 18:44:35.000000 pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Basic_Usage_27_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    24012 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_20_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    59331 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_26_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    59832 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_29_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    61999 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_32_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    12453 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_40_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    32158 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_8_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    29633 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Wedges_10_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    25092 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Wedges_20_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    78390 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Wedges_24_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    47901 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Wedges_26_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    42386 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Wedges_9_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    40325 2024-05-24 18:44:37.000000 pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_HR8799_DMS_Level1b_11_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    50157 2024-05-24 18:44:38.000000 pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Ramp_Optimization_Examples_30_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    13328 2024-05-24 18:44:38.000000 pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Ramp_Optimization_Examples_32_1.png
+-rw-r--r--   0 jarron     (501) staff       (20)    48589 2024-05-24 18:44:38.000000 pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Ramp_Optimization_Examples_35_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    21707 2024-05-24 18:44:38.000000 pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Ramp_Optimization_Examples_43_1.png
+drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-24 18:46:08.419799 pynrc-1.2.1/docs/_build/html/
+drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-24 18:46:08.429664 pynrc-1.2.1/docs/_build/html/_images/
+-rw-r--r--   0 jarron     (501) staff       (20)    49182 2024-05-24 18:44:35.000000 pynrc-1.2.1/docs/_build/html/_images/tutorials_Basic_Usage_14_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    19831 2024-05-24 18:44:35.000000 pynrc-1.2.1/docs/_build/html/_images/tutorials_Basic_Usage_16_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    19084 2024-05-24 18:44:35.000000 pynrc-1.2.1/docs/_build/html/_images/tutorials_Basic_Usage_27_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    24012 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Basics_20_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    59331 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Basics_26_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    59832 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Basics_29_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    61999 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Basics_32_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    12453 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Basics_40_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    32158 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Basics_8_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    29633 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Wedges_10_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    25092 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Wedges_20_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    78390 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Wedges_24_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    47901 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Wedges_26_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    42386 2024-05-24 18:44:36.000000 pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Wedges_9_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    40325 2024-05-24 18:44:37.000000 pynrc-1.2.1/docs/_build/html/_images/tutorials_HR8799_DMS_Level1b_11_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    50157 2024-05-24 18:44:38.000000 pynrc-1.2.1/docs/_build/html/_images/tutorials_Ramp_Optimization_Examples_30_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    13328 2024-05-24 18:44:38.000000 pynrc-1.2.1/docs/_build/html/_images/tutorials_Ramp_Optimization_Examples_32_1.png
+-rw-r--r--   0 jarron     (501) staff       (20)    48589 2024-05-24 18:44:38.000000 pynrc-1.2.1/docs/_build/html/_images/tutorials_Ramp_Optimization_Examples_35_0.png
+-rw-r--r--   0 jarron     (501) staff       (20)    21707 2024-05-24 18:44:38.000000 pynrc-1.2.1/docs/_build/html/_images/tutorials_Ramp_Optimization_Examples_43_1.png
+drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-24 18:46:08.430078 pynrc-1.2.1/docs/_build/html/_static/
+-rw-r--r--   0 jarron     (501) staff       (20)      286 2022-07-14 07:38:21.000000 pynrc-1.2.1/docs/_build/html/_static/file.png
+-rw-r--r--   0 jarron     (501) staff       (20)       90 2022-07-14 07:38:21.000000 pynrc-1.2.1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 jarron     (501) staff       (20)       90 2022-07-14 07:38:21.000000 pynrc-1.2.1/docs/_build/html/_static/plus.png
+drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-24 18:46:08.430457 pynrc-1.2.1/docs/_templates/
+-rw-r--r--   0 jarron     (501) staff       (20)      106 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/_templates/base.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      611 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/_templates/custom-class-template.rst
+-rw-r--r--   0 jarron     (501) staff       (20)     1219 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/_templates/custom-module-template.rst
+drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-24 18:46:08.431261 pynrc-1.2.1/docs/api/
+drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-24 18:46:08.479601 pynrc-1.2.1/docs/api/_autosummary/
+-rw-r--r--   0 jarron     (501) staff       (20)     1492 2023-06-14 14:41:38.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.DetectorOps.rst
+-rw-r--r--   0 jarron     (501) staff       (20)     2855 2024-05-14 04:44:59.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.NIRCam.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      104 2023-06-14 14:41:38.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.detops.config2.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      124 2023-06-14 14:41:38.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.detops.create_detops.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      115 2023-06-14 14:41:38.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.detops.nrc_header.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      377 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.logging_utils.FilterLevelRange.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      150 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.logging_utils.restart_logging.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      383 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.logging_utils.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.logging_utils.setup_logging.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      136 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.maths.coords.Tel2Sci_info.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      132 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.maths.coords.det_to_sci.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      245 2024-05-14 04:44:59.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.maths.coords.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      132 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.maths.coords.sci_to_det.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      153 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.maths.coords.siafap_sci_coords.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.maths.image_manip.align_LSQ.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      156 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.maths.image_manip.align_leastsq.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      147 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.maths.image_manip.crop_image.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      165 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.maths.image_manip.crop_observation.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      172 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.maths.image_manip.fix_nans_with_med.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      171 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.maths.image_manip.optimal_difference.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      406 2024-05-14 04:44:59.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.maths.image_manip.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      164 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.maths.image_manip.scale_ref_image.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      159 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.maths.image_manip.shift_subtract.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      153 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.maths.image_manip.subtract_psf.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      629 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.multiaccum.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      132 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.average_slopes.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      134 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.disk_rim_model.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      123 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.do_contrast.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      125 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.do_gen_hdus.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      108 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.do_opt.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      143 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.do_plot_contrasts.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      146 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.do_plot_contrasts2.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      131 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.do_sat_levels.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      114 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.make_key.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      120 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.model_info.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      126 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.obs_optimize.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      111 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.obs_wfe.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      123 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.planet_mags.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      132 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.plot_contrasts.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      149 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.plot_contrasts_mjup.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      126 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.plot_hdulist.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      123 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.plot_images.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      140 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.plot_images_swlw.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      149 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.plot_planet_patches.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      129 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.plot_spectrum.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      608 2024-05-14 04:44:59.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      129 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.update_yscale.rst
+-rw-r--r--   0 jarron     (501) staff       (20)     3080 2024-05-14 04:44:59.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_hci.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      154 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.bias_dark_high_temp.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      129 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.bin_spectrum.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      123 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.build_mask.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      143 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.build_mask_detid.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.channel_select.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      134 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.coron_ap_locs.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.coron_detector.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      126 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.coron_trans.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      134 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.dark_ramp_80K.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      152 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.do_charge_migration.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      111 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.do_fft.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      201 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.gen_unconvolved_point_source_image.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      126 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.get_detname.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      141 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.grism_background.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      155 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.grism_background_com.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      161 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.grism_background_image.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      143 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.make_grism_slope.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      149 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.nproc_use_convolve.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      123 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.offset_bar.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      132 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.pickoff_image.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      123 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.pickoff_xy.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      120 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.pix_noise.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      143 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.place_grism_spec.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      143 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.place_grismr_tso.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      662 2024-05-14 04:44:59.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      146 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.segment_pupil_opd.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      131 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.var_ex_model.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      126 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.zodi_euclid.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      120 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.zodi_spec.rst
+-rw-r--r--   0 jarron     (501) staff       (20)     3574 2024-05-14 04:44:59.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.obs_hci.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      108 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.opds.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      145 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.apply_linearity.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      136 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.apply_nonlin.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      118 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.bp_fix.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      159 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.broken_pink_powspec.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      139 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.calc_cdsnoise.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.calc_eff_noise.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      124 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.calc_ktc.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      162 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.calc_linearity_coeff.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      153 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.calc_nonlin_coeff.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      130 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.chisqr_red.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      124 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.cube_fit.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      159 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.deconv_single_image.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      150 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.detname_to_scaid.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.find_group_sat.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      124 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.find_sat.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      150 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.fit_corr_powspec.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      149 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.fit_func_var_ex.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.gen_cds_dict.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      156 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.gen_col_variations.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.gen_ref_dict.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.gen_super_bias.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.gen_super_dark.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.gen_super_ramp.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      150 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.get_bias_offsets.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      141 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.get_fits_data.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.get_flat_fields.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.get_freq_array.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.get_ipc_kernel.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      153 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.get_linear_coeffs.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      159 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.get_oddeven_offsets.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.get_power_spec.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      158 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.get_power_spec_all.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      159 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.get_ref_instability.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      142 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.ipc_deconvolve.rst
+-rw-r--r--   0 jarron     (501) staff       (20)     2344 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.nircam_cal.rst
+-rw-r--r--   0 jarron     (501) staff       (20)     2408 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.nircam_dark.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      165 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.pixel_linearity_gains.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      159 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.plot_dark_histogram.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      133 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.plot_kernel.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      141 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.pow_spec_ramp.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      155 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.pow_spec_ramp_pix.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      142 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.ppc_deconvolve.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      145 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.ramp_derivative.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      139 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.ramp_resample.rst
+-rw-r--r--   0 jarron     (501) staff       (20)     1257 2023-06-14 14:41:38.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.time_to_sat.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      787 2023-06-14 14:41:38.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.ref_pixels.NRC_refs.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      158 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.ref_pixels.calc_avg_amps.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      158 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.ref_pixels.calc_avg_cols.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      164 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.ref_pixels.calc_col_smooth.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      168 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.ref_pixels.channel_averaging.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      182 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.ref_pixels.channel_smooth_butter.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      173 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.ref_pixels.channel_smooth_fft.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      182 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.ref_pixels.channel_smooth_savgol.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.ref_pixels.chrem_med.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      150 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.ref_pixels.mask_helper.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.ref_pixels.ref_filter.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      150 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.ref_pixels.reffix_amps.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      150 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.ref_pixels.reffix_hxrg.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      616 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.ref_pixels.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.ref_pixels.smooth_fft.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      764 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.AptInput.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      570 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.DMS_input.rst
+-rw-r--r--   0 jarron     (501) staff       (20)     1100 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.ReadAPTXML.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      152 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.build_dict_from_xml.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      141 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.create_det_class.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.create_obs_params.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      136 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.file_segmenting.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      149 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.gen_all_apt_visits.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.gen_jwst_pointing.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.gen_pointing_info.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      133 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.get_ditherinfo.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      129 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.get_exp_type.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.get_filter_info.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.get_orient_specreq.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.get_pointing_info.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.get_proposal_info.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      130 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.get_readmodes.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      132 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.get_roll_info.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.get_siaf_detectors.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.get_target_info.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.get_tel_angles.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.get_timing_info.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      132 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.pitch_vs_time.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      150 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.populate_obs_params.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      182 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.read_subarray_definition_file.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      924 2023-06-14 14:41:38.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      153 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.update_eng_detectors.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      162 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.update_subarray_imaging.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      127 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.dms.DMS_filename.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.dms.compute_local_roll.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.dms.create_DMS_HDUList.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.dms.create_group_entry.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      132 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.dms.dec_to_base36.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      150 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.dms.filename_visit_info.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      120 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.dms.jw_obs_id.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.dms.level1b_data_model.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      153 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.dms.populate_group_table.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      482 2023-06-14 14:41:38.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.dms.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.dms.save_level1b_fits.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.dms.update_dms_headers.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      170 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.dms.update_headers_pynrc_info.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.add_col_noise.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.add_cosmic_rays.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      118 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.add_ipc.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      118 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.add_ppc.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      124 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.add_xtalk.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      127 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.apply_flat.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      156 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.create_level1b_FITS.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      124 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.fft_noise.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.gen_col_noise.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.gen_dark_ramp.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.gen_ramp_biases.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.gen_wfe_drift.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      167 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.make_gaia_source_table.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      150 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.make_ramp_poisson.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      173 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.make_simbad_source_table.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      127 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.pink_noise.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      728 2024-05-14 04:44:59.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.save_slope_image.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.sim_dark_ramp.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      141 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.sim_image_ramp.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      141 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.sim_noise_data.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      165 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.simulate_detector_ramp.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      156 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.slope_to_fitswriter.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.slope_to_level1b.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      153 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.sources_to_level1b.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.sources_to_slope.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      130 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.xtalk_image.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      125 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.skyvec2ins.ad2lb.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      125 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.skyvec2ins.ei2lb.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      125 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.skyvec2ins.lb2ad.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      125 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.skyvec2ins.lb2ei.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      308 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.skyvec2ins.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      140 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.skyvec2ins.skyvec2ins.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      180 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.skyvec2ins.sun_ecliptic_longitude.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.bp_2mass.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.bp_gaia.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.bp_igood.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.bp_wise.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      150 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.filter_width.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.miri_filter.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      155 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.nircam_com_nd.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      155 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.nircam_com_th.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      153 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.nircam_filter.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      164 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.nircam_grism_res.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      172 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.nircam_grism_si_ar.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      161 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.nircam_grism_th.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      167 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.nircam_grism_wref.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      158 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.nircam_lyot_th.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      164 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.niriss_grism_res.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      167 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.niriss_grism_wref.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      141 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.qe_nircam.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      164 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.qe_nircam_flight.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      173 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.qe_nircam_preflight.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.qe_nirspec.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.read_filter.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      615 2024-05-14 04:44:59.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      158 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.coords.NIRCam_V2V3_limits.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      126 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.coords.ap_radec.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      146 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.coords.convert_to_sky.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      132 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.coords.dist_image.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      149 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.coords.gen_sgd_offsets.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      163 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.coords.get_NRC_v2v3_limits.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      146 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.coords.get_idl_offset.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      149 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.coords.get_sgd_offsets.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      793 2023-06-14 14:41:38.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.coords.jwst_point.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      124 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.coords.plotAxes.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.coords.radec_offset.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      146 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.coords.radec_to_coord.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      143 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.coords.radec_to_v2v3.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      647 2024-05-14 04:44:59.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.coords.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      140 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.coords.rtheta_to_xy.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      143 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.coords.v2v3_to_pixel.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      120 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.coords.xy_rot.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      140 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.coords.xy_to_rtheta.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      140 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.add_ipc.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      140 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.add_ppc.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      184 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.apply_pixel_diffusion.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      137 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.bp_fix.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      161 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.convolve_image.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      149 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.crop_image.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      167 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.crop_observation.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      180 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.crop_zero_rows_cols.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      143 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.cv_shift.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      158 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.distort_image.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      152 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.expand_mask.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      164 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.fourier_imshift.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      187 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.fractional_image_shift.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.frebin.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.fshift.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      151 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.get_im_cen.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      158 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.image_rescale.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      166 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.make_disk_image.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      169 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.model_to_hdulist.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      179 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.pad_or_cut_to_size.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      158 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.rotate_offset.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      175 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.rotate_shift_image.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      659 2024-05-14 05:17:51.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      397 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.logging_utils.FilterLevelRange.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      170 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.logging_utils.restart_logging.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      403 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.logging_utils.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      164 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.logging_utils.setup_logging.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.maths.binned_statistic.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.maths.find_closest.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.maths.fit_bootstrap.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.maths.hist_indices.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      120 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.maths.jl_poly.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      134 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.maths.jl_poly_fit.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      129 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.maths.radial_std.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      126 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.maths.round_int.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      347 2024-05-14 04:44:59.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.maths.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      152 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.opds.OPDFile_to_HDUList.rst
+-rw-r--r--   0 jarron     (501) staff       (20)     1961 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.opds.OTE_WFE_Drift_Model.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      117 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.opds.plot_im.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      120 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.opds.plot_opd.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      405 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.opds.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      123 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.opds.slew_time.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.psfs.create_obslist.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.psfs.create_waveset.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      146 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.psfs.field_coeff_func.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      160 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.psfs.gen_image_from_coeff.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      163 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.psfs.make_coeff_resid_grid.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      123 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.psfs.nproc_use.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      334 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.psfs.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      136 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.robust.biweightMean.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      124 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.robust.checkfit.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      121 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.robust.linefit.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      112 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.robust.mean.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      127 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.robust.medabsdev.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      112 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.robust.mode.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      121 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.robust.polyfit.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      314 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.robust.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      109 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.robust.std.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.spectra.BOSZ_filename.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.spectra.BOSZ_spectrum.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      141 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.spectra.bin_spectrum.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      147 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.spectra.companion_spec.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      138 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.spectra.cond_filter.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.spectra.cond_table.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      173 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.spectra.download_BOSZ_spectrum.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      153 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.spectra.download_votable.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      141 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.spectra.jupiter_spec.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      144 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.spectra.linder_filter.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      141 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.spectra.linder_table.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      146 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.spectra.mag_to_counts.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      173 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.spectra.mass_sensitivity_table.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      753 2024-05-14 04:44:59.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.spectra.planets_sb12.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      670 2024-05-14 04:44:59.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.spectra.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      543 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.spectra.source_spectrum.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      126 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.spectra.sp_accr.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      153 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.spectra.stellar_spectrum.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      135 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.utils.check_fitsgz.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      132 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.utils.get_detname.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      137 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.utils.get_one_siaf.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      143 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.utils.load_plt_style.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      137 2024-05-14 05:27:40.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.utils.pix_ang_size.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      297 2024-05-14 04:44:59.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.utils.rst
+-rw-r--r--   0 jarron     (501) staff       (20)     2060 2024-05-14 04:44:59.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.webbpsf_ext_core.MIRI_ext.rst
+-rw-r--r--   0 jarron     (501) staff       (20)     2596 2024-05-14 04:44:59.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.webbpsf_ext_core.NIRCam_ext.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      166 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.webbpsf_ext_core.coron_grid.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      180 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.webbpsf_ext_core.nrc_mask_trans.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      419 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.webbpsf_ext_core.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      354 2023-06-14 14:41:38.000000 pynrc-1.2.1/docs/api/detector_classes.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      201 2023-06-14 14:41:38.000000 pynrc-1.2.1/docs/api/obs_classes.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      200 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/reduction.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      221 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/simul.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      246 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/utils.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      291 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api/webbpsf_ext.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      202 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/api.rst
+-rw-r--r--   0 jarron     (501) staff       (20)       52 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/change_log.rst
+-rw-r--r--   0 jarron     (501) staff       (20)     6101 2024-05-14 04:44:59.000000 pynrc-1.2.1/docs/conf.py
+-rw-r--r--   0 jarron     (501) staff       (20)       33 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/contributing.rst
+-rw-r--r--   0 jarron     (501) staff       (20)     2006 2024-05-24 18:45:18.000000 pynrc-1.2.1/docs/index.rst
+-rw-r--r--   0 jarron     (501) staff       (20)    10026 2024-05-14 04:44:59.000000 pynrc-1.2.1/docs/install_clean.rst
+-rw-r--r--   0 jarron     (501) staff       (20)     4056 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/installation.rst
+-rw-r--r--   0 jarron     (501) staff       (20)     1202 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/license.rst
+-rw-r--r--   0 jarron     (501) staff       (20)      809 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/make.bat
+drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-24 18:46:08.420093 pynrc-1.2.1/docs/paper/
+drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-24 18:46:08.479730 pynrc-1.2.1/docs/paper/pandexo_paper/
+-rw-r--r--   0 jarron     (501) staff       (20)     3163 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/paper/pandexo_paper/Makefile
+-rw-r--r--   0 jarron     (501) staff       (20)       27 2023-06-14 14:36:11.000000 pynrc-1.2.1/docs/readme.rst
+drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-24 18:46:08.481362 pynrc-1.2.1/pynrc/
+-rw-r--r--   0 jarron     (501) staff       (20)     4222 2023-06-14 14:41:38.000000 pynrc-1.2.1/pynrc/__init__.py
+-rw-r--r--   0 jarron     (501) staff       (20)    55121 2023-06-14 14:41:38.000000 pynrc-1.2.1/pynrc/detops.py
+-rw-r--r--   0 jarron     (501) staff       (20)     5257 2023-06-14 14:41:38.000000 pynrc-1.2.1/pynrc/logging_utils.py
+drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-24 18:46:08.482830 pynrc-1.2.1/pynrc/maths/
+-rw-r--r--   0 jarron     (501) staff       (20)       31 2023-06-14 14:36:13.000000 pynrc-1.2.1/pynrc/maths/__init__.py
+-rw-r--r--   0 jarron     (501) staff       (20)    27869 2023-06-14 14:36:13.000000 pynrc-1.2.1/pynrc/maths/_robust.py
+-rw-r--r--   0 jarron     (501) staff       (20)     5845 2024-05-14 04:44:59.000000 pynrc-1.2.1/pynrc/maths/coords.py
+-rw-r--r--   0 jarron     (501) staff       (20)      213 2023-06-14 14:36:13.000000 pynrc-1.2.1/pynrc/maths/fast_poly.py
+-rw-r--r--   0 jarron     (501) staff       (20)    21477 2024-05-14 04:44:59.000000 pynrc-1.2.1/pynrc/maths/image_manip.py
+-rw-r--r--   0 jarron     (501) staff       (20)    60838 2024-05-14 04:44:59.000000 pynrc-1.2.1/pynrc/nb_funcs.py
+-rw-r--r--   0 jarron     (501) staff       (20)    63124 2024-05-14 04:44:59.000000 pynrc-1.2.1/pynrc/nrc_utils.py
+-rw-r--r--   0 jarron     (501) staff       (20)   116379 2024-05-14 04:44:59.000000 pynrc-1.2.1/pynrc/obs_nircam.py
+-rw-r--r--   0 jarron     (501) staff       (20)     1149 2023-06-14 14:36:13.000000 pynrc-1.2.1/pynrc/opds.py
+-rw-r--r--   0 jarron     (501) staff       (20)   138443 2024-05-14 04:44:59.000000 pynrc-1.2.1/pynrc/pynrc_core.py
+drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-24 18:46:08.483946 pynrc-1.2.1/pynrc/reduce/
+-rw-r--r--   0 jarron     (501) staff       (20)        0 2023-06-14 14:36:13.000000 pynrc-1.2.1/pynrc/reduce/__init__.py
+-rw-r--r--   0 jarron     (501) staff       (20)   113058 2024-05-14 05:27:40.000000 pynrc-1.2.1/pynrc/reduce/analysis.py
+-rw-r--r--   0 jarron     (501) staff       (20)   204848 2023-06-14 14:41:38.000000 pynrc-1.2.1/pynrc/reduce/calib.py
+-rw-r--r--   0 jarron     (501) staff       (20)    52586 2024-05-14 05:27:40.000000 pynrc-1.2.1/pynrc/reduce/nmf.py
+-rw-r--r--   0 jarron     (501) staff       (20)    37560 2024-05-14 05:27:40.000000 pynrc-1.2.1/pynrc/reduce/pca.py
+-rw-r--r--   0 jarron     (501) staff       (20)    49931 2023-06-14 14:41:38.000000 pynrc-1.2.1/pynrc/reduce/ref_pixels.py
+drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-24 18:46:08.485270 pynrc-1.2.1/pynrc/simul/
+-rw-r--r--   0 jarron     (501) staff       (20)        0 2023-06-14 14:36:13.000000 pynrc-1.2.1/pynrc/simul/__init__.py
+-rw-r--r--   0 jarron     (501) staff       (20)    42594 2023-06-14 14:36:13.000000 pynrc-1.2.1/pynrc/simul/_nghxrg.py
+-rw-r--r--   0 jarron     (501) staff       (20)   294607 2023-06-14 14:41:38.000000 pynrc-1.2.1/pynrc/simul/apt.py
+-rw-r--r--   0 jarron     (501) staff       (20)    37043 2023-06-14 14:41:38.000000 pynrc-1.2.1/pynrc/simul/dms.py
+-rw-r--r--   0 jarron     (501) staff       (20)   121399 2024-05-14 04:44:59.000000 pynrc-1.2.1/pynrc/simul/ngNRC.py
+-rw-r--r--   0 jarron     (501) staff       (20)    20489 2023-06-14 14:36:13.000000 pynrc-1.2.1/pynrc/simul/skyvec2ins.py
+-rw-r--r--   0 jarron     (501) staff       (20)    34331 2024-05-14 04:44:59.000000 pynrc-1.2.1/pynrc/speckle_noise.py
+-rw-r--r--   0 jarron     (501) staff       (20)     4424 2023-06-14 14:41:38.000000 pynrc-1.2.1/pynrc/testing.py
+-rw-r--r--   0 jarron     (501) staff       (20)      150 2024-05-24 18:44:04.000000 pynrc-1.2.1/pynrc/version.py
+drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-24 18:46:08.482144 pynrc-1.2.1/pynrc.egg-info/
+-rw-r--r--   0 jarron     (501) staff       (20)     9360 2024-05-24 18:46:08.000000 pynrc-1.2.1/pynrc.egg-info/PKG-INFO
+-rw-r--r--   0 jarron     (501) staff       (20)    24006 2024-05-24 18:46:08.000000 pynrc-1.2.1/pynrc.egg-info/SOURCES.txt
+-rw-r--r--   0 jarron     (501) staff       (20)        1 2024-05-24 18:46:08.000000 pynrc-1.2.1/pynrc.egg-info/dependency_links.txt
+-rw-r--r--   0 jarron     (501) staff       (20)        1 2024-05-24 18:46:08.000000 pynrc-1.2.1/pynrc.egg-info/not-zip-safe
+-rw-r--r--   0 jarron     (501) staff       (20)      114 2024-05-24 18:46:08.000000 pynrc-1.2.1/pynrc.egg-info/requires.txt
+-rw-r--r--   0 jarron     (501) staff       (20)        6 2024-05-24 18:46:08.000000 pynrc-1.2.1/pynrc.egg-info/top_level.txt
+-rw-r--r--   0 jarron     (501) staff       (20)      349 2024-05-24 18:46:08.486313 pynrc-1.2.1/setup.cfg
+-rwxr-xr-x   0 jarron     (501) staff       (20)     5445 2024-05-24 18:41:12.000000 pynrc-1.2.1/setup.py
+drwxr-xr-x   0 jarron     (501) staff       (20)        0 2024-05-24 18:46:08.485734 pynrc-1.2.1/tests/
+-rw-r--r--   0 jarron     (501) staff       (20)      407 2023-06-14 14:36:13.000000 pynrc-1.2.1/tests/cli.py.old.py
+-rw-r--r--   0 jarron     (501) staff       (20)      255 2023-06-14 14:36:13.000000 pynrc-1.2.1/tests/test_pynrc.py
+-rw-r--r--   0 jarron     (501) staff       (20)      982 2023-06-14 14:36:13.000000 pynrc-1.2.1/tests/test_pynrc.py.old
```

### Comparing `pynrc-1.2.0/CONTRIBUTING.rst` & `pynrc-1.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/HISTORY.rst` & `pynrc-1.2.1/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/LICENSE` & `pynrc-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/PKG-INFO` & `pynrc-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynrc
-Version: 1.2.0
+Version: 1.2.1
 Summary: JWST NIRCam ETC and Simulator
 Home-page: https://pynrc.readthedocs.io
 Author: Jarron Leisenring
 Author-email: jarronl@arizona.edu
 License: MIT license
 Keywords: jwst nircam etc simulator
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,15 +23,19 @@
 
 A JWST NIRCam ETC and Simulator
 ===============================
 
 .. image:: https://img.shields.io/pypi/v/pynrc.svg
         :target: https://pypi.python.org/pypi/pynrc
         :alt: Badge showing current released PyPI version
-
+        
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5829553.svg
+        :target: https://doi.org/10.5281/zenodo.5829553
+        :alt: Zenodo DOI
+   
 .. image:: https://readthedocs.org/projects/pynrc/badge/?version=latest
         :target: https://pynrc.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 *Authors:* `Jarron Leisenring <https://github.com/JarronL>`_ 
 (U. of Arizona, Steward Observatory)
```

### Comparing `pynrc-1.2.0/README.rst` & `pynrc-1.2.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 
 A JWST NIRCam ETC and Simulator
 ===============================
 
 .. image:: https://img.shields.io/pypi/v/pynrc.svg
         :target: https://pypi.python.org/pypi/pynrc
         :alt: Badge showing current released PyPI version
-
+        
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5829553.svg
+        :target: https://doi.org/10.5281/zenodo.5829553
+        :alt: Zenodo DOI
+   
 .. image:: https://readthedocs.org/projects/pynrc/badge/?version=latest
         :target: https://pynrc.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 *Authors:* `Jarron Leisenring <https://github.com/JarronL>`_ 
 (U. of Arizona, Steward Observatory)
```

### Comparing `pynrc-1.2.0/docs/Makefile` & `pynrc-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Basic_Usage_14_0.png` & `pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Basic_Usage_14_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Basic_Usage_16_0.png` & `pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Basic_Usage_16_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Basic_Usage_27_0.png` & `pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Basic_Usage_27_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_20_0.png` & `pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_20_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_26_0.png` & `pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_26_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_29_0.png` & `pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_29_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_32_0.png` & `pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_32_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_40_0.png` & `pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_40_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_8_0.png` & `pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Basics_8_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Wedges_10_0.png` & `pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Wedges_10_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Wedges_20_0.png` & `pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Wedges_20_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Wedges_24_0.png` & `pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Wedges_24_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Wedges_26_0.png` & `pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Wedges_26_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Wedges_9_0.png` & `pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Coronagraph_Wedges_9_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_HR8799_DMS_Level1b_11_0.png` & `pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_HR8799_DMS_Level1b_11_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Ramp_Optimization_Examples_30_0.png` & `pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Ramp_Optimization_Examples_30_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Ramp_Optimization_Examples_32_1.png` & `pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Ramp_Optimization_Examples_32_1.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Ramp_Optimization_Examples_35_0.png` & `pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Ramp_Optimization_Examples_35_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/doctrees/nbsphinx/tutorials_Ramp_Optimization_Examples_43_1.png` & `pynrc-1.2.1/docs/_build/doctrees/nbsphinx/tutorials_Ramp_Optimization_Examples_43_1.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/html/_images/tutorials_Basic_Usage_14_0.png` & `pynrc-1.2.1/docs/_build/html/_images/tutorials_Basic_Usage_14_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/html/_images/tutorials_Basic_Usage_16_0.png` & `pynrc-1.2.1/docs/_build/html/_images/tutorials_Basic_Usage_16_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/html/_images/tutorials_Basic_Usage_27_0.png` & `pynrc-1.2.1/docs/_build/html/_images/tutorials_Basic_Usage_27_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Basics_20_0.png` & `pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Basics_20_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Basics_26_0.png` & `pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Basics_26_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Basics_29_0.png` & `pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Basics_29_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Basics_32_0.png` & `pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Basics_32_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Basics_40_0.png` & `pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Basics_40_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Basics_8_0.png` & `pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Basics_8_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Wedges_10_0.png` & `pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Wedges_10_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Wedges_20_0.png` & `pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Wedges_20_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Wedges_24_0.png` & `pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Wedges_24_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Wedges_26_0.png` & `pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Wedges_26_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/html/_images/tutorials_Coronagraph_Wedges_9_0.png` & `pynrc-1.2.1/docs/_build/html/_images/tutorials_Coronagraph_Wedges_9_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/html/_images/tutorials_HR8799_DMS_Level1b_11_0.png` & `pynrc-1.2.1/docs/_build/html/_images/tutorials_HR8799_DMS_Level1b_11_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/html/_images/tutorials_Ramp_Optimization_Examples_30_0.png` & `pynrc-1.2.1/docs/_build/html/_images/tutorials_Ramp_Optimization_Examples_30_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/html/_images/tutorials_Ramp_Optimization_Examples_32_1.png` & `pynrc-1.2.1/docs/_build/html/_images/tutorials_Ramp_Optimization_Examples_32_1.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/html/_images/tutorials_Ramp_Optimization_Examples_35_0.png` & `pynrc-1.2.1/docs/_build/html/_images/tutorials_Ramp_Optimization_Examples_35_0.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_build/html/_images/tutorials_Ramp_Optimization_Examples_43_1.png` & `pynrc-1.2.1/docs/_build/html/_images/tutorials_Ramp_Optimization_Examples_43_1.png`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_templates/custom-class-template.rst` & `pynrc-1.2.1/docs/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/_templates/custom-module-template.rst` & `pynrc-1.2.1/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/pynrc.DetectorOps.rst` & `pynrc-1.2.1/docs/api/_autosummary/pynrc.DetectorOps.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/pynrc.NIRCam.rst` & `pynrc-1.2.1/docs/api/_autosummary/pynrc.NIRCam.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/pynrc.multiaccum.rst` & `pynrc-1.2.1/docs/api/_autosummary/pynrc.multiaccum.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/pynrc.nb_funcs.rst` & `pynrc-1.2.1/docs/api/_autosummary/pynrc.nb_funcs.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_hci.rst` & `pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_hci.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/pynrc.nrc_utils.rst` & `pynrc-1.2.1/docs/api/_autosummary/pynrc.nrc_utils.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/pynrc.obs_hci.rst` & `pynrc-1.2.1/docs/api/_autosummary/pynrc.obs_hci.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.nircam_cal.rst` & `pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.nircam_cal.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.nircam_dark.rst` & `pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.nircam_dark.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.calib.rst` & `pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.calib.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.ref_pixels.NRC_refs.rst` & `pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.ref_pixels.NRC_refs.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/pynrc.reduce.ref_pixels.rst` & `pynrc-1.2.1/docs/api/_autosummary/pynrc.reduce.ref_pixels.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.AptInput.rst` & `pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.AptInput.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.DMS_input.rst` & `pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.DMS_input.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.ReadAPTXML.rst` & `pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.ReadAPTXML.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.apt.rst` & `pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.apt.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/pynrc.simul.ngNRC.rst` & `pynrc-1.2.1/docs/api/_autosummary/pynrc.simul.ngNRC.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.bandpasses.rst` & `pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.bandpasses.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.coords.jwst_point.rst` & `pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.coords.jwst_point.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.coords.rst` & `pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.coords.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.image_manip.rst` & `pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.image_manip.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.opds.OTE_WFE_Drift_Model.rst` & `pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.opds.OTE_WFE_Drift_Model.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.spectra.planets_sb12.rst` & `pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.spectra.planets_sb12.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.spectra.rst` & `pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.spectra.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.spectra.source_spectrum.rst` & `pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.spectra.source_spectrum.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.webbpsf_ext_core.MIRI_ext.rst` & `pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.webbpsf_ext_core.MIRI_ext.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/api/_autosummary/webbpsf_ext.webbpsf_ext_core.NIRCam_ext.rst` & `pynrc-1.2.1/docs/api/_autosummary/webbpsf_ext.webbpsf_ext_core.NIRCam_ext.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/conf.py` & `pynrc-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/index.rst` & `pynrc-1.2.1/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ===================
 
 pyNRC - Python ETC and Simulator for JWST NIRCam
 ----------------------------------------------------------------------------
 
 pyNRC is a set of Python-based tools for planning observations with JWST NIRCam. It includes an ETC, a simple image slope simulator, and an enhanced data simulator compatible with the JWST pipeline. This package works for a variety of NIRCam observing modes including direct imaging, coronagraphic imaging, slitless grism spectroscopy, and weak lens imaging. All PSFs are generated via `WebbPSF <https://webbpsf.readthedocs.io>`_ and `WebbPSF Extensions <https://github.com/JarronL/webbpsf_ext>`_ to reproduce realistic JWST images and spectra.
 
-Developed by Jarron Leisenring and contributors at University of Arizona (2015 - 2021). 
+Developed by Jarron Leisenring and contributors at University of Arizona (2015 - 2024). 
 
 .. toctree::
    :caption: Getting Started
    :maxdepth: 1
    
    readme.rst
```

### Comparing `pynrc-1.2.0/docs/install_clean.rst` & `pynrc-1.2.1/docs/install_clean.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/installation.rst` & `pynrc-1.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/license.rst` & `pynrc-1.2.1/docs/license.rst`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/make.bat` & `pynrc-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/docs/paper/pandexo_paper/Makefile` & `pynrc-1.2.1/docs/paper/pandexo_paper/Makefile`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/__init__.py` & `pynrc-1.2.1/pynrc/__init__.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/detops.py` & `pynrc-1.2.1/pynrc/detops.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/logging_utils.py` & `pynrc-1.2.1/pynrc/logging_utils.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/maths/_robust.py` & `pynrc-1.2.1/pynrc/maths/_robust.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/maths/coords.py` & `pynrc-1.2.1/pynrc/maths/coords.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/maths/image_manip.py` & `pynrc-1.2.1/pynrc/maths/image_manip.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/nb_funcs.py` & `pynrc-1.2.1/pynrc/nb_funcs.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/nrc_utils.py` & `pynrc-1.2.1/pynrc/nrc_utils.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/obs_nircam.py` & `pynrc-1.2.1/pynrc/obs_nircam.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/opds.py` & `pynrc-1.2.1/pynrc/opds.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/pynrc_core.py` & `pynrc-1.2.1/pynrc/pynrc_core.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/reduce/analysis.py` & `pynrc-1.2.1/pynrc/reduce/analysis.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/reduce/calib.py` & `pynrc-1.2.1/pynrc/reduce/calib.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/reduce/nmf.py` & `pynrc-1.2.1/pynrc/reduce/nmf.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/reduce/pca.py` & `pynrc-1.2.1/pynrc/reduce/pca.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/reduce/ref_pixels.py` & `pynrc-1.2.1/pynrc/reduce/ref_pixels.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/simul/_nghxrg.py` & `pynrc-1.2.1/pynrc/simul/_nghxrg.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/simul/apt.py` & `pynrc-1.2.1/pynrc/simul/apt.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/simul/dms.py` & `pynrc-1.2.1/pynrc/simul/dms.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/simul/ngNRC.py` & `pynrc-1.2.1/pynrc/simul/ngNRC.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/simul/skyvec2ins.py` & `pynrc-1.2.1/pynrc/simul/skyvec2ins.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/speckle_noise.py` & `pynrc-1.2.1/pynrc/speckle_noise.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc/testing.py` & `pynrc-1.2.1/pynrc/testing.py`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/pynrc.egg-info/PKG-INFO` & `pynrc-1.2.1/pynrc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynrc
-Version: 1.2.0
+Version: 1.2.1
 Summary: JWST NIRCam ETC and Simulator
 Home-page: https://pynrc.readthedocs.io
 Author: Jarron Leisenring
 Author-email: jarronl@arizona.edu
 License: MIT license
 Keywords: jwst nircam etc simulator
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,15 +23,19 @@
 
 A JWST NIRCam ETC and Simulator
 ===============================
 
 .. image:: https://img.shields.io/pypi/v/pynrc.svg
         :target: https://pypi.python.org/pypi/pynrc
         :alt: Badge showing current released PyPI version
-
+        
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5829553.svg
+        :target: https://doi.org/10.5281/zenodo.5829553
+        :alt: Zenodo DOI
+   
 .. image:: https://readthedocs.org/projects/pynrc/badge/?version=latest
         :target: https://pynrc.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 *Authors:* `Jarron Leisenring <https://github.com/JarronL>`_ 
 (U. of Arizona, Steward Observatory)
```

### Comparing `pynrc-1.2.0/pynrc.egg-info/SOURCES.txt` & `pynrc-1.2.1/pynrc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynrc-1.2.0/setup.py` & `pynrc-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 install_requires = [
     'tqdm>4',
-    'poppy>=1.2.0',
+    'poppy>=1.1.0',
     'webbpsf>=1.2.0',
     'webbpsf_ext>=1.2.1',
     'astroquery>=0.4.6',
     'jwst',
 ]
 
 setup_requirements = ['pytest-runner', ]
```

### Comparing `pynrc-1.2.0/tests/test_pynrc.py.old` & `pynrc-1.2.1/tests/test_pynrc.py.old`

 * *Files identical despite different names*


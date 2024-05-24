# Comparing `tmp/acoular-24.3.tar.gz` & `tmp/acoular-24.5.tar.gz`

## Comparing `acoular-24.3.tar` & `acoular-24.5.tar`

### file list

```diff
@@ -1,229 +1,51 @@
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 acoular-24.3/.gitlab-ci.yml
--rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 acoular-24.3/.travis.yml
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 acoular-24.3/.zenodo.json
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 acoular-24.3/MANIFEST.in
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 acoular-24.3/build_conda.sh
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 acoular-24.3/noxfile.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 acoular-24.3/.github/workflows/build_docs.yml
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 acoular-24.3/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 acoular-24.3/acoular/__init__.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 acoular-24.3/acoular/calib.py
--rw-r--r--   0        0        0     7221 2020-02-02 00:00:00.000000 acoular-24.3/acoular/configuration.py
--rw-r--r--   0        0        0    22349 2020-02-02 00:00:00.000000 acoular-24.3/acoular/environments.py
--rw-r--r--   0        0        0    38191 2020-02-02 00:00:00.000000 acoular-24.3/acoular/fastFuncs.py
--rw-r--r--   0        0        0   117815 2020-02-02 00:00:00.000000 acoular-24.3/acoular/fbeamform.py
--rw-r--r--   0        0        0    13285 2020-02-02 00:00:00.000000 acoular-24.3/acoular/fileimport.py
--rw-r--r--   0        0        0    41908 2020-02-02 00:00:00.000000 acoular-24.3/acoular/grids.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 acoular-24.3/acoular/h5cache.py
--rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 acoular-24.3/acoular/h5files.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 acoular-24.3/acoular/internal.py
--rw-r--r--   0        0        0     4684 2020-02-02 00:00:00.000000 acoular-24.3/acoular/microphones.py
--rw-r--r--   0        0        0    10702 2020-02-02 00:00:00.000000 acoular-24.3/acoular/nidaqimport.py
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 acoular-24.3/acoular/sdinput.py
--rw-r--r--   0        0        0    11865 2020-02-02 00:00:00.000000 acoular-24.3/acoular/signals.py
--rw-r--r--   0        0        0    51086 2020-02-02 00:00:00.000000 acoular-24.3/acoular/sources.py
--rw-r--r--   0        0        0    28975 2020-02-02 00:00:00.000000 acoular-24.3/acoular/spectra.py
--rw-r--r--   0        0        0    31193 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tbeamform.py
--rw-r--r--   0        0        0     7383 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tfastfuncs.py
--rwxr-xr-x   0        0        0    14934 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tools.py
--rw-r--r--   0        0        0    91140 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tprocess.py
--rw-r--r--   0        0        0    17655 2020-02-02 00:00:00.000000 acoular-24.3/acoular/traitsviews.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 acoular-24.3/acoular/trajectory.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 acoular-24.3/acoular/version.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 acoular-24.3/acoular/demo/__init__.py
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 acoular-24.3/acoular/demo/acoular_demo.py
--rwxr-xr-x   0        0        0      288 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/run_tests.sh
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/run_tests_osx.sh
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/test.npy
--rw-r--r--   0        0        0    10612 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/test_beamformer_results.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/test_classes.py
--rw-r--r--   0        0        0     8645 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/test_digest.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/test_environments.py
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/test_example1.py
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/test_grid.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/test_integrate.py
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/test_signals.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/test_sources.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/test_spectra.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/test_timecache.py
--rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/test_tprocess.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/test_traj_beamformer_results.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerBase.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerBaseFalse1.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerBaseFalse2.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerBaseFalse3.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerBaseFalse4.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerBaseTrue1.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerBaseTrue2.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerBaseTrue3.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerBaseTrue4.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerCMFLassoLarsBIC.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerCMFNNLS.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerCapon.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerClean.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerCleansc.npy
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerCleant.npy
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerCleantSq.npy
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerCleantSqTraj.npy
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerCleantTraj.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerDamas.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerDamasPlus.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerEig.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerEigFalse1.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerEigFalse2.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerEigFalse3.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerEigFalse4.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerEigTrue1.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerEigTrue2.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerEigTrue3.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerEigTrue4.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerFunctional.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerGIB.npy
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerGridlessOrth.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerMusic.npy
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerOrth.npy
--rw-r--r--   0        0        0    73136 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerSODIX.npy
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerTime.npy
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerTimeSq.npy
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerTimeSqTraj.npy
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/BeamformerTimeTraj.npy
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/Environment.npy
--rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/Example1_numerical_values_testsum.h5
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/FiltFiltOctave__.npy
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/FiltFiltOctave_band_100_0_fraction_Thirdoctave_.npy
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/FiltFreqWeight_weight_A_.npy
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/FiltFreqWeight_weight_C_.npy
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/FiltFreqWeight_weight_Z_.npy
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/FiltOctave__.npy
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/FiltOctave_band_100_0_fraction_Thirdoctave_.npy
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/Filter__.npy
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/GeneralFlowEnvironment.npy
--rw-r--r--   0        0        0    15808 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/OctaveFilterBank__.npy
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/OpenJet.npy
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/PointSource.npy
--rw-r--r--   0        0        0    46784 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/PowerSpectra_csm.npy
--rw-r--r--   0        0        0    46784 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/PowerSpectra_ev.npy
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/RotatingFlow.npy
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/SlotJet.npy
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/TimeAverage__.npy
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/TimeCumAverage__.npy
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/TimeExpAverage_weight_F_.npy
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/TimeExpAverage_weight_I_.npy
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/TimeExpAverage_weight_S_.npy
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/TimeInOut__.npy
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/TimePower__.npy
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/TimeReverse__.npy
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/UniformFlowEnvironment.npy
--rw-r--r--   0        0        0    69960 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/reference_data/beamformer_traj_time_data.h5
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/unsupported/functionalBeamformer.py
--rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/unsupported/precisionTest.py
--rw-r--r--   0        0        0    13815 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/unsupported/validationOfBeamformerFuncsPOSTAcoularIntegration.py
--rw-r--r--   0        0        0    31698 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/unsupported/validationOfBeamformerFuncsPREeAcoularIntegration.py
--rw-r--r--   0        0        0   131252 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/unsupported/SpeedComparison/OvernightTestcasesBeamformer_nMics32_nGridPoints100_nFreqs4_nTrials10.png
--rw-r--r--   0        0        0    10727 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/unsupported/SpeedComparison/cythonBeamformer.pyx
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/unsupported/SpeedComparison/mainForCython.py
--rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/unsupported/SpeedComparison/mainForParallelJit.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/unsupported/SpeedComparison/setupCythonOpenMP.py
--rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/unsupported/SpeedComparison/sharedFunctions.py
--rw-r--r--   0        0        0   172747 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/unsupported/SpeedComparison/timeOverNMics_AllImportantMethods.png
--rw-r--r--   0        0        0   131665 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/unsupported/SpeedComparison/timeOverNMics_faverage.png
--rw-r--r--   0        0        0    10020 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/unsupported/SpeedComparison/vglOptimierungFAverage.py
--rw-r--r--   0        0        0     9712 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/unsupported/SpeedComparison/vglOptimierungGaussSeidel.py
--rwxr-xr-x   0        0        0    40111 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/unsupported/SpeedComparison/vglOptimierungR_BEAMFULL_INVERSE.py
--rw-r--r--   0        0        0    13445 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/unsupported/SpeedComparison/vglOptimierungR_BEAM_OS.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 acoular-24.3/acoular/tests/unsupported/SpeedComparison/whatsFastestWayFor_absASquared.py
--rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 acoular-24.3/acoular/xml/HW90D240_f10.xml
--rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 acoular-24.3/acoular/xml/W90_D105_f10.xml
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 acoular-24.3/acoular/xml/acousticam_2c.xml
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 acoular-24.3/acoular/xml/acousticam_4c.xml
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 acoular-24.3/acoular/xml/array38.xml
--rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 acoular-24.3/acoular/xml/array92x.xml
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 acoular-24.3/acoular/xml/array_56.xml
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 acoular-24.3/acoular/xml/array_56_10_9.xml
--rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 acoular-24.3/acoular/xml/array_56_bomb.xml
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 acoular-24.3/acoular/xml/array_56_v2.xml
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 acoular-24.3/acoular/xml/array_64.xml
--rw-r--r--   0        0        0     6558 2020-02-02 00:00:00.000000 acoular-24.3/acoular/xml/array_84_10_9.xml
--rw-r--r--   0        0        0     6248 2020-02-02 00:00:00.000000 acoular-24.3/acoular/xml/array_84_bomb_v3.xml
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 acoular-24.3/acoular/xml/calib_vw_ring32.xml
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 acoular-24.3/acoular/xml/gfai_ring32.xml
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 acoular-24.3/acoular/xml/minidsp_uma16.xml
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 acoular-24.3/acoular/xml/tub_vogel64.xml
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 acoular-24.3/docs/Makefile
--rw-r--r--   0        0        0     7524 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/conf.py
--rw-r--r--   0        0        0    39963 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/gen_rst.py
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/index.rst
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/requirements.txt
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/_static/Acoular_logo.png
--rw-r--r--   0        0        0   248866 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/_static/Airfoil_selfnoise_3d.png
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/_static/acoular_logo.ico
--rw-r--r--   0        0        0    37466 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/_static/airfoil_leading_edge_noise.png
--rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/_static/no_image.png
--rw-r--r--   0        0        0    60494 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/_static/pantograph_noise_3d.png
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/_themes/haikuac/layout.html
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/_themes/haikuac/theme.conf
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/_themes/haikuac/static/alert_info_32.png
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/_themes/haikuac/static/alert_warning_32.png
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/_themes/haikuac/static/bg-page.png
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/_themes/haikuac/static/bullet_orange.png
--rw-r--r--   0        0        0     8867 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/_themes/haikuac/static/haikuac.css_t
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/api_ref/index.rst
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/examples/example_3D_beamforming.rst
--rw-r--r--   0        0        0    78071 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/examples/example_3D_beamforming_1.png
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/examples/example_airfoil_in_open_jet_beamforming.rst
--rw-r--r--   0        0        0    61537 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/examples/example_airfoil_in_open_jet_beamforming_1.png
--rw-r--r--   0        0        0    45784 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/examples/example_airfoil_in_open_jet_beamforming_2.png
--rw-r--r--   0        0        0    46411 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/examples/example_airfoil_in_open_jet_beamforming_3.png
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/examples/example_airfoil_in_open_jet_cmf.rst
--rw-r--r--   0        0        0    36576 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/examples/example_airfoil_in_open_jet_cmf_1.png
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/examples/example_airfoil_in_open_jet_steering_vectors.rst
--rw-r--r--   0        0        0    54480 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/examples/example_airfoil_in_open_jet_steering_vectors_1.png
--rw-r--r--   0        0        0    61898 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/examples/example_airfoil_in_open_jet_steering_vectors_2.png
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/examples/example_rotating_point_source.rst
--rw-r--r--   0        0        0    65341 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/examples/example_rotating_point_source_1.png
--rw-r--r--   0        0        0    57493 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/examples/example_rotating_point_source_2.png
--rw-r--r--   0        0        0    31515 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/examples/example_rotating_point_source_3.png
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/examples/index.rst
--rw-r--r--   0        0        0    21039 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/get_started/array64.png
--rw-r--r--   0        0        0    15250 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/get_started/array64_py3colormap.png
--rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/get_started/index.rst
--rw-r--r--   0        0        0    64624 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/get_started/map_three_sources.png
--rw-r--r--   0        0        0    34929 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/get_started/three_source_py3_colormap.png
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/install/index.rst
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/literature/index.rst
--rw-r--r--   0        0        0    11094 2020-02-02 00:00:00.000000 acoular-24.3/docs/source/news/index.rst
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 acoular-24.3/examples/README.txt
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 acoular-24.3/examples/acoular_demo.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 acoular-24.3/examples/basic_beamformer_example.py
--rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 acoular-24.3/examples/example_3D_beamforming.py
--rwxr-xr-x   0        0        0      459 2020-02-02 00:00:00.000000 acoular-24.3/examples/example_GenericSignal.py
--rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 acoular-24.3/examples/example_SampleSplitter_bufferhandling.py
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 acoular-24.3/examples/example_SampleSplitter_multithreading.py
--rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 acoular-24.3/examples/example_airfoil_in_open_jet_beamforming.py
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 acoular-24.3/examples/example_airfoil_in_open_jet_cmf.py
--rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 acoular-24.3/examples/example_airfoil_in_open_jet_steering_vectors.py
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 acoular-24.3/examples/example_airfoil_in_open_jet_time_beamforming.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 acoular-24.3/examples/example_calib.xml
--rw-r--r--   0        0        0  5807392 2020-02-02 00:00:00.000000 acoular-24.3/examples/example_data.h5
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 acoular-24.3/examples/example_evaluate.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 acoular-24.3/examples/example_filter.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 acoular-24.3/examples/example_power_spectra_import.py
--rw-r--r--   0        0        0     8778 2020-02-02 00:00:00.000000 acoular-24.3/examples/example_rotating_point_source.py
--rwxr-xr-x   0        0        0     4507 2020-02-02 00:00:00.000000 acoular-24.3/examples/example_sectors_and_intergration.py
--rwxr-xr-x   0        0        0     1926 2020-02-02 00:00:00.000000 acoular-24.3/examples/example_tools.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 acoular-24.3/examples/three_sources.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 acoular-24.3/examples/benchmark/run_benchmarks.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 acoular-24.3/examples/benchmark/test_beamformerfreq.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 acoular-24.3/examples/benchmark/test_delayandsum.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 acoular-24.3/examples/benchmark/test_dist_mat.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 acoular-24.3/recipe.local/meta.yaml
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 acoular-24.3/recipe.local/run_test.sh
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 acoular-24.3/scripts/plot_examples.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 acoular-24.3/.gitignore
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 acoular-24.3/AUTHORS.rst
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 acoular-24.3/LICENSE
--rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 acoular-24.3/README.md
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 acoular-24.3/pyproject.toml
--rw-r--r--   0        0        0     9964 2020-02-02 00:00:00.000000 acoular-24.3/PKG-INFO
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 acoular-24.5/acoular/__init__.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 acoular-24.5/acoular/calib.py
+-rw-r--r--   0        0        0     8352 2020-02-02 00:00:00.000000 acoular-24.5/acoular/configuration.py
+-rw-r--r--   0        0        0    22271 2020-02-02 00:00:00.000000 acoular-24.5/acoular/environments.py
+-rw-r--r--   0        0        0    38794 2020-02-02 00:00:00.000000 acoular-24.5/acoular/fastFuncs.py
+-rw-r--r--   0        0        0   113833 2020-02-02 00:00:00.000000 acoular-24.5/acoular/fbeamform.py
+-rw-r--r--   0        0        0    40017 2020-02-02 00:00:00.000000 acoular-24.5/acoular/grids.py
+-rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 acoular-24.5/acoular/h5cache.py
+-rw-r--r--   0        0        0     7593 2020-02-02 00:00:00.000000 acoular-24.5/acoular/h5files.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 acoular-24.5/acoular/internal.py
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 acoular-24.5/acoular/microphones.py
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 acoular-24.5/acoular/sdinput.py
+-rw-r--r--   0        0        0    11351 2020-02-02 00:00:00.000000 acoular-24.5/acoular/signals.py
+-rw-r--r--   0        0        0    52776 2020-02-02 00:00:00.000000 acoular-24.5/acoular/sources.py
+-rw-r--r--   0        0        0    28069 2020-02-02 00:00:00.000000 acoular-24.5/acoular/spectra.py
+-rw-r--r--   0        0        0    30274 2020-02-02 00:00:00.000000 acoular-24.5/acoular/tbeamform.py
+-rw-r--r--   0        0        0     7883 2020-02-02 00:00:00.000000 acoular-24.5/acoular/tfastfuncs.py
+-rw-r--r--   0        0        0    88682 2020-02-02 00:00:00.000000 acoular-24.5/acoular/tprocess.py
+-rw-r--r--   0        0        0    13741 2020-02-02 00:00:00.000000 acoular-24.5/acoular/traitsviews.py
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 acoular-24.5/acoular/trajectory.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 acoular-24.5/acoular/version.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 acoular-24.5/acoular/demo/__init__.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 acoular-24.5/acoular/demo/acoular_demo.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 acoular-24.5/acoular/tools/__init__.py
+-rw-r--r--   0        0        0     6409 2020-02-02 00:00:00.000000 acoular-24.5/acoular/tools/aiaa.py
+-rw-r--r--   0        0        0     6292 2020-02-02 00:00:00.000000 acoular-24.5/acoular/tools/helpers.py
+-rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 acoular-24.5/acoular/tools/metrics.py
+-rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 acoular-24.5/acoular/xml/HW90D240_f10.xml
+-rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 acoular-24.5/acoular/xml/W90_D105_f10.xml
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 acoular-24.5/acoular/xml/acousticam_2c.xml
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 acoular-24.5/acoular/xml/acousticam_4c.xml
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 acoular-24.5/acoular/xml/array38.xml
+-rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 acoular-24.5/acoular/xml/array92x.xml
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 acoular-24.5/acoular/xml/array_56.xml
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 acoular-24.5/acoular/xml/array_56_10_9.xml
+-rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 acoular-24.5/acoular/xml/array_56_bomb.xml
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 acoular-24.5/acoular/xml/array_56_v2.xml
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 acoular-24.5/acoular/xml/array_64.xml
+-rw-r--r--   0        0        0     6558 2020-02-02 00:00:00.000000 acoular-24.5/acoular/xml/array_84_10_9.xml
+-rw-r--r--   0        0        0     6248 2020-02-02 00:00:00.000000 acoular-24.5/acoular/xml/array_84_bomb_v3.xml
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 acoular-24.5/acoular/xml/calib_vw_ring32.xml
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 acoular-24.5/acoular/xml/gfai_ring32.xml
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 acoular-24.5/acoular/xml/minidsp_uma-16.xml
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 acoular-24.5/acoular/xml/minidsp_uma-16_mirrored.xml
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 acoular-24.5/acoular/xml/tub_vogel64.xml
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 acoular-24.5/.gitignore
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 acoular-24.5/AUTHORS.rst
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 acoular-24.5/LICENSE
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 acoular-24.5/README.md
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 acoular-24.5/pyproject.toml
+-rw-r--r--   0        0        0    10258 2020-02-02 00:00:00.000000 acoular-24.5/PKG-INFO
```

### Comparing `acoular-24.3/acoular/configuration.py` & `acoular-24.5/acoular/configuration.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,195 +1,238 @@
-# -*- coding: utf-8 -*-
-#pylint: disable-msg=E0611, E1101, C0103, R0901, R0902, R0903, R0904, W0232
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 # Copyright (c) Acoular Development Team.
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 """Implements global configuration of Acoular.
 
 .. autosummary::
     :toctree: generated/
 
     Config
     config
 """
 
-from os import path, mkdir, environ
+import importlib.util
+import sys
+from os import environ, mkdir, path
 from warnings import warn
-import sys 
 
 # When numpy is using OpenBLAS then it runs with OPENBLAS_NUM_THREADS which may lead to
 # overcommittment when called from within numba jitted function that run on
 # NUMBA_NUM_THREADS. If overcommitted, things get extremely! slow. Therefore we make an
 # attempt to avoid this situation. The main problem is that OPENBLAS_NUM_THREADS is
 # only respected once numpy starts. Later on, it cannot be changed.
 
 # we check if numpy already loaded
-if 'numpy' in sys.modules: 
-    # numpy is loaded 
+if 'numpy' in sys.modules:
+    # numpy is loaded
     # temporarily route stdout to string
     import io
-    import numpy 
+
+    import numpy as np
+
     orig_stdout = sys.stdout
     temp_stdout = io.StringIO()
     sys.stdout = temp_stdout
-    numpy.show_config()
+    np.show_config()
     sys.stdout = orig_stdout
     # check if it uses OpenBLAS or another library
     if 'openblas' in temp_stdout.getvalue().lower():
         # it's OpenBLAS, set numba threads=1 to avoid overcommittment
         import numba
+
         numba.set_num_threads(1)
-        warn("We detected that Numpy is already loaded and uses OpenBLAS. Because "
-             "this conflicts with Numba parallel execution, we disable parallel "
-             "execution for now and processing might be slower. To speed up, "
-             "either import Numpy after Acoular or set environment variable "
-             "OPENBLAS_NUM_THREADS=1 before start of the program.",
-             UserWarning, stacklevel = 2)
+        warn(
+            'We detected that Numpy is already loaded and uses OpenBLAS. Because '
+            'this conflicts with Numba parallel execution, we disable parallel '
+            'execution for now and processing might be slower. To speed up, '
+            'either import Numpy after Acoular or set environment variable '
+            'OPENBLAS_NUM_THREADS=1 before start of the program.',
+            UserWarning,
+            stacklevel=2,
+        )
 else:
     # numpy is not loaded
-    environ['OPENBLAS_NUM_THREADS'] = "1"
+    environ['OPENBLAS_NUM_THREADS'] = '1'
 
 # this loads numpy, so we have to defer loading until OpenBLAS check is done
-from traits.api import Trait, Bool, Str, Property, HasStrictTraits
+from traits.api import Bool, Either, HasStrictTraits, Property, Str, Trait, cached_property
+
 
 class Config(HasStrictTraits):
-    """
-    This class implements the global configuration of the Acoular package.
+    """Implements the global configuration of the Acoular package.
 
-    An instance of this class can be accessed for adjustment of the following 
+    An instance of this class can be accessed for adjustment of the following
     properties.
     General caching behaviour can be controlled by :attr:`global_caching`.
-    The package used to read and write .h5 files can be specified 
-    by :attr:`h5library`.    
+    The package used to read and write .h5 files can be specified
+    by :attr:`h5library`.
 
-    Example: 
+    Example:
+    --------
         For using Acoular with h5py package and overwrite existing cache:
-        
+
         >>>    import acoular
         >>>    acoular.config.h5library = "h5py"
         >>>    acoular.config.global_caching = "overwrite"
+
     """
-    
+
     def __init__(self):
         HasStrictTraits.__init__(self)
         self._assert_h5library()
-    
+
     #: Flag that globally defines caching behaviour of Acoular classes
     #: defaults to 'individual'.
     #:
     #: * 'individual': Acoular classes handle caching behavior individually.
     #: * 'all': Acoular classes cache everything and read from cache if possible.
     #: * 'none': Acoular classes do not cache results. Cachefiles are not created.
     #: * 'readonly': Acoular classes do not actively cache, but read from cache if existing.
     #: * 'overwrite': Acoular classes replace existing cachefile content with new data.
     global_caching = Property()
-    
-    _global_caching = Trait('individual','all','none','readonly','overwrite') 
 
-    #: Flag that globally defines package used to read and write .h5 files 
-    #: defaults to 'pytables'. If 'pytables' can not be imported, 'h5py' is used
+    _global_caching = Trait('individual', 'all', 'none', 'readonly', 'overwrite')
+
+    #: Flag that globally defines package used to read and write .h5 files
+    #: defaults to 'pytables'. It is also possible to set it to 'tables', which is an alias for 'pytables'.
+    #: If 'pytables' can not be imported, 'h5py' is used.
     h5library = Property()
-    
-    _h5library = Trait('pytables','h5py')
-    
+
+    _h5library = Either('pytables', 'tables', 'h5py', default='pytables')
+
     #: Defines the path to the directory containing Acoulars cache files.
     #: If the specified :attr:`cache_dir` directory does not exist,
-    #: it will be created. attr:`cache_dir` defaults to current session path.  
+    #: it will be created. :attr:`cache_dir` defaults to current session path.
     cache_dir = Property()
 
-    _cache_dir = Str("")
+    _cache_dir = Str('')
 
-    #: Defines the working directory containing files that can be loaded by the
-    #: fileimport.py module. 
-    #: Defaults to current session path.  
+    #: Defines the working directory containing data files. Used only by
+    #: :class:`~acoular.tprocess.WriteH5` class.
+    #: Defaults to current session path.
     td_dir = Property()
 
     _td_dir = Str(path.curdir)
 
     #: Boolean Flag that determines whether user has access to traitsui features.
     #: Defaults to False.
     use_traitsui = Property()
-    
+
     _use_traitsui = Bool(False)
-    
-    
+
+    #: Boolean Flag that determines whether tables is installed.
+    have_tables = Property()
+
+    #: Boolean Flag that determines whether h5py is installed.
+    have_h5py = Property()
+
+    #: Boolean Flag that determines whether matplotlib is installed.
+    have_matplotlib = Property()
+
+    #: Boolean Flag that determines whether pylops is installed.
+    have_pylops = Property()
+
+    #: Boolean Flag that determines whether sounddevice is installed.
+    have_sounddevice = Property()
+
     def _get_global_caching(self):
         return self._global_caching
 
-    def _set_global_caching(self,globalCachingValue):
+    def _set_global_caching(self, globalCachingValue):
         self._global_caching = globalCachingValue
-        
+
     def _get_h5library(self):
         return self._h5library
-    
-    def _set_h5library(self,libraryName):
-        self._h5library = libraryName 
-    
+
+    def _set_h5library(self, libraryName):
+        self._h5library = libraryName
+
     def _get_use_traitsui(self):
         return self._use_traitsui
-    
+
     def _set_use_traitsui(self, use_tui):
         if use_tui:
-            from  . import traitsviews
+            from . import traitsviews
             # If user tries to use traitsuis and it's not installed, this will throw an error.
-        self._use_traitsui = use_tui 
-    
+        self._use_traitsui = use_tui
+
     def _assert_h5library(self):
-        try:
-            import tables  
-            self.h5library = 'pytables'
-        except:
-            try:
-                import h5py
-                self.h5library = 'h5py'
-            except:
-                raise ImportError("packages h5py and pytables are missing!")
+        if not self.have_tables and not self.have_h5py:
+            msg = 'Packages H5py and PyTables are missing! At least one of them is required for Acoular to work.'
+            raise ImportError(msg)
+        if not self.have_tables:
+            self.h5library = 'h5py'
 
     def _get_cache_dir(self):
-        if self._cache_dir == "":
-            cache_dir = path.join(path.curdir,'cache')
+        if self._cache_dir == '':
+            cache_dir = path.join(path.curdir, 'cache')
             if not path.exists(cache_dir):
                 mkdir(cache_dir)
             self._cache_dir = cache_dir
         return self._cache_dir
-    
-    def _set_cache_dir(self,cdir):
+
+    def _set_cache_dir(self, cdir):
         if not path.exists(cdir):
             mkdir(cdir)
         self._cache_dir = cdir
 
     def _get_td_dir(self):
         return self._td_dir
-    
-    def _set_td_dir(self,tddir):
+
+    def _set_td_dir(self, tddir):
         self._td_dir = tddir
 
+    def _have_module(self, module_name):
+        spec = importlib.util.find_spec(module_name)
+        return spec is not None
+
+    @cached_property
+    def _get_have_matplotlib(self):
+        return self._have_module('matplotlib')
+
+    @cached_property
+    def _get_have_pylops(self):
+        return self._have_module('pylops')
+
+    @cached_property
+    def _get_have_sounddevice(self):
+        return self._have_module('sounddevice')
+
+    @cached_property
+    def _get_have_tables(self):
+        return self._have_module('tables')
+
+    @cached_property
+    def _get_have_h5py(self):
+        return self._have_module('h5py')
+
+
 config = Config()
 """
 This instance implements the global configuration of the Acoular package.
 
 General caching behaviour can be controlled by the :attr:`global_caching` attribute:
 * 'individual': Acoular classes handle caching behavior individually.
 * 'all': Acoular classes cache everything and read from cache if possible.
 * 'none': Acoular classes do not cache results. Cachefiles are not created.
 * 'readonly': Acoular classes do not actively cache, but read from cache if existing.
 * 'overwrite': Acoular classes replace existing cachefile content with new data.
 
-The package used to read and write .h5 files can be specified 
-by :attr:`h5library`:  
-* 'pytables': Use 'tables' (or 'pytables', depending on python distribution).
-* 'h5py': Use 'h5py'.
+The package used to read and write .h5 files can be specified
+by :attr:`h5library`:
+* 'PyTables': Use 'tables' (or 'pytables', depending on python distribution).
+* 'H5py': Use 'h5py'.
 
 Some Acoular classes support GUI elements for usage with tools from the TraitsUI package.
 If desired, this package has to be installed manually, as it is not a prerequisite for
 installing Acoular.
 To enable the functionality, the flag attribute :attr:`use_traitsui` has to be set to True (default: False).
 Note: this is independent from the GUI tools implemented in the spectAcoular package.
 
 
-Example: 
+Example:
     For using Acoular with h5py package and overwrite existing cache:
-    
+
     >>>    import acoular
     >>>    acoular.config.h5library = "h5py"
     >>>    acoular.config.global_caching = "overwrite"
 """
```

### Comparing `acoular-24.3/acoular/environments.py` & `acoular-24.5/acoular/environments.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,208 +1,228 @@
-# -*- coding: utf-8 -*-
-#pylint: disable-msg=E0611, E1103, C0103, R0901, R0902, R0903, R0904, W0232
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 # Copyright (c) Acoular Development Team.
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 """Implements acoustic environments with and without flow.
 
 .. autosummary::
     :toctree: generated/
 
     Environment
     UniformFlowEnvironment
     GeneralFlowEnvironment
     FlowField
     OpenJet
     RotatingFlow
     SlotJet
 
 """
+
 import numba as nb
-from numpy import array, isscalar, float32, float64, newaxis, \
-sqrt, arange, pi, exp, sin, cos, arccos, zeros_like, empty, dot, hstack, \
-vstack, identity, cross, sign, arctan2, matmul, sum, ascontiguousarray
+from numpy import (
+    arange,
+    arccos,
+    arctan2,
+    array,
+    ascontiguousarray,
+    cos,
+    cross,
+    dot,
+    empty,
+    exp,
+    float32,
+    float64,
+    hstack,
+    identity,
+    isscalar,
+    matmul,
+    newaxis,
+    pi,
+    sign,
+    sin,
+    sqrt,
+    sum,
+    vstack,
+    zeros_like,
+)
 from numpy.linalg.linalg import norm
 from scipy.integrate import ode
 from scipy.interpolate import LinearNDInterpolator
 from scipy.spatial import ConvexHull
-from traits.api import HasPrivateTraits, Float, Property, Int, \
-CArray, cached_property, Trait, Dict
+from traits.api import CArray, Dict, Float, HasPrivateTraits, Int, Property, Trait, cached_property
 
 from .internal import digest
 
-f64ro = nb.types.Array(nb.types.float64,2,'C',readonly=True)
-f32ro = nb.types.Array(nb.types.float32,2,'C',readonly=True)
+f64ro = nb.types.Array(nb.types.float64, 2, 'C', readonly=True)
+f32ro = nb.types.Array(nb.types.float32, 2, 'C', readonly=True)
+
 
-@nb.njit([(f64ro, f64ro), (f64ro, f32ro), (f32ro, f64ro),(f32ro, f32ro)],
-                cache=True, fastmath=True)
-def dist_mat(gpos,mpos):
-    """computes distance matrix, accelerated with numba
+@nb.njit([(f64ro, f64ro), (f64ro, f32ro), (f32ro, f64ro), (f32ro, f32ro)], cache=True, fastmath=True)
+def dist_mat(gpos, mpos):
+    """Computes distance matrix, accelerated with numba.
 
     Args:
+    ----
         gpos (3,N)
         mpos (3,M)
 
-    Returns:
+    Returns
+    -------
         (N,M) distance matrix
-    """    
-    _,M = mpos.shape
-    _,N = gpos.shape
-    rm = empty((N,M),dtype=gpos.dtype)
-    TWO = rm.dtype.type(2.0) # make sure to have a float32 or float 64 literal
+
+    """
+    _, M = mpos.shape
+    _, N = gpos.shape
+    rm = empty((N, M), dtype=gpos.dtype)
+    TWO = rm.dtype.type(2.0)  # make sure to have a float32 or float 64 literal
     m0 = mpos[0]
     m1 = mpos[1]
     m2 = mpos[2]
     for n in range(N):
-        g0 = gpos[0,n]
-        g1 = gpos[1,n]
-        g2 = gpos[2,n]
+        g0 = gpos[0, n]
+        g1 = gpos[1, n]
+        g2 = gpos[2, n]
         for m in range(M):
-            rm[n,m] = sqrt((g0 - m0[m])**TWO + (g1 - m1[m])**TWO + (g2 - m2[m])**TWO)
+            rm[n, m] = sqrt((g0 - m0[m]) ** TWO + (g1 - m1[m]) ** TWO + (g2 - m2[m]) ** TWO)
     return rm
 
 
-def cartToCyl(x, Q=identity(3)):
-    """
-    Returns the cylindrical coordinate representation of a input position 
+def cartToCyl(x, Q=None):
+    """Returns the cylindrical coordinate representation of a input position
     which was before transformed into a modified cartesian coordinate, which
     has flow into positive z direction.
-    
+
     Parameters
     ----------
     x : float[3, nPoints]
         cartesian coordinates of n points
     Q : float[3,3]
         Orthogonal transformation matrix. If provided, the pos vectors are
         transformed via posiMod = Q * x, before transforming those modified
         coordinates into cylindrical ones. Default is identity matrix.
-        
+
     Returns
     -------
     cylCoord : [3, nPoints]
         cylindrical representation of those n points with (phi, r, z)
+
     """
-    if not (Q == identity(3)).all():
+    Q = identity(3) if Q is None else Q
+    if not (Q == identity(3)).all():  # noqa: SIM300
         x = matmul(Q, x)  # modified position vector
-    cylCoord = array([arctan2(x[1], x[0]), sqrt(x[0]**2 + x[1]**2), x[2]])
-    return cylCoord
+    return array([arctan2(x[1], x[0]), sqrt(x[0] ** 2 + x[1] ** 2), x[2]])
 
 
-def cylToCart(x, Q=identity(3)):
-        """
-        Returns the cartesian coordinate representation of a input position 
-        which was before transformed into a cylindrical coordinate, which
-        has flow into positive z direction.
-        
-        Parameters
-        ----------
-        x : float[3, nPoints]
-            cylindrical representation of those n points with (phi, r, z)
-            cartesian coordinates of n points
-    
-        Q : float[3,3]
-        Orthogonal transformation matrix. If provided, the pos vectors are
-        transformed via posiMod = Q * x, before transforming those modified
-        coordinates into cylindrical ones. Default is identity matrix.
-        
-            
-        Returns
-        -------
-        CartCoord : [3, nPoints]
+def cylToCart(x, Q=None):
+    """Returns the cartesian coordinate representation of a input position
+    which was before transformed into a cylindrical coordinate, which
+    has flow into positive z direction.
+
+    Parameters
+    ----------
+    x : float[3, nPoints]
+        cylindrical representation of those n points with (phi, r, z)
         cartesian coordinates of n points
-            
-        """
-        if not (Q == identity(3)).all():
-            x = matmul(Q, x)  # modified position vector
-        CartCoord = array([x[1]*sin(x[0]),x[1]*cos(x[0]) , x[2]])
-        return CartCoord
+
+    Q : float[3,3]
+    Orthogonal transformation matrix. If provided, the pos vectors are
+    transformed via posiMod = Q * x, before transforming those modified
+    coordinates into cylindrical ones. Default is identity matrix.
 
 
-class Environment( HasPrivateTraits ):
+    Returns
+    -------
+    CartCoord : [3, nPoints]
+    cartesian coordinates of n points
+
     """
-    A simple acoustic environment without flow.
+    Q = identity(3) if Q is None else Q
+    if not (Q == identity(3)).all():  # noqa: SIM300
+        x = matmul(Q, x)  # modified position vector
+    return array([x[1] * sin(x[0]), x[1] * cos(x[0]), x[2]])
+
+
+class Environment(HasPrivateTraits):
+    """A simple acoustic environment without flow.
 
     This class provides the facilities to calculate the travel time (distances)
     between grid point locations and microphone locations.
     """
+
     # internal identifier
     digest = Property(
-        depends_on=['c'], 
-        )
+        depends_on=['c'],
+    )
 
     #: The speed of sound, defaults to 343 m/s
-    c = Float(343., 
-        desc="speed of sound")
+    c = Float(343.0, desc='speed of sound')
 
     #: The region of interest (ROI), not needed for most types of environment
-    roi = Trait(None,(None,CArray))
+    roi = Trait(None, (None, CArray))
 
-    def _get_digest( self ):
-        return digest( self )
+    def _get_digest(self):
+        return digest(self)
 
-    def _r( self, gpos, mpos=0.0):
-        """
-        Calculates distances between grid point locations and microphone
+    def _r(self, gpos, mpos=0.0):
+        """Calculates distances between grid point locations and microphone
         locations or the origin. Functionality may change in the future.
 
         Parameters
         ----------
         gpos : array of floats of shape (3, N)
             The locations of points in the beamforming map grid in 3D cartesian
-            co-ordinates. 
+            co-ordinates.
         mpos : array of floats of shape (3, M), optional
             The locations of microphones in 3D cartesian co-ordinates. If not
             given, then only one microphone at the origin (0, 0, 0) is
             considered.
 
         Returns
         -------
         r : array of floats
-            The distances in a twodimensional (N, M) array of floats. If M==1, 
+            The distances in a twodimensional (N, M) array of floats. If M==1,
             then only a one-dimensional array is returned.
+
         """
         if isscalar(mpos):
-            mpos = array((0, 0, 0), dtype = float64)[:, newaxis]
-        rm = dist_mat(ascontiguousarray(gpos),ascontiguousarray(mpos))
-#        mpos = mpos[:, newaxis, :]
-#        rmv = gpos[:, :, newaxis]-mpos
-#        rm = sum(rmv*rmv, 0)**0.5
+            mpos = array((0, 0, 0), dtype=float64)[:, newaxis]
+        rm = dist_mat(ascontiguousarray(gpos), ascontiguousarray(mpos))
+        #        mpos = mpos[:, newaxis, :]
+        #        rmv = gpos[:, :, newaxis]-mpos
+        #        rm = sum(rmv*rmv, 0)**0.5
         if rm.shape[1] == 1:
             rm = rm[:, 0]
         return rm
 
-class UniformFlowEnvironment( Environment):
-    """
-    An acoustic environment with uniform flow.
+
+class UniformFlowEnvironment(Environment):
+    """An acoustic environment with uniform flow.
 
     This class provides the facilities to calculate the travel time (distances)
     between grid point locations and microphone locations in a uniform flow
     field.
     """
+
     #: The Mach number, defaults to 0.
-    ma = Float(0.0, 
-        desc="flow mach number")
+    ma = Float(0.0, desc='flow mach number')
 
     #: The unit vector that gives the direction of the flow, defaults to
     #: flow in x-direction.
-    fdv = CArray( dtype=float64, shape=(3, ), value=array((1.0, 0, 0)), 
-        desc="flow direction")
+    fdv = CArray(dtype=float64, shape=(3,), value=array((1.0, 0, 0)), desc='flow direction')
 
     # internal identifier
     digest = Property(
-        depends_on=['c', 'ma', 'fdv'], 
-        )
+        depends_on=['c', 'ma', 'fdv'],
+    )
 
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
+    def _get_digest(self):
+        return digest(self)
 
-    def _r( self, gpos, mpos=0.0):
-        """
-        Calculates the virtual distances between grid point locations and
+    def _r(self, gpos, mpos=0.0):
+        """Calculates the virtual distances between grid point locations and
         microphone locations or the origin. These virtual distances correspond
         to travel times of the sound. Functionality may change in the future.
 
         Parameters
         ----------
         gpos : array of floats of shape (3, N)
             The locations of points in the beamforming map grid in 3D cartesian
@@ -211,357 +231,339 @@
             The locations of microphones in 3D cartesian co-ordinates. If not
             given, then only one microphone at the origin (0, 0, 0) is
             considered.
 
         Returns
         -------
         array of floats
-            The distances in a twodimensional (N, M) array of floats. If M==1, 
+            The distances in a twodimensional (N, M) array of floats. If M==1,
             then only a one-dimensional array is returned.
+
         """
         if isscalar(mpos):
-            mpos = array((0, 0, 0), dtype = float32)[:, newaxis]
-        fdv = self.fdv/sqrt((self.fdv*self.fdv).sum())
+            mpos = array((0, 0, 0), dtype=float32)[:, newaxis]
+        fdv = self.fdv / sqrt((self.fdv * self.fdv).sum())
         mpos = mpos[:, newaxis, :]
-        rmv = gpos[:, :, newaxis]-mpos
-        rm = sqrt(sum(rmv*rmv, 0))
-        macostheta = (self.ma*sum(rmv.reshape((3, -1))*fdv[:, newaxis], 0)\
-            /rm.reshape(-1)).reshape(rm.shape)
-        rm *= 1/(-macostheta + sqrt(macostheta*macostheta-self.ma*self.ma+1))
+        rmv = gpos[:, :, newaxis] - mpos
+        rm = sqrt(sum(rmv * rmv, 0))
+        macostheta = (self.ma * sum(rmv.reshape((3, -1)) * fdv[:, newaxis], 0) / rm.reshape(-1)).reshape(rm.shape)
+        rm *= 1 / (-macostheta + sqrt(macostheta * macostheta - self.ma * self.ma + 1))
         if rm.shape[1] == 1:
             rm = rm[:, 0]
         return rm
-    
 
-class FlowField( HasPrivateTraits ):
-    """
-    An abstract base class for a spatial flow field.
-    """
+
+class FlowField(HasPrivateTraits):
+    """An abstract base class for a spatial flow field."""
+
     digest = Property
 
-    def _get_digest( self ):
+    def _get_digest(self):
         return ''
 
-    def v( self, xx):
-        """
-        Provides the flow field as a function of the location. This is
+    def v(self, xx):  # noqa: ARG002
+        """Provides the flow field as a function of the location. This is
         implemented here for the possibly most simple case: a quiescent fluid.
 
         Parameters
         ----------
         xx : array of floats of shape (3, )
             Location in the fluid for which to provide the data.
 
         Returns
         -------
         tuple with two elements
             The first element in the tuple is the velocity vector and the
             second is the Jacobian of the velocity vector field, both at the
             given location.
+
         """
-        v = array((0., 0., 0.))
-        dv = array(((0., 0., 0.), (0., 0., 0.), (0., 0., 0.)))
+        v = array((0.0, 0.0, 0.0))
+        dv = array(((0.0, 0.0, 0.0), (0.0, 0.0, 0.0), (0.0, 0.0, 0.0)))
         return -v, -dv
 
-class SlotJet( FlowField ):
-    """
-    Provides an analytical approximation of the flow field of a slot jet, 
+
+class SlotJet(FlowField):
+    """Provides an analytical approximation of the flow field of a slot jet,
     see :ref:`Albertson et al., 1950<Albertson1950>`.
     """
+
     #: Exit velocity at jet origin, i.e. the nozzle. Defaults to 0.
-    v0 = Float(0.0, 
-        desc="exit velocity")
+    v0 = Float(0.0, desc='exit velocity')
 
-    #: Location of a point at the slot center line, 
+    #: Location of a point at the slot center line,
     #: defaults to the co-ordinate origin.
-    origin = CArray( dtype=float64, shape=(3, ), value=array((0., 0., 0.)), 
-        desc="center of nozzle")
+    origin = CArray(dtype=float64, shape=(3,), value=array((0.0, 0.0, 0.0)), desc='center of nozzle')
 
     #: Unit flow direction of the slot jet, defaults to (1,0,0).
-    flow = CArray( dtype=float64, shape=(3, ), value=array((1., 0., 0.)), 
-        desc="flow direction")
+    flow = CArray(dtype=float64, shape=(3,), value=array((1.0, 0.0, 0.0)), desc='flow direction')
 
     #: Unit vector parallel to slot center plane, defaults to (0,1,0).
-    plane = CArray( dtype=float64, shape=(3, ), value=array((0., 1., 0.)), 
-        desc="slot center line direction")
-        
+    plane = CArray(dtype=float64, shape=(3,), value=array((0.0, 1.0, 0.0)), desc='slot center line direction')
+
     #: Width of the slot, defaults to 0.2 .
-    B = Float(0.2, 
-        desc="nozzle diameter")
+    B = Float(0.2, desc='nozzle diameter')
 
     # internal identifier
     digest = Property(
-        depends_on=['v0', 'origin', 'flow', 'plane', 'B'], 
-        )
+        depends_on=['v0', 'origin', 'flow', 'plane', 'B'],
+    )
 
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
+    def _get_digest(self):
+        return digest(self)
 
-    def v( self, xx):
-        """
-        Provides the flow field as a function of the location. This is
+    def v(self, xx):
+        """Provides the flow field as a function of the location. This is
         implemented here only for the component in the direction of :attr:`flow`;
         entrainment components are set to zero.
 
         Parameters
         ----------
         xx : array of floats of shape (3, )
             Location in the fluid for which to provide the data.
 
         Returns
         -------
         tuple with two elements
             The first element in the tuple is the velocity vector and the
             second is the Jacobian of the velocity vector field, both at the
             given location.
+
         """
         # TODO: better to make sure that self.flow and self.plane are indeed unit vectors before
         # normalize
-        flow = self.flow/norm(self.flow)
-        plane = self.plane/norm(self.plane)
+        flow = self.flow / norm(self.flow)
+        plane = self.plane / norm(self.plane)
         # additional axes of global co-ordinate system
-        yy = -cross(flow,plane)
-        zz = cross(flow,yy)
+        yy = -cross(flow, plane)
+        zz = cross(flow, yy)
         # distance from slot exit plane
-        xx1 = xx-self.origin
-        # local co-ordinate system 
-        x = dot(flow,xx1)
-        y = dot(yy,xx1)
-        x1 = 0.109*x
-        h1 = abs(y)+sqrt(pi)*0.5*x1-0.5*self.B
+        xx1 = xx - self.origin
+        # local co-ordinate system
+        x = dot(flow, xx1)
+        y = dot(yy, xx1)
+        x1 = 0.109 * x
+        h1 = abs(y) + sqrt(pi) * 0.5 * x1 - 0.5 * self.B
         if h1 < 0.0:
             # core jet
             Ux = self.v0
             Udx = 0
             Udy = 0
         else:
             # shear layer
-            Ux = self.v0*exp(-h1*h1/(2*x1*x1))
-            Udx = (h1*h1/(x*x1*x1)-sqrt(pi)*0.5*h1/(x*x1))*Ux
-            Udy = -sign(y)*h1*Ux/(x1*x1)
+            Ux = self.v0 * exp(-h1 * h1 / (2 * x1 * x1))
+            Udx = (h1 * h1 / (x * x1 * x1) - sqrt(pi) * 0.5 * h1 / (x * x1)) * Ux
+            Udy = -sign(y) * h1 * Ux / (x1 * x1)
         # Jacobi matrix
-        dU = array(((Udx,0,0),(Udy,0,0),(0,0,0))).T
+        dU = array(((Udx, 0, 0), (Udy, 0, 0), (0, 0, 0))).T
         # rotation matrix
-        R = array((flow,yy,zz)).T
-        return dot(R,array((Ux,0,0))), dot(dot(R,dU),R.T)
+        R = array((flow, yy, zz)).T
+        return dot(R, array((Ux, 0, 0))), dot(dot(R, dU), R.T)
 
-class OpenJet( FlowField ):
-    """
-    Provides an analytical approximation of the flow field of an open jet, 
+
+class OpenJet(FlowField):
+    """Provides an analytical approximation of the flow field of an open jet,
     see :ref:`Albertson et al., 1950<Albertson1950>`.
 
     Notes
     -----
     This is not a fully generic implementation and is limited to flow in the
     x-direction only. No other directions are possible at the moment and flow
     components in the other direction are zero.
+
     """
+
     #: Exit velocity at jet origin, i.e. the nozzle. Defaults to 0.
-    v0 = Float(0.0, 
-        desc="exit velocity")
+    v0 = Float(0.0, desc='exit velocity')
 
     #: Location of the nozzle center, defaults to the co-ordinate origin.
-    origin = CArray( dtype=float64, shape=(3, ), value=array((0., 0., 0.)), 
-        desc="center of nozzle")
+    origin = CArray(dtype=float64, shape=(3,), value=array((0.0, 0.0, 0.0)), desc='center of nozzle')
 
     #: Diameter of the nozzle, defaults to 0.2 .
-    D = Float(0.2, 
-        desc="nozzle diameter")
+    D = Float(0.2, desc='nozzle diameter')
 
     # internal identifier
     digest = Property(
-        depends_on=['v0', 'origin', 'D'], 
-        )
+        depends_on=['v0', 'origin', 'D'],
+    )
 
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
+    def _get_digest(self):
+        return digest(self)
 
-    def v( self, xx):
-        """
-        Provides the flow field as a function of the location. This is
+    def v(self, xx):
+        """Provides the flow field as a function of the location. This is
         implemented here only for a jet in `x`-direction and the `y`- and
         `z`-components are set to zero.
 
         Parameters
         ----------
         xx : array of floats of shape (3, )
             Location in the fluid for which to provide the data.
 
         Returns
         -------
         tuple with two elements
             The first element in the tuple is the velocity vector and the
             second is the Jacobian of the velocity vector field, both at the
             given location.
+
         """
-        x, y, z = xx-self.origin
-        r = sqrt(y*y+z*z)
-        x1 = 0.081*x
-        h1 = r+x1-0.5*self.D
-        U = self.v0*exp(-h1*h1/(2*x1*x1))
+        x, y, z = xx - self.origin
+        r = sqrt(y * y + z * z)
+        x1 = 0.081 * x
+        h1 = r + x1 - 0.5 * self.D
+        U = self.v0 * exp(-h1 * h1 / (2 * x1 * x1))
         if h1 < 0.0:
             Udr = 0.0
             U = self.v0
         else:
-            Udr = -h1*U/(x1*x1)
+            Udr = -h1 * U / (x1 * x1)
         if r > 0.0:
-            Udy = y*Udr/r
-            Udz = z*Udr/r
+            Udy = y * Udr / r
+            Udz = z * Udr / r
         else:
             Udy = Udz = 0.0
-        Udx = (h1*h1/(x*x1*x1)-h1/(x*x1))*U
+        Udx = (h1 * h1 / (x * x1 * x1) - h1 / (x * x1)) * U
         if h1 < 0.0:
             Udx = 0
 
         # flow field
-        v = array( (U, 0., 0.) )
+        v = array((U, 0.0, 0.0))
         # Jacobi matrix
-        dv = array( ((Udx, 0., 0.), (Udy, 0., 0.), (Udz, 0., 0.)) ).T
+        dv = array(((Udx, 0.0, 0.0), (Udy, 0.0, 0.0), (Udz, 0.0, 0.0))).T
         return v, dv
 
 
+class RotatingFlow(FlowField):
+    """Provides an analytical approximation of the flow field of a rotating fluid with constant flow."""
 
-
-class RotatingFlow( FlowField ):
-    """
-    Provides an analytical approximation of the flow field of a rotating fluid with constant flow. 
-
-
-    """
     #: Exit velocity at jet origin, i.e. the nozzle. Defaults to 0.
-    rpm = Float(0.0,
-        desc="revolutions per minute of the virtual array; negative values for clockwise rotation")
+    rpm = Float(0.0, desc='revolutions per minute of the virtual array; negative values for clockwise rotation')
 
-    v0 = Float(0.0, 
-        desc="flow velocity")
+    v0 = Float(0.0, desc='flow velocity')
 
     #: Location of the nozzle center, defaults to the co-ordinate origin.
-    origin = CArray( dtype=float64, shape=(3, ), value=array((0., 0., 0.)), 
-        desc="center of nozzle")
+    origin = CArray(dtype=float64, shape=(3,), value=array((0.0, 0.0, 0.0)), desc='center of nozzle')
 
     # internal identifier
     digest = Property(
-        depends_on=['v0', 'origin', 'rpm'], 
-        )
+        depends_on=['v0', 'origin', 'rpm'],
+    )
 
     # internal identifier
     omega = Property(
-        depends_on=['rpm'], 
-        )
+        depends_on=['rpm'],
+    )
 
     @cached_property
     def _get_omega(self):
         return 2 * pi * self.rpm / 60
 
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
+    def _get_digest(self):
+        return digest(self)
 
-    def v( self, xx):
-        """
-        Provides the rotating flow field around the z-Axis as a function of the location.
+    def v(self, xx):
+        """Provides the rotating flow field around the z-Axis as a function of the location.
 
         Parameters
         ----------
         xx : array of floats of shape (3, )
             Location in the fluid for which to provide the data.
 
         Returns
         -------
         tuple with two elements
             The first element in the tuple is the velocity vector and the
             second is the Jacobian of the velocity vector field, both at the
             given location.
+
         """
-        x, y, z = xx-self.origin
+        x, y, z = xx - self.origin
 
         # rotational speed
         omega = self.omega
 
-        #velocity vector
+        # velocity vector
         U = omega * y
         V = -omega * x
-        W = self.v0 
-        
+        W = self.v0
+
         # flow field
-        v = array( (U, V, W) )
+        v = array((U, V, W))
         # Jacobi matrix
-        dv = array( ((0, -omega, 0.), (omega, 0, 0.), (0., 0., 0.)) ).T
+        dv = array(((0, -omega, 0.0), (omega, 0, 0.0), (0.0, 0.0, 0.0))).T
         return v, dv
 
 
-
-
-def spiral_sphere(N, Om=2*pi, b=array((0, 0, 1))):    #change to 4*pi
-    """
-    Internal helper function for the raycasting that returns an array of
+def spiral_sphere(N, Om=None, b=None):  # change to 4*pi
+    """Internal helper function for the raycasting that returns an array of
     unit vectors (N, 3) giving equally distributed directions on a part of
     sphere given by the center direction b and the solid angle Om.
     """
+    Om = 2 * pi if Om is None else Om
+    b = array((0, 0, 1)) if b is None else b
     # first produce 'equally' distributed directions in spherical coords
-    o = 4*pi/Om 
-    h = -1+ 2*arange(N)/(N*o-1.)
+    o = 4 * pi / Om
+    h = -1 + 2 * arange(N) / (N * o - 1.0)
     theta = arccos(h)
     phi = zeros_like(theta)
     for i, hk in enumerate(h[1:]):
-        phi[i+1] = phi[i]+3.6/sqrt(N*o*(1-hk*hk)) % (2*pi)
+        phi[i + 1] = phi[i] + 3.6 / sqrt(N * o * (1 - hk * hk)) % (2 * pi)
     # translate to cartesian coords
     xyz = vstack((sin(theta) * cos(phi), sin(theta) * sin(phi), cos(theta)))
     # mirror everything on a plane so that b points into the center
     a = xyz[:, 0]
-    b = b/norm(b)
-    ab = (a-b)[:, newaxis]
-    if norm(ab)<1e-10:
+    b = b / norm(b)
+    ab = (a - b)[:, newaxis]
+    if norm(ab) < 1e-10:
         return xyz
     # this is the Householder matrix for mirroring
-    H = identity(3)-dot(ab, ab.T)/dot(ab.T, a)
+    H = identity(3) - dot(ab, ab.T) / dot(ab.T, a)
     # actual mirroring
     return dot(H, xyz)
 
+
 class GeneralFlowEnvironment(Environment):
-    """
-    An acoustic environment with a generic flow field.
+    """An acoustic environment with a generic flow field.
 
     This class provides the facilities to calculate the travel time (distances)
     between grid point locations and microphone locations in a generic flow
     field with non-uniform velocities that depend on the location. The
     algorithm for the calculation uses a ray-tracing approach that bases on
     rays cast from every microphone position in multiple directions and traced
     backwards in time. The result is interpolated within a tetrahedal grid
     spanned between these rays.
     """
+
     #: The flow field, must be of type :class:`~acoular.environments.FlowField`.
-    ff = Trait(FlowField, 
-        desc="flow field")
+    ff = Trait(FlowField, desc='flow field')
 
     #: Number of rays used per solid angle :math:`\Omega`, defaults to 200.
-    N = Int(200, 
-        desc="number of rays per Om")
+    N = Int(200, desc='number of rays per Om')
 
     #: The maximum solid angle used in the algorithm, defaults to :math:`\pi`.
-    Om = Float(pi, 
-        desc="maximum solid angle")
+    Om = Float(pi, desc='maximum solid angle')
 
     # internal identifier
     digest = Property(
-        depends_on=['c', 'ff.digest', 'N', 'Om'], 
-        )
+        depends_on=['c', 'ff.digest', 'N', 'Om'],
+    )
 
     # internal dictionary of interpolators
     idict = Dict
 
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
+    def _get_digest(self):
+        return digest(self)
 
-    def _r( self, gpos, mpos=0.0):
-        """
-        Calculates the virtual distances between grid point locations and
+    def _r(self, gpos, mpos=0.0):
+        """Calculates the virtual distances between grid point locations and
         microphone locations or the origin. These virtual distances correspond
         to travel times of the sound along a ray that is traced through the
         medium. Functionality may change in the future.
 
         Parameters
         ----------
         gpos : array of floats of shape (3, N)
@@ -571,111 +573,112 @@
             The locations of microphones in 3D cartesian co-ordinates. If not
             given, then only one microphone at the origin (0, 0, 0) is
             considered.
 
         Returns
         -------
         array of floats
-            The distances in a twodimensional (N, M) array of floats. If M==1, 
+            The distances in a twodimensional (N, M) array of floats. If M==1,
             then only a one-dimensional array is returned.
+
         """
         c = self.c
-        
+
         if isscalar(mpos):
-            mpos = array((0, 0, 0), dtype = float32)[:, newaxis]
+            mpos = array((0, 0, 0), dtype=float32)[:, newaxis]
 
         gt = empty((gpos.shape[-1], mpos.shape[-1]))
         for micnum, x0 in enumerate(mpos.T):
-            key = x0.tobytes() # make array hashable
-            #todo: the interpolator also depends the roi, so idict keys should also depend on roi
+            key = x0.tobytes()  # make array hashable
+            # TODO: the interpolator also depends the roi, so idict keys should also depend on roi
             # OR the idict should be cleaned if roi changes
             try:
-                li = self.idict[key] # fetch stored interpolator
+                li = self.idict[key]  # fetch stored interpolator
             except KeyError:
                 # if interpolator doesn't exist, construct it
                 roi = gpos
                 if self.roi is not None:
                     roi = self.roi
                 li = self.get_interpolator(roi, x0)
                 self.idict[key] = li
             # do the interpolation
             gt[:, micnum] = li(gpos.T)
         if gt.shape[1] == 1:
             gt = gt[:, 0]
-        return c*gt #return distance along ray
+        return c * gt  # return distance along ray
 
-    def get_interpolator( self, roi, x0 ):
-        """
-        gets an LinearNDInterpolator object
+    def get_interpolator(self, roi, x0):
+        """Gets an LinearNDInterpolator object.
 
         Parameters
         ----------
         roi : array of floats of shape (3, N)
             The locations of points in the region of interest in 3D cartesian
             co-ordinates. Used to estimate the maximum distance and ROI
             extension and center.
         x0 : array of floats of shape (3)
-            The location of the microphone in 3D cartesian co-ordinates. 
+            The location of the microphone in 3D cartesian co-ordinates.
 
         Returns
         -------
         LinearNDInterpolator object
+
         """
         c = self.c
 
         # the DE system
-        def f1(t, y, v):
+        def f1(t, y, v):  # noqa: ARG001
             x = y[0:3]
             s = y[3:6]
             vv, dv = v(x)
-            sa = sqrt(s[0]*s[0]+s[1]*s[1]+s[2]*s[2])
+            sa = sqrt(s[0] * s[0] + s[1] * s[1] + s[2] * s[2])
             x = empty(6)
-            x[0:3] = c*s/sa - vv # time reversal
-            x[3:6] = dot(s, -dv.T) # time reversal
+            x[0:3] = c * s / sa - vv  # time reversal
+            x[3:6] = dot(s, -dv.T)  # time reversal
             return x
 
         # integration along a single ray
         def fr(x0, n0, rmax, dt, v, xyz, t):
-            s0 = n0 / (c+dot(v(x0)[0], n0))
+            s0 = n0 / (c + dot(v(x0)[0], n0))
             y0 = hstack((x0, s0))
             oo = ode(f1)
             oo.set_f_params(v)
-            oo.set_integrator('vode', 
-                              rtol=1e-4, # accuracy !
-                              max_step=1e-4*rmax) # for thin shear layer
+            oo.set_integrator(
+                'vode',
+                rtol=1e-4,  # accuracy !
+                max_step=1e-4 * rmax,
+            )  # for thin shear layer
             oo.set_initial_value(y0, 0)
             while oo.successful():
                 xyz.append(oo.y[0:3])
                 t.append(oo.t)
-                if norm(oo.y[0:3]-x0)>rmax:
+                if norm(oo.y[0:3] - x0) > rmax:
                     break
-                oo.integrate(oo.t+dt)
+                oo.integrate(oo.t + dt)
 
         gs2 = roi.shape[-1]
         vv = self.ff.v
         NN = int(sqrt(self.N))
-        xe = roi.mean(1) # center of grid
-        r = x0[:, newaxis]-roi
-        rmax = sqrt((r*r).sum(0).max()) # maximum distance
-        nv = spiral_sphere(self.N, self.Om, b=xe-x0)
-        rstep = rmax/sqrt(self.N)
+        xe = roi.mean(1)  # center of grid
+        r = x0[:, newaxis] - roi
+        rmax = sqrt((r * r).sum(0).max())  # maximum distance
+        nv = spiral_sphere(self.N, self.Om, b=xe - x0)
+        rstep = rmax / sqrt(self.N)
         rmax += rstep
-        tstep = rstep/c
+        tstep = rstep / c
         xyz = []
         t = []
         lastind = 0
         for i, n0 in enumerate(nv.T):
             fr(x0, n0, rmax, tstep, vv, xyz, t)
             if i and i % NN == 0:
                 if not lastind:
                     dd = ConvexHull(vstack((roi.T, xyz)), incremental=True)
                 else:
                     dd.add_points(xyz[lastind:], restart=True)
                 lastind = len(xyz)
                 # ConvexHull includes grid if no grid points on hull
-                if dd.simplices.min()>=gs2:
+                if dd.simplices.min() >= gs2:
                     break
         xyz = array(xyz)
         t = array(t)
         return LinearNDInterpolator(xyz, t)
-
-
```

### Comparing `acoular-24.3/acoular/fastFuncs.py` & `acoular-24.5/acoular/fastFuncs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,58 +1,64 @@
-#!/usr/bin/env python2
-# -*- coding: utf-8 -*-
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 # Copyright (c) Acoular Development Team.
-#------------------------------------------------------------------------------
-"""
-This file contains all the functionalities which are very expansive, regarding
+# ------------------------------------------------------------------------------
+"""Contains all the functionalities which are very expansive, regarding
 computational costs. All functionalities are optimized via NUMBA.
 """
-import numpy as np
+
 import numba as nb
+import numpy as np
 
 cachedOption = True  # if True: saves the numba func as compiled func in sub directory
 parallelOption = 'parallel'  # if numba.guvectorize is used: 'CPU' for single threading; 'parallel' for multithreading; 'cuda' for calculating on GPU
-fastOption = True # fastmath options 
+fastOption = True  # fastmath options
 
 
 # Formerly known as 'faverage'
-@nb.njit([nb.complex128[:,:,::1](nb.complex128[:,:,::1], nb.complex128[:,::1]), 
-          nb.complex64[:,:,::1](nb.complex64[:,:,::1], nb.complex64[:,::1])], cache=cachedOption, parallel=True, fastmath=fastOption)
+@nb.njit(
+    [
+        nb.complex128[:, :, ::1](nb.complex128[:, :, ::1], nb.complex128[:, ::1]),
+        nb.complex64[:, :, ::1](nb.complex64[:, :, ::1], nb.complex64[:, ::1]),
+    ],
+    cache=cachedOption,
+    parallel=True,
+    fastmath=fastOption,
+)
 def calcCSM(csm, SpecAllMics):
-    """ Adds a given spectrum to the Cross-Spectral-Matrix (CSM).
+    """Adds a given spectrum to the Cross-Spectral-Matrix (CSM).
     Here only the upper triangular matrix of the CSM is calculated. After
-    averaging over the various ensembles, the whole CSM is created via complex 
-    conjugation transposing. This happens outside 
-    (in :class:`PowerSpectra<acoular.spectra.PowerSpectra>`). 
+    averaging over the various ensembles, the whole CSM is created via complex
+    conjugation transposing. This happens outside
+    (in :class:`PowerSpectra<acoular.spectra.PowerSpectra>`).
     This method was called 'faverage' in acoular versions <= 16.5.
-    
+
     Parameters
     ----------
-    csm : complex128[nFreqs, nMics, nMics] 
+    csm : complex128[nFreqs, nMics, nMics]
         The cross spectral matrix which gets updated with the spectrum of the ensemble.
-    SpecAllMics : complex128[nFreqs, nMics] 
+    SpecAllMics : complex128[nFreqs, nMics]
         Spectrum of the added ensemble at all Mics.
-    
+
     Returns
     -------
     None : as the input csm gets overwritten.
+
     """
     nFreqs = csm.shape[0]
     nMics = csm.shape[1]
     for cntFreq in nb.prange(nFreqs):
         for cntColumn in range(nMics):
             temp = SpecAllMics[cntFreq, cntColumn].conjugate()
             for cntRow in range(cntColumn + 1):  # calculate upper triangular matrix (of every frequency-slice) only
                 csm[cntFreq, cntRow, cntColumn] += temp * SpecAllMics[cntFreq, cntRow]
     return csm
 
-    
+
 def beamformerFreq(steerVecType, boolRemovedDiagOfCSM, normFactor, inputTupleSteer, inputTupleCsm):
-    """ Conventional beamformer in frequency domain. Use either a predefined
+    r"""Conventional beamformer in frequency domain. Use either a predefined
     steering vector formulation (see Sarradj 2012) or pass your own
     steering vector.
 
     Parameters
     ----------
     steerVecType : (one of the following strings: 'classic' (I), 'inverse' (II), 'true level' (III), 'true location' (IV), 'custom')
         Either build the steering vector via the predefined formulations
@@ -79,217 +85,234 @@
         perform standard CSM-beamformer:
             inputTupleCsm = csm
                 csm : complex128[ nMics, nMics]
                     The cross spectral matrix for one frequency
         perform beamformer on eigenvalue decomposition of csm:
             inputTupleCsm = (eigValues, eigVectors)    , with
                 eigValues : float64[nEV]
-                    nEV is the number of eigenvalues which should be taken into account. 
+                    nEV is the number of eigenvalues which should be taken into account.
                     All passed eigenvalues will be evaluated.
                 eigVectors : complex128[nMics, nEV]
                     Eigen vectors corresponding to eigValues. All passed eigenvector slices will be evaluated.
 
     Returns
     -------
-    *Autopower spectrum beamforming map [nGridPoints] 
-         
-    *steer normalization factor [nGridPoints]... contains the values the autopower needs to be multiplied with, in order to 
-    fullfill 'steer^H * steer = 1' as needed for functional beamforming. 
-    
+    *Autopower spectrum beamforming map [nGridPoints]
+
+    *steer normalization factor [nGridPoints]... contains the values the autopower needs to be multiplied with, in order to
+    fullfill 'steer^H * steer = 1' as needed for functional beamforming.
+
     Some Notes on the optimization of all subroutines
     -------------------------------------------------
     Reducing beamforming equation:
-        Let the csm be C and the steering vector be h, than, using Linear Albegra, the conventional beamformer can be written as 
-        
+        Let the csm be C and the steering vector be h, than, using Linear Albegra, the conventional beamformer can be written as
+
         .. math:: B = h^H \\cdot C \\cdot h,
         with ^H meaning the complex conjugated transpose.
         When using that C is a hermitian matrix one can reduce the equation to
-        
+
         .. math:: B = h^H \\cdot C_D \\cdot h + 2 \\cdot Real(h^H \\cdot C_U \\cdot h),
         where C_D and C_U are the diagonal part and upper part of C respectively.
     Steering vector:
-        Theoretically the steering vector always includes the term "exp(distMicsGrid - distArrayCenterGrid)", 
-        but as the steering vector gets multplied with its complex conjugation in all beamformer routines, 
+        Theoretically the steering vector always includes the term "exp(distMicsGrid - distArrayCenterGrid)",
+        but as the steering vector gets multplied with its complex conjugation in all beamformer routines,
         the constant "distArrayCenterGrid" cancels out --> In order to save operations, it is not implemented.
     Spectral decomposition of the CSM:
         In Linear Algebra the spectral decomposition of the CSM matrix would be:
-        
+
         .. math:: CSM = \\sum_{i=1}^{nEigenvalues} \\lambda_i (v_i \\cdot v_i^H) ,
-        where lambda_i is the i-th eigenvalue and 
-        v_i is the eigenvector[nEigVal,1] belonging to lambda_i and ^H denotes the complex conjug transpose. 
-        Using this, one must not build the whole CSM (which would be time consuming), but can drag the 
+        where lambda_i is the i-th eigenvalue and
+        v_i is the eigenvector[nEigVal,1] belonging to lambda_i and ^H denotes the complex conjug transpose.
+        Using this, one must not build the whole CSM (which would be time consuming), but can drag the
         steering vector into the sum of the spectral decomp. This saves a lot of operations.
     Squares:
         Seemingly "a * a" is slightly faster than "a**2" in numba
     Square of abs():
-        Even though "a.real**2 + a.imag**2" would have fewer operations, modern processors seem to be optimized 
+        Even though "a.real**2 + a.imag**2" would have fewer operations, modern processors seem to be optimized
         for "a * a.conj" and are slightly faster the latter way. Both Versions are much faster than "abs(a)**2".
     Using Cascading Sums:
-        When using the Spectral-Decomposition-Beamformer one could use numpys cascading sums for the scalar product 
-        "eigenVec.conj * steeringVector". BUT (at the moment) this only brings benefits in comp-time for a very 
+        When using the Spectral-Decomposition-Beamformer one could use numpys cascading sums for the scalar product
+        "eigenVec.conj * steeringVector". BUT (at the moment) this only brings benefits in comp-time for a very
         small range of nMics (approx 250) --> Therefor it is not implemented here.
+
     """
-    boolIsEigValProb = isinstance(inputTupleCsm, tuple)# len(inputTupleCsm) > 1
+    boolIsEigValProb = isinstance(inputTupleCsm, tuple)  # len(inputTupleCsm) > 1
     # get the beamformer type (key-tuple = (isEigValProblem, formulationOfSteeringVector, RemovalOfCSMDiag))
-    beamformerDict = {(False, 'custom', False) : _freqBeamformer_SpecificSteerVec_FullCSM,
-                      (False, 'custom', True) : _freqBeamformer_SpecificSteerVec_CsmRemovedDiag,
-                      (True, 'custom', False) : _freqBeamformer_EigValProb_SpecificSteerVec_FullCSM,
-                      (True, 'custom', True) : _freqBeamformer_EigValProb_SpecificSteerVec_CsmRemovedDiag}
-    sth = {'classic':1, 'inverse':2,'true level':3, 'true location':4}
-   
+    beamformerDict = {
+        (False, 'custom', False): _freqBeamformer_SpecificSteerVec_FullCSM,
+        (False, 'custom', True): _freqBeamformer_SpecificSteerVec_CsmRemovedDiag,
+        (True, 'custom', False): _freqBeamformer_EigValProb_SpecificSteerVec_FullCSM,
+        (True, 'custom', True): _freqBeamformer_EigValProb_SpecificSteerVec_CsmRemovedDiag,
+    }
+    sth = {'classic': 1, 'inverse': 2, 'true level': 3, 'true location': 4}
+
     # prepare Input
     if steerVecType == 'custom':  # beamformer with custom steering vector
         steerVec = inputTupleSteer
         nGridPoints = steerVec.shape[0]
     else:  # predefined beamformers (Formulation I - IV)
         distGridToArrayCenter, distGridToAllMics, waveNumber = inputTupleSteer
-        if not isinstance(waveNumber, np.ndarray): waveNumber = np.array([waveNumber]) #for backward compatibility
+        if not isinstance(waveNumber, np.ndarray):
+            waveNumber = np.array([waveNumber])  # for backward compatibility
         nGridPoints = distGridToAllMics.shape[0]
     if boolIsEigValProb:
-        eigVal, eigVec = inputTupleCsm#[0], inputTupleCsm[1]
+        eigVal, eigVec = inputTupleCsm  # [0], inputTupleCsm[1]
     else:
         csm = inputTupleCsm
-    
+
     # beamformer routine: parallelized over Gridpoints
     beamformOutput = np.zeros(nGridPoints, np.float64)
     steerNormalizeOutput = np.zeros_like(beamformOutput)
     result = np.zeros(nGridPoints, np.float64)
     normalHelp = np.zeros_like(result)
     if steerVecType == 'custom':  # beamformer with custom steering vector
         coreFunc = beamformerDict[(boolIsEigValProb, steerVecType, boolRemovedDiagOfCSM)]
         if boolIsEigValProb:
             coreFunc(eigVal, eigVec, steerVec, normFactor, result, normalHelp)
         else:
             coreFunc(csm, steerVec, normFactor, result, normalHelp)
     else:  # predefined beamformers (Formulation I - IV)
         if boolIsEigValProb:
-            _freqBeamformer_EigValues(eigVal, np.ascontiguousarray(eigVec), distGridToArrayCenter, distGridToAllMics, waveNumber[0], normFactor, 
-                                    boolRemovedDiagOfCSM, sth[steerVecType],
-                                    result, normalHelp)
+            _freqBeamformer_EigValues(
+                eigVal,
+                np.ascontiguousarray(eigVec),
+                distGridToArrayCenter,
+                distGridToAllMics,
+                waveNumber[0],
+                normFactor,
+                boolRemovedDiagOfCSM,
+                sth[steerVecType],
+                result,
+                normalHelp,
+            )
         else:
-            _freqBeamformer_FullCSM(csm, distGridToArrayCenter, distGridToAllMics, waveNumber[0], normFactor, 
-                                    boolRemovedDiagOfCSM, sth[steerVecType],
-                                    result, normalHelp)
+            _freqBeamformer_FullCSM(
+                csm,
+                distGridToArrayCenter,
+                distGridToAllMics,
+                waveNumber[0],
+                normFactor,
+                boolRemovedDiagOfCSM,
+                sth[steerVecType],
+                result,
+                normalHelp,
+            )
     beamformOutput = result
-    steerNormalizeOutput = normalHelp 
-    return beamformOutput, steerNormalizeOutput 
+    steerNormalizeOutput = normalHelp
+    return beamformOutput, steerNormalizeOutput
+
 
 # fast implementation of full matrix beamformers
 @nb.njit(
     [
         (
             nb.complex128[:, ::1],
             nb.float64[::1],
             nb.float64[:, ::1],
             nb.float64,
             nb.float64,
             nb.boolean,
             nb.int64,
             nb.float64[::1],
             nb.float64[::1],
-        )
+        ),
     ],
     cache=cachedOption,
     parallel=True,
-    error_model="numpy"
+    error_model='numpy',
 )
 def _freqBeamformer_FullCSM(
     csm,
     distGridToArrayCenter,
     distGridToAllMics,
     waveNumber,
     signalLossNormalization,
     r_diag,
     steer_type,
     result,
     normalizeSteer,
 ):
     # see bottom of information header of 'beamformerFreq' for information on which steps are taken, in order to gain speed improvements.
     nMics = csm.shape[0]
-    st2 = (steer_type == 2)
-    st34 = (steer_type == 3 or steer_type == 4)
-    helpNormalize = 0.0 # just a hint for the compiler
+    st2 = steer_type == 2
+    st34 = steer_type == 3 or steer_type == 4
+    helpNormalize = 0.0  # just a hint for the compiler
     for gi in nb.prange(distGridToArrayCenter.shape[0]):
         steerVec = np.empty((nMics), np.complex128)
         # building steering vector: in order to save some operation -> some normalization steps are applied after mat-vec-multipl.
         for cntMics in range(nMics):
             expArg = np.float32(waveNumber * distGridToAllMics[gi, cntMics])
             steerVec[cntMics] = np.cos(expArg) - 1j * np.sin(expArg)
-        if st2:    
+        if st2:
             helpNormalize = 0.0
             for cntMics in range(nMics):
-                helpNormalize += distGridToAllMics[gi,cntMics] * distGridToAllMics[gi,cntMics]
-                steerVec[cntMics] *= distGridToAllMics[gi,cntMics]  # r_{t,i}-normalization is handled here
+                helpNormalize += distGridToAllMics[gi, cntMics] * distGridToAllMics[gi, cntMics]
+                steerVec[cntMics] *= distGridToAllMics[gi, cntMics]  # r_{t,i}-normalization is handled here
         if st34:
             helpNormalize = 0.0
             for cntMics in range(nMics):
-                helpNormalize += 1.0 / (distGridToAllMics[gi,cntMics] * distGridToAllMics[gi,cntMics])  
-                steerVec[cntMics] /= distGridToAllMics[gi,cntMics]  # r_{t,i}-normalization is handled here
+                helpNormalize += 1.0 / (distGridToAllMics[gi, cntMics] * distGridToAllMics[gi, cntMics])
+                steerVec[cntMics] /= distGridToAllMics[gi, cntMics]  # r_{t,i}-normalization is handled here
 
         # performing matrix-vector-multiplication (see bottom of information header of 'beamformerFreq)
         scalarProd = 0.0
         for cntMics in range(nMics):
             leftVecMatrixProd = 0.0 + 0.0j
             for cntMics2 in range(
-                cntMics
+                cntMics,
             ):  # calculate 'steer^H * CSM' of upper-triangular-part of csm (without diagonal)
-                leftVecMatrixProd += (
-                    csm[cntMics2, cntMics] * steerVec[cntMics2].conjugate()
-                )
+                leftVecMatrixProd += csm[cntMics2, cntMics] * steerVec[cntMics2].conjugate()
             scalarProd += (
                 2 * (leftVecMatrixProd * steerVec[cntMics]).real
             )  # use that csm is Hermitian (lower triangular of csm can be reduced to factor '2')
         if not r_diag:
             for cntMics in range(nMics):
                 scalarProd += (
-                    csm[cntMics, cntMics]
-                    * steerVec[cntMics].conjugate()
-                    * steerVec[cntMics]
+                    csm[cntMics, cntMics] * steerVec[cntMics].conjugate() * steerVec[cntMics]
                 ).real  # include diagonal of csm
 
         # specific normalzation for different steering vector formulations
         if steer_type == 1:
             normalizeFactor = nMics
             normalizeSteer[gi] = 1.0 / nMics
-            result[gi] = (
-                scalarProd / (normalizeFactor * normalizeFactor) * signalLossNormalization
-            )
+            result[gi] = scalarProd / (normalizeFactor * normalizeFactor) * signalLossNormalization
         elif steer_type == 2:
             normalizeFactor = nMics * distGridToArrayCenter[gi]
             normalizeFactorSquared = normalizeFactor * normalizeFactor
             normalizeSteer[gi] = helpNormalize / normalizeFactorSquared
             result[gi] = scalarProd / normalizeFactorSquared * signalLossNormalization
         elif steer_type == 3:
             normalizeFactor = distGridToArrayCenter[gi] * helpNormalize
             normalizeSteer[gi] = 1.0 / (distGridToArrayCenter[gi] * distGridToArrayCenter[gi]) / helpNormalize
             result[gi] = scalarProd / (normalizeFactor * normalizeFactor) * signalLossNormalization
         elif steer_type == 4:
             normalizeFactor = nMics * helpNormalize
             normalizeSteer[gi] = 1.0 / nMics
             result[gi] = scalarProd / normalizeFactor * signalLossNormalization
 
+
 # fast implementation of eigenvalue beamformers
 @nb.njit(
     [
         (
             nb.float64[::1],
             nb.complex128[:, ::1],
             nb.float64[::1],
             nb.float64[:, ::1],
             nb.float64,
             nb.float64,
             nb.boolean,
             nb.int64,
             nb.float64[::1],
             nb.float64[::1],
-        )
+        ),
     ],
     cache=cachedOption,
     parallel=True,
-    error_model="numpy"
+    error_model='numpy',
 )
 def _freqBeamformer_EigValues(
     eigVal,
     eigVec,
     distGridToArrayCenter,
     distGridToAllMics,
     waveNumber,
@@ -298,391 +321,538 @@
     steer_type,
     result,
     normalizeSteer,
 ):
     # see bottom of information header of 'beamformerFreq' for information on which steps are taken, in order to gain speed improvements.
     nMics = eigVec.shape[0]
     nEigs = len(eigVal)
-    st2 = (steer_type == 2)
-    st34 = (steer_type == 3 or steer_type == 4)
-    helpNormalize = 0.0 # just a hint for the compiler
+    st2 = steer_type == 2
+    st34 = steer_type == 3 or steer_type == 4
+    helpNormalize = 0.0  # just a hint for the compiler
     for gi in nb.prange(distGridToArrayCenter.shape[0]):
         steerVec = np.empty((nMics), np.complex128)
         # building steering vector: in order to save some operation -> some normalization steps are applied after mat-vec-multipl.
         for cntMics in range(nMics):
             expArg = np.float32(waveNumber * distGridToAllMics[gi, cntMics])
             steerVec[cntMics] = np.cos(expArg) - 1j * np.sin(expArg)
-        if st2:    
+        if st2:
             helpNormalize = 0.0
             for cntMics in range(nMics):
-                helpNormalize += distGridToAllMics[gi,cntMics] * distGridToAllMics[gi,cntMics]
-                steerVec[cntMics] *= distGridToAllMics[gi,cntMics]  # r_{t,i}-normalization is handled here
+                helpNormalize += distGridToAllMics[gi, cntMics] * distGridToAllMics[gi, cntMics]
+                steerVec[cntMics] *= distGridToAllMics[gi, cntMics]  # r_{t,i}-normalization is handled here
         if st34:
             helpNormalize = 0.0
             for cntMics in range(nMics):
-                helpNormalize += 1.0 / (distGridToAllMics[gi,cntMics] * distGridToAllMics[gi,cntMics])  
-                steerVec[cntMics] /= distGridToAllMics[gi,cntMics]  # r_{t,i}-normalization is handled here
+                helpNormalize += 1.0 / (distGridToAllMics[gi, cntMics] * distGridToAllMics[gi, cntMics])
+                steerVec[cntMics] /= distGridToAllMics[gi, cntMics]  # r_{t,i}-normalization is handled here
 
-        # eigenvalue beamforming    
+        # eigenvalue beamforming
         scalarProd = 0.0
         if r_diag:
             for cntEigVal in range(len(eigVal)):
                 scalarProdFullCSMperEigVal = 0.0 + 0.0j
                 scalarProdDiagCSMperEigVal = 0.0
                 for cntMics in range(nMics):
-                    temp1 = eigVec[cntMics, cntEigVal].conjugate() * steerVec[cntMics]  
+                    temp1 = eigVec[cntMics, cntEigVal].conjugate() * steerVec[cntMics]
                     scalarProdFullCSMperEigVal += temp1
-                    scalarProdDiagCSMperEigVal += (temp1 * temp1.conjugate()).real  
+                    scalarProdDiagCSMperEigVal += (temp1 * temp1.conjugate()).real
                 scalarProdFullCSMAbsSquared = (scalarProdFullCSMperEigVal * scalarProdFullCSMperEigVal.conjugate()).real
                 scalarProd += (scalarProdFullCSMAbsSquared - scalarProdDiagCSMperEigVal) * eigVal[cntEigVal]
         else:
             for cntEigVal in range(nEigs):
                 scalarProdFullCSMperEigVal = 0.0 + 0.0j
                 for cntMics in range(nMics):
                     scalarProdFullCSMperEigVal += eigVec[cntMics, cntEigVal].conjugate() * steerVec[cntMics]
-                scalarProdFullCSMAbsSquared = (scalarProdFullCSMperEigVal * scalarProdFullCSMperEigVal.conjugate()).real  
+                scalarProdFullCSMAbsSquared = (scalarProdFullCSMperEigVal * scalarProdFullCSMperEigVal.conjugate()).real
                 scalarProd += scalarProdFullCSMAbsSquared * eigVal[cntEigVal]
 
         # specific normalzation for different steering vector formulations
         if steer_type == 1:
             normalizeFactor = nMics
             normalizeSteer[gi] = 1.0 / nMics
-            result[gi] = (
-                scalarProd / (normalizeFactor * normalizeFactor) * signalLossNormalization
-            )
+            result[gi] = scalarProd / (normalizeFactor * normalizeFactor) * signalLossNormalization
         elif steer_type == 2:
             normalizeFactor = nMics * distGridToArrayCenter[gi]
             normalizeFactorSquared = normalizeFactor * normalizeFactor
             normalizeSteer[gi] = helpNormalize / normalizeFactorSquared
             result[gi] = scalarProd / normalizeFactorSquared * signalLossNormalization
         elif steer_type == 3:
             normalizeFactor = distGridToArrayCenter[gi] * helpNormalize
             normalizeSteer[gi] = 1.0 / (distGridToArrayCenter[gi] * distGridToArrayCenter[gi]) / helpNormalize
             result[gi] = scalarProd / (normalizeFactor * normalizeFactor) * signalLossNormalization
         elif steer_type == 4:
             normalizeFactor = nMics * helpNormalize
             normalizeSteer[gi] = 1.0 / nMics
             result[gi] = scalarProd / normalizeFactor * signalLossNormalization
 
-@nb.guvectorize([(nb.complex128[:,:], nb.complex128[:], nb.float64[:], nb.float64[:], nb.float64[:])], 
-                '(m,m),(m),()->(),()', nopython=True, target=parallelOption, cache=cachedOption, fastmath=fastOption)
+
+@nb.guvectorize(
+    [(nb.complex128[:, :], nb.complex128[:], nb.float64[:], nb.float64[:], nb.float64[:])],
+    '(m,m),(m),()->(),()',
+    nopython=True,
+    target=parallelOption,
+    cache=cachedOption,
+    fastmath=fastOption,
+)
 def _freqBeamformer_SpecificSteerVec_FullCSM(csm, steerVec, signalLossNormalization, result, normalizeSteer):
     # see bottom of information header of 'beamformerFreq' for information on which steps are taken, in order to gain speed improvements.
     nMics = csm.shape[0]
 
     # performing matrix-vector-multiplication (see bottom of information header of 'beamformerFreq')
     scalarProd = 0.0
     helpNormalize = 0.0
     for cntMics in range(nMics):
         helpNormalize += steerVec[cntMics] * steerVec[cntMics].conjugate()
         leftVecMatrixProd = 0.0 + 0.0j
         for cntMics2 in range(cntMics):  # calculate 'steer^H * CSM' of upper-triangular-part of csm (without diagonal)
             leftVecMatrixProd += csm[cntMics2, cntMics] * steerVec[cntMics2].conjugate()
-        scalarProd += 2 * (leftVecMatrixProd * steerVec[cntMics]).real  # use that csm is Hermitian (lower triangular of csm can be reduced to factor '2')
-        scalarProd += (csm[cntMics, cntMics] * steerVec[cntMics].conjugate() * steerVec[cntMics]).real  # include diagonal of csm
+        scalarProd += (
+            2 * (leftVecMatrixProd * steerVec[cntMics]).real
+        )  # use that csm is Hermitian (lower triangular of csm can be reduced to factor '2')
+        scalarProd += (
+            csm[cntMics, cntMics] * steerVec[cntMics].conjugate() * steerVec[cntMics]
+        ).real  # include diagonal of csm
     normalizeSteer[0] = helpNormalize.real
     result[0] = scalarProd * signalLossNormalization[0]
 
 
-@nb.guvectorize([(nb.complex128[:,:], nb.complex128[:], nb.float64[:], nb.float64[:], nb.float64[:])], 
-                '(m,m),(m),()->(),()', nopython=True, target=parallelOption, cache=cachedOption, fastmath=fastOption)
+@nb.guvectorize(
+    [(nb.complex128[:, :], nb.complex128[:], nb.float64[:], nb.float64[:], nb.float64[:])],
+    '(m,m),(m),()->(),()',
+    nopython=True,
+    target=parallelOption,
+    cache=cachedOption,
+    fastmath=fastOption,
+)
 def _freqBeamformer_SpecificSteerVec_CsmRemovedDiag(csm, steerVec, signalLossNormalization, result, normalizeSteer):
     # see bottom of information header of 'beamformerFreq' for information on which steps are taken, in order to gain speed improvements.
     nMics = csm.shape[0]
 
     # performing matrix-vector-multiplication (see bottom of information header of 'beamformerFreq')
     scalarProd = 0.0
     helpNormalize = 0.0
     for cntMics in range(nMics):
         helpNormalize += steerVec[cntMics] * steerVec[cntMics].conjugate()
         leftVecMatrixProd = 0.0 + 0.0j
         for cntMics2 in range(cntMics):  # calculate 'steer^H * CSM' of upper-triangular-part of csm (without diagonal)
             leftVecMatrixProd += csm[cntMics2, cntMics] * steerVec[cntMics2].conjugate()
-        scalarProd += 2 * (leftVecMatrixProd * steerVec[cntMics]).real  # use that csm is Hermitian (lower triangular of csm can be reduced to factor '2')
+        scalarProd += (
+            2 * (leftVecMatrixProd * steerVec[cntMics]).real
+        )  # use that csm is Hermitian (lower triangular of csm can be reduced to factor '2')
     normalizeSteer[0] = helpNormalize.real
     result[0] = scalarProd * signalLossNormalization[0]
-@nb.guvectorize([(nb.float64[:], nb.complex128[:,:], nb.complex128[:], nb.float64[:], nb.float64[:], nb.float64[:])],
-                 '(e),(m,e),(m),()->(),()', nopython=True, target=parallelOption, cache=cachedOption, fastmath=fastOption)
-def _freqBeamformer_EigValProb_SpecificSteerVec_FullCSM(eigVal, eigVec, steerVec, signalLossNormalization, result, normalizeSteer):
+
+
+@nb.guvectorize(
+    [(nb.float64[:], nb.complex128[:, :], nb.complex128[:], nb.float64[:], nb.float64[:], nb.float64[:])],
+    '(e),(m,e),(m),()->(),()',
+    nopython=True,
+    target=parallelOption,
+    cache=cachedOption,
+    fastmath=fastOption,
+)
+def _freqBeamformer_EigValProb_SpecificSteerVec_FullCSM(
+    eigVal,
+    eigVec,
+    steerVec,
+    signalLossNormalization,
+    result,
+    normalizeSteer,
+):
     # see bottom of information header of 'beamformerFreq' for information on which steps are taken, in order to gain speed improvements.
     nMics = eigVec.shape[0]
-    
+
     # get h^H * h for normalization
     helpNormalize = 0.0
     for cntMics in range(nMics):
         helpNormalize += steerVec[cntMics] * steerVec[cntMics].conjugate()
 
     # performing matrix-vector-multplication via spectral decomp. (see bottom of information header of 'beamformerFreq')
     scalarProdFullCSM = 0.0
     for cntEigVal in range(len(eigVal)):
         scalarProdFullCSMperEigVal = 0.0 + 0.0j
         for cntMics in range(nMics):
             scalarProdFullCSMperEigVal += eigVec[cntMics, cntEigVal].conjugate() * steerVec[cntMics]
-        scalarProdFullCSMAbsSquared = (scalarProdFullCSMperEigVal * scalarProdFullCSMperEigVal.conjugate()).real  
+        scalarProdFullCSMAbsSquared = (scalarProdFullCSMperEigVal * scalarProdFullCSMperEigVal.conjugate()).real
         scalarProdFullCSM += scalarProdFullCSMAbsSquared * eigVal[cntEigVal]
     normalizeSteer[0] = helpNormalize.real
     result[0] = scalarProdFullCSM * signalLossNormalization[0]
 
 
-@nb.guvectorize([(nb.float64[:], nb.complex128[:,:], nb.complex128[:], nb.float64[:], nb.float64[:], nb.float64[:])],
-                 '(e),(m,e),(m),()->(),()', nopython=True, target=parallelOption, cache=cachedOption, fastmath=fastOption)
-def _freqBeamformer_EigValProb_SpecificSteerVec_CsmRemovedDiag(eigVal, eigVec, steerVec, signalLossNormalization, result, normalizeSteer):
+@nb.guvectorize(
+    [(nb.float64[:], nb.complex128[:, :], nb.complex128[:], nb.float64[:], nb.float64[:], nb.float64[:])],
+    '(e),(m,e),(m),()->(),()',
+    nopython=True,
+    target=parallelOption,
+    cache=cachedOption,
+    fastmath=fastOption,
+)
+def _freqBeamformer_EigValProb_SpecificSteerVec_CsmRemovedDiag(
+    eigVal,
+    eigVec,
+    steerVec,
+    signalLossNormalization,
+    result,
+    normalizeSteer,
+):
     # see bottom of information header of 'beamformerFreq' for information on which steps are taken, in order to gain speed improvements.
     nMics = eigVec.shape[0]
-    
+
     # get h^H * h for normalization
     helpNormalize = 0.0
     for cntMics in range(nMics):
         helpNormalize += steerVec[cntMics] * steerVec[cntMics].conjugate()
 
     # performing matrix-vector-multplication via spectral decomp. (see bottom of information header of 'beamformerFreq')
     scalarProdReducedCSM = 0.0
     for cntEigVal in range(len(eigVal)):
         scalarProdFullCSMperEigVal = 0.0 + 0.0j
         scalarProdDiagCSMperEigVal = 0.0
         for cntMics in range(nMics):
             temp1 = eigVec[cntMics, cntEigVal].conjugate() * steerVec[cntMics]
             scalarProdFullCSMperEigVal += temp1
-            scalarProdDiagCSMperEigVal += (temp1 * temp1.conjugate()).real  
+            scalarProdDiagCSMperEigVal += (temp1 * temp1.conjugate()).real
         scalarProdFullCSMAbsSquared = (scalarProdFullCSMperEigVal * scalarProdFullCSMperEigVal.conjugate()).real
         scalarProdReducedCSM += (scalarProdFullCSMAbsSquared - scalarProdDiagCSMperEigVal) * eigVal[cntEigVal]
     normalizeSteer[0] = helpNormalize.real
     result[0] = scalarProdReducedCSM * signalLossNormalization[0]
 
-#%% Point - Spread - Function
+
+# %% Point - Spread - Function
 def calcPointSpreadFunction(steerVecType, distGridToArrayCenter, distGridToAllMics, waveNumber, indSource, dtype):
-    """ Calculates the Point-Spread-Functions. Use either a predefined steering vector 
+    r"""Calculates the Point-Spread-Functions. Use either a predefined steering vector
     formulation (see :ref:`Sarradj, 2012<Sarradj2012>`) or pass it your own steering vector.
 
     Parameters
     ----------
     steerVecType : (one of the following strings: 'classic' (I), 'inverse' (II), 'true level' (III), 'true location' (IV))
         One of the predefined formulations I - IV (see :ref:`Sarradj, 2012<Sarradj2012>`).
     distGridToArrayCenter : float64[nGridpoints]
         Distance of all gridpoints to the center of sensor array
     distGridToAllMics : float64[nGridpoints, nMics]
         Distance of all gridpoints to all sensors of array
     waveNumber : float64
         The free field wave number.
     indSource : a LIST of int (e.g. indSource=[5] is fine; indSource=5 doesn't work):
-        specifies which gridpoints should be assumed to be sources 
+        specifies which gridpoints should be assumed to be sources
         --> a seperate psf will be calculated for each source
     dtype : either 'float64' or 'float32'
         Determines the precision of the result. For big maps this could be worth downgrading.
 
     Returns
     -------
     Autopower spectrum PSF map : [nFreqs, nGridPoints, nSources]
-    
+
     Some Notes on the optimization of all subroutines
     -------------------------------------------------
     Reducing beamforming equation:
         Let the steering vector be h, than, using Linear Albegra, the PSF of a SourcePoint S would be
-        
+
         .. math:: B = h^H \\cdot (a_S \\cdot a_S^H) \\cdot h,
         with ^H meaning the complex conjugated transpose and a_s the transfer function from source to gridpoint.
-        The (...)-part equals the CSM that the source would produce via the chosen steering vec formulation. 
+        The (...)-part equals the CSM that the source would produce via the chosen steering vec formulation.
         Using (for example) tensor calculus, one can reduce the equation to:
-        
+
         .. math:: B = \\left| h^H \\cdot a_S \\right| ^ 2.
     Steering vector:
-        Theoretically the steering vector always includes the term "exp(distMicsGrid - distArrayCenterGrid)", but as the steering vector gets multplied with its complex conjugation in 
+        Theoretically the steering vector always includes the term "exp(distMicsGrid - distArrayCenterGrid)", but as the steering vector gets multplied with its complex conjugation in
         all beamformer routines, the constant "distArrayCenterGrid" cancels out --> In order to save operations, it is not implemented.
     Squares:
         Seemingly "a * a" is slightly faster than "a**2" in numba
     Square of abs():
         Even though "a.real**2 + a.imag**^2" would have fewer operations, modern processors seem to be optimized for "a * a.conj" and are slightly faster the latter way.
         Both Versions are much faster than "abs(a)**2".
+
     """
     # get the steering vector formulation
-    psfDict = {'classic' : _psf_Formulation1AkaClassic,
-               'inverse' : _psf_Formulation2AkaInverse,
-               'true level' : _psf_Formulation3AkaTrueLevel,
-               'true location' : _psf_Formulation4AkaTrueLocation}
+    psfDict = {
+        'classic': _psf_Formulation1AkaClassic,
+        'inverse': _psf_Formulation2AkaInverse,
+        'true level': _psf_Formulation3AkaTrueLevel,
+        'true location': _psf_Formulation4AkaTrueLocation,
+    }
     coreFunc = psfDict[steerVecType]
 
     # prepare input
     nGridPoints = distGridToAllMics.shape[0]
     nSources = len(indSource)
-    if not isinstance(waveNumber, np.ndarray): waveNumber = np.array([waveNumber])
-    
+    if not isinstance(waveNumber, np.ndarray):
+        waveNumber = np.array([waveNumber])
+
     # psf routine: parallelized over Gridpoints
     psfOutput = np.zeros((nGridPoints, nSources), dtype=dtype)
-    coreFunc(distGridToArrayCenter, 
-             distGridToAllMics, 
-             distGridToArrayCenter[indSource], 
-             distGridToAllMics[indSource, :], 
-             waveNumber, 
-             psfOutput)
+    coreFunc(
+        distGridToArrayCenter,
+        distGridToAllMics,
+        distGridToArrayCenter[indSource],
+        distGridToAllMics[indSource, :],
+        waveNumber,
+        psfOutput,
+    )
 
     return psfOutput
 
 
-@nb.guvectorize([(nb.float64[:], nb.float64[:], nb.float64[:], nb.float64[:,:], nb.float64[:], nb.float64[:]),
-                 (nb.float64[:], nb.float64[:], nb.float64[:], nb.float64[:,:], nb.float64[:], nb.float32[:])],
-                 '(),(m),(s),(s,m),()->(s)', nopython=True, target=parallelOption, cache=cachedOption, fastmath=fastOption)
-def _psf_Formulation1AkaClassic(distGridToArrayCenter, distGridToAllMics, distSourcesToArrayCenter, distSourcesToAllMics, waveNumber, result):
+@nb.guvectorize(
+    [
+        (nb.float64[:], nb.float64[:], nb.float64[:], nb.float64[:, :], nb.float64[:], nb.float64[:]),
+        (nb.float64[:], nb.float64[:], nb.float64[:], nb.float64[:, :], nb.float64[:], nb.float32[:]),
+    ],
+    '(),(m),(s),(s,m),()->(s)',
+    nopython=True,
+    target=parallelOption,
+    cache=cachedOption,
+    fastmath=fastOption,
+)
+def _psf_Formulation1AkaClassic(
+    distGridToArrayCenter,
+    distGridToAllMics,
+    distSourcesToArrayCenter,
+    distSourcesToAllMics,
+    waveNumber,
+    result,
+):  # noqa ARG001
     nMics = distGridToAllMics.shape[0]
     for cntSources in range(len(distSourcesToArrayCenter)):
         # see bottom of information header of 'calcPointSpreadFunction' for infos on the PSF calculation and speed improvements.
         scalarProd = 0.0 + 0.0j
         for cntMics in range(nMics):
-            expArg = np.float32(waveNumber[0] * (distGridToAllMics[cntMics] - distSourcesToAllMics[cntSources, cntMics]))
+            expArg = np.float32(
+                waveNumber[0] * (distGridToAllMics[cntMics] - distSourcesToAllMics[cntSources, cntMics]),
+            )
             scalarProd += (np.cos(expArg) - 1j * np.sin(expArg)) / distSourcesToAllMics[cntSources, cntMics]
         normalizeFactor = distSourcesToArrayCenter[cntSources] / nMics
         scalarProdAbsSquared = (scalarProd * scalarProd.conjugate()).real
         result[cntSources] = scalarProdAbsSquared * (normalizeFactor * normalizeFactor)
 
 
-@nb.guvectorize([(nb.float64[:], nb.float64[:], nb.float64[:], nb.float64[:,:], nb.float64[:], nb.float64[:]),
-                 (nb.float64[:], nb.float64[:], nb.float64[:], nb.float64[:,:], nb.float64[:], nb.float32[:])],
-                 '(),(m),(s),(s,m),()->(s)', nopython=True, target=parallelOption, cache=cachedOption, fastmath=fastOption)
-def _psf_Formulation2AkaInverse(distGridToArrayCenter, distGridToAllMics, distSourcesToArrayCenter, distSourcesToAllMics, waveNumber, result):
+@nb.guvectorize(
+    [
+        (nb.float64[:], nb.float64[:], nb.float64[:], nb.float64[:, :], nb.float64[:], nb.float64[:]),
+        (nb.float64[:], nb.float64[:], nb.float64[:], nb.float64[:, :], nb.float64[:], nb.float32[:]),
+    ],
+    '(),(m),(s),(s,m),()->(s)',
+    nopython=True,
+    target=parallelOption,
+    cache=cachedOption,
+    fastmath=fastOption,
+)
+def _psf_Formulation2AkaInverse(
+    distGridToArrayCenter,
+    distGridToAllMics,
+    distSourcesToArrayCenter,
+    distSourcesToAllMics,
+    waveNumber,
+    result,
+):
     nMics = distGridToAllMics.shape[0]
     for cntSources in range(len(distSourcesToArrayCenter)):
         # see bottom of information header of 'calcPointSpreadFunction' for infos on the PSF calculation and speed improvements.
         scalarProd = 0.0 + 0.0j
         for cntMics in range(nMics):
-            expArg = np.float32(waveNumber[0] * (distGridToAllMics[cntMics] - distSourcesToAllMics[cntSources, cntMics]))
-            scalarProd += (np.cos(expArg) - 1j * np.sin(expArg)) / distSourcesToAllMics[cntSources, cntMics] * distGridToAllMics[cntMics]
+            expArg = np.float32(
+                waveNumber[0] * (distGridToAllMics[cntMics] - distSourcesToAllMics[cntSources, cntMics]),
+            )
+            scalarProd += (
+                (np.cos(expArg) - 1j * np.sin(expArg))
+                / distSourcesToAllMics[cntSources, cntMics]
+                * distGridToAllMics[cntMics]
+            )
         normalizeFactor = distSourcesToArrayCenter[cntSources] / distGridToArrayCenter[0] / nMics
-        scalarProdAbsSquared = (scalarProd * scalarProd.conjugate()).real  
-        result[cntSources] = scalarProdAbsSquared * (normalizeFactor * normalizeFactor)  
+        scalarProdAbsSquared = (scalarProd * scalarProd.conjugate()).real
+        result[cntSources] = scalarProdAbsSquared * (normalizeFactor * normalizeFactor)
 
 
-@nb.guvectorize([(nb.float64[:], nb.float64[:], nb.float64[:], nb.float64[:,:], nb.float64[:], nb.float64[:]),
-                 (nb.float64[:], nb.float64[:], nb.float64[:], nb.float64[:,:], nb.float64[:], nb.float32[:])],
-                 '(),(m),(s),(s,m),()->(s)', nopython=True, target=parallelOption, cache=cachedOption, fastmath=fastOption)
-def _psf_Formulation3AkaTrueLevel(distGridToArrayCenter, distGridToAllMics, distSourcesToArrayCenter, distSourcesToAllMics, waveNumber, result):
+@nb.guvectorize(
+    [
+        (nb.float64[:], nb.float64[:], nb.float64[:], nb.float64[:, :], nb.float64[:], nb.float64[:]),
+        (nb.float64[:], nb.float64[:], nb.float64[:], nb.float64[:, :], nb.float64[:], nb.float32[:]),
+    ],
+    '(),(m),(s),(s,m),()->(s)',
+    nopython=True,
+    target=parallelOption,
+    cache=cachedOption,
+    fastmath=fastOption,
+)
+def _psf_Formulation3AkaTrueLevel(
+    distGridToArrayCenter,
+    distGridToAllMics,
+    distSourcesToArrayCenter,
+    distSourcesToAllMics,
+    waveNumber,
+    result,
+):
     nMics = distGridToAllMics.shape[0]
     for cntSources in range(len(distSourcesToArrayCenter)):
         # see bottom of information header of 'calcPointSpreadFunction' for infos on the PSF calculation and speed improvements.
         scalarProd = 0.0 + 0.0j
         helpNormalizeGrid = 0.0
         for cntMics in range(nMics):
-            expArg = np.float32(waveNumber[0] * (distGridToAllMics[cntMics] - distSourcesToAllMics[cntSources, cntMics]))
-            scalarProd += (np.cos(expArg) - 1j * np.sin(expArg)) / distSourcesToAllMics[cntSources, cntMics] / distGridToAllMics[cntMics]
+            expArg = np.float32(
+                waveNumber[0] * (distGridToAllMics[cntMics] - distSourcesToAllMics[cntSources, cntMics]),
+            )
+            scalarProd += (
+                (np.cos(expArg) - 1j * np.sin(expArg))
+                / distSourcesToAllMics[cntSources, cntMics]
+                / distGridToAllMics[cntMics]
+            )
             helpNormalizeGrid += 1.0 / (distGridToAllMics[cntMics] * distGridToAllMics[cntMics])
         normalizeFactor = distSourcesToArrayCenter[cntSources] / distGridToArrayCenter[0] / helpNormalizeGrid
         scalarProdAbsSquared = (scalarProd * scalarProd.conjugate()).real
         result[cntSources] = scalarProdAbsSquared * (normalizeFactor * normalizeFactor)
 
 
-@nb.guvectorize([(nb.float64[:], nb.float64[:], nb.float64[:], nb.float64[:,:], nb.float64[:], nb.float64[:]),
-                 (nb.float64[:], nb.float64[:], nb.float64[:], nb.float64[:,:], nb.float64[:], nb.float32[:])],
-                 '(),(m),(s),(s,m),()->(s)', nopython=True, target=parallelOption, cache=cachedOption, fastmath=fastOption)
-def _psf_Formulation4AkaTrueLocation(distGridToArrayCenter, distGridToAllMics, distSourcesToArrayCenter, distSourcesToAllMics, waveNumber, result):
+@nb.guvectorize(
+    [
+        (nb.float64[:], nb.float64[:], nb.float64[:], nb.float64[:, :], nb.float64[:], nb.float64[:]),
+        (nb.float64[:], nb.float64[:], nb.float64[:], nb.float64[:, :], nb.float64[:], nb.float32[:]),
+    ],
+    '(),(m),(s),(s,m),()->(s)',
+    nopython=True,
+    target=parallelOption,
+    cache=cachedOption,
+    fastmath=fastOption,
+)
+def _psf_Formulation4AkaTrueLocation(
+    distGridToArrayCenter,
+    distGridToAllMics,
+    distSourcesToArrayCenter,
+    distSourcesToAllMics,
+    waveNumber,
+    result,
+):  # noqa ARG001
     nMics = distGridToAllMics.shape[0]
     for cntSources in range(len(distSourcesToArrayCenter)):
         # see bottom of information header of 'calcPointSpreadFunction' for infos on the PSF calculation and speed improvements.
         scalarProd = 0.0 + 0.0j
         helpNormalizeGrid = 0.0
         for cntMics in range(nMics):
-            expArg = np.float32(waveNumber[0] * (distGridToAllMics[cntMics] - distSourcesToAllMics[cntSources, cntMics]))
-            scalarProd += (np.cos(expArg) - 1j * np.sin(expArg)) / distSourcesToAllMics[cntSources, cntMics] / distGridToAllMics[cntMics]
+            expArg = np.float32(
+                waveNumber[0] * (distGridToAllMics[cntMics] - distSourcesToAllMics[cntSources, cntMics]),
+            )
+            scalarProd += (
+                (np.cos(expArg) - 1j * np.sin(expArg))
+                / distSourcesToAllMics[cntSources, cntMics]
+                / distGridToAllMics[cntMics]
+            )
             helpNormalizeGrid += 1.0 / (distGridToAllMics[cntMics] * distGridToAllMics[cntMics])
         normalizeFactor = distSourcesToArrayCenter[cntSources]
         scalarProdAbsSquared = (scalarProd * scalarProd.conjugate()).real
         result[cntSources] = scalarProdAbsSquared * (normalizeFactor * normalizeFactor) / nMics / helpNormalizeGrid
 
+
 # CURRENTLY NOT NEEDED, AS CUSTOM PSF WILL BE CALCULATED IN fbeamform.SteeringVector WITH THE USE OF Trait transfer
-#@nb.guvectorize([(nb.float64[:], nb.float64[:], nb.float64[:], nb.float64[:,:], nb.float64[:], nb.float64[:]),
+# @nb.guvectorize([(nb.float64[:], nb.float64[:], nb.float64[:], nb.float64[:,:], nb.float64[:], nb.float64[:]),
 #                 (nb.float64[:], nb.float64[:], nb.float64[:], nb.float64[:,:], nb.float64[:], nb.float32[:])],
 #                 '(),(m),(s),(s,m),()->(s)', nopython=True, target=parallelOption, cache=cachedOption)
-#def _psf_SpecificSteerVec(steerVec, steerVecSources, result):
+# def _psf_SpecificSteerVec(steerVec, steerVecSources, result):
 #    nMics = len(steerVec)
 #    for cntSources in range(steerVecSources.shape[0]):
 #        # see bottom of information header of 'calcPointSpreadFunction' for infos on the PSF calculation and speed improvements.
 #        scalarProd = 0.0 + 0.0j
 #        for cntMics in range(nMics):
 #            scalarProd += steerVec[cntMics].conjugate() * steerVecSources[cntSources, cntMics]
-#        scalarProdAbsSquared = (scalarProd * scalarProd.conjugate()).real  
+#        scalarProdAbsSquared = (scalarProd * scalarProd.conjugate()).real
 #        result[cntSources] = scalarProdAbsSquared
 
 
-#%% Damas - Gauss Seidel
+# %% Damas - Gauss Seidel
 # Formerly known as 'gseidel'
-@nb.guvectorize([#(nb.float32[:,:], nb.float32[:], nb.int64[:], nb.float64[:], nb.float32[:]), 
-                 (nb.float64[:,:], nb.float64[:], nb.int64[:], nb.float64[:], nb.float64[:]),
-                 #(nb.float32[:,:], nb.float64[:], nb.int64[:], nb.float64[:], nb.float64[:]),
-                 #(nb.float64[:,:], nb.float32[:], nb.int64[:], nb.float64[:], nb.float32[:])
-                 ], 
-                 '(g,g),(g),(),()->(g)', nopython=True, target=parallelOption, cache=cachedOption, fastmath=fastOption)
+@nb.guvectorize(
+    [  # (nb.float32[:,:], nb.float32[:], nb.int64[:], nb.float64[:], nb.float32[:]),
+        (nb.float64[:, :], nb.float64[:], nb.int64[:], nb.float64[:], nb.float64[:]),
+        # (nb.float32[:,:], nb.float64[:], nb.int64[:], nb.float64[:], nb.float64[:]),
+        # (nb.float64[:,:], nb.float32[:], nb.int64[:], nb.float64[:], nb.float32[:])
+    ],
+    '(g,g),(g),(),()->(g)',
+    nopython=True,
+    target=parallelOption,
+    cache=cachedOption,
+    fastmath=fastOption,
+)
 def damasSolverGaussSeidel(A, dirtyMap, nIterations, relax, damasSolution):
-    """ Solves the DAMAS inverse problem via modified gauss seidel.
+    """Solves the DAMAS inverse problem via modified gauss seidel.
     This is the original formulation from :ref:`Brooks and Humphreys, 2006<BrooksHumphreys2006>`.
-    
+
     Parameters
     ----------
     A : float32/float64[nFreqs, nGridpoints, nGridpoints] (or float64[...])
         The PSF build matrix (see :ref:`Brooks and Humphreys, 2006<BrooksHumphreys2006>`)
     dirtyMap : float32/float64[nFreqs, nGridpoints] (or float64[...])
         The conventional beamformer map
-    nIterations : int64[scalar] 
+    nIterations : int64[scalar]
         number of Iterations the damas solver has to go through
-    relax : int64[scalar] 
+    relax : int64[scalar]
         relaxation parameter (=1.0 in :ref:`Brooks and Humphreys, 2006<BrooksHumphreys2006>`)
-    damasSolution : float32/float64[nFreqs, nGridpoints] (or float64[...]) 
+    damasSolution : float32/float64[nFreqs, nGridpoints] (or float64[...])
         starting solution
-    
+
     Returns
     -------
     None : as damasSolution is overwritten with end result of the damas iterative solver.
+
     """
-#    nGridPoints = len(dirtyMap)
-#    for cntIter in range(nIterations[0]):
-#        for cntGrid in range(nGridPoints):
-#            solHelp = np.float32(0)
-#            for cntGridHelp in range(cntGrid):  # lower sum
-#                solHelp += A[cntGrid, cntGridHelp] * damasSolution[cntGridHelp]
-#            for cntGridHelp in range(cntGrid + 1, nGridPoints):  # upper sum
-#                solHelp += A[cntGrid, cntGridHelp] * damasSolution[cntGridHelp]
-#            solHelp = (1 - relax[0]) * damasSolution[cntGrid] + relax[0] * (dirtyMap[cntGrid] - solHelp)
-#            if solHelp > 0.0:
-#                damasSolution[cntGrid] = solHelp
-#            else:
-#                damasSolution[cntGrid] = 0.0
+    #    nGridPoints = len(dirtyMap)
+    #    for cntIter in range(nIterations[0]):
+    #        for cntGrid in range(nGridPoints):
+    #            solHelp = np.float32(0)
+    #            for cntGridHelp in range(cntGrid):  # lower sum
+    #                solHelp += A[cntGrid, cntGridHelp] * damasSolution[cntGridHelp]
+    #            for cntGridHelp in range(cntGrid + 1, nGridPoints):  # upper sum
+    #                solHelp += A[cntGrid, cntGridHelp] * damasSolution[cntGridHelp]
+    #            solHelp = (1 - relax[0]) * damasSolution[cntGrid] + relax[0] * (dirtyMap[cntGrid] - solHelp)
+    #            if solHelp > 0.0:
+    #                damasSolution[cntGrid] = solHelp
+    #            else:
+    #                damasSolution[cntGrid] = 0.0
     nGridPoints = len(dirtyMap)
-    for cntIter in range(nIterations[0]):
+    for _cntIter in range(nIterations[0]):
         for cntGrid in range(nGridPoints):
             solHelp = 0.0
             for cntGridHelp in range(nGridPoints):  # full sum
                 solHelp += A[cntGrid, cntGridHelp] * damasSolution[cntGridHelp]
             solHelp -= A[cntGrid, cntGrid] * damasSolution[cntGrid]
             solHelp = (1 - relax[0]) * damasSolution[cntGrid] + relax[0] * (dirtyMap[cntGrid] - solHelp)
             if solHelp > 0.0:
                 damasSolution[cntGrid] = solHelp
             else:
                 damasSolution[cntGrid] = 0.0
 
 
-#%% Transfer - Function
+# %% Transfer - Function
 def calcTransfer(distGridToArrayCenter, distGridToAllMics, waveNumber):
-    """ Calculates the transfer functions between the various mics and gridpoints.
-    
+    """Calculates the transfer functions between the various mics and gridpoints.
+
     Parameters
     ----------
     distGridToArrayCenter : float64[nGridpoints]
         Distance of all gridpoints to the center of sensor array
     distGridToAllMics : float64[nGridpoints, nMics]
         Distance of all gridpoints to all sensors of array
     waveNumber : complex128
         The wave number should be stored in the imag-part
 
     Returns
     -------
     The Transferfunctions in format complex128[nGridPoints, nMics].
+
     """
     nGridPoints, nMics = distGridToAllMics.shape[0], distGridToAllMics.shape[1]
     result = np.zeros((nGridPoints, nMics), np.complex128)
     # transfer routine: parallelized over Gridpoints
     _transferCoreFunc(distGridToArrayCenter, distGridToAllMics, np.array([waveNumber]), result)
     return result
 
-@nb.guvectorize([(nb.float64[:], nb.float64[:], nb.float64[:], nb.complex128[:])], '(),(m),()->(m)', 
-                nopython=True, target=parallelOption, cache=cachedOption, fastmath=fastOption)
+
+@nb.guvectorize(
+    [(nb.float64[:], nb.float64[:], nb.float64[:], nb.complex128[:])],
+    '(),(m),()->(m)',
+    nopython=True,
+    target=parallelOption,
+    cache=cachedOption,
+    fastmath=fastOption,
+)
 def _transferCoreFunc(distGridToArrayCenter, distGridToAllMics, waveNumber, result):
     nMics = distGridToAllMics.shape[0]
     for cntMics in range(nMics):
         expArg = np.float32(waveNumber[0] * (distGridToAllMics[cntMics] - distGridToArrayCenter[0]))
         result[cntMics] = (np.cos(expArg) - 1j * np.sin(expArg)) * distGridToArrayCenter[0] / distGridToAllMics[cntMics]
-
```

### Comparing `acoular-24.3/acoular/fbeamform.py` & `acoular-24.5/acoular/fbeamform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-# -*- coding: utf-8 -*-
-#pylint: disable-msg=E0611, E1101, C0103, R0901, R0902, R0903, R0904, W0232
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 # Copyright (c) Acoular Development Team.
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 """Implements beamformers in the frequency domain.
 
 .. autosummary::
     :toctree: generated/
-    
+
     SteeringVector
 
-    
+
     BeamformerBase
     BeamformerFunctional
     BeamformerCapon
     BeamformerEig
     BeamformerMusic
     BeamformerClean
     BeamformerDamas
@@ -30,2708 +28,2766 @@
     PointSpreadFunction
     L_p
     integrate
 
 """
 
 # imports from other packages
-from __future__ import print_function, division
 
 import warnings
+from warnings import warn
 
-from numpy import array, ones, full, \
-invert, dot, newaxis, zeros, linalg, \
-searchsorted, pi, sign, diag, arange, sqrt, log10, \
-reshape, hstack, vstack, eye, tril, size, clip, tile, round, delete, \
-absolute, argsort, sum, hsplit, fill_diagonal, zeros_like, \
-einsum, ndarray, isscalar, inf, real, unique, atleast_2d, einsum_path,trace
-
-from numpy.linalg import norm
-
-from sklearn.linear_model import LassoLars, LassoLarsCV, LassoLarsIC,\
-OrthogonalMatchingPursuitCV, LinearRegression
-
-#check for sklearn version to account for incompatible behavior
+# check for sklearn version to account for incompatible behavior
 import sklearn
+from numpy import (
+    absolute,
+    arange,
+    argsort,
+    array,
+    atleast_2d,
+    clip,
+    delete,
+    diag,
+    dot,
+    einsum,
+    einsum_path,
+    eye,
+    fill_diagonal,
+    full,
+    hsplit,
+    hstack,
+    inf,
+    invert,
+    isscalar,
+    linalg,
+    log10,
+    ndarray,
+    newaxis,
+    ones,
+    pi,
+    real,
+    reshape,
+    round,
+    searchsorted,
+    sign,
+    size,
+    sqrt,
+    sum,
+    tile,
+    trace,
+    tril,
+    unique,
+    vstack,
+    zeros,
+    zeros_like,
+)
+from numpy.linalg import norm
 from packaging.version import parse
-sklearn_ndict = {}
-if parse(sklearn.__version__)<parse('1.4'):
-    sklearn_ndict['normalize'] = False
-
-from scipy.optimize import nnls, linprog, fmin_l_bfgs_b, shgo
-from scipy.linalg import inv, eigh, eigvals, fractional_matrix_power
-from warnings import warn
-
-#pylops imports for CMF solvers
-try:
-    from  pylops import Identity, MatrixMult
-    from pylops.optimization.sparsity import SplitBregman,FISTA
-    PYLOPS_TRUE = True
-except:
-    PYLOPS_TRUE = False
-
-from traits.api import HasPrivateTraits, Float, Int, \
-CArray, Property, Instance, Trait, Bool, Range, Delegate, Enum, Any, \
-cached_property, on_trait_change, property_depends_on, List, Tuple, Dict
+from scipy.linalg import eigh, eigvals, fractional_matrix_power, inv
+from scipy.optimize import fmin_l_bfgs_b, linprog, nnls, shgo
+from sklearn.linear_model import LassoLars, LassoLarsCV, LassoLarsIC, LinearRegression, OrthogonalMatchingPursuitCV
+from traits.api import (
+    Any,
+    Bool,
+    CArray,
+    Delegate,
+    Dict,
+    Enum,
+    Float,
+    HasPrivateTraits,
+    Instance,
+    Int,
+    List,
+    Property,
+    Range,
+    Trait,
+    Tuple,
+    cached_property,
+    on_trait_change,
+    property_depends_on,
+)
 from traits.trait_errors import TraitError
 
-from .fastFuncs import beamformerFreq, calcTransfer, calcPointSpreadFunction, \
-damasSolverGaussSeidel
-
+from .configuration import config
+from .environments import Environment
+from .fastFuncs import beamformerFreq, calcPointSpreadFunction, calcTransfer, damasSolverGaussSeidel
+from .grids import Grid, Sector
 from .h5cache import H5cache
 from .h5files import H5CacheFileBase
 from .internal import digest
-from .grids import Grid, Sector
 from .microphones import MicGeom
-from .configuration import config
-from .environments import Environment
 from .spectra import PowerSpectra
 
-class SteeringVector( HasPrivateTraits ):
-    """ 
-    Basic class for implementing steering vectors with monopole source transfer models
-    """
-    
+sklearn_ndict = {}
+if parse(sklearn.__version__) < parse('1.4'):
+    sklearn_ndict['normalize'] = False
+
+
+class SteeringVector(HasPrivateTraits):
+    """Basic class for implementing steering vectors with monopole source transfer models."""
+
     #: :class:`~acoular.grids.Grid`-derived object that provides the grid locations.
-    grid = Trait(Grid, 
-        desc="beamforming grid")
-    
+    grid = Trait(Grid, desc='beamforming grid')
+
     #: :class:`~acoular.microphones.MicGeom` object that provides the microphone locations.
-    mics = Trait(MicGeom, 
-        desc="microphone geometry")
-        
+    mics = Trait(MicGeom, desc='microphone geometry')
+
     #: Type of steering vectors, see also :ref:`Sarradj, 2012<Sarradj2012>`. Defaults to 'true level'.
-    steer_type = Trait('true level', 'true location', 'classic', 'inverse',
-                  desc="type of steering vectors used")
-    
-    #: :class:`~acoular.environments.Environment` or derived object, 
+    steer_type = Trait('true level', 'true location', 'classic', 'inverse', desc='type of steering vectors used')
+
+    #: :class:`~acoular.environments.Environment` or derived object,
     #: which provides information about the sound propagation in the medium.
     #: Defaults to standard :class:`~acoular.environments.Environment` object.
     env = Instance(Environment(), Environment)
-    
+
     # TODO: add caching capability for transfer function
-    # Flag, if "True" (not default), the transfer function is 
-    # cached in h5 files and does not have to be recomputed during subsequent 
-    # program runs. 
+    # Flag, if "True" (not default), the transfer function is
+    # cached in h5 files and does not have to be recomputed during subsequent
+    # program runs.
     # Be aware that setting this to "True" may result in high memory usage.
-    #cached = Bool(False, 
-    #              desc="cache flag for transfer function")    
-    
-    
-    # Sound travel distances from microphone array center to grid 
+    # cached = Bool(False,
+    #              desc="cache flag for transfer function")
+
+    # Sound travel distances from microphone array center to grid
     # points or reference position (readonly). Feature may change.
-    r0 = Property(desc="array center to grid distances")
+    r0 = Property(desc='array center to grid distances')
 
-    # Sound travel distances from array microphones to grid 
+    # Sound travel distances from array microphones to grid
     # points (readonly). Feature may change.
-    rm = Property(desc="all array mics to grid distances")
-    
+    rm = Property(desc='all array mics to grid distances')
+
     # mirror trait for ref
-    _ref = Any(array([0.,0.,0.]),
-               desc="reference position or distance")
-    
-    #: Reference position or distance at which to evaluate the sound pressure 
-    #: of a grid point. 
+    _ref = Any(array([0.0, 0.0, 0.0]), desc='reference position or distance')
+
+    #: Reference position or distance at which to evaluate the sound pressure
+    #: of a grid point.
     #: If set to a scalar, this is used as reference distance to the grid points.
     #: If set to a vector, this is interpreted as x,y,z coordinates of the reference position.
     #: Defaults to [0.,0.,0.].
-    ref = Property(desc="reference position or distance")
-    
-    def _set_ref (self, ref):
+    ref = Property(desc='reference position or distance')
+
+    def _set_ref(self, ref):
         if isscalar(ref):
             try:
                 self._ref = absolute(float(ref))
             except:
-                raise TraitError(args=self,
-                                 name='ref', 
-                                 info='Float or CArray(3,)',
-                                 value=ref) 
+                raise TraitError(args=self, name='ref', info='Float or CArray(3,)', value=ref)
         elif len(ref) == 3:
             self._ref = array(ref, dtype=float)
         else:
-            raise TraitError(args=self,
-                             name='ref', 
-                             info='Float or CArray(3,)',
-                             value=ref)
-      
-    def _get_ref (self):
+            raise TraitError(args=self, name='ref', info='Float or CArray(3,)', value=ref)
+
+    def _get_ref(self):
         return self._ref
-    
-    
+
     # internal identifier
-    digest = Property( 
-        depends_on = ['steer_type', 'env.digest', 'grid.digest', 'mics.digest', '_ref'])
-    
+    digest = Property(depends_on=['steer_type', 'env.digest', 'grid.digest', 'mics.digest', '_ref'])
+
     # internal identifier, use for inverse methods, excluding steering vector type
-    inv_digest = Property( 
-        depends_on = ['env.digest', 'grid.digest', 'mics.digest', '_ref'])
-        
+    inv_digest = Property(depends_on=['env.digest', 'grid.digest', 'mics.digest', '_ref'])
+
     @property_depends_on('grid.digest, env.digest, _ref')
-    def _get_r0 ( self ):
+    def _get_r0(self):
         if isscalar(self.ref):
             if self.ref > 0:
                 return full((self.grid.size,), self.ref)
-            else:
-                return self.env._r(self.grid.pos())
-        else:
-            return self.env._r(self.grid.pos(), self.ref[:,newaxis])
+            return self.env._r(self.grid.pos())
+        return self.env._r(self.grid.pos(), self.ref[:, newaxis])
 
     @property_depends_on('grid.digest, mics.digest, env.digest')
-    def _get_rm ( self ):
+    def _get_rm(self):
         return atleast_2d(self.env._r(self.grid.pos(), self.mics.mpos))
- 
+
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
-    
+    def _get_digest(self):
+        return digest(self)
+
     @cached_property
-    def _get_inv_digest( self ):
-        return digest( self )
-    
+    def _get_inv_digest(self):
+        return digest(self)
+
     def transfer(self, f, ind=None):
-        """
-        Calculates the transfer matrix for one frequency. 
-        
+        """Calculates the transfer matrix for one frequency.
+
         Parameters
         ----------
         f   : float
             Frequency for which to calculate the transfer matrix
         ind : (optional) array of ints
-            If set, only the transfer function of the gridpoints addressed by 
+            If set, only the transfer function of the gridpoints addressed by
             the given indices will be calculated. Useful for algorithms like CLEAN-SC,
             where not the full transfer matrix is needed
-        
+
         Returns
         -------
         array of complex128
             array of shape (ngridpts, nmics) containing the transfer matrix for the given frequency
+
         """
-        #if self.cached:
+        # if self.cached:
         #    warn('Caching of transfer function is not yet supported!', Warning)
         #    self.cached = False
-        
+
         if ind is None:
-            trans = calcTransfer(self.r0, self.rm, array(2*pi*f/self.env.c))
-        elif not isinstance(ind,ndarray):
-            trans = calcTransfer(self.r0[ind], self.rm[ind, :][newaxis], array(2*pi*f/self.env.c))#[0, :]
+            trans = calcTransfer(self.r0, self.rm, array(2 * pi * f / self.env.c))
+        elif not isinstance(ind, ndarray):
+            trans = calcTransfer(self.r0[ind], self.rm[ind, :][newaxis], array(2 * pi * f / self.env.c))  # [0, :]
         else:
-            trans = calcTransfer(self.r0[ind], self.rm[ind, :], array(2*pi*f/self.env.c))
+            trans = calcTransfer(self.r0[ind], self.rm[ind, :], array(2 * pi * f / self.env.c))
         return trans
-    
+
     def steer_vector(self, f, ind=None):
-        """
-        Calculates the steering vectors based on the transfer function
+        """Calculates the steering vectors based on the transfer function
         See also :ref:`Sarradj, 2012<Sarradj2012>`.
-        
+
         Parameters
         ----------
         f   : float
             Frequency for which to calculate the transfer matrix
         ind : (optional) array of ints
-            If set, only the steering vectors of the gridpoints addressed by 
+            If set, only the steering vectors of the gridpoints addressed by
             the given indices will be calculated. Useful for algorithms like CLEAN-SC,
             where not the full transfer matrix is needed
-        
+
         Returns
         -------
         array of complex128
             array of shape (ngridpts, nmics) containing the steering vectors for the given frequency
+
         """
-        func = {'classic' : lambda x: x / absolute(x) / x.shape[-1],
-                'inverse' : lambda x: 1. / x.conj() / x.shape[-1],
-                'true level' : lambda x: x / einsum('ij,ij->i',x,x.conj())[:,newaxis],
-                'true location' : lambda x: x / sqrt(einsum('ij,ij->i',x,x.conj()) * x.shape[-1])[:,newaxis]
-                }[self.steer_type]
+        func = {
+            'classic': lambda x: x / absolute(x) / x.shape[-1],
+            'inverse': lambda x: 1.0 / x.conj() / x.shape[-1],
+            'true level': lambda x: x / einsum('ij,ij->i', x, x.conj())[:, newaxis],
+            'true location': lambda x: x / sqrt(einsum('ij,ij->i', x, x.conj()) * x.shape[-1])[:, newaxis],
+        }[self.steer_type]
         return func(self.transfer(f, ind))
-    
-    
-class BeamformerBase( HasPrivateTraits ):
-    """
-    Beamforming using the basic delay-and-sum algorithm in the frequency domain.
-    """
-    
-    
+
+
+class BeamformerBase(HasPrivateTraits):
+    """Beamforming using the basic delay-and-sum algorithm in the frequency domain."""
+
     # Instance of :class:`~acoular.fbeamform.SteeringVector` or its derived classes
     # that contains information about the steering vector. This is a private trait.
     # Do not set this directly, use `steer` trait instead.
-    _steer_obj = Instance(SteeringVector(), SteeringVector)   
-    
-    #: :class:`~acoular.fbeamform.SteeringVector` or derived object. 
+    _steer_obj = Instance(SteeringVector(), SteeringVector)
+
+    #: :class:`~acoular.fbeamform.SteeringVector` or derived object.
     #: Defaults to :class:`~acoular.fbeamform.SteeringVector` object.
-    steer = Property(desc="steering vector object")  
-    
+    steer = Property(desc='steering vector object')
+
     def _get_steer(self):
         return self._steer_obj
-    
+
     def _set_steer(self, steer):
         if isinstance(steer, SteeringVector):
             self._steer_obj = steer
         elif steer in ('true level', 'true location', 'classic', 'inverse'):
             # Type of steering vectors, see also :ref:`Sarradj, 2012<Sarradj2012>`.
-            warn("Deprecated use of 'steer' trait. "
-                 "Please use object of class 'SteeringVector' in the future.", 
-                 Warning, stacklevel = 2)
+            warn(
+                "Deprecated use of 'steer' trait. Please use object of class 'SteeringVector' in the future.",
+                Warning,
+                stacklevel=2,
+            )
             self._steer_obj.steer_type = steer
         else:
-            raise(TraitError(args=self,
-                             name='steer', 
-                             info='SteeringVector',
-                             value=steer))
+            raise (TraitError(args=self, name='steer', info='SteeringVector', value=steer))
 
     # --- List of backwards compatibility traits and their setters/getters -----------
-    
-    # :class:`~acoular.environments.Environment` or derived object. 
-    # Deprecated! Only kept for backwards compatibility. 
+
+    # :class:`~acoular.environments.Environment` or derived object.
+    # Deprecated! Only kept for backwards compatibility.
     # Now governed by :attr:`steer` trait.
     env = Property()
-    
+
     def _get_env(self):
-        return self._steer_obj.env    
-    
+        return self._steer_obj.env
+
     def _set_env(self, env):
-        warn("Deprecated use of 'env' trait. ", Warning, stacklevel = 2)
+        warn("Deprecated use of 'env' trait. ", Warning, stacklevel=2)
         self._steer_obj.env = env
-    
+
     # The speed of sound.
-    # Deprecated! Only kept for backwards compatibility. 
+    # Deprecated! Only kept for backwards compatibility.
     # Now governed by :attr:`steer` trait.
     c = Property()
-    
+
     def _get_c(self):
         return self._steer_obj.env.c
-    
+
     def _set_c(self, c):
-        warn("Deprecated use of 'c' trait. ", Warning, stacklevel = 2)
+        warn("Deprecated use of 'c' trait. ", Warning, stacklevel=2)
         self._steer_obj.env.c = c
-   
+
     # :class:`~acoular.grids.Grid`-derived object that provides the grid locations.
-    # Deprecated! Only kept for backwards compatibility. 
+    # Deprecated! Only kept for backwards compatibility.
     # Now governed by :attr:`steer` trait.
     grid = Property()
 
     def _get_grid(self):
         return self._steer_obj.grid
-    
+
     def _set_grid(self, grid):
-        warn("Deprecated use of 'grid' trait. ", Warning, stacklevel = 2)
+        warn("Deprecated use of 'grid' trait. ", Warning, stacklevel=2)
         self._steer_obj.grid = grid
-    
+
     # :class:`~acoular.microphones.MicGeom` object that provides the microphone locations.
-    # Deprecated! Only kept for backwards compatibility. 
+    # Deprecated! Only kept for backwards compatibility.
     # Now governed by :attr:`steer` trait
     mpos = Property()
-    
+
     def _get_mpos(self):
         return self._steer_obj.mics
-    
+
     def _set_mpos(self, mpos):
-        warn("Deprecated use of 'mpos' trait. ", Warning, stacklevel = 2)
+        warn("Deprecated use of 'mpos' trait. ", Warning, stacklevel=2)
         self._steer_obj.mics = mpos
-    
-    
+
     # Sound travel distances from microphone array center to grid points (r0)
     # and all array mics to grid points (rm). Readonly.
-    # Deprecated! Only kept for backwards compatibility. 
+    # Deprecated! Only kept for backwards compatibility.
     # Now governed by :attr:`steer` trait
     r0 = Property()
+
     def _get_r0(self):
         return self._steer_obj.r0
-    
+
     rm = Property()
+
     def _get_rm(self):
         return self._steer_obj.rm
-    
+
     # --- End of backwards compatibility traits --------------------------------------
 
-    #: :class:`~acoular.spectra.PowerSpectra` object that provides the 
+    #: :class:`~acoular.spectra.PowerSpectra` object that provides the
     #: cross spectral matrix and eigenvalues
-    freq_data = Trait(PowerSpectra, 
-                      desc="freq data object")
+    freq_data = Trait(PowerSpectra, desc='freq data object')
 
     #: Boolean flag, if 'True' (default), the main diagonal is removed before beamforming.
-    r_diag = Bool(True, 
-                  desc="removal of diagonal")
-    
-    #: If r_diag==True: if r_diag_norm==0.0, the standard  
-    #: normalization = num_mics/(num_mics-1) is used. 
-    #: If r_diag_norm !=0.0, the user input is used instead.  
-    #: If r_diag==False, the normalization is 1.0 either way. 
-    r_diag_norm = Float(0.0, 
-                        desc="If diagonal of the csm is removed, some signal energy is lost." 
-                        "This is handled via this normalization factor." 
-                        "Internally, the default is: num_mics / (num_mics - 1).") 
-    
+    r_diag = Bool(True, desc='removal of diagonal')
+
+    #: If r_diag==True: if r_diag_norm==0.0, the standard
+    #: normalization = num_mics/(num_mics-1) is used.
+    #: If r_diag_norm !=0.0, the user input is used instead.
+    #: If r_diag==False, the normalization is 1.0 either way.
+    r_diag_norm = Float(
+        0.0,
+        desc='If diagonal of the csm is removed, some signal energy is lost.'
+        'This is handled via this normalization factor.'
+        'Internally, the default is: num_mics / (num_mics - 1).',
+    )
+
     #: Floating point precision of property result. Corresponding to numpy dtypes. Default = 64 Bit.
-    precision = Trait('float64', 'float32',
-            desc="precision (32/64 Bit) of result, corresponding to numpy dtypes")
-    
+    precision = Trait('float64', 'float32', desc='precision (32/64 Bit) of result, corresponding to numpy dtypes')
+
     #: Boolean flag, if 'True' (default), the result is cached in h5 files.
-    cached = Bool(True, 
-        desc="cached flag")
-                  
+    cached = Bool(True, desc='cached flag')
+
     # hdf5 cache file
-    h5f = Instance( H5CacheFileBase, transient = True )
-    
-    #: The beamforming result as squared sound pressure values 
+    h5f = Instance(H5CacheFileBase, transient=True)
+
+    #: The beamforming result as squared sound pressure values
     #: at all grid point locations (readonly).
     #: Returns a (number of frequencies, number of gridpoints) array of floats.
-    result = Property(
-        desc="beamforming result")
-    
+    result = Property(desc='beamforming result')
+
     # internal identifier
-    digest = Property( 
-        depends_on = ['freq_data.digest', 'r_diag', 'r_diag_norm', 'precision', '_steer_obj.digest'])
+    digest = Property(depends_on=['freq_data.digest', 'r_diag', 'r_diag_norm', 'precision', '_steer_obj.digest'])
 
     # internal identifier
-    ext_digest = Property( 
-        depends_on = ['digest', 'freq_data.ind_low', 'freq_data.ind_high'], 
-        )
+    ext_digest = Property(
+        depends_on=['digest', 'freq_data.ind_low', 'freq_data.ind_high'],
+    )
 
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
-    
+    def _get_digest(self):
+        return digest(self)
+
     @cached_property
-    def _get_ext_digest( self ):
-        return digest( self, 'ext_digest' )
-    
-    def _get_filecache( self ):
-        """
-        function collects cached results from file depending on 
-        global/local caching behaviour. Returns (None, None) if no cachefile/data 
+    def _get_ext_digest(self):
+        return digest(self, 'ext_digest')
+
+    def _get_filecache(self):
+        """Function collects cached results from file depending on
+        global/local caching behaviour. Returns (None, None) if no cachefile/data
         exist and global caching mode is 'readonly'.
         """
-#        print("get cachefile:", self.freq_data.basename)
-        H5cache.get_cache_file( self, self.freq_data.basename ) 
-        if not self.h5f: 
-#            print("no cachefile:", self.freq_data.basename)
-            return (None, None, None)# only happens in case of global caching readonly
+        #        print("get cachefile:", self.freq_data.basename)
+        H5cache.get_cache_file(self, self.freq_data.basename)
+        if not self.h5f:
+            #            print("no cachefile:", self.freq_data.basename)
+            return (None, None, None)  # only happens in case of global caching readonly
 
         nodename = self.__class__.__name__ + self.digest
-#        print("collect filecache for nodename:",nodename)
+        #        print("collect filecache for nodename:",nodename)
         if config.global_caching == 'overwrite' and self.h5f.is_cached(nodename):
-#            print("remove existing data for nodename",nodename)
-            self.h5f.remove_data(nodename) # remove old data before writing in overwrite mode
-        
+            #            print("remove existing data for nodename",nodename)
+            self.h5f.remove_data(nodename)  # remove old data before writing in overwrite mode
+
         if not self.h5f.is_cached(nodename):
-#            print("no data existent for nodename:", nodename)
-            if config.global_caching == 'readonly': 
+            #            print("no data existent for nodename:", nodename)
+            if config.global_caching == 'readonly':
                 return (None, None, None)
+            numfreq = self.freq_data.fftfreq().shape[0]  # block_size/2 + 1steer_obj
+            group = self.h5f.create_new_group(nodename)
+            self.h5f.create_compressible_array(
+                'freqs',
+                (numfreq,),
+                'int8',  #'bool',
+                group,
+            )
+            if isinstance(self, BeamformerAdaptiveGrid):
+                self.h5f.create_compressible_array('gpos', (3, self.size), 'float64', group)
+                self.h5f.create_compressible_array('result', (numfreq, self.size), self.precision, group)
             else:
-#                print("initialize data.")
-                numfreq = self.freq_data.fftfreq().shape[0]# block_size/2 + 1steer_obj
-                group = self.h5f.create_new_group(nodename)
-                self.h5f.create_compressible_array('freqs',
-                                      (numfreq, ),
-                                      'int8',#'bool', 
-                                      group)
-                if isinstance(self,BeamformerAdaptiveGrid):
-                    self.h5f.create_compressible_array('gpos',
-                                      (3, self.size),
-                                      'float64',
-                                      group)
-                    self.h5f.create_compressible_array('result',
-                                      (numfreq, self.size),
-                                      self.precision,
-                                      group)
-                else:
-                    self.h5f.create_compressible_array('result',
-                                      (numfreq, self.steer.grid.size),
-                                      self.precision,
-                                      group)
-
-        ac = self.h5f.get_data_by_reference('result','/'+nodename)
-        fr = self.h5f.get_data_by_reference('freqs','/'+nodename)
-        if isinstance(self,BeamformerAdaptiveGrid):
-            gpos = self.h5f.get_data_by_reference('gpos','/'+nodename)
+                self.h5f.create_compressible_array('result', (numfreq, self.steer.grid.size), self.precision, group)
+
+        ac = self.h5f.get_data_by_reference('result', '/' + nodename)
+        fr = self.h5f.get_data_by_reference('freqs', '/' + nodename)
+        if isinstance(self, BeamformerAdaptiveGrid):
+            gpos = self.h5f.get_data_by_reference('gpos', '/' + nodename)
         else:
             gpos = None
-        return (ac,fr,gpos)        
+        return (ac, fr, gpos)
 
     def _assert_equal_channels(self):
         numchannels = self.freq_data.numchannels
-        if  numchannels != self.steer.mics.num_mics or numchannels == 0:
-            raise ValueError("%i channels do not fit %i mics" % (numchannels, self.steer.mics.num_mics))        
+        if numchannels != self.steer.mics.num_mics or numchannels == 0:
+            raise ValueError('%i channels do not fit %i mics' % (numchannels, self.steer.mics.num_mics))
 
     @property_depends_on('ext_digest')
-    def _get_result ( self ):
-        """
-        This is the :attr:`result` getter routine.
+    def _get_result(self):
+        """Implements the :attr:`result` getter routine.
         The beamforming result is either loaded or calculated.
         """
         f = self.freq_data
-        numfreq = f.fftfreq().shape[0]# block_size/2 + 1steer_obj
+        numfreq = f.fftfreq().shape[0]  # block_size/2 + 1steer_obj
         _digest = ''
         while self.digest != _digest:
             _digest = self.digest
             self._assert_equal_channels()
             ac, fr = (None, None)
-            if not ( # if result caching is active
-                    config.global_caching == 'none' or 
-                    (config.global_caching == 'individual' and self.cached == False)
-                ):
-#                print("get filecache..")
-                (ac,fr,gpos) = self._get_filecache() 
+            if not (  # if result caching is active
+                config.global_caching == 'none' or (config.global_caching == 'individual' and not self.cached)
+            ):
+                #                print("get filecache..")
+                (ac, fr, gpos) = self._get_filecache()
                 if gpos:
                     self._gpos = gpos
-            if ac and fr: 
-#                    print("cached data existent")
-                if not fr[f.ind_low:f.ind_high].all():
-#                        print("calculate missing results")                            
-                    if config.global_caching == 'readonly': 
+            if ac and fr:
+                #                    print("cached data existent")
+                if not fr[f.ind_low : f.ind_high].all():
+                    #                        print("calculate missing results")
+                    if config.global_caching == 'readonly':
                         (ac, fr) = (ac[:], fr[:])
-                    self.calc(ac,fr)
+                    self.calc(ac, fr)
                     self.h5f.flush()
-#                    else:
-#                        print("cached results are complete! return.")
+            #                    else:
+            #                        print("cached results are complete! return.")
             else:
-#                print("no caching or not activated, calculate result")
-                if isinstance(self,BeamformerAdaptiveGrid):
+                #                print("no caching or not activated, calculate result")
+                if isinstance(self, BeamformerAdaptiveGrid):
                     self._gpos = zeros((3, self.size), dtype=self.precision)
                     ac = zeros((numfreq, self.size), dtype=self.precision)
                 else:
                     ac = zeros((numfreq, self.steer.grid.size), dtype=self.precision)
                 fr = zeros(numfreq, dtype='int8')
-                self.calc(ac,fr)
+                self.calc(ac, fr)
         return ac
-      
+
     def sig_loss_norm(self):
-        """ 
-        If the diagonal of the CSM is removed one has to handle the loss 
+        """If the diagonal of the CSM is removed one has to handle the loss
         of signal energy --> Done via a normalization factor.
         """
-        if not self.r_diag:  # Full CSM --> no normalization needed 
-            normFactor = 1.0 
-        elif self.r_diag_norm == 0.0:  # Removed diag: standard normalization factor 
-            nMics = float(self.freq_data.numchannels) 
-            normFactor = nMics / (nMics - 1) 
-        elif self.r_diag_norm != 0.0:  # Removed diag: user defined normalization factor 
-            normFactor = self.r_diag_norm 
+        if not self.r_diag:  # Full CSM --> no normalization needed
+            normFactor = 1.0
+        elif self.r_diag_norm == 0.0:  # Removed diag: standard normalization factor
+            nMics = float(self.freq_data.numchannels)
+            normFactor = nMics / (nMics - 1)
+        elif self.r_diag_norm != 0.0:  # Removed diag: user defined normalization factor
+            normFactor = self.r_diag_norm
         return normFactor
 
-
     def _beamformer_params(self):
-        """
-        Manages the parameters for calling of the core beamformer functionality.
+        """Manages the parameters for calling of the core beamformer functionality.
         This is a workaround to allow faster calculation and may change in the
         future.
-        
+
         Returns
         -------
             - String containing the steering vector type
             - Function for frequency-dependent steering vector calculation
-                
+
         """
-        if type(self.steer) == SteeringVector: # for simple steering vector, use faster method
+        if type(self.steer) == SteeringVector:  # for simple steering vector, use faster method
             param_type = self.steer.steer_type
-            def param_steer_func(f): return (self.steer.r0, self.steer.rm, 2*pi*f/self.steer.env.c )
+
+            def param_steer_func(f):
+                return (self.steer.r0, self.steer.rm, 2 * pi * f / self.steer.env.c)
         else:
             param_type = 'custom'
             param_steer_func = self.steer.steer_vector
         return param_type, param_steer_func
 
     def calc(self, ac, fr):
-        """
-        Calculates the delay-and-sum beamforming result for the frequencies 
-        defined by :attr:`freq_data`
-        
-        This is an internal helper function that is automatically called when 
+        """Calculates the delay-and-sum beamforming result for the frequencies
+        defined by :attr:`freq_data`.
+
+        This is an internal helper function that is automatically called when
         accessing the beamformer's :attr:`result` or calling
-        its :meth:`synthetic` method.        
-        
+        its :meth:`synthetic` method.
+
         Parameters
         ----------
         ac : array of floats
             This array of dimension ([number of frequencies]x[number of gridpoints])
             is used as call-by-reference parameter and contains the calculated
-            value after calling this method. 
+            value after calling this method.
         fr : array of booleans
-            The entries of this [number of frequencies]-sized array are either 
+            The entries of this [number of frequencies]-sized array are either
             'True' (if the result for this frequency has already been calculated)
             or 'False' (for the frequencies where the result has yet to be calculated).
             After the calculation at a certain frequency the value will be set
             to 'True'
-        
+
         Returns
         -------
         This method only returns values through the *ac* and *fr* parameters
+
         """
-        f = self.freq_data.fftfreq()#[inds]
+        f = self.freq_data.fftfreq()  # [inds]
         param_steer_type, steer_vector = self._beamformer_params()
         for i in self.freq_data.indices:
             if not fr[i]:
                 csm = array(self.freq_data.csm[i], dtype='complex128')
-                beamformerOutput = beamformerFreq(param_steer_type, 
-                                                  self.r_diag, 
-                                                  self.sig_loss_norm(), 
-                                                  steer_vector(f[i]), 
-                                                  csm)[0]
+                beamformerOutput = beamformerFreq(
+                    param_steer_type,
+                    self.r_diag,
+                    self.sig_loss_norm(),
+                    steer_vector(f[i]),
+                    csm,
+                )[0]
                 if self.r_diag:  # set (unphysical) negative output values to 0
                     indNegSign = sign(beamformerOutput) < 0
                     beamformerOutput[indNegSign] = 0.0
                 ac[i] = beamformerOutput
                 fr[i] = 1
-    
-    def synthetic( self, f, num=0):
-        """
-        Evaluates the beamforming result for an arbitrary frequency band.
-        
+
+    def synthetic(self, f, num=0):
+        """Evaluates the beamforming result for an arbitrary frequency band.
+
         Parameters
         ----------
         f: float
-            Band center frequency. 
+            Band center frequency.
         num : integer
             Controls the width of the frequency bands considered; defaults to
             0 (single frequency line).
-            
+
             ===  =====================
             num  frequency band width
             ===  =====================
             0    single frequency line
             1    octave band
             3    third-octave band
             n    1/n-octave band
             ===  =====================
-              
+
         Returns
         -------
         array of floats
-            The synthesized frequency band values of the beamforming result at 
+            The synthesized frequency band values of the beamforming result at
             each grid point .
-            Note that the frequency resolution and therefore the bandwidth 
-            represented by a single frequency line depends on 
-            the :attr:`sampling frequency<acoular.tprocess.SamplesGenerator.sample_freq>` and 
+            Note that the frequency resolution and therefore the bandwidth
+            represented by a single frequency line depends on
+            the :attr:`sampling frequency<acoular.tprocess.SamplesGenerator.sample_freq>` and
             used :attr:`FFT block size<acoular.spectra.PowerSpectra.block_size>`.
+
         """
-        res = self.result # trigger calculation
+        res = self.result  # trigger calculation
         freq = self.freq_data.fftfreq()
         if len(freq) == 0:
             return None
-        
+
         indices = self.freq_data.indices
-        
+
         if num == 0:
             # single frequency line
             ind = searchsorted(freq, f)
             if ind >= len(freq):
-                warn('Queried frequency (%g Hz) not in resolved '
-                              'frequency range. Returning zeros.' % f, 
-                              Warning, stacklevel = 2)
+                warn(
+                    'Queried frequency (%g Hz) not in resolved frequency range. Returning zeros.' % f,
+                    Warning,
+                    stacklevel=2,
+                )
                 h = zeros_like(res[0])
             else:
                 if freq[ind] != f:
-                    warn('Queried frequency (%g Hz) not in set of '
-                         'discrete FFT sample frequencies. '
-                         'Using frequency %g Hz instead.' % (f,freq[ind]), 
-                         Warning, stacklevel = 2)
-                if not (ind in indices):
-                    warn('Beamforming result may not have been calculated '
-                         'for queried frequency. Check '
-                         'freq_data.ind_low and freq_data.ind_high!',
-                          Warning, stacklevel = 2)
+                    warn(
+                        f'Queried frequency ({f:g} Hz) not in set of '
+                        'discrete FFT sample frequencies. '
+                        f'Using frequency {freq[ind]:g} Hz instead.',
+                        Warning,
+                        stacklevel=2,
+                    )
+                if ind not in indices:
+                    warn(
+                        'Beamforming result may not have been calculated '
+                        'for queried frequency. Check '
+                        'freq_data.ind_low and freq_data.ind_high!',
+                        Warning,
+                        stacklevel=2,
+                    )
                 h = res[ind]
         else:
             # fractional octave band
-            if isinstance(num,list):
-                f1=num[0]
-                f2=num[-1]
+            if isinstance(num, list):
+                f1 = num[0]
+                f2 = num[-1]
             else:
-                f1 = f*2.**(-0.5/num)
-                f2 = f*2.**(+0.5/num)
+                f1 = f * 2.0 ** (-0.5 / num)
+                f2 = f * 2.0 ** (+0.5 / num)
             ind1 = searchsorted(freq, f1)
             ind2 = searchsorted(freq, f2)
             if ind1 == ind2:
-                warn('Queried frequency band (%g to %g Hz) does not '
-                     'include any discrete FFT sample frequencies. '
-                     'Returning zeros.' % (f1,f2), 
-                     Warning, stacklevel = 2)
+                warn(
+                    f'Queried frequency band ({f1:g} to {f2:g} Hz) does not '
+                    'include any discrete FFT sample frequencies. '
+                    'Returning zeros.',
+                    Warning,
+                    stacklevel=2,
+                )
                 h = zeros_like(res[0])
             else:
                 h = sum(res[ind1:ind2], 0)
                 if not ((ind1 in indices) and (ind2 in indices)):
-                    warn('Beamforming result may not have been calculated '
-                         'for all queried frequencies. Check '
-                         'freq_data.ind_low and freq_data.ind_high!',
-                          Warning, stacklevel = 2)
-        if isinstance(self,BeamformerAdaptiveGrid):
+                    warn(
+                        'Beamforming result may not have been calculated '
+                        'for all queried frequencies. Check '
+                        'freq_data.ind_low and freq_data.ind_high!',
+                        Warning,
+                        stacklevel=2,
+                    )
+        if isinstance(self, BeamformerAdaptiveGrid):
             return h
-        else:
-            return h.reshape(self.steer.grid.shape)
-
+        return h.reshape(self.steer.grid.shape)
 
     def integrate(self, sector):
-        """
-        Integrates result map over a given sector.
-        
+        """Integrates result map over a given sector.
+
         Parameters
         ----------
         sector: array of floats
-              Tuple with arguments for the 'indices' method 
-              of a :class:`~acoular.grids.Grid`-derived class 
-              (e.g. :meth:`RectGrid.indices<acoular.grids.RectGrid.indices>` 
+              Tuple with arguments for the 'indices' method
+              of a :class:`~acoular.grids.Grid`-derived class
+              (e.g. :meth:`RectGrid.indices<acoular.grids.RectGrid.indices>`
               or :meth:`RectGrid3D.indices<acoular.grids.RectGrid3D.indices>`).
-              Possible sectors would be *array([xmin, ymin, xmax, ymax])* 
+              Possible sectors would be *array([xmin, ymin, xmax, ymax])*
               or *array([x, y, radius])*.
-              
+
         Returns
         -------
         array of floats
             The spectrum (all calculated frequency bands) for the integrated sector.
+
         """
-        #resp. array([rmin, phimin, rmax, phimax]), array([r, phi, radius]).
-        
-#        ind = self.grid.indices(*sector)
-#        gshape = self.grid.shape
-#        r = self.result
-#        rshape = r.shape
-#        mapshape = (rshape[0], ) + gshape
-#        h = r[:].reshape(mapshape)[ (s_[:], ) + ind ]
-#        return h.reshape(h.shape[0], prod(h.shape[1:])).sum(axis=1)
+        # resp. array([rmin, phimin, rmax, phimax]), array([r, phi, radius]).
+
+        #        ind = self.grid.indices(*sector)
+        #        gshape = self.grid.shape
+        #        r = self.result
+        #        rshape = r.shape
+        #        mapshape = (rshape[0], ) + gshape
+        #        h = r[:].reshape(mapshape)[ (s_[:], ) + ind ]
+        #        return h.reshape(h.shape[0], prod(h.shape[1:])).sum(axis=1)
         if isinstance(sector, Sector):
             ind = self.steer.grid.subdomain(sector)
         elif hasattr(self.steer.grid, 'indices'):
             ind = self.steer.grid.indices(*sector)
         else:
+            msg = (
+                f'Grid of type {self.steer.grid.__class__.__name__} does not have an indices method! '
+                f'Please use a sector derived instance of type :class:`~acoular.grids.Sector` '
+                'instead of type numpy.array.'
+            )
             raise NotImplementedError(
-            f'Grid of type {self.steer.grid.__class__.__name__} does not have an indices method! '
-            f'Please use a sector derived instance of type :class:`~acoular.grids.Sector` '
-            'instead of type numpy.array.'
+                msg,
             )
         gshape = self.steer.grid.shape
         r = self.result
         h = zeros(r.shape[0])
         for i in range(r.shape[0]):
             h[i] = r[i].reshape(gshape)[ind].sum()
         return h
 
-class BeamformerFunctional( BeamformerBase ):
-    """
-    Functional beamforming after :ref:`Dougherty, 2014<Dougherty2014>`.
-    """
+
+class BeamformerFunctional(BeamformerBase):
+    """Functional beamforming after :ref:`Dougherty, 2014<Dougherty2014>`."""
 
     #: Functional exponent, defaults to 1 (= Classic Beamforming).
-    gamma = Float(1, 
-        desc="functional exponent")
+    gamma = Float(1, desc='functional exponent')
 
     # internal identifier
-    digest = Property(depends_on = ['freq_data.digest', '_steer_obj.digest', 'r_diag', 'gamma'])
-    
+    digest = Property(depends_on=['freq_data.digest', '_steer_obj.digest', 'r_diag', 'gamma'])
+
     #: Functional Beamforming is only well defined for full CSM
-    r_diag = Enum(False, 
-                  desc="False, as Functional Beamformer is only well defined for the full CSM")
+    r_diag = Enum(False, desc='False, as Functional Beamformer is only well defined for the full CSM')
 
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
+    def _get_digest(self):
+        return digest(self)
 
     def calc(self, ac, fr):
-        """
-        Calculates the Functional Beamformer result for the frequencies defined by :attr:`freq_data`
-        
-        This is an internal helper function that is automatically called when 
+        """Calculates the Functional Beamformer result for the frequencies defined by :attr:`freq_data`.
+
+        This is an internal helper function that is automatically called when
         accessing the beamformer's :attr:`~BeamformerBase.result` or calling
-        its :meth:`~BeamformerBase.synthetic` method.        
-        
+        its :meth:`~BeamformerBase.synthetic` method.
+
         Parameters
         ----------
         ac : array of floats
             This array of dimension ([number of frequencies]x[number of gridpoints])
             is used as call-by-reference parameter and contains the calculated
-            value after calling this method. 
+            value after calling this method.
         fr : array of booleans
-            The entries of this [number of frequencies]-sized array are either 
+            The entries of this [number of frequencies]-sized array are either
             'True' (if the result for this frequency has already been calculated)
             or 'False' (for the frequencies where the result has yet to be calculated).
             After the calculation at a certain frequency the value will be set
             to 'True'
-        
+
         Returns
         -------
         This method only returns values through the *ac* and *fr* parameters
+
         """
         f = self.freq_data.fftfreq()
         normFactor = self.sig_loss_norm()
         param_steer_type, steer_vector = self._beamformer_params()
         for i in self.freq_data.indices:
             if not fr[i]:
                 if self.r_diag:
-                    # This case is not used at the moment (see Trait r_diag)  
+                    # This case is not used at the moment (see Trait r_diag)
                     # It would need some testing as structural changes were not tested...
-#==============================================================================
-#                     One cannot use spectral decomposition when diagonal of csm is removed,
-#                     as the resulting modified eigenvectors are not orthogonal to each other anymore.
-#                     Therefor potentiating cannot be applied only to the eigenvalues.
-#                     --> To avoid this the root of the csm (removed diag) is calculated directly.
-#                     WATCH OUT: This doesn't really produce good results.
-#==============================================================================
+                    # ==============================================================================
+                    #                     One cannot use spectral decomposition when diagonal of csm is removed,
+                    #                     as the resulting modified eigenvectors are not orthogonal to each other anymore.
+                    #                     Therefor potentiating cannot be applied only to the eigenvalues.
+                    #                     --> To avoid this the root of the csm (removed diag) is calculated directly.
+                    #                     WATCH OUT: This doesn't really produce good results.
+                    # ==============================================================================
                     csm = self.freq_data.csm[i]
                     fill_diagonal(csm, 0)
                     csmRoot = fractional_matrix_power(csm, 1.0 / self.gamma)
-                    beamformerOutput, steerNorm = beamformerFreq(param_steer_type, 
-                                                                 self.r_diag, 
-                                                                 1.0, 
-                                                                 steer_vector(f[i]), 
-                                                                 csmRoot)
+                    beamformerOutput, steerNorm = beamformerFreq(
+                        param_steer_type,
+                        self.r_diag,
+                        1.0,
+                        steer_vector(f[i]),
+                        csmRoot,
+                    )
                     beamformerOutput /= steerNorm  # take normalized steering vec
-                    
+
                     # set (unphysical) negative output values to 0
                     indNegSign = sign(beamformerOutput) < 0
                     beamformerOutput[indNegSign] = 0.0
                 else:
                     eva = array(self.freq_data.eva[i], dtype='float64') ** (1.0 / self.gamma)
                     eve = array(self.freq_data.eve[i], dtype='complex128')
-                    beamformerOutput, steerNorm = beamformerFreq(param_steer_type, 
-                                                                 self.r_diag, 
-                                                                 1.0, 
-                                                                 steer_vector(f[i]), 
-                                                                 (eva, eve))
+                    beamformerOutput, steerNorm = beamformerFreq(
+                        param_steer_type,
+                        self.r_diag,
+                        1.0,
+                        steer_vector(f[i]),
+                        (eva, eve),
+                    )
                     beamformerOutput /= steerNorm  # take normalized steering vec
-                ac[i] = (beamformerOutput ** self.gamma) * steerNorm * normFactor  # the normalization must be done outside the beamformer
+                ac[i] = (
+                    (beamformerOutput**self.gamma) * steerNorm * normFactor
+                )  # the normalization must be done outside the beamformer
                 fr[i] = 1
-            
-class BeamformerCapon( BeamformerBase ):
-    """
-    Beamforming using the Capon (Mininimum Variance) algorithm, 
+
+
+class BeamformerCapon(BeamformerBase):
+    """Beamforming using the Capon (Mininimum Variance) algorithm,
     see :ref:`Capon, 1969<Capon1969>`.
     """
+
     # Boolean flag, if 'True', the main diagonal is removed before beamforming;
     # for Capon beamforming r_diag is set to 'False'.
-    r_diag = Enum(False, 
-        desc="removal of diagonal")
+    r_diag = Enum(False, desc='removal of diagonal')
 
     def calc(self, ac, fr):
-        """
-        Calculates the Capon result for the frequencies defined by :attr:`freq_data`
-        
-        This is an internal helper function that is automatically called when 
+        """Calculates the Capon result for the frequencies defined by :attr:`freq_data`.
+
+        This is an internal helper function that is automatically called when
         accessing the beamformer's :attr:`~BeamformerBase.result` or calling
-        its :meth:`~BeamformerBase.synthetic` method.        
-        
+        its :meth:`~BeamformerBase.synthetic` method.
+
         Parameters
         ----------
         ac : array of floats
             This array of dimension ([number of frequencies]x[number of gridpoints])
             is used as call-by-reference parameter and contains the calculated
-            value after calling this method. 
+            value after calling this method.
         fr : array of booleans
-            The entries of this [number of frequencies]-sized array are either 
+            The entries of this [number of frequencies]-sized array are either
             'True' (if the result for this frequency has already been calculated)
             or 'False' (for the frequencies where the result has yet to be calculated).
             After the calculation at a certain frequency the value will be set
             to 'True'
-        
+
         Returns
         -------
         This method only returns values through the *ac* and *fr* parameters
-        """        
+
+        """
         f = self.freq_data.fftfreq()
         nMics = self.freq_data.numchannels
         normFactor = self.sig_loss_norm() * nMics**2
         param_steer_type, steer_vector = self._beamformer_params()
         for i in self.freq_data.indices:
             if not fr[i]:
                 csm = array(linalg.inv(array(self.freq_data.csm[i], dtype='complex128')), order='C')
-                beamformerOutput = beamformerFreq(param_steer_type, 
-                                                  self.r_diag, 
-                                                  normFactor, 
-                                                  steer_vector(f[i]), 
-                                                  csm)[0]
+                beamformerOutput = beamformerFreq(param_steer_type, self.r_diag, normFactor, steer_vector(f[i]), csm)[0]
                 ac[i] = 1.0 / beamformerOutput
                 fr[i] = 1
 
-class BeamformerEig( BeamformerBase ):
-    """
-    Beamforming using eigenvalue and eigenvector techniques,
+
+class BeamformerEig(BeamformerBase):
+    """Beamforming using eigenvalue and eigenvector techniques,
     see :ref:`Sarradj et al., 2005<Sarradj2005>`.
     """
-    #: Number of component to calculate: 
+
+    #: Number of component to calculate:
     #: 0 (smallest) ... :attr:`~acoular.tprocess.SamplesGenerator.numchannels`-1;
     #: defaults to -1, i.e. numchannels-1
-    n = Int(-1, 
-        desc="No. of eigenvalue")
+    n = Int(-1, desc='No. of eigenvalue')
 
     # Actual component to calculate, internal, readonly.
-    na = Property(
-        desc="No. of eigenvalue")
+    na = Property(desc='No. of eigenvalue')
 
     # internal identifier
-    digest = Property( 
-        depends_on = ['freq_data.digest', '_steer_obj.digest', 'r_diag', 'n'])
+    digest = Property(depends_on=['freq_data.digest', '_steer_obj.digest', 'r_diag', 'n'])
 
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
-    
+    def _get_digest(self):
+        return digest(self)
+
     @property_depends_on('steer.mics, n')
-    def _get_na( self ):
+    def _get_na(self):
         na = self.n
         nm = self.steer.mics.num_mics
         if na < 0:
             na = max(nm + na, 0)
         return min(nm - 1, na)
 
     def calc(self, ac, fr):
-        """
-        Calculates the result for the frequencies defined by :attr:`freq_data`
-        
-        This is an internal helper function that is automatically called when 
+        """Calculates the result for the frequencies defined by :attr:`freq_data`.
+
+        This is an internal helper function that is automatically called when
         accessing the beamformer's :attr:`~BeamformerBase.result` or calling
-        its :meth:`~BeamformerBase.synthetic` method.        
-        
+        its :meth:`~BeamformerBase.synthetic` method.
+
         Parameters
         ----------
         ac : array of floats
             This array of dimension ([number of frequencies]x[number of gridpoints])
             is used as call-by-reference parameter and contains the calculated
-            value after calling this method. 
+            value after calling this method.
         fr : array of booleans
-            The entries of this [number of frequencies]-sized array are either 
+            The entries of this [number of frequencies]-sized array are either
             'True' (if the result for this frequency has already been calculated)
             or 'False' (for the frequencies where the result has yet to be calculated).
             After the calculation at a certain frequency the value will be set
             to 'True'
-        
+
         Returns
         -------
         This method only returns values through the *ac* and *fr* parameters
+
         """
         f = self.freq_data.fftfreq()
         na = int(self.na)  # eigenvalue taken into account
         normFactor = self.sig_loss_norm()
         param_steer_type, steer_vector = self._beamformer_params()
         for i in self.freq_data.indices:
             if not fr[i]:
                 eva = array(self.freq_data.eva[i], dtype='float64')
                 eve = array(self.freq_data.eve[i], dtype='complex128')
-                beamformerOutput = beamformerFreq(param_steer_type, 
-                                                  self.r_diag, 
-                                                  normFactor, 
-                                                  steer_vector(f[i]), 
-                                                  (eva[na:na+1], eve[:, na:na+1]))[0]
+                beamformerOutput = beamformerFreq(
+                    param_steer_type,
+                    self.r_diag,
+                    normFactor,
+                    steer_vector(f[i]),
+                    (eva[na : na + 1], eve[:, na : na + 1]),
+                )[0]
                 if self.r_diag:  # set (unphysical) negative output values to 0
                     indNegSign = sign(beamformerOutput) < 0
                     beamformerOutput[indNegSign] = 0
                 ac[i] = beamformerOutput
                 fr[i] = 1
 
-class BeamformerMusic( BeamformerEig ):
-    """
-    Beamforming using the MUSIC algorithm, see :ref:`Schmidt, 1986<Schmidt1986>`.
-    """
+
+class BeamformerMusic(BeamformerEig):
+    """Beamforming using the MUSIC algorithm, see :ref:`Schmidt, 1986<Schmidt1986>`."""
 
     # Boolean flag, if 'True', the main diagonal is removed before beamforming;
     # for MUSIC beamforming r_diag is set to 'False'.
-    r_diag = Enum(False, 
-        desc="removal of diagonal")
+    r_diag = Enum(False, desc='removal of diagonal')
 
     # assumed number of sources, should be set to a value not too small
     # defaults to 1
-    n = Int(1, 
-        desc="assumed number of sources")
+    n = Int(1, desc='assumed number of sources')
 
     def calc(self, ac, fr):
-        """
-        Calculates the MUSIC result for the frequencies defined by :attr:`freq_data`
-        
-        This is an internal helper function that is automatically called when 
+        """Calculates the MUSIC result for the frequencies defined by :attr:`freq_data`.
+
+        This is an internal helper function that is automatically called when
         accessing the beamformer's :attr:`~BeamformerBase.result` or calling
-        its :meth:`~BeamformerBase.synthetic` method.        
-        
+        its :meth:`~BeamformerBase.synthetic` method.
+
         Parameters
         ----------
         ac : array of floats
             This array of dimension ([number of frequencies]x[number of gridpoints])
             is used as call-by-reference parameter and contains the calculated
-            value after calling this method. 
+            value after calling this method.
         fr : array of booleans
-            The entries of this [number of frequencies]-sized array are either 
+            The entries of this [number of frequencies]-sized array are either
             'True' (if the result for this frequency has already been calculated)
             or 'False' (for the frequencies where the result has yet to be calculated).
             After the calculation at a certain frequency the value will be set
             to 'True'
-        
+
         Returns
         -------
         This method only returns values through the *ac* and *fr* parameters
+
         """
         f = self.freq_data.fftfreq()
         nMics = self.freq_data.numchannels
-        n = int(self.steer.mics.num_mics-self.na)
+        n = int(self.steer.mics.num_mics - self.na)
         normFactor = self.sig_loss_norm() * nMics**2
         param_steer_type, steer_vector = self._beamformer_params()
         for i in self.freq_data.indices:
             if not fr[i]:
                 eva = array(self.freq_data.eva[i], dtype='float64')
                 eve = array(self.freq_data.eve[i], dtype='complex128')
-                beamformerOutput = beamformerFreq(param_steer_type, 
-                                                  self.r_diag, 
-                                                  normFactor, 
-                                                  steer_vector(f[i]), 
-                                                  (eva[:n], eve[:, :n]))[0]
-                ac[i] = 4e-10*beamformerOutput.min() / beamformerOutput
+                beamformerOutput = beamformerFreq(
+                    param_steer_type,
+                    self.r_diag,
+                    normFactor,
+                    steer_vector(f[i]),
+                    (eva[:n], eve[:, :n]),
+                )[0]
+                ac[i] = 4e-10 * beamformerOutput.min() / beamformerOutput
                 fr[i] = 1
 
-class PointSpreadFunction (HasPrivateTraits):
-    """
-    The point spread function.
-    
-    This class provides tools to calculate the PSF depending on the used 
+
+class PointSpreadFunction(HasPrivateTraits):
+    """The point spread function.
+
+    This class provides tools to calculate the PSF depending on the used
     microphone geometry, focus grid, flow environment, etc.
     The PSF is needed by several deconvolution algorithms to correct
     the aberrations when using simple delay-and-sum beamforming.
     """
-    
-        # Instance of :class:`~acoular.fbeamform.SteeringVector` or its derived classes
+
+    # Instance of :class:`~acoular.fbeamform.SteeringVector` or its derived classes
     # that contains information about the steering vector. This is a private trait.
     # Do not set this directly, use `steer` trait instead.
-    _steer_obj = Instance(SteeringVector(), SteeringVector)   
-    
-    #: :class:`~acoular.fbeamform.SteeringVector` or derived object. 
+    _steer_obj = Instance(SteeringVector(), SteeringVector)
+
+    #: :class:`~acoular.fbeamform.SteeringVector` or derived object.
     #: Defaults to :class:`~acoular.fbeamform.SteeringVector` object.
-    steer = Property(desc="steering vector object")  
-    
+    steer = Property(desc='steering vector object')
+
     def _get_steer(self):
         return self._steer_obj
-    
+
     def _set_steer(self, steer):
         if isinstance(steer, SteeringVector):
             self._steer_obj = steer
         elif steer in ('true level', 'true location', 'classic', 'inverse'):
             # Type of steering vectors, see also :ref:`Sarradj, 2012<Sarradj2012>`.
-            warn("Deprecated use of 'steer' trait. "
-                 "Please use object of class 'SteeringVector' in the future.", 
-                 Warning, stacklevel = 2)
-            self._steer_obj = SteeringVector(steer_type = steer)
+            warn(
+                "Deprecated use of 'steer' trait. Please use object of class 'SteeringVector' in the future.",
+                Warning,
+                stacklevel=2,
+            )
+            self._steer_obj = SteeringVector(steer_type=steer)
         else:
-            raise(TraitError(args=self,
-                             name='steer', 
-                             info='SteeringVector',
-                             value=steer))
+            raise (TraitError(args=self, name='steer', info='SteeringVector', value=steer))
 
     # --- List of backwards compatibility traits and their setters/getters -----------
-    
-    # :class:`~acoular.environments.Environment` or derived object. 
-    # Deprecated! Only kept for backwards compatibility. 
+
+    # :class:`~acoular.environments.Environment` or derived object.
+    # Deprecated! Only kept for backwards compatibility.
     # Now governed by :attr:`steer` trait.
     env = Property()
-    
+
     def _get_env(self):
-        return self._steer_obj.env    
-    
+        return self._steer_obj.env
+
     def _set_env(self, env):
-        warn("Deprecated use of 'env' trait. ", Warning, stacklevel = 2)
+        warn("Deprecated use of 'env' trait. ", Warning, stacklevel=2)
         self._steer_obj.env = env
-    
+
     # The speed of sound.
-    # Deprecated! Only kept for backwards compatibility. 
+    # Deprecated! Only kept for backwards compatibility.
     # Now governed by :attr:`steer` trait.
     c = Property()
-    
+
     def _get_c(self):
         return self._steer_obj.env.c
-    
+
     def _set_c(self, c):
-        warn("Deprecated use of 'c' trait. ", Warning, stacklevel = 2)
+        warn("Deprecated use of 'c' trait. ", Warning, stacklevel=2)
         self._steer_obj.env.c = c
-   
+
     # :class:`~acoular.grids.Grid`-derived object that provides the grid locations.
-    # Deprecated! Only kept for backwards compatibility. 
+    # Deprecated! Only kept for backwards compatibility.
     # Now governed by :attr:`steer` trait.
     grid = Property()
 
     def _get_grid(self):
         return self._steer_obj.grid
-    
+
     def _set_grid(self, grid):
-        warn("Deprecated use of 'grid' trait. ", Warning, stacklevel = 2)
+        warn("Deprecated use of 'grid' trait. ", Warning, stacklevel=2)
         self._steer_obj.grid = grid
-    
+
     # :class:`~acoular.microphones.MicGeom` object that provides the microphone locations.
-    # Deprecated! Only kept for backwards compatibility. 
+    # Deprecated! Only kept for backwards compatibility.
     # Now governed by :attr:`steer` trait
     mpos = Property()
-    
+
     def _get_mpos(self):
         return self._steer_obj.mics
-    
+
     def _set_mpos(self, mpos):
-        warn("Deprecated use of 'mpos' trait. ", Warning, stacklevel = 2)
+        warn("Deprecated use of 'mpos' trait. ", Warning, stacklevel=2)
         self._steer_obj.mics = mpos
-    
-    
+
     # Sound travel distances from microphone array center to grid points (r0)
     # and all array mics to grid points (rm). Readonly.
-    # Deprecated! Only kept for backwards compatibility. 
+    # Deprecated! Only kept for backwards compatibility.
     # Now governed by :attr:`steer` trait
     r0 = Property()
+
     def _get_r0(self):
         return self._steer_obj.r0
-    
+
     rm = Property()
+
     def _get_rm(self):
         return self._steer_obj.rm
-    
+
     # --- End of backwards compatibility traits --------------------------------------
-    
-    
+
     #: Indices of grid points to calculate the PSF for.
-    grid_indices = CArray( dtype=int, value=array([]), 
-                     desc="indices of grid points for psf") #value=array([]), value=self.grid.pos(),
-    
+    grid_indices = CArray(
+        dtype=int,
+        value=array([]),
+        desc='indices of grid points for psf',
+    )  # value=array([]), value=self.grid.pos(),
+
     #: Flag that defines how to calculate and store the point spread function
     #: defaults to 'single'.
     #:
     #: * 'full': Calculate the full PSF (for all grid points) in one go (should be used if the PSF at all grid points is needed, as with :class:`DAMAS<BeamformerDamas>`)
     #: * 'single': Calculate the PSF for the grid points defined by :attr:`grid_indices`, one by one (useful if not all PSFs are needed, as with :class:`CLEAN<BeamformerClean>`)
     #: * 'block': Calculate the PSF for the grid points defined by :attr:`grid_indices`, in one go (useful if not all PSFs are needed, as with :class:`CLEAN<BeamformerClean>`)
     #: * 'readonly': Do not attempt to calculate the PSF since it should already be cached (useful if multiple processes have to access the cache file)
-    calcmode = Trait('single', 'block', 'full', 'readonly',
-                     desc="mode of calculation / storage")
-              
+    calcmode = Trait('single', 'block', 'full', 'readonly', desc='mode of calculation / storage')
+
     #: Floating point precision of property psf. Corresponding to numpy dtypes. Default = 64 Bit.
-    precision = Trait('float64', 'float32',
-            desc="precision (32/64 Bit) of result, corresponding to numpy dtypes")
-    
+    precision = Trait('float64', 'float32', desc='precision (32/64 Bit) of result, corresponding to numpy dtypes')
+
     #: The actual point spread function.
-    psf = Property(desc="point spread function")
-    
-    #: Frequency to evaluate the PSF for; defaults to 1.0. 
-    freq = Float(1.0, desc="frequency")
+    psf = Property(desc='point spread function')
+
+    #: Frequency to evaluate the PSF for; defaults to 1.0.
+    freq = Float(1.0, desc='frequency')
 
     # hdf5 cache file
-    h5f = Instance( H5CacheFileBase, transient = True )
-    
+    h5f = Instance(H5CacheFileBase, transient=True)
+
     # internal identifier
-    digest = Property( depends_on = ['_steer_obj.digest', 'precision'], cached = True)
+    digest = Property(depends_on=['_steer_obj.digest', 'precision'], cached=True)
 
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
-    
-    def _get_filecache( self ):
-        """
-        function collects cached results from file depending on 
-        global/local caching behaviour. Returns (None, None) if no cachefile/data 
+    def _get_digest(self):
+        return digest(self)
+
+    def _get_filecache(self):
+        """Function collects cached results from file depending on
+        global/local caching behaviour. Returns (None, None) if no cachefile/data
         exist and global caching mode is 'readonly'.
         """
         filename = 'psf' + self.digest
         nodename = ('Hz_%.2f' % self.freq).replace('.', '_')
-#        print("get cachefile:", filename)
-        H5cache.get_cache_file( self, filename ) 
-        if not self.h5f: # only happens in case of global caching readonly
-#            print("no cachefile:", filename)
-            return (None, None)# only happens in case of global caching readonly
-                    
+        #        print("get cachefile:", filename)
+        H5cache.get_cache_file(self, filename)
+        if not self.h5f:  # only happens in case of global caching readonly
+            #            print("no cachefile:", filename)
+            return (None, None)  # only happens in case of global caching readonly
+
         if config.global_caching == 'overwrite' and self.h5f.is_cached(nodename):
-#            print("remove existing data for nodename",nodename)
-            self.h5f.remove_data(nodename) # remove old data before writing in overwrite mode
-        
+            #            print("remove existing data for nodename",nodename)
+            self.h5f.remove_data(nodename)  # remove old data before writing in overwrite mode
+
         if not self.h5f.is_cached(nodename):
-#            print("no data existent for nodename:", nodename)
+            #            print("no data existent for nodename:", nodename)
             if config.global_caching == 'readonly':
                 return (None, None)
-            else:
-#                print("initialize data.")
-                gs = self.steer.grid.size
-                group = self.h5f.create_new_group(nodename)
-                self.h5f.create_compressible_array('result',
-                                      (gs, gs),
-                                      self.precision,
-                                      group)
-                self.h5f.create_compressible_array('gridpts',
-                                      (gs,),
-                                      'int8',#'bool', 
-                                      group)
-        ac = self.h5f.get_data_by_reference('result','/'+nodename)
-        gp = self.h5f.get_data_by_reference('gridpts','/'+nodename)
-        return (ac,gp)        
+            gs = self.steer.grid.size
+            group = self.h5f.create_new_group(nodename)
+            self.h5f.create_compressible_array('result', (gs, gs), self.precision, group)
+            self.h5f.create_compressible_array(
+                'gridpts',
+                (gs,),
+                'int8',  #'bool',
+                group,
+            )
+        ac = self.h5f.get_data_by_reference('result', '/' + nodename)
+        gp = self.h5f.get_data_by_reference('gridpts', '/' + nodename)
+        return (ac, gp)
 
-    def _get_psf ( self ):
-        """
-        This is the :attr:`psf` getter routine.
+    def _get_psf(self):
+        """Implements the :attr:`psf` getter routine.
         The point spread function is either loaded or calculated.
         """
         gs = self.steer.grid.size
-        if not self.grid_indices.size: 
+        if not self.grid_indices.size:
             self.grid_indices = arange(gs)
 
-        if not config.global_caching == 'none':
-#            print("get filecache..")
-            (ac,gp) = self._get_filecache()
-            if ac and gp: 
-#                print("cached data existent")
+        if config.global_caching != 'none':
+            #            print("get filecache..")
+            (ac, gp) = self._get_filecache()
+            if ac and gp:
+                #                print("cached data existent")
                 if not gp[:][self.grid_indices].all():
-#                    print("calculate missing results")                            
+                    #                    print("calculate missing results")
                     if self.calcmode == 'readonly':
-                        raise ValueError('Cannot calculate missing PSF (points) in \'readonly\' mode.')
+                        msg = "Cannot calculate missing PSF (points) in 'readonly' mode."
+                        raise ValueError(msg)
                     if config.global_caching == 'readonly':
                         (ac, gp) = (ac[:], gp[:])
-                        self.calc_psf(ac,gp)
-                        return ac[:,self.grid_indices]
-                    else:
-                        self.calc_psf(ac,gp)
-                        self.h5f.flush()
-                        return ac[:,self.grid_indices]
-#                else:
-#                    print("cached results are complete! return.")
-                return ac[:,self.grid_indices]
-            else: # no cached data/file
-#                print("no caching, calculate result")
-                ac = zeros((gs, gs), dtype=self.precision)
-                gp = zeros((gs,), dtype='int8')
-                self.calc_psf(ac,gp)
-        else: # no caching activated
-#            print("no caching activated, calculate result")
+                        self.calc_psf(ac, gp)
+                        return ac[:, self.grid_indices]
+                    self.calc_psf(ac, gp)
+                    self.h5f.flush()
+                    return ac[:, self.grid_indices]
+                #                else:
+                #                    print("cached results are complete! return.")
+                return ac[:, self.grid_indices]
+            #           print("no caching, calculate result")
             ac = zeros((gs, gs), dtype=self.precision)
             gp = zeros((gs,), dtype='int8')
-            self.calc_psf(ac,gp)
-        return ac[:,self.grid_indices] 
+            self.calc_psf(ac, gp)
+        else:  # no caching activated
+            #            print("no caching activated, calculate result")
+            ac = zeros((gs, gs), dtype=self.precision)
+            gp = zeros((gs,), dtype='int8')
+            self.calc_psf(ac, gp)
+        return ac[:, self.grid_indices]
 
-    def calc_psf( self, ac, gp ):
-        """
-        point-spread function calculation
-        """
+    def calc_psf(self, ac, gp):
+        """point-spread function calculation."""
         if self.calcmode != 'full':
             # calc_ind has the form [True, True, False, True], except
             # when it has only 1 entry (value True/1 would be ambiguous)
-            if self.grid_indices.size == 1:
-                calc_ind = [0]
-            else:
-                calc_ind = invert(gp[:][self.grid_indices])
-        
-        # get indices which have the value True = not yet calculated
+            calc_ind = [0] if self.grid_indices.size == 1 else invert(gp[:][self.grid_indices])
+
+            # get indices which have the value True = not yet calculated
             g_ind_calc = self.grid_indices[calc_ind]
-        
-        if self.calcmode == 'single': # calculate selected psfs one-by-one
+
+        if self.calcmode == 'single':  # calculate selected psfs one-by-one
             for ind in g_ind_calc:
-                ac[:,ind] = self._psfCall([ind])[:,0]
+                ac[:, ind] = self._psfCall([ind])[:, 0]
                 gp[ind] = 1
-        elif self.calcmode == 'full': # calculate all psfs in one go
+        elif self.calcmode == 'full':  # calculate all psfs in one go
             gp[:] = 1
             ac[:] = self._psfCall(arange(self.steer.grid.size))
-        else: # 'block' # calculate selected psfs in one go
+        else:  # 'block' # calculate selected psfs in one go
             hh = self._psfCall(g_ind_calc)
-            indh = 0
-            for ind in g_ind_calc:
+            for indh, ind in enumerate(g_ind_calc):
                 gp[ind] = 1
-                ac[:,ind] = hh[:,indh]
+                ac[:, ind] = hh[:, indh]
                 indh += 1
 
     def _psfCall(self, ind):
-        """
-        Manages the calling of the core psf functionality.
-        
+        """Manages the calling of the core psf functionality.
+
         Parameters
         ----------
         ind : list of int
             Indices of gridpoints which are assumed to be sources.
             Normalization factor for the beamforming result (e.g. removal of diag is compensated with this.)
 
         Returns
         -------
         The psf [1, nGridPoints, len(ind)]
+
         """
-        if type(self.steer) == SteeringVector: # for simple steering vector, use faster method
-            result = calcPointSpreadFunction(self.steer.steer_type, 
-                                             self.steer.r0, 
-                                             self.steer.rm, 
-                                             2*pi*self.freq/self.env.c, 
-                                             ind, self.precision)
-        else: # for arbitrary steering sectors, use general calculation
+        if type(self.steer) == SteeringVector:  # for simple steering vector, use faster method
+            result = calcPointSpreadFunction(
+                self.steer.steer_type,
+                self.steer.r0,
+                self.steer.rm,
+                2 * pi * self.freq / self.env.c,
+                ind,
+                self.precision,
+            )
+        else:  # for arbitrary steering sectors, use general calculation
             # there is a version of this in fastFuncs, may be used later after runtime testing and debugging
-            product = dot(self.steer.steer_vector(self.freq).conj(), self.steer.transfer(self.freq,ind).T)
+            product = dot(self.steer.steer_vector(self.freq).conj(), self.steer.transfer(self.freq, ind).T)
             result = (product * product.conj()).real
         return result
 
-class BeamformerDamas (BeamformerBase):
-    """
-    DAMAS deconvolution, see :ref:`Brooks and Humphreys, 2006<BrooksHumphreys2006>`.
+
+class BeamformerDamas(BeamformerBase):
+    """DAMAS deconvolution, see :ref:`Brooks and Humphreys, 2006<BrooksHumphreys2006>`.
     Needs a-priori delay-and-sum beamforming (:class:`BeamformerBase`).
     """
 
     #: :class:`BeamformerBase` object that provides data for deconvolution.
     beamformer = Trait(BeamformerBase)
 
-    #: :class:`~acoular.spectra.PowerSpectra` object that provides the cross spectral matrix; 
+    #: :class:`~acoular.spectra.PowerSpectra` object that provides the cross spectral matrix;
     #: is set automatically.
     freq_data = Delegate('beamformer')
 
-    #: Boolean flag, if 'True' (default), the main diagonal is removed before beamforming; 
+    #: Boolean flag, if 'True' (default), the main diagonal is removed before beamforming;
     #: is set automatically.
-    r_diag =  Delegate('beamformer')
-    
+    r_diag = Delegate('beamformer')
+
     #: instance of :class:`~acoular.fbeamform.SteeringVector` or its derived classes,
     #: that contains information about the steering vector. Is set automatically.
     steer = Delegate('beamformer')
-    
+
     #: Floating point precision of result, is set automatically.
     precision = Delegate('beamformer')
-    
+
     #: The floating-number-precision of the PSFs. Default is 64 bit.
-    psf_precision = Trait('float64', 'float32', 
-                          desc="precision of PSF")
+    psf_precision = Trait('float64', 'float32', desc='precision of PSF')
 
     #: Number of iterations, defaults to 100.
-    n_iter = Int(100, 
-        desc="number of iterations")
-    
+    n_iter = Int(100, desc='number of iterations')
+
     #: Damping factor in modified gauss-seidel
-    damp = Float(1.0,
-                          desc="damping factor in modified gauss-seidel-DAMAS-approach")
+    damp = Float(1.0, desc='damping factor in modified gauss-seidel-DAMAS-approach')
 
-    #: Flag that defines how to calculate and store the point spread function, 
+    #: Flag that defines how to calculate and store the point spread function,
     #: defaults to 'full'. See :attr:`PointSpreadFunction.calcmode` for details.
-    calcmode = Trait('full', 'single', 'block', 'readonly',
-                     desc="mode of psf calculation / storage")
-    
+    calcmode = Trait('full', 'single', 'block', 'readonly', desc='mode of psf calculation / storage')
+
     # internal identifier
-    digest = Property( 
-        depends_on = ['beamformer.digest', 'n_iter', 'damp', 'psf_precision'], 
-        )
+    digest = Property(
+        depends_on=['beamformer.digest', 'n_iter', 'damp', 'psf_precision'],
+    )
 
     # internal identifier
-    ext_digest = Property( 
-        depends_on = ['digest', 'beamformer.ext_digest'], 
-        )
-    
+    ext_digest = Property(
+        depends_on=['digest', 'beamformer.ext_digest'],
+    )
+
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
-      
+    def _get_digest(self):
+        return digest(self)
+
     @cached_property
-    def _get_ext_digest( self ):
-        return digest( self, 'ext_digest' )
-    
+    def _get_ext_digest(self):
+        return digest(self, 'ext_digest')
+
     def calc(self, ac, fr):
-        """
-        Calculates the DAMAS result for the frequencies defined by :attr:`freq_data`
-        
-        This is an internal helper function that is automatically called when 
+        """Calculates the DAMAS result for the frequencies defined by :attr:`freq_data`.
+
+        This is an internal helper function that is automatically called when
         accessing the beamformer's :attr:`~BeamformerBase.result` or calling
-        its :meth:`~BeamformerBase.synthetic` method.        
+        its :meth:`~BeamformerBase.synthetic` method.
         A Gauss-Seidel algorithm implemented in C is used for computing the result.
-        
+
         Parameters
         ----------
         ac : array of floats
             This array of dimension ([number of frequencies]x[number of gridpoints])
             is used as call-by-reference parameter and contains the calculated
-            value after calling this method. 
+            value after calling this method.
         fr : array of booleans
-            The entries of this [number of frequencies]-sized array are either 
+            The entries of this [number of frequencies]-sized array are either
             'True' (if the result for this frequency has already been calculated)
             or 'False' (for the frequencies where the result has yet to be calculated).
             After the calculation at a certain frequency the value will be set
             to 'True'
-        
+
         Returns
         -------
         This method only returns values through the *ac* and *fr* parameters
+
         """
         f = self.freq_data.fftfreq()
         p = PointSpreadFunction(steer=self.steer, calcmode=self.calcmode, precision=self.psf_precision)
         for i in self.freq_data.indices:
             if not fr[i]:
                 y = array(self.beamformer.result[i])
                 x = y.copy()
                 p.freq = f[i]
                 psf = p.psf[:]
                 damasSolverGaussSeidel(psf, y, self.n_iter, self.damp, x)
                 ac[i] = x
                 fr[i] = 1
 
-class BeamformerDamasPlus (BeamformerDamas):
-    """
-    DAMAS deconvolution, see :ref:`Brooks and Humphreys, 2006<BrooksHumphreys2006>`,
-    for solving the system of equations, instead of the original Gauss-Seidel 
-    iterations, this class employs the NNLS or linear programming solvers from 
+
+class BeamformerDamasPlus(BeamformerDamas):
+    """DAMAS deconvolution, see :ref:`Brooks and Humphreys, 2006<BrooksHumphreys2006>`,
+    for solving the system of equations, instead of the original Gauss-Seidel
+    iterations, this class employs the NNLS or linear programming solvers from
     scipy.optimize or one  of several optimization algorithms from the scikit-learn module.
     Needs a-priori delay-and-sum beamforming (:class:`BeamformerBase`).
     """
-    
-    #: Type of fit method to be used ('LassoLars', 
+
+    #: Type of fit method to be used ('LassoLars',
     #: 'OMPCV', 'LP', or 'NNLS', defaults to 'NNLS').
-    #: These methods are implemented in 
-    #: the `scikit-learn <http://scikit-learn.org/stable/user_guide.html>`_ 
+    #: These methods are implemented in
+    #: the `scikit-learn <http://scikit-learn.org/stable/user_guide.html>`_
     #: module or within scipy.optimize respectively.
-    method = Trait('NNLS','LP','LassoLars', 'OMPCV',  
-                   desc="method used for solving deconvolution problem")
-    
+    method = Trait('NNLS', 'LP', 'LassoLars', 'OMPCV', desc='method used for solving deconvolution problem')
+
     #: Weight factor for LassoLars method,
     #: defaults to 0.0.
     # (Values in the order of 10^⁻9 should produce good results.)
-    alpha = Range(0.0, 1.0, 0.0,
-                  desc="Lasso weight factor")
-    
+    alpha = Range(0.0, 1.0, 0.0, desc='Lasso weight factor')
+
     #: Maximum number of iterations,
     #: tradeoff between speed and precision;
     #: defaults to 500
-    max_iter = Int(500,
-                   desc="maximum number of iterations")
-    
-    #: Unit multiplier for evaluating, e.g., nPa instead of Pa. 
-    #: Values are converted back before returning. 
+    max_iter = Int(500, desc='maximum number of iterations')
+
+    #: Unit multiplier for evaluating, e.g., nPa instead of Pa.
+    #: Values are converted back before returning.
     #: Temporary conversion may be necessary to not reach machine epsilon
     #: within fitting method algorithms. Defaults to 1e9.
-    unit_mult = Float(1e9,
-                      desc = "unit multiplier")
-    
+    unit_mult = Float(1e9, desc='unit multiplier')
+
     # internal identifier
-    digest = Property( 
-        depends_on = ['beamformer.digest','alpha', 'method', 
-                      'max_iter', 'unit_mult'], 
-        )
+    digest = Property(
+        depends_on=['beamformer.digest', 'alpha', 'method', 'max_iter', 'unit_mult'],
+    )
 
     # internal identifier
-    ext_digest = Property( 
-        depends_on = ['digest', 'beamformer.ext_digest'], 
-        )
-    
+    ext_digest = Property(
+        depends_on=['digest', 'beamformer.ext_digest'],
+    )
+
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
-      
+    def _get_digest(self):
+        return digest(self)
+
     @cached_property
-    def _get_ext_digest( self ):
-        return digest( self, 'ext_digest' )
-    
+    def _get_ext_digest(self):
+        return digest(self, 'ext_digest')
+
     def calc(self, ac, fr):
-        """
-        Calculates the DAMAS result for the frequencies defined by :attr:`freq_data`
-        
-        This is an internal helper function that is automatically called when 
+        """Calculates the DAMAS result for the frequencies defined by :attr:`freq_data`.
+
+        This is an internal helper function that is automatically called when
         accessing the beamformer's :attr:`~BeamformerBase.result` or calling
-        its :meth:`~BeamformerBase.synthetic` method.        
-        
+        its :meth:`~BeamformerBase.synthetic` method.
+
         Parameters
         ----------
         ac : array of floats
             This array of dimension ([number of frequencies]x[number of gridpoints])
             is used as call-by-reference parameter and contains the calculated
-            value after calling this method. 
+            value after calling this method.
         fr : array of booleans
-            The entries of this [number of frequencies]-sized array are either 
+            The entries of this [number of frequencies]-sized array are either
             'True' (if the result for this frequency has already been calculated)
             or 'False' (for the frequencies where the result has yet to be calculated).
             After the calculation at a certain frequency the value will be set
             to 'True'
-        
+
         Returns
         -------
         This method only returns values through the *ac* and *fr* parameters
+
         """
         f = self.freq_data.fftfreq()
         p = PointSpreadFunction(steer=self.steer, calcmode=self.calcmode, precision=self.psf_precision)
         unit = self.unit_mult
         for i in self.freq_data.indices:
             if not fr[i]:
                 y = self.beamformer.result[i] * unit
                 p.freq = f[i]
                 psf = p.psf[:]
 
-                if self.method == "NNLS":
+                if self.method == 'NNLS':
                     ac[i] = nnls(psf, y)[0] / unit
-                elif self.method == "LP":  # linear programming (Dougherty)
+                elif self.method == 'LP':  # linear programming (Dougherty)
                     if self.r_diag:
                         warn(
-                            "Linear programming solver may fail when CSM main "
-                            "diagonal is removed for delay-and-sum beamforming.",
+                            'Linear programming solver may fail when CSM main '
+                            'diagonal is removed for delay-and-sum beamforming.',
                             Warning,
                             stacklevel=5,
                         )
                     cT = -1 * psf.sum(1)  # turn the minimization into a maximization
-                    ac[i] = (
-                        linprog(c=cT, A_ub=psf, b_ub=y).x / unit
-                    )  # defaults to simplex method and non-negative x
+                    ac[i] = linprog(c=cT, A_ub=psf, b_ub=y).x / unit  # defaults to simplex method and non-negative x
                 else:
-                    if self.method == "LassoLars":
+                    if self.method == 'LassoLars':
                         model = LassoLars(
-                            alpha=self.alpha * unit, max_iter=self.max_iter
+                            alpha=self.alpha * unit,
+                            max_iter=self.max_iter,
                         )
-                    elif self.method == "OMPCV":
+                    elif self.method == 'OMPCV':
                         model = OrthogonalMatchingPursuitCV()
                     else:
-                        raise NotImplementedError(f"%model solver not implemented")
+                        msg = f'Method {self.method} not implemented.'
+                        raise NotImplementedError(msg)
                     model.normalize = False
                     # from sklearn 1.2, normalize=True does not work the same way anymore and the pipeline approach
                     # with StandardScaler does scale in a different way, thus we monkeypatch the code and normalize
                     # ourselves to make results the same over different sklearn versions
                     norms = norm(psf, axis=0)
                     # get rid of annoying sklearn warnings that appear
                     # for sklearn<1.2 despite any settings
                     with warnings.catch_warnings():
-                        warnings.simplefilter("ignore", category=FutureWarning)
+                        warnings.simplefilter('ignore', category=FutureWarning)
                         # normalized psf
                         model.fit(psf / norms, y)
                     # recover normalization in the coef's
                     ac[i] = model.coef_[:] / norms / unit
-                
+
                 fr[i] = 1
 
 
-class BeamformerOrth( BeamformerBase ):
-    """
-    Orthogonal deconvolution, see :ref:`Sarradj, 2010<Sarradj2010>`.
+class BeamformerOrth(BeamformerBase):
+    """Orthogonal deconvolution, see :ref:`Sarradj, 2010<Sarradj2010>`.
     New faster implementation without explicit (:class:`BeamformerEig`).
     """
+
     #: (only for backward compatibility) :class:`BeamformerEig` object
     #: if set, provides :attr:`freq_data`, :attr:`steer`, :attr:`r_diag`
     #: if not set, these have to be set explicitly
     beamformer = Trait(BeamformerEig)
 
     #: List of components to consider, use this to directly set the eigenvalues
     #: used in the beamformer. Alternatively, set :attr:`n`.
-    eva_list = CArray(dtype=int,
-        desc="components")
-        
-    #: Number of components to consider, defaults to 1. If set, 
+    eva_list = CArray(dtype=int, desc='components')
+
+    #: Number of components to consider, defaults to 1. If set,
     #: :attr:`eva_list` will contain
-    #: the indices of the n largest eigenvalues. Setting :attr:`eva_list` 
+    #: the indices of the n largest eigenvalues. Setting :attr:`eva_list`
     #: afterwards will override this value.
     n = Int(1)
 
     # internal identifier
-    digest = Property( 
-        depends_on = ['freq_data.digest', '_steer_obj.digest', 'r_diag', 
-            'eva_list'], 
-        )
-   
+    digest = Property(
+        depends_on=['freq_data.digest', '_steer_obj.digest', 'r_diag', 'eva_list'],
+    )
+
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
+    def _get_digest(self):
+        return digest(self)
 
     @cached_property
-    def _get_ext_digest( self ):
-        return digest( self, 'ext_digest' )
+    def _get_ext_digest(self):
+        return digest(self, 'ext_digest')
 
     @on_trait_change('beamformer.digest')
     def delegate_beamformer_traits(self):
         self.freq_data = self.beamformer.freq_data
         self.r_diag = self.beamformer.r_diag
         self.steer = self.beamformer.steer
 
     @on_trait_change('n')
     def set_eva_list(self):
-        """ sets the list of eigenvalues to consider """
-        self.eva_list = arange(-1, -1-self.n, -1)
+        """Sets the list of eigenvalues to consider."""
+        self.eva_list = arange(-1, -1 - self.n, -1)
 
     def calc(self, ac, fr):
-        """
-        Calculates the Orthogonal Beamforming result for the frequencies 
+        """Calculates the Orthogonal Beamforming result for the frequencies
         defined by :attr:`freq_data`.
-        
-        This is an internal helper function that is automatically called when 
+
+        This is an internal helper function that is automatically called when
         accessing the beamformer's :attr:`~BeamformerBase.result` or calling
-        its :meth:`~BeamformerBase.synthetic` method.        
-        
+        its :meth:`~BeamformerBase.synthetic` method.
+
         Parameters
         ----------
         ac : array of floats
             This array of dimension ([number of frequencies]x[number of gridpoints])
             is used as call-by-reference parameter and contains the calculated
-            value after calling this method. 
+            value after calling this method.
         fr : array of booleans
-            The entries of this [number of frequencies]-sized array are either 
+            The entries of this [number of frequencies]-sized array are either
             'True' (if the result for this frequency has already been calculated)
             or 'False' (for the frequencies where the result has yet to be calculated).
             After the calculation at a certain frequency the value will be set
             to 'True'
-        
+
         Returns
         -------
         This method only returns values through the *ac* and *fr* parameters
+
         """
         # prepare calculation
         f = self.freq_data.fftfreq()
         numchannels = self.freq_data.numchannels
         normFactor = self.sig_loss_norm()
         param_steer_type, steer_vector = self._beamformer_params()
-        for i in self.freq_data.indices:        
+        for i in self.freq_data.indices:
             if not fr[i]:
                 eva = array(self.freq_data.eva[i], dtype='float64')
                 eve = array(self.freq_data.eve[i], dtype='complex128')
                 for n in self.eva_list:
-                    beamformerOutput = beamformerFreq(param_steer_type, 
-                                                self.r_diag, 
-                                                normFactor, 
-                                                steer_vector(f[i]), 
-                                                (ones(1), eve[:, n].reshape((-1,1))))[0]
-                    ac[i, beamformerOutput.argmax()]+=eva[n]/numchannels
+                    beamformerOutput = beamformerFreq(
+                        param_steer_type,
+                        self.r_diag,
+                        normFactor,
+                        steer_vector(f[i]),
+                        (ones(1), eve[:, n].reshape((-1, 1))),
+                    )[0]
+                    ac[i, beamformerOutput.argmax()] += eva[n] / numchannels
                 fr[i] = 1
 
-class BeamformerCleansc( BeamformerBase ):
-    """
-    CLEAN-SC deconvolution, see :ref:`Sijtsma, 2007<Sijtsma2007>`.
+
+class BeamformerCleansc(BeamformerBase):
+    """CLEAN-SC deconvolution, see :ref:`Sijtsma, 2007<Sijtsma2007>`.
     Classic delay-and-sum beamforming is already included.
     """
 
     #: no of CLEAN-SC iterations
     #: defaults to 0, i.e. automatic (max 2*numchannels)
-    n = Int(0, 
-        desc="no of iterations")
+    n = Int(0, desc='no of iterations')
 
     #: iteration damping factor
     #: defaults to 0.6
-    damp = Range(0.01, 1.0, 0.6, 
-        desc="damping factor")
+    damp = Range(0.01, 1.0, 0.6, desc='damping factor')
 
     #: iteration stop criterion for automatic detection
     #: iteration stops if power[i]>power[i-stopn]
     #: defaults to 3
-    stopn = Int(3, 
-        desc="stop criterion index")
+    stopn = Int(3, desc='stop criterion index')
 
     # internal identifier
-    digest = Property( 
-        depends_on = ['freq_data.digest', '_steer_obj.digest', 'r_diag', 'n', 'damp', 'stopn'])
+    digest = Property(depends_on=['freq_data.digest', '_steer_obj.digest', 'r_diag', 'n', 'damp', 'stopn'])
 
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
+    def _get_digest(self):
+        return digest(self)
 
     def calc(self, ac, fr):
-        """
-        Calculates the CLEAN-SC result for the frequencies defined by :attr:`freq_data`
-        
-        This is an internal helper function that is automatically called when 
+        """Calculates the CLEAN-SC result for the frequencies defined by :attr:`freq_data`.
+
+        This is an internal helper function that is automatically called when
         accessing the beamformer's :attr:`~BeamformerBase.result` or calling
-        its :meth:`~BeamformerBase.synthetic` method.        
-        
+        its :meth:`~BeamformerBase.synthetic` method.
+
         Parameters
         ----------
         ac : array of floats
             This array of dimension ([number of frequencies]x[number of gridpoints])
             is used as call-by-reference parameter and contains the calculated
-            value after calling this method. 
+            value after calling this method.
         fr : array of booleans
-            The entries of this [number of frequencies]-sized array are either 
+            The entries of this [number of frequencies]-sized array are either
             'True' (if the result for this frequency has already been calculated)
             or 'False' (for the frequencies where the result has yet to be calculated).
             After the calculation at a certain frequency the value will be set
             to 'True'
-        
+
         Returns
         -------
         This method only returns values through the *ac* and *fr* parameters
-        """
 
+        """
         # prepare calculation
         normFactor = self.sig_loss_norm()
         numchannels = self.freq_data.numchannels
         f = self.freq_data.fftfreq()
-        result = zeros((self.steer.grid.size), 'f') 
+        result = zeros((self.steer.grid.size), 'f')
         normFac = self.sig_loss_norm()
-        if not self.n:
-            J = numchannels*2
-        else:
-            J = self.n
+        J = numchannels * 2 if not self.n else self.n
         powers = zeros(J, 'd')
-        
+
         param_steer_type, steer_vector = self._beamformer_params()
         for i in self.freq_data.indices:
             if not fr[i]:
                 csm = array(self.freq_data.csm[i], dtype='complex128', copy=1)
-                #h = self.steer._beamformerCall(f[i], self.r_diag, normFactor, (csm,))[0]
-                h = beamformerFreq(param_steer_type, 
-                                   self.r_diag, 
-                                   normFactor, 
-                                   steer_vector(f[i]), 
-                                   csm)[0]
+                # h = self.steer._beamformerCall(f[i], self.r_diag, normFactor, (csm,))[0]
+                h = beamformerFreq(param_steer_type, self.r_diag, normFactor, steer_vector(f[i]), csm)[0]
                 # CLEANSC Iteration
                 result *= 0.0
                 for j in range(J):
-                    xi_max = h.argmax() #index of maximum
-                    powers[j] = hmax = h[xi_max] #maximum
+                    xi_max = h.argmax()  # index of maximum
+                    powers[j] = hmax = h[xi_max]  # maximum
                     result[xi_max] += self.damp * hmax
-                    if  j > self.stopn and hmax > powers[j-self.stopn]:
+                    if j > self.stopn and hmax > powers[j - self.stopn]:
                         break
-                    wmax = self.steer.steer_vector(f[i],xi_max) * sqrt(normFac)
+                    wmax = self.steer.steer_vector(f[i], xi_max) * sqrt(normFac)
                     wmax = wmax[0].conj()  # as old code worked with conjugated csm..should be updated
                     hh = wmax.copy()
-                    D1 = dot(csm.T - diag(diag(csm)), wmax)/hmax
-                    ww = wmax.conj()*wmax
-                    for m in range(20):
-                        H = hh.conj()*hh
-                        hh = (D1+H*wmax)/sqrt(1+dot(ww, H))
+                    D1 = dot(csm.T - diag(diag(csm)), wmax) / hmax
+                    ww = wmax.conj() * wmax
+                    for _m in range(20):
+                        H = hh.conj() * hh
+                        hh = (D1 + H * wmax) / sqrt(1 + dot(ww, H))
                     hh = hh[:, newaxis]
-                    csm1 = hmax*(hh*hh.conj().T)
-                    
-                    #h1 = self.steer._beamformerCall(f[i], self.r_diag, normFactor, (array((hmax, ))[newaxis, :], hh[newaxis, :].conjugate()))[0]
-                    h1 = beamformerFreq(param_steer_type, 
-                                        self.r_diag, 
-                                        normFactor, 
-                                        steer_vector(f[i]), 
-                                        (array((hmax, )), hh.conj()))[0]
+                    csm1 = hmax * (hh * hh.conj().T)
+
+                    # h1 = self.steer._beamformerCall(f[i], self.r_diag, normFactor, (array((hmax, ))[newaxis, :], hh[newaxis, :].conjugate()))[0]
+                    h1 = beamformerFreq(
+                        param_steer_type,
+                        self.r_diag,
+                        normFactor,
+                        steer_vector(f[i]),
+                        (array((hmax,)), hh.conj()),
+                    )[0]
                     h -= self.damp * h1
-                    csm -= self.damp * csm1.T#transpose(0,2,1)
+                    csm -= self.damp * csm1.T  # transpose(0,2,1)
                 ac[i] = result
                 fr[i] = 1
 
-class BeamformerClean (BeamformerBase):
-    """
-    CLEAN deconvolution, see :ref:`Hoegbom, 1974<Hoegbom1974>`.
+
+class BeamformerClean(BeamformerBase):
+    """CLEAN deconvolution, see :ref:`Hoegbom, 1974<Hoegbom1974>`.
     Needs a-priori delay-and-sum beamforming (:class:`BeamformerBase`).
     """
 
     # BeamformerBase object that provides data for deconvolution
     beamformer = Trait(BeamformerBase)
 
     # PowerSpectra object that provides the cross spectral matrix
     freq_data = Delegate('beamformer')
 
     # flag, if true (default), the main diagonal is removed before beamforming
-    #r_diag =  Delegate('beamformer')
-    
+    # r_diag =  Delegate('beamformer')
+
     #: instance of :class:`~acoular.fbeamform.SteeringVector` or its derived classes,
     #: that contains information about the steering vector. Is set automatically.
     steer = Delegate('beamformer')
-    
+
     #: Floating point precision of result, is set automatically.
     precision = Delegate('beamformer')
-    
+
     #: The floating-number-precision of the PSFs. Default is 64 bit.
-    psf_precision = Trait('float64', 'float32', 
-                     desc="precision of PSF.")
-    
+    psf_precision = Trait('float64', 'float32', desc='precision of PSF.')
+
     # iteration damping factor
     # defaults to 0.6
-    damp = Range(0.01, 1.0, 0.6, 
-        desc="damping factor")
-        
+    damp = Range(0.01, 1.0, 0.6, desc='damping factor')
+
     # max number of iterations
-    n_iter = Int(100, 
-        desc="maximum number of iterations")
+    n_iter = Int(100, desc='maximum number of iterations')
 
     # how to calculate and store the psf
-    calcmode = Trait('block', 'full', 'single', 'readonly',
-                     desc="mode of psf calculation / storage")
-                     
+    calcmode = Trait('block', 'full', 'single', 'readonly', desc='mode of psf calculation / storage')
+
     # internal identifier
-    digest = Property( 
-        depends_on = ['beamformer.digest', 'n_iter', 'damp', 'psf_precision'], 
-        )
+    digest = Property(
+        depends_on=['beamformer.digest', 'n_iter', 'damp', 'psf_precision'],
+    )
 
     # internal identifier
-    ext_digest = Property( 
-        depends_on = ['digest', 'beamformer.ext_digest'], 
-        )
-    
+    ext_digest = Property(
+        depends_on=['digest', 'beamformer.ext_digest'],
+    )
+
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
-      
+    def _get_digest(self):
+        return digest(self)
+
     @cached_property
-    def _get_ext_digest( self ):
-        return digest( self, 'ext_digest' )
-    
+    def _get_ext_digest(self):
+        return digest(self, 'ext_digest')
+
     def calc(self, ac, fr):
-        """
-        Calculates the CLEAN result for the frequencies defined by :attr:`freq_data`
-        
-        This is an internal helper function that is automatically called when 
+        """Calculates the CLEAN result for the frequencies defined by :attr:`freq_data`.
+
+        This is an internal helper function that is automatically called when
         accessing the beamformer's :attr:`~BeamformerBase.result` or calling
-        its :meth:`~BeamformerBase.synthetic` method.        
-        
+        its :meth:`~BeamformerBase.synthetic` method.
+
         Parameters
         ----------
         ac : array of floats
             This array of dimension ([number of frequencies]x[number of gridpoints])
             is used as call-by-reference parameter and contains the calculated
-            value after calling this method. 
+            value after calling this method.
         fr : array of booleans
-            The entries of this [number of frequencies]-sized array are either 
+            The entries of this [number of frequencies]-sized array are either
             'True' (if the result for this frequency has already been calculated)
             or 'False' (for the frequencies where the result has yet to be calculated).
             After the calculation at a certain frequency the value will be set
             to 'True'
-        
+
         Returns
         -------
         This method only returns values through the *ac* and *fr* parameters
+
         """
         f = self.freq_data.fftfreq()
         gs = self.steer.grid.size
-        
+
         if self.calcmode == 'full':
-            warn("calcmode = 'full', possibly slow CLEAN performance. "
-                 "Better use 'block' or 'single'.", Warning, stacklevel = 2)
+            warn(
+                "calcmode = 'full', possibly slow CLEAN performance. Better use 'block' or 'single'.",
+                Warning,
+                stacklevel=2,
+            )
         p = PointSpreadFunction(steer=self.steer, calcmode=self.calcmode, precision=self.psf_precision)
         for i in self.freq_data.indices:
             if not fr[i]:
                 p.freq = f[i]
                 dirty = self.beamformer.result[i].copy()
                 clean = zeros(gs, dtype=dirty.dtype)
-                
+
                 i_iter = 0
                 flag = True
                 while flag:
                     # TODO: negative werte!!!
                     dirty_sum = abs(dirty).sum(0)
                     next_max = dirty.argmax(0)
                     p.grid_indices = array([next_max])
-                    psf = p.psf.reshape(gs,)
-                    new_amp = self.damp * dirty[next_max] #/ psf[next_max]
+                    psf = p.psf.reshape(gs)
+                    new_amp = self.damp * dirty[next_max]  # / psf[next_max]
                     clean[next_max] += new_amp
                     dirty -= psf * new_amp
                     i_iter += 1
-                    flag = (dirty_sum > abs(dirty).sum(0) \
-                            and i_iter < self.n_iter \
-                            and max(dirty) > 0)
-                
-                ac[i] = clean            
+                    flag = dirty_sum > abs(dirty).sum(0) and i_iter < self.n_iter and max(dirty) > 0
+
+                ac[i] = clean
                 fr[i] = 1
 
-class BeamformerCMF ( BeamformerBase ):
-    """
-    Covariance Matrix Fitting, see :ref:`Yardibi et al., 2008<Yardibi2008>`.
+
+class BeamformerCMF(BeamformerBase):
+    """Covariance Matrix Fitting, see :ref:`Yardibi et al., 2008<Yardibi2008>`.
     This is not really a beamformer, but an inverse method.
     """
 
-    #: Type of fit method to be used ('LassoLars', 'LassoLarsBIC', 
+    #: Type of fit method to be used ('LassoLars', 'LassoLarsBIC',
     #: 'OMPCV' or 'NNLS', defaults to 'LassoLars').
-    #: These methods are implemented in 
-    #: the `scikit-learn <http://scikit-learn.org/stable/user_guide.html>`_ 
+    #: These methods are implemented in
+    #: the `scikit-learn <http://scikit-learn.org/stable/user_guide.html>`_
     #: module.
-    method = Trait('LassoLars', 'LassoLarsBIC',  \
-        'OMPCV', 'NNLS','fmin_l_bfgs_b','Split_Bregman','FISTA', desc="fit method used")
-        
+    method = Trait(
+        'LassoLars',
+        'LassoLarsBIC',
+        'OMPCV',
+        'NNLS',
+        'fmin_l_bfgs_b',
+        'Split_Bregman',
+        'FISTA',
+        desc='fit method used',
+    )
+
     #: Weight factor for LassoLars method,
     #: defaults to 0.0.
     #: (Use values in the order of 10^⁻9 for good results.)
-    alpha = Range(0.0, 1.0, 0.0, 
-        desc="Lasso weight factor")
-    
+    alpha = Range(0.0, 1.0, 0.0, desc='Lasso weight factor')
+
     #: Maximum number of iterations,
     #: tradeoff between speed and precision;
     #: defaults to 500
-    max_iter = Int(500, 
-        desc="maximum number of iterations")
+    max_iter = Int(500, desc='maximum number of iterations')
 
-    
-    #: Unit multiplier for evaluating, e.g., nPa instead of Pa. 
-    #: Values are converted back before returning. 
+    #: Unit multiplier for evaluating, e.g., nPa instead of Pa.
+    #: Values are converted back before returning.
     #: Temporary conversion may be necessary to not reach machine epsilon
     #: within fitting method algorithms. Defaults to 1e9.
-    unit_mult = Float(1e9,
-                      desc = "unit multiplier")
-    
+    unit_mult = Float(1e9, desc='unit multiplier')
+
     #: If True, shows the status of the PyLops solver. Only relevant in case of FISTA or Split_Bregman
-    show = Bool(False,
-                desc = "show output of PyLops solvers")
-    
+    show = Bool(False, desc='show output of PyLops solvers')
 
     # internal identifier
-    digest = Property( 
-        depends_on = ['freq_data.digest', 'alpha', 'method', 'max_iter', 'unit_mult', 'r_diag', 'steer.inv_digest'], 
-        )
+    digest = Property(
+        depends_on=['freq_data.digest', 'alpha', 'method', 'max_iter', 'unit_mult', 'r_diag', 'steer.inv_digest'],
+    )
 
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
-   
+    def _get_digest(self):
+        return digest(self)
+
+    @on_trait_change('method')
+    def _validate(self):
+        if self.method in ['FISTA', 'Split_Bregman'] and not config.have_pylops:
+            msg = (
+                'Cannot import Pylops package. No Pylops installed.'
+                f'Solver for {self.method} in BeamformerCMF not available.'
+            )
+            raise ImportError(msg)
 
     def calc(self, ac, fr):
-        """
-        Calculates the CMF result for the frequencies defined by :attr:`freq_data`
-        
-        This is an internal helper function that is automatically called when 
+        """Calculates the CMF result for the frequencies defined by :attr:`freq_data`.
+
+        This is an internal helper function that is automatically called when
         accessing the beamformer's :attr:`~BeamformerBase.result` or calling
-        its :meth:`~BeamformerBase.synthetic` method.        
-        
+        its :meth:`~BeamformerBase.synthetic` method.
+
         Parameters
         ----------
         ac : array of floats
             This array of dimension ([number of frequencies]x[number of gridpoints])
             is used as call-by-reference parameter and contains the calculated
-            value after calling this method. 
+            value after calling this method.
         fr : array of booleans
-            The entries of this [number of frequencies]-sized array are either 
+            The entries of this [number of frequencies]-sized array are either
             'True' (if the result for this frequency has already been calculated)
             or 'False' (for the frequencies where the result has yet to be calculated).
             After the calculation at a certain frequency the value will be set
             to 'True'
-        
+
         Returns
         -------
         This method only returns values through the *ac* and *fr* parameters
+
         """
-        
+
         # function to repack complex matrices to deal with them in real number space
         def realify(M):
-            return vstack([M.real,M.imag])
+            return vstack([M.real, M.imag])
 
-            
         # prepare calculation
         i = self.freq_data.indices
         f = self.freq_data.fftfreq()
         nc = self.freq_data.numchannels
         numpoints = self.steer.grid.size
         unit = self.unit_mult
 
-        for i in self.freq_data.indices:        
+        for i in self.freq_data.indices:
             if not fr[i]:
-                csm = array(self.freq_data.csm[i], dtype='complex128',copy=1)
+                csm = array(self.freq_data.csm[i], dtype='complex128', copy=1)
 
                 h = self.steer.transfer(f[i]).T
-                
+
                 # reduced Kronecker product (only where solution matrix != 0)
-                Bc = ( h[:,:,newaxis] * \
-                       h.conjugate().T[newaxis,:,:] )\
-                         .transpose(2,0,1)
-                Ac = Bc.reshape(nc*nc,numpoints)
-                
+                Bc = (h[:, :, newaxis] * h.conjugate().T[newaxis, :, :]).transpose(2, 0, 1)
+                Ac = Bc.reshape(nc * nc, numpoints)
+
                 # get indices for upper triangular matrices (use tril b/c transposed)
-                ind = reshape(tril(ones((nc,nc))), (nc*nc,)) > 0
-                
-                ind_im0 = (reshape(eye(nc),(nc*nc,)) == 0)[ind]
+                ind = reshape(tril(ones((nc, nc))), (nc * nc,)) > 0
+
+                ind_im0 = (reshape(eye(nc), (nc * nc,)) == 0)[ind]
                 if self.r_diag:
                     # omit main diagonal for noise reduction
                     ind_reim = hstack([ind_im0, ind_im0])
                 else:
                     # take all real parts -- also main diagonal
-                    ind_reim = hstack([ones(size(ind_im0),)>0,ind_im0])
-                    ind_reim[0]=True # why this ?
+                    ind_reim = hstack([ones(size(ind_im0)) > 0, ind_im0])
+                    ind_reim[0] = True  # why this ?
 
-                A = realify( Ac [ind,:] )[ind_reim,:]
+                A = realify(Ac[ind, :])[ind_reim, :]
                 # use csm.T for column stacking reshape!
-                R = realify( reshape(csm.T, (nc*nc,1))[ind,:] )[ind_reim,:] * unit
+                R = realify(reshape(csm.T, (nc * nc, 1))[ind, :])[ind_reim, :] * unit
                 # choose method
                 if self.method == 'LassoLars':
-                    model = LassoLars(alpha = self.alpha * unit,
-                                      max_iter = self.max_iter,
-                                      **sklearn_ndict)
+                    model = LassoLars(alpha=self.alpha * unit, max_iter=self.max_iter, **sklearn_ndict)
                 elif self.method == 'LassoLarsBIC':
-                    model = LassoLarsIC(criterion = 'bic',
-                                        max_iter = self.max_iter,
-                                        **sklearn_ndict)
+                    model = LassoLarsIC(criterion='bic', max_iter=self.max_iter, **sklearn_ndict)
                 elif self.method == 'OMPCV':
                     model = OrthogonalMatchingPursuitCV(**sklearn_ndict)
                 elif self.method == 'NNLS':
                     model = LinearRegression(positive=True)
 
-                if self.method == 'Split_Bregman' and PYLOPS_TRUE:   
-                    Oop = MatrixMult(A) #tranfer operator 
-                    Iop = self.alpha*Identity(numpoints) # regularisation 
-                    ac[i],iterations = SplitBregman(Oop, [Iop] , R[:,0], 
-                                                    niter_outer=self.max_iter, niter_inner=5,
-                                                    RegsL2=None, dataregsL2=None,
-                                                    mu=1.0, epsRL1s=[1],tol=1e-10, tau=1.0,
-                                                    show=self.show)
+                if self.method == 'Split_Bregman' and config.have_pylops:
+                    from pylops import Identity, MatrixMult, SplitBregman
+
+                    Oop = MatrixMult(A)  # tranfer operator
+                    Iop = self.alpha * Identity(numpoints)  # regularisation
+                    ac[i], iterations = SplitBregman(
+                        Oop,
+                        [Iop],
+                        R[:, 0],
+                        niter_outer=self.max_iter,
+                        niter_inner=5,
+                        RegsL2=None,
+                        dataregsL2=None,
+                        mu=1.0,
+                        epsRL1s=[1],
+                        tol=1e-10,
+                        tau=1.0,
+                        show=self.show,
+                    )
                     ac[i] /= unit
-                
-                elif self.method == 'FISTA' and PYLOPS_TRUE:   
-                    Oop= MatrixMult(A) #tranfer operator 
-                    ac[i],iterations = FISTA(Op=Oop, data= R[:,0],
-                                             niter=self.max_iter, eps=self.alpha,
-                                             alpha=None, eigsiter=None, eigstol=0, tol=1e-10,
-                                             show=self.show)
+
+                elif self.method == 'FISTA' and config.have_pylops:
+                    from pylops import FISTA, MatrixMult
+
+                    Oop = MatrixMult(A)  # tranfer operator
+                    ac[i], iterations = FISTA(
+                        Op=Oop,
+                        data=R[:, 0],
+                        niter=self.max_iter,
+                        eps=self.alpha,
+                        alpha=None,
+                        eigsiter=None,
+                        eigstol=0,
+                        tol=1e-10,
+                        show=self.show,
+                    )
                     ac[i] /= unit
-                elif self.method == 'FISTA' or self.method == 'Split_Bregman' and not PYLOPS_TRUE :
-                    raise Exception(f'No Pylops installed. Solver for {self.method} in BeamformerCMF not available.')
                 elif self.method == 'fmin_l_bfgs_b':
-                    #function to minimize
+                    # function to minimize
                     def function(x):
-                        #function
-                        func = x.T@A.T@A@x - 2*R.T@A@x + R.T@R                
-                        #derivitaive
-                        der = 2*A.T@A@x.T[:, newaxis] - 2*A.T@R 
-                        return  func[0].T, der[:,0]
-                    
+                        # function
+                        func = x.T @ A.T @ A @ x - 2 * R.T @ A @ x + R.T @ R
+                        # derivitaive
+                        der = 2 * A.T @ A @ x.T[:, newaxis] - 2 * A.T @ R
+                        return func[0].T, der[:, 0]
+
                     # initial guess
-                    x0 = ones([numpoints])   
-                    #boundarys - set to non negative
-                    boundarys = tile((0, +inf), (len(x0),1))
-                    
-                    #optimize
-                    ac[i], yval, dicts =  fmin_l_bfgs_b(function, x0, fprime=None, args=(),  
-                                                          approx_grad=0, bounds=boundarys, m=10,
-                                                          factr=10000000.0, pgtol=1e-05, epsilon=1e-08,
-                                                          iprint=-1, maxfun=15000, maxiter=self.max_iter,
-                                                          disp=None, callback=None, maxls=20)
-                    
+                    x0 = ones([numpoints])
+                    # boundarys - set to non negative
+                    boundarys = tile((0, +inf), (len(x0), 1))
+
+                    # optimize
+                    ac[i], yval, dicts = fmin_l_bfgs_b(
+                        function,
+                        x0,
+                        fprime=None,
+                        args=(),
+                        approx_grad=0,
+                        bounds=boundarys,
+                        m=10,
+                        factr=10000000.0,
+                        pgtol=1e-05,
+                        epsilon=1e-08,
+                        iprint=-1,
+                        maxfun=15000,
+                        maxiter=self.max_iter,
+                        disp=None,
+                        callback=None,
+                        maxls=20,
+                    )
+
                     ac[i] /= unit
                 else:
                     # from sklearn 1.2, normalize=True does not work the same way anymore and the pipeline
-                    # approach with StandardScaler does scale in a different way, thus we monkeypatch the 
+                    # approach with StandardScaler does scale in a different way, thus we monkeypatch the
                     # code and normalize ourselves to make results the same over different sklearn versions
                     norms = norm(A, axis=0)
                     # get rid of annoying sklearn warnings that appear for sklearn<1.2 despite any settings
                     with warnings.catch_warnings():
-                        warnings.simplefilter("ignore", category=FutureWarning)
+                        warnings.simplefilter('ignore', category=FutureWarning)
                         # normalized A
-                        model.fit(A/norms,R[:,0])
+                        model.fit(A / norms, R[:, 0])
                     # recover normalization in the coef's
                     ac[i] = model.coef_[:] / norms / unit
                 fr[i] = 1
-                
-
 
 
-class BeamformerSODIX( BeamformerBase ):
-    """
-    SODIX, see Funke, Ein Mikrofonarray-Verfahren zur Untersuchung der
-    Schallabstrahlung von Turbofantriebwerken, 2017. and 
+class BeamformerSODIX(BeamformerBase):
+    """SODIX, see Funke, Ein Mikrofonarray-Verfahren zur Untersuchung der
+    Schallabstrahlung von Turbofantriebwerken, 2017. and
     Oertwig, Advancements in the source localization method SODIX and
-    application to short cowl engine data, 2019
-    
+    application to short cowl engine data, 2019.
+
     Source directivity modeling in the cross-spectral matrix
     """
+
     #: Type of fit method to be used ('fmin_l_bfgs_b').
-    #: These methods are implemented in 
+    #: These methods are implemented in
     #: the scipy module.
-    method = Trait('fmin_l_bfgs_b', desc="fit method used")
-        
+    method = Trait('fmin_l_bfgs_b', desc='fit method used')
+
     #: Maximum number of iterations,
     #: tradeoff between speed and precision;
     #: defaults to 200
-    max_iter = Int(200, 
-        desc="maximum number of iterations")
-    
-    #: Norm to consider for the regularization 
+    max_iter = Int(200, desc='maximum number of iterations')
+
+    #: Norm to consider for the regularization
     #: defaults to L-1 Norm
-    pnorm= Float(1,desc="Norm for regularization")
-    
+    pnorm = Float(1, desc='Norm for regularization')
+
     #: Weight factor for regularization,
     #: defaults to 0.0.
-    alpha = Range(0.0, 1.0, 0.0, 
-        desc="regularization factor")
+    alpha = Range(0.0, 1.0, 0.0, desc='regularization factor')
 
-    #: Unit multiplier for evaluating, e.g., nPa instead of Pa. 
-    #: Values are converted back before returning. 
+    #: Unit multiplier for evaluating, e.g., nPa instead of Pa.
+    #: Values are converted back before returning.
     #: Temporary conversion may be necessary to not reach machine epsilon
     #: within fitting method algorithms. Defaults to 1e9.
-    unit_mult = Float(1e9,
-                      desc = "unit multiplier")
-    
-    #: The beamforming result as squared sound pressure values 
+    unit_mult = Float(1e9, desc='unit multiplier')
+
+    #: The beamforming result as squared sound pressure values
     #: at all grid point locations (readonly).
     #: Returns a (number of frequencies, number of gridpoints) array of floats.
-    sodix_result = Property(
-        desc="beamforming result")
+    sodix_result = Property(desc='beamforming result')
 
     # internal identifier
-    digest = Property( 
-        depends_on = ['freq_data.digest', 'alpha', 'method', 'max_iter', 'unit_mult', 'r_diag', 'steer.inv_digest'], 
-        )
+    digest = Property(
+        depends_on=['freq_data.digest', 'alpha', 'method', 'max_iter', 'unit_mult', 'r_diag', 'steer.inv_digest'],
+    )
 
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
-    
-    def _get_filecache( self ):
-            """
-            function collects cached results from file depending on 
-            global/local caching behaviour. Returns (None, None) if no cachefile/data 
-            exist and global caching mode is 'readonly'.
-            """
-            H5cache.get_cache_file( self, self.freq_data.basename ) 
-            if not self.h5f: 
-                return (None, None)# only happens in case of global caching readonly
-    
-            nodename = self.__class__.__name__ + self.digest
-            if config.global_caching == 'overwrite' and self.h5f.is_cached(nodename):
-                self.h5f.remove_data(nodename) # remove old data before writing in overwrite mode
-            
-            if not self.h5f.is_cached(nodename):
-                if config.global_caching == 'readonly': 
-                    return (None, None)
-                else:
-    #                print("initialize data.")
-                    numfreq = self.freq_data.fftfreq().shape[0]# block_size/2 + 1steer_obj
-                    group = self.h5f.create_new_group(nodename)
-                    self.h5f.create_compressible_array('result',
-                                          (numfreq, self.steer.grid.size*self.steer.mics.num_mics),
-                                          self.precision,
-                                          group)
-                    self.h5f.create_compressible_array('freqs',
-                                          (numfreq, ),
-                                          'int8',#'bool', 
-                                          group)
-            ac = self.h5f.get_data_by_reference('result','/'+nodename)
-            fr = self.h5f.get_data_by_reference('freqs','/'+nodename)
-            gpos = None
-            return (ac,fr,gpos) 
-    
-    @property_depends_on('ext_digest')
-    def _get_sodix_result ( self ):
+    def _get_digest(self):
+        return digest(self)
+
+    def _get_filecache(self):
+        """Function collects cached results from file depending on
+        global/local caching behaviour. Returns (None, None) if no cachefile/data
+        exist and global caching mode is 'readonly'.
         """
-        This is the :attr:`result` getter routine.
+        H5cache.get_cache_file(self, self.freq_data.basename)
+        if not self.h5f:
+            return (None, None)  # only happens in case of global caching readonly
+
+        nodename = self.__class__.__name__ + self.digest
+        if config.global_caching == 'overwrite' and self.h5f.is_cached(nodename):
+            self.h5f.remove_data(nodename)  # remove old data before writing in overwrite mode
+
+        if not self.h5f.is_cached(nodename):
+            if config.global_caching == 'readonly':
+                return (None, None)
+            #                print("initialize data.")
+            numfreq = self.freq_data.fftfreq().shape[0]  # block_size/2 + 1steer_obj
+            group = self.h5f.create_new_group(nodename)
+            self.h5f.create_compressible_array(
+                'result',
+                (numfreq, self.steer.grid.size * self.steer.mics.num_mics),
+                self.precision,
+                group,
+            )
+            self.h5f.create_compressible_array(
+                'freqs',
+                (numfreq,),
+                'int8',  #'bool',
+                group,
+            )
+        ac = self.h5f.get_data_by_reference('result', '/' + nodename)
+        fr = self.h5f.get_data_by_reference('freqs', '/' + nodename)
+        gpos = None
+        return (ac, fr, gpos)
+
+    @property_depends_on('ext_digest')
+    def _get_sodix_result(self):
+        """Implements the :attr:`result` getter routine.
         The sodix beamforming result is either loaded or calculated.
         """
         f = self.freq_data
-        numfreq = f.fftfreq().shape[0]# block_size/2 + 1steer_obj
+        numfreq = f.fftfreq().shape[0]  # block_size/2 + 1steer_obj
         _digest = ''
         while self.digest != _digest:
             _digest = self.digest
             self._assert_equal_channels()
-            if not ( # if result caching is active
-                    config.global_caching == 'none' or 
-                    (config.global_caching == 'individual' and self.cached == False)
-                ):
-                (ac,fr,gpos) = self._get_filecache() 
-                if ac and fr: 
-                    if not fr[f.ind_low:f.ind_high].all():                       
-                        if config.global_caching == 'readonly': 
+            if not (  # if result caching is active
+                config.global_caching == 'none' or (config.global_caching == 'individual' and not self.cached)
+            ):
+                (ac, fr, gpos) = self._get_filecache()
+                if ac and fr:
+                    if not fr[f.ind_low : f.ind_high].all():
+                        if config.global_caching == 'readonly':
                             (ac, fr) = (ac[:], fr[:])
-                        self.calc(ac,fr)
+                        self.calc(ac, fr)
                         self.h5f.flush()
 
                 else:
-                    ac = zeros((numfreq, self.steer.grid.size*self.steer.mics.num_mics), dtype=self.precision)
+                    ac = zeros((numfreq, self.steer.grid.size * self.steer.mics.num_mics), dtype=self.precision)
                     fr = zeros(numfreq, dtype='int8')
-                    self.calc(ac,fr)
+                    self.calc(ac, fr)
             else:
-                ac = zeros((numfreq, self.steer.grid.size*self.steer.mics.num_mics), dtype=self.precision)
+                ac = zeros((numfreq, self.steer.grid.size * self.steer.mics.num_mics), dtype=self.precision)
                 fr = zeros(numfreq, dtype='int8')
-                self.calc(ac,fr)
+                self.calc(ac, fr)
         return ac
-    
-    def synthetic( self, f, num=0):
-        """
-        Evaluates the beamforming result for an arbitrary frequency band.
-        
+
+    def synthetic(self, f, num=0):
+        """Evaluates the beamforming result for an arbitrary frequency band.
+
         Parameters
         ----------
         f: float
-            Band center frequency. 
+            Band center frequency.
         num : integer
             Controls the width of the frequency bands considered; defaults to
             0 (single frequency line).
-            
+
             ===  =====================
             num  frequency band width
             ===  =====================
             0    single frequency line
             1    octave band
             3    third-octave band
             n    1/n-octave band
             ===  =====================
-              
+
         Returns
         -------
         array of floats
-            The synthesized frequency band values of the beamforming result at 
+            The synthesized frequency band values of the beamforming result at
             each grid point and each microphone .
-            Note that the frequency resolution and therefore the bandwidth 
-            represented by a single frequency line depends on 
+            Note that the frequency resolution and therefore the bandwidth
+            represented by a single frequency line depends on
             the :attr:`sampling frequency<acoular.sources.SamplesGenerator.sample_freq>` and conjugate
             used :attr:`FFT block size<acoular.spectra.PowerSpectra.block_size>`.
+
         """
-        res = self.sodix_result # trigger calculation
+        res = self.sodix_result  # trigger calculation
         freq = self.freq_data.fftfreq()
         if len(freq) == 0:
             return None
-        
+
         indices = self.freq_data.indices
-        
+
         if num == 0:
             # single frequency line
             ind = searchsorted(freq, f)
             if ind >= len(freq):
-                warn('Queried frequency (%g Hz) not in resolved '
-                              'frequency range. Returning zeros.' % f, 
-                              Warning, stacklevel = 2)
+                warn(
+                    'Queried frequency (%g Hz) not in resolved frequency range. Returning zeros.' % f,
+                    Warning,
+                    stacklevel=2,
+                )
                 h = zeros_like(res[0])
             else:
                 if freq[ind] != f:
-                    warn('Queried frequency (%g Hz) not in set of '
-                         'discrete FFT sample frequencies. '
-                         'Using frequency %g Hz instead.' % (f,freq[ind]), 
-                         Warning, stacklevel = 2)
-                if not (ind in indices):
-                    warn('Beamforming result may not have been calculated '
-                         'for queried frequency. Check '
-                         'freq_data.ind_low and freq_data.ind_high!',
-                          Warning, stacklevel = 2)
+                    warn(
+                        f'Queried frequency ({f:g} Hz) not in set of '
+                        'discrete FFT sample frequencies. '
+                        f'Using frequency {freq[ind]:g} Hz instead.',
+                        Warning,
+                        stacklevel=2,
+                    )
+                if ind not in indices:
+                    warn(
+                        'Beamforming result may not have been calculated '
+                        'for queried frequency. Check '
+                        'freq_data.ind_low and freq_data.ind_high!',
+                        Warning,
+                        stacklevel=2,
+                    )
                 h = res[ind]
         else:
             # fractional octave band
-            f1 = f*2.**(-0.5/num)
-            f2 = f*2.**(+0.5/num)
+            f1 = f * 2.0 ** (-0.5 / num)
+            f2 = f * 2.0 ** (+0.5 / num)
             ind1 = searchsorted(freq, f1)
             ind2 = searchsorted(freq, f2)
             if ind1 == ind2:
-                warn('Queried frequency band (%g to %g Hz) does not '
-                     'include any discrete FFT sample frequencies. '
-                     'Returning zeros.' % (f1,f2), 
-                     Warning, stacklevel = 2)
+                warn(
+                    f'Queried frequency band ({f1:g} to {f2:g} Hz) does not '
+                    'include any discrete FFT sample frequencies. '
+                    'Returning zeros.',
+                    Warning,
+                    stacklevel=2,
+                )
                 h = zeros_like(res[0])
             else:
                 h = sum(res[ind1:ind2], 0)
                 if not ((ind1 in indices) and (ind2 in indices)):
-                    warn('Beamforming result may not have been calculated '
-                         'for all queried frequencies. Check '
-                         'freq_data.ind_low and freq_data.ind_high!',
-                          Warning, stacklevel = 2)
-        return h.reshape([self.steer.grid.size,self.steer.mics.num_mics])
-   
+                    warn(
+                        'Beamforming result may not have been calculated '
+                        'for all queried frequencies. Check '
+                        'freq_data.ind_low and freq_data.ind_high!',
+                        Warning,
+                        stacklevel=2,
+                    )
+        return h.reshape([self.steer.grid.size, self.steer.mics.num_mics])
 
     def calc(self, ac, fr):
-        """
-        Calculates the SODIX result for the frequencies defined by :attr:`freq_data`
-        
-        This is an internal helper function that is automatically called when 
+        """Calculates the SODIX result for the frequencies defined by :attr:`freq_data`.
+
+        This is an internal helper function that is automatically called when
         accessing the beamformer's :attr:`~Beamformer.sodix_result` or calling
-        its :meth:`~BeamformerSODIX.synthetic` method.        
-        
+        its :meth:`~BeamformerSODIX.synthetic` method.
+
         Parameters
         ----------
         ac : array of floats
             This array of dimension ([number of frequencies]x[number of gridpoints]x[number of microphones])
             is used as call-by-reference parameter and contains the calculated
-            value after calling this method. 
+            value after calling this method.
         fr : array of booleans
-            The entries of this [number of frequencies]-sized array are either 
+            The entries of this [number of frequencies]-sized array are either
             'True' (if the result for this frequency has already been calculated)
             or 'False' (for the frequencies where the result has yet to be calculated).
             After the calculation at a certain frequency the value will be set
             to 'True'
-        
+
         Returns
         -------
         This method only returns values through the *ac* and *fr* parameters
+
         """
-        
         # prepare calculation
         i = self.freq_data.indices
         f = self.freq_data.fftfreq()
         numpoints = self.steer.grid.size
-        #unit = self.unit_mult
+        # unit = self.unit_mult
         num_mics = self.steer.mics.num_mics
 
-        for i in self.freq_data.indices:        
+        for i in self.freq_data.indices:
             if not fr[i]:
-                
-                #measured csm
-                csm = array(self.freq_data.csm[i], dtype='complex128',copy=1) 
-                #transfer function
-                h = self.steer.transfer(f[i]).T           
-                   
+                # measured csm
+                csm = array(self.freq_data.csm[i], dtype='complex128', copy=1)
+                # transfer function
+                h = self.steer.transfer(f[i]).T
+
                 if self.method == 'fmin_l_bfgs_b':
-                    #function to minimize
-                    def function(D): 
-                        '''
-                        Parameters
+                    # function to minimize
+                    def function(D):
+                        """Parameters
                         ----------
-                        D 
+                        D
                         [numpoints*num_mics]
-                        
+
                         Returns
                         -------
                         func - Sodix function to optimize
                              [1]
                         derdrl - derivitaives in direction of D
                             [num_mics*numpoints].
 
-                        '''           
+                        """
                         #### the sodix function ####
-                        Djm = D.reshape([numpoints,num_mics])
+                        Djm = D.reshape([numpoints, num_mics])
                         p = h.T * Djm
                         csm_mod = dot(p.T, p.conj())
                         Q = csm - csm_mod
-                        func = sum((absolute(Q))**2)
+                        func = sum((absolute(Q)) ** 2)
 
                         # subscripts and operands for numpy einsum and einsum_path
                         subscripts = 'rl,rm,ml->rl'
-                        operands = (h.T,h.T.conj()*Djm,Q)
+                        operands = (h.T, h.T.conj() * Djm, Q)
                         es_path = einsum_path(subscripts, *operands, optimize='greedy')[0]
 
                         #### the sodix derivative ####
                         derdrl = einsum(subscripts, *operands, optimize=es_path)
                         derdrl = -4 * real(derdrl)
                         return func, derdrl.ravel()
 
-                    ##### initial guess #### 
-                    if all(ac[(i-1)]==0):
-                         D0 = ones([numpoints,num_mics])
+                    ##### initial guess ####
+                    if all(ac[(i - 1)] == 0):
+                        D0 = ones([numpoints, num_mics])
                     else:
-                         D0 = sqrt(ac[(i-1)]*
-                             real((trace(csm)/trace(array(self.freq_data.csm[i-1], dtype='complex128',copy=1)))))
-                    
-                    #boundarys - set to non negative [2*(numpoints*num_mics)]
-                    boundarys = tile((0, +inf), (numpoints*num_mics,1))
-
-                    #optimize with gradient solver
-                    # see https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.fmin_l_bfgs_b.html                    
-
-                    qi = ones([numpoints,num_mics])
-                    qi, yval, dicts =  fmin_l_bfgs_b(function, D0, fprime=None, args=(),
-                                                         approx_grad=0, bounds=boundarys, 
-                                                         factr=100.0, pgtol=1e-12, epsilon=1e-08,
-                                                          iprint=-1, maxfun=1500000, maxiter=self.max_iter,
-                                                          disp=-1, callback=None, maxls=20)
-                    #squared pressure
-                    ac[i]=qi**2
+                        D0 = sqrt(
+                            ac[(i - 1)]
+                            * real(trace(csm) / trace(array(self.freq_data.csm[i - 1], dtype='complex128', copy=1))),
+                        )
+
+                    # boundarys - set to non negative [2*(numpoints*num_mics)]
+                    boundarys = tile((0, +inf), (numpoints * num_mics, 1))
+
+                    # optimize with gradient solver
+                    # see https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.fmin_l_bfgs_b.html
+
+                    qi = ones([numpoints, num_mics])
+                    qi, yval, dicts = fmin_l_bfgs_b(
+                        function,
+                        D0,
+                        fprime=None,
+                        args=(),
+                        approx_grad=0,
+                        bounds=boundarys,
+                        factr=100.0,
+                        pgtol=1e-12,
+                        epsilon=1e-08,
+                        iprint=-1,
+                        maxfun=1500000,
+                        maxiter=self.max_iter,
+                        disp=-1,
+                        callback=None,
+                        maxls=20,
+                    )
+                    # squared pressure
+                    ac[i] = qi**2
                 else:
                     pass
                 fr[i] = 1
 
-                
-                
-                
-                
-class BeamformerGIB(BeamformerEig):  #BeamformerEig #BeamformerBase
-    """
-    Beamforming GIB methods with different normalizations,
-    """
-    
-    #: Unit multiplier for evaluating, e.g., nPa instead of Pa. 
-    #: Values are converted back before returning. 
+
+class BeamformerGIB(BeamformerEig):  # BeamformerEig #BeamformerBase
+    """Beamforming GIB methods with different normalizations,."""
+
+    #: Unit multiplier for evaluating, e.g., nPa instead of Pa.
+    #: Values are converted back before returning.
     #: Temporary conversion may be necessary to not reach machine epsilon
     #: within fitting method algorithms. Defaults to 1e9.
-    unit_mult = Float(1e9,
-                      desc = "unit multiplier")
+    unit_mult = Float(1e9, desc='unit multiplier')
 
     #: Maximum number of iterations,
     #: tradeoff between speed and precision;
     #: defaults to 10
-    max_iter = Int(10, 
-                   desc="maximum number of iterations")
+    max_iter = Int(10, desc='maximum number of iterations')
 
-    #: Type of fit method to be used ('Suzuki', 'LassoLars', 'LassoLarsCV', 'LassoLarsBIC', 
+    #: Type of fit method to be used ('Suzuki', 'LassoLars', 'LassoLarsCV', 'LassoLarsBIC',
     #: 'OMPCV' or 'NNLS', defaults to 'Suzuki').
-    #: These methods are implemented in 
-    #: the `scikit-learn <http://scikit-learn.org/stable/user_guide.html>`_ 
+    #: These methods are implemented in
+    #: the `scikit-learn <http://scikit-learn.org/stable/user_guide.html>`_
     #: module.
-    method = Trait('Suzuki', 'InverseIRLS', 'LassoLars', 'LassoLarsBIC','LassoLarsCV',  \
-        'OMPCV', 'NNLS', desc="fit method used")
+    method = Trait(
+        'Suzuki',
+        'InverseIRLS',
+        'LassoLars',
+        'LassoLarsBIC',
+        'LassoLarsCV',
+        'OMPCV',
+        'NNLS',
+        desc='fit method used',
+    )
 
     #: Weight factor for LassoLars method,
     #: defaults to 0.0.
-    alpha = Range(0.0, 1.0, 0.0, 
-        desc="Lasso weight factor")
-    # (use values in the order of 10^⁻9 for good results) 
-    
-    #: Norm to consider for the regularization in InverseIRLS and Suzuki methods 
+    alpha = Range(0.0, 1.0, 0.0, desc='Lasso weight factor')
+    # (use values in the order of 10^⁻9 for good results)
+
+    #: Norm to consider for the regularization in InverseIRLS and Suzuki methods
     #: defaults to L-1 Norm
-    pnorm= Float(1,desc="Norm for regularization")
+    pnorm = Float(1, desc='Norm for regularization')
 
     #: Beta - Fraction of sources maintained after each iteration
-    #: defaults to 0.9 
-    beta =  Float(0.9,desc="fraction of sources maintained")
-    
+    #: defaults to 0.9
+    beta = Float(0.9, desc='fraction of sources maintained')
+
     #: eps - Regularization parameter for Suzuki algorithm
-    #: defaults to 0.05. 
-    eps_perc =  Float(0.05,desc="regularization parameter")
+    #: defaults to 0.05.
+    eps_perc = Float(0.05, desc='regularization parameter')
 
-    # This feature is not fully supported may be changed in the next release 
+    # This feature is not fully supported may be changed in the next release
     # First eigenvalue to consider. Defaults to 0.
-    m = Int(0,
-                      desc = "First eigenvalue to consider")
-    
-    
+    m = Int(0, desc='First eigenvalue to consider')
+
     # internal identifier++++++++++++++++++++++++++++++++++++++++++++++++++
-    digest = Property( 
-        depends_on = ['steer.inv_digest', 'freq_data.digest', \
-            'alpha', 'method', 'max_iter', 'unit_mult', 'eps_perc',\
-            'pnorm', 'beta','n', 'm'], 
-        )
+    digest = Property(
+        depends_on=[
+            'steer.inv_digest',
+            'freq_data.digest',
+            'alpha',
+            'method',
+            'max_iter',
+            'unit_mult',
+            'eps_perc',
+            'pnorm',
+            'beta',
+            'n',
+            'm',
+        ],
+    )
 
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
-    
+    def _get_digest(self):
+        return digest(self)
+
     @property_depends_on('n')
-    def _get_na( self ):
+    def _get_na(self):
         na = self.n
         nm = self.steer.mics.num_mics
         if na < 0:
             na = max(nm + na, 0)
         return min(nm - 1, na)
 
     def calc(self, ac, fr):
-        
-        """
-        Calculates the result for the frequencies defined by :attr:`freq_data`
-        
-        This is an internal helper function that is automatically called when 
+        """Calculates the result for the frequencies defined by :attr:`freq_data`.
+
+        This is an internal helper function that is automatically called when
         accessing the beamformer's :attr:`~BeamformerBase.result` or calling
-        its :meth:`~BeamformerBase.synthetic` method.        
-        
+        its :meth:`~BeamformerBase.synthetic` method.
+
         Parameters
         ----------
         ac : array of floats
             This array of dimension ([number of frequencies]x[number of gridpoints])
             is used as call-by-reference parameter and contains the calculated
-            value after calling this method. 
+            value after calling this method.
         fr : array of booleans
-            The entries of this [number of frequencies]-sized array are either 
+            The entries of this [number of frequencies]-sized array are either
             'True' (if the result for this frequency has already been calculated)
             or 'False' (for the frequencies where the result has yet to be calculated).
             After the calculation at a certain frequency the value will be set
             to 'True'
-        
+
         Returns
         -------
         This method only returns values through the *ac* and *fr* parameters
 
-        """        
+        """
         # prepare calculation
         f = self.freq_data.fftfreq()
-        n = int(self.na)   #number of eigenvalues
-        m = int(self.m)    #number of first eigenvalue
-        numchannels = self.freq_data.numchannels   #number of channels
+        n = int(self.na)  # number of eigenvalues
+        m = int(self.m)  # number of first eigenvalue
+        numchannels = self.freq_data.numchannels  # number of channels
         numpoints = self.steer.grid.size
         hh = zeros((1, numpoints, numchannels), dtype='D')
-        
-        #Generate a cross spectral matrix, and perform the eigenvalue decomposition
-        for i in self.freq_data.indices:        
+
+        # Generate a cross spectral matrix, and perform the eigenvalue decomposition
+        for i in self.freq_data.indices:
             if not fr[i]:
-                #for monopole and source strenght Q needs to define density
-                #calculate a transfer matrix A 
+                # for monopole and source strenght Q needs to define density
+                # calculate a transfer matrix A
                 hh = self.steer.transfer(f[i])
-                A=hh.T                 
-                #eigenvalues and vectors               
-                csm = array(self.freq_data.csm[i], dtype='complex128',copy=1)
-                eva,eve=eigh(csm)
+                A = hh.T
+                # eigenvalues and vectors
+                csm = array(self.freq_data.csm[i], dtype='complex128', copy=1)
+                eva, eve = eigh(csm)
                 eva = eva[::-1]
-                eve = eve[:, ::-1] 
-                eva[eva < max(eva)/1e12] = 0 #set small values zo 0, lowers numerical errors in simulated data
-                #init sources    
-                qi=zeros([n+m,numpoints], dtype='complex128')
-                #Select the number of coherent modes to be processed referring to the eigenvalue distribution.
-                #for s in arange(n):  
-                for s in list(range(m,n+m)):
-                    if eva[s] > 0:                    
-                        #Generate the corresponding eigenmodes
-                        emode=array(sqrt(eva[s])*eve[:,s], dtype='complex128')
+                eve = eve[:, ::-1]
+                eva[eva < max(eva) / 1e12] = 0  # set small values zo 0, lowers numerical errors in simulated data
+                # init sources
+                qi = zeros([n + m, numpoints], dtype='complex128')
+                # Select the number of coherent modes to be processed referring to the eigenvalue distribution.
+                # for s in arange(n):
+                for s in list(range(m, n + m)):
+                    if eva[s] > 0:
+                        # Generate the corresponding eigenmodes
+                        emode = array(sqrt(eva[s]) * eve[:, s], dtype='complex128')
                         # choose method for computation
                         if self.method == 'Suzuki':
-                            leftpoints=numpoints
-                            locpoints=arange(numpoints)         
-                            weights=diag(ones(numpoints))             
-                            epsilon=arange(self.max_iter)              
-                            for it in arange(self.max_iter): 
-                                if numchannels<=leftpoints:
-                                    AWA= dot(dot(A[:,locpoints],weights),A[:,locpoints].conj().T)
-                                    epsilon[it] = max(absolute(eigvals(AWA)))*self.eps_perc
-                                    qi[s,locpoints]=dot(dot(dot(weights,A[:,locpoints].conj().T),inv(AWA+eye(numchannels)*epsilon[it])),emode)
-                                elif numchannels>leftpoints:
-                                    AA=dot(A[:,locpoints].conj().T,A[:,locpoints])
-                                    epsilon[it] = max(absolute(eigvals(AA)))*self.eps_perc
-                                    qi[s,locpoints]=dot(dot(inv(AA+inv(weights)*epsilon[it]),A[:,locpoints].conj().T),emode)                                                       
-                                if self.beta < 1 and it > 1:   
-                                    #Reorder from the greatest to smallest magnitude to define a reduced-point source distribution , and reform a reduced transfer matrix 
-                                    leftpoints=int(round(numpoints*self.beta**(it+1)))                                                                                          
-                                    idx = argsort(abs(qi[s,locpoints]))[::-1]   
-                                    #print(it, leftpoints, locpoints, idx )
-                                    locpoints= delete(locpoints,[idx[leftpoints::]])             
-                                    qix=zeros([n+m,leftpoints], dtype='complex128')                      
-                                    qix[s,:]=qi[s,locpoints]
-                                    #calc weights for next iteration 
-                                    weights=diag(absolute(qix[s,:])**(2-self.pnorm))    
-                                else:                          
-                                    weights=diag((absolute(qi[s,:])**(2-self.pnorm)))    
-                             
-                        elif self.method == 'InverseIRLS':                         
-                            weights=eye(numpoints)
-                            locpoints=arange(numpoints)
-                            for it in arange(self.max_iter): 
-                                if numchannels<=numpoints: 
-                                    wtwi=inv(dot(weights.T,weights))  
-                                    aH=A.conj().T                       
-                                    qi[s,:]=dot(dot(wtwi,aH),dot(inv(dot(A,dot(wtwi,aH))),emode))                            
-                                    weights=diag(absolute(qi[s,:])**((2-self.pnorm)/2))
-                                    weights=weights/sum(absolute(weights))                                 
-                                elif numchannels>numpoints:
-                                    wtw=dot(weights.T,weights)
-                                    qi[s,:]= dot(dot(inv(dot(dot(A.conj.T,wtw),A)),dot( A.conj().T,wtw)) ,emode)
-                                    weights=diag(absolute(qi[s,:])**((2-self.pnorm)/2))
-                                    weights=weights/sum(absolute(weights))                  
+                            leftpoints = numpoints
+                            locpoints = arange(numpoints)
+                            weights = diag(ones(numpoints))
+                            epsilon = arange(self.max_iter)
+                            for it in arange(self.max_iter):
+                                if numchannels <= leftpoints:
+                                    AWA = dot(dot(A[:, locpoints], weights), A[:, locpoints].conj().T)
+                                    epsilon[it] = max(absolute(eigvals(AWA))) * self.eps_perc
+                                    qi[s, locpoints] = dot(
+                                        dot(
+                                            dot(weights, A[:, locpoints].conj().T),
+                                            inv(AWA + eye(numchannels) * epsilon[it]),
+                                        ),
+                                        emode,
+                                    )
+                                elif numchannels > leftpoints:
+                                    AA = dot(A[:, locpoints].conj().T, A[:, locpoints])
+                                    epsilon[it] = max(absolute(eigvals(AA))) * self.eps_perc
+                                    qi[s, locpoints] = dot(
+                                        dot(inv(AA + inv(weights) * epsilon[it]), A[:, locpoints].conj().T),
+                                        emode,
+                                    )
+                                if self.beta < 1 and it > 1:
+                                    # Reorder from the greatest to smallest magnitude to define a reduced-point source distribution , and reform a reduced transfer matrix
+                                    leftpoints = int(round(numpoints * self.beta ** (it + 1)))
+                                    idx = argsort(abs(qi[s, locpoints]))[::-1]
+                                    # print(it, leftpoints, locpoints, idx )
+                                    locpoints = delete(locpoints, [idx[leftpoints::]])
+                                    qix = zeros([n + m, leftpoints], dtype='complex128')
+                                    qix[s, :] = qi[s, locpoints]
+                                    # calc weights for next iteration
+                                    weights = diag(absolute(qix[s, :]) ** (2 - self.pnorm))
+                                else:
+                                    weights = diag(absolute(qi[s, :]) ** (2 - self.pnorm))
+
+                        elif self.method == 'InverseIRLS':
+                            weights = eye(numpoints)
+                            locpoints = arange(numpoints)
+                            for _it in arange(self.max_iter):
+                                if numchannels <= numpoints:
+                                    wtwi = inv(dot(weights.T, weights))
+                                    aH = A.conj().T
+                                    qi[s, :] = dot(dot(wtwi, aH), dot(inv(dot(A, dot(wtwi, aH))), emode))
+                                    weights = diag(absolute(qi[s, :]) ** ((2 - self.pnorm) / 2))
+                                    weights = weights / sum(absolute(weights))
+                                elif numchannels > numpoints:
+                                    wtw = dot(weights.T, weights)
+                                    qi[s, :] = dot(dot(inv(dot(dot(A.conj.T, wtw), A)), dot(A.conj().T, wtw)), emode)
+                                    weights = diag(absolute(qi[s, :]) ** ((2 - self.pnorm) / 2))
+                                    weights = weights / sum(absolute(weights))
                         else:
-                            locpoints=arange(numpoints) 
+                            locpoints = arange(numpoints)
                             unit = self.unit_mult
-                            AB = vstack([hstack([A.real,-A.imag]),hstack([A.imag,A.real])])
-                            R  = hstack([emode.real.T,emode.imag.T]) * unit
+                            AB = vstack([hstack([A.real, -A.imag]), hstack([A.imag, A.real])])
+                            R = hstack([emode.real.T, emode.imag.T]) * unit
                             if self.method == 'LassoLars':
-                                model = LassoLars(alpha=self.alpha * unit,
-                                                  max_iter=self.max_iter)
+                                model = LassoLars(alpha=self.alpha * unit, max_iter=self.max_iter)
                             elif self.method == 'LassoLarsBIC':
-                                model = LassoLarsIC(criterion='bic',
-                                                    max_iter=self.max_iter)
+                                model = LassoLarsIC(criterion='bic', max_iter=self.max_iter)
                             elif self.method == 'OMPCV':
                                 model = OrthogonalMatchingPursuitCV()
                             elif self.method == 'LassoLarsCV':
                                 model = LassoLarsCV()
                             elif self.method == 'NNLS':
                                 model = LinearRegression(positive=True)
                             model.normalize = False
-                            # from sklearn 1.2, normalize=True does not work 
-                            # the same way anymore and the pipeline approach 
-                            # with StandardScaler does scale in a different 
+                            # from sklearn 1.2, normalize=True does not work
+                            # the same way anymore and the pipeline approach
+                            # with StandardScaler does scale in a different
                             # way, thus we monkeypatch the code and normalize
                             # ourselves to make results the same over different
                             # sklearn versions
                             norms = norm(AB, axis=0)
                             # get rid of annoying sklearn warnings that appear
                             # for sklearn<1.2 despite any settings
                             with warnings.catch_warnings():
-                                warnings.simplefilter("ignore",
-                                                      category=FutureWarning)
+                                warnings.simplefilter('ignore', category=FutureWarning)
                                 # normalized A
-                                model.fit(AB/norms,R)
+                                model.fit(AB / norms, R)
                             # recover normalization in the coef's
-                            qi_real,qi_imag = hsplit(model.coef_[:]/norms/unit, 2)
-                            #print(s,qi.size)    
-                            qi[s,locpoints] = qi_real+qi_imag*1j
+                            qi_real, qi_imag = hsplit(model.coef_[:] / norms / unit, 2)
+                            # print(s,qi.size)
+                            qi[s, locpoints] = qi_real + qi_imag * 1j
                     else:
-                        warn('Eigenvalue %g <= 0 for frequency index %g. Will not be calculated!' % (s, i),Warning, stacklevel = 2)
-                    #Generate source maps of all selected eigenmodes, and superpose source intensity for each source type.
+                        warn(
+                            f'Eigenvalue {s:g} <= 0 for frequency index {i:g}. Will not be calculated!',
+                            Warning,
+                            stacklevel=2,
+                        )
+                    # Generate source maps of all selected eigenmodes, and superpose source intensity for each source type.
                 temp = zeros(numpoints)
-                temp[locpoints] = sum(absolute(qi[:,locpoints])**2,axis=0)
+                temp[locpoints] = sum(absolute(qi[:, locpoints]) ** 2, axis=0)
                 ac[i] = temp
-                fr[i] = 1    
+                fr[i] = 1
+
+
+class BeamformerAdaptiveGrid(BeamformerBase, Grid):
+    """Base class for array methods without predefined grid."""
 
-class BeamformerAdaptiveGrid(BeamformerBase,Grid):
-    """
-    Base class for array methods without predefined grid
-    """
-    
     # the grid positions live in a shadow trait
     _gpos = Any
 
-    def _get_shape ( self ):
+    def _get_shape(self):
         return (self.size,)
 
-    def _get_gpos( self ):
+    def _get_gpos(self):
         return self._gpos
 
     def integrate(self, sector):
-        """
-        Integrates result map over a given sector.
-        
+        """Integrates result map over a given sector.
+
         Parameters
         ----------
         sector: :class:`~acoular.grids.Sector` or derived
             Gives the sector over which to integrate
-              
+
         Returns
         -------
         array of floats
             The spectrum (all calculated frequency bands) for the integrated sector.
+
         """
         if not isinstance(sector, Sector):
+            msg = (
+                f'Please use a sector derived instance of type :class:`~acoular.grids.Sector` '
+                f'instead of type {type(sector)}.'
+            )
             raise NotImplementedError(
-            f'Please use a sector derived instance of type :class:`~acoular.grids.Sector` '
-            f'instead of type {type(sector)}.'
+                msg,
             )
 
         ind = self.subdomain(sector)
         r = self.result
         h = zeros(r.shape[0])
         for i in range(r.shape[0]):
             h[i] = r[i][ind].sum()
         return h
 
+
 class BeamformerGridlessOrth(BeamformerAdaptiveGrid):
-    """
-    Orthogonal beamforming without predefined grid
-    """
+    """Orthogonal beamforming without predefined grid."""
 
     #: List of components to consider, use this to directly set the eigenvalues
     #: used in the beamformer. Alternatively, set :attr:`n`.
-    eva_list = CArray(dtype=int,
-        desc="components")
-        
-    #: Number of components to consider, defaults to 1. If set, 
+    eva_list = CArray(dtype=int, desc='components')
+
+    #: Number of components to consider, defaults to 1. If set,
     #: :attr:`eva_list` will contain
-    #: the indices of the n largest eigenvalues. Setting :attr:`eva_list` 
+    #: the indices of the n largest eigenvalues. Setting :attr:`eva_list`
     #: afterwards will override this value.
     n = Int(1)
 
     #: Geometrical bounds of the search domain to consider.
-    #: :attr:`bound` ist a list that contains exactly three tuple of 
-    #: (min,max) for each of the coordinates x, y, z. 
+    #: :attr:`bound` ist a list that contains exactly three tuple of
+    #: (min,max) for each of the coordinates x, y, z.
     #: Defaults to [(-1.,1.),(-1.,1.),(0.01,1.)]
-    bounds = List( Tuple(Float,Float), minlen=3, maxlen=3,
-        value = [(-1.,1.),(-1.,1.),(0.01,1.)])
+    bounds = List(Tuple(Float, Float), minlen=3, maxlen=3, value=[(-1.0, 1.0), (-1.0, 1.0), (0.01, 1.0)])
 
-    #: options dictionary for the SHGO solver, see 
+    #: options dictionary for the SHGO solver, see
     #: `scipy docs <https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.shgo.html>`_.
-    #: Default is Sobol sampling Nelder-Mead local minimizer, 256 initial sampling points 
+    #: Default is Sobol sampling Nelder-Mead local minimizer, 256 initial sampling points
     #: and 1 iteration
     shgo = Dict
 
     # internal identifier
-    digest = Property( 
-        depends_on = ['freq_data.digest', '_steer_obj.digest', 'r_diag', 
-            'eva_list','bounds','shgo'], 
-        )
-   
+    digest = Property(
+        depends_on=['freq_data.digest', '_steer_obj.digest', 'r_diag', 'eva_list', 'bounds', 'shgo'],
+    )
+
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
+    def _get_digest(self):
+        return digest(self)
 
     @on_trait_change('n')
     def set_eva_list(self):
-        """ sets the list of eigenvalues to consider """
-        self.eva_list = arange(-1, -1-self.n, -1)
+        """Sets the list of eigenvalues to consider."""
+        self.eva_list = arange(-1, -1 - self.n, -1)
 
     @on_trait_change('eva_list')
     def set_n(self):
-        """ sets the list of eigenvalues to consider """
+        """Sets the list of eigenvalues to consider."""
         self.n = self.eva_list.shape[0]
-    
+
     @property_depends_on('n')
-    def _get_size ( self ):
-        return self.n*self.freq_data.fftfreq().shape[0]
+    def _get_size(self):
+        return self.n * self.freq_data.fftfreq().shape[0]
 
     def calc(self, ac, fr):
-        """
-        Calculates the result for the frequencies defined by :attr:`freq_data`
-        
-        This is an internal helper function that is automatically called when 
+        """Calculates the result for the frequencies defined by :attr:`freq_data`.
+
+        This is an internal helper function that is automatically called when
         accessing the beamformer's :attr:`~BeamformerBase.result` or calling
-        its :meth:`~BeamformerBase.synthetic` method.        
-        
+        its :meth:`~BeamformerBase.synthetic` method.
+
         Parameters
         ----------
         ac : array of floats
             This array of dimension ([number of frequencies]x[number of gridpoints])
             is used as call-by-reference parameter and contains the calculated
-            value after calling this method. 
+            value after calling this method.
         fr : array of booleans
-            The entries of this [number of frequencies]-sized array are either 
+            The entries of this [number of frequencies]-sized array are either
             'True' (if the result for this frequency has already been calculated)
             or 'False' (for the frequencies where the result has yet to be calculated).
             After the calculation at a certain frequency the value will be set
             to 'True'
-        
+
         Returns
         -------
         This method only returns values through the *ac* and *fr* parameters
+
         """
         f = self.freq_data.fftfreq()
         numchannels = self.freq_data.numchannels
-        # eigenvalue number list in standard form from largest to smallest 
+        # eigenvalue number list in standard form from largest to smallest
         eva_list = unique(self.eva_list % self.steer.mics.num_mics)[::-1]
         steer_type = self.steer.steer_type
         if steer_type == 'custom':
-            raise NotImplementedError('custom steer_type is not implemented')
+            msg = 'custom steer_type is not implemented'
+            raise NotImplementedError(msg)
         mpos = self.steer.mics.mpos
         env = self.steer.env
-        shgo_opts = {'n':256,'iters':1,'sampling_method':'sobol',
-                        'options':{'local_iter':1},
-                        'minimizer_kwargs':{'method':'Nelder-Mead'}
-                        }
+        shgo_opts = {
+            'n': 256,
+            'iters': 1,
+            'sampling_method': 'sobol',
+            'options': {'local_iter': 1},
+            'minimizer_kwargs': {'method': 'Nelder-Mead'},
+        }
         shgo_opts.update(self.shgo)
         roi = []
         for x in self.bounds[0]:
             for y in self.bounds[1]:
                 for z in self.bounds[2]:
-                    roi.append((x,y,z))
+                    roi.append((x, y, z))
         self.steer.env.roi = array(roi).T
-        bmin = array(tuple(map(min,self.bounds)))
-        bmax = array(tuple(map(max,self.bounds)))
+        bmin = array(tuple(map(min, self.bounds)))
+        bmax = array(tuple(map(max, self.bounds)))
         for i in self.freq_data.indices:
             if not fr[i]:
                 eva = array(self.freq_data.eva[i], dtype='float64')
                 eve = array(self.freq_data.eve[i], dtype='complex128')
-                k = 2*pi*f[i]/env.c
-                for j,n in enumerate(eva_list):
-                    #print(f[i],n)
+                k = 2 * pi * f[i] / env.c
+                for j, n in enumerate(eva_list):
+                    # print(f[i],n)
 
                     def func(xy):
                         # function to minimize globally
-                        xy = clip(xy,bmin,bmax)
-                        r0 = env._r(xy[:,newaxis])
-                        rm = env._r(xy[:,newaxis],mpos)
-                        return -beamformerFreq(steer_type,
-                                                self.r_diag,
-                                                1.0,
-                                                (r0, rm, k),
-                                                (ones(1), eve[:,n:n+1]))[0][0]
+                        xy = clip(xy, bmin, bmax)
+                        r0 = env._r(xy[:, newaxis])
+                        rm = env._r(xy[:, newaxis], mpos)
+                        return -beamformerFreq(steer_type, self.r_diag, 1.0, (r0, rm, k), (ones(1), eve[:, n : n + 1]))[
+                            0
+                        ][0]  # noqa: B023
 
                     # simplical global homotopy optimizer
-                    oR = shgo(func,self.bounds,**shgo_opts)
+                    oR = shgo(func, self.bounds, **shgo_opts)
                     # index in grid
-                    ind = i*self.n+j 
+                    ind = i * self.n + j
                     # store result for position
-                    self._gpos[:,ind] = oR['x']
+                    self._gpos[:, ind] = oR['x']
                     # store result for level
-                    ac[i,ind] = eva[n]/numchannels
-                    #print(oR['x'],eva[n]/numchannels,oR)
+                    ac[i, ind] = eva[n] / numchannels
+                    # print(oR['x'],eva[n]/numchannels,oR)
                 fr[i] = 1
 
 
-def L_p ( x ):
-    """
-    Calculates the sound pressure level from the squared sound pressure.
-    
+def L_p(x):
+    r"""Calculates the sound pressure level from the squared sound pressure.
+
     :math:`L_p = 10 \lg ( x / 4\cdot 10^{-10})`
-    
+
     Parameters
     ----------
     x: array of floats
         The squared sound pressure values
-        
+
     Returns
     -------
     array of floats
-        The corresponding sound pressure levels in dB. 
+        The corresponding sound pressure levels in dB.
         If `x<0`, -350.0 dB is returned.
+
     """
     # new version to prevent division by zero warning for float32 arguments
-    return 10*log10(clip(x/4e-10,1e-35,None))
+    return 10 * log10(clip(x / 4e-10, 1e-35, None))
+
+
 #    return where(x>0, 10*log10(x/4e-10), -1000.)
 
+
 def integrate(data, grid, sector):
-    """
-    Integrates a sound pressure map over a given sector.
-    
+    """Integrates a sound pressure map over a given sector.
+
     This function can be applied on beamforming results to
     quantitatively analyze the sound pressure in a given sector.
-    If used with :meth:`Beamformer.result()<acoular.fbeamform.BeamformerBase.result>`, 
-    the output is identical to the result of the intrinsic 
+    If used with :meth:`Beamformer.result()<acoular.fbeamform.BeamformerBase.result>`,
+    the output is identical to the result of the intrinsic
     :meth:`Beamformer.integrate<acoular.fbeamform.BeamformerBase.integrate>` method.
-    It can, however, also be used with the 
+    It can, however, also be used with the
     :meth:`Beamformer.synthetic<acoular.fbeamform.BeamformerBase.synthetic>`
     output.
-    
+
     Parameters
     ----------
     data: array of floats
-        Contains the calculated squared sound pressure values in Pa**2.        
+        Contains the calculated squared sound pressure values in Pa**2.
         If data has the same number of entries than the number of grid points
         only one value is returned.
-        In case of a 2-D array with the second dimension identical 
+        In case of a 2-D array with the second dimension identical
         to the number of grid points an array containing as many entries as
         the first dimension is returned.
-    grid: Grid object 
-        Object of a :class:`~acoular.grids.Grid`-derived class 
-        that provides the grid locations.        
+    grid: Grid object
+        Object of a :class:`~acoular.grids.Grid`-derived class
+        that provides the grid locations.
     sector: array of floats or :class:`~acoular.grids.Sector`-derived object
-        Tuple with arguments for the `indices` method 
-        of a :class:`~acoular.grids.Grid`-derived class 
-        (e.g. :meth:`RectGrid.indices<acoular.grids.RectGrid.indices>` 
+        Tuple with arguments for the `indices` method
+        of a :class:`~acoular.grids.Grid`-derived class
+        (e.g. :meth:`RectGrid.indices<acoular.grids.RectGrid.indices>`
         or :meth:`RectGrid3D.indices<acoular.grids.RectGrid3D.indices>`).
         Possible sectors would be `array([xmin, ymin, xmax, ymax])`
         or `array([x, y, radius])`.
         Alternatively, a :class:`~acoular.grids.Sector`-derived object
         can be used.
-          
+
     Returns
     -------
     array of floats
         The spectrum (all calculated frequency bands) for the integrated sector.
+
     """
-    
     if isinstance(sector, Sector):
         ind = grid.subdomain(sector)
     elif hasattr(grid, 'indices'):
         ind = grid.indices(*sector)
     else:
+        msg = (
+            f'Grid of type {grid.__class__.__name__} does not have an indices method! '
+            f'Please use a sector derived instance of type :class:`~acoular.grids.Sector` '
+            'instead of type numpy.array.'
+        )
         raise NotImplementedError(
-        f'Grid of type {grid.__class__.__name__} does not have an indices method! '
-        f'Please use a sector derived instance of type :class:`~acoular.grids.Sector` '
-        'instead of type numpy.array.'
+            msg,
         )
-    
+
     gshape = grid.shape
     gsize = grid.size
-    if size(data) == gsize: # one value per grid point
+    if size(data) == gsize:  # one value per grid point
         h = data.reshape(gshape)[ind].sum()
     elif data.ndim == 2 and data.shape[1] == gsize:
         h = zeros(data.shape[0])
         for i in range(data.shape[0]):
             h[i] = data[i].reshape(gshape)[ind].sum()
     return h
```

### Comparing `acoular-24.3/acoular/grids.py` & `acoular-24.5/acoular/grids.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# -*- coding: utf-8 -*-
-#pylint: disable-msg=E0611, E1101, C0103, R0901, R0902, R0903, R0904, W0232
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 # Copyright (c) Acoular Development Team.
-#------------------------------------------------------------------------------
-"""Implements support for two- and threedimensional grids
+# ------------------------------------------------------------------------------
+"""Implements support for two- and threedimensional grids.
 
 .. autosummary::
     :toctree: generated/
 
     Grid
     RectGrid
     RectGrid3D
@@ -22,97 +20,133 @@
     PolySector
     ConvexSector
     MultiSector
 
 """
 
 # imports from other packages
-from numpy import mgrid, s_, array, arange, isscalar, absolute, ones, argmin,\
-zeros, where,  asfarray,concatenate,sum,ma,ones_like,inf,copysign,fabs ,append,\
-tile,newaxis, unique
+from os import path
+
+from numpy import (
+    absolute,
+    append,
+    arange,
+    argmin,
+    array,
+    asfarray,
+    concatenate,
+    copysign,
+    fabs,
+    inf,
+    isscalar,
+    ma,
+    mgrid,
+    newaxis,
+    ones,
+    ones_like,
+    s_,
+    sum,
+    tile,
+    unique,
+    where,
+    zeros,
+)
 from numpy.linalg import norm
-from traits.api import HasPrivateTraits, Float, Property, Any, \
-property_depends_on, cached_property, Bool, List, Instance, File ,on_trait_change,\
-CArray, Tuple, Int
-from traits.trait_errors import TraitError
-#from matplotlib.path import Path
+
+# from matplotlib.path import Path
 from scipy.spatial import Delaunay
-from os import path
+from traits.api import (
+    Any,
+    Bool,
+    CArray,
+    File,
+    Float,
+    HasPrivateTraits,
+    Instance,
+    Int,
+    List,
+    Property,
+    Tuple,
+    cached_property,
+    on_trait_change,
+    property_depends_on,
+)
+from traits.trait_errors import TraitError
+
 from .internal import digest
 
 
-def in_hull(p, hull, border= True, tol = 0 ):
-    """
-    test if points in `p` are in `hull`
+def in_hull(p, hull, border=True, tol=0):
+    """Test if points in `p` are in `hull`
     `p` should be a `NxK` coordinates of `N` points in `K` dimensions
-    `hull` is either a scipy.spatial.Delaunay object or the `MxK` array of the 
+    `hull` is either a scipy.spatial.Delaunay object or the `MxK` array of the
     coordinates of `M` points in `K`dimensions for which Delaunay triangulation
-    will be computed
+    will be computed.
     """
-    if not isinstance(hull,Delaunay):
+    if not isinstance(hull, Delaunay):
         hull = Delaunay(hull)
-    
+
     if border:
-        return hull.find_simplex(p,tol = tol)>=0
-    else:
-        return hull.find_simplex(p,tol = tol)>0
-        
+        return hull.find_simplex(p, tol=tol) >= 0
+    return hull.find_simplex(p, tol=tol) > 0
+
 
 def _det(xvert, yvert):
-    '''Compute twice the area of the triangle defined by points with using
+    """Compute twice the area of the triangle defined by points with using
     determinant formula.
 
     Input parameters:
 
     xvert -- A vector of nodal x-coords (array-like).
     yvert -- A vector of nodal y-coords (array-like).
 
     Output parameters:
     Twice the area of the triangle defined by the points.
 
-    Notes:
-
+    Notes
+    -----
     _det is positive if points define polygon in anticlockwise order.
     _det is negative if points define polygon in clockwise order.
     _det is zero if at least two of the points are concident or if
         all points are collinear.
 
-    '''
+    """
     xvert = asfarray(xvert)
     yvert = asfarray(yvert)
     x_prev = concatenate(([xvert[-1]], xvert[:-1]))
     y_prev = concatenate(([yvert[-1]], yvert[:-1]))
     return sum(yvert * x_prev - xvert * y_prev, axis=0)
 
 
 class Polygon:
-    '''Polygon object.
+    """Polygon object.
     Input parameters:
     x -- A sequence of nodal x-coords.
     y -- A sequence of nodal y-coords.
-    '''
+    """
 
     def __init__(self, x, y):
         if len(x) != len(y):
-            raise IndexError('x and y must be equally sized.')
+            msg = 'x and y must be equally sized.'
+            raise IndexError(msg)
         self.x = asfarray(x)
         self.y = asfarray(y)
         # Closes the polygon if were open
         x1, y1 = x[0], y[0]
         xn, yn = x[-1], y[-1]
         if x1 != xn or y1 != yn:
             self.x = concatenate((self.x, [x1]))
             self.y = concatenate((self.y, [y1]))
         # Anti-clockwise coordinates
         if _det(self.x, self.y) < 0:
             self.x = self.x[::-1]
             self.y = self.y[::-1]
 
     def is_inside(self, xpoint, ypoint, smalld=1e-12):
-        '''Check if point is inside a general polygon.
+        """Check if point is inside a general polygon.
 
         Input parameters:
         xpoint -- The x-coord of the point to be tested.
         ypoint -- The y-coords of the point to be tested.
         smalld -- A small float number.
 
         xpoint and ypoint could be scalars or array-like sequences.
@@ -121,32 +155,34 @@
 
         mindst -- The distance from the point to the nearest point of the
                   polygon.
                   If mindst < 0 then point is outside the polygon.
                   If mindst = 0 then point in on a side of the polygon.
                   If mindst > 0 then point is inside the polygon.
 
-        Notes:
+        Notes
+        -----
         An improved version of the algorithm of Nordbeck and Rydstedt.
         REF: SLOAN, S.W. (1985): A point-in-polygon program. Adv. Eng.
              Software, Vol 7, No. 1, pp 45-47.
 
-        '''
+        """
         xpoint = asfarray(xpoint)
         ypoint = asfarray(ypoint)
         # Scalar to array
-        if xpoint.shape is tuple():
+        if xpoint.shape == ():
             xpoint = array([xpoint], dtype=float)
             ypoint = array([ypoint], dtype=float)
             scalar = True
         else:
             scalar = False
         # Check consistency
         if xpoint.shape != ypoint.shape:
-            raise IndexError('x and y has different shapes')
+            msg = 'x and y has different shapes'
+            raise IndexError(msg)
         # If snear = True: Dist to nearest side < nearest vertex
         # If snear = False: Dist to nearest vertex < nearest side
         snear = ma.masked_all(xpoint.shape, dtype=bool)
         # Initialize arrays
         mindst = ones_like(xpoint, dtype=float) * inf
         j = ma.masked_all(xpoint.shape, dtype=int)
         x = self.x
@@ -168,34 +204,34 @@
             #     x = x1 + t * (x1 - x2)
             #     y = y1 + t * (y1 - y2)
             # where
             #     t = 0    at (x1, y1)
             #     t = 1    at (x2, y2)
             # Find where normal passing through (xpoint, ypoint) intersects
             # infinite line
-            t = -(x1p * x21 + y1p * y21) / (x21 ** 2 + y21 ** 2)
+            t = -(x1p * x21 + y1p * y21) / (x21**2 + y21**2)
             tlt0 = t < 0
-            tle1 = (0 <= t) & (t <= 1)
+            tle1 = (t >= 0) & (t <= 1)
             # Normal intersects side
-            d[tle1] = ((x1p[tle1] + t[tle1] * x21) ** 2 +
-                       (y1p[tle1] + t[tle1] * y21) ** 2)
+            d[tle1] = (x1p[tle1] + t[tle1] * x21) ** 2 + (y1p[tle1] + t[tle1] * y21) ** 2
             # Normal does not intersects side
             # Point is closest to vertex (x1, y1)
             # Compute square of distance to this vertex
             d[tlt0] = x1p[tlt0] ** 2 + y1p[tlt0] ** 2
             # Store distances
             mask = d < mindst
             mindst[mask] = d[mask]
             j[mask] = i
             # Point is closer to (x1, y1) than any other vertex or side
             snear[mask & tlt0] = False
             # Point is closer to this side than to any other side or vertex
             snear[mask & tle1] = True
         if ma.count(snear) != snear.size:
-            raise IndexError('Error computing distances')
+            msg = 'Error computing distances'
+            raise IndexError(msg)
         mindst **= 0.5
         # Point is closer to its nearest vertex than its nearest side, check if
         # nearest vertex is concave.
         # If the nearest vertex is concave then point is inside the polygon,
         # else the point is outside the polygon.
         jo = j.copy()
         jo[j == 0] -= 1
@@ -211,1040 +247,960 @@
         mindst[fabs(mindst) < smalld] = 0
         # If input values were scalar then the output should be too
         if scalar:
             mindst = float(mindst)
         return mindst
 
 
-class Grid( HasPrivateTraits ):
-    """
-    Virtual base class for grid geometries.
-    
+class Grid(HasPrivateTraits):
+    """Virtual base class for grid geometries.
+
     Defines the common interface for all grid classes and
     provides facilities to query grid properties and related data. This class
     may be used as a base for specialized grid implementaions. It should not
     be used directly as it contains no real functionality.
     """
 
     #: Overall number of grid points. Readonly; is set automatically when
     #: other grid defining properties are set
-    size = Property(desc="overall number of grid points")
+    size = Property(desc='overall number of grid points')
 
     #: Shape of grid. Readonly, gives the shape as tuple, useful for cartesian
     #: grids
-    shape = Property(desc="grid shape as tuple")
+    shape = Property(desc='grid shape as tuple')
 
     #: Grid positions as (3, :attr:`size`) array of floats, without invalid
     #: microphones; readonly.
-    gpos = Property(desc="x, y, z positions of grid points")
+    gpos = Property(desc='x, y, z positions of grid points')
 
     # internal identifier
     digest = Property
 
-    def _get_digest( self ):
+    def _get_digest(self):
         return ''
 
     # 'digest' is a placeholder for other properties in derived classes,
     # necessary to trigger the depends on mechanism
     @property_depends_on('digest')
-    def _get_size ( self ):
+    def _get_size(self):
         return 1
 
     # 'digest' is a placeholder for other properties in derived classes
     @property_depends_on('digest')
-    def _get_shape ( self ):
+    def _get_shape(self):
         return (1, 1)
 
     @property_depends_on('digest')
-    def _get_gpos( self ):
-        return array([[0.], [0.], [0.]])
-    
-    def pos ( self ):
-        """
-        Calculates grid co-ordinates. 
+    def _get_gpos(self):
+        return array([[0.0], [0.0], [0.0]])
+
+    def pos(self):
+        """Calculates grid co-ordinates.
         Deprecated; use :attr:`gpos` attribute instead.
-        
+
         Returns
         -------
         array of floats of shape (3, :attr:`size`)
             The grid point x, y, z-coordinates in one array.
+
         """
-        return self.gpos# array([[0.], [0.], [0.]])
-    
-    def subdomain (self, sector) :
-        """
-        Queries the indices for a subdomain in the grid.
-        
+        return self.gpos  # array([[0.], [0.], [0.]])
+
+    def subdomain(self, sector):
+        """Queries the indices for a subdomain in the grid.
+
         Allows arbitrary subdomains of type :class:`Sector`
-        
+
         Parameters
         ----------
         sector : :class:`Sector`
             Sector describing the subdomain.
 
         Returns
         -------
         2-tuple of arrays of integers or of numpy slice objects
-            The indices that can be used to mask/select the grid subdomain from 
-            an array with the same shape as the grid.            
+            The indices that can be used to mask/select the grid subdomain from
+            an array with the same shape as the grid.
+
         """
-        
         xpos = self.gpos
         # construct grid-shaped array with "True" entries where sector is
         xyi = sector.contains(xpos).reshape(self.shape)
         # return indices of "True" entries
         return where(xyi)
 
 
-class RectGrid( Grid ):
-    """
-    Provides a cartesian 2D grid for the beamforming results.
-    
+class RectGrid(Grid):
+    """Provides a cartesian 2D grid for the beamforming results.
+
     The grid has square or nearly square cells and is on a plane perpendicular
-    to the z-axis. It is defined by lower and upper x- and  y-limits and the 
+    to the z-axis. It is defined by lower and upper x- and  y-limits and the
     z co-ordinate.
     """
-    
+
     #: The lower x-limit that defines the grid, defaults to -1.
-    x_min = Float(-1.0,
-        desc="minimum  x-value")
+    x_min = Float(-1.0, desc='minimum  x-value')
 
     #: The upper x-limit that defines the grid, defaults to 1.
-    x_max = Float(1.0,
-        desc="maximum  x-value")
+    x_max = Float(1.0, desc='maximum  x-value')
 
     #: The lower y-limit that defines the grid, defaults to -1.
-    y_min = Float(-1.0,
-        desc="minimum  y-value")
+    y_min = Float(-1.0, desc='minimum  y-value')
 
     #: The upper y-limit that defines the grid, defaults to 1.
-    y_max = Float(1.0,
-        desc="maximum  y-value")
+    y_max = Float(1.0, desc='maximum  y-value')
 
     #: The z co-ordinate that defines the grid, defaults to 1.
-    z = Float(1.0,
-        desc="position on z-axis")
+    z = Float(1.0, desc='position on z-axis')
 
     #: The cell side length for the grid, defaults to 0.1.
-    increment = Float(0.1,
-        desc="step size")
+    increment = Float(0.1, desc='step size')
 
     #: Number of grid points along x-axis, readonly.
-    nxsteps = Property(
-        desc="number of grid points along x-axis")
+    nxsteps = Property(desc='number of grid points along x-axis')
 
     #: Number of grid points along y-axis, readonly.
-    nysteps = Property(
-        desc="number of grid points along y-axis")
+    nysteps = Property(desc='number of grid points along y-axis')
 
     # internal identifier
     digest = Property(
-        depends_on = ['x_min', 'x_max', 'y_min', 'y_max', 'z', 'increment']
-        )
+        depends_on=['x_min', 'x_max', 'y_min', 'y_max', 'z', 'increment'],
+    )
 
     @property_depends_on('nxsteps, nysteps')
-    def _get_size ( self ):
-        return self.nxsteps*self.nysteps
+    def _get_size(self):
+        return self.nxsteps * self.nysteps
 
     @property_depends_on('nxsteps, nysteps')
-    def _get_shape ( self ):
+    def _get_shape(self):
         return (self.nxsteps, self.nysteps)
 
     @property_depends_on('x_min, x_max, increment')
-    def _get_nxsteps ( self ):
+    def _get_nxsteps(self):
         i = abs(self.increment)
         if i != 0:
-            return int(round((abs(self.x_max-self.x_min)+i)/i))
+            return int(round((abs(self.x_max - self.x_min) + i) / i))
         return 1
 
     @property_depends_on('y_min, y_max, increment')
-    def _get_nysteps ( self ):
+    def _get_nysteps(self):
         i = abs(self.increment)
         if i != 0:
-            return int(round((abs(self.y_max-self.y_min)+i)/i))
+            return int(round((abs(self.y_max - self.y_min) + i) / i))
         return 1
 
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
+    def _get_digest(self):
+        return digest(self)
 
     @property_depends_on('x_min, x_max, y_min, y_max, increment')
-    def _get_gpos ( self ):
-        """
-        Calculates grid co-ordinates.
-        
+    def _get_gpos(self):
+        """Calculates grid co-ordinates.
+
         Returns
         -------
         array of floats of shape (3, :attr:`~Grid.size`)
             The grid point x, y, z-coordinates in one array.
+
         """
-        bpos = mgrid[self.x_min:self.x_max:self.nxsteps*1j, \
-                     self.y_min:self.y_max:self.nysteps*1j, \
-                     self.z:self.z+0.1]
+        bpos = mgrid[
+            self.x_min : self.x_max : self.nxsteps * 1j,
+            self.y_min : self.y_max : self.nysteps * 1j,
+            self.z : self.z + 0.1,
+        ]
         bpos.resize((3, self.size))
         return bpos
 
-    def index ( self, x, y ):
-        """
-        Queries the indices for a grid point near a certain co-ordinate.
+    def index(self, x, y):
+        """Queries the indices for a grid point near a certain co-ordinate.
 
         This can be used to query results or co-ordinates at/near a certain
         co-ordinate.
-        
+
         Parameters
         ----------
         x, y : float
             The co-ordinates for which the indices are queried.
 
         Returns
         -------
         2-tuple of integers
             The indices that give the grid point nearest to the given x, y
-            co-ordinates from an array with the same shape as the grid.            
+            co-ordinates from an array with the same shape as the grid.
+
         """
         if x < self.x_min or x > self.x_max:
-            raise ValueError("x-value out of range")
-        if y  <  self.y_min or y > self.y_max:
-            raise ValueError("y-value out of range")
-        xi = int((x-self.x_min)/self.increment+0.5)
-        yi = int((y-self.y_min)/self.increment+0.5)
+            msg = 'x-value out of range'
+            raise ValueError(msg)
+        if y < self.y_min or y > self.y_max:
+            msg = 'y-value out of range'
+            raise ValueError(msg)
+        xi = int((x - self.x_min) / self.increment + 0.5)
+        yi = int((y - self.y_min) / self.increment + 0.5)
         return xi, yi
 
-    def indices ( self, *r):
-        """
-        Queries the indices for a subdomain in the grid.
-        
+    def indices(self, *r):
+        """Queries the indices for a subdomain in the grid.
+
         Allows either rectangular, circular or polygonial subdomains.
-        This can be used to mask or to query results from a certain 
+        This can be used to mask or to query results from a certain
         sector or subdomain.
-        
+
         Parameters
         ----------
         x1, y1, x2, y2, ... : float
             If three parameters are given, then a circular sector is assumed
             that is given by its center (x1, y1) and the radius x2.
             If four paramters are given, then a rectangular sector is
-            assumed that is given by two corners (x1, y1) and (x2, y2). 
+            assumed that is given by two corners (x1, y1) and (x2, y2).
             If more parameters are given, the subdomain is assumed to have
             polygonial shape with corners at (x_n, y_n).
 
         Returns
         -------
         2-tuple of arrays of integers or of numpy slice objects
-            The indices that can be used to mask/select the grid subdomain from 
-            an array with the same shape as the grid.            
+            The indices that can be used to mask/select the grid subdomain from
+            an array with the same shape as the grid.
+
         """
-        
-        if len(r) == 3: # only 3 values given -> use x,y,radius method
+        if len(r) == 3:  # only 3 values given -> use x,y,radius method
             xpos = self.gpos
             xis = []
             yis = []
-            dr2 = (xpos[0, :]-r[0])**2 + (xpos[1, :]-r[1])**2
+            dr2 = (xpos[0, :] - r[0]) ** 2 + (xpos[1, :] - r[1]) ** 2
             # array with true/false entries
-            inds = dr2 <= r[2]**2 
-            for np in arange(self.size)[inds]: # np -- points in x2-circle
+            inds = dr2 <= r[2] ** 2
+            for np in arange(self.size)[inds]:  # np -- points in x2-circle
                 xi, yi = self.index(xpos[0, np], xpos[1, np])
                 xis += [xi]
                 yis += [yi]
-            if not (xis and yis): # if no points in circle, take nearest one
+            if not (xis and yis):  # if no points in circle, take nearest one
                 return self.index(r[0], r[1])
-            else:
-                return array(xis), array(yis)
-        elif len(r) == 4: # rectangular subdomain - old functionality
+            return array(xis), array(yis)
+        if len(r) == 4:  # rectangular subdomain - old functionality
             xi1, yi1 = self.index(min(r[0], r[2]), min(r[1], r[3]))
             xi2, yi2 = self.index(max(r[0], r[2]), max(r[1], r[3]))
-            return s_[xi1:xi2+1], s_[yi1:yi2+1]
-        else: # use enveloping polygon
-            xpos = self.gpos
-            xis = []
-            yis = []
-            #replaced matplotlib Path by numpy
-            #p = Path(array(r).reshape(-1,2))
-            #inds = p.contains_points()
-            #inds = in_poly(xpos[:2,:].T,array(r).reshape(-1,2))
-            poly = Polygon(array(r).reshape(-1,2)[:,0],array(r).reshape(-1,2)[:,1])
-            dists = poly.is_inside(xpos[0,:],xpos[1,:])   
-            inds = dists >= 0
-            for np in arange(self.size)[inds]: # np -- points in x2-circle
-                xi, yi = self.index(xpos[0, np], xpos[1, np])
-                xis += [xi]
-                yis += [yi]
-            if not (xis and yis): # if no points inside, take nearest to center
-                center = array(r).reshape(-1,2).mean(0)
-                return self.index(center[0], center[1])
-            else:
-                return array(xis), array(yis)
-                #return arange(self.size)[inds]
+            return s_[xi1 : xi2 + 1], s_[yi1 : yi2 + 1]
+        xpos = self.gpos
+        xis = []
+        yis = []
+        # replaced matplotlib Path by numpy
+        # p = Path(array(r).reshape(-1,2))
+        # inds = p.contains_points()
+        # inds = in_poly(xpos[:2,:].T,array(r).reshape(-1,2))
+        poly = Polygon(array(r).reshape(-1, 2)[:, 0], array(r).reshape(-1, 2)[:, 1])
+        dists = poly.is_inside(xpos[0, :], xpos[1, :])
+        inds = dists >= 0
+        for np in arange(self.size)[inds]:  # np -- points in x2-circle
+            xi, yi = self.index(xpos[0, np], xpos[1, np])
+            xis += [xi]
+            yis += [yi]
+        if not (xis and yis):  # if no points inside, take nearest to center
+            center = array(r).reshape(-1, 2).mean(0)
+            return self.index(center[0], center[1])
+        return array(xis), array(yis)
+        # return arange(self.size)[inds]
 
-    def extend (self) :
-        """
-        The extension of the grid in pylab.imshow compatible form.
+    def extend(self):
+        """The extension of the grid in pylab.imshow compatible form.
 
         Returns
         -------
         4-tuple of floats
             The extent of the grid as a tuple of x_min, x_max, y_min, y_max)
+
         """
         return (self.x_min, self.x_max, self.y_min, self.y_max)
 
 
-class RectGrid3D( RectGrid):
-    """
-    Provides a cartesian 3D grid for the beamforming results.
-    
-    The grid has cubic or nearly cubic cells. It is defined by lower and upper 
+class RectGrid3D(RectGrid):
+    """Provides a cartesian 3D grid for the beamforming results.
+
+    The grid has cubic or nearly cubic cells. It is defined by lower and upper
     x-, y- and  z-limits.
     """
 
     #: The lower z-limit that defines the grid, defaults to -1.
-    z_min = Float(-1.0,
-        desc="minimum  z-value")
+    z_min = Float(-1.0, desc='minimum  z-value')
 
     #: The upper z-limit that defines the grid, defaults to 1.
-    z_max = Float(1.0,
-        desc="maximum  z-value")
+    z_max = Float(1.0, desc='maximum  z-value')
 
     #: Number of grid points along x-axis, readonly.
-    nxsteps = Property(
-        desc="number of grid points along x-axis")
+    nxsteps = Property(desc='number of grid points along x-axis')
 
     #: Number of grid points along y-axis, readonly.
-    nysteps = Property(
-        desc="number of grid points along y-axis")
+    nysteps = Property(desc='number of grid points along y-axis')
 
     #: Number of grid points along x-axis, readonly.
-    nzsteps = Property(
-        desc="number of grid points along x-axis")
+    nzsteps = Property(desc='number of grid points along x-axis')
 
-    
     # Private trait for increment handling
     _increment = Any(0.1)
-    
-    #: The cell side length for the grid. This can either be a scalar (same 
-    #: increments in all 3 dimensions) or a (3,) array of floats with 
-    #: respective increments in x,y, and z-direction (in m). 
+
+    #: The cell side length for the grid. This can either be a scalar (same
+    #: increments in all 3 dimensions) or a (3,) array of floats with
+    #: respective increments in x,y, and z-direction (in m).
     #: Defaults to 0.1.
-    increment = Property(desc="step size")
-    
+    increment = Property(desc='step size')
+
     def _get_increment(self):
         return self._increment
-    
+
     def _set_increment(self, increment):
         if isscalar(increment):
             try:
                 self._increment = absolute(float(increment))
             except:
-                raise TraitError(args=self,
-                                 name='increment', 
-                                 info='Float or CArray(3,)',
-                                 value=increment) 
+                raise TraitError(args=self, name='increment', info='Float or CArray(3,)', value=increment)
         elif len(increment) == 3:
-            self._increment = array(increment,dtype=float)
+            self._increment = array(increment, dtype=float)
         else:
-            raise(TraitError(args=self,
-                             name='increment', 
-                             info='Float or CArray(3,)',
-                             value=increment))
-    
+            raise (TraitError(args=self, name='increment', info='Float or CArray(3,)', value=increment))
+
     # Respective increments in x,y, and z-direction (in m).
     # Deprecated: Use :attr:`~RectGrid.increment` for this functionality
-    increment3D = Property(desc="3D step sizes")
-    
+    increment3D = Property(desc='3D step sizes')
+
     def _get_increment3D(self):
         if isscalar(self._increment):
-            return array([self._increment,self._increment,self._increment])
-        else:
-            return self._increment
-    
+            return array([self._increment, self._increment, self._increment])
+        return self._increment
+
     def _set_increment3D(self, inc):
         if not isscalar(inc) and len(inc) == 3:
-            self._increment = array(inc,dtype=float)
+            self._increment = array(inc, dtype=float)
         else:
-            raise(TraitError(args=self,
-                             name='increment3D', 
-                             info='CArray(3,)',
-                             value=inc))
-    
+            raise (TraitError(args=self, name='increment3D', info='CArray(3,)', value=inc))
+
     # internal identifier
     digest = Property(
-        depends_on = ['x_min', 'x_max', 'y_min', 'y_max', 'z_min', 'z_max', \
-        '_increment']
-        )
+        depends_on=['x_min', 'x_max', 'y_min', 'y_max', 'z_min', 'z_max', '_increment'],
+    )
 
     @property_depends_on('nxsteps, nysteps, nzsteps')
-    def _get_size ( self ):
-        return self.nxsteps*self.nysteps*self.nzsteps
+    def _get_size(self):
+        return self.nxsteps * self.nysteps * self.nzsteps
 
     @property_depends_on('nxsteps, nysteps, nzsteps')
-    def _get_shape ( self ):
+    def _get_shape(self):
         return (self.nxsteps, self.nysteps, self.nzsteps)
-    
+
     @property_depends_on('x_min, x_max, _increment')
-    def _get_nxsteps ( self ):
+    def _get_nxsteps(self):
         i = abs(self.increment3D[0])
         if i != 0:
-            return int(round((abs(self.x_max-self.x_min)+i)/i))
+            return int(round((abs(self.x_max - self.x_min) + i) / i))
         return 1
 
     @property_depends_on('y_min, y_max, _increment')
-    def _get_nysteps ( self ):
+    def _get_nysteps(self):
         i = abs(self.increment3D[1])
         if i != 0:
-            return int(round((abs(self.y_max-self.y_min)+i)/i))
+            return int(round((abs(self.y_max - self.y_min) + i) / i))
         return 1
-        
+
     @property_depends_on('z_min, z_max, _increment')
-    def _get_nzsteps ( self ):
+    def _get_nzsteps(self):
         i = abs(self.increment3D[2])
         if i != 0:
-            return int(round((abs(self.z_max-self.z_min)+i)/i))
+            return int(round((abs(self.z_max - self.z_min) + i) / i))
         return 1
 
     @property_depends_on('digest')
-    def _get_gpos ( self ):
-        """
-        Calculates grid co-ordinates.
-        
+    def _get_gpos(self):
+        """Calculates grid co-ordinates.
+
         Returns
         -------
         array of floats of shape (3, :attr:`~Grid.size`)
             The grid point x, y, z-coordinates in one array.
+
         """
-        bpos = mgrid[self.x_min:self.x_max:self.nxsteps*1j, \
-                     self.y_min:self.y_max:self.nysteps*1j, \
-                     self.z_min:self.z_max:self.nzsteps*1j]
+        bpos = mgrid[
+            self.x_min : self.x_max : self.nxsteps * 1j,
+            self.y_min : self.y_max : self.nysteps * 1j,
+            self.z_min : self.z_max : self.nzsteps * 1j,
+        ]
         bpos.resize((3, self.size))
         return bpos
 
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
-
-   
+    def _get_digest(self):
+        return digest(self)
 
-    def index ( self, x, y, z ):
-        """
-        Queries the indices for a grid point near a certain co-ordinate.
+    def index(self, x, y, z):
+        """Queries the indices for a grid point near a certain co-ordinate.
 
         This can be used to query results or co-ordinates at/near a certain
         co-ordinate.
-        
+
         Parameters
         ----------
         x, y, z : float
             The co-ordinates for which the indices is queried.
 
         Returns
         -------
         3-tuple of integers
             The indices that give the grid point nearest to the given x, y, z
-            co-ordinates from an array with the same shape as the grid.            
+            co-ordinates from an array with the same shape as the grid.
+
         """
         if x < self.x_min or x > self.x_max:
-            raise ValueError("x-value out of range %f (%f, %f)" % \
-                (x,self.x_min,self.x_max))
+            msg = f'x-value out of range {x:f} ({self.x_min:f}, {self.x_max:f})'
+            raise ValueError(msg)
         if y < self.y_min or y > self.y_max:
-            raise ValueError("y-value out of range %f (%f, %f)" % \
-                (y,self.y_min,self.y_max))
+            msg = f'y-value out of range {y:f} ({self.y_min:f}, {self.y_max:f})'
+            raise ValueError(msg)
         if z < self.z_min or z > self.z_max:
-            raise ValueError("z-value out of range %f (%f, %f)" % \
-                (z,self.z_min,self.z_max))
-        xi = int(round((x-self.x_min)/self.increment3D[0]))
-        yi = int(round((y-self.y_min)/self.increment3D[1]))
-        zi = int(round((z-self.z_min)/self.increment3D[2]))
+            msg = f'z-value out of range {z:f} ({self.z_min:f}, {self.z_max:f})'
+            raise ValueError(msg)
+        xi = int(round((x - self.x_min) / self.increment3D[0]))
+        yi = int(round((y - self.y_min) / self.increment3D[1]))
+        zi = int(round((z - self.z_min) / self.increment3D[2]))
         return xi, yi, zi
 
-    def indices ( self, x1, y1, z1, x2, y2, z2 ):
-        """
-        Queries the indices for a subdomain in the grid.
-        
+    def indices(self, x1, y1, z1, x2, y2, z2):
+        """Queries the indices for a subdomain in the grid.
+
         Allows box-shaped subdomains. This can be used to
         mask or to query results from a certain sector or subdomain.
-        
+
         Parameters
         ----------
         x1, y1, z1, x2, y2, z2 : float
             A box-shaped sector is assumed that is given by two corners
-            (x1,y1,z1) and (x2,y2,z2). 
+            (x1,y1,z1) and (x2,y2,z2).
 
         Returns
         -------
         3-tuple of numpy slice objects
-            The indices that can be used to mask/select the grid subdomain from 
-            an array with the same shape as the grid.            
+            The indices that can be used to mask/select the grid subdomain from
+            an array with the same shape as the grid.
+
         """
         xi1, yi1, zi1 = self.index(min(x1, x2), min(y1, y2), min(z1, z2))
         xi2, yi2, zi2 = self.index(max(x1, x2), max(y1, y2), max(z1, z2))
-        return s_[xi1:xi2+1], s_[yi1:yi2+1], s_[zi1:zi2+1]
+        return s_[xi1 : xi2 + 1], s_[yi1 : yi2 + 1], s_[zi1 : zi2 + 1]
 
 
-class ImportGrid( Grid ):
-    """
-    Loads a 3D grid from xml file.
-    """
+class ImportGrid(Grid):
+    """Loads a 3D grid from xml file."""
 
-    # internal identifier
-    digest = Property
-    
     #: Name of the .xml-file from wich to read the data.
-    from_file = File(filter=['*.xml'],
-        desc="name of the xml file to import")
-    
-    
-    gpos_file = CArray(dtype=float,
-        desc="x, y, z position of all Grid Points")
-    
+    from_file = File(filter=['*.xml'], desc='name of the xml file to import')
+
+    gpos_file = CArray(dtype=float, desc='x, y, z position of all Grid Points')
 
     #: Basename of the .xml-file, without the extension; is set automatically / readonly.
-    basename = Property( depends_on = 'from_file',
-        desc="basename of xml file")
-    
-        # internal identifier
+    basename = Property(depends_on='from_file', desc='basename of xml file')
+
+    # internal identifier
     digest = Property(
-        depends_on = ['from_file']
-        )
-    
+        depends_on=['from_file'],
+    )
+
     @cached_property
-    def _get_basename( self ):
+    def _get_basename(self):
         return path.splitext(path.basename(self.from_file))[0]
 
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
+    def _get_digest(self):
+        return digest(self)
 
     # 'digest' is a placeholder for other properties in derived classes,
     # necessary to trigger the depends on mechanism
     @property_depends_on('basename')
-    def _get_size ( self ):
+    def _get_size(self):
         return self.gpos.shape[-1]
 
     # 'digest' is a placeholder for other properties in derived classes
     @property_depends_on('basename')
-    def _get_shape ( self ):
+    def _get_shape(self):
         return (self.gpos.shape[-1],)
 
     @property_depends_on('basename')
-    def _get_gpos( self ):
+    def _get_gpos(self):
         return self.gpos_file
 
+    subgrids = CArray(desc='names of subgrids for each point')
 
-    subgrids = CArray(
-        desc="names of subgrids for each point")
-
-    
     @on_trait_change('basename')
-    def import_gpos( self ):
-        """
-        Import the the grid point locations from .xml file.
+    def import_gpos(self):
+        """Import the the grid point locations from .xml file.
         Called when :attr:`basename` changes.
         """
         if not path.isfile(self.from_file):
             # no file there
             self.gpos_file = array([], 'd')
             return
         import xml.dom.minidom
+
         doc = xml.dom.minidom.parse(self.from_file)
         names = []
         xyz = []
         for el in doc.getElementsByTagName('pos'):
             names.append(el.getAttribute('subgrid'))
-            xyz.append(list(map(lambda a : float(el.getAttribute(a)), 'xyz')))
+            xyz.append([float(el.getAttribute(a)) for a in 'xyz'])
         self.gpos_file = array(xyz, 'd').swapaxes(0, 1)
         self.subgrids = array(names)
 
-class LineGrid( Grid ):
-    """
-    Class for Line grid geometries.
-    
-    """
-    
+
+class LineGrid(Grid):
+    """Class for Line grid geometries."""
+
     #: Staring point of the Grid
     loc = Tuple((0.0, 0.0, 0.0))
 
     #: Vector to define the orientation of the line source
-    direction = Tuple((1.0, 0.0, 0.0),
-        desc="Line orientation ")
-    
+    direction = Tuple((1.0, 0.0, 0.0), desc='Line orientation ')
+
     #: Vector to define the length of the line source in meter
-    length = Float(1,desc="length of the line source")
-    
+    length = Float(1, desc='length of the line source')
+
     #:number of grid points.
-    numpoints = Int(1,desc="length of the line source")
-    
+    numpoints = Int(1, desc='length of the line source')
+
     #: Overall number of grid points. Readonly; is set automatically when
     #: other grid defining properties are set
-    size = Property(desc="overall number of grid points")
+    size = Property(desc='overall number of grid points')
 
     #: Grid positions as (3, :attr:`size`) array of floats, without invalid
     #: microphones; readonly.
-    gpos = Property(desc="x, y, z positions of grid points")
+    gpos = Property(desc='x, y, z positions of grid points')
 
     digest = Property(
-    depends_on = ['loc', 'direction', 'length', 'numpoints', 'size']
+        depends_on=['loc', 'direction', 'length', 'numpoints', 'size'],
     )
 
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
+    def _get_digest(self):
+        return digest(self)
 
     # 'digest' is a placeholder for other properties in derived classes,
     # necessary to trigger the depends on mechanism
     @property_depends_on('numpoints')
-    def _get_size ( self ):
+    def _get_size(self):
         return self.gpos.shape[-1]
 
     # 'digest' is a placeholder for other properties in derived classes
     @property_depends_on('numpoints')
-    def _get_shape ( self ):
+    def _get_shape(self):
         return self.gpos.shape[-1]
 
     @property_depends_on('numpoints,length,direction,loc')
-    def _get_gpos( self ):
+    def _get_gpos(self):
         dist = self.length / (self.numpoints - 1)
-        loc = array(self.loc, dtype = float).reshape((3, 1)) 
-        direc_n = self.direction/norm(self.direction)
-        pos = zeros((self.numpoints,3))
+        loc = array(self.loc, dtype=float).reshape((3, 1))
+        direc_n = self.direction / norm(self.direction)
+        pos = zeros((self.numpoints, 3))
         for s in range(self.numpoints):
-            pos[s] = (loc.T+direc_n*dist*s)
+            pos[s] = loc.T + direc_n * dist * s
         return pos.T
 
 
-class MergeGrid( Grid ):
-    """
-    Base class for merging different grid geometries.
-    
-    """
+class MergeGrid(Grid):
+    """Base class for merging different grid geometries."""
 
     #: List of Grids to be merged
     #: each grid gets a new subdomain in the new grid
     #: other grid defining properties are set
-    grids = List(desc="list of grids")
-    
-    grid_digest = Property(desc="digest of the merged grids")
+    grids = List(desc='list of grids')
+
+    grid_digest = Property(desc='digest of the merged grids')
+
+    subgrids = Property(desc='names of subgrids for each point')
 
-    subgrids = Property(desc="names of subgrids for each point")
-    
     # internal identifier
     digest = Property(
-    depends_on = ['grids','grid_digest']
+        depends_on=['grids', 'grid_digest'],
     )
 
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
-    
+    def _get_digest(self):
+        return digest(self)
+
     @cached_property
-    def _get_grid_digest( self ):
+    def _get_grid_digest(self):
         griddigest = []
         for grid in self.grids:
             griddigest.append(grid.digest)
         return griddigest
 
     # 'digest' is a placeholder for other properties in derived classes,
     # necessary to trigger the depends on mechanism
     @property_depends_on('digest')
-    def _get_size ( self ):
+    def _get_size(self):
         return self.gpos.shape[-1]
 
     # 'digest' is a placeholder for other properties in derived classes
     @property_depends_on('digest')
-    def _get_shape ( self ):
+    def _get_shape(self):
         return self.gpos.shape[-1]
-    
+
     @property_depends_on('digest')
-    def _get_subgrids( self ):
-        subgrids = zeros((1,0),dtype=str)
+    def _get_subgrids(self):
+        subgrids = zeros((1, 0), dtype=str)
         for grid in self.grids:
-            subgrids = append(subgrids,tile(grid.__class__.__name__+grid.digest,grid.size))
-        return subgrids[:,newaxis].T
-    
+            subgrids = append(subgrids, tile(grid.__class__.__name__ + grid.digest, grid.size))
+        return subgrids[:, newaxis].T
+
     @property_depends_on('digest')
-    def _get_gpos( self ):
-        bpos = zeros((3,0))
-        #subgrids = zeros((1,0))
+    def _get_gpos(self):
+        bpos = zeros((3, 0))
+        # subgrids = zeros((1,0))
         for grid in self.grids:
-            bpos = append(bpos,grid.gpos, axis = 1)
-            #subgrids = append(subgrids,str(grid))
-        bpos = unique(bpos,axis=1)
-        return bpos
+            bpos = append(bpos, grid.gpos, axis=1)
+            # subgrids = append(subgrids,str(grid))
+        return unique(bpos, axis=1)
+
+
+class Sector(HasPrivateTraits):
+    """Base class for all sector types.
 
-class Sector( HasPrivateTraits ):
-    """
-    Base class for all sector types.
-    
     Defines the common interface for all tbdsector classes. This class
     may be used as a base for diverse sector implementaions. If used
     directly, it implements a sector encompassing the whole grid.
     """
-    
-    def contains ( self, pos ):
-        """
-        Queries whether the coordinates in a given array lie within the 
-        defined sector. 
+
+    def contains(self, pos):
+        """Queries whether the coordinates in a given array lie within the
+        defined sector.
         For this sector type, any position is valid.
-        
+
         Parameters
         ----------
         pos : array of floats
             Array with the shape 3x[number of gridpoints] containing the
             grid positions
-        
+
         Returns
         -------
         array of bools with as many entries as columns in pos
             Array indicating which of the given positions lie within the
-            given sector                
+            given sector
+
         """
         return ones(pos.shape[1], dtype=bool)
 
 
-class SingleSector( Sector ):
-    """
-    Base class for single sector types.
-    
+class SingleSector(Sector):
+    """Base class for single sector types.
+
     Defines the common interface for all single sector classes. This class
     may be used as a base for diverse single sector implementaions. If used
     directly, it implements a sector encompassing the whole grid.
     """
-    
+
     #: Boolean flag, if 'True' (default), grid points lying on the sector border are included.
-    include_border = Bool(True, 
-                          desc="include points on the border")    
-    
+    include_border = Bool(True, desc='include points on the border')
+
     #: Absolute tolerance for sector border
-    abs_tol = Float(1e-12,
-                    desc="absolute tolerance for sector border")
+    abs_tol = Float(1e-12, desc='absolute tolerance for sector border')
 
     #: Boolean flag, if 'True' (default), the nearest grid point is returned if none is inside the sector.
-    default_nearest = Bool(True, 
-                          desc="return nearest grid point to center of none inside sector")
+    default_nearest = Bool(True, desc='return nearest grid point to center of none inside sector')
 
 
+class RectSector(SingleSector):
+    """Class for defining a rectangular sector.
 
-class RectSector( SingleSector ):
-    """
-    Class for defining a rectangular sector.
-    
     Can be used for 2D Grids for definining a rectangular sector or
     for 3D grids for a rectangular cylinder sector parallel to the z-axis.
     """
-    
+
     #: The lower x position of the rectangle
-    x_min = Float(-1.0,
-                  desc="minimum x position of the rectangle")
+    x_min = Float(-1.0, desc='minimum x position of the rectangle')
 
     #: The upper x position of the rectangle
-    x_max = Float(1.0,
-                  desc="maximum x position of the rectangle")
+    x_max = Float(1.0, desc='maximum x position of the rectangle')
 
     #: The lower y position of the rectangle
-    y_min = Float(-1.0,
-                  desc="minimum y position of the rectangle")
-    
+    y_min = Float(-1.0, desc='minimum y position of the rectangle')
+
     #: The upper y position of the rectangle
-    y_max = Float(1.0,
-                  desc="maximum y position of the rectangle")
+    y_max = Float(1.0, desc='maximum y position of the rectangle')
 
-    def contains ( self, pos ):
-        """
-        Queries whether the coordinates in a given array lie within the 
-        rectangular sector. 
+    def contains(self, pos):
+        """Queries whether the coordinates in a given array lie within the
+        rectangular sector.
         If no coordinate is inside, the nearest one to the rectangle center
         is returned if :attr:`~Sector.default_nearest` is True.
-        
+
         Parameters
         ----------
         pos : array of floats
             Array with the shape 3x[number of gridpoints] containing the
             grid positions
-        
+
         Returns
         -------
         array of bools with as many entries as columns in pos
             Array indicating which of the given positions lie within the
-            given sector                
+            given sector
+
         """
         # make sure xmin is minimum etc
-        xmin = min(self.x_min,self.x_max)
-        xmax = max(self.x_min,self.x_max)
-        ymin = min(self.y_min,self.y_max)
-        ymax = max(self.y_min,self.y_max)
-        
+        xmin = min(self.x_min, self.x_max)
+        xmax = max(self.x_min, self.x_max)
+        ymin = min(self.y_min, self.y_max)
+        ymax = max(self.y_min, self.y_max)
+
         abs_tol = self.abs_tol
         # get pos indices inside rectangle (* == and)
         if self.include_border:
-            inds = (pos[0, :] - xmin > -abs_tol) * \
-                   (pos[0, :] - xmax < abs_tol) * \
-                   (pos[1, :] - ymin > -abs_tol) * \
-                   (pos[1, :] - ymax < abs_tol)
+            inds = (
+                (pos[0, :] - xmin > -abs_tol)
+                * (pos[0, :] - xmax < abs_tol)
+                * (pos[1, :] - ymin > -abs_tol)
+                * (pos[1, :] - ymax < abs_tol)
+            )
         else:
-            inds = (pos[0, :] - xmin > abs_tol) * \
-                   (pos[0, :] - xmax < -abs_tol) * \
-                   (pos[1, :] - ymin > abs_tol) * \
-                   (pos[1, :] - ymax < -abs_tol)
-        
-        
+            inds = (
+                (pos[0, :] - xmin > abs_tol)
+                * (pos[0, :] - xmax < -abs_tol)
+                * (pos[1, :] - ymin > abs_tol)
+                * (pos[1, :] - ymax < -abs_tol)
+            )
+
         # if none inside, take nearest
         if ~inds.any() and self.default_nearest:
             x = (xmin + xmax) / 2.0
             y = (ymin + ymax) / 2.0
-            dr2 = (pos[0, :] - x)**2 + (pos[1, :] - y)**2
+            dr2 = (pos[0, :] - x) ** 2 + (pos[1, :] - y) ** 2
             inds[argmin(dr2)] = True
-        
+
         return inds.astype(bool)
 
 
-class RectSector3D( RectSector ):
-    """
-    Class for defining a cuboid sector.
-    
+class RectSector3D(RectSector):
+    """Class for defining a cuboid sector.
+
     Can be used for 3D Grids for definining a cuboid sector.
     """
-    
+
     #: The lower z position of the cuboid
-    z_min = Float(-1.0,
-                  desc="minimum z position of the cuboid")
+    z_min = Float(-1.0, desc='minimum z position of the cuboid')
 
     #: The upper z position of the cuboid
-    z_max = Float(1.0,
-                  desc="maximum z position of the cuboid")
+    z_max = Float(1.0, desc='maximum z position of the cuboid')
 
-    def contains ( self, pos ):
-        """
-        Queries whether the coordinates in a given array lie within the 
-        rectangular sector. 
+    def contains(self, pos):
+        """Queries whether the coordinates in a given array lie within the
+        rectangular sector.
         If no coordinate is inside, the nearest one to the rectangle center
         is returned if :attr:`~Sector.default_nearest` is True.
-        
+
         Parameters
         ----------
         pos : array of floats
             Array with the shape 3x[number of gridpoints] containing the
             grid positions
-        
+
         Returns
         -------
         array of bools with as many entries as columns in pos
             Array indicating which of the given positions lie within the
-            given sector                
+            given sector
+
         """
         # make sure xmin is minimum etc
-        xmin = min(self.x_min,self.x_max)
-        xmax = max(self.x_min,self.x_max)
-        ymin = min(self.y_min,self.y_max)
-        ymax = max(self.y_min,self.y_max)
-        zmin = min(self.z_min,self.z_max)
-        zmax = max(self.z_min,self.z_max)
-        
+        xmin = min(self.x_min, self.x_max)
+        xmax = max(self.x_min, self.x_max)
+        ymin = min(self.y_min, self.y_max)
+        ymax = max(self.y_min, self.y_max)
+        zmin = min(self.z_min, self.z_max)
+        zmax = max(self.z_min, self.z_max)
+
         abs_tol = self.abs_tol
         # get pos indices inside rectangle (* == and)
         if self.include_border:
-            inds = (pos[0, :] - xmin > -abs_tol) * \
-                   (pos[0, :] - xmax < abs_tol) * \
-                   (pos[1, :] - ymin > -abs_tol) * \
-                   (pos[1, :] - ymax < abs_tol) * \
-                   (pos[2, :] - zmin > -abs_tol) * \
-                   (pos[2, :] - zmax < abs_tol)
+            inds = (
+                (pos[0, :] - xmin > -abs_tol)
+                * (pos[0, :] - xmax < abs_tol)
+                * (pos[1, :] - ymin > -abs_tol)
+                * (pos[1, :] - ymax < abs_tol)
+                * (pos[2, :] - zmin > -abs_tol)
+                * (pos[2, :] - zmax < abs_tol)
+            )
         else:
-            inds = (pos[0, :] - xmin > abs_tol) * \
-                   (pos[0, :] - xmax < -abs_tol) * \
-                   (pos[1, :] - ymin > abs_tol) * \
-                   (pos[1, :] - ymax < -abs_tol) * \
-                   (pos[2, :] - zmin > abs_tol) * \
-                   (pos[2, :] - zmax < -abs_tol)
-        
+            inds = (
+                (pos[0, :] - xmin > abs_tol)
+                * (pos[0, :] - xmax < -abs_tol)
+                * (pos[1, :] - ymin > abs_tol)
+                * (pos[1, :] - ymax < -abs_tol)
+                * (pos[2, :] - zmin > abs_tol)
+                * (pos[2, :] - zmax < -abs_tol)
+            )
+
         # if none inside, take nearest
         if ~inds.any() and self.default_nearest:
             x = (xmin + xmax) / 2.0
             y = (ymin + ymax) / 2.0
-            dr2 = (pos[0, :] - x)**2 + (pos[1, :] - y)**2
+            dr2 = (pos[0, :] - x) ** 2 + (pos[1, :] - y) ** 2
             inds[argmin(dr2)] = True
-        
+
         return inds.astype(bool)
 
 
-class CircSector( SingleSector ):
-    """
-    Class for defining a circular sector.
-    
+class CircSector(SingleSector):
+    """Class for defining a circular sector.
+
     Can be used for 2D Grids for definining a circular sector or
     for 3D grids for a cylindrical sector parallel to the z-axis.
     """
-    
+
     #: x position of the circle center
-    x = Float(0.0,
-        desc="x position of the circle center")
+    x = Float(0.0, desc='x position of the circle center')
 
     #: y position of the circle center
-    y = Float(0.0,
-        desc="y position of the circle center")
-    
+    y = Float(0.0, desc='y position of the circle center')
+
     #: radius of the circle
-    r = Float(1.0,
-        desc="radius of the circle")
-        
-    
-    def contains ( self, pos ):
-        """
-        Queries whether the coordinates in a given array lie within the 
-        circular sector. 
+    r = Float(1.0, desc='radius of the circle')
+
+    def contains(self, pos):
+        """Queries whether the coordinates in a given array lie within the
+        circular sector.
         If no coordinate is inside, the nearest one outside is returned
         if :attr:`~Sector.default_nearest` is True.
-        
+
         Parameters
         ----------
         pos : array of floats
             Array with the shape 3x[number of gridpoints] containing the
             grid positions
-        
+
         Returns
         -------
         array of bools with as many entries as columns in pos
             Array indicating which of the given positions lie within the
-            given sector                
+            given sector
+
         """
-        dr2 = (pos[0, :]-self.x)**2 + (pos[1, :]-self.y)**2
+        dr2 = (pos[0, :] - self.x) ** 2 + (pos[1, :] - self.y) ** 2
         # which points are in the circle?
-        if self.include_border:
-            inds = (dr2 - self.r**2) < self.abs_tol
-        else:
-            inds = (dr2 - self.r**2) < -self.abs_tol
-        
-        
+        inds = dr2 - self.r**2 < self.abs_tol if self.include_border else dr2 - self.r**2 < -self.abs_tol
+
         # if there's no poit inside
-        if ~inds.any() and self.default_nearest: 
+        if ~inds.any() and self.default_nearest:
             inds[argmin(dr2)] = True
-        
+
         return inds
 
 
-class PolySector( SingleSector ):
-    """
-     Class for defining a polygon sector.
-     
-     Can be used for 2D Grids for definining a polygon sector.
+class PolySector(SingleSector):
+    """Class for defining a polygon sector.
+
+    Can be used for 2D Grids for definining a polygon sector.
     """
+
     # x1, y1, x2, y2, ... xn, yn :
-    edges = List( Float ) 
-    
+    edges = List(Float)
 
-    def contains ( self, pos ):
-        """
-        Queries whether the coordinates in a given array lie within the 
-        ploygon sector. 
+    def contains(self, pos):
+        """Queries whether the coordinates in a given array lie within the
+        ploygon sector.
         If no coordinate is inside, the nearest one to the rectangle center
         is returned if :attr:`~Sector.default_nearest` is True.
-        
+
         Parameters
         ----------
         pos : array of floats
             Array with the shape 3x[number of gridpoints] containing the
             grid positions
-        
+
         Returns
         -------
         array of bools with as many entries as columns in pos
             Array indicating which of the given positions lie within the
-            given sector                
+            given sector
+
         """
-                
-        poly = Polygon(array(self.edges).reshape(-1,2)[:,0],array(self.edges).reshape(-1,2)[:,1])
-        dists = poly.is_inside(pos[0,:],pos[1,:])   
-        if  self.include_border:
-            inds = dists >= -self.abs_tol
-        else:
-            inds = dists > 0
-            
-        
+        poly = Polygon(array(self.edges).reshape(-1, 2)[:, 0], array(self.edges).reshape(-1, 2)[:, 1])
+        dists = poly.is_inside(pos[0, :], pos[1, :])
+        inds = dists >= -self.abs_tol if self.include_border else dists > 0
+
         # if none inside, take nearest
         if ~inds.any() and self.default_nearest:
-            dr2 = array(self.edges).reshape(-1,2).mean(0)
+            dr2 = array(self.edges).reshape(-1, 2).mean(0)
             inds[argmin(dr2)] = True
-          
+
         return inds
 
-class ConvexSector( SingleSector ):
-    """
-     Class for defining a convex hull sector.
-    
-     Can be used for 2D Grids for definining a convex hull sector.
+
+class ConvexSector(SingleSector):
+    """Class for defining a convex hull sector.
+
+    Can be used for 2D Grids for definining a convex hull sector.
     """
+
     # x1, y1, x2, y2, ... xn, yn :
-    edges = List( Float ) 
-    
+    edges = List(Float)
 
-    def contains ( self, pos ):
-        """
-        Queries whether the coordinates in a given array lie within the 
-        convex sector. 
+    def contains(self, pos):
+        """Queries whether the coordinates in a given array lie within the
+        convex sector.
         If no coordinate is inside, the nearest one to the rectangle center
-        is returned if :attr:`~Sector.default_nearest` is True. 
-        
+        is returned if :attr:`~Sector.default_nearest` is True.
+
         Parameters
         ----------
         pos : array of floats
             Array with the shape 3x[number of gridpoints] containing the
             grid positions
-        
+
         Returns
         -------
         array of bools with as many entries as columns in pos
             Array indicating which of the given positions lie within the
-            given sector                
+            given sector
+
         """
-        
-        inds = in_hull(pos[:2,:].T, array(self.edges).reshape(-1,2), \
-                           border = self.include_border ,tol = self.abs_tol)
-        
+        inds = in_hull(pos[:2, :].T, array(self.edges).reshape(-1, 2), border=self.include_border, tol=self.abs_tol)
+
         # if none inside, take nearest
         if ~inds.any() and self.default_nearest:
-            dr2 = array(self.edges).reshape(-1,2).mean(0)
+            dr2 = array(self.edges).reshape(-1, 2).mean(0)
             inds[argmin(dr2)] = True
-          
-        return inds
 
+        return inds
 
 
 class MultiSector(Sector):
-    """
-    Class for defining a sector consisting of multiple sectors.
-    
+    """Class for defining a sector consisting of multiple sectors.
+
     Can be used to sum over different sectors. Takes a list of sectors
     and returns the points contained in each sector.
-    
+
     """
-    
+
     #: List of :class:`acoular.grids.Sector` objects
     #: to be mixed.
-    sectors = List(Instance(Sector)) 
-    
-    def contains ( self, pos ):
-        """
-        Queries whether the coordinates in a given array lie within any 
-        of the sub-sectors. 
-        
+    sectors = List(Instance(Sector))
+
+    def contains(self, pos):
+        """Queries whether the coordinates in a given array lie within any
+        of the sub-sectors.
+
         Parameters
         ----------
         pos : array of floats
             Array with the shape 3x[number of gridpoints] containing the
             grid positions
-        
+
         Returns
         -------
         array of bools with as many entries as columns in pos
             Array indicating which of the given positions lie within the
-            sectors              
+            sectors
+
         """
         # initialize with only "False" entries
         inds = zeros(pos.shape[1], dtype=bool)
-        
+
         # add points contained in each sector
         for sec in self.sectors:
             inds += sec.contains(pos)
-        
-        return inds.astype(bool)
-
-
-
-
-
 
+        return inds.astype(bool)
```

### Comparing `acoular-24.3/acoular/h5cache.py` & `acoular-24.5/acoular/h5cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,136 +1,127 @@
-# -*- coding: utf-8 -*-
-#pylint: disable-msg=E0611,C0111,C0103,R0901,R0902,R0903,R0904,W0232
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 # Copyright (c) Acoular Development Team.
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 
 # imports from other packages
-from __future__ import print_function
-from traits.api import HasPrivateTraits, Bool, Str, Dict, Instance, Delegate
-from os import path, mkdir, environ, listdir
-from weakref import WeakValueDictionary
 import gc
+from os import listdir, path
+from weakref import WeakValueDictionary
+
+from traits.api import Bool, Delegate, Dict, HasPrivateTraits, Instance
 
 from .configuration import Config, config
 from .h5files import _get_cachefile_class
 
+
 class H5cache_class(HasPrivateTraits):
-    """
-    Cache class that handles opening and closing 'tables.File' objects
-    """
+    """Cache class that handles opening and closing 'tables.File' objects."""
 
     config = Instance(Config)
 
-    cache_dir = Delegate('config')    
+    cache_dir = Delegate('config')
 
     busy = Bool(False)
-    
+
     open_files = WeakValueDictionary()
-    
-    openFileReferenceCount = dict()
-    
+
+    openFileReferenceCount = Dict()
+
     def _idle_if_busy(self):
         while self.busy:
             pass
 
-    def open_cachefile(self,cacheFileName,mode):
+    def open_cachefile(self, cacheFileName, mode):
         File = _get_cachefile_class()
         return File(path.join(self.cache_dir, cacheFileName), mode)
-    
-    def close_cachefile(self,cachefile):
+
+    def close_cachefile(self, cachefile):
         self.openFileReferenceCount.pop(get_basename(cachefile))
         cachefile.close()
-        
-    def get_filename(self,file):
+
+    def get_filename(self, file):
         File = _get_cachefile_class()
-        if isinstance(file, File): 
+        if isinstance(file, File):
             return get_basename(file)
-        else:
-            return 0
+        return 0
 
     def get_open_cachefiles(self):
         try:
             return self.open_files.itervalues()
         except AttributeError:
             return iter(self.open_files.values())
 
     def close_unreferenced_cachefiles(self):
         for openCacheFile in self.get_open_cachefiles():
             if not self.is_reference_existent(openCacheFile):
-#                print("close unreferenced File:",get_basename(openCacheFile))
+                #                print("close unreferenced File:",get_basename(openCacheFile))
                 self.close_cachefile(openCacheFile)
 
-    def is_reference_existent(self,file):
+    def is_reference_existent(self, file):
         existFlag = False
         # inspect all refererres to the file object
-        gc.collect() #clear garbage before collecting referrers
+        gc.collect()  # clear garbage before collecting referrers
         for ref in gc.get_referrers(file):
-            # does the file object have a referrer that has a 'h5f' 
+            # does the file object have a referrer that has a 'h5f'
             # attribute?
-            if isinstance(ref,dict) and 'h5f' in ref:
+            if isinstance(ref, dict) and 'h5f' in ref:
                 # file is still referred, must not be closed
                 existFlag = True
                 break
         return existFlag
 
-    def is_cachefile_existent(self,cacheFileName):
+    def is_cachefile_existent(self, cacheFileName):
         if cacheFileName in listdir(self.cache_dir):
             return True
-        else:
-            return False
+        return False
 
     def _increase_file_reference_counter(self, cacheFileName):
         self.openFileReferenceCount[cacheFileName] = self.openFileReferenceCount.get(cacheFileName, 0) + 1
 
     def _decrease_file_reference_counter(self, cacheFileName):
         self.openFileReferenceCount[cacheFileName] = self.openFileReferenceCount[cacheFileName] - 1
 
     def _print_open_files(self):
         print(list(self.openFileReferenceCount.items()))
 
-    def get_cache_file( self, obj, basename, mode='a' ):
-        '''
-        returns pytables .h5 file to h5f trait of calling object for caching
-        '''        
-        
-        self._idle_if_busy() # 
+    def get_cache_file(self, obj, basename, mode='a'):
+        """Returns pytables .h5 file to h5f trait of calling object for caching."""
+        self._idle_if_busy()  #
         self.busy = True
 
         cacheFileName = basename + '_cache.h5'
         objFileName = self.get_filename(obj.h5f)
-        
+
         if objFileName:
-            if objFileName == cacheFileName: 
+            if objFileName == cacheFileName:
                 self.busy = False
                 return
-            else: # in case the base name has changed ( different source ) 
-                self._decrease_file_reference_counter(objFileName)
+            self._decrease_file_reference_counter(objFileName)
 
-        if cacheFileName not in self.open_files: # or tables.file._open_files.filenames
-            if (
-                config.global_caching == 'readonly' 
-                and not self.is_cachefile_existent(cacheFileName)
-                ): # condition ensures that cachefile is not created in readonly mode
+        if cacheFileName not in self.open_files:  # or tables.file._open_files.filenames
+            if config.global_caching == 'readonly' and not self.is_cachefile_existent(
+                cacheFileName,
+            ):  # condition ensures that cachefile is not created in readonly mode
                 obj.h5f = None
                 self.busy = False
-#                self._print_open_files()   
+                #                self._print_open_files()
                 return
-            else:
-                if config.global_caching == 'readonly': mode = 'r'
-                f = self.open_cachefile(cacheFileName,mode)
-                self.open_files[cacheFileName] = f
-        
+            if config.global_caching == 'readonly':
+                mode = 'r'
+            f = self.open_cachefile(cacheFileName, mode)
+            self.open_files[cacheFileName] = f
+
         obj.h5f = self.open_files[cacheFileName]
         self._increase_file_reference_counter(cacheFileName)
-        
+
         # garbage collection
         self.close_unreferenced_cachefiles()
-        
+
         self.busy = False
-        self._print_open_files()   
+        self._print_open_files()
+
 
 H5cache = H5cache_class(config=config)
 
-def get_basename(file): 
-    return path.basename(file.filename)
 
+def get_basename(file):
+    return path.basename(file.filename)
```

### Comparing `acoular-24.3/acoular/h5files.py` & `acoular-24.5/acoular/h5files.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,204 +1,221 @@
-# -*- coding: utf-8 -*-
-#pylint: disable-msg=E0611, E1101, C0103, R0901, R0902, R0903, R0904, W0232
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 # Copyright (c) Acoular Development Team.
-#------------------------------------------------------------------------------
-
-try:
-    import tables 
-    is_tables = True
-except:
-    is_tables = False
-    pass
-try:
-    import h5py
-    is_h5py = True
-except:
-    is_h5py = False
+# ------------------------------------------------------------------------------
 
 from .configuration import config
 
 
+class H5FileBase:
+    """Base class for File objects that handle writing and reading of .h5 files."""
+
+    def create_extendable_array(self, nodename, shape, precision, group=None):
+        pass
 
-class H5FileBase(object):
-    '''
-    Base class for File objects that handle writing and reading of .h5 files 
-    '''
-    
-    def create_extendable_array(self,nodename,shape,precision,group=None):
+    def get_data_by_reference(self, nodename, group=None):
         pass
-    
-    def get_data_by_reference(self, nodename,group=None):
+
+    def set_node_attribute(self, node, attrname, value):
         pass
-    
-    def set_node_attribute(self,node,attrname,value):
+
+    def get_node_attribute(self, node, attrname):
         pass
 
-    def get_node_attribute(self,node,attrname):
+    def append_data(self, node, data):
         pass
 
-    def append_data(self,node,data):
+    def remove_data(self, nodename):
         pass
 
-    def remove_data(self,nodename):
-        pass           
-    
-    def create_new_group(self,name,group=None):
+    def create_new_group(self, name, group=None):
         pass
 
-    def get_node_children(self, group):
-        yield
 
+class H5CacheFileBase:
+    """Base class for File objects that handle writing and reading of .h5 cache files."""
 
-class H5CacheFileBase(object):
-    '''
-    Base class for File objects that handle writing and reading of .h5 cache files 
-    '''
-    
     compressionFilter = None
 
-    
-    def is_cached(self,nodename,group=None):
+    def is_cached(self, nodename, group=None):
         pass
-        
-    def create_compressible_array(self,nodename,shape,precision,group=None):
-        pass    
 
+    def create_compressible_array(self, nodename, shape, precision, group=None):
+        pass
+
+
+if config.have_tables:
+    import tables
 
-if is_tables:
-    
     precision_to_atom = {
-        'float32' : tables.Float32Atom(),
-        'complex64' : tables.ComplexAtom(8),
-        'float64' : tables.Float64Atom(),
-        'complex128' : tables.ComplexAtom(16),
-        'bool' : tables.BoolAtom(),
-        'int32' : tables.Int32Atom(),
-        'int16' : tables.Int16Atom(),
-        'int8' : tables.Int8Atom(),        
-        }
-    
-    class H5FileTables(H5FileBase,tables.File):
-        
-        def create_extendable_array(self,nodename,shape,precision,group=None):
-            if not group: group = self.root
+        'float32': tables.Float32Atom(),
+        'complex64': tables.ComplexAtom(8),
+        'float64': tables.Float64Atom(),
+        'complex128': tables.ComplexAtom(16),
+        'bool': tables.BoolAtom(),
+        'int32': tables.Int32Atom(),
+        'int16': tables.Int16Atom(),
+        'int8': tables.Int8Atom(),
+    }
+
+    class H5FileTables(H5FileBase, tables.File):
+        def create_extendable_array(self, nodename, shape, precision, group=None):
+            if not group:
+                group = self.root
             atom = precision_to_atom[precision]
-            self.create_earray(group, nodename, atom, shape) 
-            
-        def get_data_by_reference(self, nodename,group=None):
-            if not group: group = self.root
+            self.create_earray(group, nodename, atom, shape)
+
+        def get_data_by_reference(self, nodename, group=None):
+            if not group:
+                group = self.root
             return self.get_node(group, nodename)
 
-        def set_node_attribute(self,node,attrname,value):
-            node.set_attr(attrname,value)
+        def set_node_attribute(self, node, attrname, value):
+            node.set_attr(attrname, value)
 
-        def get_node_attribute(self,node,attrname):
-            return node.get_attr(attrname)
+        def get_node_attribute(self, node, attrname):
+            return node._v_attrs[attrname]
 
-        def append_data(self,node,data):
+        def append_data(self, node, data):
             node.append(data)
-            
-        def remove_data(self,nodename):
-            self.remove_node('/',nodename,recursive=True)            
-    
-        def create_new_group(self,name,group=None):
-            if not group: group = self.root
-            return self.create_group(group,name)
+
+        def remove_data(self, nodename):
+            self.remove_node('/', nodename, recursive=True)
+
+        def create_new_group(self, name, group=None):
+            if not group:
+                group = self.root
+            return self.create_group(group, name)
 
         def get_child_nodes(self, nodename):
             for childnode in self.list_nodes(nodename):
                 yield (childnode.name, childnode)
 
+        def node_to_dict(self, nodename):
+            """Recursively convert an HDF5 node to a dictionary."""
+            node = self.get_node(nodename)
+            # initialize node-dict with node's own attributes
+            result = {attr: node._v_attrs[attr] for attr in node._v_attrs._f_list()}
+            if isinstance(node, tables.Group):
+                # if node is a group, recursively add its children
+                for childname in node._v_children:
+                    result[childname] = self.node_to_dict(f'{nodename}/{childname}')
+            elif isinstance(node, tables.Leaf):
+                # if node contains only data, add it
+                return node
+            else:
+                return None
+            return result
 
     class H5CacheFileTables(H5FileTables, H5CacheFileBase):
-        
         compressionFilter = tables.Filters(complevel=5, complib='blosc')
-        
-        def is_cached(self,nodename,group=None):
-            if not group: group = self.root
-            if nodename in group: 
+
+        def is_cached(self, nodename, group=None):
+            if not group:
+                group = self.root
+            if nodename in group:
                 return True
-            else:
-                return False
-            
-        def create_compressible_array(self,nodename,shape,precision,group=None):
-            if not group: group = self.root
+            return False
+
+        def create_compressible_array(self, nodename, shape, precision, group=None):
+            if not group:
+                group = self.root
             atom = precision_to_atom[precision]
-            self.create_carray(group, nodename, atom, shape, 
-                                        filters=self.compressionFilter)
+            self.create_carray(group, nodename, atom, shape, filters=self.compressionFilter)
+
 
-    
+if config.have_h5py:
+    import h5py
 
-if is_h5py:
-    
-    class H5FileH5py(H5FileBase,h5py.File):
-        
-        def _get_in_file_path(self,nodename,group=None):
-            if not group: return '/'+nodename
-            else: return group+'/'+nodename
-
-        def create_array(self,where, name, obj):
-            self.create_dataset(f'{where}/{name}',data=obj)
-                  
-        def create_extendable_array(self,nodename,shape,precision,group=None):
-            in_file_path = self._get_in_file_path(nodename,group)
-            self.create_dataset(in_file_path, shape=shape, dtype=precision,
-                                maxshape=(None,shape[1])) 
-            
-        def get_data_by_reference(self,nodename,group=None):
-            in_file_path = self._get_in_file_path(nodename,group)
+    class H5FileH5py(H5FileBase, h5py.File):
+        def _get_in_file_path(self, nodename, group=None):
+            if not group:
+                return '/' + nodename
+            return group + '/' + nodename
+
+        def create_array(self, where, name, obj):
+            self.create_dataset(f'{where}/{name}', data=obj)
+
+        def create_extendable_array(self, nodename, shape, precision, group=None):
+            in_file_path = self._get_in_file_path(nodename, group)
+            self.create_dataset(in_file_path, shape=shape, dtype=precision, maxshape=(None, shape[1]))
+
+        def get_data_by_reference(self, nodename, group=None):
+            in_file_path = self._get_in_file_path(nodename, group)
             return self[in_file_path]
 
-        def set_node_attribute(self,node,attrname,value):
+        def set_node_attribute(self, node, attrname, value):
             node.attrs[attrname] = value
 
-        def get_node_attribute(self,node,attrname):
+        def get_node_attribute(self, node, attrname):
             return node.attrs[attrname]
 
-        def append_data(self,node,data):
+        def append_data(self, node, data):
             oldShape = node.shape
             newShape = (oldShape[0] + data.shape[0], data.shape[1])
             node.resize(newShape)
-            node[oldShape[0]:newShape[0],:] = data
-    
-        def remove_data(self,nodename,group=None):
-            in_file_path = self._get_in_file_path(nodename,group)
+            node[oldShape[0] : newShape[0], :] = data
+
+        def remove_data(self, nodename, group=None):
+            in_file_path = self._get_in_file_path(nodename, group)
             del self[in_file_path]
 
-        def create_new_group(self,name,group=None):
-            in_file_path = self._get_in_file_path(name,group)
-            self.create_group(in_file_path)    
+        def create_new_group(self, name, group=None):
+            in_file_path = self._get_in_file_path(name, group)
+            self.create_group(in_file_path)
             return in_file_path
 
         def get_child_nodes(self, nodename):
             for childnode in self[nodename]:
                 yield (childnode, self[f'{nodename}/{childnode}'])
 
+        def node_to_dict(self, nodename):
+            """Recursively convert an HDF5 node to a dictionary."""
+            node = self[nodename]
+            # initialize node-dict with node's own attributes
+            result = {attr: node.attrs[attr] for attr in node.attrs}
+            if isinstance(node, h5py.Group):
+                # if node is a group, recursively add its children
+                for childname in node:
+                    result[childname] = self.node_to_dict(f'{nodename}/{childname}')
+            elif isinstance(node, h5py.Dataset):
+                # if node contains only data, add it
+                return node
+            else:
+                return None
+            return result
 
     class H5CacheFileH5py(H5CacheFileBase, H5FileH5py):
+        compressionFilter = 'lzf'
+        #        compressionFilter = 'blosc' # unavailable...
 
-        compressionFilter = "lzf"
-#        compressionFilter = 'blosc' # unavailable...
-    
-        def is_cached(self,nodename,group=None):
-            if not group: group = '/'
-            if group+nodename in self: 
+        def is_cached(self, nodename, group=None):
+            if not group:
+                group = '/'
+            if group + nodename in self:
                 return True
-            else:
-                return False
-            
-        def create_compressible_array(self,nodename,shape,precision,group=None):
-            in_file_path = self._get_in_file_path(nodename,group)
-            self.create_dataset(in_file_path, dtype=precision, shape=shape, 
-                                        compression=self.compressionFilter,
-                                        chunks=True)        
+            return False
 
+        def create_compressible_array(self, nodename, shape, precision, group=None):
+            in_file_path = self._get_in_file_path(nodename, group)
+            self.create_dataset(
+                in_file_path,
+                dtype=precision,
+                shape=shape,
+                compression=self.compressionFilter,
+                chunks=True,
+            )
 
 
 def _get_h5file_class():
-    if config.h5library == "pytables": return H5FileTables
-    elif config.h5library == "h5py": return H5FileH5py    
+    if config.h5library in ['pytables', 'tables']:
+        return H5FileTables
+    if config.h5library == 'h5py':
+        return H5FileH5py
+    return None
+
 
 def _get_cachefile_class():
-    if config.h5library == "pytables": return H5CacheFileTables
-    elif config.h5library == "h5py": return H5CacheFileH5py
+    if config.h5library in ['pytables', 'tables']:
+        return H5CacheFileTables
+    if config.h5library == 'h5py':
+        return H5CacheFileH5py
+    return None
```

### Comparing `acoular-24.3/acoular/microphones.py` & `acoular-24.5/acoular/microphones.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,135 +1,139 @@
-# -*- coding: utf-8 -*-
-#pylint: disable-msg=E0611, E1103, C0103, R0901, R0902, R0903, R0904, W0232
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 # Copyright (c) Acoular Development Team.
-#------------------------------------------------------------------------------
-"""Implements support for array microphone arrangements
+# ------------------------------------------------------------------------------
+"""Implements support for array microphone arrangements.
 
 .. autosummary::
     :toctree: generated/
 
     MicGeom
 
 """
 
 # imports from other packages
-from numpy import array, average 
-from scipy.spatial.distance import cdist
-from traits.api import HasPrivateTraits, Property, File, \
-CArray, cached_property, on_trait_change, ListInt , Bool
-from os import path, strerror
 import errno
+from os import path, strerror
+
+from numpy import array, average
+from scipy.spatial.distance import cdist
+from traits.api import Bool, CArray, File, HasPrivateTraits, ListInt, Property, cached_property, on_trait_change
 
 from .internal import digest
 
 
-class MicGeom( HasPrivateTraits ):
-    """
-    Provides the geometric arrangement of microphones in the array.
-    
-    The geometric arrangement of microphones is read in from an 
-    xml-source with element tag names `pos` and attributes Name, `x`, `y` and `z`. 
+class MicGeom(HasPrivateTraits):
+    """Provides the geometric arrangement of microphones in the array.
+
+    The geometric arrangement of microphones is read in from an
+    xml-source with element tag names `pos` and attributes Name, `x`, `y` and `z`.
     Can also be used with programmatically generated arrangements.
     """
 
     #: Name of the .xml-file from wich to read the data.
-    from_file = File(filter=['*.xml'],
-        desc="name of the xml file to import")
+    from_file = File(filter=['*.xml'], desc='name of the xml file to import')
 
     #: Validate mic geom from file
-    validate_file = Bool(True,
-            desc="Validate mic geom from file")
+    validate_file = Bool(True, desc='Validate mic geom from file')
 
     #: Basename of the .xml-file, without the extension; is set automatically / readonly.
-    basename = Property( depends_on = 'from_file',
-        desc="basename of xml file")
+    basename = Property(depends_on='from_file', desc='basename of xml file')
 
     #: List that gives the indices of channels that should not be considered.
     #: Defaults to a blank list.
-    invalid_channels = ListInt(
-        desc="list of invalid channels")
+    invalid_channels = ListInt(desc='list of invalid channels')
 
     #: Number of microphones in the array; readonly.
-    num_mics = Property( depends_on = ['mpos', ],
-        desc="number of microphones in the geometry")
+    num_mics = Property(depends_on=['mpos'], desc='number of microphones in the geometry')
 
     #: Center of the array (arithmetic mean of all used array positions); readonly.
-    center = Property( depends_on = ['mpos', ],
-        desc="array center")
+    center = Property(depends_on=['mpos'], desc='array center')
 
     #: Aperture of the array (greatest extent between two microphones); readonly.
-    aperture = Property( depends_on = ['mpos', ],
-        desc="array aperture")
+    aperture = Property(depends_on=['mpos'], desc='array aperture')
 
     #: Positions as (3, :attr:`num_mics`) array of floats, may include also invalid
     #: microphones (if any). Set either automatically on change of the
     #: :attr:`from_file` argument or explicitely by assigning an array of floats.
-    mpos_tot = CArray(dtype=float,
-        desc="x, y, z position of all microphones")
+    mpos_tot = CArray(dtype=float, desc='x, y, z position of all microphones')
 
     #: Positions as (3, :attr:`num_mics`) array of floats, without invalid
     #: microphones; readonly.
-    mpos = Property( depends_on = ['mpos_tot', 'invalid_channels'],
-        desc="x, y, z position of microphones")
+    mpos = Property(depends_on=['mpos_tot', 'invalid_channels'], desc='x, y, z position of microphones')
 
     # internal identifier
-    digest = Property( depends_on = ['mpos', ])
+    digest = Property(depends_on=['mpos'])
 
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
     @cached_property
-    def _get_basename( self ):
+    def _get_basename(self):
         return path.splitext(path.basename(self.from_file))[0]
 
     @cached_property
-    def _get_mpos( self ):
+    def _get_mpos(self):
         if self.validate_file:
-            if len(self.invalid_channels)==0:
+            if len(self.invalid_channels) == 0:
                 return self.mpos_tot
-            allr=[i for i in range(self.mpos_tot.shape[-1]) if i not in self.invalid_channels]
+            allr = [i for i in range(self.mpos_tot.shape[-1]) if i not in self.invalid_channels]
             return self.mpos_tot[:, array(allr)]
-        else:             
-            raise FileNotFoundError(
-                    errno.ENOENT, strerror(errno.ENOENT), self.from_file)
+        raise FileNotFoundError(errno.ENOENT, strerror(errno.ENOENT), self.from_file)
 
     @cached_property
-    def _get_num_mics( self ):
+    def _get_num_mics(self):
         return self.mpos.shape[-1]
 
     @cached_property
-    def _get_center( self ):
+    def _get_center(self):
         if self.mpos.any():
-            center = average(self.mpos,axis=1)
+            center = average(self.mpos, axis=1)
             # set very small values to zero
-            center[abs(center) < 1e-16] = 0.
+            center[abs(center) < 1e-16] = 0.0
             return center
+        return None
 
     @cached_property
-    def _get_aperture( self ):
+    def _get_aperture(self):
         if self.mpos.any():
-            return cdist(self.mpos.T,self.mpos.T).max()
+            return cdist(self.mpos.T, self.mpos.T).max()
+        return None
 
     @on_trait_change('basename')
-    def import_mpos( self ):
-        """
-        Import the microphone positions from .xml file.
+    def import_mpos(self):
+        """Import the microphone positions from .xml file.
         Called when :attr:`basename` changes.
         """
         if not path.isfile(self.from_file):
             # no file there
             self.mpos_tot = array([], 'd')
             # raise error: File not found on _get functions
             self.validate_file = False
 
         import xml.dom.minidom
+
         doc = xml.dom.minidom.parse(self.from_file)
         names = []
         xyz = []
         for el in doc.getElementsByTagName('pos'):
             names.append(el.getAttribute('Name'))
-            xyz.append(list(map(lambda a : float(el.getAttribute(a)), 'xyz')))
+            xyz.append([float(el.getAttribute(a)) for a in 'xyz'])
         self.mpos_tot = array(xyz, 'd').swapaxes(0, 1)
         self.validate_file = True
 
+    def export_mpos(self, filename):
+        """Export the microphone positions to .xml file.
+
+        Parameters
+        ----------
+        filename : str
+            Name of the file to which the microphone positions are written.
+        """
+        basename = path.splitext(path.basename(filename))[0]
+        with open(filename, 'w') as f:
+            f.write(f'<?xml version="1.1" encoding="utf-8"?><MicArray name="{basename}">\n')
+            for i in range(self.mpos.shape[-1]):
+                f.write(
+                    f'  <pos Name="Point {i+1}" x="{self.mpos[0, i]}" y="{self.mpos[1, i]}" z="{self.mpos[2, i]}"/>\n',
+                )
+            f.write('</MicArray>')
```

### Comparing `acoular-24.3/acoular/sdinput.py` & `acoular-24.5/acoular/sdinput.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,118 +1,113 @@
-# -*- coding: utf-8 -*-
-#pylint: disable-msg=E0611, E1101, C0103, R0901, R0902, R0903, R0904, W0232
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 # Copyright (c) Acoular Development Team.
-#------------------------------------------------------------------------------
-""" Input from soundcard hardware using the SoundDevice library
+# ------------------------------------------------------------------------------
+"""Input from soundcard hardware using the SoundDevice library.
 
 .. autosummary::
     :toctree: generated/
 
     SoundDeviceSamplesGenerator
 """
+
 import sounddevice as sd
-from traits.api import Int, Long, Bool, Property, Any, observe, cached_property
-from .tprocess import SamplesGenerator
+from traits.api import Any, Bool, Int, Long, Property, cached_property, observe
+
 from .internal import digest
+from .tprocess import SamplesGenerator
 
-class SoundDeviceSamplesGenerator(SamplesGenerator):
 
-    """
-    Controller for sound card hardware using sounddevice library
+class SoundDeviceSamplesGenerator(SamplesGenerator):
+    """Controller for sound card hardware using sounddevice library.
 
     Uses the device with index :attr:`device` to read samples
     from input stream, generates output stream via the generator
     :meth:`result`.
     """
 
     #: input device index, refers to sounddevice list
-    device = Int(0, desc="input device index")
+    device = Int(0, desc='input device index')
 
     #: Number of input channels, maximum depends on device
-    numchannels = Long(1,
-       desc="number of analog input channels that collects data")
+    numchannels = Long(1, desc='number of analog input channels that collects data')
 
     #: Number of samples to collect; defaults to -1.
     # If is set to -1 device collects till user breaks streaming by setting Trait: collectsamples = False
-    numsamples = Long(-1,
-        desc="number of samples to collect")    
+    numsamples = Long(-1, desc='number of samples to collect')
 
     #: Indicates if samples are collected, helper trait to break result loop
-    collectsamples = Bool(True,
-        desc="Indicates if samples are collected")
+    collectsamples = Bool(True, desc='Indicates if samples are collected')
 
     #: Sampling frequency of the signal, changes with sinusdevices
-    sample_freq = Property(
-        desc="sampling frequency")
+    sample_freq = Property(desc='sampling frequency')
 
     #: Indicates that the sounddevice buffer has overflown
-    overflow = Bool(False,
-        desc="Indicates if sounddevice buffer overflow")
+    overflow = Bool(False, desc='Indicates if sounddevice buffer overflow')
 
     #: Indicates that the stream is collecting samples
-    running = Bool(False,
-        desc="Indicates that the stream is collecting samples")
+    running = Bool(False, desc='Indicates that the stream is collecting samples')
 
     #: The sounddevice InputStream object for inspection
     stream = Any
 
     # internal identifier
-    digest = Property( depends_on=['device', 'numchannels', 'numsamples'])
-    
+    digest = Property(depends_on=['device', 'numchannels', 'numsamples'])
+
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
     # checks that numchannels are not more than device can provide
     @observe('device,numchannels')
-    def _get_numchannels( self, change ):
-        self.numchannels = min(self.numchannels,sd.query_devices(self.device)['max_input_channels'])
+    def _get_numchannels(self, event):  # noqa ARG002
+        self.numchannels = min(self.numchannels, sd.query_devices(self.device)['max_input_channels'])
 
-    def _get_sample_freq( self ):
+    def _get_sample_freq(self):
         return sd.query_devices(self.device)['default_samplerate']
 
-    def device_properties( self ):
-        """
-        Returns
+    def device_properties(self):
+        """Returns
         -------
         Dictionary of device properties according to sounddevice
         """
         return sd.query_devices(self.device)
 
     def result(self, num):
-        """
-        Python generator that yields the output block-wise. Use at least a 
-        block-size of one ring cache block. 
-        
+        """Python generator that yields the output block-wise. Use at least a
+        block-size of one ring cache block.
+
         Parameters
         ----------
         num : integer
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block).
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, :attr:`numchannels`). 
+        Samples in blocks of shape (num, :attr:`numchannels`).
             The last block may be shorter than num.
+
         """
-        print(self.device_properties(),self.sample_freq)
+        print(self.device_properties(), self.sample_freq)
         self.stream = stream_obj = sd.InputStream(
-                device=self.device, channels=self.numchannels, 
-                clip_off=True, samplerate=self.sample_freq)
+            device=self.device,
+            channels=self.numchannels,
+            clip_off=True,
+            samplerate=self.sample_freq,
+        )
 
         with stream_obj as stream:
             self.running = True
-            if self.numsamples == -1: 
-                while self.collectsamples: # yield data as long as collectsamples is True
-                    data,self.overflow = stream.read(num)
-                    yield data[:num]   
-                                           
-            elif self.numsamples > 0: # amount of samples to collect is specified by user            
-                samples_count = 0 # numsamples counter 
-                while samples_count < self.numsamples: 
-                    anz = min(num, self.numsamples-samples_count)
+            if self.numsamples == -1:
+                while self.collectsamples:  # yield data as long as collectsamples is True
+                    data, self.overflow = stream.read(num)
+                    yield data[:num]
+
+            elif self.numsamples > 0:  # amount of samples to collect is specified by user
+                samples_count = 0  # numsamples counter
+                while samples_count < self.numsamples:
+                    anz = min(num, self.numsamples - samples_count)
                     data, self.overflow = stream.read(num)
-                    yield data[:anz]   
+                    yield data[:anz]
                     samples_count += anz
         self.running = False
-        return  
+        return
```

### Comparing `acoular-24.3/acoular/signals.py` & `acoular-24.5/acoular/signals.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-# -*- coding: utf-8 -*-
-#pylint: disable-msg=E0611, E1101, C0103, R0901, R0902, R0903, R0904, W0232
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 # Copyright (c) Acoular Development Team.
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 """Implements signal generators for the simulation of acoustic sources.
 
 .. autosummary::
     :toctree: generated/
 
     SignalGenerator
     WNoiseGenerator
@@ -14,356 +12,346 @@
     FiltWNoiseGenerator
     SineGenerator
     GenericSignalGenerator
 
 """
 
 # imports from other packages
-from __future__ import print_function, division
-from numpy import pi, arange, sin, sqrt, repeat, tile, log, zeros, array
+from warnings import warn
+
+from numpy import arange, array, log, pi, repeat, sin, sqrt, tile, zeros
 from numpy.random import RandomState
-from traits.api import HasPrivateTraits, Trait, Float, Int, CLong, Bool, \
-Property, cached_property, Delegate, CArray
 from scipy.signal import resample, sosfilt, tf2sos
-from warnings import warn
+from traits.api import Bool, CArray, CLong, Delegate, Float, HasPrivateTraits, Int, Property, Trait, cached_property
+
+from .internal import digest
 
 # acoular imports
 from .tprocess import SamplesGenerator
-from .internal import digest
 
-class SignalGenerator( HasPrivateTraits ):
-    """
-    Virtual base class for a simple one-channel signal generator.
-    
+
+class SignalGenerator(HasPrivateTraits):
+    """Virtual base class for a simple one-channel signal generator.
+
     Defines the common interface for all SignalGenerator classes. This class
     may be used as a base for specialized SignalGenerator implementations. It
     should not be used directly as it contains no real functionality.
     """
 
     #: RMS amplitude of source signal (for point source: in 1 m distance).
-    rms = Float(1.0, 
-        desc="rms amplitude")
-    
+    rms = Float(1.0, desc='rms amplitude')
+
     #: Sampling frequency of the signal.
-    sample_freq = Float(1.0, 
-        desc="sampling frequency")
-                   
+    sample_freq = Float(1.0, desc='sampling frequency')
+
     #: Number of samples to generate.
     numsamples = CLong
-    
+
     # internal identifier
     digest = Property
 
-    def _get_digest( self ):
+    def _get_digest(self):
         return ''
 
     def signal(self):
-        """
-        Deliver the signal.
-        """
-        pass
-    
+        """Deliver the signal."""
+
     def usignal(self, factor):
-        """
-        Delivers the signal resampled with a multiple of the sampling freq.
-        
+        """Delivers the signal resampled with a multiple of the sampling freq.
+
         Uses fourier transform method for resampling (from scipy.signal).
-        
+
         Parameters
         ----------
         factor : integer
             The factor defines how many times the new sampling frequency is
             larger than :attr:`sample_freq`.
-        
+
         Returns
         -------
         array of floats
             The resulting signal of length `factor` * :attr:`numsamples`.
+
         """
-        return resample(self.signal(), factor*self.numsamples)
+        return resample(self.signal(), factor * self.numsamples)
 
-class WNoiseGenerator( SignalGenerator ):
-    """
-    White noise signal generator. 
-    """
+
+class WNoiseGenerator(SignalGenerator):
+    """White noise signal generator."""
 
     #: Seed for random number generator, defaults to 0.
     #: This parameter should be set differently for different instances
     #: to guarantee statistically independent (non-correlated) outputs.
-    seed = Int(0, 
-        desc="random seed value")
+    seed = Int(0, desc='random seed value')
 
     # internal identifier
-    digest = Property( 
-        depends_on = ['rms', 'numsamples', \
-        'sample_freq', 'seed', '__class__'], 
-        )
-               
+    digest = Property(
+        depends_on=['rms', 'numsamples', 'sample_freq', 'seed', '__class__'],
+    )
+
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
     def signal(self):
-        """
-        Deliver the signal.
+        """Deliver the signal.
 
         Returns
         -------
         Array of floats
             The resulting signal as an array of length :attr:`~SignalGenerator.numsamples`.
+
         """
         rnd_gen = RandomState(self.seed)
-        return self.rms*rnd_gen.standard_normal(self.numsamples)
-    
+        return self.rms * rnd_gen.standard_normal(self.numsamples)
+
+
+class PNoiseGenerator(SignalGenerator):
+    """Pink noise signal generator.
 
-class PNoiseGenerator( SignalGenerator ):
-    """
-    Pink noise signal generator.
-    
     Simulation of pink noise is based on the Voss-McCartney algorithm.
     Ref.:
-        
+
       * S.J. Orfanidis: Signal Processing (2010), pp. 729-733
       * online discussion: http://www.firstpr.com.au/dsp/pink-noise/
-      
-    The idea is to iteratively add larger-wavelength noise to get 1/f 
+
+    The idea is to iteratively add larger-wavelength noise to get 1/f
     characteristic.
     """
-    
+
     #: Seed for random number generator, defaults to 0.
     #: This parameter should be set differently for different instances
     #: to guarantee statistically independent (non-correlated) outputs.
-    seed = Int(0, 
-        desc="random seed value")
-    
-    #: "Octave depth" -- higher values for 1/f spectrum at low frequencies, 
+    seed = Int(0, desc='random seed value')
+
+    #: "Octave depth" -- higher values for 1/f spectrum at low frequencies,
     #: but longer calculation, defaults to 16.
-    depth = Int(16,
-        desc="octave depth")
+    depth = Int(16, desc='octave depth')
 
     # internal identifier
-    digest = Property( 
-        depends_on = ['rms', 'numsamples', \
-        'sample_freq', 'seed', 'depth', '__class__'], 
-        )
-               
+    digest = Property(
+        depends_on=['rms', 'numsamples', 'sample_freq', 'seed', 'depth', '__class__'],
+    )
+
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
     def signal(self):
         nums = self.numsamples
         depth = self.depth
         # maximum depth depending on number of samples
-        max_depth = int( log(nums) / log(2) )
-        
+        max_depth = int(log(nums) / log(2))
+
         if depth > max_depth:
             depth = max_depth
-            print("Pink noise filter depth set to maximum possible value of %d." % max_depth)
-        
+            print('Pink noise filter depth set to maximum possible value of %d.' % max_depth)
+
         rnd_gen = RandomState(self.seed)
         s = rnd_gen.standard_normal(nums)
         for _ in range(depth):
-            ind = 2**_-1
-            lind = nums-ind
-            dind = 2**(_+1)
-            s[ind:] += repeat( rnd_gen.standard_normal(nums // dind+1 ), dind)[:lind]
+            ind = 2**_ - 1
+            lind = nums - ind
+            dind = 2 ** (_ + 1)
+            s[ind:] += repeat(rnd_gen.standard_normal(nums // dind + 1), dind)[:lind]
         # divide by sqrt(depth+1.5) to get same overall level as white noise
-        return self.rms/sqrt(depth+1.5) * s
+        return self.rms / sqrt(depth + 1.5) * s
 
 
 class FiltWNoiseGenerator(WNoiseGenerator):
-    """
-    Filtered white noise signal following an autoregressive (AR), moving-average
+    """Filtered white noise signal following an autoregressive (AR), moving-average
     (MA) or autoregressive moving-average (ARMA) process.
-    
-    The desired frequency response of the filter can be defined by specifying 
-    the filter coefficients :attr:`ar` and :attr:`ma`. 
-    The RMS value specified via the :attr:`rms` attribute belongs to the white noise 
-    signal and differs from the RMS value of the filtered signal.  
-    For numerical stability at high orders, the filter is a combination of second order 
-    sections (sos). 
+
+    The desired frequency response of the filter can be defined by specifying
+    the filter coefficients :attr:`ar` and :attr:`ma`.
+    The RMS value specified via the :attr:`rms` attribute belongs to the white noise
+    signal and differs from the RMS value of the filtered signal.
+    For numerical stability at high orders, the filter is a combination of second order
+    sections (sos).
     """
 
-    ar = CArray(value=array([]),dtype=float,
-        desc="autoregressive coefficients (coefficients of the denominator)")
-    
-    ma = CArray(value=array([]),dtype=float,
-        desc="moving-average coefficients (coefficients of the numerator)")
-    
+    ar = CArray(value=array([]), dtype=float, desc='autoregressive coefficients (coefficients of the denominator)')
+
+    ma = CArray(value=array([]), dtype=float, desc='moving-average coefficients (coefficients of the numerator)')
+
     # internal identifier
-    digest = Property( 
-        depends_on = [
-            'ar', 'ma', 'rms', 'numsamples', \
-        'sample_freq', 'seed', '__class__'
-        ], 
-        )
-        
+    digest = Property(
+        depends_on=[
+            'ar',
+            'ma',
+            'rms',
+            'numsamples',
+            'sample_freq',
+            'seed',
+            '__class__',
+        ],
+    )
+
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
-    def handle_empty_coefficients(self,coefficients):
+    def handle_empty_coefficients(self, coefficients):
         if coefficients.size == 0:
             return array([1.0])
-        else:
-            return coefficients
-      
+        return coefficients
+
     def signal(self):
-        """
-        Deliver the signal.
+        """Deliver the signal.
 
         Returns
         -------
         Array of floats
             The resulting signal as an array of length :attr:`~SignalGenerator.numsamples`.
+
         """
         rnd_gen = RandomState(self.seed)
         ma = self.handle_empty_coefficients(self.ma)
         ar = self.handle_empty_coefficients(self.ar)
         sos = tf2sos(ma, ar)
         ntaps = ma.shape[0]
-        sdelay = round(0.5*(ntaps-1)) 
-        wnoise = self.rms*rnd_gen.standard_normal(self.numsamples+sdelay) # create longer signal to compensate delay
+        sdelay = round(0.5 * (ntaps - 1))
+        wnoise = self.rms * rnd_gen.standard_normal(
+            self.numsamples + sdelay,
+        )  # create longer signal to compensate delay
         return sosfilt(sos, x=wnoise)[sdelay:]
 
 
-class SineGenerator( SignalGenerator ):
-    """
-    Sine signal generator with adjustable frequency and phase.
-    """
+class SineGenerator(SignalGenerator):
+    """Sine signal generator with adjustable frequency and phase."""
 
     #: Sine wave frequency, float, defaults to 1000.0.
-    freq = Float(1000.0, 
-        desc="Frequency")
+    freq = Float(1000.0, desc='Frequency')
 
     #: Sine wave phase (in radians), float, defaults to 0.0.
-    phase = Float(0.0, 
-        desc="Phase")
+    phase = Float(0.0, desc='Phase')
 
     # Internal shadow trait for rms/amplitude values.
     # Do not set directly.
     _amp = Float(1.0)
-    
+
     #: RMS of source signal (for point source: in 1 m distance).
     #: Deprecated. For amplitude use :attr:`amplitude`.
     rms = Property(desc='rms amplitude')
-    
+
     def _get_rms(self):
-        return self._amp/2**0.5
-    
+        return self._amp / 2**0.5
+
     def _set_rms(self, rms):
-        warn("Up to Acoular 20.02, rms is interpreted as sine amplitude. "
-             "This has since been corrected (rms now is 1/sqrt(2) of amplitude). "
-             "Use 'amplitude' trait to directly set the ampltiude.", 
-             Warning, stacklevel = 2)
+        warn(
+            'Up to Acoular 20.02, rms is interpreted as sine amplitude. '
+            'This has since been corrected (rms now is 1/sqrt(2) of amplitude). '
+            "Use 'amplitude' trait to directly set the ampltiude.",
+            Warning,
+            stacklevel=2,
+        )
         self._amp = rms * 2**0.5
-    
-    #: Amplitude of source signal (for point source: in 1 m distance). 
+
+    #: Amplitude of source signal (for point source: in 1 m distance).
     #: Defaults to 1.0.
     amplitude = Property(desc='amplitude')
-    
+
     def _get_amplitude(self):
         return self._amp
-    
+
     def _set_amplitude(self, amp):
         self._amp = amp
-    
+
     # internal identifier
-    digest = Property( 
-        depends_on = ['_amp', 'numsamples', \
-        'sample_freq', 'freq', 'phase', '__class__'], 
-        )
-               
+    digest = Property(
+        depends_on=['_amp', 'numsamples', 'sample_freq', 'freq', 'phase', '__class__'],
+    )
+
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
     def signal(self):
-        """
-        Deliver the signal.
+        """Deliver the signal.
 
         Returns
         -------
         array of floats
             The resulting signal as an array of length :attr:`~SignalGenerator.numsamples`.
+
         """
-        t = arange(self.numsamples, dtype=float)/self.sample_freq
-        return self.amplitude * sin(2*pi*self.freq * t + self.phase)
+        t = arange(self.numsamples, dtype=float) / self.sample_freq
+        return self.amplitude * sin(2 * pi * self.freq * t + self.phase)
 
 
-class GenericSignalGenerator( SignalGenerator ):
-    """
-    Generate signal from output of :class:`~acoular.tprocess.SamplesGenerator` object.
-    """
+class GenericSignalGenerator(SignalGenerator):
+    """Generate signal from output of :class:`~acoular.tprocess.SamplesGenerator` object."""
+
     #: Data source; :class:`~acoular.tprocess.SamplesGenerator` or derived object.
     source = Trait(SamplesGenerator)
-    
+
     #: Sampling frequency of output signal, as given by :attr:`source`.
     sample_freq = Delegate('source')
-    
+
     _numsamples = CLong(0)
-   
+
     #: Number of samples to generate. Is set to source.numsamples by default.
     numsamples = Property()
-    
-    def _get_numsamples( self ):
+
+    def _get_numsamples(self):
         if self._numsamples:
             return self._numsamples
-        else:
-            return self.source.numsamples
-    
-    def _set_numsamples( self, numsamples ):
+        return self.source.numsamples
+
+    def _set_numsamples(self, numsamples):
         self._numsamples = numsamples
 
-    #: Boolean flag, if 'True' (default), signal track is repeated if requested 
+    #: Boolean flag, if 'True' (default), signal track is repeated if requested
     #: :attr:`numsamples` is higher than available sample number
     loop_signal = Bool(True)
-    
+
     # internal identifier
-    digest = Property( 
-        depends_on = ['source.digest', 'loop_signal', 'numsamples', \
-        'rms', '__class__'], 
-        )
-               
+    digest = Property(
+        depends_on=['source.digest', 'loop_signal', 'numsamples', 'rms', '__class__'],
+    )
+
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
-    
+
     def signal(self):
-        """
-        Deliver the signal.
+        """Deliver the signal.
 
         Returns
         -------
         array of floats
             The resulting signal as an array of length :attr:`~GenericSignalGenerator.numsamples`.
+
         """
         block = 1024
         if self.source.numchannels > 1:
-            warn("Signal source has more than one channel. Only channel 0 will be used for signal.", Warning, stacklevel = 2)
+            warn(
+                'Signal source has more than one channel. Only channel 0 will be used for signal.',
+                Warning,
+                stacklevel=2,
+            )
         nums = self.numsamples
         track = zeros(nums)
-        
+
         # iterate through source generator to fill signal track
         for i, temp in enumerate(self.source.result(block)):
-            start = block*i
-            stop = start + len(temp[:,0])
+            start = block * i
+            stop = start + len(temp[:, 0])
             if nums > stop:
-                track[start:stop] = temp[:,0]
-            else: # exit loop preliminarily if wanted signal samples are reached
-                track[start:nums] = temp[:nums-start,0]
+                track[start:stop] = temp[:, 0]
+            else:  # exit loop preliminarily if wanted signal samples are reached
+                track[start:nums] = temp[: nums - start, 0]
                 break
-        
+
         # if the signal should be repeated after finishing and there are still samples open
         if self.loop_signal and (nums > stop):
-            
             # fill up empty track with as many full source signals as possible
             nloops = nums // stop
-            if nloops>1: track[stop:stop*nloops] = tile(track[:stop], nloops-1)
+            if nloops > 1:
+                track[stop : stop * nloops] = tile(track[:stop], nloops - 1)
             # fill up remaining empty track
-            res = nums % stop # last part of unfinished loop
-            if res > 0: track[stop*nloops:] = track[:res]
-        
+            res = nums % stop  # last part of unfinished loop
+            if res > 0:
+                track[stop * nloops :] = track[:res]
+
         # The rms value is just an amplification here
-        return self.rms*track
-    
+        return self.rms * track
```

### Comparing `acoular-24.3/acoular/sources.py` & `acoular-24.5/acoular/sources.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-# -*- coding: utf-8 -*-
-#pylint: disable-msg=E0611, E1101, C0103, R0901, R0902, R0903, R0904, W0232
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 # Copyright (c) Acoular Development Team.
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 """Measured multichannel data managment and simulation of acoustic sources.
 
 .. autosummary::
     :toctree: generated/
 
     TimeSamples
     MaskedTimeSamples
@@ -20,1405 +18,1532 @@
     UncorrelatedNoiseSource
     SourceMixer
     PointSourceConvolve
 """
 
 # imports from other packages
 
-from numpy import array, sqrt, ones, empty, newaxis, uint32, arange, dot, int64 ,real, pi, tile,\
-cross, zeros, ceil, repeat
-from numpy import min as npmin
-from numpy import any as npany
-
-from numpy.fft import ifft, fft
-from numpy.linalg import norm
-
-import numba as nb
-
-from traits.api import Float, Int, Property, Trait, Delegate, \
-cached_property, Tuple, CLong, File, Instance, Any, Str, \
-on_trait_change, observe, List, ListInt, CArray, Bool, Dict, Enum
 from os import path
 from warnings import warn
 
+import numba as nb
+from numpy import any as npany
+from numpy import (
+    arange,
+    arctan2,
+    array,
+    ceil,
+    complex128,
+    cross,
+    dot,
+    empty,
+    int64,
+    mod,
+    newaxis,
+    ones,
+    pi,
+    real,
+    repeat,
+    sqrt,
+    tile,
+    uint32,
+    zeros,
+)
+from numpy import min as npmin
+from numpy.fft import fft, ifft
+from numpy.linalg import norm
+from scipy.special import sph_harm, spherical_jn, spherical_yn
+from traits.api import (
+    Any,
+    Bool,
+    CArray,
+    CLong,
+    Delegate,
+    Dict,
+    Enum,
+    File,
+    Float,
+    Instance,
+    Int,
+    List,
+    ListInt,
+    Property,
+    Str,
+    Trait,
+    Tuple,
+    cached_property,
+    observe,
+    on_trait_change,
+)
+
 # acoular imports
 from .calib import Calib
-from .trajectory import Trajectory
+from .environments import Environment
+from .h5files import H5FileBase, _get_h5file_class
 from .internal import digest, ldigest
 from .microphones import MicGeom
-from .environments import Environment
-from .tprocess import SamplesGenerator, TimeConvolve
 from .signals import SignalGenerator
-from .h5files import H5FileBase, _get_h5file_class
-from .tools import get_modes
+from .tprocess import SamplesGenerator, TimeConvolve
+from .trajectory import Trajectory
 
 
-@nb.njit(cache=True, error_model="numpy") # jit with nopython        
-def _fill_mic_signal_block(out,signal,rm,ind,blocksize,numchannels,up,prepadding):
+@nb.njit(cache=True, error_model='numpy')  # jit with nopython
+def _fill_mic_signal_block(out, signal, rm, ind, blocksize, numchannels, up, prepadding):
     if prepadding:
         for b in range(blocksize):
             for m in range(numchannels):
-                if ind[0,m]<0:
-                    out[b,m] = 0
+                if ind[0, m] < 0:
+                    out[b, m] = 0
                 else:
-                    out[b,m] = signal[int(0.5+ind[0,m])]/rm[0,m]
+                    out[b, m] = signal[int(0.5 + ind[0, m])] / rm[0, m]
             ind += up
     else:
         for b in range(blocksize):
             for m in range(numchannels):
-                out[b,m] = signal[int(0.5+ind[0,m])]/rm[0,m]
+                out[b, m] = signal[int(0.5 + ind[0, m])] / rm[0, m]
             ind += up
     return out
 
 
-class TimeSamples( SamplesGenerator ):
+def spherical_hn1(n, z, derivativearccos=False):
+    """Spherical Hankel Function of the First Kind."""
+    return spherical_jn(n, z, derivative=False) + 1j * spherical_yn(n, z, derivative=False)
+
+
+def get_radiation_angles(direction, mpos, sourceposition):
+    """Returns azimuthal and elevation angles between the mics and the source.
+
+    Parameters
+    ----------
+    direction : array of floats
+        Spherical Harmonic orientation
+    mpos : array of floats
+        x, y, z position of microphones
+    sourceposition : array of floats
+        position of the source
+
+    Returns
+    -------
+    azi, ele : array of floats
+        the angle between the mics and the source
+
+    """
+    # direction of the Spherical Harmonics
+    direc = array(direction, dtype=float)
+    direc = direc / norm(direc)
+    # distances
+    source_to_mic_vecs = mpos - array(sourceposition).reshape((3, 1))
+    source_to_mic_vecs[2] *= -1  # invert z-axis (acoular)    #-1
+    # z-axis (acoular) -> y-axis (spherical)
+    # y-axis (acoular) -> z-axis (spherical)
+    # theta
+    ele = arctan2(sqrt(source_to_mic_vecs[0] ** 2 + source_to_mic_vecs[2] ** 2), source_to_mic_vecs[1])
+    ele += arctan2(sqrt(direc[0] ** 2 + direc[2] ** 2), direc[1])
+    ele += pi * 0.5  # convert from [-pi/2, pi/2] to [0,pi] range
+    # phi
+    azi = arctan2(source_to_mic_vecs[2], source_to_mic_vecs[0])
+    azi += arctan2(direc[2], direc[0])
+    azi = mod(azi, 2 * pi)
+    return azi, ele
+
+
+def get_modes(lOrder, direction, mpos, sourceposition=None):
+    """Returns Spherical Harmonic Radiation Pattern at the Microphones.
+
+    Parameters
+    ----------
+    lOrder : int
+        Maximal order of spherical harmonic
+    direction : array of floats
+        Spherical Harmonic orientation
+    mpos : array of floats
+        x, y, z position of microphones
+    sourceposition : array of floats
+        position of the source
+
+    Returns
+    -------
+    modes : array of floats
+        the radiation values at each microphone for each mode
+
     """
-    Container for time data in `*.h5` format.
-    
+    sourceposition = sourceposition if sourceposition is not None else array([0, 0, 0])
+    azi, ele = get_radiation_angles(direction, mpos, sourceposition)  # angles between source and mics
+    modes = zeros((azi.shape[0], (lOrder + 1) ** 2), dtype=complex128)
+    i = 0
+    for l in range(lOrder + 1):
+        for m in range(-l, l + 1):
+            modes[:, i] = sph_harm(m, l, azi, ele)
+            if m < 0:
+                modes[:, i] = modes[:, i].conj() * 1j
+            i += 1
+    return modes
+
+
+class TimeSamples(SamplesGenerator):
+    """Container for time data in `*.h5` format.
+
     This class loads measured data from h5 files and
     and provides information about this data.
     It also serves as an interface where the data can be accessed
     (e.g. for use in a block chain) via the :meth:`result` generator.
     """
 
     #: Full name of the .h5 file with data.
-    name = File(filter=['*.h5'], 
-        desc="name of data file")
+    name = File(filter=['*.h5'], desc='name of data file')
 
     #: Basename of the .h5 file with data, is set automatically.
-    basename = Property( depends_on = 'name', #filter=['*.h5'], 
-        desc="basename of data file")
-    
+    basename = Property(
+        depends_on='name',  # filter=['*.h5'],
+        desc='basename of data file',
+    )
+
     #: Calibration data, instance of :class:`~acoular.calib.Calib` class, optional .
-    calib = Trait( Calib, 
-        desc="Calibration data")
-    
+    calib = Trait(Calib, desc='Calibration data')
+
     #: Number of channels, is set automatically / read from file.
-    numchannels = CLong(0, 
-        desc="number of input channels")
+    numchannels = CLong(0, desc='number of input channels')
 
     #: Number of time data samples, is set automatically / read from file.
-    numsamples = CLong(0, 
-        desc="number of samples")
+    numsamples = CLong(0, desc='number of samples')
 
     #: The time data as array of floats with dimension (numsamples, numchannels).
-    data = Any( transient = True, 
-        desc="the actual time data array")
+    data = Any(transient=True, desc='the actual time data array')
 
     #: HDF5 file object
-    h5f = Instance(H5FileBase, transient = True)
-    
+    h5f = Instance(H5FileBase, transient=True)
+
     #: Provides metadata stored in HDF5 file object
-    metadata = Dict(
-        desc="metadata contained in .h5 file")
-    
+    metadata = Dict(desc='metadata contained in .h5 file')
+
     # Checksum over first data entries of all channels
     _datachecksum = Property()
-    
+
     # internal identifier
-    digest = Property( depends_on = ['basename', 'calib.digest', '_datachecksum'])
+    digest = Property(depends_on=['basename', 'calib.digest', '_datachecksum'])
+
+    def _get__datachecksum(self):
+        return self.data[0, :].sum()
 
-    def _get__datachecksum( self ):
-        return self.data[0,:].sum()
-    
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
-    
+
     @cached_property
-    def _get_basename( self ):
+    def _get_basename(self):
         return path.splitext(path.basename(self.name))[0]
-    
+
     @on_trait_change('basename')
-    def load_data( self ):
-        """ 
-        Open the .h5 file and set attributes.
-        """
+    def load_data(self):
+        """Open the .h5 file and set attributes."""
         if not path.isfile(self.name):
             # no file there
             self.numsamples = 0
             self.numchannels = 0
             self.sample_freq = 0
-            raise IOError("No such file: %s" % self.name)
-        if self.h5f != None:
+            raise OSError('No such file: %s' % self.name)
+        if self.h5f is not None:
             try:
                 self.h5f.close()
-            except IOError:
+            except OSError:
                 pass
         file = _get_h5file_class()
         self.h5f = file(self.name)
         self.load_timedata()
         self.load_metadata()
 
-    def load_timedata( self ):
-        """ loads timedata from .h5 file. Only for internal use. """
-        self.data = self.h5f.get_data_by_reference('time_data')    
-        self.sample_freq = self.h5f.get_node_attribute(self.data,'sample_freq')
+    def load_timedata(self):
+        """Loads timedata from .h5 file. Only for internal use."""
+        self.data = self.h5f.get_data_by_reference('time_data')
+        self.sample_freq = self.h5f.get_node_attribute(self.data, 'sample_freq')
         (self.numsamples, self.numchannels) = self.data.shape
 
-    def load_metadata( self ):
-        """ loads metadata from .h5 file. Only for internal use. """
+    def load_metadata(self):
+        """Loads metadata from .h5 file. Only for internal use."""
         self.metadata = {}
         if '/metadata' in self.h5f:
-            for nodename, nodedata in self.h5f.get_child_nodes('/metadata'):
-                self.metadata[nodename] = nodedata
+            self.metadata = self.h5f.node_to_dict('/metadata')
 
     def result(self, num=128):
-        """
-        Python generator that yields the output block-wise.
-                
+        """Python generator that yields the output block-wise.
+
         Parameters
         ----------
         num : integer, defaults to 128
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block) .
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, numchannels). 
+        Samples in blocks of shape (num, numchannels).
             The last block may be shorter than num.
+
         """
         if self.numsamples == 0:
-            raise IOError("no samples available")
-        self._datachecksum # trigger checksum calculation
+            msg = 'no samples available'
+            raise OSError(msg)
+        self._datachecksum  # trigger checksum calculation # noqa: B018
         i = 0
         if self.calib:
             if self.calib.num_mics == self.numchannels:
                 cal_factor = self.calib.data[newaxis]
             else:
-                raise ValueError("calibration data not compatible: %i, %i" % \
-                            (self.calib.num_mics, self.numchannels))
+                raise ValueError('calibration data not compatible: %i, %i' % (self.calib.num_mics, self.numchannels))
             while i < self.numsamples:
-                yield self.data[i:i+num]*cal_factor
+                yield self.data[i : i + num] * cal_factor
                 i += num
         else:
             while i < self.numsamples:
-                yield self.data[i:i+num]
+                yield self.data[i : i + num]
                 i += num
 
-class MaskedTimeSamples( TimeSamples ):
-    """
-    Container for time data in `*.h5` format.
-    
-    This class loads measured data from h5 files 
+
+class MaskedTimeSamples(TimeSamples):
+    """Container for time data in `*.h5` format.
+
+    This class loads measured data from h5 files
     and provides information about this data.
     It supports storing information about (in)valid samples and (in)valid channels
     It also serves as an interface where the data can be accessed
     (e.g. for use in a block chain) via the :meth:`result` generator.
-    
+
     """
-    
+
     #: Index of the first sample to be considered valid.
-    start = CLong(0, 
-        desc="start of valid samples")
-    
+    start = CLong(0, desc='start of valid samples')
+
     #: Index of the last sample to be considered valid.
-    stop = Trait(None, None, CLong, 
-        desc="stop of valid samples")
-    
+    stop = Trait(None, None, CLong, desc='stop of valid samples')
+
     #: Channels that are to be treated as invalid.
-    invalid_channels = ListInt(
-        desc="list of invalid channels")
-    
+    invalid_channels = ListInt(desc='list of invalid channels')
+
     #: Channel mask to serve as an index for all valid channels, is set automatically.
-    channels = Property(depends_on = ['invalid_channels', 'numchannels_total'], 
-        desc="channel mask")
-        
+    channels = Property(depends_on=['invalid_channels', 'numchannels_total'], desc='channel mask')
+
     #: Number of channels (including invalid channels), is set automatically.
-    numchannels_total = CLong(0, 
-        desc="total number of input channels")
+    numchannels_total = CLong(0, desc='total number of input channels')
 
     #: Number of time data samples (including invalid samples), is set automatically.
-    numsamples_total = CLong(0, 
-        desc="total number of samples per channel")
+    numsamples_total = CLong(0, desc='total number of samples per channel')
 
     #: Number of valid channels, is set automatically.
-    numchannels = Property(depends_on = ['invalid_channels', \
-        'numchannels_total'], desc="number of valid input channels")
+    numchannels = Property(depends_on=['invalid_channels', 'numchannels_total'], desc='number of valid input channels')
 
     #: Number of valid time data samples, is set automatically.
-    numsamples = Property(depends_on = ['start', 'stop', 'numsamples_total'], 
-        desc="number of valid samples per channel")
+    numsamples = Property(depends_on=['start', 'stop', 'numsamples_total'], desc='number of valid samples per channel')
 
     # internal identifier
-    digest = Property( depends_on = ['basename', 'start', 'stop', \
-        'calib.digest', 'invalid_channels','_datachecksum'])
+    digest = Property(depends_on=['basename', 'start', 'stop', 'calib.digest', 'invalid_channels', '_datachecksum'])
 
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
-    
+
     @cached_property
-    def _get_basename( self ):
+    def _get_basename(self):
         return path.splitext(path.basename(self.name))[0]
-    
+
     @cached_property
-    def _get_channels( self ):
-        if len(self.invalid_channels)==0:
+    def _get_channels(self):
+        if len(self.invalid_channels) == 0:
             return slice(0, None, None)
-        allr=[i for i in range(self.numchannels_total) if i not in self.invalid_channels]
+        allr = [i for i in range(self.numchannels_total) if i not in self.invalid_channels]
         return array(allr)
-    
+
     @cached_property
-    def _get_numchannels( self ):
-        if len(self.invalid_channels)==0:
+    def _get_numchannels(self):
+        if len(self.invalid_channels) == 0:
             return self.numchannels_total
         return len(self.channels)
-    
+
     @cached_property
-    def _get_numsamples( self ):
+    def _get_numsamples(self):
         sli = slice(self.start, self.stop).indices(self.numsamples_total)
-        return sli[1]-sli[0]
+        return sli[1] - sli[0]
 
     @on_trait_change('basename')
-    def load_data( self ):
-        #""" open the .h5 file and set attributes
-        #"""
+    def load_data(self):
+        # """ open the .h5 file and set attributes
+        # """
         if not path.isfile(self.name):
             # no file there
             self.numsamples_total = 0
             self.numchannels_total = 0
             self.sample_freq = 0
-            raise IOError("No such file: %s" % self.name)
-        if self.h5f != None:
+            raise OSError('No such file: %s' % self.name)
+        if self.h5f is not None:
             try:
                 self.h5f.close()
-            except IOError:
+            except OSError:
                 pass
         file = _get_h5file_class()
         self.h5f = file(self.name)
         self.load_timedata()
         self.load_metadata()
 
-    def load_timedata( self ):
-        """ loads timedata from .h5 file. Only for internal use. """
-        self.data = self.h5f.get_data_by_reference('time_data')    
-        self.sample_freq = self.h5f.get_node_attribute(self.data,'sample_freq')
+    def load_timedata(self):
+        """Loads timedata from .h5 file. Only for internal use."""
+        self.data = self.h5f.get_data_by_reference('time_data')
+        self.sample_freq = self.h5f.get_node_attribute(self.data, 'sample_freq')
         (self.numsamples_total, self.numchannels_total) = self.data.shape
 
     def result(self, num=128):
-        """
-        Python generator that yields the output block-wise.
-        
+        """Python generator that yields the output block-wise.
+
         Parameters
         ----------
         num : integer, defaults to 128
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block).
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, numchannels). 
+        Samples in blocks of shape (num, numchannels).
             The last block may be shorter than num.
+
         """
         sli = slice(self.start, self.stop).indices(self.numsamples_total)
         i = sli[0]
         stop = sli[1]
         cal_factor = 1.0
         if i >= stop:
-            raise IOError("no samples available")
-        self._datachecksum # trigger checksum calculation
+            msg = 'no samples available'
+            raise OSError(msg)
+        self._datachecksum  # trigger checksum calculation # noqa: B018
         if self.calib:
             if self.calib.num_mics == self.numchannels_total:
                 cal_factor = self.calib.data[self.channels][newaxis]
             elif self.calib.num_mics == self.numchannels:
                 cal_factor = self.calib.data[newaxis]
             elif self.calib.num_mics == 0:
-                warn("No calibration data used.", Warning, stacklevel = 2)    
+                warn('No calibration data used.', Warning, stacklevel=2)
             else:
-                raise ValueError("calibration data not compatible: %i, %i" % \
-                            (self.calib.num_mics, self.numchannels))
+                raise ValueError('calibration data not compatible: %i, %i' % (self.calib.num_mics, self.numchannels))
         while i < stop:
-            yield self.data[i:min(i+num, stop)][:, self.channels]*cal_factor
+            yield self.data[i : min(i + num, stop)][:, self.channels] * cal_factor
             i += num
 
 
-class PointSource( SamplesGenerator ):
-    """
-    Class to define a fixed point source with an arbitrary signal.
+class PointSource(SamplesGenerator):
+    """Class to define a fixed point source with an arbitrary signal.
     This can be used in simulations.
-    
+
     The output is being generated via the :meth:`result` generator.
     """
-    
+
     #:  Emitted signal, instance of the :class:`~acoular.signals.SignalGenerator` class.
     signal = Trait(SignalGenerator)
-    
+
     #: Location of source in (`x`, `y`, `z`) coordinates (left-oriented system).
-    loc = Tuple((0.0, 0.0, 1.0),
-        desc="source location")
-               
-    #: Number of channels in output, is set automatically / 
+    loc = Tuple((0.0, 0.0, 1.0), desc='source location')
+
+    #: Number of channels in output, is set automatically /
     #: depends on used microphone geometry.
     numchannels = Delegate('mics', 'num_mics')
 
     #: :class:`~acoular.microphones.MicGeom` object that provides the microphone locations.
-    mics = Trait(MicGeom, 
-        desc="microphone geometry")
+    mics = Trait(MicGeom, desc='microphone geometry')
 
     def _validate_locations(self):
         dist = self.env._r(array(self.loc).reshape((3, 1)), self.mics.mpos)
         if npany(dist < 1e-7):
-            warn("Source and microphone locations are identical.", Warning, stacklevel = 2)
-    
-    #: :class:`~acoular.environments.Environment` or derived object, 
+            warn('Source and microphone locations are identical.', Warning, stacklevel=2)
+
+    #: :class:`~acoular.environments.Environment` or derived object,
     #: which provides information about the sound propagation in the medium.
     env = Trait(Environment(), Environment)
 
     # --- List of backwards compatibility traits and their setters/getters -----------
 
     # Microphone locations.
     # Deprecated! Use :attr:`mics` trait instead.
     mpos = Property()
-    
+
     def _get_mpos(self):
         return self.mics
-    
+
     def _set_mpos(self, mpos):
-        warn("Deprecated use of 'mpos' trait. ", Warning, stacklevel = 2)
+        warn("Deprecated use of 'mpos' trait. ", Warning, stacklevel=2)
         self.mics = mpos
-        
+
     # The speed of sound.
-    # Deprecated! Only kept for backwards compatibility. 
+    # Deprecated! Only kept for backwards compatibility.
     # Now governed by :attr:`env` trait.
     c = Property()
-    
+
     def _get_c(self):
         return self.env.c
-    
+
     def _set_c(self, c):
-        warn("Deprecated use of 'c' trait. ", Warning, stacklevel = 2)
+        warn("Deprecated use of 'c' trait. ", Warning, stacklevel=2)
         self.env.c = c
 
     # --- End of backwards compatibility traits --------------------------------------
-        
+
     #: Start time of the signal in seconds, defaults to 0 s.
-    start_t = Float(0.0,
-        desc="signal start time")
-    
-    #: Start time of the data aquisition at microphones in seconds, 
+    start_t = Float(0.0, desc='signal start time')
+
+    #: Start time of the data aquisition at microphones in seconds,
     #: defaults to 0 s.
-    start = Float(0.0,
-        desc="sample start time")
+    start = Float(0.0, desc='sample start time')
 
     #: Signal behaviour for negative time indices, i.e. if :attr:`start` < :attr:start_t.
     #: `loop` take values from the end of :attr:`signal.signal()` array.
     #: `zeros` set source signal to zero, advisable for deterministic signals.
     #: defaults to `loop`.
-    prepadding = Trait('loop','zeros', desc="Behaviour for negative time indices.")
+    prepadding = Trait('loop', 'zeros', desc='Behaviour for negative time indices.')
 
     #: Upsampling factor, internal use, defaults to 16.
-    up = Int(16, 
-        desc="upsampling factor")        
-    
-    #: Number of samples, is set automatically / 
+    up = Int(16, desc='upsampling factor')
+
+    #: Number of samples, is set automatically /
     #: depends on :attr:`signal`.
     numsamples = Delegate('signal')
-    
-    #: Sampling frequency of the signal, is set automatically / 
+
+    #: Sampling frequency of the signal, is set automatically /
     #: depends on :attr:`signal`.
-    sample_freq = Delegate('signal') 
+    sample_freq = Delegate('signal')
 
     # internal identifier
-    digest = Property( 
-        depends_on = ['mics.digest', 'signal.digest', 'loc', \
-         'env.digest', 'start_t', 'start', 'up', 'prepadding', '__class__'], 
-        )
-               
+    digest = Property(
+        depends_on=[
+            'mics.digest',
+            'signal.digest',
+            'loc',
+            'env.digest',
+            'start_t',
+            'start',
+            'up',
+            'prepadding',
+            '__class__',
+        ],
+    )
+
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
     def result(self, num=128):
-        """
-        Python generator that yields the output at microphones block-wise.
+        """Python generator that yields the output at microphones block-wise.
 
         Parameters
         ----------
         num : integer, defaults to 128
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block) .
 
         Returns
         -------
-        Samples in blocks of shape (num, numchannels). 
+        Samples in blocks of shape (num, numchannels).
             The last block may be shorter than num.
+
         """
-        
         self._validate_locations()
-        N = int(ceil(self.numsamples/num)) # number of output blocks
+        N = int(ceil(self.numsamples / num))  # number of output blocks
         signal = self.signal.usignal(self.up)
         out = empty((num, self.numchannels))
         # distances
-        rm = self.env._r(array(self.loc).reshape((3, 1)), self.mics.mpos).reshape(1,-1)
+        rm = self.env._r(array(self.loc).reshape((3, 1)), self.mics.mpos).reshape(1, -1)
         # emission time relative to start_t (in samples) for first sample
-        ind = (-rm/self.env.c-self.start_t+self.start)*self.sample_freq*self.up
+        ind = (-rm / self.env.c - self.start_t + self.start) * self.sample_freq * self.up
 
         if self.prepadding == 'zeros':
             # number of blocks where signal behaviour is amended
-            pre = -int(npmin(ind[0])//(self.up*num))
+            pre = -int(npmin(ind[0]) // (self.up * num))
             # amend signal for first blocks
             # if signal stops during prepadding, terminate
-            if N <= pre:
-                for nb in range(N-1):
-                    out = _fill_mic_signal_block(out,signal,rm,ind,num,self.numchannels,self.up,True)
+            if pre >= N:
+                for _nb in range(N - 1):
+                    out = _fill_mic_signal_block(out, signal, rm, ind, num, self.numchannels, self.up, True)
                     yield out
 
-                blocksize = self.numsamples%num or num
-                out = _fill_mic_signal_block(out,signal,rm,ind,blocksize,self.numchannels,self.up,True)
+                blocksize = self.numsamples % num or num
+                out = _fill_mic_signal_block(out, signal, rm, ind, blocksize, self.numchannels, self.up, True)
                 yield out[:blocksize]
                 return
             else:
-                for nb in range(pre):
-                    out = _fill_mic_signal_block(out,signal,rm,ind,num,self.numchannels,self.up,True)
+                for _nb in range(pre):
+                    out = _fill_mic_signal_block(out, signal, rm, ind, num, self.numchannels, self.up, True)
                     yield out
 
         else:
             pre = 0
 
         # main generator
-        for nb in range(N-pre-1):
-            out = _fill_mic_signal_block(out,signal,rm,ind,num,self.numchannels,self.up,False)
+        for _nb in range(N - pre - 1):
+            out = _fill_mic_signal_block(out, signal, rm, ind, num, self.numchannels, self.up, False)
             yield out
 
         # last block of variable size
-        blocksize = self.numsamples%num or num
-        out = _fill_mic_signal_block(out,signal,rm,ind,blocksize,self.numchannels,self.up,False)
+        blocksize = self.numsamples % num or num
+        out = _fill_mic_signal_block(out, signal, rm, ind, blocksize, self.numchannels, self.up, False)
         yield out[:blocksize]
 
 
-class SphericalHarmonicSource( PointSource ):
-    """
-    Class to define a fixed Spherical Harmonic Source with an arbitrary signal.
+class SphericalHarmonicSource(PointSource):
+    """Class to define a fixed Spherical Harmonic Source with an arbitrary signal.
     This can be used in simulations.
-    
+
     The output is being generated via the :meth:`result` generator.
     """
-    
+
     #: Order of spherical harmonic source
-    lOrder = Int(0,
-                   desc ="Order of spherical harmonic")
-    
-    alpha = CArray(desc="coefficients of the (lOrder,) spherical harmonic mode")
-    
-    
-    #: Vector to define the orientation of the SphericalHarmonic. 
-    direction = Tuple((1.0, 0.0, 0.0),
-        desc="Spherical Harmonic orientation")
+    lOrder = Int(0, desc='Order of spherical harmonic')
+
+    alpha = CArray(desc='coefficients of the (lOrder,) spherical harmonic mode')
+
+    #: Vector to define the orientation of the SphericalHarmonic.
+    direction = Tuple((1.0, 0.0, 0.0), desc='Spherical Harmonic orientation')
+
+    prepadding = Enum('loop', desc='Behaviour for negative time indices.')
 
-    prepadding = Enum('loop', desc="Behaviour for negative time indices.")
-    
     # internal identifier
-    digest = Property( 
-        depends_on = ['mics.digest', 'signal.digest', 'loc', \
-         'env.digest', 'start_t', 'start', 'up', '__class__', 'alpha','lOrder', 'prepadding'], 
-        )
-               
+    digest = Property(
+        depends_on=[
+            'mics.digest',
+            'signal.digest',
+            'loc',
+            'env.digest',
+            'start_t',
+            'start',
+            'up',
+            '__class__',
+            'alpha',
+            'lOrder',
+            'prepadding',
+        ],
+    )
+
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
-    def transform(self,signals):
-        Y_lm = get_modes(lOrder = self.lOrder, direction= self.direction, mpos = self.mics.mpos,sourceposition = array(self.loc))
-        return real(ifft(fft(signals,axis=0) * (Y_lm @ self.alpha),axis=0))
+    def transform(self, signals):
+        Y_lm = get_modes(
+            lOrder=self.lOrder,
+            direction=self.direction,
+            mpos=self.mics.mpos,
+            sourceposition=array(self.loc),
+        )
+        return real(ifft(fft(signals, axis=0) * (Y_lm @ self.alpha), axis=0))
 
     def result(self, num=128):
-        """
-        Python generator that yields the output at microphones block-wise.
-                
+        """Python generator that yields the output at microphones block-wise.
+
         Parameters
         ----------
         num : integer, defaults to 128
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block) .
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, numchannels). 
+        Samples in blocks of shape (num, numchannels).
             The last block may be shorter than num.
+
         """
-        #If signal samples are needed for te < t_start, then samples are taken
-        #from the end of the calculated signal.
-        
+        # If signal samples are needed for te < t_start, then samples are taken
+        # from the end of the calculated signal.
+
         signal = self.signal.usignal(self.up)
         # emission time relative to start_t (in samples) for first sample
         rm = self.env._r(array(self.loc).reshape((3, 1)), self.mics.mpos)
-        ind = (-rm/self.env.c-self.start_t+self.start)*self.sample_freq   + pi/30 
+        ind = (-rm / self.env.c - self.start_t + self.start) * self.sample_freq + pi / 30
         i = 0
         n = self.numsamples
         out = empty((num, self.numchannels))
         while n:
             n -= 1
             try:
-                out[i] = signal[array(0.5+ind*self.up, dtype=int64)]/rm
+                out[i] = signal[array(0.5 + ind * self.up, dtype=int64)] / rm
                 ind += 1
                 i += 1
                 if i == num:
                     yield self.transform(out)
                     i = 0
-            except IndexError: #if no more samples available from the source
+            except IndexError:  # if no more samples available from the source
                 break
-        if i > 0: # if there are still samples to yield
+        if i > 0:  # if there are still samples to yield
             yield self.transform(out[:i])
-            
-class MovingPointSource( PointSource ):
-    """
-    Class to define a point source with an arbitrary 
+
+
+class MovingPointSource(PointSource):
+    """Class to define a point source with an arbitrary
     signal moving along a given trajectory.
     This can be used in simulations.
-    
+
     The output is being generated via the :meth:`result` generator.
     """
 
     #: Considering of convective amplification
-    conv_amp = Bool(False, 
-        desc="determines if convective amplification is considered")
+    conv_amp = Bool(False, desc='determines if convective amplification is considered')
 
-    #: Trajectory of the source, 
+    #: Trajectory of the source,
     #: instance of the :class:`~acoular.trajectory.Trajectory` class.
     #: The start time is assumed to be the same as for the samples.
-    trajectory = Trait(Trajectory, 
-        desc="trajectory of the source")
+    trajectory = Trait(Trajectory, desc='trajectory of the source')
 
-    prepadding = Enum('loop', desc="Behaviour for negative time indices.")
+    prepadding = Enum('loop', desc='Behaviour for negative time indices.')
 
     # internal identifier
-    digest = Property( 
-        depends_on = ['mics.digest', 'signal.digest', 'loc', 'conv_amp', \
-         'env.digest', 'start_t', 'start', 'trajectory.digest', 'prepadding', '__class__'], 
-        )
-               
+    digest = Property(
+        depends_on=[
+            'mics.digest',
+            'signal.digest',
+            'loc',
+            'conv_amp',
+            'env.digest',
+            'start_t',
+            'start',
+            'trajectory.digest',
+            'prepadding',
+            '__class__',
+        ],
+    )
+
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
     def result(self, num=128):
-        """
-        Python generator that yields the output at microphones block-wise.
-                
+        """Python generator that yields the output at microphones block-wise.
+
         Parameters
         ----------
         num : integer, defaults to 128
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block).
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, numchannels). 
+        Samples in blocks of shape (num, numchannels).
             The last block may be shorter than num.
-        """   
-        #If signal samples are needed for te < t_start, then samples are taken
-        #from the end of the calculated signal.
-        
+
+        """
+        # If signal samples are needed for te < t_start, then samples are taken
+        # from the end of the calculated signal.
+
         signal = self.signal.usignal(self.up)
         out = empty((num, self.numchannels))
         # shortcuts and intial values
         m = self.mics
-        t = self.start*ones(m.num_mics)
+        t = self.start * ones(m.num_mics)
         i = 0
-        epslim = 0.1/self.up/self.sample_freq
+        epslim = 0.1 / self.up / self.sample_freq
         c0 = self.env.c
         tr = self.trajectory
         n = self.numsamples
         while n:
             n -= 1
             eps = ones(m.num_mics)
-            te = t.copy() # init emission time = receiving time
+            te = t.copy()  # init emission time = receiving time
             j = 0
             # Newton-Rhapson iteration
-            while abs(eps).max()>epslim and j<100:
+            while abs(eps).max() > epslim and j < 100:
                 loc = array(tr.location(te))
-                rm = loc-m.mpos# distance vectors to microphones
-                rm = sqrt((rm*rm).sum(0))# absolute distance
-                loc /= sqrt((loc*loc).sum(0))# distance unit vector
+                rm = loc - m.mpos  # distance vectors to microphones
+                rm = sqrt((rm * rm).sum(0))  # absolute distance
+                loc /= sqrt((loc * loc).sum(0))  # distance unit vector
                 der = array(tr.location(te, der=1))
-                Mr = (der*loc).sum(0)/c0# radial Mach number
-                eps = (te + rm/c0 - t)/(1+Mr)# discrepancy in time 
+                Mr = (der * loc).sum(0) / c0  # radial Mach number
+                eps = (te + rm / c0 - t) / (1 + Mr)  # discrepancy in time
                 te -= eps
-                j += 1 #iteration count
-            t += 1./self.sample_freq
+                j += 1  # iteration count
+            t += 1.0 / self.sample_freq
             # emission time relative to start time
-            ind = (te-self.start_t+self.start)*self.sample_freq
-            if self.conv_amp: rm *= (1-Mr)**2
+            ind = (te - self.start_t + self.start) * self.sample_freq
+            if self.conv_amp:
+                rm *= (1 - Mr) ** 2
             try:
-                out[i] = signal[array(0.5+ind*self.up, dtype=int64)]/rm
+                out[i] = signal[array(0.5 + ind * self.up, dtype=int64)] / rm
                 i += 1
                 if i == num:
                     yield out
                     i = 0
-            except IndexError: #if no more samples available from the source 
+            except IndexError:  # if no more samples available from the source
                 break
-        if i > 0: # if there are still samples to yield
+        if i > 0:  # if there are still samples to yield
             yield out[:i]
-            
 
-class PointSourceDipole ( PointSource ):
-    """
-    Class to define a fixed point source with an arbitrary signal and
+
+class PointSourceDipole(PointSource):
+    """Class to define a fixed point source with an arbitrary signal and
     dipole characteristics via superposition of two nearby inversely
     phased monopoles.
     This can be used in simulations.
-    
+
     The output is being generated via the :meth:`result` generator.
     """
-    
+
     #: Vector to define the orientation of the dipole lobes. Its magnitude
     #: governs the distance between the monopoles
     #: (dist = [lowest wavelength in spectrum] x [magnitude] x 1e-5).
-    #: Note: Use vectors with order of magnitude around 1.0 or less 
+    #: Note: Use vectors with order of magnitude around 1.0 or less
     #: for good results.
-    direction = Tuple((0.0, 0.0, 1.0),
-        desc="dipole orientation and distance of the inversely phased monopoles")
+    direction = Tuple((0.0, 0.0, 1.0), desc='dipole orientation and distance of the inversely phased monopoles')
+
+    prepadding = Enum('loop', desc='Behaviour for negative time indices.')
 
-    prepadding = Enum('loop', desc="Behaviour for negative time indices.")
-    
     # internal identifier
-    digest = Property( 
-        depends_on = ['mics.digest', 'signal.digest', 'loc', \
-         'env.digest', 'start_t', 'start', 'up', 'direction', 'prepadding', '__class__'], 
-        )
-               
+    digest = Property(
+        depends_on=[
+            'mics.digest',
+            'signal.digest',
+            'loc',
+            'env.digest',
+            'start_t',
+            'start',
+            'up',
+            'direction',
+            'prepadding',
+            '__class__',
+        ],
+    )
+
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
-        
-        
+
     def result(self, num=128):
-        """
-        Python generator that yields the output at microphones block-wise.
-                
+        """Python generator that yields the output at microphones block-wise.
+
         Parameters
         ----------
         num : integer, defaults to 128
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block) .
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, numchannels). 
+        Samples in blocks of shape (num, numchannels).
             The last block may be shorter than num.
+
         """
-        #If signal samples are needed for te < t_start, then samples are taken
-        #from the end of the calculated signal.
-        
+        # If signal samples are needed for te < t_start, then samples are taken
+        # from the end of the calculated signal.
+
         mpos = self.mics.mpos
         # position of the dipole as (3,1) vector
-        loc = array(self.loc, dtype = float).reshape((3, 1)) 
+        loc = array(self.loc, dtype=float).reshape((3, 1))
         # direction vector from tuple
-        direc = array(self.direction, dtype = float) * 1e-5
-        direc_mag =  sqrt(dot(direc,direc))
-        
+        direc = array(self.direction, dtype=float) * 1e-5
+        direc_mag = sqrt(dot(direc, direc))
+
         # normed direction vector
         direc_n = direc / direc_mag
-        
+
         c = self.env.c
-        
+
         # distance between monopoles as function of c, sample freq, direction vector
         dist = c / self.sample_freq * direc_mag
-        
+
         # vector from dipole center to one of the monopoles
         dir2 = (direc_n * dist / 2.0).reshape((3, 1))
-        
+
         signal = self.signal.usignal(self.up)
         out = empty((num, self.numchannels))
-        
+
         # distance from dipole center to microphones
         rm = self.env._r(loc, mpos)
-        
+
         # distances from monopoles to microphones
         rm1 = self.env._r(loc + dir2, mpos)
         rm2 = self.env._r(loc - dir2, mpos)
-        
+
         # emission time relative to start_t (in samples) for first sample
-        ind1 = (-rm1 / c - self.start_t + self.start) * self.sample_freq   
+        ind1 = (-rm1 / c - self.start_t + self.start) * self.sample_freq
         ind2 = (-rm2 / c - self.start_t + self.start) * self.sample_freq
-        
+
         i = 0
-        n = self.numsamples        
+        n = self.numsamples
         while n:
             n -= 1
             try:
                 # subtract the second signal b/c of phase inversion
-                out[i] = rm / dist * \
-                         (signal[array(0.5 + ind1 * self.up, dtype=int64)] / rm1 - \
-                          signal[array(0.5 + ind2 * self.up, dtype=int64)] / rm2)
-                ind1 += 1.
-                ind2 += 1.
-                
+                out[i] = (
+                    rm
+                    / dist
+                    * (
+                        signal[array(0.5 + ind1 * self.up, dtype=int64)] / rm1
+                        - signal[array(0.5 + ind2 * self.up, dtype=int64)] / rm2
+                    )
+                )
+                ind1 += 1.0
+                ind2 += 1.0
+
                 i += 1
                 if i == num:
                     yield out
                     i = 0
             except IndexError:
                 break
-            
+
         yield out[:i]
 
+
 class MovingPointSourceDipole(PointSourceDipole, MovingPointSource):
-    
     # internal identifier
-    digest = Property( 
-        depends_on = ['mics.digest', 'signal.digest', 'loc', \
-         'env.digest', 'start_t', 'start', 'up', 'direction', '__class__'], 
-        )
-               
+    digest = Property(
+        depends_on=[
+            'mics.digest',
+            'signal.digest',
+            'loc',
+            'env.digest',
+            'start_t',
+            'start',
+            'up',
+            'direction',
+            '__class__',
+        ],
+    )
+
     #: Reference vector, perpendicular to the x and y-axis of moving source.
     #: rotation source directivity around this axis
-    rvec = CArray( dtype=float, shape=(3, ), value=array((0, 0, 0)), 
-        desc="reference vector")
-    
+    rvec = CArray(dtype=float, shape=(3,), value=array((0, 0, 0)), desc='reference vector')
+
     @cached_property
-    def _get_digest( self ):
-        return digest(self)    
+    def _get_digest(self):
+        return digest(self)
 
-    def get_emission_time(self,t,direction):
+    def get_emission_time(self, t, direction):
         eps = ones(self.mics.num_mics)
-        epslim = 0.1/self.up/self.sample_freq
-        te = t.copy() # init emission time = receiving time
+        epslim = 0.1 / self.up / self.sample_freq
+        te = t.copy()  # init emission time = receiving time
         j = 0
         # Newton-Rhapson iteration
-        while abs(eps).max()>epslim and j<100:
+        while abs(eps).max() > epslim and j < 100:
             xs = array(self.trajectory.location(te))
             loc = xs.copy()
             loc += direction
-            rm = loc-self.mics.mpos# distance vectors to microphones
-            rm = sqrt((rm*rm).sum(0))# absolute distance
-            loc /= sqrt((loc*loc).sum(0))# distance unit vector
+            rm = loc - self.mics.mpos  # distance vectors to microphones
+            rm = sqrt((rm * rm).sum(0))  # absolute distance
+            loc /= sqrt((loc * loc).sum(0))  # distance unit vector
             der = array(self.trajectory.location(te, der=1))
-            Mr = (der*loc).sum(0)/self.env.c# radial Mach number
-            eps = (te + rm/self.env.c - t)/(1+Mr)# discrepancy in time 
+            Mr = (der * loc).sum(0) / self.env.c  # radial Mach number
+            eps = (te + rm / self.env.c - t) / (1 + Mr)  # discrepancy in time
             te -= eps
-            j += 1 #iteration count
+            j += 1  # iteration count
         return te, rm, Mr, xs
-           
-                
-    def get_moving_direction(self,direction,time=0):
-        """
-        function that yields the moving coordinates along the trajectory  
-        """
 
-        trajg1 = array(self.trajectory.location( time, der=1))[:,0][:,newaxis]
-        rflag = (self.rvec == 0).all() #flag translation vs. rotation
+    def get_moving_direction(self, direction, time=0):
+        """Function that yields the moving coordinates along the trajectory."""
+        trajg1 = array(self.trajectory.location(time, der=1))[:, 0][:, newaxis]
+        rflag = (self.rvec == 0).all()  # flag translation vs. rotation
         if rflag:
-            return direction 
-        else:
-            dx = array(trajg1.T) #direction vector (new x-axis)
-            dy = cross(self.rvec, dx) # new y-axis
-            dz = cross(dx, dy) # new z-axis
-            RM = array((dx, dy, dz)).T # rotation matrix
-            RM /= sqrt((RM*RM).sum(0)) # column normalized
-            newdir = dot(RM, direction)
-            return cross(newdir[:,0].T,self.rvec.T).T
+            return direction
+        dx = array(trajg1.T)  # direction vector (new x-axis)
+        dy = cross(self.rvec, dx)  # new y-axis
+        dz = cross(dx, dy)  # new z-axis
+        RM = array((dx, dy, dz)).T  # rotation matrix
+        RM /= sqrt((RM * RM).sum(0))  # column normalized
+        newdir = dot(RM, direction)
+        return cross(newdir[:, 0].T, self.rvec.T).T
 
     def result(self, num=128):
-        """
-        Python generator that yields the output at microphones block-wise.
-                
+        """Python generator that yields the output at microphones block-wise.
+
         Parameters
         ----------
         num : integer, defaults to 128
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block) .
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, numchannels). 
+        Samples in blocks of shape (num, numchannels).
             The last block may be shorter than num.
+
         """
-        #If signal samples are needed for te < t_start, then samples are taken
-        #from the end of the calculated signal.
+        # If signal samples are needed for te < t_start, then samples are taken
+        # from the end of the calculated signal.
         mpos = self.mics.mpos
-        
+
         # direction vector from tuple
-        direc = array(self.direction, dtype = float) * 1e-5
-        direc_mag =  sqrt(dot(direc,direc))   
+        direc = array(self.direction, dtype=float) * 1e-5
+        direc_mag = sqrt(dot(direc, direc))
         # normed direction vector
         direc_n = direc / direc_mag
         c = self.env.c
         # distance between monopoles as function of c, sample freq, direction vector
         dist = c / self.sample_freq * direc_mag * 2
-        
+
         # vector from dipole center to one of the monopoles
         dir2 = (direc_n * dist / 2.0).reshape((3, 1))
-        
+
         signal = self.signal.usignal(self.up)
         out = empty((num, self.numchannels))
         # shortcuts and intial values
         m = self.mics
-        t = self.start*ones(m.num_mics)
+        t = self.start * ones(m.num_mics)
 
         i = 0
-        n = self.numsamples        
+        n = self.numsamples
         while n:
             n -= 1
-            te, rm, Mr, locs = self.get_emission_time(t,0)                
-            t += 1./self.sample_freq
-            #location of the center
-            loc = array(self.trajectory.location(te), dtype = float)[:,0][:,newaxis] 
-            #distance of the dipoles from the center
-            diff = self.get_moving_direction(dir2,te)
- 
+            te, rm, Mr, locs = self.get_emission_time(t, 0)
+            t += 1.0 / self.sample_freq
+            # location of the center
+            loc = array(self.trajectory.location(te), dtype=float)[:, 0][:, newaxis]
+            # distance of the dipoles from the center
+            diff = self.get_moving_direction(dir2, te)
+
             # distance of sources
-            rm1 = self.env._r(loc + diff, mpos) 
+            rm1 = self.env._r(loc + diff, mpos)
             rm2 = self.env._r(loc - diff, mpos)
-                                   
-            ind = (te-self.start_t+self.start)*self.sample_freq
-            if self.conv_amp: 
-                rm *= (1-Mr)**2
-                rm1 *= (1-Mr)**2 # assume that Mr is the same for both poles
-                rm2 *= (1-Mr)**2
+
+            ind = (te - self.start_t + self.start) * self.sample_freq
+            if self.conv_amp:
+                rm *= (1 - Mr) ** 2
+                rm1 *= (1 - Mr) ** 2  # assume that Mr is the same for both poles
+                rm2 *= (1 - Mr) ** 2
             try:
                 # subtract the second signal b/c of phase inversion
-                out[i] = rm / dist * \
-                         (signal[array(0.5 + ind * self.up, dtype=int64)] / rm1 - \
-                          signal[array(0.5 + ind * self.up, dtype=int64)] / rm2)
+                out[i] = (
+                    rm
+                    / dist
+                    * (
+                        signal[array(0.5 + ind * self.up, dtype=int64)] / rm1
+                        - signal[array(0.5 + ind * self.up, dtype=int64)] / rm2
+                    )
+                )
                 i += 1
                 if i == num:
                     yield out
                     i = 0
             except IndexError:
                 break
-        yield out[:i]        
-
+        yield out[:i]
 
 
-class LineSource( PointSource ):
-    """
-    Class to define a fixed Line source with an arbitrary signal.
+class LineSource(PointSource):
+    """Class to define a fixed Line source with an arbitrary signal.
     This can be used in simulations.
-    
+
     The output is being generated via the :meth:`result` generator.
     """
-    
+
     #: Vector to define the orientation of the line source
-    direction = Tuple((0.0, 0.0, 1.0),
-        desc="Line orientation ")
-    
+    direction = Tuple((0.0, 0.0, 1.0), desc='Line orientation ')
+
     #: Vector to define the length of the line source in m
-    length = Float(1,desc="length of the line source")
-    
+    length = Float(1, desc='length of the line source')
+
     #: number of monopol sources in the line source
     num_sources = Int(1)
-    
+
     #: source strength for every monopole
-    source_strength = CArray(desc="coefficients of the source strength")
-    
+    source_strength = CArray(desc='coefficients of the source strength')
+
     #:coherence
-    coherence = Trait( 'coherent', 'incoherent', 
-        desc="coherence mode")
-       
+    coherence = Trait('coherent', 'incoherent', desc='coherence mode')
+
     # internal identifier
-    digest = Property( 
-        depends_on = ['mics.digest', 'signal.digest', 'loc', \
-         'env.digest', 'start_t', 'start', 'up', 'direction',\
-             'source_strength','coherence','__class__'], 
+    digest = Property(
+        depends_on=[
+            'mics.digest',
+            'signal.digest',
+            'loc',
+            'env.digest',
+            'start_t',
+            'start',
+            'up',
+            'direction',
+            'source_strength',
+            'coherence',
+            '__class__',
+        ],
+    )
 
-        )
-               
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
     def result(self, num=128):
-        """
-        Python generator that yields the output at microphones block-wise.
-                
+        """Python generator that yields the output at microphones block-wise.
+
         Parameters
         ----------
         num : integer, defaults to 128
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block) .
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, numchannels). 
+        Samples in blocks of shape (num, numchannels).
             The last block may be shorter than num.
+
         """
-        #If signal samples are needed for te < t_start, then samples are taken
-        #from the end of the calculated signal.
+        # If signal samples are needed for te < t_start, then samples are taken
+        # from the end of the calculated signal.
 
         mpos = self.mics.mpos
-        
+
         # direction vector from tuple
-        direc = array(self.direction, dtype = float)         
+        direc = array(self.direction, dtype=float)
         # normed direction vector
-        direc_n = direc/norm(direc)
+        direc_n = direc / norm(direc)
         c = self.env.c
-        
-        # distance between monopoles in the line 
-        dist = self.length / self.num_sources 
-        
-        #blocwise output
+
+        # distance between monopoles in the line
+        dist = self.length / self.num_sources
+
+        # blocwise output
         out = zeros((num, self.numchannels))
-        
-        # distance from line start position to microphones   
-        loc = array(self.loc, dtype = float).reshape((3, 1)) 
-        
+
+        # distance from line start position to microphones
+        loc = array(self.loc, dtype=float).reshape((3, 1))
+
         # distances from monopoles in the line to microphones
-        rms = empty(( self.numchannels,self.num_sources))
-        inds = empty((self.numchannels,self.num_sources))
+        rms = empty((self.numchannels, self.num_sources))
+        inds = empty((self.numchannels, self.num_sources))
         signals = empty((self.num_sources, len(self.signal.usignal(self.up))))
-        #for every source - distances
+        # for every source - distances
         for s in range(self.num_sources):
-            rms[:,s] = self.env._r((loc.T+direc_n*dist*s).T, mpos)
-            inds[:,s] = (-rms[:,s]  / c - self.start_t + self.start) * self.sample_freq 
-            #new seed for every source
+            rms[:, s] = self.env._r((loc.T + direc_n * dist * s).T, mpos)
+            inds[:, s] = (-rms[:, s] / c - self.start_t + self.start) * self.sample_freq
+            # new seed for every source
             if self.coherence == 'incoherent':
-                self.signal.seed = s + abs(int(hash(self.digest)//10e12))
+                self.signal.seed = s + abs(int(hash(self.digest) // 10e12))
             self.signal.rms = self.signal.rms * self.source_strength[s]
             signals[s] = self.signal.usignal(self.up)
         i = 0
-        n = self.numsamples        
+        n = self.numsamples
         while n:
             n -= 1
             try:
                 for s in range(self.num_sources):
-                # sum sources
-                    out[i] += (signals[s,array(0.5 + inds[:,s].T * self.up, dtype=int64)] / rms[:,s])
-                
-                inds += 1.
+                    # sum sources
+                    out[i] += signals[s, array(0.5 + inds[:, s].T * self.up, dtype=int64)] / rms[:, s]
+
+                inds += 1.0
                 i += 1
                 if i == num:
                     yield out
                     out = zeros((num, self.numchannels))
                     i = 0
             except IndexError:
                 break
-            
+
         yield out[:i]
-        
-class MovingLineSource(LineSource,MovingPointSource):
-    
+
+
+class MovingLineSource(LineSource, MovingPointSource):
     # internal identifier
-    digest = Property( 
-        depends_on = ['mics.digest', 'signal.digest', 'loc', \
-         'env.digest', 'start_t', 'start', 'up', 'direction', '__class__'], 
-        )
-        
+    digest = Property(
+        depends_on=[
+            'mics.digest',
+            'signal.digest',
+            'loc',
+            'env.digest',
+            'start_t',
+            'start',
+            'up',
+            'direction',
+            '__class__',
+        ],
+    )
 
     #: Reference vector, perpendicular to the x and y-axis of moving source.
     #: rotation source directivity around this axis
-    rvec = CArray( dtype=float, shape=(3, ), value=array((0, 0, 0)), 
-        desc="reference vector")
-    
+    rvec = CArray(dtype=float, shape=(3,), value=array((0, 0, 0)), desc='reference vector')
+
     @cached_property
-    def _get_digest( self ):
-        return digest(self) 
-    
-    def get_moving_direction(self,direction,time=0):
-        """
-        function that yields the moving coordinates along the trajectory  
-        """
-    
-        trajg1 = array(self.trajectory.location( time, der=1))[:,0][:,newaxis]
-        rflag = (self.rvec == 0).all() #flag translation vs. rotation
+    def _get_digest(self):
+        return digest(self)
+
+    def get_moving_direction(self, direction, time=0):
+        """Function that yields the moving coordinates along the trajectory."""
+        trajg1 = array(self.trajectory.location(time, der=1))[:, 0][:, newaxis]
+        rflag = (self.rvec == 0).all()  # flag translation vs. rotation
         if rflag:
-            return direction 
-        else:
-            dx = array(trajg1.T) #direction vector (new x-axis)
-            dy = cross(self.rvec, dx) # new y-axis
-            dz = cross(dx, dy) # new z-axis
-            RM = array((dx, dy, dz)).T # rotation matrix
-            RM /= sqrt((RM*RM).sum(0)) # column normalized
-            newdir = dot(RM, direction)
-            return cross(newdir[:,0].T,self.rvec.T).T
+            return direction
+        dx = array(trajg1.T)  # direction vector (new x-axis)
+        dy = cross(self.rvec, dx)  # new y-axis
+        dz = cross(dx, dy)  # new z-axis
+        RM = array((dx, dy, dz)).T  # rotation matrix
+        RM /= sqrt((RM * RM).sum(0))  # column normalized
+        newdir = dot(RM, direction)
+        return cross(newdir[:, 0].T, self.rvec.T).T
 
-    def get_emission_time(self,t,direction):
+    def get_emission_time(self, t, direction):
         eps = ones(self.mics.num_mics)
-        epslim = 0.1/self.up/self.sample_freq
-        te = t.copy() # init emission time = receiving time
+        epslim = 0.1 / self.up / self.sample_freq
+        te = t.copy()  # init emission time = receiving time
         j = 0
         # Newton-Rhapson iteration
-        while abs(eps).max()>epslim and j<100:
+        while abs(eps).max() > epslim and j < 100:
             xs = array(self.trajectory.location(te))
             loc = xs.copy()
             loc += direction
-            rm = loc-self.mics.mpos# distance vectors to microphones
-            rm = sqrt((rm*rm).sum(0))# absolute distance
-            loc /= sqrt((loc*loc).sum(0))# distance unit vector
+            rm = loc - self.mics.mpos  # distance vectors to microphones
+            rm = sqrt((rm * rm).sum(0))  # absolute distance
+            loc /= sqrt((loc * loc).sum(0))  # distance unit vector
             der = array(self.trajectory.location(te, der=1))
-            Mr = (der*loc).sum(0)/self.env.c# radial Mach number
-            eps = (te + rm/self.env.c - t)/(1+Mr)# discrepancy in time 
+            Mr = (der * loc).sum(0) / self.env.c  # radial Mach number
+            eps = (te + rm / self.env.c - t) / (1 + Mr)  # discrepancy in time
             te -= eps
-            j += 1 #iteration count
+            j += 1  # iteration count
         return te, rm, Mr, xs
-        
+
     def result(self, num=128):
-        """
-        Python generator that yields the output at microphones block-wise.
-                
+        """Python generator that yields the output at microphones block-wise.
+
         Parameters
         ----------
         num : integer, defaults to 128
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block) .
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, numchannels). 
+        Samples in blocks of shape (num, numchannels).
             The last block may be shorter than num.
+
         """
-        
-        #If signal samples are needed for te < t_start, then samples are taken
-        #from the end of the calculated signal.
+        # If signal samples are needed for te < t_start, then samples are taken
+        # from the end of the calculated signal.
         mpos = self.mics.mpos
-        
+
         # direction vector from tuple
-        direc = array(self.direction, dtype = float)         
+        direc = array(self.direction, dtype=float)
         # normed direction vector
-        direc_n = direc/norm(direc)
-        
-        # distance between monopoles in the line 
-        dist = self.length / self.num_sources 
+        direc_n = direc / norm(direc)
+
+        # distance between monopoles in the line
+        dist = self.length / self.num_sources
         dir2 = (direc_n * dist).reshape((3, 1))
-        
-        #blocwise output
+
+        # blocwise output
         out = zeros((num, self.numchannels))
-        
+
         # distances from monopoles in the line to microphones
-        rms = empty(( self.numchannels,self.num_sources))
-        inds = empty((self.numchannels,self.num_sources))
+        rms = empty((self.numchannels, self.num_sources))
+        inds = empty((self.numchannels, self.num_sources))
         signals = empty((self.num_sources, len(self.signal.usignal(self.up))))
-        #coherence
+        # coherence
         for s in range(self.num_sources):
-            #new seed for every source
+            # new seed for every source
             if self.coherence == 'incoherent':
-                self.signal.seed = s + abs(int(hash(self.digest)//10e12))
+                self.signal.seed = s + abs(int(hash(self.digest) // 10e12))
             self.signal.rms = self.signal.rms * self.source_strength[s]
             signals[s] = self.signal.usignal(self.up)
         mpos = self.mics.mpos
-    
+
         # shortcuts and intial values
         m = self.mics
-        t = self.start*ones(m.num_mics)
+        t = self.start * ones(m.num_mics)
         i = 0
-        n = self.numsamples        
+        n = self.numsamples
         while n:
-            n -= 1                         
-            t += 1./self.sample_freq
-            te1, rm1, Mr1, locs1 = self.get_emission_time(t,0)         
-            #trajg1 = array(self.trajectory.location( te1, der=1))[:,0][:,newaxis]
-            
+            n -= 1
+            t += 1.0 / self.sample_freq
+            te1, rm1, Mr1, locs1 = self.get_emission_time(t, 0)
+            # trajg1 = array(self.trajectory.location( te1, der=1))[:,0][:,newaxis]
+
             # get distance and ind for every source in the line
             for s in range(self.num_sources):
-                diff = self.get_moving_direction(dir2,te1)
-                te, rm, Mr, locs = self.get_emission_time(t,tile((diff*s).T,(self.numchannels,1)).T)
-                loc = array(self.trajectory.location(te), dtype = float)[:,0][:,newaxis] 
-                diff = self.get_moving_direction(dir2,te)
-                rms[:,s] = self.env._r((loc+diff*s), mpos)
-                inds[:,s] = (te-self.start_t+self.start)*self.sample_freq      
-            
-            if self.conv_amp: 
-                rm *= (1-Mr)**2
-                rms[:,s] *= (1-Mr)**2 # assume that Mr is the same 
+                diff = self.get_moving_direction(dir2, te1)
+                te, rm, Mr, locs = self.get_emission_time(t, tile((diff * s).T, (self.numchannels, 1)).T)
+                loc = array(self.trajectory.location(te), dtype=float)[:, 0][:, newaxis]
+                diff = self.get_moving_direction(dir2, te)
+                rms[:, s] = self.env._r((loc + diff * s), mpos)
+                inds[:, s] = (te - self.start_t + self.start) * self.sample_freq
+
+            if self.conv_amp:
+                rm *= (1 - Mr) ** 2
+                rms[:, s] *= (1 - Mr) ** 2  # assume that Mr is the same
             try:
                 # subtract the second signal b/c of phase inversion
                 for s in range(self.num_sources):
-                # sum sources
-                    out[i] += (signals[s,array(0.5 + inds[:,s].T * self.up, dtype=int64)] / rms[:,s])
-                                    
+                    # sum sources
+                    out[i] += signals[s, array(0.5 + inds[:, s].T * self.up, dtype=int64)] / rms[:, s]
+
                 i += 1
                 if i == num:
                     yield out
                     out = zeros((num, self.numchannels))
                     i = 0
             except IndexError:
                 break
         yield out[:i]
 
 
-class UncorrelatedNoiseSource( SamplesGenerator ):
-    """
-    Class to simulate white or pink noise as uncorrelated signal at each
+class UncorrelatedNoiseSource(SamplesGenerator):
+    """Class to simulate white or pink noise as uncorrelated signal at each
     channel.
-    
+
     The output is being generated via the :meth:`result` generator.
     """
-    
-    #: Type of noise to generate at the channels. 
-    #: The `~acoular.signals.SignalGenerator`-derived class has to 
+
+    #: Type of noise to generate at the channels.
+    #: The `~acoular.signals.SignalGenerator`-derived class has to
     # feature the parameter "seed" (i.e. white or pink noise).
-    signal = Trait(SignalGenerator,
-                   desc = "type of noise")
+    signal = Trait(SignalGenerator, desc='type of noise')
 
     #: Array with seeds for random number generator.
-    #: When left empty, arange(:attr:`numchannels`) + :attr:`signal`.seed  
+    #: When left empty, arange(:attr:`numchannels`) + :attr:`signal`.seed
     #: will be used.
-    seed = CArray(dtype = uint32,
-                  desc = "random seed values")
-    
-    #: Number of channels in output; is set automatically / 
+    seed = CArray(dtype=uint32, desc='random seed values')
+
+    #: Number of channels in output; is set automatically /
     #: depends on used microphone geometry.
     numchannels = Delegate('mics', 'num_mics')
 
     #: :class:`~acoular.microphones.MicGeom` object that provides the microphone locations.
-    mics = Trait(MicGeom, 
-        desc="microphone geometry")
+    mics = Trait(MicGeom, desc='microphone geometry')
 
     # --- List of backwards compatibility traits and their setters/getters -----------
 
     # Microphone locations.
     # Deprecated! Use :attr:`mics` trait instead.
     mpos = Property()
-    
+
     def _get_mpos(self):
         return self.mics
-    
+
     def _set_mpos(self, mpos):
-        warn("Deprecated use of 'mpos' trait. ", Warning, stacklevel = 2)
+        warn("Deprecated use of 'mpos' trait. ", Warning, stacklevel=2)
         self.mics = mpos
 
     # --- End of backwards compatibility traits --------------------------------------
-        
+
     #: Start time of the signal in seconds, defaults to 0 s.
-    start_t = Float(0.0,
-        desc="signal start time")
-    
-    #: Start time of the data aquisition at microphones in seconds, 
+    start_t = Float(0.0, desc='signal start time')
+
+    #: Start time of the data aquisition at microphones in seconds,
     #: defaults to 0 s.
-    start = Float(0.0,
-        desc="sample start time")
+    start = Float(0.0, desc='sample start time')
 
-    
-    #: Number of samples is set automatically / 
+    #: Number of samples is set automatically /
     #: depends on :attr:`signal`.
     numsamples = Delegate('signal')
-    
-    #: Sampling frequency of the signal; is set automatically / 
+
+    #: Sampling frequency of the signal; is set automatically /
     #: depends on :attr:`signal`.
-    sample_freq = Delegate('signal') 
-    
+    sample_freq = Delegate('signal')
+
     # internal identifier
-    digest = Property( 
-        depends_on = ['mics.digest', 'signal.rms', 'signal.numsamples', \
-        'signal.sample_freq', 'signal.__class__' , 'seed', 'loc', \
-         'start_t', 'start', '__class__'], 
-        )
+    digest = Property(
+        depends_on=[
+            'mics.digest',
+            'signal.rms',
+            'signal.numsamples',
+            'signal.sample_freq',
+            'signal.__class__',
+            'seed',
+            'loc',
+            'start_t',
+            'start',
+            '__class__',
+        ],
+    )
 
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
-    
-    def result ( self, num=128 ):
-        """
-        Python generator that yields the output at microphones block-wise.
-                
+
+    def result(self, num=128):
+        """Python generator that yields the output at microphones block-wise.
+
         Parameters
         ----------
         num : integer, defaults to 128
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block) .
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, numchannels). 
+        Samples in blocks of shape (num, numchannels).
             The last block may be shorter than num.
-        """
 
+        """
         Noise = self.signal.__class__
         # create or get the array of random seeds
-        if not self.seed:            
+        if not self.seed:
             seed = arange(self.numchannels) + self.signal.seed
         elif self.seed.shape == (self.numchannels,):
             seed = self.seed
         else:
-            raise ValueError(\
-               "Seed array expected to be of shape (%i,), but has shape %s." \
-                % (self.numchannels, str(self.seed.shape)) )
-        
+            raise ValueError(
+                'Seed array expected to be of shape (%i,), but has shape %s.'
+                % (self.numchannels, str(self.seed.shape)),
+            )
+
         # create array with [numchannels] noise signal tracks
-        signal = array([Noise(seed = s, 
-                              numsamples = self.numsamples,
-                              sample_freq = self.sample_freq,
-                              rms = self.signal.rms).signal() \
-                        for s in seed]).T
+        signal = array(
+            [
+                Noise(seed=s, numsamples=self.numsamples, sample_freq=self.sample_freq, rms=self.signal.rms).signal()
+                for s in seed
+            ],
+        ).T
 
-        n = num        
+        n = num
         while n <= self.numsamples:
-            yield signal[n-num:n,:]
+            yield signal[n - num : n, :]
             n += num
         else:
-            if (n-num) < self.numsamples:
-                yield signal[n-num:,:]
+            if (n - num) < self.numsamples:
+                yield signal[n - num :, :]
             else:
                 return
 
 
-
-class SourceMixer( SamplesGenerator ):
-    """
-    Mixes the signals from several sources. 
-    """
+class SourceMixer(SamplesGenerator):
+    """Mixes the signals from several sources."""
 
     #: List of :class:`~acoular.tprocess.SamplesGenerator` objects
     #: to be mixed.
-    sources = List( Instance(SamplesGenerator, ()) ) 
+    sources = List(Instance(SamplesGenerator, ()))
 
     #: Sampling frequency of the signal.
-    sample_freq = Property( depends_on=['sdigest'] )
-    
+    sample_freq = Property(depends_on=['sdigest'])
+
     #: Number of channels.
-    numchannels = Property( depends_on=['sdigest'] )
-               
+    numchannels = Property(depends_on=['sdigest'])
+
     #: Number of samples.
-    numsamples = Property( depends_on=['sdigest'] )
-    
-    #: Amplitude weight(s) for the sources as array. If not set, 
+    numsamples = Property(depends_on=['sdigest'])
+
+    #: Amplitude weight(s) for the sources as array. If not set,
     #: all source signals are equally weighted.
     #: Must match the number of sources in :attr:`sources`.
-    weights = CArray(desc="channel weights")
+    weights = CArray(desc='channel weights')
 
-    # internal identifier    
+    # internal identifier
     sdigest = Str()
 
     @observe('sources.items.digest')
-    def _set_sources_digest( self, event ):
-        self.sdigest = ldigest(self.sources) 
+    def _set_sources_digest(self, event):  # noqa ARG002
+        self.sdigest = ldigest(self.sources)
 
     # internal identifier
-    digest = Property( depends_on = ['sdigest', 'weights'])
+    digest = Property(depends_on=['sdigest', 'weights'])
 
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
     @cached_property
-    def _get_sample_freq( self ):
-        if self.sources:
-            sample_freq = self.sources[0].sample_freq
-        else:
-            sample_freq = 0
-        return sample_freq
+    def _get_sample_freq(self):
+        return self.sources[0].sample_freq if self.sources else 0
 
     @cached_property
-    def _get_numchannels( self ):
-        if self.sources:
-            numchannels = self.sources[0].numchannels
-        else:
-            numchannels = 0
-        return numchannels
+    def _get_numchannels(self):
+        return self.sources[0].numchannels if self.sources else 0
 
     @cached_property
-    def _get_numsamples( self ):
-        if self.sources:
-            numsamples = self.sources[0].numsamples
-        else:
-            numsamples = 0
-        return numsamples
+    def _get_numsamples(self):
+        return self.sources[0].numsamples if self.sources else 0
 
-    def validate_sources( self ):
-        """ Validates if sources fit together. """
+    def validate_sources(self):
+        """Validates if sources fit together."""
         if len(self.sources) < 1:
-            raise ValueError("Number of sources in SourceMixer should be at least 1.")
+            msg = 'Number of sources in SourceMixer should be at least 1.'
+            raise ValueError(msg)
         for s in self.sources[1:]:
             if self.sample_freq != s.sample_freq:
-                raise ValueError("Sample frequency of %s does not fit" % s)
+                raise ValueError('Sample frequency of %s does not fit' % s)
             if self.numchannels != s.numchannels:
-                raise ValueError("Channel count of %s does not fit" % s)
+                raise ValueError('Channel count of %s does not fit' % s)
             if self.numsamples != s.numsamples:
-                raise ValueError("Number of samples of %s does not fit" % s)
+                raise ValueError('Number of samples of %s does not fit' % s)
 
     def result(self, num):
-        """
-        Python generator that yields the output block-wise.
+        """Python generator that yields the output block-wise.
         The outputs from the sources in the list are being added.
-        
+
         Parameters
         ----------
         num : integer
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block).
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, numchannels). 
+        Samples in blocks of shape (num, numchannels).
             The last block may be shorter than num.
+
         """
         # check whether all sources fit together
         self.validate_sources()
 
         gens = [i.result(num) for i in self.sources[1:]]
         weights = self.weights.copy()
         if weights.size == 0:
-            weights = array([1. for j in range(len( self.sources))])
+            weights = array([1.0 for j in range(len(self.sources))])
         assert weights.shape[0] == len(self.sources)
         for temp in self.sources[0].result(num):
             temp *= weights[0]
             sh = temp.shape[0]
-            for j,g in enumerate(gens):
-                temp1 = next(g)*weights[j+1]
+            for j, g in enumerate(gens):
+                temp1 = next(g) * weights[j + 1]
                 if temp.shape[0] > temp1.shape[0]:
-                    temp = temp[:temp1.shape[0]]
-                temp += temp1[:temp.shape[0]]
+                    temp = temp[: temp1.shape[0]]
+                temp += temp1[: temp.shape[0]]
             yield temp
             if sh > temp.shape[0]:
                 break
 
 
-class PointSourceConvolve( PointSource ):
-    """
-    Class to blockwise convolve an arbitrary source signal with a spatial room impulse response
-    """
+class PointSourceConvolve(PointSource):
+    """Class to blockwise convolve an arbitrary source signal with a spatial room impulse response."""
 
     #: Convolution kernel in the time domain.
     #: The second dimension of the kernel array has to be either 1 or match :attr:`~SamplesGenerator.numchannels`.
     #: If only a single kernel is supplied, it is applied to all channels.
-    kernel = CArray(dtype=float, desc="Convolution kernel.")
+    kernel = CArray(dtype=float, desc='Convolution kernel.')
 
     # ------------- overwrite traits that are not supported by this class -------------
-    
+
     #: Start time of the signal in seconds, defaults to 0 s.
-    start_t = Enum(0.0,
-        desc="signal start time")
-    
-    #: Start time of the data aquisition at microphones in seconds, 
+    start_t = Enum(0.0, desc='signal start time')
+
+    #: Start time of the data aquisition at microphones in seconds,
     #: defaults to 0 s.
-    start = Enum(0.0,
-        desc="sample start time")
+    start = Enum(0.0, desc='sample start time')
 
     #: Signal behaviour for negative time indices, i.e. if :attr:`start` < :attr:start_t.
     #: `loop` take values from the end of :attr:`signal.signal()` array.
     #: `zeros` set source signal to zero, advisable for deterministic signals.
     #: defaults to `loop`.
-    prepadding = Enum(None, desc="Behaviour for negative time indices.")
+    prepadding = Enum(None, desc='Behaviour for negative time indices.')
 
     #: Upsampling factor, internal use, defaults to 16.
-    up = Enum(None, desc="upsampling factor") 
-            
+    up = Enum(None, desc='upsampling factor')
+
     # internal identifier
-    digest = Property( 
-        depends_on = ['mics.digest', 'signal.digest', 'loc', 'kernel', '__class__'], 
-        )
-               
+    digest = Property(
+        depends_on=['mics.digest', 'signal.digest', 'loc', 'kernel', '__class__'],
+    )
+
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
     def result(self, num=128):
-        """
-        Python generator that yields the output at microphones block-wise.
+        """Python generator that yields the output at microphones block-wise.
 
         Parameters
         ----------
         num : integer, defaults to 128
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block) .
 
         Returns
         -------
-        Samples in blocks of shape (num, numchannels). 
+        Samples in blocks of shape (num, numchannels).
             The last block may be shorter than num.
+
         """
-        data = repeat(
-            self.signal.signal()[:,newaxis],self.mics.num_mics,axis=1)
+        data = repeat(self.signal.signal()[:, newaxis], self.mics.num_mics, axis=1)
         source = TimeSamples(
             data=data,
             sample_freq=self.sample_freq,
             numsamples=self.numsamples,
             numchannels=self.mics.num_mics,
         )
         time_convolve = TimeConvolve(
-            source = source,
-            kernel = self.kernel,
+            source=source,
+            kernel=self.kernel,
         )
-        for block in time_convolve.result(num):
-            yield block
+        yield from time_convolve.result(num)
```

### Comparing `acoular-24.3/acoular/spectra.py` & `acoular-24.5/acoular/tbeamform.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,778 +1,813 @@
-# -*- coding: utf-8 -*-
-#pylint: disable-msg=E0611, E1101, E1103, C0103, R0901, R0902, R0903, R0904
-#pylint: disable-msg=W0232
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 # Copyright (c) Acoular Development Team.
-#------------------------------------------------------------------------------
-"""Estimation of power spectra and related tools
+# ------------------------------------------------------------------------------
+"""Implements beamformers in the time domain.
 
 .. autosummary::
     :toctree: generated/
 
-    BaseSpectra
-    FFTSpectra    
-    PowerSpectra
-    synthetic
-    PowerSpectraImport
+    BeamformerTime
+    BeamformerTimeTraj
+    BeamformerTimeSq
+    BeamformerTimeSqTraj
+    BeamformerCleant
+    BeamformerCleantTraj
+    BeamformerCleantSq
+    BeamformerCleantSqTraj
+    IntegratorSectorTime
 """
+
+# imports from other packages
 from warnings import warn
 
-from numpy import array, ones, hanning, hamming, bartlett, blackman, \
-dot, newaxis, zeros, empty, linalg, sqrt,real, imag,\
-searchsorted, isscalar, fill_diagonal, arange, zeros_like, sum, ndarray
-from scipy import fft
-from traits.api import HasPrivateTraits, Int, Property, Instance, Trait, \
-Bool, cached_property, property_depends_on, Delegate, Float, Enum, \
-    CArray
-
-from .fastFuncs import calcCSM
-from .h5cache import H5cache
-from .h5files import H5CacheFileBase
+from numpy import (
+    arange,
+    argmax,
+    array,
+    ceil,
+    concatenate,
+    dot,
+    empty,
+    float32,
+    float64,
+    histogram,
+    int32,
+    int64,
+    interp,
+    isscalar,
+    newaxis,
+    r_,
+    s_,
+    sqrt,
+    sum,
+    unique,
+    where,
+    zeros,
+)
+from numpy.linalg import norm
+from traits.api import Bool, CArray, Delegate, Enum, Float, Instance, Int, List, Property, Range, Trait, cached_property
+from traits.trait_errors import TraitError
+
+from .fbeamform import SteeringVector
+from .grids import RectGrid
+
+# acoular imports
 from .internal import digest
-from .tprocess import SamplesGenerator, TimeInOut
-from .calib import Calib
-from .configuration import config
-
-
-class BaseSpectra( HasPrivateTraits ):
-
-    #: Data source; :class:`~acoular.sources.SamplesGenerator` or derived object.
-    source = Trait(SamplesGenerator)
-
-    #: Sampling frequency of output signal, as given by :attr:`source`.
-    sample_freq = Delegate('source')
-
-    #: Number of time data channels 
-    numchannels = Delegate('source')
-
-    #: Window function for FFT, one of:
-    #:   * 'Rectangular' (default)
-    #:   * 'Hanning'
-    #:   * 'Hamming'
-    #:   * 'Bartlett'
-    #:   * 'Blackman'
-    window = Trait('Rectangular', 
-        {'Rectangular':ones, 
-        'Hanning':hanning, 
-        'Hamming':hamming, 
-        'Bartlett':bartlett, 
-        'Blackman':blackman}, 
-        desc="type of window for FFT")
-
-    #: Overlap factor for averaging: 'None'(default), '50%', '75%', '87.5%'.
-    overlap = Trait('None', {'None':1, '50%':2, '75%':4, '87.5%':8}, 
-        desc="overlap of FFT blocks")
-    
-    #: FFT block size, one of: 128, 256, 512, 1024, 2048 ... 65536,
-    #: defaults to 1024.
-    block_size = Trait(1024, 128, 256, 512, 1024, 2048, 4096, 8192, 16384, 32768, 65536,
-        desc="number of samples per FFT block")
-
-    #: The floating-number-precision of entries of csm, eigenvalues and 
-    #: eigenvectors, corresponding to numpy dtypes. Default is 64 bit.
-    precision = Trait('complex128', 'complex64', 
-                      desc="precision of the fft")
-    
-    # internal identifier
-    digest = Property( depends_on = ['precision','block_size',
-                                    'window','overlap'])
+from .tfastfuncs import _delayandsum4, _delayandsum5, _delays, _steer_I, _steer_II, _steer_III, _steer_IV
+from .tprocess import TimeInOut
+from .trajectory import Trajectory
 
-    @cached_property
-    def _get_digest( self ):
-        return digest(self)
 
-    def fftfreq ( self ):
-        """
-        Return the Discrete Fourier Transform sample frequencies.
-        
-        Returns
-        -------
-        f : ndarray
-            Array of length *block_size/2+1* containing the sample frequencies.
-        """
-        if self.source is not None:
-            return abs(fft.fftfreq(self.block_size, 1./self.source.sample_freq)\
-                        [:int(self.block_size/2+1)])
-        else:
-            return None
+def const_power_weight(bf):
+    """Internal helper function for :class:`BeamformerTime`.
 
-    #generator that yields the time data blocks for every channel (with optional overlap)
-    def get_source_data(self):
-        bs = self.block_size
-        temp = empty((2*bs, self.numchannels))
-        pos = bs
-        posinc = bs/self.overlap_
-        for data_block in self.source.result(bs):
-            ns = data_block.shape[0]
-            temp[bs:bs+ns] = data_block # fill from right
-            while pos+bs <= bs+ns:
-                yield temp[int(pos):int(pos+bs)]
-                pos += posinc
-            else:
-                temp[0:bs] = temp[bs:] # copy to left
-                pos -= bs
+    Provides microphone weighting
+    to make the power per unit area of the
+    microphone array geometry constant.
+
+    Parameters
+    ----------
+    bf: :class:`BeamformerTime` object
 
 
-class FFTSpectra( BaseSpectra,TimeInOut ):
-    """Provides the spectra of multichannel time data. 
-    
-    Returns Spectra per block over a Generator.       
+    Returns
+    -------
+    array of floats
+        The weight factors.
+
     """
-    
+    r = bf.steer.env._r(zeros((3, 1)), bf.steer.mics.mpos)  # distances to center
+    # round the relative distances to one decimal place
+    r = (r / r.max()).round(decimals=1)
+    ru, ind = unique(r, return_inverse=True)
+    ru = (ru[1:] + ru[:-1]) / 2
+    count, bins = histogram(r, r_[0, ru, 1.5 * r.max() - 0.5 * ru[-1]])
+    bins *= bins
+    weights = sqrt((bins[1:] - bins[:-1]) / count)
+    weights /= weights.mean()
+    return weights[ind]
+
+
+# possible choices for spatial weights
+possible_weights = {'none': None, 'power': const_power_weight}
+
+
+class BeamformerTime(TimeInOut):
+    """Provides a basic time domain beamformer with time signal output
+    for a spatially fixed grid.
+    """
+
+    # Instance of :class:`~acoular.fbeamform.SteeringVector` or its derived classes
+    # that contains information about the steering vector. This is a private trait.
+    # Do not set this directly, use `steer` trait instead.
+    _steer_obj = Instance(SteeringVector(), SteeringVector)
+
+    #: :class:`~acoular.fbeamform.SteeringVector` or derived object.
+    #: Defaults to :class:`~acoular.fbeamform.SteeringVector` object.
+    steer = Property(desc='steering vector object')
+
+    def _get_steer(self):
+        return self._steer_obj
+
+    def _set_steer(self, steer):
+        if type(steer) == SteeringVector:
+            # This condition may be replaced at a later time by: isinstance(steer, SteeringVector): -- (derived classes allowed)
+            self._steer_obj = steer
+        elif steer in ('true level', 'true location', 'classic', 'inverse'):
+            # Type of steering vectors, see also :ref:`Sarradj, 2012<Sarradj2012>`.
+            warn(
+                "Deprecated use of 'steer' trait. Please use object of class 'SteeringVector' in the future.",
+                Warning,
+                stacklevel=2,
+            )
+            self._steer_obj.steer_type = steer
+        else:
+            raise (TraitError(args=self, name='steer', info='SteeringVector', value=steer))
+
+    # --- List of backwards compatibility traits and their setters/getters -----------
+
+    # :class:`~acoular.environments.Environment` or derived object.
+    # Deprecated! Only kept for backwards compatibility.
+    # Now governed by :attr:`steer` trait.
+    env = Property()
+
+    def _get_env(self):
+        return self._steer_obj.env
+
+    def _set_env(self, env):
+        warn("Deprecated use of 'env' trait. ", Warning, stacklevel=2)
+        self._steer_obj.env = env
+
+    # The speed of sound.
+    # Deprecated! Only kept for backwards compatibility.
+    # Now governed by :attr:`steer` trait.
+    c = Property()
+
+    def _get_c(self):
+        return self._steer_obj.env.c
+
+    def _set_c(self, c):
+        warn("Deprecated use of 'c' trait. ", Warning, stacklevel=2)
+        self._steer_obj.env.c = c
+
+    # :class:`~acoular.grids.Grid`-derived object that provides the grid locations.
+    # Deprecated! Only kept for backwards compatibility.
+    # Now governed by :attr:`steer` trait.
+    grid = Property()
+
+    def _get_grid(self):
+        return self._steer_obj.grid
+
+    def _set_grid(self, grid):
+        warn("Deprecated use of 'grid' trait. ", Warning, stacklevel=2)
+        self._steer_obj.grid = grid
+
+    # :class:`~acoular.microphones.MicGeom` object that provides the microphone locations.
+    # Deprecated! Only kept for backwards compatibility.
+    # Now governed by :attr:`steer` trait
+    mpos = Property()
+
+    def _get_mpos(self):
+        return self._steer_obj.mics
+
+    def _set_mpos(self, mpos):
+        warn("Deprecated use of 'mpos' trait. ", Warning, stacklevel=2)
+        self._steer_obj.mics = mpos
+
+    # Sound travel distances from microphone array center to grid points (r0)
+    # and all array mics to grid points (rm). Readonly.
+    # Deprecated! Only kept for backwards compatibility.
+    # Now governed by :attr:`steer` trait
+    r0 = Property()
+
+    def _get_r0(self):
+        return self._steer_obj.r0
+
+    rm = Property()
+
+    def _get_rm(self):
+        return self._steer_obj.rm
+
+    # --- End of backwards compatibility traits --------------------------------------
+
+    #: Number of channels in output (=number of grid points).
+    numchannels = Delegate('grid', 'size')
+
+    #: Spatial weighting function.
+    weights = Trait('none', possible_weights, desc='spatial weighting function')
+    # (from timedomain.possible_weights)
+
+    # buffer with microphone time signals used for processing. Internal use
+    buffer = CArray(desc='buffer containing microphone signals')
+
+    # index indicating position of current processing sample. Internal use.
+    bufferIndex = Int(desc='index indicating position in buffer')
+
     # internal identifier
-    digest = Property( depends_on = ['source.digest','precision','block_size',
-                                    'window','overlap'])
+    digest = Property(
+        depends_on=['_steer_obj.digest', 'source.digest', 'weights', '__class__'],
+    )
 
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
-    #generator that yields the fft for every channel
-    def result(self):
-        """ 
-        Python generator that yields the output block-wise.
-        
+    def _get_weights(self):
+        return self.weights_(self)[newaxis] if self.weights_ else 1.0
+
+    def _fill_buffer(self, num):
+        """Generator that fills the signal buffer."""
+        weights = self._get_weights()
+        for block in self.source.result(num):
+            block *= weights
+            ns = block.shape[0]
+            bufferSize = self.buffer.shape[0]
+            self.buffer[0 : (bufferSize - ns)] = self.buffer[-(bufferSize - ns) :]
+            self.buffer[-ns:, :] = block
+            self.bufferIndex -= ns
+            yield
+
+    def result(self, num=2048):
+        """Python generator that yields the *squared* deconvolved beamformer
+        output with optional removal of autocorrelation block-wise.
+
         Parameters
         ----------
-        num : integer
+        num : integer, defaults to 2048
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block).
-        
+
         Returns
         -------
-        Samples in blocks of shape (numfreq, :attr:`numchannels`). 
-            The last block may be shorter than num.
-            """
-        wind = self.window_( self.block_size )
-        weight=sqrt(2)/self.block_size*sqrt(self.block_size/dot(wind,wind))*wind[:, newaxis]
-        for data in self.get_source_data():
-            ft = fft.rfft(data*weight, None, 0).astype(self.precision)
-            yield ft
-
-
-class PowerSpectra( BaseSpectra ):
-    """Provides the cross spectral matrix of multichannel time data
-     and its eigen-decomposition.
-    
-    This class includes the efficient calculation of the full cross spectral
-    matrix using the Welch method with windows and overlap. It also contains 
-    the CSM's eigenvalues and eigenvectors and additional properties. 
-    
-    The result is computed only when needed, that is when the :attr:`csm`,
-    :attr:`eva`, or :attr:`eve` attributes are acturally read.
-    Any change in the input data or parameters leads to a new calculation, 
-    again triggered when an attribute is read. The result may be 
-    cached on disk in HDF5 files and need not to be recomputed during
-    subsequent program runs with identical input data and parameters. The
-    input data is taken to be identical if the source has identical parameters
-    and the same file name in case of that the data is read from a file.
+        Samples in blocks of shape  \
+        (num, :attr:`~BeamformerTime.numchannels`).
+            :attr:`~BeamformerTime.numchannels` is usually very \
+            large (number of grid points).
+            The last block may be shorter than num. \
+            The output starts for signals that were emitted
+            from the grid at `t=0`.
+
+        """
+        # initialize values
+        fdtype = float64
+        idtype = int64
+        numMics = self.steer.mics.num_mics
+        n_index = arange(0, num + 1)[:, newaxis]
+        c = self.steer.env.c / self.source.sample_freq
+        amp = empty((1, self.grid.size, numMics), dtype=fdtype)
+        # delays = empty((1,self.grid.size,numMics),dtype=fdtype)
+        d_index = empty((1, self.grid.size, numMics), dtype=idtype)
+        d_interp2 = empty((1, self.grid.size, numMics), dtype=fdtype)
+        _steer_III(self.rm[newaxis, :, :], self.r0[newaxis, :], amp)
+        _delays(self.rm[newaxis, :, :], c, d_interp2, d_index)
+        amp.shape = amp.shape[1:]
+        # delays.shape = delays.shape[1:]
+        d_index.shape = d_index.shape[1:]
+        d_interp2.shape = d_interp2.shape[1:]
+        maxdelay = int((self.rm / c).max()) + 2 + num  # +2 because of interpolation
+        initialNumberOfBlocks = int(ceil(maxdelay / num))
+        bufferSize = initialNumberOfBlocks * num
+        self.buffer = zeros((bufferSize, numMics), dtype=float)
+        self.bufferIndex = bufferSize  # indexing current time sample in buffer
+        fill_buffer_generator = self._fill_buffer(num)
+        for _ in range(initialNumberOfBlocks):
+            next(fill_buffer_generator)
+
+        # start processing
+        flag = True
+        while flag:
+            samplesleft = self.buffer.shape[0] - self.bufferIndex
+            if samplesleft - maxdelay <= 0:
+                num += samplesleft - maxdelay
+                maxdelay += samplesleft - maxdelay
+                n_index = arange(0, num + 1)[:, newaxis]
+                flag = False
+            # init step
+            p_res = array(self.buffer[self.bufferIndex : self.bufferIndex + maxdelay, :])
+            Phi, autopow = self.delay_and_sum(num, p_res, d_interp2, d_index, amp)
+            if 'Cleant' not in self.__class__.__name__:
+                if 'Sq' not in self.__class__.__name__:
+                    yield Phi[:num]
+                elif self.r_diag:
+                    yield (Phi[:num] ** 2 - autopow[:num]).clip(min=0)
+                else:
+                    yield Phi[:num] ** 2
+            else:
+                Gamma = zeros(Phi.shape)
+                Gamma_autopow = zeros(Phi.shape)
+                J = 0
+                # deconvolution
+                while self.n_iter > J:
+                    # print(f"start clean iteration {J+1} of max {self.n_iter}")
+                    powPhi = (Phi[:num] ** 2 - autopow).sum(0).clip(min=0) if self.r_diag else (Phi[:num] ** 2).sum(0)
+                    imax = argmax(powPhi)
+                    t_float = d_interp2[imax] + d_index[imax] + n_index
+                    t_ind = t_float.astype(int64)
+                    for m in range(numMics):
+                        p_res[t_ind[: num + 1, m], m] -= self.damp * interp(
+                            t_ind[: num + 1, m],
+                            t_float[:num, m],
+                            Phi[:num, imax] * self.r0[imax] / self.rm[imax, m],
+                        )
+                    nextPhi, nextAutopow = self.delay_and_sum(num, p_res, d_interp2, d_index, amp)
+                    if self.r_diag:
+                        pownextPhi = (nextPhi[:num] ** 2 - nextAutopow).sum(0).clip(min=0)
+                    else:
+                        pownextPhi = (nextPhi[:num] ** 2).sum(0)
+                    # print(f"total signal power: {powPhi.sum()}")
+                    if pownextPhi.sum() < powPhi.sum():  # stopping criterion
+                        Gamma[:num, imax] += self.damp * Phi[:num, imax]
+                        Gamma_autopow[:num, imax] = autopow[:num, imax].copy()
+                        Phi = nextPhi
+                        autopow = nextAutopow
+                        # print(f"clean max: {L_p((Gamma**2).sum(0)/num).max()} dB")
+                        J += 1
+                    else:
+                        break
+                if 'Sq' not in self.__class__.__name__:
+                    yield Gamma[:num]
+                elif self.r_diag:
+                    yield Gamma[:num] ** 2 - (self.damp**2) * Gamma_autopow[:num]
+                else:
+                    yield Gamma[:num] ** 2
+            self.bufferIndex += num
+            try:
+                next(fill_buffer_generator)
+            except:
+                pass
+
+    def delay_and_sum(self, num, p_res, d_interp2, d_index, amp):
+        """Standard delay-and-sum method."""
+        result = empty((num, self.grid.size), dtype=float)  # output array
+        autopow = empty((num, self.grid.size), dtype=float)  # output array
+        _delayandsum4(p_res, d_index, d_interp2, amp, result, autopow)
+        return result, autopow
+
+
+class BeamformerTimeSq(BeamformerTime):
+    """Provides a time domain beamformer with time-dependend
+    power signal output and possible autopower removal
+    for a spatially fixed grid.
     """
 
-    # Shadow trait, should not be set directly, for internal use.
-    _source = Trait(SamplesGenerator)
-
-    #: Data source; :class:`~acoular.sources.SamplesGenerator` or derived object. 
-    source = Property(_source,
-        desc="time data object")
-
-    #: The :class:`~acoular.tprocess.SamplesGenerator` object that provides the data.
-    time_data = Property(_source, 
-        desc="deprecated attribute holding the time data object. Use PowerSpectra.source instead!")
-
-    #: The :class:`~acoular.calib.Calib` object that provides the calibration data, 
-    #: defaults to no calibration, i.e. the raw time data is used.
-    #:
-    #: **deprecated**:      use :attr:`~acoular.sources.TimeSamples.calib` property of 
-    #: :class:`~acoular.sources.TimeSamples` objects
-    calib = Instance(Calib)
-
-    # Shadow trait, should not be set directly, for internal use.
-    _ind_low = Int(1,
-        desc="index of lowest frequency line")
-
-    # Shadow trait, should not be set directly, for internal use.
-    _ind_high = Trait(-1,(Int,None),
-        desc="index of highest frequency line")
-
-    #: Index of lowest frequency line to compute, integer, defaults to 1,
-    #: is used only by objects that fetch the csm, PowerSpectra computes every
-    #: frequency line.
-    ind_low = Property(_ind_low,
-        desc="index of lowest frequency line")
-
-    #: Index of highest frequency line to compute, integer, 
-    #: defaults to -1 (last possible line for default block_size).
-    ind_high = Property(_ind_high,
-        desc="index of lowest frequency line")
-
-    # Stores the set lower frequency, for internal use, should not be set directly.
-    _freqlc = Float(0)
-
-    # Stores the set higher frequency, for internal use, should not be set directly.
-    _freqhc = Trait(0,(Float,None))
-
-    # Saves whether the user set indices or frequencies last, for internal use only,
-    # not to be set directly, if True (default), indices are used for setting
-    # the freq_range interval.
-    _index_set_last = Bool(True)
-      
-    #: Flag, if true (default), the result is cached in h5 files and need not
-    #: to be recomputed during subsequent program runs.
-    cached = Bool(True, 
-        desc="cached flag")   
-
-    #: Number of FFT blocks to average, readonly
-    #: (set from block_size and overlap).
-    num_blocks = Property(
-        desc="overall number of FFT blocks")
-
-    #: 2-element array with the lowest and highest frequency. If set, 
-    #: will overwrite :attr:`_freqlc` and :attr:`_freqhc` according to
-    #: the range. 
-    #: The freq_range interval will be the smallest discrete frequency
-    #: inside the half-open interval [_freqlc, _freqhc[ and the smallest
-    #: upper frequency outside of the interval.
-    #: If user chooses the higher frequency larger than the max frequency,
-    #: the max frequency will be the upper bound.
-    freq_range = Property(
-        desc = "frequency range" )
-        
-    #: Array with a sequence of indices for all frequencies 
-    #: between :attr:`ind_low` and :attr:`ind_high` within the result, readonly.
-    indices = Property(
-        desc = "index range" )
-        
-    #: Name of the cache file without extension, readonly.
-    basename = Property( depends_on = '_source.digest', 
-        desc="basename for cache file")
-
-    #: The cross spectral matrix, 
-    #: (number of frequencies, numchannels, numchannels) array of complex;
-    #: readonly.
-    csm = Property( 
-        desc="cross spectral matrix")
-    
-    #: Eigenvalues of the cross spectral matrix as an
-    #: (number of frequencies) array of floats, readonly.
-    eva = Property( 
-        desc="eigenvalues of cross spectral matrix")
-
-    #: Eigenvectors of the cross spectral matrix as an
-    #: (number of frequencies, numchannels, numchannels) array of floats,
-    #: readonly.
-    eve = Property( 
-        desc="eigenvectors of cross spectral matrix")
+    #: Boolean flag, if 'True' (default), the main diagonal is removed before beamforming.
+    r_diag = Bool(True, desc='removal of diagonal')
 
     # internal identifier
-    digest = Property( 
-        depends_on = ['_source.digest', 'calib.digest', 'block_size', 
-            'window', 'overlap', 'precision'], 
-        )
-
-    # hdf5 cache file
-    h5f = Instance( H5CacheFileBase, transient = True )
-    
-    @property_depends_on('_source.numsamples, block_size, overlap')
-    def _get_num_blocks ( self ):
-        return self.overlap_*self._source.numsamples/self.block_size-\
-        self.overlap_+1
-
-    @property_depends_on('_source.sample_freq, block_size, ind_low, ind_high')
-    def _get_freq_range ( self ):
-        fftfreq = self.fftfreq()
-        if fftfreq is not None:
-            if self._ind_high is None:
-                return array([fftfreq[self.ind_low],None])
-            else:
-                return fftfreq[[ self.ind_low, self.ind_high ]]
+    digest = Property(
+        depends_on=['_steer_obj.digest', 'source.digest', 'r_diag', 'weights', '__class__'],
+    )
 
-    def _set_freq_range( self, freq_range ):# by setting this the user sets _freqlc and _freqhc
-        self._index_set_last = False
-        self._freqlc = freq_range[0]
-        self._freqhc = freq_range[1]
-
-    @property_depends_on( '_source.sample_freq, block_size, _ind_low, _freqlc' )
-    def _get_ind_low( self ):
-        fftfreq = self.fftfreq()
-        if fftfreq is not None:
-            if self._index_set_last:
-                return min(self._ind_low, fftfreq.shape[0]-1)
-            else:
-                return searchsorted(fftfreq[:-1], self._freqlc)
-
-    @property_depends_on( '_source.sample_freq, block_size, _ind_high, _freqhc' )
-    def _get_ind_high( self ):
-        fftfreq = self.fftfreq()
-        if fftfreq is not None:
-            if self._index_set_last:
-                if self._ind_high is None: 
-                    return None
-                else:
-                    return min(self._ind_high, fftfreq.shape[0]-1)
-            else:
-                if self._freqhc is None:
-                    return None
-                else:
-                    return searchsorted(fftfreq[:-1], self._freqhc)
+    @cached_property
+    def _get_digest(self):
+        return digest(self)
 
-    def _set_ind_high(self, ind_high):# by setting this the user sets the lower index
-        self._index_set_last = True
-        self._ind_high = ind_high
 
-    def _set_ind_low( self, ind_low):# by setting this the user sets the higher index
-        self._index_set_last = True
-        self._ind_low = ind_low
+class BeamformerTimeTraj(BeamformerTime):
+    """Provides a basic time domain beamformer with time signal output
+    for a grid moving along a trajectory.
+    """
 
-    def _set_time_data(self, time_data):
-        self._source = time_data
+    #: :class:`~acoular.trajectory.Trajectory` or derived object.
+    #: Start time is assumed to be the same as for the samples.
+    trajectory = Trait(Trajectory, desc='trajectory of the grid center')
 
-    def _set_source(self, source):
-        self._source = source
+    #: Reference vector, perpendicular to the y-axis of moving grid.
+    rvec = CArray(dtype=float, shape=(3,), value=array((0, 0, 0)), desc='reference vector')
 
-    def _get_time_data(self):
-        return self._source
+    #: Considering of convective amplification in beamforming formula.
+    conv_amp = Bool(False, desc='determines if convective amplification of source is considered')
 
-    def _get_source(self):
-        return self._source
+    #: Floating point and integer precision
+    precision = Trait(64, [32, 64], desc='numeric precision')
 
-    @property_depends_on( 'block_size, ind_low, ind_high' )
-    def _get_indices ( self ):
-        fftfreq = self.fftfreq()
-        if fftfreq is not None:
-            try:
-                indices = arange(fftfreq.shape[0],dtype=int)
-                if self.ind_high is None:
-                    return indices[ self.ind_low:]
-                else:
-                    return indices[ self.ind_low: self.ind_high ]
-            except IndexError:
-                return range(0)
+    # internal identifier
+    digest = Property(
+        depends_on=[
+            '_steer_obj.digest',
+            'source.digest',
+            'weights',
+            'precision',
+            'rvec',
+            'conv_amp',
+            'trajectory.digest',
+            '__class__',
+        ],
+    )
 
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
+    def _get_digest(self):
+        return digest(self)
 
-    @cached_property
-    def _get_basename( self ):
-        if 'basename' in self._source.all_trait_names():
-            return self._source.basename
-        else: 
-            return self._source.__class__.__name__ + self._source.digest
-
-    def calc_csm( self ):
-        """ csm calculation """
-        t = self.source
-        wind = self.window_( self.block_size )
-        weight = dot( wind, wind )
-        wind = wind[newaxis, :].swapaxes( 0, 1 )
-        numfreq = int(self.block_size/2 + 1)
-        csm_shape = (numfreq, t.numchannels, t.numchannels)
-        csmUpper = zeros(csm_shape, dtype=self.precision)
-        #print "num blocks", self.num_blocks
-        # for backward compatibility
-        if self.calib and self.calib.num_mics > 0:
-            if self.calib.num_mics == t.numchannels:
-                wind = wind * self.calib.data[newaxis, :]
-            else:
-                raise ValueError(
-                        "Calibration data not compatible: %i, %i" % \
-                        (self.calib.num_mics, t.numchannels))
-        # get time data blockwise
-        for data in self.get_source_data():
-            ft = fft.rfft(data*wind, None, 0).astype(self.precision)
-            calcCSM(csmUpper, ft)  # only upper triangular part of matrix is calculated (for speed reasons)
-        # create the full csm matrix via transposing and complex conj.
-        csmLower = csmUpper.conj().transpose(0,2,1)
-        [fill_diagonal(csmLower[cntFreq, :, :], 0) for cntFreq in range(csmLower.shape[0])]
-        csm = csmLower + csmUpper
-        # onesided spectrum: multiplication by 2.0=sqrt(2)^2
-        csm = csm*(2.0/self.block_size/weight/self.num_blocks)
-        return csm
-
-    def calc_ev ( self ):
-        """ eigenvalues / eigenvectors calculation """
-        if self.precision == 'complex128': eva_dtype = 'float64'
-        elif self.precision == 'complex64': eva_dtype = 'float32'
-#        csm = self.csm #trigger calculation
-        csm_shape = self.csm.shape
-        eva = empty(csm_shape[0:2], dtype=eva_dtype)
-        eve = empty(csm_shape, dtype=self.precision)
-        for i in range(csm_shape[0]):
-            (eva[i], eve[i])=linalg.eigh(self.csm[i])
-        return (eva,eve)
-
-    def calc_eva( self ):
-        """ calculates eigenvalues of csm """
-        return self.calc_ev()[0]
-    
-    def calc_eve( self ):
-        """ calculates eigenvectors of csm """
-        return self.calc_ev()[1]
-                
-    def _handle_dual_calibration(self):
-        obj = self.source # start with time_data obj
-        while obj:
-            if 'calib' in obj.all_trait_names(): # at original source?
-                if obj.calib and self.calib:
-                    if obj.calib.digest == self.calib.digest:
-                        self.calib = None # ignore it silently
-                    else:
-                        raise ValueError("Non-identical dual calibration for "\
-                                    "both TimeSamples and PowerSpectra object")
-                obj = None
-            else:
-                try:
-                    obj = obj.source # traverse down until original data source
-                except AttributeError:
-                    obj = None
+    def get_moving_gpos(self):
+        """Python generator that yields the moving grid coordinates samplewise."""
 
-    def _get_filecache( self, traitname ):
-        """
-        function handles result caching of csm, eigenvectors and eigenvalues
-        calculation depending on global/local caching behaviour.  
-        """
-        if traitname == 'csm':
-            func = self.calc_csm
-            numfreq = int(self.block_size/2 + 1)
-            shape = (numfreq, self._source.numchannels, self._source.numchannels)
-            precision = self.precision
-        elif traitname == 'eva':
-            func = self.calc_eva
-            shape = self.csm.shape[0:2]
-            if self.precision == 'complex128': precision = 'float64'
-            elif self.precision == 'complex64': precision = 'float32'
-        elif traitname == 'eve':
-            func = self.calc_eve
-            shape = self.csm.shape
-            precision = self.precision
-
-        H5cache.get_cache_file( self, self.basename ) 
-        if not self.h5f: # in case of global caching readonly
-            return func() 
-
-        nodename = traitname + '_' + self.digest 
-        if config.global_caching == 'overwrite' and self.h5f.is_cached(nodename):
-            #print("remove existing node",nodename)
-            self.h5f.remove_data(nodename) # remove old data before writing in overwrite mode
-        
-        if not self.h5f.is_cached(nodename): 
-            if config.global_caching == 'readonly': 
-                return func()
-#            print("create array, data not cached for",nodename)
-            self.h5f.create_compressible_array(nodename,shape,precision)
-            
-        ac = self.h5f.get_data_by_reference(nodename)
-        if ac[:].sum() == 0: # only initialized
-#            print("write {} to:".format(traitname),nodename)
-            ac[:] = func()
-            self.h5f.flush()
-        return ac
-             
-    @property_depends_on('digest')
-    def _get_csm ( self ):
-        """
-        Main work is done here:
-        Cross spectral matrix is either loaded from cache file or
-        calculated and then additionally stored into cache.
-        """
-        self._handle_dual_calibration()
-        if (
-                config.global_caching == 'none' or 
-                (config.global_caching == 'individual' and self.cached is False)
-            ):
-            return self.calc_csm()
-        else:
-            return self._get_filecache('csm')
-                          
-    @property_depends_on('digest')
-    def _get_eva ( self ):
-        """
-        Eigenvalues of cross spectral matrix are either loaded from cache file or
-        calculated and then additionally stored into cache.
-        """
-        if (
-                config.global_caching == 'none' or 
-                (config.global_caching == 'individual' and self.cached is False)
-            ):
-            return self.calc_eva()
-        else:
-            return self._get_filecache('eva')
+        def cross(a, b):
+            """Cross product for fast computation
+            because numpy.cross is ultra slow in this case.
+            """
+            return array([a[1] * b[2] - a[2] * b[1], a[2] * b[0] - a[0] * b[2], a[0] * b[1] - a[1] * b[0]])
 
-    @property_depends_on('digest')
-    def _get_eve ( self ):
-        """
-        Eigenvectors of cross spectral matrix are either loaded from cache file or
-        calculated and then additionally stored into cache.
-        """
-        if (
-                config.global_caching == 'none' or 
-                (config.global_caching == 'individual' and self.cached is False)
-            ):
-            return self.calc_eve()
+        start_t = 0.0
+        gpos = self.grid.pos()
+        trajg = self.trajectory.traj(start_t, delta_t=1 / self.source.sample_freq)
+        trajg1 = self.trajectory.traj(start_t, delta_t=1 / self.source.sample_freq, der=1)
+        rflag = (self.rvec == 0).all()  # flag translation vs. rotation
+        if rflag:
+            for g in trajg:
+                # grid is only translated, not rotated
+                tpos = gpos + array(g)[:, newaxis]
+                yield tpos
         else:
-            return self._get_filecache('eve')
+            for g, g1 in zip(trajg, trajg1):
+                # grid is both translated and rotated
+                loc = array(g)  # translation array([0., 0.4, 1.])
+                dx = array(g1)  # direction vector (new x-axis)
+                dy = cross(self.rvec, dx)  # new y-axis
+                dz = cross(dx, dy)  # new z-axis
+                RM = array((dx, dy, dz)).T  # rotation matrix
+                RM /= sqrt((RM * RM).sum(0))  # column normalized
+                tpos = dot(RM, gpos) + loc[:, newaxis]  # rotation+translation
+                #                print(loc[:])
+                yield tpos
+
+    def get_macostheta(self, g1, tpos, rm):
+        vvec = array(g1)  # velocity vector
+        ma = norm(vvec) / self.steer.env.c  # machnumber
+        fdv = (vvec / sqrt((vvec * vvec).sum()))[:, newaxis]  # unit vecor velocity
+        mpos = self.steer.mics.mpos[:, newaxis, :]
+        rmv = tpos[:, :, newaxis] - mpos
+        return (ma * sum(rmv.reshape((3, -1)) * fdv, 0) / rm.reshape(-1)).reshape(rm.shape)
+
+    def get_r0(self, tpos):
+        if isscalar(self.steer.ref) and self.steer.ref > 0:
+            return self.steer.ref  # full((self.steer.grid.size,), self.steer.ref)
+        return self.env._r(tpos)
+
+    def increase_buffer(self, num):
+        ar = zeros((num, self.steer.mics.num_mics), dtype=self.buffer.dtype)
+        self.buffer = concatenate((ar, self.buffer), axis=0)
+        self.bufferIndex += num
+
+    def result(self, num=2048):
+        """Python generator that yields the deconvolved output block-wise.
 
-    def synthetic_ev( self, freq, num=0):
-        """Return synthesized frequency band values of the eigenvalues.
-        
         Parameters
         ----------
-        freq : float 
-            Band center frequency for which to return the results.
-        num : integer
-            Controls the width of the frequency bands considered; defaults to
-            3 (third-octave band).
-            
-            ===  =====================
-            num  frequency band width
-            ===  =====================
-            0    single frequency line
-            1    octave band
-            3    third-octave band
-            n    1/n-octave band
-            ===  =====================
+        num : integer, defaults to 2048
+            This parameter defines the size of the blocks to be yielded
+            (i.e. the number of samples per block).
 
         Returns
         -------
-        float 
-            Synthesized frequency band value of the eigenvalues (the sum of
-            all values that are contained in the band).
+        Samples in blocks of shape  \
+        (num, :attr:`~BeamformerTime.numchannels`).
+            :attr:`~BeamformerTime.numchannels` is usually very \
+            large (number of grid points).
+            The last block may be shorter than num. \
+            The output starts for signals that were emitted
+            from the grid at `t=0`.
+
         """
-        f = self.fftfreq()
-        if num == 0:
-            # single frequency line
-            return self.eva[searchsorted(f, freq)]
+        # initialize values
+        if self.precision == 64:
+            fdtype = float64
+            idtype = int64
         else:
-            f1 = searchsorted(f, freq*2.**(-0.5/num))
-            f2 = searchsorted(f, freq*2.**(0.5/num))
-            if f1 == f2:
-                return self.eva[f1]
+            fdtype = float32
+            idtype = int32
+        w = self._get_weights()
+        c = self.steer.env.c / self.source.sample_freq
+        numMics = self.steer.mics.num_mics
+        mpos = self.steer.mics.mpos.astype(fdtype)
+        m_index = arange(numMics, dtype=idtype)
+        n_index = arange(num, dtype=idtype)[:, newaxis]
+        blockrm = empty((num, self.grid.size, numMics), dtype=fdtype)
+        blockrmconv = empty((num, self.grid.size, numMics), dtype=fdtype)
+        amp = empty((num, self.grid.size, numMics), dtype=fdtype)
+        # delays = empty((num,self.grid.size,numMics),dtype=fdtype)
+        d_index = empty((num, self.grid.size, numMics), dtype=idtype)
+        d_interp2 = empty((num, self.grid.size, numMics), dtype=fdtype)
+        blockr0 = empty((num, self.grid.size), dtype=fdtype)
+        self.buffer = zeros((2 * num, numMics), dtype=fdtype)
+        self.bufferIndex = self.buffer.shape[0]
+        movgpos = self.get_moving_gpos()  # create moving grid pos generator
+        movgspeed = self.trajectory.traj(0.0, delta_t=1 / self.source.sample_freq, der=1)
+        fill_buffer_generator = self._fill_buffer(num)
+        for _i in range(2):
+            next(fill_buffer_generator)
+
+        # preliminary implementation of different steering vectors
+        steer_func = {
+            'classic': _steer_I,
+            'inverse': _steer_II,
+            'true level': _steer_III,
+            'true location': _steer_IV,
+        }[self.steer.steer_type]
+
+        # start processing
+        flag = True
+        dflag = True  # data is available
+        while flag:
+            for i in range(num):
+                tpos = next(movgpos).astype(fdtype)
+                rm = self.steer.env._r(tpos, mpos)  # .astype(fdtype)
+                blockr0[i, :] = self.get_r0(tpos)
+                blockrm[i, :, :] = rm
+                if self.conv_amp:
+                    ht = next(movgspeed)
+                    blockrmconv[i, :, :] = rm * (1 - self.get_macostheta(ht, tpos, rm)) ** 2
+            if self.conv_amp:
+                steer_func(blockrmconv, blockr0, amp)
             else:
-                return sum(self.eva[f1:f2], 0)
+                steer_func(blockrm, blockr0, amp)
+            _delays(blockrm, c, d_interp2, d_index)
+            # _modf(delays, d_interp2, d_index)
+            maxdelay = (d_index.max((1, 2)) + arange(0, num)).max() + 2  # + because of interpolation
+            # increase buffer size because of greater delays
+            while maxdelay > self.buffer.shape[0] and dflag:
+                self.increase_buffer(num)
+                try:
+                    next(fill_buffer_generator)
+                except:
+                    dflag = False
+            samplesleft = self.buffer.shape[0] - self.bufferIndex
+            # last block may be shorter
+            if samplesleft - maxdelay <= 0:
+                num = sum((d_index.max((1, 2)) + 1 + arange(0, num)) < samplesleft)
+                n_index = arange(num, dtype=idtype)[:, newaxis]
+                flag = False
+            # init step
+            p_res = self.buffer[self.bufferIndex : self.bufferIndex + maxdelay, :].copy()
+            Phi, autopow = self.delay_and_sum(num, p_res, d_interp2, d_index, amp)
+            if 'Cleant' not in self.__class__.__name__:
+                if 'Sq' not in self.__class__.__name__:
+                    yield Phi[:num]
+                elif self.r_diag:
+                    yield (Phi[:num] ** 2 - autopow[:num]).clip(min=0)
+                else:
+                    yield Phi[:num] ** 2
+            else:
+                # choose correct distance
+                blockrm1 = blockrmconv if self.conv_amp else blockrm
+                Gamma = zeros(Phi.shape, dtype=fdtype)
+                Gamma_autopow = zeros(Phi.shape, dtype=fdtype)
+                J = 0
+                t_ind = arange(p_res.shape[0], dtype=idtype)
+                # deconvolution
+                while self.n_iter > J:
+                    # print(f"start clean iteration {J+1} of max {self.n_iter}")
+                    if self.r_diag:
+                        powPhi = (Phi[:num] * Phi[:num] - autopow).sum(0).clip(min=0)
+                    else:
+                        powPhi = (Phi[:num] * Phi[:num]).sum(0)
+                    # find index of max power focus point
+                    imax = argmax(powPhi)
+                    # find backward delays
+                    t_float = (d_interp2[:num, imax, m_index] + d_index[:num, imax, m_index] + n_index).astype(fdtype)
+                    # determine max/min delays in sample units
+                    # + 2 because we do not want to extrapolate behind the last sample
+                    ind_max = t_float.max(0).astype(idtype) + 2
+                    ind_min = t_float.min(0).astype(idtype)
+                    # store time history at max power focus point
+                    h = Phi[:num, imax] * blockr0[:num, imax]
+                    for m in range(numMics):
+                        # subtract interpolated time history from microphone signals
+                        p_res[ind_min[m] : ind_max[m], m] -= self.damp * interp(
+                            t_ind[ind_min[m] : ind_max[m]],
+                            t_float[:num, m],
+                            h / blockrm1[:num, imax, m],
+                        )
+                    nextPhi, nextAutopow = self.delay_and_sum(num, p_res, d_interp2, d_index, amp)
+                    if self.r_diag:
+                        pownextPhi = (nextPhi[:num] * nextPhi[:num] - nextAutopow).sum(0).clip(min=0)
+                    else:
+                        pownextPhi = (nextPhi[:num] * nextPhi[:num]).sum(0)
+                    # print(f"total signal power: {powPhi.sum()}")
+                    if pownextPhi.sum() < powPhi.sum():  # stopping criterion
+                        Gamma[:num, imax] += self.damp * Phi[:num, imax]
+                        Gamma_autopow[:num, imax] = autopow[:num, imax].copy()
+                        Phi = nextPhi
+                        autopow = nextAutopow
+                        # print(f"clean max: {L_p((Gamma**2).sum(0)/num).max()} dB")
+                        J += 1
+                    else:
+                        break
+                if 'Sq' not in self.__class__.__name__:
+                    yield Gamma[:num]
+                elif self.r_diag:
+                    yield Gamma[:num] ** 2 - (self.damp**2) * Gamma_autopow[:num]
+                else:
+                    yield Gamma[:num] ** 2
+            self.bufferIndex += num
+            try:
+                next(fill_buffer_generator)
+            except:
+                dflag = False
+
+    def delay_and_sum(self, num, p_res, d_interp2, d_index, amp):
+        """Standard delay-and-sum method."""
+        fdtype = float64 if self.precision == 64 else float32
+        result = empty((num, self.grid.size), dtype=fdtype)  # output array
+        autopow = empty((num, self.grid.size), dtype=fdtype)  # output array
+        _delayandsum5(p_res, d_index, d_interp2, amp, result, autopow)
+        return result, autopow
+
+
+class BeamformerTimeSqTraj(BeamformerTimeSq, BeamformerTimeTraj):
+    """Provides a time domain beamformer with time-dependent
+    power signal output and possible autopower removal
+    for a grid moving along a trajectory.
+    """
 
+    # internal identifier
+    digest = Property(
+        depends_on=[
+            '_steer_obj.digest',
+            'source.digest',
+            'r_diag',
+            'weights',
+            'precision',
+            'rvec',
+            'conv_amp',
+            'trajectory.digest',
+            '__class__',
+        ],
+    )
 
+    @cached_property
+    def _get_digest(self):
+        return digest(self)
 
-def synthetic (data, freqs, f, num=3):
-    """
-    Returns synthesized frequency band values of spectral data.
-    
-    If used with :meth:`Beamformer.result()<acoular.fbeamform.BeamformerBase.result>` 
-    and only one frequency band, the output is identical to the result of the intrinsic 
-    :meth:`Beamformer.synthetic<acoular.fbeamform.BeamformerBase.synthetic>` method.
-    It can, however, also be used with the 
-    :meth:`Beamformer.integrate<acoular.fbeamform.BeamformerBase.integrate>`
-    output and more frequency bands.
-    
-    Parameters
-    ----------
-    data : array of floats
-        The spectral data (squared sound pressures in Pa^2) in an array with one value 
-        per frequency line.
-        The number of entries must be identical to the number of
-        grid points.
-    freq : array of floats
-        The frequencies that correspon to the input *data* (as yielded by
-        the :meth:`PowerSpectra.fftfreq<acoular.spectra.PowerSpectra.fftfreq>`
-        method).
-    f : float or list of floats
-        Band center frequency/frequencies for which to return the results.
-    num : integer
-        Controls the width of the frequency bands considered; defaults to
-        3 (third-octave band).
-        
-        ===  =====================
-        num  frequency band width
-        ===  =====================
-        0    single frequency line
-        1    octave band
-        3    third-octave band
-        n    1/n-octave band
-        ===  =====================
 
-    Returns
-    -------
-    array of floats
-        Synthesized frequency band values of the beamforming result at 
-        each grid point (the sum of all values that are contained in the band).
-        Note that the frequency resolution and therefore the bandwidth 
-        represented by a single frequency line depends on 
-        the :attr:`sampling frequency<acoular.tprocess.SamplesGenerator.sample_freq>` 
-        and used :attr:`FFT block size<acoular.spectra.PowerSpectra.block_size>`.
-    """
-    if isscalar(f):
-        f = (f,)
-    if num == 0:
-        # single frequency lines
-        res = list()
-        for i in f:
-            ind = searchsorted(freqs, i)
-            if ind >= len(freqs):
-                warn('Queried frequency (%g Hz) not in resolved '
-                     'frequency range. Returning zeros.' % i, 
-                     Warning, stacklevel = 2)
-                h = zeros_like(data[0])
-            else:
-                if freqs[ind] != i:
-                    warn('Queried frequency (%g Hz) not in set of '
-                         'discrete FFT sample frequencies. '
-                         'Using frequency %g Hz instead.' % (i,freqs[ind]), 
-                         Warning, stacklevel = 2)
-                h = data[ind]
-            res += [h]      
-    else:
-        # fractional octave bands
-        res = list()
-        for i in f:
-            f1 = i*2.**(-0.5/num)
-            f2 = i*2.**(+0.5/num)
-            ind1 = searchsorted(freqs, f1)
-            ind2 = searchsorted(freqs, f2)
-            if ind1 == ind2:
-                warn('Queried frequency band (%g to %g Hz) does not '
-                     'include any discrete FFT sample frequencies. '
-                     'Returning zeros.' % (f1,f2), 
-                     Warning, stacklevel = 2)
-                h = zeros_like(data[0])
-            else:
-                h = sum(data[ind1:ind2], 0)
-            res += [h]
-    return array(res)
-
-
-class PowerSpectraImport( PowerSpectra ):
-    """Provides a dummy class for using pre-calculated cross-spectral
-    matrices. 
-
-    This class does not calculate the cross-spectral matrix. Instead, 
-    the user can inject one or multiple existing CSMs by setting the 
-    :attr:`csm` attribute. This can be useful when algorithms shall be
-    evaluated with existing CSM matrices.
-    The frequency or frequencies contained by the CSM must be set via the 
-    attr:`frequencies` attribute. The attr:`numchannels` attributes
-    is determined on the basis of the CSM shape. 
-    In contrast to the PowerSpectra object, the attributes 
-    :attr:`sample_freq`, :attr:`time_data`, :attr:`source`,
-    :attr:`block_size`, :attr:`calib`, :attr:`window`, 
-    :attr:`overlap`, :attr:`cached`, and :attr:`num_blocks`
-    have no functionality. 
+class BeamformerCleant(BeamformerTime):
+    """CLEANT deconvolution method, see :ref:`Cousson et al., 2019<Cousson2019>`.
+
+    An implementation of the CLEAN method in time domain. This class can only
+    be used for static sources.
     """
 
-    #: The cross spectral matrix, 
-    #: (number of frequencies, numchannels, numchannels) array of complex;
-    csm = Property( 
-        desc="cross spectral matrix")
+    #: Boolean flag, always False
+    r_diag = Enum(False, desc='False, as we do not remove autopower in this beamformer')
 
-    #: frequencies included in the cross-spectral matrix in ascending order.
-    #: Compound trait that accepts arguments of type list, array, and float
-    frequencies = Trait(None,(CArray,Float),
-        desc="frequencies included in the cross-spectral matrix")
+    #: iteration damping factor also referred as loop gain in Cousson et al.
+    #: defaults to 0.6
+    damp = Range(0.01, 1.0, 0.6, desc='damping factor (loop gain)')
 
-    #: Number of time data channels 
-    numchannels = Property(depends_on=['digest'])
+    #: max number of iterations
+    n_iter = Int(100, desc='maximum number of iterations')
 
-    time_data = Enum(None, 
-        desc="PowerSpectraImport cannot consume time data")
+    # internal identifier
+    digest = Property(
+        depends_on=['_steer_obj.digest', 'source.digest', 'weights', '__class__', 'damp', 'n_iter'],
+    )
 
-    source = Enum(None, 
-        desc="PowerSpectraImport cannot consume time data")
+    @cached_property
+    def _get_digest(self):
+        return digest(self)
 
-    # Sampling frequency of the signal, defaults to None
-    sample_freq = Enum(None, 
-        desc="sampling frequency")
 
-    block_size = Enum(None, 
-        desc="PowerSpectraImport does not operate on blocks of time data")
+class BeamformerCleantSq(BeamformerCleant):
+    """CLEANT deconvolution method, see :ref:`Cousson et al., 2019<Cousson2019>`
+    with optional removal of autocorrelation.
 
-    calib = Enum(None,
-        desc="PowerSpectraImport cannot calibrate the time data")
+    An implementation of the CLEAN method in time domain. This class can only
+    be used for static sources.
+    """
+
+    #: Boolean flag, if 'True' (default), the main diagonal is removed before beamforming.
+    r_diag = Bool(True, desc='removal of diagonal')
 
-    window = Enum(None,
-            desc="PowerSpectraImport does not perform windowing")
+    # internal identifier
+    digest = Property(
+        depends_on=['_steer_obj.digest', 'source.digest', 'weights', '__class__', 'damp', 'n_iter', 'r_diag'],
+    )
 
-    overlap = Enum(None,
-            desc="PowerSpectraImport does not consume time data")
+    @cached_property
+    def _get_digest(self):
+        return digest(self)
 
-    cached = Enum(False,
-            desc="PowerSpectraImport has no caching capabilities")
 
-    num_blocks = Enum(None,
-            desc="PowerSpectraImport cannot determine the number of blocks")
+class BeamformerCleantTraj(BeamformerCleant, BeamformerTimeTraj):
+    """CLEANT deconvolution method, see :ref:`Cousson et al., 2019<Cousson2019>`.
 
-    # Shadow trait, should not be set directly, for internal use.
-    _ind_low = Int(0,
-        desc="index of lowest frequency line")
+    An implementation of the CLEAN method in time domain for moving sources
+    with known trajectory.
+    """
 
-    # Shadow trait, should not be set directly, for internal use.
-    _ind_high = Trait(None,(Int,None),
-        desc="index of highest frequency line")
+    #: Floating point and integer precision
+    precision = Trait(32, [32, 64], desc='numeric precision')
 
     # internal identifier
-    digest = Property( 
-        depends_on = ['_csmsum', 
-            ], 
-        )
-
-    #: Name of the cache file without extension, readonly.
-    basename = Property( depends_on = 'digest', 
-        desc="basename for cache file")
-
-    # csm shadow trait, only for internal use.
-    _csm = CArray()
-        
-    # CSM checksum to trigger digest calculation, only for internal use.
-    _csmsum = Float() 
+    digest = Property(
+        depends_on=[
+            '_steer_obj.digest',
+            'source.digest',
+            'weights',
+            'precision',
+            '__class__',
+            'damp',
+            'n_iter',
+            'rvec',
+            'conv_amp',
+            'trajectory.digest',
+        ],
+    )
+
+    @cached_property
+    def _get_digest(self):
+        return digest(self)
+
 
-    def _get_basename( self ):
-        return "csm_import_"+self.digest
+class BeamformerCleantSqTraj(BeamformerCleantTraj, BeamformerTimeSq):
+    """CLEANT deconvolution method, see :ref:`Cousson et al., 2019<Cousson2019>`
+    with optional removal of autocorrelation.
+
+    An implementation of the CLEAN method in time domain for moving sources
+    with known trajectory.
+    """
+
+    #: Boolean flag, if 'True' (default), the main diagonal is removed before beamforming.
+    r_diag = Bool(True, desc='removal of diagonal')
+
+    # internal identifier
+    digest = Property(
+        depends_on=[
+            '_steer_obj.digest',
+            'source.digest',
+            'weights',
+            'precision',
+            '__class__',
+            'damp',
+            'n_iter',
+            'rvec',
+            'conv_amp',
+            'trajectory.digest',
+            'r_diag',
+        ],
+    )
 
     @cached_property
-    def _get_digest( self ):
-        return digest( self )
+    def _get_digest(self):
+        return digest(self)
 
-    def _get_numchannels( self ):
-        return self.csm.shape[1]
 
-    def _get_csm ( self ):
-        return self._csm
+class IntegratorSectorTime(TimeInOut):
+    """Provides an Integrator in the time domain."""
 
-    def _set_csm (self, csm):
-        if (len(csm.shape) != 3) or (csm.shape[1] != csm.shape[2]):
-            raise ValueError(
-                "The cross spectral matrix must have the following shape: (number of frequencies, numchannels, numchannels)!")
-        self._csmsum = real(self._csm).sum() + (imag(self._csm)**2).sum() # to trigger new digest creation
-        self._csm = csm
+    #: :class:`~acoular.grids.RectGrid` object that provides the grid locations.
+    grid = Trait(RectGrid, desc='beamforming grid')
 
-    @property_depends_on('digest')
-    def _get_eva ( self ):
-        """
-        Eigenvalues of cross spectral matrix are either loaded from cache file or
-        calculated and then additionally stored into cache.
-        """
-        return self.calc_eva()
+    #: List of sectors in grid
+    sectors = List()
 
-    @property_depends_on('digest')
-    def _get_eve ( self ):
-        """
-        Eigenvectors of cross spectral matrix are either loaded from cache file or
-        calculated and then additionally stored into cache.
-        """
-        return self.calc_eve()
+    #: Clipping, in Dezibel relative to maximum (negative values)
+    clip = Float(-350.0)
+
+    #: Number of channels in output (= number of sectors).
+    numchannels = Property(depends_on=['sectors'])
+
+    # internal identifier
+    digest = Property(
+        depends_on=['sectors', 'clip', 'grid.digest', 'source.digest', '__class__'],
+    )
+
+    @cached_property
+    def _get_digest(self):
+        return digest(self)
+
+    @cached_property
+    def _get_numchannels(self):
+        return len(self.sectors)
+
+    def result(self, num=1):
+        """Python generator that yields the source output integrated over the given
+        sectors, block-wise.
+
+        Parameters
+        ----------
+        num : integer, defaults to 1
+            This parameter defines the size of the blocks to be yielded
+            (i.e. the number of samples per block).
 
-    def fftfreq ( self ):
-        """
-        Return the Discrete Fourier Transform sample frequencies.
-        
         Returns
         -------
-        f : ndarray
-            Array containing the frequencies.
-        """
-        if isinstance(self.frequencies,float): 
-            return array([self.frequencies])
-        elif isinstance(self.frequencies,ndarray):
-            return self.frequencies
-        elif self.frequencies is None:
-            warn("No frequencies defined for PowerSpectraImport object!")
-            return self.frequencies
-        else:
-            return self.frequencies
+        Samples in blocks of shape (num, :attr:`numchannels`).
+        :attr:`numchannels` is the number of sectors.
+        The last block may be shorter than num.
+
+        """
+        inds = [self.grid.indices(*sector) for sector in self.sectors]
+        gshape = self.grid.shape
+        o = empty((num, self.numchannels), dtype=float)  # output array
+        for r in self.source.result(num):
+            ns = r.shape[0]
+            mapshape = (ns,) + gshape
+            rmax = r.max()
+            rmin = rmax * 10 ** (self.clip / 10.0)
+            r = where(r > rmin, r, 0.0)
+            for i, ind in enumerate(inds):
+                h = r[:].reshape(mapshape)[(s_[:],) + ind]
+                o[:ns, i] = h.reshape(h.shape[0], -1).sum(axis=1)
+                i += 1
+            yield o[:ns]
```

### Comparing `acoular-24.3/acoular/tprocess.py` & `acoular-24.5/acoular/tprocess.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-# -*- coding: utf-8 -*-
-#pylint: disable-msg=E0611, E1101, C0103, R0901, R0902, R0903, R0904, W0232
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 # Copyright (c) Acoular Development Team.
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 """Implements processing in the time domain.
 
 .. autosummary::
     :toctree: generated/
 
     SamplesGenerator
     TimeInOut
@@ -33,752 +31,815 @@
     WriteWAV
     WriteH5
     SampleSplitter
     TimeConvolve
 """
 
 # imports from other packages
-from numpy import array, empty, empty_like, pi, sin, sqrt, zeros, newaxis, unique, \
-int16, nan, concatenate, sum, float64, identity, argsort, interp, arange, append, \
-linspace, flatnonzero, argmin, argmax, delete, mean, inf, asarray, stack, sinc, exp, \
-polymul, arange, cumsum, ceil, split, array_equal
+import threading
+import wave
+from collections import deque
+from datetime import datetime, timezone
+from inspect import currentframe
+from os import path
+from warnings import warn
 
+import numba as nb
+from numpy import (
+    append,
+    arange,
+    argmax,
+    argmin,
+    argsort,
+    array,
+    array_equal,
+    asarray,
+    ceil,
+    concatenate,
+    cumsum,
+    delete,
+    empty,
+    empty_like,
+    exp,
+    flatnonzero,
+    float64,
+    identity,
+    inf,
+    int16,
+    interp,
+    linspace,
+    mean,
+    nan,
+    newaxis,
+    pi,
+    polymul,
+    sin,
+    sinc,
+    split,
+    sqrt,
+    stack,
+    sum,
+    unique,
+    zeros,
+)
 from numpy.linalg import norm
 from numpy.matlib import repmat
-
+from scipy.fft import irfft, rfft
+from scipy.interpolate import CloughTocher2DInterpolator, CubicSpline, LinearNDInterpolator, Rbf, splev, splrep
+from scipy.signal import bilinear, butter, sosfilt, sosfiltfilt, tf2sos
 from scipy.spatial import Delaunay
-from scipy.interpolate import LinearNDInterpolator,splrep, splev, \
-CloughTocher2DInterpolator, CubicSpline, Rbf
-from traits.api import HasPrivateTraits, Float, Int, CLong, Bool, ListInt, \
-Constant, File, Property, Instance, Trait, Delegate, Str, \
-cached_property, on_trait_change, List, CArray, Dict, PrefixMap, Callable,\
-observe
-
-from scipy.fft import rfft, irfft
-import numba as nb
+from traits.api import (
+    Bool,
+    CArray,
+    CLong,
+    Constant,
+    Delegate,
+    Dict,
+    File,
+    Float,
+    HasPrivateTraits,
+    Instance,
+    Int,
+    List,
+    ListInt,
+    Property,
+    Str,
+    Trait,
+    cached_property,
+    observe,
+    on_trait_change,
+)
 
-from datetime import datetime
-from os import path
-import wave
-from scipy.signal import butter, filtfilt, bilinear, tf2sos, sosfilt, sosfiltfilt
-from warnings import warn
-from collections import deque
-from inspect import currentframe
-import threading
+from .configuration import config
+from .environments import cartToCyl, cylToCart
+from .h5cache import H5cache
+from .h5files import H5CacheFileBase, _get_h5file_class
 
 # acoular imports
 from .internal import digest, ldigest
-from .h5cache import H5cache
-from .h5files import H5CacheFileBase, _get_h5file_class
-from .environments import cartToCyl,cylToCart
 from .microphones import MicGeom
-from .configuration import config
 
 
-class SamplesGenerator( HasPrivateTraits ):
-    """
-    Base class for any generating signal processing block
-    
+class SamplesGenerator(HasPrivateTraits):
+    """Base class for any generating signal processing block.
+
     It provides a common interface for all SamplesGenerator classes, which
     generate an output via the generator :meth:`result`.
-    This class has no real functionality on its own and should not be 
+    This class has no real functionality on its own and should not be
     used directly.
     """
 
     #: Sampling frequency of the signal, defaults to 1.0
-    sample_freq = Float(1.0, 
-        desc="sampling frequency")
-    
-    #: Number of channels 
+    sample_freq = Float(1.0, desc='sampling frequency')
+
+    #: Number of channels
     numchannels = CLong
-               
-    #: Number of samples 
+
+    #: Number of samples
     numsamples = CLong
-    
+
     # internal identifier
-    digest = Property(depends_on = ['sample_freq', 'numchannels', 'numsamples'])
-    
-    def _get_digest( self ): 
-        return digest( self )
-               
+    digest = Property(depends_on=['sample_freq', 'numchannels', 'numsamples'])
+
+    def _get_digest(self):
+        return digest(self)
+
     def result(self, num):
-        """
-        Python generator that yields the output block-wise.
-                
+        """Python generator that yields the output block-wise.
+
         Parameters
         ----------
         num : integer
             This parameter defines the size of the blocks to be yielded
-            (i.e. the number of samples per block) 
-        
+            (i.e. the number of samples per block)
+
         Returns
         -------
         No output since `SamplesGenerator` only represents a base class to derive
         other classes from.
+
         """
-        pass
 
 
-class TimeInOut( SamplesGenerator ):
-    """
-    Base class for any time domain signal processing block, 
-    gets samples from :attr:`source` and generates output via the 
-    generator :meth:`result`
+class TimeInOut(SamplesGenerator):
+    """Base class for any time domain signal processing block,
+    gets samples from :attr:`source` and generates output via the
+    generator :meth:`result`.
     """
 
     #: Data source; :class:`~acoular.sources.SamplesGenerator` or derived object.
     source = Trait(SamplesGenerator)
 
     #: Sampling frequency of output signal, as given by :attr:`source`.
     sample_freq = Delegate('source')
-    
+
     #: Number of channels in output, as given by :attr:`source`.
     numchannels = Delegate('source')
-               
+
     #: Number of samples in output, as given by :attr:`source`.
     numsamples = Delegate('source')
-            
+
     # internal identifier
-    digest = Property( depends_on = ['source.digest'])
+    digest = Property(depends_on=['source.digest'])
 
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
     def result(self, num):
-        """ 
-        Python generator: dummy function, just echoes the output of source,
+        """Python generator: dummy function, just echoes the output of source,
         yields samples in blocks of shape (num, :attr:`numchannels`), the last block
         may be shorter than num.
         """
-        for temp in self.source.result(num):
-            # effectively no processing
-            yield temp
+        yield from self.source.result(num)
 
 
-class MaskedTimeInOut ( TimeInOut ):
-    """
-    Signal processing block for channel and sample selection.
-    
-    This class serves as intermediary to define (in)valid 
-    channels and samples for any 
+class MaskedTimeInOut(TimeInOut):
+    """Signal processing block for channel and sample selection.
+
+    This class serves as intermediary to define (in)valid
+    channels and samples for any
     :class:`~acoular.sources.SamplesGenerator` (or derived) object.
-    It gets samples from :attr:`~acoular.tprocess.TimeInOut.source` 
+    It gets samples from :attr:`~acoular.tprocess.TimeInOut.source`
     and generates output via the generator :meth:`result`.
     """
-        
+
     #: Index of the first sample to be considered valid.
-    start = CLong(0, 
-        desc="start of valid samples")
-    
+    start = CLong(0, desc='start of valid samples')
+
     #: Index of the last sample to be considered valid.
-    stop = Trait(None, None, CLong, 
-        desc="stop of valid samples")
-    
+    stop = Trait(None, None, CLong, desc='stop of valid samples')
+
     #: Channels that are to be treated as invalid.
-    invalid_channels = ListInt(
-        desc="list of invalid channels")
-    
+    invalid_channels = ListInt(desc='list of invalid channels')
+
     #: Channel mask to serve as an index for all valid channels, is set automatically.
-    channels = Property(depends_on = ['invalid_channels', 'source.numchannels'], 
-        desc="channel mask")
-    
+    channels = Property(depends_on=['invalid_channels', 'source.numchannels'], desc='channel mask')
+
     #: Number of channels in input, as given by :attr:`~acoular.tprocess.TimeInOut.source`.
     numchannels_total = Delegate('source', 'numchannels')
-               
+
     #: Number of samples in input, as given by :attr:`~acoular.tprocess.TimeInOut.source`.
     numsamples_total = Delegate('source', 'numsamples')
 
     #: Number of valid channels, is set automatically.
-    numchannels = Property(depends_on = ['invalid_channels', \
-        'source.numchannels'], desc="number of valid input channels")
+    numchannels = Property(depends_on=['invalid_channels', 'source.numchannels'], desc='number of valid input channels')
 
     #: Number of valid time samples, is set automatically.
-    numsamples = Property(depends_on = ['start', 'stop', 'source.numsamples'], 
-        desc="number of valid samples per channel")
+    numsamples = Property(depends_on=['start', 'stop', 'source.numsamples'], desc='number of valid samples per channel')
 
     #: Name of the cache file without extension, readonly.
-    basename = Property( depends_on = 'source.digest', 
-        desc="basename for cache file")
+    basename = Property(depends_on='source.digest', desc='basename for cache file')
 
     # internal identifier
-    digest = Property( depends_on = ['source.digest', 'start', 'stop', \
-        'invalid_channels'])
+    digest = Property(depends_on=['source.digest', 'start', 'stop', 'invalid_channels'])
 
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
     @cached_property
-    def _get_basename( self ):
+    def _get_basename(self):
         if 'basename' in self.source.all_trait_names():
             return self.source.basename
-        else: 
-            return self.source.__class__.__name__ + self.source.digest
-    
+        return self.source.__class__.__name__ + self.source.digest
+
     @cached_property
-    def _get_channels( self ):
-        if len(self.invalid_channels)==0:
+    def _get_channels(self):
+        if len(self.invalid_channels) == 0:
             return slice(0, None, None)
-        allr=[i for i in range(self.numchannels_total) if not (i in self.invalid_channels)]
+        allr = [i for i in range(self.numchannels_total) if i not in self.invalid_channels]
         return array(allr)
-    
+
     @cached_property
-    def _get_numchannels( self ):
-        if len(self.invalid_channels)==0:
+    def _get_numchannels(self):
+        if len(self.invalid_channels) == 0:
             return self.numchannels_total
         return len(self.channels)
-    
+
     @cached_property
-    def _get_numsamples( self ):
+    def _get_numsamples(self):
         sli = slice(self.start, self.stop).indices(self.numsamples_total)
-        return sli[1]-sli[0]
+        return sli[1] - sli[0]
 
     def result(self, num):
-        """ 
-        Python generator that yields the output block-wise.
-        
+        """Python generator that yields the output block-wise.
+
         Parameters
         ----------
         num : integer
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block).
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, :attr:`numchannels`). 
+        Samples in blocks of shape (num, :attr:`numchannels`).
             The last block may be shorter than num.
+
         """
         sli = slice(self.start, self.stop).indices(self.numsamples_total)
         start = sli[0]
         stop = sli[1]
         if start >= stop:
-            raise IOError("no samples available")
-        
+            msg = 'no samples available'
+            raise OSError(msg)
+
         if start != 0 or stop != self.numsamples_total:
             offset = -start % num
-            if offset == 0: offset = num
-            buf = empty((num + offset , self.numchannels), dtype=float)
+            if offset == 0:
+                offset = num
+            buf = empty((num + offset, self.numchannels), dtype=float)
             bsize = 0
             i = 0
             fblock = True
             for block in self.source.result(num):
                 bs = block.shape[0]
                 i += bs
-                if fblock and i >= start : # first block in the chosen interval
-                    if i>= stop: # special case that start and stop are in one block
-                        yield block[bs-(i-start):bs-(i-stop),self.channels]
+                if fblock and i >= start:  # first block in the chosen interval
+                    if i >= stop:  # special case that start and stop are in one block
+                        yield block[bs - (i - start) : bs - (i - stop), self.channels]
                         break
-                    bsize += (i-start)
-                    buf[:(i-start),:] = block[bs-(i-start):,self.channels]
+                    bsize += i - start
+                    buf[: (i - start), :] = block[bs - (i - start) :, self.channels]
                     fblock = False
-                elif i >= stop: # last block
-                    buf[bsize:bsize+bs-(i-stop),:] = block[:bs-(i-stop),self.channels]
-                    bsize += bs-(i-stop)
-                    if bsize >num:
+                elif i >= stop:  # last block
+                    buf[bsize : bsize + bs - (i - stop), :] = block[: bs - (i - stop), self.channels]
+                    bsize += bs - (i - stop)
+                    if bsize > num:
                         yield buf[:num]
-                        buf[:bsize-num,:] = buf[num:bsize,:]
+                        buf[: bsize - num, :] = buf[num:bsize, :]
                         bsize -= num
-                    yield buf[:bsize,:]
+                    yield buf[:bsize, :]
                     break
-                elif i >=start :
-                    buf[bsize:bsize+bs,:] = block[:,self.channels]
+                elif i >= start:
+                    buf[bsize : bsize + bs, :] = block[:, self.channels]
                     bsize += bs
-                if bsize>=num:
+                if bsize >= num:
                     yield buf[:num]
-                    buf[:bsize-num,:] = buf[num:bsize,:]
+                    buf[: bsize - num, :] = buf[num:bsize, :]
                     bsize -= num
-        
-        else: # if no start/stop given, don't do the resorting thing
+
+        else:  # if no start/stop given, don't do the resorting thing
             for block in self.source.result(num):
                 yield block[:, self.channels]
 
 
-class ChannelMixer( TimeInOut ):
-    """
-    Class for directly mixing the channels of a multi-channel source. 
+class ChannelMixer(TimeInOut):
+    """Class for directly mixing the channels of a multi-channel source.
     Outputs a single channel.
     """
-    
+
     #: Amplitude weight(s) for the channels as array. If not set, all channels are equally weighted.
-    weights = CArray(desc="channel weights")
-    
+    weights = CArray(desc='channel weights')
+
     # Number of channels is always one here.
     numchannels = Constant(1)
-    
+
     # internal identifier
-    digest = Property( depends_on = ['source.digest', 'weights'])
+    digest = Property(depends_on=['source.digest', 'weights'])
 
     @cached_property
-    def _get_digest( self ):
-        return digest(self)         
+    def _get_digest(self):
+        return digest(self)
 
     def result(self, num):
-        """ 
-        Python generator that yields the output block-wise.
-        
+        """Python generator that yields the output block-wise.
+
         Parameters
         ----------
         num : integer
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block).
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, 1). 
+        Samples in blocks of shape (num, 1).
             The last block may be shorter than num.
+
         """
         if self.weights.size:
             if self.weights.shape in {(self.source.numchannels,), (1,)}:
                 weights = self.weights
             else:
-                raise ValueError("Weight factors can not be broadcasted: %s, %s" % \
-                                 (self.weights.shape, (self.source.numchannels,)))
-        else: 
+                msg = f'Weight factors can not be broadcasted: {self.weights.shape}, {(self.source.numchannels,)}'
+                raise ValueError(msg)
+        else:
             weights = 1
-        
+
         for block in self.source.result(num):
-            yield sum(weights*block, 1, keepdims=True)
-  
-    
+            yield sum(weights * block, 1, keepdims=True)
+
+
 class Trigger(TimeInOut):
-    """
-    Class for identifying trigger signals.
+    """Class for identifying trigger signals.
     Gets samples from :attr:`source` and stores the trigger samples in :meth:`trigger_data`.
-    
+
     The algorithm searches for peaks which are above/below a signed threshold.
     A estimate for approximative length of one revolution is found via the greatest
     number of samples between the adjacent peaks.
     The algorithm then defines hunks as percentages of the estimated length of one revolution.
-    If there are multiple peaks within one hunk, the algorithm just takes one of them 
+    If there are multiple peaks within one hunk, the algorithm just takes one of them
     into account (e.g. the first peak, the peak with extremum value, ...).
     In the end, the algorithm checks if the found peak locations result in rpm that don't
     vary too much.
     """
+
     #: Data source; :class:`~acoular.tprocess.SamplesGenerator` or derived object.
     source = Instance(SamplesGenerator)
-    
-    #: Threshold of trigger. Has different meanings for different 
+
+    #: Threshold of trigger. Has different meanings for different
     #: :attr:`~acoular.tprocess.Trigger.trigger_type`. The sign is relevant.
-    #: If a sample of the signal is above/below the positive/negative threshold, 
+    #: If a sample of the signal is above/below the positive/negative threshold,
     #: it is assumed to be a peak.
     #: Default is None, in which case a first estimate is used: The threshold
-    #: is assumed to be 75% of the max/min difference between all extremums and the 
+    #: is assumed to be 75% of the max/min difference between all extremums and the
     #: mean value of the trigger signal. E.g: the mean value is 0 and there are positive
-    #: extremums at 400 and negative extremums at -800. Then the estimated threshold would be 
+    #: extremums at 400 and negative extremums at -800. Then the estimated threshold would be
     #: 0.75 * -800 = -600.
     threshold = Float(None)
-    
+
     #: Maximum allowable variation of length of each revolution duration. Default is
     #: 2%. A warning is thrown, if any revolution length surpasses this value:
     #: abs(durationEachRev - meanDuration) > 0.02 * meanDuration
     max_variation_of_duration = Float(0.02)
-    
+
     #: Defines the length of hunks via lenHunk = hunk_length * maxOncePerRevDuration.
-    #: If there are multiple peaks within lenHunk, then the algorithm will 
+    #: If there are multiple peaks within lenHunk, then the algorithm will
     #: cancel all but one out (see :attr:`~acoular.tprocess.Trigger.multiple_peaks_in_hunk`).
     #: Default is to 0.1.
     hunk_length = Float(0.1)
-    
+
     #: Type of trigger.
     #:
-    #: 'dirac': a single puls is assumed (sign of  
+    #: 'dirac': a single puls is assumed (sign of
     #: :attr:`~acoular.tprocess.Trigger.trigger_type` is important).
     #: Sample will trigger if its value is above/below the pos/neg threshold.
-    #: 
-    #: 'rect' : repeating rectangular functions. Only every second 
-    #: edge is assumed to be a trigger. The sign of 
+    #:
+    #: 'rect' : repeating rectangular functions. Only every second
+    #: edge is assumed to be a trigger. The sign of
     #: :attr:`~acoular.tprocess.Trigger.trigger_type` gives information
     #: on which edge should be used (+ for rising edge, - for falling edge).
     #: Sample will trigger if the difference between its value and its predecessors value
     #: is above/below the pos/neg threshold.
-    #: 
+    #:
     #: Default is 'dirac'.
     trigger_type = Trait('dirac', 'rect')
-    
+
     #: Identifier which peak to consider, if there are multiple peaks in one hunk
-    #: (see :attr:`~acoular.tprocess.Trigger.hunk_length`). Default is to 'extremum', 
+    #: (see :attr:`~acoular.tprocess.Trigger.hunk_length`). Default is to 'extremum',
     #: in which case the extremal peak (maximum if threshold > 0, minimum if threshold < 0) is considered.
     multiple_peaks_in_hunk = Trait('extremum', 'first')
-    
-    #: Tuple consisting of 3 entries: 
-    #: 
+
+    #: Tuple consisting of 3 entries:
+    #:
     #: 1.: -Vector with the sample indices of the 1/Rev trigger samples
-    #: 
+    #:
     #: 2.: -maximum of number of samples between adjacent trigger samples
-    #: 
+    #:
     #: 3.: -minimum of number of samples between adjacent trigger samples
-    trigger_data = Property(depends_on=['source.digest', 'threshold', 'max_variation_of_duration', \
-                                        'hunk_length', 'trigger_type', 'multiple_peaks_in_hunk'])
-    
+    trigger_data = Property(
+        depends_on=[
+            'source.digest',
+            'threshold',
+            'max_variation_of_duration',
+            'hunk_length',
+            'trigger_type',
+            'multiple_peaks_in_hunk',
+        ],
+    )
+
     # internal identifier
-    digest = Property(depends_on=['source.digest', 'threshold', 'max_variation_of_duration', \
-                                        'hunk_length', 'trigger_type', 'multiple_peaks_in_hunk'])
-    
+    digest = Property(
+        depends_on=[
+            'source.digest',
+            'threshold',
+            'max_variation_of_duration',
+            'hunk_length',
+            'trigger_type',
+            'multiple_peaks_in_hunk',
+        ],
+    )
+
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
-    
+
     @cached_property
     def _get_trigger_data(self):
         self._check_trigger_existence()
-        triggerFunc = {'dirac' : self._trigger_dirac,
-                       'rect' : self._trigger_rect}[self.trigger_type]
+        triggerFunc = {'dirac': self._trigger_dirac, 'rect': self._trigger_rect}[self.trigger_type]
         nSamples = 2048  # number samples for result-method of source
         threshold = self._threshold(nSamples)
-        
+
         # get all samples which surpasse the threshold
         peakLoc = array([], dtype='int')  # all indices which surpasse the threshold
         triggerData = array([])
         x0 = []
         dSamples = 0
         for triggerSignal in self.source.result(nSamples):
             localTrigger = flatnonzero(triggerFunc(x0, triggerSignal, threshold))
-            if not len(localTrigger) == 0:
+            if len(localTrigger) != 0:
                 peakLoc = append(peakLoc, localTrigger + dSamples)
                 triggerData = append(triggerData, triggerSignal[localTrigger])
             dSamples += nSamples
             x0 = triggerSignal[-1]
         if len(peakLoc) <= 1:
-            raise Exception('Not enough trigger info. Check *threshold* sign and value!')
+            msg = 'Not enough trigger info. Check *threshold* sign and value!'
+            raise Exception(msg)
 
         peakDist = peakLoc[1:] - peakLoc[:-1]
         maxPeakDist = max(peakDist)  # approximate distance between the revolutions
-        
-        # if there are hunks which contain multiple peaks -> check for each hunk, 
+
+        # if there are hunks which contain multiple peaks -> check for each hunk,
         # which peak is the correct one -> delete the other one.
-        # if there are no multiple peaks in any hunk left -> leave the while 
+        # if there are no multiple peaks in any hunk left -> leave the while
         # loop and continue with program
         multiplePeaksWithinHunk = flatnonzero(peakDist < self.hunk_length * maxPeakDist)
         while len(multiplePeaksWithinHunk) > 0:
             peakLocHelp = multiplePeaksWithinHunk[0]
             indHelp = [peakLocHelp, peakLocHelp + 1]
             if self.multiple_peaks_in_hunk == 'extremum':
                 values = triggerData[indHelp]
                 deleteInd = indHelp[argmin(abs(values))]
             elif self.multiple_peaks_in_hunk == 'first':
                 deleteInd = indHelp[1]
             peakLoc = delete(peakLoc, deleteInd)
             triggerData = delete(triggerData, deleteInd)
             peakDist = peakLoc[1:] - peakLoc[:-1]
             multiplePeaksWithinHunk = flatnonzero(peakDist < self.hunk_length * maxPeakDist)
-        
+
         # check whether distances between peaks are evenly distributed
         meanDist = mean(peakDist)
         diffDist = abs(peakDist - meanDist)
         faultyInd = flatnonzero(diffDist > self.max_variation_of_duration * meanDist)
         if faultyInd.size != 0:
-            warn('In Trigger-Identification: The distances between the peaks (and therefor the lengths of the revolutions) vary too much (check samples %s).' % str(peakLoc[faultyInd] + self.source.start), Warning, stacklevel = 2)
+            warn(
+                'In Trigger-Identification: The distances between the peaks (and therefor the lengths of the revolutions) vary too much (check samples %s).'
+                % str(peakLoc[faultyInd] + self.source.start),
+                Warning,
+                stacklevel=2,
+            )
         return peakLoc, max(peakDist), min(peakDist)
-    
+
     def _trigger_dirac(self, x0, x, threshold):
         # x0 not needed here, but needed in _trigger_rect
         return self._trigger_value_comp(x, threshold)
-    
+
     def _trigger_rect(self, x0, x, threshold):
         # x0 stores the last value of the the last generator cycle
         xNew = append(x0, x)
-       #indPeakHunk = abs(xNew[1:] - xNew[:-1]) > abs(threshold)  # with this line: every edge would be located
-        indPeakHunk = self._trigger_value_comp(xNew[1:] - xNew[:-1], threshold)
-        return indPeakHunk
-    
+        # indPeakHunk = abs(xNew[1:] - xNew[:-1]) > abs(threshold)  # with this line: every edge would be located
+        return self._trigger_value_comp(xNew[1:] - xNew[:-1], threshold)
+
     def _trigger_value_comp(self, triggerData, threshold):
-        if threshold > 0.0:
-            indPeaks= triggerData > threshold
-        else:
-            indPeaks = triggerData < threshold
-        return indPeaks
-    
+        return triggerData > threshold if threshold > 0.0 else triggerData < threshold
+
     def _threshold(self, nSamples):
-        if self.threshold == None:  # take a guessed threshold
+        if self.threshold is None:  # take a guessed threshold
             # get max and min values of whole trigger signal
             maxVal = -inf
             minVal = inf
             meanVal = 0
             cntMean = 0
             for triggerData in self.source.result(nSamples):
                 maxVal = max(maxVal, triggerData.max())
                 minVal = min(minVal, triggerData.min())
                 meanVal += triggerData.mean()
                 cntMean += 1
             meanVal /= cntMean
-            
+
             # get 75% of maximum absolute value of trigger signal
             maxTriggerHelp = [minVal, maxVal] - meanVal
             argInd = argmax(abs(maxTriggerHelp))
             thresh = maxTriggerHelp[argInd] * 0.75  # 0.75 for 75% of max trigger signal
-            warn('No threshold was passed. An estimated threshold of %s is assumed.' % thresh, Warning, stacklevel = 2)
+            warn('No threshold was passed. An estimated threshold of %s is assumed.' % thresh, Warning, stacklevel=2)
         else:  # take user defined  threshold
             thresh = self.threshold
         return thresh
-    
+
     def _check_trigger_existence(self):
         nChannels = self.source.numchannels
         if not nChannels == 1:
             raise Exception('Trigger signal must consist of ONE channel, instead %s channels are given!' % nChannels)
         return 0
 
+
 class AngleTracker(MaskedTimeInOut):
-    '''
-    Calculates rotation angle and rpm per sample from a trigger signal 
-    using spline interpolation in the time domain. 
-    
+    """Calculates rotation angle and rpm per sample from a trigger signal
+    using spline interpolation in the time domain.
+
     Gets samples from :attr:`trigger` and stores the angle and rpm samples in :meth:`angle` and :meth:`rpm`.
 
-    '''
+    """
 
     #: Data source; :class:`~acoular.tprocess.SamplesGenerator` or derived object.
-    source = Instance(SamplesGenerator)    
-    
+    source = Instance(SamplesGenerator)
+
     #: Trigger data from :class:`acoular.tprocess.Trigger`.
-    trigger = Instance(Trigger) 
-    
+    trigger = Instance(Trigger)
+
     # internal identifier
-    digest = Property(depends_on=['source.digest', 
-                                  'trigger.digest', 
-                                  'trigger_per_revo',
-                                  'rot_direction',
-                                  'interp_points',
-                                  'start_angle'])
-    
+    digest = Property(
+        depends_on=[
+            'source.digest',
+            'trigger.digest',
+            'trigger_per_revo',
+            'rot_direction',
+            'interp_points',
+            'start_angle',
+        ],
+    )
+
     #: Trigger signals per revolution,
     #: defaults to 1.
-    trigger_per_revo = Int(1,
-                   desc ="trigger signals per revolution")
-        
+    trigger_per_revo = Int(1, desc='trigger signals per revolution')
+
     #: Flag to set counter-clockwise (1) or clockwise (-1) rotation,
     #: defaults to -1.
-    rot_direction = Int(-1,
-                   desc ="mathematical direction of rotation")
-    
+    rot_direction = Int(-1, desc='mathematical direction of rotation')
+
     #: Points of interpolation used for spline,
     #: defaults to 4.
-    interp_points = Int(4,
-                   desc ="Points of interpolation used for spline")
-    
+    interp_points = Int(4, desc='Points of interpolation used for spline')
+
     #: rotation angle in radians for first trigger position
-    start_angle = Float(0,
-                   desc ="rotation angle for trigger position")
-    
+    start_angle = Float(0, desc='rotation angle for trigger position')
+
     #: revolutions per minute for each sample, read-only
-    rpm = Property( depends_on = 'digest', desc ="revolutions per minute for each sample")
-    
+    rpm = Property(depends_on='digest', desc='revolutions per minute for each sample')
+
     #: average revolutions per minute, read-only
-    average_rpm = Property( depends_on = 'digest', desc ="average revolutions per minute")      
-    
+    average_rpm = Property(depends_on='digest', desc='average revolutions per minute')
+
     #: rotation angle in radians for each sample, read-only
-    angle = Property( depends_on = 'digest', desc ="rotation angle for each sample")
-    
+    angle = Property(depends_on='digest', desc='rotation angle for each sample')
+
     # Internal flag to determine whether rpm and angle calculation has been processed,
     # prevents recalculation
-    _calc_flag = Bool(False) 
-    
+    _calc_flag = Bool(False)
+
     # Revolutions per minute, internal use
     _rpm = CArray()
-          
+
     # Rotation angle in radians, internal use
     _angle = CArray()
-    
 
-    
-    @cached_property 
-    def _get_digest( self ):
+    @cached_property
+    def _get_digest(self):
         return digest(self)
-    
-    #helperfunction for trigger index detection
+
+    # helperfunction for trigger index detection
     def _find_nearest_idx(self, peakarray, value):
         peakarray = asarray(peakarray)
-        idx = (abs(peakarray - value)).argmin()
-        return idx
-    
+        return (abs(peakarray - value)).argmin()
+
     def _to_rpm_and_angle(self):
-        """ 
-        Internal helper function 
+        """Internal helper function
         Calculates angles in radians for one or more instants in time.
-        
-        Current version supports only trigger and sources with the same samplefreq. 
-        This behaviour may change in future releases 
-        """
 
-        #init
-        ind=0
-        #trigger data
-        peakloc,maxdist,mindist= self.trigger._get_trigger_data()
-        TriggerPerRevo= self.trigger_per_revo
+        Current version supports only trigger and sources with the same samplefreq.
+        This behaviour may change in future releases
+        """
+        # init
+        ind = 0
+        # trigger data
+        peakloc, maxdist, mindist = self.trigger._get_trigger_data()
+        TriggerPerRevo = self.trigger_per_revo
         rotDirection = self.rot_direction
-        nSamples =  self.source.numsamples
-        samplerate =  self.source.sample_freq
+        nSamples = self.source.numsamples
+        samplerate = self.source.sample_freq
         self._rpm = zeros(nSamples)
         self._angle = zeros(nSamples)
-        #number of spline points
-        InterpPoints=self.interp_points
-        
-        #loop over alle timesamples
-        while ind < nSamples :     
-            #when starting spline forward
-            if ind<peakloc[InterpPoints]:
-                peakdist=peakloc[self._find_nearest_idx(peakarray= peakloc,value=ind)+1] - peakloc[self._find_nearest_idx(peakarray= peakloc,value=ind)]
-                splineData = stack((range(InterpPoints), peakloc[ind//peakdist:ind//peakdist+InterpPoints]), axis=0)
-            #spline backwards    
+        # number of spline points
+        InterpPoints = self.interp_points
+
+        # loop over alle timesamples
+        while ind < nSamples:
+            # when starting spline forward
+            if ind < peakloc[InterpPoints]:
+                peakdist = (
+                    peakloc[self._find_nearest_idx(peakarray=peakloc, value=ind) + 1]
+                    - peakloc[self._find_nearest_idx(peakarray=peakloc, value=ind)]
+                )
+                splineData = stack(
+                    (range(InterpPoints), peakloc[ind // peakdist : ind // peakdist + InterpPoints]),
+                    axis=0,
+                )
+            # spline backwards
             else:
-                peakdist=peakloc[self._find_nearest_idx(peakarray= peakloc,value=ind)] - peakloc[self._find_nearest_idx(peakarray= peakloc,value=ind)-1]
-                splineData = stack((range(InterpPoints), peakloc[ind//peakdist-InterpPoints:ind//peakdist]), axis=0)
-            #calc angles and rpm    
-            Spline = splrep(splineData[:,:][1], splineData[:,:][0], k=3)    
-            self._rpm[ind]=splev(ind, Spline, der=1, ext=0)*60*samplerate
-            self._angle[ind] = (splev(ind, Spline, der=0, ext=0)*2*pi*rotDirection/TriggerPerRevo + self.start_angle) % (2*pi)
-            #next sample
-            ind+=1
-        #calculation complete    
+                peakdist = (
+                    peakloc[self._find_nearest_idx(peakarray=peakloc, value=ind)]
+                    - peakloc[self._find_nearest_idx(peakarray=peakloc, value=ind) - 1]
+                )
+                splineData = stack(
+                    (range(InterpPoints), peakloc[ind // peakdist - InterpPoints : ind // peakdist]),
+                    axis=0,
+                )
+            # calc angles and rpm
+            Spline = splrep(splineData[:, :][1], splineData[:, :][0], k=3)
+            self._rpm[ind] = splev(ind, Spline, der=1, ext=0) * 60 * samplerate
+            self._angle[ind] = (
+                splev(ind, Spline, der=0, ext=0) * 2 * pi * rotDirection / TriggerPerRevo + self.start_angle
+            ) % (2 * pi)
+            # next sample
+            ind += 1
+        # calculation complete
         self._calc_flag = True
-    
+
     # reset calc flag if something has changed
     @on_trait_change('digest')
-    def _reset_calc_flag( self ):
+    def _reset_calc_flag(self):
         self._calc_flag = False
-    
-    #calc rpm from trigger data
+
+    # calc rpm from trigger data
     @cached_property
-    def _get_rpm( self ):
+    def _get_rpm(self):
         if not self._calc_flag:
             self._to_rpm_and_angle()
         return self._rpm
 
-    #calc of angle from trigger data
+    # calc of angle from trigger data
     @cached_property
     def _get_angle(self):
         if not self._calc_flag:
             self._to_rpm_and_angle()
         return self._angle
 
-    #calc average rpm from trigger data
+    # calc average rpm from trigger data
     @cached_property
-    def _get_average_rpm( self ):
-        """ 
-        Returns average revolutions per minute (rpm) over the source samples.
-    
+    def _get_average_rpm(self):
+        """Returns average revolutions per minute (rpm) over the source samples.
+
         Returns
         -------
         rpm : float
             rpm in 1/min.
+
         """
-        #trigger indices data
+        # trigger indices data
         peakloc = self.trigger._get_trigger_data()[0]
-        #calculation of average rpm in 1/min
-        return (len(peakloc)-1) / (peakloc[-1]-peakloc[0]) / self.trigger_per_revo * self.source.sample_freq * 60
+        # calculation of average rpm in 1/min
+        return (len(peakloc) - 1) / (peakloc[-1] - peakloc[0]) / self.trigger_per_revo * self.source.sample_freq * 60
+
 
 class SpatialInterpolator(TimeInOut):
+    """Base class for spatial interpolation of microphone data.
+    Gets samples from :attr:`source` and generates output via the
+    generator :meth:`result`.
     """
-    Base class for spatial interpolation of microphone data.
-    Gets samples from :attr:`source` and generates output via the 
-    generator :meth:`result`
-    """
+
     #: :class:`~acoular.microphones.MicGeom` object that provides the real microphone locations.
-    mics = Instance(MicGeom(), 
-        desc="microphone geometry")
-    
+    mics = Instance(MicGeom(), desc='microphone geometry')
+
     #: :class:`~acoular.microphones.MicGeom` object that provides the virtual microphone locations.
-    mics_virtual = Property(
-        desc="microphone geometry")
-    
-    _mics_virtual = Instance(MicGeom,
-        desc="internal microphone geometry;internal usage, read only")
-        
+    mics_virtual = Property(desc='microphone geometry')
+
+    _mics_virtual = Instance(MicGeom, desc='internal microphone geometry;internal usage, read only')
+
     def _get_mics_virtual(self):
         if not self._mics_virtual and self.mics:
             self._mics_virtual = self.mics
         return self._mics_virtual
-    
+
     def _set_mics_virtual(self, mics_virtual):
         self._mics_virtual = mics_virtual
 
-    
     #: Data source; :class:`~acoular.tprocess.SamplesGenerator` or derived object.
     source = Instance(SamplesGenerator)
-    
+
     #: Interpolation method in spacial domain, defaults to linear
     #: linear uses numpy linear interpolation
     #: spline uses scipy CloughTocher algorithm
     #: rbf is scipy radial basis function with multiquadric, cubic and sinc functions
-    #: idw refers to the inverse distance weighting algorithm 
-    method = Trait('linear', 'spline', 'rbf-multiquadric', 'rbf-cubic','IDW',\
-        'custom', 'sinc', desc="method for interpolation used")
-    
+    #: idw refers to the inverse distance weighting algorithm
+    method = Trait(
+        'linear',
+        'spline',
+        'rbf-multiquadric',
+        'rbf-cubic',
+        'IDW',
+        'custom',
+        'sinc',
+        desc='method for interpolation used',
+    )
+
     #: spacial dimensionality of the array geometry
-    array_dimension= Trait('1D', '2D',  \
-        'ring', '3D', 'custom', desc="spacial dimensionality of the array geometry")
-    
+    array_dimension = Trait('1D', '2D', 'ring', '3D', 'custom', desc='spacial dimensionality of the array geometry')
+
     #: Sampling frequency of output signal, as given by :attr:`source`.
     sample_freq = Delegate('source', 'sample_freq')
-    
+
     #: Number of channels in output.
     numchannels = Property()
-    
+
     #: Number of samples in output, as given by :attr:`source`.
     numsamples = Delegate('source', 'numsamples')
-    
 
-    #:Interpolate a point at the origin of the Array geometry 
-    interp_at_zero =  Bool(False)
+    #:Interpolate a point at the origin of the Array geometry
+    interp_at_zero = Bool(False)
 
     #: The rotation must be around the z-axis, which means from x to y axis.
-    #: If the coordinates are not build like that, than this 3x3 orthogonal 
+    #: If the coordinates are not build like that, than this 3x3 orthogonal
     #: transformation matrix Q can be used to modify the coordinates.
-    #: It is assumed that with the modified coordinates the rotation is around the z-axis. 
+    #: It is assumed that with the modified coordinates the rotation is around the z-axis.
     #: The transformation is done via [x,y,z]_mod = Q * [x,y,z]. (default is Identity).
     Q = CArray(dtype=float64, shape=(3, 3), value=identity(3))
-    
-    num_IDW= Trait(3,dtype = int, \
-                    desc='number of neighboring microphones, DEFAULT=3')
 
-    p_weight = Trait(2,dtype = float,\
-                desc='used in interpolation for virtual microphone, weighting power exponent for IDW')
+    num_IDW = Trait(3, dtype=int, desc='number of neighboring microphones, DEFAULT=3')
 
+    p_weight = Trait(
+        2,
+        dtype=float,
+        desc='used in interpolation for virtual microphone, weighting power exponent for IDW',
+    )
 
     #: Stores the output of :meth:`_virtNewCoord_func`; Read-Only
-    _virtNewCoord_func = Property(depends_on=['mics.digest',
-                                              'mics_virtual.digest',
-                                              'method','array_dimension',
-                                              'interp_at_zero'])
-    
+    _virtNewCoord_func = Property(
+        depends_on=['mics.digest', 'mics_virtual.digest', 'method', 'array_dimension', 'interp_at_zero'],
+    )
+
     #: internal identifier
-    digest = Property(depends_on=['mics.digest', 'mics_virtual.digest', 'source.digest', \
-                                   'method','array_dimension', 'Q', 'interp_at_zero'])
-    
+    digest = Property(
+        depends_on=[
+            'mics.digest',
+            'mics_virtual.digest',
+            'source.digest',
+            'method',
+            'array_dimension',
+            'Q',
+            'interp_at_zero',
+        ],
+    )
+
     def _get_numchannels(self):
         return self.mics_virtual.num_mics
-    
+
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
-    
+
     @cached_property
     def _get_virtNewCoord(self):
-        return self._virtNewCoord_func(self.mics.mpos, self.mics_virtual.mpos,self.method, self.array_dimension)
-        
-    
+        return self._virtNewCoord_func(self.mics.mpos, self.mics_virtual.mpos, self.method, self.array_dimension)
+
     def sinc_mic(self, r):
-        """ 
-        Modified Sinc function for Radial Basis function approximation
-        
-        """
-        return sinc((r*self.mics_virtual.mpos.shape[1])/(pi))    
-    
-    def _virtNewCoord_func(self, mic, micVirt, method ,array_dimension, interp_at_zero = False):
-        """ 
-        Core functionality for getting the  interpolation .
-        
+        """Modified Sinc function for Radial Basis function approximation."""
+        return sinc((r * self.mics_virtual.mpos.shape[1]) / (pi))
+
+    def _virtNewCoord_func(self, mic, micVirt, method, array_dimension):
+        """Core functionality for getting the  interpolation .
+
         Parameters
         ----------
         mic : float[3, nPhysicalMics]
             The mic positions of the physical (really existing) mics
         micVirt : float[3, nVirtualMics]
             The mic positions of the virtual mics
         method : string
-            The Interpolation method to use     
+            The Interpolation method to use
         array_dimension : string
             The Array Dimensions in cylinder coordinates
 
         Returns
         -------
         mesh : List[]
             The items of these lists are dependent of the reduced interpolation dimension of each subarray.
@@ -790,894 +851,914 @@
                     correspond to their initial pressure values
             If the Array is 2D or 3d the list items are:
                 1. item : Delaunay mesh object
                     Delauney mesh (see scipy.spatial.Delaunay) for the specific Array
                 2. item : int64[nMicsInArray]
                     same as 1d case, BUT with the difference, that here the rotational periodicy is handled, when constructing the mesh.
                     Therefor the mesh could have more vertices than the actual Array mics.
-                    
+
         virtNewCoord : float64[3, nVirtualMics]
             Projection of each virtual mic onto its new coordinates. The columns of virtNewCoord correspond to [phi, rho, z]
-            
+
         newCoord : float64[3, nMics]
             Projection of each mic onto its new coordinates. The columns of newCoordinates correspond to [phi, rho, z]
-        """     
+
+        """
         # init positions of virtual mics in cyl coordinates
         nVirtMics = micVirt.shape[1]
         virtNewCoord = zeros((3, nVirtMics))
         virtNewCoord.fill(nan)
-        #init real positions in cyl coordinates
+        # init real positions in cyl coordinates
         nMics = mic.shape[1]
         newCoord = zeros((3, nMics))
         newCoord.fill(nan)
-        #empty mesh object
+        # empty mesh object
         mesh = []
-        
-        if self.array_dimension =='1D' or self.array_dimension =='ring':
-                # get projections onto new coordinate, for real mics
-                projectionOnNewAxis = cartToCyl(mic,self.Q)[0]
-                indReorderHelp = argsort(projectionOnNewAxis)
-                mesh.append([projectionOnNewAxis[indReorderHelp], indReorderHelp])
-               
-                #new coordinates of real mics
-                indReorderHelp = argsort(cartToCyl(mic,self.Q)[0])
-                newCoord = (cartToCyl(mic,self.Q).T)[indReorderHelp].T
-
-                # and for virtual mics
-                virtNewCoord = cartToCyl(micVirt)
-                
-        elif self.array_dimension =='2D':  # 2d case0
 
+        if self.array_dimension == '1D' or self.array_dimension == 'ring':
+            # get projections onto new coordinate, for real mics
+            projectionOnNewAxis = cartToCyl(mic, self.Q)[0]
+            indReorderHelp = argsort(projectionOnNewAxis)
+            mesh.append([projectionOnNewAxis[indReorderHelp], indReorderHelp])
+
+            # new coordinates of real mics
+            indReorderHelp = argsort(cartToCyl(mic, self.Q)[0])
+            newCoord = (cartToCyl(mic, self.Q).T)[indReorderHelp].T
+
+            # and for virtual mics
+            virtNewCoord = cartToCyl(micVirt)
+
+        elif self.array_dimension == '2D':  # 2d case0
             # get virtual mic projections on new coord system
-            virtNewCoord = cartToCyl(micVirt,self.Q)
-            
-            #new coordinates of real mics
-            indReorderHelp = argsort(cartToCyl(mic,self.Q)[0])
-            newCoord = cartToCyl(mic,self.Q) 
-            
-            #scipy delauney triangulation            
-            #Delaunay
-            tri = Delaunay(newCoord.T[:,:2], incremental=True) #
-            
-            
+            virtNewCoord = cartToCyl(micVirt, self.Q)
+
+            # new coordinates of real mics
+            indReorderHelp = argsort(cartToCyl(mic, self.Q)[0])
+            newCoord = cartToCyl(mic, self.Q)
+
+            # scipy delauney triangulation
+            # Delaunay
+            tri = Delaunay(newCoord.T[:, :2], incremental=True)  #
+
             if self.interp_at_zero:
-                #add a point at zero 
-                tri.add_points(array([[0 ], [0]]).T)
-            
-            # extend mesh with closest boundary points of repeating mesh 
+                # add a point at zero
+                tri.add_points(array([[0], [0]]).T)
+
+            # extend mesh with closest boundary points of repeating mesh
             pointsOriginal = arange(tri.points.shape[0])
             hull = tri.convex_hull
             hullPoints = unique(hull)
-                    
+
             addRight = tri.points[hullPoints]
-            addRight[:, 0] += 2*pi
-            addLeft= tri.points[hullPoints]
-            addLeft[:, 0] -= 2*pi
-            
+            addRight[:, 0] += 2 * pi
+            addLeft = tri.points[hullPoints]
+            addLeft[:, 0] -= 2 * pi
+
             indOrigPoints = concatenate((pointsOriginal, pointsOriginal[hullPoints], pointsOriginal[hullPoints]))
-            # add all hull vertices to original mesh and check which of those 
+            # add all hull vertices to original mesh and check which of those
             # are actual neighbors of the original array. Cancel out all others.
             tri.add_points(concatenate([addLeft, addRight]))
             indices, indptr = tri.vertex_neighbor_vertices
             hullNeighbor = empty((0), dtype='int32')
             for currHull in hullPoints:
-                neighborOfHull = indptr[indices[currHull]:indices[currHull + 1]]
+                neighborOfHull = indptr[indices[currHull] : indices[currHull + 1]]
                 hullNeighbor = append(hullNeighbor, neighborOfHull)
             hullNeighborUnique = unique(hullNeighbor)
             pointsNew = unique(append(pointsOriginal, hullNeighborUnique))
             tri = Delaunay(tri.points[pointsNew])  # re-meshing
             mesh.append([tri, indOrigPoints[pointsNew]])
-            
-            
-            
-        elif self.array_dimension =='3D':  # 3d case
-            
+
+        elif self.array_dimension == '3D':  # 3d case
             # get virtual mic projections on new coord system
-            virtNewCoord = cartToCyl(micVirt,self.Q)
+            virtNewCoord = cartToCyl(micVirt, self.Q)
             # get real mic projections on new coord system
-            indReorderHelp = argsort(cartToCyl(mic,self.Q)[0])
-            newCoord = (cartToCyl(mic,self.Q))
-            #Delaunay
-            tri =Delaunay(newCoord.T, incremental=True) #, incremental=True,qhull_options =  "Qc QJ Q12" 
+            indReorderHelp = argsort(cartToCyl(mic, self.Q)[0])
+            newCoord = cartToCyl(mic, self.Q)
+            # Delaunay
+            tri = Delaunay(newCoord.T, incremental=True)  # , incremental=True,qhull_options =  "Qc QJ Q12"
 
             if self.interp_at_zero:
-                #add a point at zero 
-                tri.add_points(array([[0 ], [0], [0]]).T)
+                # add a point at zero
+                tri.add_points(array([[0], [0], [0]]).T)
 
-            # extend mesh with closest boundary points of repeating mesh 
+            # extend mesh with closest boundary points of repeating mesh
             pointsOriginal = arange(tri.points.shape[0])
             hull = tri.convex_hull
             hullPoints = unique(hull)
-        
+
             addRight = tri.points[hullPoints]
-            addRight[:, 0] += 2*pi
-            addLeft= tri.points[hullPoints]
-            addLeft[:, 0] -= 2*pi
-            
+            addRight[:, 0] += 2 * pi
+            addLeft = tri.points[hullPoints]
+            addLeft[:, 0] -= 2 * pi
+
             indOrigPoints = concatenate((pointsOriginal, pointsOriginal[hullPoints], pointsOriginal[hullPoints]))
-            # add all hull vertices to original mesh and check which of those 
+            # add all hull vertices to original mesh and check which of those
             # are actual neighbors of the original array. Cancel out all others.
             tri.add_points(concatenate([addLeft, addRight]))
             indices, indptr = tri.vertex_neighbor_vertices
             hullNeighbor = empty((0), dtype='int32')
             for currHull in hullPoints:
-                neighborOfHull = indptr[indices[currHull]:indices[currHull + 1]]
+                neighborOfHull = indptr[indices[currHull] : indices[currHull + 1]]
                 hullNeighbor = append(hullNeighbor, neighborOfHull)
             hullNeighborUnique = unique(hullNeighbor)
             pointsNew = unique(append(pointsOriginal, hullNeighborUnique))
             tri = Delaunay(tri.points[pointsNew])  # re-meshing
             mesh.append([tri, indOrigPoints[pointsNew]])
-         
-        return  mesh, virtNewCoord , newCoord
-    
 
-    def _result_core_func(self, p, phiDelay=[], period=None, Q=Q, interp_at_zero = False):
-        """
-        Performs the actual Interpolation
-        
+        return mesh, virtNewCoord, newCoord
+
+    def _result_core_func(self, p, phiDelay=None, period=None, Q=Q, interp_at_zero=False):
+        """Performs the actual Interpolation.
+
         Parameters
         ----------
         p : float[nSamples, nMicsReal]
             The pressure field of the yielded sample at real mics.
-        phiDelay : empty list (default) or float[nSamples] 
-            If passed (rotational case), this list contains the angular delay 
+        phiDelay : empty list (default) or float[nSamples]
+            If passed (rotational case), this list contains the angular delay
             of each sample in rad.
         period : None (default) or float
-            If periodicity can be assumed (rotational case) 
+            If periodicity can be assumed (rotational case)
             this parameter contains the periodicity length
-        
+
         Returns
         -------
         pInterp : float[nSamples, nMicsVirtual]
             The interpolated time data at the virtual mics
+
         """
-        
-        #number of time samples
+        if phiDelay is None:
+            phiDelay = []
+        # number of time samples
         nTime = p.shape[0]
-        #number of virtual mixcs 
+        # number of virtual mixcs
         nVirtMics = self.mics_virtual.mpos.shape[1]
         # mesh and projection onto polar Coordinates
         meshList, virtNewCoord, newCoord = self._get_virtNewCoord()
-        # pressure interpolation init     
-        pInterp = zeros((nTime,nVirtMics))
-        #Coordinates in cartesian CO - for IDW interpolation
-        newCoordCart=cylToCart(newCoord)
-        
+        # pressure interpolation init
+        pInterp = zeros((nTime, nVirtMics))
+        # Coordinates in cartesian CO - for IDW interpolation
+        newCoordCart = cylToCart(newCoord)
+
         if self.interp_at_zero:
-            #interpolate point at 0 in Kartesian CO
-            interpolater = LinearNDInterpolator(cylToCart(newCoord[:,argsort(newCoord[0])])[:2,:].T,
-                                            p[:, (argsort(newCoord[0]))].T, fill_value = 0)
-            pZero  = interpolater((0,0))
-            #add the interpolated pressure at origin to pressure channels
+            # interpolate point at 0 in Kartesian CO
+            interpolater = LinearNDInterpolator(
+                cylToCart(newCoord[:, argsort(newCoord[0])])[:2, :].T,
+                p[:, (argsort(newCoord[0]))].T,
+                fill_value=0,
+            )
+            pZero = interpolater((0, 0))
+            # add the interpolated pressure at origin to pressure channels
             p = concatenate((p, pZero[:, newaxis]), axis=1)
 
-        
-        #helpfunction reordered for reordered pressure values 
+        # helpfunction reordered for reordered pressure values
         pHelp = p[:, meshList[0][1]]
-        
-        # Interpolation for 1D Arrays 
-        if self.array_dimension =='1D' or self.array_dimension =='ring':
-            #for rotation add phidelay
-            if not array_equal(phiDelay,[]):
+
+        # Interpolation for 1D Arrays
+        if self.array_dimension == '1D' or self.array_dimension == 'ring':
+            # for rotation add phidelay
+            if not array_equal(phiDelay, []):
                 xInterpHelp = repmat(virtNewCoord[0, :], nTime, 1) + repmat(phiDelay, virtNewCoord.shape[1], 1).T
-                xInterp = ((xInterpHelp + pi ) % (2 * pi)) - pi #  shifting phi cootrdinate into feasible area [-pi, pi]
-            #if no rotation given
+                xInterp = ((xInterpHelp + pi) % (2 * pi)) - pi  #  shifting phi cootrdinate into feasible area [-pi, pi]
+            # if no rotation given
             else:
                 xInterp = repmat(virtNewCoord[0, :], nTime, 1)
-            #get ordered microphone posions in radiant
+            # get ordered microphone posions in radiant
             x = newCoord[0]
             for cntTime in range(nTime):
-                
                 if self.method == 'linear':
-                    #numpy 1-d interpolation
-                    pInterp[cntTime] = interp(xInterp[cntTime, :], x, pHelp[cntTime, :], period=period, left=nan, right=nan)
-                    
-                    
+                    # numpy 1-d interpolation
+                    pInterp[cntTime] = interp(
+                        xInterp[cntTime, :],
+                        x,
+                        pHelp[cntTime, :],
+                        period=period,
+                        left=nan,
+                        right=nan,
+                    )
+
                 elif self.method == 'spline':
-                    #scipy cubic spline interpolation
-                    SplineInterp = CubicSpline(append(x,(2*pi)+x[0]), append(pHelp[cntTime, :],pHelp[cntTime, :][0]), axis=0, bc_type='periodic', extrapolate=None)
-                    pInterp[cntTime] = SplineInterp(xInterp[cntTime, :])    
-                    
+                    # scipy cubic spline interpolation
+                    SplineInterp = CubicSpline(
+                        append(x, (2 * pi) + x[0]),
+                        append(pHelp[cntTime, :], pHelp[cntTime, :][0]),
+                        axis=0,
+                        bc_type='periodic',
+                        extrapolate=None,
+                    )
+                    pInterp[cntTime] = SplineInterp(xInterp[cntTime, :])
+
                 elif self.method == 'sinc':
-                    #compute using 3-D Rbfs for sinc
-                    rbfi = Rbf(x,newCoord[1],
-                                 newCoord[2] ,
-                                 pHelp[cntTime, :], function=self.sinc_mic)  # radial basis function interpolator instance
-                    
-                    pInterp[cntTime] = rbfi(xInterp[cntTime, :],
-                                            virtNewCoord[1],
-                                            virtNewCoord[2]) 
-                    
+                    # compute using 3-D Rbfs for sinc
+                    rbfi = Rbf(
+                        x,
+                        newCoord[1],
+                        newCoord[2],
+                        pHelp[cntTime, :],
+                        function=self.sinc_mic,
+                    )  # radial basis function interpolator instance
+
+                    pInterp[cntTime] = rbfi(xInterp[cntTime, :], virtNewCoord[1], virtNewCoord[2])
+
                 elif self.method == 'rbf-cubic':
-                    #compute using 3-D Rbfs with multiquadratics
-                    rbfi = Rbf(x,newCoord[1],
-                                 newCoord[2] ,
-                                 pHelp[cntTime, :], function='cubic')  # radial basis function interpolator instance
-                    
-                    pInterp[cntTime] = rbfi(xInterp[cntTime, :],
-                                            virtNewCoord[1],
-                                            virtNewCoord[2]) 
-                    
-        
+                    # compute using 3-D Rbfs with multiquadratics
+                    rbfi = Rbf(
+                        x,
+                        newCoord[1],
+                        newCoord[2],
+                        pHelp[cntTime, :],
+                        function='cubic',
+                    )  # radial basis function interpolator instance
+
+                    pInterp[cntTime] = rbfi(xInterp[cntTime, :], virtNewCoord[1], virtNewCoord[2])
+
         # Interpolation for arbitrary 2D Arrays
-        elif self.array_dimension =='2D':
-            #check rotation
-            if not array_equal(phiDelay,[]):
+        elif self.array_dimension == '2D':
+            # check rotation
+            if not array_equal(phiDelay, []):
                 xInterpHelp = repmat(virtNewCoord[0, :], nTime, 1) + repmat(phiDelay, virtNewCoord.shape[1], 1).T
-                xInterp = ((xInterpHelp + pi ) % (2 * pi)) - pi #shifting phi cootrdinate into feasible area [-pi, pi]
+                xInterp = ((xInterpHelp + pi) % (2 * pi)) - pi  # shifting phi cootrdinate into feasible area [-pi, pi]
             else:
-                xInterp = repmat(virtNewCoord[0, :], nTime, 1)  
-                
-            mesh = meshList[0][0]
-            for cntTime in range(nTime):    
+                xInterp = repmat(virtNewCoord[0, :], nTime, 1)
 
+            mesh = meshList[0][0]
+            for cntTime in range(nTime):
                 # points for interpolation
-                newPoint = concatenate((xInterp[cntTime, :][:, newaxis], virtNewCoord[1, :][:, newaxis]), axis=1) 
-                #scipy 1D interpolation
+                newPoint = concatenate((xInterp[cntTime, :][:, newaxis], virtNewCoord[1, :][:, newaxis]), axis=1)
+                # scipy 1D interpolation
                 if self.method == 'linear':
-                    interpolater = LinearNDInterpolator(mesh, pHelp[cntTime, :], fill_value = 0)
-                    pInterp[cntTime] = interpolater(newPoint)    
-                    
+                    interpolater = LinearNDInterpolator(mesh, pHelp[cntTime, :], fill_value=0)
+                    pInterp[cntTime] = interpolater(newPoint)
+
                 elif self.method == 'spline':
                     # scipy CloughTocher interpolation
-                    f = CloughTocher2DInterpolator(mesh, pHelp[cntTime, :], fill_value = 0)
-                    pInterp[cntTime] = f(newPoint)    
-                    
+                    f = CloughTocher2DInterpolator(mesh, pHelp[cntTime, :], fill_value=0)
+                    pInterp[cntTime] = f(newPoint)
+
                 elif self.method == 'sinc':
-                    #compute using 3-D Rbfs for sinc
-                    rbfi = Rbf(newCoord[0],
-                               newCoord[1],
-                               newCoord[2] ,
-                                 pHelp[cntTime, :len(newCoord[0])], function=self.sinc_mic)  # radial basis function interpolator instance
-                    
-                    pInterp[cntTime] = rbfi(xInterp[cntTime, :],
-                                            virtNewCoord[1],
-                                            virtNewCoord[2]) 
-                    
-                    
+                    # compute using 3-D Rbfs for sinc
+                    rbfi = Rbf(
+                        newCoord[0],
+                        newCoord[1],
+                        newCoord[2],
+                        pHelp[cntTime, : len(newCoord[0])],
+                        function=self.sinc_mic,
+                    )  # radial basis function interpolator instance
+
+                    pInterp[cntTime] = rbfi(xInterp[cntTime, :], virtNewCoord[1], virtNewCoord[2])
+
                 elif self.method == 'rbf-cubic':
-                    #compute using 3-D Rbfs
-                    rbfi = Rbf( newCoord[0],
-                                newCoord[1],
-                                newCoord[2],
-                               pHelp[cntTime, :len(newCoord[0])], function='cubic')  # radial basis function interpolator instance
-                    
-                    virtshiftcoord= array([xInterp[cntTime, :],virtNewCoord[1], virtNewCoord[2]])
-                    pInterp[cntTime] = rbfi(virtshiftcoord[0],
-                                            virtshiftcoord[1],
-                                            virtshiftcoord[2]) 
-                
+                    # compute using 3-D Rbfs
+                    rbfi = Rbf(
+                        newCoord[0],
+                        newCoord[1],
+                        newCoord[2],
+                        pHelp[cntTime, : len(newCoord[0])],
+                        function='cubic',
+                    )  # radial basis function interpolator instance
+
+                    virtshiftcoord = array([xInterp[cntTime, :], virtNewCoord[1], virtNewCoord[2]])
+                    pInterp[cntTime] = rbfi(virtshiftcoord[0], virtshiftcoord[1], virtshiftcoord[2])
+
                 elif self.method == 'rbf-multiquadric':
-                    #compute using 3-D Rbfs
-                    rbfi = Rbf(newCoord[0],
-                               newCoord[1],
-                               newCoord[2],
-                               pHelp[cntTime, :len(newCoord[0])], function='multiquadric')  # radial basis function interpolator instance
-                    
-                    virtshiftcoord= array([xInterp[cntTime, :],virtNewCoord[1], virtNewCoord[2]])
-                    pInterp[cntTime] = rbfi(virtshiftcoord[0],
-                                            virtshiftcoord[1],
-                                            virtshiftcoord[2])        
+                    # compute using 3-D Rbfs
+                    rbfi = Rbf(
+                        newCoord[0],
+                        newCoord[1],
+                        newCoord[2],
+                        pHelp[cntTime, : len(newCoord[0])],
+                        function='multiquadric',
+                    )  # radial basis function interpolator instance
+
+                    virtshiftcoord = array([xInterp[cntTime, :], virtNewCoord[1], virtNewCoord[2]])
+                    pInterp[cntTime] = rbfi(virtshiftcoord[0], virtshiftcoord[1], virtshiftcoord[2])
                 # using inverse distance weighting
-                elif self.method=='IDW':                
+                elif self.method == 'IDW':
                     newPoint2_M = newPoint.T
-                    newPoint3_M = append(newPoint2_M,zeros([1,self.numchannels]),axis=0)
+                    newPoint3_M = append(newPoint2_M, zeros([1, self.numchannels]), axis=0)
                     newPointCart = cylToCart(newPoint3_M)
-                    for ind in arange(len(newPoint[:,0])):
-                        newPoint_Rep = repmat(newPointCart[:,ind], len(newPoint[:,0]),1).T  
+                    for ind in arange(len(newPoint[:, 0])):
+                        newPoint_Rep = repmat(newPointCart[:, ind], len(newPoint[:, 0]), 1).T
                         subtract = newPoint_Rep - newCoordCart
-                        normDistance = norm(subtract,axis=0)
-                        index_norm = argsort(normDistance)[:self.num_IDW]
-                        pHelpNew = pHelp[cntTime,index_norm]
+                        normDistance = norm(subtract, axis=0)
+                        index_norm = argsort(normDistance)[: self.num_IDW]
+                        pHelpNew = pHelp[cntTime, index_norm]
                         normNew = normDistance[index_norm]
                         if normNew[0] < 1e-3:
-                            pInterp[cntTime,ind] = pHelpNew[0]
+                            pInterp[cntTime, ind] = pHelpNew[0]
                         else:
-                            wholeD = sum((1 / normNew ** self.p_weight))
-                            weight = (1 / normNew ** self.p_weight) / wholeD
-                            weight_sum = sum(weight)
-                            pInterp[cntTime,ind] = sum(pHelpNew * weight)
-                 
-                                 
-        # Interpolation for arbitrary 3D Arrays             
-        elif self.array_dimension =='3D':
-            #check rotation
-            if not array_equal(phiDelay,[]):
+                            wholeD = sum(1 / normNew**self.p_weight)
+                            weight = (1 / normNew**self.p_weight) / wholeD
+                            pInterp[cntTime, ind] = sum(pHelpNew * weight)
+
+        # Interpolation for arbitrary 3D Arrays
+        elif self.array_dimension == '3D':
+            # check rotation
+            if not array_equal(phiDelay, []):
                 xInterpHelp = repmat(virtNewCoord[0, :], nTime, 1) + repmat(phiDelay, virtNewCoord.shape[1], 1).T
-                xInterp = ((xInterpHelp + pi  ) % (2 * pi)) - pi  #shifting phi cootrdinate into feasible area [-pi, pi]
+                xInterp = ((xInterpHelp + pi) % (2 * pi)) - pi  # shifting phi cootrdinate into feasible area [-pi, pi]
             else:
-                xInterp = repmat(virtNewCoord[0, :], nTime, 1)  
-                
+                xInterp = repmat(virtNewCoord[0, :], nTime, 1)
+
             mesh = meshList[0][0]
             for cntTime in range(nTime):
                 # points for interpolation
                 newPoint = concatenate((xInterp[cntTime, :][:, newaxis], virtNewCoord[1:, :].T), axis=1)
-                
-                if self.method == 'linear':     
-                    interpolater = LinearNDInterpolator(mesh, pHelp[cntTime, :], fill_value = 0)
+
+                if self.method == 'linear':
+                    interpolater = LinearNDInterpolator(mesh, pHelp[cntTime, :], fill_value=0)
                     pInterp[cntTime] = interpolater(newPoint)
-                
+
                 elif self.method == 'sinc':
-                    #compute using 3-D Rbfs for sinc
-                    rbfi = Rbf(newCoord[0],
-                               newCoord[1],
-                               newCoord[2],
-                                 pHelp[cntTime, :len(newCoord[0])], function=self.sinc_mic)  # radial basis function interpolator instance
-                    
-                    pInterp[cntTime] = rbfi(xInterp[cntTime, :],
-                                            virtNewCoord[1],
-                                            virtNewCoord[2]) 
-                                       
+                    # compute using 3-D Rbfs for sinc
+                    rbfi = Rbf(
+                        newCoord[0],
+                        newCoord[1],
+                        newCoord[2],
+                        pHelp[cntTime, : len(newCoord[0])],
+                        function=self.sinc_mic,
+                    )  # radial basis function interpolator instance
+
+                    pInterp[cntTime] = rbfi(xInterp[cntTime, :], virtNewCoord[1], virtNewCoord[2])
+
                 elif self.method == 'rbf-cubic':
-                    #compute using 3-D Rbfs
-                    rbfi = Rbf(newCoord[0],
-                               newCoord[1],
-                               newCoord[2],
-                               pHelp[cntTime, :len(newCoord[0])], function='cubic')  # radial basis function interpolator instance
-                    
-                    pInterp[cntTime] = rbfi(xInterp[cntTime, :],
-                                            virtNewCoord[1],
-                                            virtNewCoord[2])
-                
+                    # compute using 3-D Rbfs
+                    rbfi = Rbf(
+                        newCoord[0],
+                        newCoord[1],
+                        newCoord[2],
+                        pHelp[cntTime, : len(newCoord[0])],
+                        function='cubic',
+                    )  # radial basis function interpolator instance
+
+                    pInterp[cntTime] = rbfi(xInterp[cntTime, :], virtNewCoord[1], virtNewCoord[2])
+
                 elif self.method == 'rbf-multiquadric':
-                    #compute using 3-D Rbfs
-                    rbfi = Rbf(newCoord[0],
-                               newCoord[1],
-                               newCoord[2],
-                               pHelp[cntTime, :len(newCoord[0])], function='multiquadric')  # radial basis function interpolator instance
-                    
-                    pInterp[cntTime] = rbfi(xInterp[cntTime, :],
-                                            virtNewCoord[1],
-                                            virtNewCoord[2]) 
-                          
-                       
-        #return interpolated pressure values            
+                    # compute using 3-D Rbfs
+                    rbfi = Rbf(
+                        newCoord[0],
+                        newCoord[1],
+                        newCoord[2],
+                        pHelp[cntTime, : len(newCoord[0])],
+                        function='multiquadric',
+                    )  # radial basis function interpolator instance
+
+                    pInterp[cntTime] = rbfi(xInterp[cntTime, :], virtNewCoord[1], virtNewCoord[2])
+
+        # return interpolated pressure values
         return pInterp
 
-   
+
 class SpatialInterpolatorRotation(SpatialInterpolator):
+    """Spatial  Interpolation for rotating sources. Gets samples from :attr:`source`
+    and angles from  :attr:`AngleTracker`.Generates output via the generator :meth:`result`.
+
     """
-    Spatial  Interpolation for rotating sources. Gets samples from :attr:`source`
-    and angles from  :attr:`AngleTracker`.Generates output via the generator :meth:`result`
-    
-    """
+
     #: Angle data from AngleTracker class
     angle_source = Instance(AngleTracker)
-    
+
     #: Internal identifier
-    digest = Property( depends_on = ['source.digest', 'angle_source.digest',\
-                                     'mics.digest', 'mics_virtual.digest', \
-                                     'method','array_dimension', 'Q', 'interp_at_zero'])
-    
-    @cached_property
-    def _get_digest( self ):
-        return digest(self) 
-    
+    digest = Property(
+        depends_on=[
+            'source.digest',
+            'angle_source.digest',
+            'mics.digest',
+            'mics_virtual.digest',
+            'method',
+            'array_dimension',
+            'Q',
+            'interp_at_zero',
+        ],
+    )
+
+    @cached_property
+    def _get_digest(self):
+        return digest(self)
+
     def result(self, num=128):
-        """ 
-        Python generator that yields the output block-wise.
-        
+        """Python generator that yields the output block-wise.
+
         Parameters
         ----------
         num : integer
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block).
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, :attr:`numchannels`). 
+        Samples in blocks of shape (num, :attr:`numchannels`).
             The last block may be shorter than num.
+
         """
-        #period for rotation
+        # period for rotation
         period = 2 * pi
-        #get angle
+        # get angle
         angle = self.angle_source._get_angle()
-        #counter to track angle position in time for each block
-        count=0
+        # counter to track angle position in time for each block
+        count = 0
         for timeData in self.source.result(num):
-            phiDelay = angle[count:count+num]
-            interpVal = self._result_core_func(timeData, phiDelay, period, self.Q, interp_at_zero = False)
+            phiDelay = angle[count : count + num]
+            interpVal = self._result_core_func(timeData, phiDelay, period, self.Q, interp_at_zero=False)
             yield interpVal
-            count += num    
+            count += num
+
 
 class SpatialInterpolatorConstantRotation(SpatialInterpolator):
+    """Spatial linear Interpolation for constantly rotating sources.
+    Gets samples from :attr:`source` and generates output via the
+    generator :meth:`result`.
     """
-    Spatial linear Interpolation for constantly rotating sources.
-    Gets samples from :attr:`source` and generates output via the 
-    generator :meth:`result`
-    """
+
     #: Rotational speed in rps. Positive, if rotation is around positive z-axis sense,
     #: which means from x to y axis.
     rotational_speed = Float(0.0)
-    
+
     # internal identifier
-    digest = Property( depends_on = ['source.digest','mics.digest', \
-                                     'mics_virtual.digest','method','array_dimension', \
-                                     'Q', 'interp_at_zero','rotational_speed'])
-    
+    digest = Property(
+        depends_on=[
+            'source.digest',
+            'mics.digest',
+            'mics_virtual.digest',
+            'method',
+            'array_dimension',
+            'Q',
+            'interp_at_zero',
+            'rotational_speed',
+        ],
+    )
+
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
-    
-    
+
     def result(self, num=1):
-        """ 
-        Python generator that yields the output block-wise.
-        
+        """Python generator that yields the output block-wise.
+
         Parameters
         ----------
         num : integer
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block).
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, :attr:`numchannels`). 
+        Samples in blocks of shape (num, :attr:`numchannels`).
             The last block may be shorter than num.
+
         """
         omega = 2 * pi * self.rotational_speed
         period = 2 * pi
         phiOffset = 0.0
         for timeData in self.source.result(num):
             nTime = timeData.shape[0]
             phiDelay = phiOffset + linspace(0, nTime / self.sample_freq * omega, nTime, endpoint=False)
-            interpVal = self._result_core_func(timeData, phiDelay, period, self.Q, interp_at_zero = False)
+            interpVal = self._result_core_func(timeData, phiDelay, period, self.Q, interp_at_zero=False)
             phiOffset = phiDelay[-1] + omega / self.sample_freq
-            yield interpVal    
-      
-    
-class Mixer( TimeInOut ):
-    """
-    Mixes the signals from several sources.
-    """
+            yield interpVal
+
+
+class Mixer(TimeInOut):
+    """Mixes the signals from several sources."""
 
     #: Data source; :class:`~acoular.tprocess.SamplesGenerator` object.
     source = Trait(SamplesGenerator)
 
     #: List of additional :class:`~acoular.tprocess.SamplesGenerator` objects
     #: to be mixed.
-    sources = List( Instance(SamplesGenerator, ()) ) 
+    sources = List(Instance(SamplesGenerator, ()))
 
     #: Sampling frequency of the signal as given by :attr:`source`.
     sample_freq = Delegate('source')
-    
+
     #: Number of channels in output as given by :attr:`source`.
     numchannels = Delegate('source')
-               
+
     #: Number of samples in output as given by :attr:`source`.
     numsamples = Delegate('source')
 
-    # internal identifier    
+    # internal identifier
     sdigest = Str()
 
     @observe('sources.items.digest')
-    def _set_sources_digest( self, event ):
-        self.sdigest = ldigest(self.sources) 
-    
+    def _set_sources_digest(self, event):  # noqa ARG002
+        self.sdigest = ldigest(self.sources)
+
     # internal identifier
-    digest = Property( depends_on = ['source.digest','sdigest'])
+    digest = Property(depends_on=['source.digest', 'sdigest'])
 
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
-    def validate_sources( self ):
-        """ validates if sources fit together """
+    def validate_sources(self):
+        """Validates if sources fit together."""
         if self.source:
             for s in self.sources:
                 if self.sample_freq != s.sample_freq:
-                    raise ValueError("Sample frequency of %s does not fit" % s)
+                    raise ValueError('Sample frequency of %s does not fit' % s)
                 if self.numchannels != s.numchannels:
-                    raise ValueError("Channel count of %s does not fit" % s)
+                    raise ValueError('Channel count of %s does not fit' % s)
 
     def result(self, num):
-        """
-        Python generator that yields the output block-wise.
-        The output from the source and those in the list 
+        """Python generator that yields the output block-wise.
+        The output from the source and those in the list
         sources are being added.
-        
+
         Parameters
         ----------
         num : integer
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block).
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, numchannels). 
+        Samples in blocks of shape (num, numchannels).
             The last block may be shorter than num.
+
         """
-        
         # check whether all sources fit together
         self.validate_sources()
-        
+
         gens = [i.result(num) for i in self.sources]
         for temp in self.source.result(num):
             sh = temp.shape[0]
             for g in gens:
                 try:
                     temp1 = next(g)
                 except StopIteration:
                     return
                 if temp.shape[0] > temp1.shape[0]:
-                    temp = temp[:temp1.shape[0]]
-                temp += temp1[:temp.shape[0]]
+                    temp = temp[: temp1.shape[0]]
+                temp += temp1[: temp.shape[0]]
             yield temp
             if sh > temp.shape[0]:
                 break
 
 
-class TimePower( TimeInOut ):
-    """
-    Calculates time-depended power of the signal.
-    """
+class TimePower(TimeInOut):
+    """Calculates time-depended power of the signal."""
 
     def result(self, num):
-        """
-        Python generator that yields the output block-wise.
-        
+        """Python generator that yields the output block-wise.
+
         Parameters
         ----------
         num : integer
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block).
-        
+
         Returns
         -------
-        Squared output of source. 
-            Yields samples in blocks of shape (num, numchannels). 
+        Squared output of source.
+            Yields samples in blocks of shape (num, numchannels).
             The last block may be shorter than num.
+
         """
         for temp in self.source.result(num):
-            yield temp*temp
-    
-class TimeAverage( TimeInOut ) :
-    """
-    Calculates time-dependent average of the signal
-    """
+            yield temp * temp
+
+
+class TimeAverage(TimeInOut):
+    """Calculates time-dependent average of the signal."""
+
     #: Number of samples to average over, defaults to 64.
-    naverage = Int(64, 
-        desc = "number of samples to average over")
-        
+    naverage = Int(64, desc='number of samples to average over')
+
     #: Sampling frequency of the output signal, is set automatically.
-    sample_freq = Property( depends_on = 'source.sample_freq, naverage')
-    
+    sample_freq = Property(depends_on='source.sample_freq, naverage')
+
     #: Number of samples of the output signal, is set automatically.
-    numsamples = Property( depends_on = 'source.numsamples, naverage')
-    
+    numsamples = Property(depends_on='source.numsamples, naverage')
+
     # internal identifier
-    digest = Property( depends_on = ['source.digest', '__class__', 'naverage'])
+    digest = Property(depends_on=['source.digest', '__class__', 'naverage'])
 
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
-        
+
     @cached_property
-    def _get_sample_freq ( self ):
+    def _get_sample_freq(self):
         if self.source:
             return 1.0 * self.source.sample_freq / self.naverage
+        return None
 
     @cached_property
-    def _get_numsamples ( self ):
+    def _get_numsamples(self):
         if self.source:
             return self.source.numsamples / self.naverage
+        return None
 
     def result(self, num):
-        """
-        Python generator that yields the output block-wise.
+        """Python generator that yields the output block-wise.
 
-        
         Parameters
         ----------
         num : integer
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block).
-        
+
         Returns
         -------
-        Average of the output of source. 
-            Yields samples in blocks of shape (num, numchannels). 
+        Average of the output of source.
+            Yields samples in blocks of shape (num, numchannels).
             The last block may be shorter than num.
+
         """
         nav = self.naverage
-        for temp in self.source.result(num*nav):
+        for temp in self.source.result(num * nav):
             ns, nc = temp.shape
-            nso = int(ns/nav)
+            nso = int(ns / nav)
             if nso > 0:
-                yield temp[:nso*nav].reshape((nso, -1, nc)).mean(axis=1)
+                yield temp[: nso * nav].reshape((nso, -1, nc)).mean(axis=1)
+
+
+class TimeCumAverage(TimeInOut):
+    """Calculates cumulative average of the signal, useful for Leq."""
 
-class TimeCumAverage( TimeInOut):
-    """
-    Calculates cumulative average of the signal, useful for Leq
-    """
     def result(self, num):
-        """
-        Python generator that yields the output block-wise.
+        """Python generator that yields the output block-wise.
 
-        
         Parameters
         ----------
         num : integer
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block).
-        
+
         Returns
         -------
-        Cumulative average of the output of source. 
-            Yields samples in blocks of shape (num, numchannels). 
+        Cumulative average of the output of source.
+            Yields samples in blocks of shape (num, numchannels).
             The last block may be shorter than num.
+
         """
-        count = (arange(num) + 1)[:,newaxis]
-        for i,temp in enumerate(self.source.result(num)):
+        count = (arange(num) + 1)[:, newaxis]
+        for i, temp in enumerate(self.source.result(num)):
             ns, nc = temp.shape
             if not i:
-                accu = zeros((1,nc))
-            temp = (accu*(count[0]-1) + cumsum(temp,axis=0))/count[:ns]
+                accu = zeros((1, nc))
+            temp = (accu * (count[0] - 1) + cumsum(temp, axis=0)) / count[:ns]
             accu = temp[-1]
             count += ns
             yield temp
-        
-class TimeReverse( TimeInOut ):
-    """
-    Calculates the time-reversed signal of a source. 
-    """
+
+
+class TimeReverse(TimeInOut):
+    """Calculates the time-reversed signal of a source."""
+
     def result(self, num):
-        """
-        Python generator that yields the output block-wise.
+        """Python generator that yields the output block-wise.
 
-        
         Parameters
         ----------
         num : integer
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block).
-        
+
         Returns
         -------
-        Yields samples in blocks of shape (num, numchannels). 
-            Time-reversed output of source. 
+        Yields samples in blocks of shape (num, numchannels).
+            Time-reversed output of source.
             The last block may be shorter than num.
+
         """
         l = []
         l.extend(self.source.result(num))
         temp = empty_like(l[0])
         h = l.pop()
         nsh = h.shape[0]
         temp[:nsh] = h[::-1]
         for h in l[::-1]:
-            temp[nsh:] = h[:nsh-1:-1]
+            temp[nsh:] = h[: nsh - 1 : -1]
             yield temp
-            temp[:nsh] = h[nsh-1::-1]
+            temp[:nsh] = h[nsh - 1 :: -1]
         yield temp[:nsh]
-        
+
+
 class Filter(TimeInOut):
-    """
-    Abstract base class for IIR filters based on scipy lfilter
+    """Abstract base class for IIR filters based on scipy lfilter
     implements a filter with coefficients that may be changed
-    during processing
-    
+    during processing.
+
     Should not be instanciated by itself
     """
+
     #: Filter coefficients
     sos = Property()
 
-    def _get_sos( self ):
-        return tf2sos([1],[1])
+    def _get_sos(self):
+        return tf2sos([1], [1])
 
     def result(self, num):
-        """ 
-        Python generator that yields the output block-wise.
+        """Python generator that yields the output block-wise.
 
-        
         Parameters
         ----------
         num : integer
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block).
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, numchannels). 
+        Samples in blocks of shape (num, numchannels).
             Delivers the bandpass filtered output of source.
             The last block may be shorter than num.
+
         """
         sos = self.sos
         zi = zeros((sos.shape[0], 2, self.source.numchannels))
         for block in self.source.result(num):
-            sos = self.sos # this line is useful in case of changes 
-                            # to self.sos during generator lifetime
+            sos = self.sos  # this line is useful in case of changes
+            # to self.sos during generator lifetime
             block, zi = sosfilt(sos, block, axis=0, zi=zi)
             yield block
 
-class FiltOctave( Filter ):
-    """
-    Octave or third-octave filter (causal, non-zero phase delay).    
-    """
+
+class FiltOctave(Filter):
+    """Octave or third-octave filter (causal, non-zero phase delay)."""
+
     #: Band center frequency; defaults to 1000.
-    band = Float(1000.0, 
-        desc = "band center frequency")
-        
+    band = Float(1000.0, desc='band center frequency')
+
     #: Octave fraction: 'Octave' or 'Third octave'; defaults to 'Octave'.
-    fraction = Trait('Octave', {'Octave':1, 'Third octave':3}, 
-        desc = "fraction of octave")
+    fraction = Trait('Octave', {'Octave': 1, 'Third octave': 3}, desc='fraction of octave')
 
     #: Filter order
-    order = Int(3, desc = "IIR filter order")
-        
-    sos = Property( depends_on = ['band', 'fraction', 'source.digest', 'order'])
+    order = Int(3, desc='IIR filter order')
+
+    sos = Property(depends_on=['band', 'fraction', 'source.digest', 'order'])
 
     # internal identifier
-    digest = Property( depends_on = ['source.digest', '__class__', \
-        'band', 'fraction','order'])
+    digest = Property(depends_on=['source.digest', '__class__', 'band', 'fraction', 'order'])
 
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
-        
+
     @cached_property
-    def _get_sos( self ):
+    def _get_sos(self):
         # filter design
         fs = self.sample_freq
         # adjust filter edge frequencies for correct power bandwidth (see ANSI 1.11 1987
         # and Kalb,J.T.: "A thirty channel real time audio analyzer and its applications",
         # PhD Thesis: Georgia Inst. of Techn., 1975
-        beta = pi/(2*self.order)
-        alpha = pow(2.0, 1.0/(2.0*self.fraction_))
-        beta = 2 * beta / sin(beta) / (alpha-1/alpha)
-        alpha = (1+sqrt(1+beta*beta))/beta
-        fr = 2*self.band/fs
-        if fr > 1/sqrt(2):
-            raise ValueError("band frequency too high:%f,%f" % (self.band, fs))
-        om1 = fr/alpha 
-        om2 = fr*alpha
-        return butter(self.order, [om1, om2], 'bandpass', output = 'sos') 
+        beta = pi / (2 * self.order)
+        alpha = pow(2.0, 1.0 / (2.0 * self.fraction_))
+        beta = 2 * beta / sin(beta) / (alpha - 1 / alpha)
+        alpha = (1 + sqrt(1 + beta * beta)) / beta
+        fr = 2 * self.band / fs
+        if fr > 1 / sqrt(2):
+            msg = f'band frequency too high:{self.band:f},{fs:f}'
+            raise ValueError(msg)
+        om1 = fr / alpha
+        om2 = fr * alpha
+        return butter(self.order, [om1, om2], 'bandpass', output='sos')
+
+
+class FiltFiltOctave(FiltOctave):
+    """Octave or third-octave filter with zero phase delay.
 
-class FiltFiltOctave( FiltOctave ):
-    """
-    Octave or third-octave filter with zero phase delay.
-    
     This filter can be applied on time signals.
-    It requires large amounts of memory!   
+    It requires large amounts of memory!
     """
+
     #: Filter order (applied for forward filter and backward filter)
-    order = Int(2, desc = "IIR filter half order")
+    order = Int(2, desc='IIR filter half order')
 
     # internal identifier
-    digest = Property( depends_on = ['source.digest', '__class__', \
-        'band', 'fraction','order'])
+    digest = Property(depends_on=['source.digest', '__class__', 'band', 'fraction', 'order'])
 
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
- 
+
     @cached_property
-    def _get_sos( self ):
+    def _get_sos(self):
         # filter design
         fs = self.sample_freq
         # adjust filter edge frequencies for correct power bandwidth (see FiltOctave)
-        beta = pi/(2*self.order)
-        alpha = pow(2.0, 1.0/(2.0*self.fraction_))
-        beta = 2 * beta / sin(beta) / (alpha-1/alpha)
-        alpha = (1+sqrt(1+beta*beta))/beta
+        beta = pi / (2 * self.order)
+        alpha = pow(2.0, 1.0 / (2.0 * self.fraction_))
+        beta = 2 * beta / sin(beta) / (alpha - 1 / alpha)
+        alpha = (1 + sqrt(1 + beta * beta)) / beta
         # additional bandwidth correction for double-pass
-        alpha = alpha * {6:1.01,5:1.012,4:1.016,3:1.022,2:1.036,1:1.083}.get(self.order,1.0)**(3/self.fraction_)
-        fr = 2*self.band/fs
-        if fr > 1/sqrt(2):
-            raise ValueError("band frequency too high:%f,%f" % (self.band, fs))
-        om1 = fr/alpha 
-        om2 = fr*alpha
-        return butter(self.order, [om1, om2], 'bandpass', output = 'sos')   
-           
+        alpha = alpha * {6: 1.01, 5: 1.012, 4: 1.016, 3: 1.022, 2: 1.036, 1: 1.083}.get(self.order, 1.0) ** (
+            3 / self.fraction_
+        )
+        fr = 2 * self.band / fs
+        if fr > 1 / sqrt(2):
+            msg = f'band frequency too high:{self.band:f},{fs:f}'
+            raise ValueError(msg)
+        om1 = fr / alpha
+        om2 = fr * alpha
+        return butter(self.order, [om1, om2], 'bandpass', output='sos')
+
     def result(self, num):
-        """
-        Python generator that yields the output block-wise.
+        """Python generator that yields the output block-wise.
 
-        
         Parameters
         ----------
         num : integer
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block).
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, numchannels). 
+        Samples in blocks of shape (num, numchannels).
             Delivers the zero-phase bandpass filtered output of source.
             The last block may be shorter than num.
+
         """
-        sos = self.sos 
+        sos = self.sos
         data = empty((self.source.numsamples, self.source.numchannels))
         j = 0
         for block in self.source.result(num):
             ns, nc = block.shape
-            data[j:j+ns] = block
+            data[j : j + ns] = block
             j += ns
         # filter one channel at a time to save memory
         for j in range(self.source.numchannels):
             data[:, j] = sosfiltfilt(sos, data[:, j])
         j = 0
         ns = data.shape[0]
         while j < ns:
-            yield data[j:j+num]
+            yield data[j : j + num]
             j += num
 
+
 class TimeExpAverage(Filter):
-    """
-    Computes exponential averaging according to IEC 61672-1
+    """Computes exponential averaging according to IEC 61672-1
     time constant: F -> 125 ms, S -> 1 s
-    I (non-standard) -> 35 ms 
+    I (non-standard) -> 35 ms.
     """
 
     #: time weighting
-    weight = Trait('F', {'F':0.125, 'S':1.0, 'I':0.035}, 
-        desc = "time weighting")    
+    weight = Trait('F', {'F': 0.125, 'S': 1.0, 'I': 0.035}, desc='time weighting')
+
+    sos = Property(depends_on=['weight', 'source.digest'])
 
-    sos = Property( depends_on = ['weight', 'source.digest'])
-       
     # internal identifier
-    digest = Property( depends_on = ['source.digest', '__class__', \
-        'weight'])
+    digest = Property(depends_on=['source.digest', '__class__', 'weight'])
 
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
-        
+
     @cached_property
-    def _get_sos( self ):
-        alpha = 1-exp(-1/self.weight_/self.sample_freq)
-        a = [1, alpha-1]
+    def _get_sos(self):
+        alpha = 1 - exp(-1 / self.weight_ / self.sample_freq)
+        a = [1, alpha - 1]
         b = [alpha]
-        return tf2sos(b,a)
+        return tf2sos(b, a)
+
+
+class FiltFreqWeight(Filter):
+    """Frequency weighting filter accoring to IEC 61672."""
 
-class FiltFreqWeight( Filter ):
-    """
-    Frequency weighting filter accoring to IEC 61672
-    """
     #: weighting characteristics
-    weight = Trait('A',('A','C','Z'), desc="frequency weighting")
+    weight = Trait('A', ('A', 'C', 'Z'), desc='frequency weighting')
 
-    sos = Property( depends_on = ['weight', 'source.digest'])
+    sos = Property(depends_on=['weight', 'source.digest'])
 
     # internal identifier
-    digest = Property( depends_on = ['source.digest', '__class__', \
-        'weight'])
+    digest = Property(depends_on=['source.digest', '__class__', 'weight'])
 
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
     @cached_property
-    def _get_sos( self ):
+    def _get_sos(self):
         # s domain coefficients
         f1 = 20.598997
         f2 = 107.65265
         f3 = 737.86223
         f4 = 12194.217
-        a = polymul([1, 4*pi * f4, (2*pi * f4)**2],
-                    [1, 4*pi * f1, (2*pi * f1)**2])
+        a = polymul([1, 4 * pi * f4, (2 * pi * f4) ** 2], [1, 4 * pi * f1, (2 * pi * f1) ** 2])
         if self.weight == 'A':
-            a = polymul(polymul(a, [1, 2*pi * f3]), [1, 2*pi * f2])
-            b = [(2*pi * f4)**2 * 10**(1.9997/20) , 0, 0, 0, 0]
-            b,a = bilinear(b,a,self.sample_freq)
+            a = polymul(polymul(a, [1, 2 * pi * f3]), [1, 2 * pi * f2])
+            b = [(2 * pi * f4) ** 2 * 10 ** (1.9997 / 20), 0, 0, 0, 0]
+            b, a = bilinear(b, a, self.sample_freq)
         elif self.weight == 'C':
-            b = [(2*pi * f4)**2 * 10**(0.0619/20) , 0, 0]
-            b,a = bilinear(b,a,self.sample_freq)
-            b = append(b,zeros(2)) # make 6th order
-            a = append(a,zeros(2))
+            b = [(2 * pi * f4) ** 2 * 10 ** (0.0619 / 20), 0, 0]
+            b, a = bilinear(b, a, self.sample_freq)
+            b = append(b, zeros(2))  # make 6th order
+            a = append(a, zeros(2))
         else:
             b = zeros(7)
             b[0] = 1.0
-            a = b # 6th order flat response
-        return tf2sos(b,a)
+            a = b  # 6th order flat response
+        return tf2sos(b, a)
+
 
 class FilterBank(TimeInOut):
-    """
-    Abstract base class for IIR filter banks based on scipy lfilter
-    implements a bank of parallel filters 
-    
+    """Abstract base class for IIR filter banks based on scipy lfilter
+    implements a bank of parallel filters.
+
     Should not be instanciated by itself
     """
 
     #: List of filter coefficients for all filters
     sos = Property()
 
     #: List of labels for bands
@@ -1685,700 +1766,677 @@
 
     #: Number of bands
     numbands = Property()
 
     #: Number of bands
     numchannels = Property()
 
-    def _get_sos( self ):
-        return [tf2sos([1],[1])]
+    def _get_sos(self):
+        return [tf2sos([1], [1])]
 
-    def _get_bands( self ):
+    def _get_bands(self):
         return ['']
 
-    def _get_numbands( self ):
+    def _get_numbands(self):
         return 0
 
-    def _get_numchannels( self ):
-        return self.numbands*self.source.numchannels
+    def _get_numchannels(self):
+        return self.numbands * self.source.numchannels
 
     def result(self, num):
-        """ 
-        Python generator that yields the output block-wise.
-        
+        """Python generator that yields the output block-wise.
+
         Parameters
         ----------
         num : integer
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block).
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, numchannels). 
+        Samples in blocks of shape (num, numchannels).
             Delivers the bandpass filtered output of source.
             The last block may be shorter than num.
+
         """
         numbands = self.numbands
         snumch = self.source.numchannels
         sos = self.sos
-        zi = [zeros( (sos[0].shape[0],2, snumch)) for _ in range(numbands)]
-        res = zeros((num,self.numchannels),dtype='float')
+        zi = [zeros((sos[0].shape[0], 2, snumch)) for _ in range(numbands)]
+        res = zeros((num, self.numchannels), dtype='float')
         for block in self.source.result(num):
-            bl = block.shape[0]
             for i in range(numbands):
-                res[:,i*snumch:(i+1)*snumch], zi[i] = sosfilt(sos[i], block, axis=0, zi=zi[i])
+                res[:, i * snumch : (i + 1) * snumch], zi[i] = sosfilt(sos[i], block, axis=0, zi=zi[i])
             yield res
 
+
 class OctaveFilterBank(FilterBank):
-    """
-    Octave or third-octave filter bank
-    """
+    """Octave or third-octave filter bank."""
+
     #: Lowest band center frequency index; defaults to 21 (=125 Hz).
-    lband = Int(21, 
-        desc = "lowest band center frequency index")
+    lband = Int(21, desc='lowest band center frequency index')
 
     #: Lowest band center frequency index + 1; defaults to 40 (=8000 Hz).
-    hband = Int(40, 
-        desc = "lowest band center frequency index")
-        
+    hband = Int(40, desc='lowest band center frequency index')
+
     #: Octave fraction: 'Octave' or 'Third octave'; defaults to 'Octave'.
-    fraction = Trait('Octave', {'Octave':1, 'Third octave':3}, 
-        desc = "fraction of octave")
+    fraction = Trait('Octave', {'Octave': 1, 'Third octave': 3}, desc='fraction of octave')
 
     #: List of filter coefficients for all filters
-    ba = Property( depends_on = ['lband', 'hband', 'fraction', 'source.digest'])
+    ba = Property(depends_on=['lband', 'hband', 'fraction', 'source.digest'])
 
     #: List of labels for bands
-    bands = Property(depends_on = ['lband', 'hband', 'fraction'])
+    bands = Property(depends_on=['lband', 'hband', 'fraction'])
 
     #: Number of bands
-    numbands = Property(depends_on = ['lband', 'hband', 'fraction'])
-    
-        # internal identifier
-    digest = Property( depends_on = ['source.digest', '__class__', \
-        'lband','hband','fraction','order'])
+    numbands = Property(depends_on=['lband', 'hband', 'fraction'])
+
+    # internal identifier
+    digest = Property(depends_on=['source.digest', '__class__', 'lband', 'hband', 'fraction', 'order'])
 
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
     @cached_property
-    def _get_bands( self ):
-        return [10**(i/10) for i in range(self.lband,self.hband,4-self.fraction_)]
+    def _get_bands(self):
+        return [10 ** (i / 10) for i in range(self.lband, self.hband, 4 - self.fraction_)]
 
     @cached_property
-    def _get_numbands( self ):
+    def _get_numbands(self):
         return len(self.bands)
 
     @cached_property
-    def _get_sos( self ):
+    def _get_sos(self):
         of = FiltOctave(source=self.source, fraction=self.fraction)
         sos = []
-        for i in range(self.lband,self.hband,4-self.fraction_):
-            of.band = 10**(i/10)
+        for i in range(self.lband, self.hband, 4 - self.fraction_):
+            of.band = 10 ** (i / 10)
             sos_ = of.sos
             sos.append(sos_)
         return sos
 
-class TimeCache( TimeInOut ):
-    """
-    Caches time signal in cache file.
-    """
+
+class TimeCache(TimeInOut):
+    """Caches time signal in cache file."""
+
     # basename for cache
-    basename = Property( depends_on = 'digest')
-    
+    basename = Property(depends_on='digest')
+
     # hdf5 cache file
-    h5f = Instance( H5CacheFileBase, transient = True )
-    
+    h5f = Instance(H5CacheFileBase, transient=True)
+
     # internal identifier
-    digest = Property( depends_on = ['source.digest', '__class__'])
+    digest = Property(depends_on=['source.digest', '__class__'])
 
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
     @cached_property
-    def _get_basename ( self ):
-        obj = self.source # start with source
-        basename = 'void' # if no file source is found
+    def _get_basename(self):
+        obj = self.source  # start with source
+        basename = 'void'  # if no file source is found
         while obj:
-            if 'basename' in obj.all_trait_names(): # at original source?
-                basename = obj.basename # get the name
+            if 'basename' in obj.all_trait_names():  # at original source?
+                basename = obj.basename  # get the name
                 break
-            else:
-                try:
-                    obj = obj.source # traverse down until original data source
-                except AttributeError:
-                    obj = None
+            try:
+                obj = obj.source  # traverse down until original data source
+            except AttributeError:
+                obj = None
         return basename
 
-    def _pass_data(self,num):
-        for data in self.source.result(num):
-            yield data
+    def _pass_data(self, num):
+        yield from self.source.result(num)
 
-    def _write_data_to_cache(self,num):
+    def _write_data_to_cache(self, num):
         nodename = 'tc_' + self.digest
-        self.h5f.create_extendable_array(
-                nodename, (0, self.numchannels), "float32")
+        self.h5f.create_extendable_array(nodename, (0, self.numchannels), 'float32')
         ac = self.h5f.get_data_by_reference(nodename)
-        self.h5f.set_node_attribute(ac,'sample_freq',self.sample_freq)
-        self.h5f.set_node_attribute(ac,'complete',False)
+        self.h5f.set_node_attribute(ac, 'sample_freq', self.sample_freq)
+        self.h5f.set_node_attribute(ac, 'complete', False)
         for data in self.source.result(num):
-            self.h5f.append_data(ac,data)
+            self.h5f.append_data(ac, data)
             yield data
-        self.h5f.set_node_attribute(ac,'complete',True)
-    
-    def _get_data_from_cache(self,num):
+        self.h5f.set_node_attribute(ac, 'complete', True)
+
+    def _get_data_from_cache(self, num):
         nodename = 'tc_' + self.digest
         ac = self.h5f.get_data_by_reference(nodename)
         i = 0
         while i < ac.shape[0]:
-            yield ac[i:i+num]
+            yield ac[i : i + num]
             i += num
 
-    def _get_data_from_incomplete_cache(self,num):
+    def _get_data_from_incomplete_cache(self, num):
         nodename = 'tc_' + self.digest
         ac = self.h5f.get_data_by_reference(nodename)
         i = 0
         nblocks = 0
-        while i+num <= ac.shape[0]:
-            yield ac[i:i+num]
+        while i + num <= ac.shape[0]:
+            yield ac[i : i + num]
             nblocks += 1
             i += num
         self.h5f.remove_data(nodename)
-        self.h5f.create_extendable_array(
-                nodename, (0, self.numchannels), "float32")
+        self.h5f.create_extendable_array(nodename, (0, self.numchannels), 'float32')
         ac = self.h5f.get_data_by_reference(nodename)
-        self.h5f.set_node_attribute(ac,'sample_freq',self.sample_freq)
-        self.h5f.set_node_attribute(ac,'complete',False)
-        for j,data in enumerate(self.source.result(num)):
-            self.h5f.append_data(ac,data)
-            if j>=nblocks:
+        self.h5f.set_node_attribute(ac, 'sample_freq', self.sample_freq)
+        self.h5f.set_node_attribute(ac, 'complete', False)
+        for j, data in enumerate(self.source.result(num)):
+            self.h5f.append_data(ac, data)
+            if j >= nblocks:
                 yield data
-        self.h5f.set_node_attribute(ac,'complete',True)
+        self.h5f.set_node_attribute(ac, 'complete', True)
 
     # result generator: delivers input, possibly from cache
     def result(self, num):
-        """ 
-        Python generator that yields the output from cache block-wise.
+        """Python generator that yields the output from cache block-wise.
 
-        
         Parameters
         ----------
         num : integer
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block).
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, numchannels). 
+        Samples in blocks of shape (num, numchannels).
             The last block may be shorter than num.
             Echos the source output, but reads it from cache
             when available and prevents unnecassary recalculation.
+
         """
-        
         if config.global_caching == 'none':
             generator = self._pass_data
-        else: 
+        else:
             nodename = 'tc_' + self.digest
-            H5cache.get_cache_file( self, self.basename )
+            H5cache.get_cache_file(self, self.basename)
             if not self.h5f:
                 generator = self._pass_data
             elif self.h5f.is_cached(nodename):
                 generator = self._get_data_from_cache
                 if config.global_caching == 'overwrite':
                     self.h5f.remove_data(nodename)
                     generator = self._write_data_to_cache
                 elif not self.h5f.get_data_by_reference(nodename).attrs.__contains__('complete'):
-                    if config.global_caching =='readonly':
+                    if config.global_caching == 'readonly':
                         generator = self._pass_data
                     else:
                         generator = self._get_data_from_incomplete_cache
                 elif not self.h5f.get_data_by_reference(nodename).attrs['complete']:
-                    if config.global_caching =='readonly':
-                        warn("Cache file is incomplete for nodename %s. With config.global_caching='readonly', the cache file will not be used!" %str(nodename), Warning, stacklevel = 1)
+                    if config.global_caching == 'readonly':
+                        warn(
+                            "Cache file is incomplete for nodename %s. With config.global_caching='readonly', the cache file will not be used!"
+                            % str(nodename),
+                            Warning,
+                            stacklevel=1,
+                        )
                         generator = self._pass_data
                     else:
                         generator = self._get_data_from_incomplete_cache
             elif not self.h5f.is_cached(nodename):
                 generator = self._write_data_to_cache
                 if config.global_caching == 'readonly':
                     generator = self._pass_data
-        for temp in generator(num):
-            yield temp
+        yield from generator(num)
 
 
-class WriteWAV( TimeInOut ):
-    """
-    Saves time signal from one or more channels as mono/stereo/multi-channel
+class WriteWAV(TimeInOut):
+    """Saves time signal from one or more channels as mono/stereo/multi-channel
     `*.wav` file.
     """
-    
+
     #: Name of the file to be saved. If none is given, the name will be
     #: automatically generated from the sources.
-    name = File(filter=['*.wav'], 
-        desc="name of wave file")    
-    
+    name = File(filter=['*.wav'], desc='name of wave file')
+
     #: Basename for cache, readonly.
-    basename = Property( depends_on = 'digest')
-       
+    basename = Property(depends_on='digest')
+
     #: Channel(s) to save. List can only contain one or two channels.
-    channels = ListInt(desc="channel to save")
-       
+    channels = ListInt(desc='channel to save')
+
     # internal identifier
-    digest = Property( depends_on = ['source.digest', 'channels', '__class__'])
+    digest = Property(depends_on=['source.digest', 'channels', '__class__'])
 
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
     @cached_property
-    def _get_basename ( self ):
-        obj = self.source # start with source
+    def _get_basename(self):
+        obj = self.source  # start with source
         try:
             while obj:
-                if 'basename' in obj.all_trait_names(): # at original source?
-                    basename = obj.basename # get the name
+                if 'basename' in obj.all_trait_names():  # at original source?
+                    basename = obj.basename  # get the name
                     break
-                else:
-                    obj = obj.source # traverse down until original data source
+                obj = obj.source  # traverse down until original data source
             else:
                 basename = 'void'
         except AttributeError:
-            basename = 'void' # if no file source is found
+            basename = 'void'  # if no file source is found
         return basename
 
     def save(self):
-        """ 
-        Saves source output to one- or multiple-channel `*.wav` file. 
-        """
+        """Saves source output to one- or multiple-channel `*.wav` file."""
         nc = len(self.channels)
         if nc == 0:
-            raise ValueError("No channels given for output.")
+            msg = 'No channels given for output.'
+            raise ValueError(msg)
         if nc > 2:
-            warn("More than two channels given for output, exported file will have %i channels" % nc)
+            warn('More than two channels given for output, exported file will have %i channels' % nc, stacklevel=1)
         if self.name == '':
             name = self.basename
             for nr in self.channels:
                 name += '_%i' % nr
             name += '.wav'
         else:
             name = self.name
-        wf = wave.open(name,'w')
+        wf = wave.open(name, 'w')
         wf.setnchannels(nc)
         wf.setsampwidth(2)
         wf.setframerate(self.source.sample_freq)
         wf.setnframes(self.source.numsamples)
         mx = 0.0
         ind = array(self.channels)
         for data in self.source.result(1024):
             mx = max(abs(data[:, ind]).max(), mx)
-        scale = 0.9*2**15/mx
+        scale = 0.9 * 2**15 / mx
         for data in self.source.result(1024):
-            wf.writeframesraw(array(data[:, ind]*scale, dtype=int16).tostring())
+            wf.writeframesraw(array(data[:, ind] * scale, dtype=int16).tostring())
         wf.close()
 
-class WriteH5( TimeInOut ):
-    """
-    Saves time signal as `*.h5` file
-    """
+
+class WriteH5(TimeInOut):
+    """Saves time signal as `*.h5` file."""
+
     #: Name of the file to be saved. If none is given, the name will be
     #: automatically generated from a time stamp.
-    name = File(filter=['*.h5'], 
-        desc="name of data file")    
+    name = File(filter=['*.h5'], desc='name of data file')
 
-    #: Number of samples to write to file by `result` method. 
-    #: defaults to -1 (write as long as source yields data). 
+    #: Number of samples to write to file by `result` method.
+    #: defaults to -1 (write as long as source yields data).
     numsamples_write = Int(-1)
-    
+
     # flag that can be raised to stop file writing
     writeflag = Bool(True)
-      
+
     # internal identifier
-    digest = Property( depends_on = ['source.digest', '__class__'])
+    digest = Property(depends_on=['source.digest', '__class__'])
 
-    #: The floating-number-precision of entries of H5 File corresponding 
+    #: The floating-number-precision of entries of H5 File corresponding
     #: to numpy dtypes. Default is 32 bit.
-    precision = Trait('float32', 'float64', 
-                      desc="precision of H5 File")
+    precision = Trait('float32', 'float64', desc='precision of H5 File')
 
     #: Metadata to be stored in HDF5 file object
-    metadata = Dict(
-        desc="metadata to be stored in .h5 file")
+    metadata = Dict(desc='metadata to be stored in .h5 file')
 
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
     def create_filename(self):
         if self.name == '':
-            name = datetime.now().isoformat('_').replace(':','-').replace('.','_')
-            self.name = path.join(config.td_dir,name+'.h5')
+            name = datetime.now(tz=timezone.utc).isoformat('_').replace(':', '-').replace('.', '_')
+            self.name = path.join(config.td_dir, name + '.h5')
 
     def get_initialized_file(self):
         file = _get_h5file_class()
         self.create_filename()
-        f5h = file(self.name, mode = 'w')
-        f5h.create_extendable_array(
-                'time_data', (0, self.numchannels), self.precision)
+        f5h = file(self.name, mode='w')
+        f5h.create_extendable_array('time_data', (0, self.numchannels), self.precision)
         ac = f5h.get_data_by_reference('time_data')
-        f5h.set_node_attribute(ac,'sample_freq',self.sample_freq)
+        f5h.set_node_attribute(ac, 'sample_freq', self.sample_freq)
         self.add_metadata(f5h)
         return f5h
-        
+
     def save(self):
-        """ 
-        Saves source output to `*.h5` file 
-        """
-        
+        """Saves source output to `*.h5` file."""
         f5h = self.get_initialized_file()
         ac = f5h.get_data_by_reference('time_data')
         for data in self.source.result(4096):
-            f5h.append_data(ac,data)
+            f5h.append_data(ac, data)
         f5h.close()
 
     def add_metadata(self, f5h):
-        """ adds metadata to .h5 file """
+        """Adds metadata to .h5 file."""
         nitems = len(self.metadata.items())
         if nitems > 0:
-            f5h.create_new_group("metadata","/")
+            f5h.create_new_group('metadata', '/')
             for key, value in self.metadata.items():
-                f5h.create_array('/metadata',key, value)
+                f5h.create_array('/metadata', key, value)
 
     def result(self, num):
-        """ 
-        Python generator that saves source output to `*.h5` file and
+        """Python generator that saves source output to `*.h5` file and
         yields the source output block-wise.
 
-        
+
         Parameters
         ----------
         num : integer
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block).
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, numchannels). 
+        Samples in blocks of shape (num, numchannels).
             The last block may be shorter than num.
             Echos the source output, but reads it from cache
             when available and prevents unnecassary recalculation.
+
         """
-        
         self.writeflag = True
         f5h = self.get_initialized_file()
         ac = f5h.get_data_by_reference('time_data')
         scount = 0
         stotal = self.numsamples_write
         source_gen = self.source.result(num)
-        while self.writeflag: 
-            sleft = stotal-scount
-            if not stotal == -1 and sleft > 0: 
-                anz = min(num,sleft)
+        while self.writeflag:
+            sleft = stotal - scount
+            if stotal != -1 and sleft > 0:
+                anz = min(num, sleft)
             elif stotal == -1:
                 anz = num
             else:
                 break
             try:
                 data = next(source_gen)
             except:
                 break
-            f5h.append_data(ac,data[:anz])
+            f5h.append_data(ac, data[:anz])
             yield data
             f5h.flush()
             scount += anz
         f5h.close()
-        
-class LockedGenerator():
-    """
-    Creates a Thread Safe Iterator.
+
+
+class LockedGenerator:
+    """Creates a Thread Safe Iterator.
     Takes an iterator/generator and makes it thread-safe by
     serializing call to the `next` method of given iterator/generator.
     """
-    
+
     def __init__(self, it):
         self.it = it
         self.lock = threading.Lock()
 
-    def __next__(self): # this function implementation is not python 2 compatible!
+    def __next__(self):  # this function implementation is not python 2 compatible!
         with self.lock:
             return self.it.__next__()
 
-class SampleSplitter(TimeInOut): 
-    '''
-    This class distributes data blocks from source to several following objects.
-    A separate block buffer is created for each registered object in 
+
+class SampleSplitter(TimeInOut):
+    """Distributes data blocks from source to several following objects.
+    A separate block buffer is created for each registered object in
     (:attr:`block_buffer`) .
-    '''
+    """
 
     #: dictionary with block buffers (dict values) of registered objects (dict
-    #: keys).  
-    block_buffer = Dict(key_trait=Instance(SamplesGenerator)) 
+    #: keys).
+    block_buffer = Dict(key_trait=Instance(SamplesGenerator))
 
-    #: max elements/blocks in block buffers. 
+    #: max elements/blocks in block buffers.
     buffer_size = Int(100)
 
     #: defines behaviour in case of block_buffer overflow. Can be set individually
     #: for each registered object.
     #:
     #: * 'error': an IOError is thrown by the class
     #: * 'warning': a warning is displayed. Possibly leads to lost blocks of data
     #: * 'none': nothing happens. Possibly leads to lost blocks of data
-    buffer_overflow_treatment = Dict(key_trait=Instance(SamplesGenerator),
-                              value_trait=Trait('error','warning','none'),
-                              desc='defines buffer overflow behaviour.')       
- 
+    buffer_overflow_treatment = Dict(
+        key_trait=Instance(SamplesGenerator),
+        value_trait=Trait('error', 'warning', 'none'),
+        desc='defines buffer overflow behaviour.',
+    )
+
     # shadow trait to monitor if source deliver samples or is empty
-    _source_generator_exist = Bool(False) 
+    _source_generator_exist = Bool(False)
 
-    # shadow trait to monitor if buffer of objects with overflow treatment = 'error' 
+    # shadow trait to monitor if buffer of objects with overflow treatment = 'error'
     # or warning is overfilled. Error will be raised in all threads.
     _buffer_overflow = Bool(False)
 
-    # Helper Trait holds source generator     
+    # Helper Trait holds source generator
     _source_generator = Trait()
-           
-    def _create_block_buffer(self,obj):        
-        self.block_buffer[obj] = deque([],maxlen=self.buffer_size)
-        
-    def _create_buffer_overflow_treatment(self,obj):
-        self.buffer_overflow_treatment[obj] = 'error' 
-    
-    def _clear_block_buffer(self,obj):
+
+    def _create_block_buffer(self, obj):
+        self.block_buffer[obj] = deque([], maxlen=self.buffer_size)
+
+    def _create_buffer_overflow_treatment(self, obj):
+        self.buffer_overflow_treatment[obj] = 'error'
+
+    def _clear_block_buffer(self, obj):
         self.block_buffer[obj].clear()
-        
-    def _remove_block_buffer(self,obj):
+
+    def _remove_block_buffer(self, obj):
         del self.block_buffer[obj]
 
-    def _remove_buffer_overflow_treatment(self,obj):
+    def _remove_buffer_overflow_treatment(self, obj):
         del self.buffer_overflow_treatment[obj]
-        
-    def _assert_obj_registered(self,obj):
-        if not obj in self.block_buffer.keys(): 
-            raise IOError("calling object %s is not registered." %obj)
+
+    def _assert_obj_registered(self, obj):
+        if obj not in self.block_buffer:
+            raise OSError('calling object %s is not registered.' % obj)
 
     def _get_objs_to_inspect(self):
-        return [obj for obj in self.buffer_overflow_treatment.keys() 
-                            if not self.buffer_overflow_treatment[obj] == 'none']
- 
-    def _inspect_buffer_levels(self,inspect_objs):
+        return [obj for obj in self.buffer_overflow_treatment if self.buffer_overflow_treatment[obj] != 'none']
+
+    def _inspect_buffer_levels(self, inspect_objs):
         for obj in inspect_objs:
             if len(self.block_buffer[obj]) == self.buffer_size:
-                if self.buffer_overflow_treatment[obj] == 'error': 
+                if self.buffer_overflow_treatment[obj] == 'error':
                     self._buffer_overflow = True
                 elif self.buffer_overflow_treatment[obj] == 'warning':
-                    warn(
-                        'overfilled buffer for object: %s data will get lost' %obj,
-                        UserWarning)
-
-    def _create_source_generator(self,num):
-        for obj in self.block_buffer.keys(): self._clear_block_buffer(obj)
-        self._buffer_overflow = False # reset overflow bool
+                    warn('overfilled buffer for object: %s data will get lost' % obj, UserWarning, stacklevel=1)
+
+    def _create_source_generator(self, num):
+        for obj in self.block_buffer:
+            self._clear_block_buffer(obj)
+        self._buffer_overflow = False  # reset overflow bool
         self._source_generator = LockedGenerator(self.source.result(num))
-        self._source_generator_exist = True # indicates full generator
+        self._source_generator_exist = True  # indicates full generator
 
-    def _fill_block_buffers(self): 
-        next_block = next(self._source_generator)                
-        [self.block_buffer[obj].appendleft(next_block) for obj in self.block_buffer.keys()]
+    def _fill_block_buffers(self):
+        next_block = next(self._source_generator)
+        [self.block_buffer[obj].appendleft(next_block) for obj in self.block_buffer]
 
     @on_trait_change('buffer_size')
-    def _change_buffer_size(self): # 
-        for obj in self.block_buffer.keys():
+    def _change_buffer_size(self):  #
+        for obj in self.block_buffer:
             self._remove_block_buffer(obj)
-            self._create_block_buffer(obj)      
+            self._create_block_buffer(obj)
 
-    def register_object(self,*objects_to_register):
-        """
-        Function that can be used to register objects that receive blocks from 
-        this class.
-        """
+    def register_object(self, *objects_to_register):
+        """Function that can be used to register objects that receive blocks from this class."""
         for obj in objects_to_register:
-            if obj not in self.block_buffer.keys():
+            if obj not in self.block_buffer:
                 self._create_block_buffer(obj)
                 self._create_buffer_overflow_treatment(obj)
 
-    def remove_object(self,*objects_to_remove):
-        """
-        Function that can be used to remove registered objects.
-        """
+    def remove_object(self, *objects_to_remove):
+        """Function that can be used to remove registered objects."""
         for obj in objects_to_remove:
             self._remove_block_buffer(obj)
             self._remove_buffer_overflow_treatment(obj)
-            
-    def result(self,num):
-        """ 
-        Python generator that yields the output block-wise from block-buffer.
 
-        
+    def result(self, num):
+        """Python generator that yields the output block-wise from block-buffer.
+
         Parameters
         ----------
         num : integer
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block).
-        
+
         Returns
         -------
-        Samples in blocks of shape (num, numchannels). 
+        Samples in blocks of shape (num, numchannels).
             Delivers a block of samples to the calling object.
             The last block may be shorter than num.
-        """
 
-        calling_obj = currentframe().f_back.f_locals['self'] 
+        """
+        calling_obj = currentframe().f_back.f_locals['self']
         self._assert_obj_registered(calling_obj)
-        objs_to_inspect = self._get_objs_to_inspect() 
-        
-        if not self._source_generator_exist: 
-            self._create_source_generator(num) 
+        objs_to_inspect = self._get_objs_to_inspect()
+
+        if not self._source_generator_exist:
+            self._create_source_generator(num)
 
         while not self._buffer_overflow:
             if self.block_buffer[calling_obj]:
                 yield self.block_buffer[calling_obj].pop()
             else:
                 self._inspect_buffer_levels(objs_to_inspect)
-                try: 
+                try:
                     self._fill_block_buffers()
                 except StopIteration:
                     self._source_generator_exist = False
                     return
-        else: 
-            raise IOError('Maximum size of block buffer is reached!')   
+        else:
+            msg = 'Maximum size of block buffer is reached!'
+            raise OSError(msg)
+
 
-        
 class TimeConvolve(TimeInOut):
-    """
-    Uniformly partitioned overlap-save method (UPOLS) for fast convolution in the frequency domain, see :ref:`Wefers, 2015<Wefers2015>`.
-    """
+    """Uniformly partitioned overlap-save method (UPOLS) for fast convolution in the frequency domain, see :ref:`Wefers, 2015<Wefers2015>`."""
 
     #: Convolution kernel in the time domain.
     #: The second dimension of the kernel array has to be either 1 or match :attr:`~SamplesGenerator.numchannels`.
     #: If only a single kernel is supplied, it is applied to all channels.
-    kernel = CArray(dtype=float, desc="Convolution kernel.")
+    kernel = CArray(dtype=float, desc='Convolution kernel.')
 
-    _block_size = Int(desc="Block size")
+    _block_size = Int(desc='Block size')
 
     _kernel_blocks = Property(
-        depends_on=["kernel", "_block_size"],
-        desc="Frequency domain Kernel blocks",
+        depends_on=['kernel', '_block_size'],
+        desc='Frequency domain Kernel blocks',
     )
 
     # internal identifier
-    digest = Property( depends_on = ['source.digest', 'kernel', '__class__'])
+    digest = Property(depends_on=['source.digest', 'kernel', '__class__'])
 
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
 
     def _validate_kernel(self):
         # reshape kernel for broadcasting
         if self.kernel.ndim == 1:
             self.kernel = self.kernel.reshape([-1, 1])
             return
         # check dimensionality
-        elif self.kernel.ndim > 2:
-            raise ValueError("Only one or two dimensional kernels accepted.")
-
+        if self.kernel.ndim > 2:
+            msg = 'Only one or two dimensional kernels accepted.'
+            raise ValueError(msg)
         # check if number of kernels matches numchannels
         if self.kernel.shape[1] not in (1, self.source.numchannels):
-            raise ValueError("Number of kernels must be either `numchannels` or one.")
+            msg = 'Number of kernels must be either `numchannels` or one.'
+            raise ValueError(msg)
 
     # compute the rfft of the kernel blockwise
     @cached_property
     def _get__kernel_blocks(self):
         [L, N] = self.kernel.shape
         num = self._block_size
         P = int(ceil(L / num))
         trim = num * (P - 1)
-        blocks = zeros([P, num + 1, N], dtype="complex128")
+        blocks = zeros([P, num + 1, N], dtype='complex128')
 
         if P > 1:
             for i, block in enumerate(split(self.kernel[:trim], P - 1, axis=0)):
-                blocks[i] = rfft(concatenate([block, zeros([num, N])], axis=0),axis=0)
+                blocks[i] = rfft(concatenate([block, zeros([num, N])], axis=0), axis=0)
 
         blocks[-1] = rfft(
-            concatenate([self.kernel[trim:], zeros([2 * num - L + trim, N])], axis=0),axis=0
+            concatenate([self.kernel[trim:], zeros([2 * num - L + trim, N])], axis=0),
+            axis=0,
         )
         return blocks
 
-    
     def result(self, num=128):
-        """
-        Python generator that yields the output block-wise.
+        """Python generator that yields the output block-wise.
         The source output is convolved with the kernel.
 
         Parameters
         ----------
         num : integer
             This parameter defines the size of the blocks to be yielded
             (i.e. the number of samples per block).
 
         Returns
         -------
         Samples in blocks of shape (num, numchannels).
             The last block may be shorter than num.
-        """
 
+        """
         self._validate_kernel()
         # initialize variables
         self._block_size = num
         L = self.kernel.shape[0]
         N = self.source.numchannels
         M = self.source.numsamples
         P = int(ceil(L / num))  # number of kernel blocks
         Q = int(ceil(M / num))  # number of signal blocks
         R = int(ceil((L + M - 1) / num))  # number of output blocks
-        last_size = (L + M - 1) % num # size of final block
+        last_size = (L + M - 1) % num  # size of final block
 
         idx = 0
-        FDL = zeros([P, num + 1, N], dtype="complex128")
+        FDL = zeros([P, num + 1, N], dtype='complex128')
         buff = zeros([2 * num, N])  # time-domain input buffer
-        spec_sum = zeros([num+1,N],dtype="complex128")
+        spec_sum = zeros([num + 1, N], dtype='complex128')
 
         signal_blocks = self.source.result(num)
         temp = next(signal_blocks)
-        buff[num : num + temp.shape[0]] = temp # append new time-data
+        buff[num : num + temp.shape[0]] = temp  # append new time-data
 
         # for very short signals, we are already done
         if R == 1:
-            _append_to_FDL(FDL, idx, P, rfft(buff,axis=0))
-            spec_sum = _spectral_sum(spec_sum, FDL, self._kernel_blocks) 
+            _append_to_FDL(FDL, idx, P, rfft(buff, axis=0))
+            spec_sum = _spectral_sum(spec_sum, FDL, self._kernel_blocks)
             # truncate s.t. total length is L+M-1 (like numpy convolve w/ mode="full")
-            yield irfft(spec_sum,axis=0)[num: last_size + num]
+            yield irfft(spec_sum, axis=0)[num : last_size + num]
             return
 
         # stream processing of source signal
         for temp in signal_blocks:
-            _append_to_FDL(FDL, idx, P, rfft(buff,axis=0))
-            spec_sum = _spectral_sum(spec_sum, FDL, self._kernel_blocks )
-            yield irfft(spec_sum,axis=0)[num:]
+            _append_to_FDL(FDL, idx, P, rfft(buff, axis=0))
+            spec_sum = _spectral_sum(spec_sum, FDL, self._kernel_blocks)
+            yield irfft(spec_sum, axis=0)[num:]
             buff = concatenate(
-                [buff[num:], zeros([num, N])], axis=0
+                [buff[num:], zeros([num, N])],
+                axis=0,
             )  # shift input buffer to the left
-            buff[num : num + temp.shape[0]] = temp # append new time-data
+            buff[num : num + temp.shape[0]] = temp  # append new time-data
 
-        for _ in range(R-Q):
-            _append_to_FDL(FDL, idx, P, rfft(buff,axis=0))
-            spec_sum = _spectral_sum(spec_sum, FDL, self._kernel_blocks )
-            yield irfft(spec_sum,axis=0)[num:]
+        for _ in range(R - Q):
+            _append_to_FDL(FDL, idx, P, rfft(buff, axis=0))
+            spec_sum = _spectral_sum(spec_sum, FDL, self._kernel_blocks)
+            yield irfft(spec_sum, axis=0)[num:]
             buff = concatenate(
-                [buff[num:], zeros([num, N])], axis=0
+                [buff[num:], zeros([num, N])],
+                axis=0,
             )  # shift input buffer to the left
 
-        _append_to_FDL(FDL, idx, P, rfft(buff,axis=0))
-        spec_sum = _spectral_sum(spec_sum, FDL, self._kernel_blocks )
+        _append_to_FDL(FDL, idx, P, rfft(buff, axis=0))
+        spec_sum = _spectral_sum(spec_sum, FDL, self._kernel_blocks)
         # truncate s.t. total length is L+M-1 (like numpy convolve w/ mode="full")
-        yield irfft(spec_sum, axis=0)[num: last_size + num]
+        yield irfft(spec_sum, axis=0)[num : last_size + num]
+
 
 @nb.jit(nopython=True, cache=True)
-def _append_to_FDL(FDL,idx,P,buff):
+def _append_to_FDL(FDL, idx, P, buff):
     FDL[idx] = buff
-    idx = int(idx +1 % P)
+    idx = int(idx + 1 % P)
+
 
 @nb.jit(nopython=True, cache=True)
-def _spectral_sum(out,FDL,KB):
-    P,B,N = KB.shape
+def _spectral_sum(out, FDL, KB):
+    P, B, N = KB.shape
     for n in range(N):
         for b in range(B):
-            out[b,n] = 0
+            out[b, n] = 0
             for i in range(P):
-                out[b,n] += FDL[i,b,n]*KB[i,b,n]
+                out[b, n] += FDL[i, b, n] * KB[i, b, n]
 
     return out
```

### Comparing `acoular-24.3/acoular/trajectory.py` & `acoular-24.5/acoular/trajectory.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,126 +1,124 @@
-# -*- coding: utf-8 -*-
-#pylint: disable-msg=E0611, E1101, C0103, R0901, R0902, R0903, R0904, W0232
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 # Copyright (c) Acoular Development Team.
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 """Implements the definition of trajectories.
 
 .. autosummary::
     :toctree: generated/
 
     Trajectory
 """
 
 # imports from other packages
-from numpy import array, arange, sort, r_
-from scipy.interpolate import splprep, splev
-from traits.api import HasPrivateTraits, Float, \
-Property, cached_property, property_depends_on, Dict, Tuple
+from numpy import arange, array, r_, sort
+from scipy.interpolate import splev, splprep
+from traits.api import Dict, Float, HasPrivateTraits, Property, Tuple, cached_property, property_depends_on
 
 # acoular imports
 from .internal import digest
 
 
-class Trajectory( HasPrivateTraits ):
-    """
-    Describes a trajectory from sampled points.
-    
-    Based on a discrete number of points in space and time, a 
-    continuous trajectory is calculated using spline interpolation 
+class Trajectory(HasPrivateTraits):
+    """Describes a trajectory from sampled points.
+
+    Based on a discrete number of points in space and time, a
+    continuous trajectory is calculated using spline interpolation
     of positions between samples.
     """
-    #: Dictionary that assigns discrete time instants (keys) to 
+
+    #: Dictionary that assigns discrete time instants (keys) to
     #: sampled `(x, y, z)` positions along the trajectory (values).
-    points = Dict(key_trait = Float, value_trait = Tuple(Float, Float, Float), 
-        desc = "sampled positions along the trajectory")
-    
-    #: Tuple of the start and end time, is set automatically 
+    points = Dict(
+        key_trait=Float,
+        value_trait=Tuple(Float, Float, Float),
+        desc='sampled positions along the trajectory',
+    )
+
+    #: Tuple of the start and end time, is set automatically
     #: (depending on :attr:`points`).
     interval = Property()
-    #t_min, t_max tuple
-    
+    # t_min, t_max tuple
+
     #: Spline data, internal use.
     tck = Property()
-    
+
     # internal identifier
-    digest = Property( 
-        depends_on = ['points[]'], 
-        )
+    digest = Property(
+        depends_on=['points[]'],
+    )
 
     @cached_property
-    def _get_digest( self ):
+    def _get_digest(self):
         return digest(self)
-        
+
     @property_depends_on('points[]')
-    def _get_interval( self ):
+    def _get_interval(self):
         return sort(list(self.points.keys()))[r_[0, -1]]
 
     @property_depends_on('points[]')
-    def _get_tck( self ):
+    def _get_tck(self):
         t = sort(list(self.points.keys()))
         xp = array([self.points[i] for i in t]).T
-        k = min(3, len(self.points)-1)
+        k = min(3, len(self.points) - 1)
         tcku = splprep(xp, u=t, s=0, k=k)
         return tcku[0]
-    
+
     def location(self, t, der=0):
-        """ 
-        Returns the positions for one or more instants in time.
-        
+        """Returns the positions for one or more instants in time.
+
         Parameters
         ----------
         t : array of floats
             Instances in time to calculate the positions at.
         der : integer
             The order of derivative of the spline to compute, defaults to 0.
-        
+
         Returns
         -------
         (x, y, z) : tuple with arrays of floats
             Positions at the given times; `x`, `y` and `z` have the same shape as `t`.
+
         """
         return splev(t, self.tck, der)
-    
+
     def traj(self, t_start, t_end=None, delta_t=None, der=0):
-        """
-        Python generator that yields locations along the trajectory.
-        
+        """Python generator that yields locations along the trajectory.
+
         Parameters
         ----------
         t_start : float
-            Starting time of the trajectory, defaults to the earliest  
+            Starting time of the trajectory, defaults to the earliest
             time in :attr:`points`.
         t_end : float
-            Ending time of the trajectory, defaults to the latest  
+            Ending time of the trajectory, defaults to the latest
             time in :attr:`points`.
         delta_t : float
-            Time interval between yielded trajectory points, defaults to earliest  
+            Time interval between yielded trajectory points, defaults to earliest
             time in :attr:`points`.
-        
+
         Returns
         -------
         (x, y, z) : tuples of floats
             Positions at the desired times are yielded.
-            
+
         Examples
         --------
-        x.traj(0.1)  
-            Yields the position every 0.1 s within the 
+        x.traj(0.1)
+            Yields the position every 0.1 s within the
             given :attr:`interval`.
-        x.traj(2.5, 4.5, 0.1)  
+        x.traj(2.5, 4.5, 0.1)
             Yields the position every 0.1 s between 2.5 s and 4.5 s.
-        x.traj(0.1, der=1)  
-            Yields the 1st derivative of the spline (= velocity vector) every 0.1 s 
+        x.traj(0.1, der=1)
+            Yields the 1st derivative of the spline (= velocity vector) every 0.1 s
             within the given :attr:`interval`.
+
         """
         if not delta_t:
             delta_t = t_start
             t_start, t_end = self.interval
         if not t_end:
             t_end = self.interval[1]
         # all locations are fetched in one go because thats much faster
         # further improvement could be possible if interpolated locations are fetched
         # in blocks
-        for l in zip(*self.location(arange(t_start, t_end, delta_t),der)):
-            yield l
-        
+        yield from zip(*self.location(arange(t_start, t_end, delta_t), der))
```

### Comparing `acoular-24.3/acoular/demo/acoular_demo.py` & `acoular-24.5/acoular/demo/acoular_demo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,105 @@
-#! /usr/bin/env python
-# -*- coding: utf-8 -*-
-#pylint: disable-msg=E0611, E1101, C0103, R0901, R0902, R0903, R0904, W0232
-#------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 # Copyright (c) Acoular Development Team.
-#------------------------------------------------------------------------------
-"""Demo for Acoular
+# ------------------------------------------------------------------------------
+"""Demo for Acoular.
+
+To run the demo, execute the following commands:
+
+.. code-block:: python
+
+    import acoular
+
+    acoular.demo.acoular_demo.run()
+
 
 Generates a test data set for three sources, analyzes them and generates a
 map of the three sources.
- 
+
 The simulation generates the sound pressure at 64 microphones that are
 arrangend in the 'array64' geometry, which is part of the package. The sound
 pressure signals are sampled at 51200 Hz for a duration of 1 second.
 
 Source location (relative to array center) and levels:
 
 ====== =============== ======
-Source Location        Level 
+Source Location        Level
 ====== =============== ======
 1      (-0.1,-0.1,0.3) 1.0 Pa
-2      (0.15,0,0.3)    0.7 Pa 
+2      (0.15,0,0.3)    0.7 Pa
 3      (0,0.1,0.3)     0.5 Pa
 ====== =============== ======
+
 """
 
+
 def run():
+    """Run the Acoular demo."""
+    from pathlib import Path
+
+    from acoular import (
+        BeamformerBase,
+        L_p,
+        MicGeom,
+        Mixer,
+        PointSource,
+        PowerSpectra,
+        RectGrid,
+        SteeringVector,
+        TimeSamples,
+        WNoiseGenerator,
+        WriteH5,
+        config,
+    )
+    from acoular import __file__ as bpath
 
-    from os import path
-    from acoular import __file__ as bpath, MicGeom, WNoiseGenerator, PointSource,\
-     Mixer, WriteH5, TimeSamples, PowerSpectra, RectGrid, SteeringVector,\
-     BeamformerBase, L_p
-    from pylab import figure, plot, axis, imshow, colorbar, show
-    
     # set up the parameters
-    sfreq = 51200 
+    sfreq = 51200
     duration = 1
-    nsamples = duration*sfreq
-    micgeofile = path.join(path.split(bpath)[0],'xml','array_64.xml')
+    nsamples = duration * sfreq
+    micgeofile = Path(bpath).parent / 'xml' / 'array_64.xml'
     h5savefile = 'three_sources.h5'
-    
+
     # generate test data, in real life this would come from an array measurement
-    mg = MicGeom( from_file=micgeofile )
-    n1 = WNoiseGenerator( sample_freq=sfreq, numsamples=nsamples, seed=1 )
-    n2 = WNoiseGenerator( sample_freq=sfreq, numsamples=nsamples, seed=2, rms=0.7 )
-    n3 = WNoiseGenerator( sample_freq=sfreq, numsamples=nsamples, seed=3, rms=0.5 )
-    p1 = PointSource( signal=n1, mics=mg,  loc=(-0.1,-0.1,0.3) )
-    p2 = PointSource( signal=n2, mics=mg,  loc=(0.15,0,0.3) )
-    p3 = PointSource( signal=n3, mics=mg,  loc=(0,0.1,0.3) )
-    pa = Mixer( source=p1, sources=[p2,p3] )
-    wh5 = WriteH5( source=pa, name=h5savefile )
+    mg = MicGeom(from_file=micgeofile)
+    n1 = WNoiseGenerator(sample_freq=sfreq, numsamples=nsamples, seed=1)
+    n2 = WNoiseGenerator(sample_freq=sfreq, numsamples=nsamples, seed=2, rms=0.7)
+    n3 = WNoiseGenerator(sample_freq=sfreq, numsamples=nsamples, seed=3, rms=0.5)
+    p1 = PointSource(signal=n1, mics=mg, loc=(-0.1, -0.1, 0.3))
+    p2 = PointSource(signal=n2, mics=mg, loc=(0.15, 0, 0.3))
+    p3 = PointSource(signal=n3, mics=mg, loc=(0, 0.1, 0.3))
+    pa = Mixer(source=p1, sources=[p2, p3])
+    wh5 = WriteH5(source=pa, name=h5savefile)
     wh5.save()
-    
+
     # analyze the data and generate map
-    
-    ts = TimeSamples( name=h5savefile )
-    ps = PowerSpectra( time_data=ts, block_size=128, window='Hanning' )
-    
-    rg = RectGrid( x_min=-0.2, x_max=0.2, y_min=-0.2, y_max=0.2, z=0.3, \
-    increment=0.01 )
+
+    ts = TimeSamples(name=h5savefile)
+    ps = PowerSpectra(time_data=ts, block_size=128, window='Hanning')
+
+    rg = RectGrid(x_min=-0.2, x_max=0.2, y_min=-0.2, y_max=0.2, z=0.3, increment=0.01)
     st = SteeringVector(grid=rg, mics=mg)
-    
-    bb = BeamformerBase( freq_data=ps, steer=st )
-    pm = bb.synthetic( 8000, 3 )
-    Lm = L_p( pm )
-    
-    # show map
-    imshow( Lm.T, origin='lower', vmin=Lm.max()-10, extent=rg.extend(), \
-    interpolation='bicubic')
-    colorbar()
-    
-    # plot microphone geometry
-    figure(2)
-    plot(mg.mpos[0],mg.mpos[1],'o')
-    axis('equal')
-    
-    show()
 
-if __name__ == "__main__":
+    bb = BeamformerBase(freq_data=ps, steer=st)
+    pm = bb.synthetic(8000, 3)
+    Lm = L_p(pm)
+
+    if config.have_matplotlib:
+        from pylab import axis, colorbar, figure, imshow, plot, show
+
+        # show map
+        imshow(Lm.T, origin='lower', vmin=Lm.max() - 10, extent=rg.extend(), interpolation='bicubic')
+        colorbar()
+
+        # plot microphone geometry
+        figure(2)
+        plot(mg.mpos[0], mg.mpos[1], 'o')
+        axis('equal')
+
+        show()
+
+    else:
+        print('Matplotlib not found! Please install matplotlib if you want to plot the results.')
+
+
+if __name__ == '__main__':
     run()
```

### Comparing `acoular-24.3/acoular/xml/HW90D240_f10.xml` & `acoular-24.5/acoular/xml/HW90D240_f10.xml`

 * *Files identical despite different names*

### Comparing `acoular-24.3/acoular/xml/W90_D105_f10.xml` & `acoular-24.5/acoular/xml/W90_D105_f10.xml`

 * *Files identical despite different names*

### Comparing `acoular-24.3/acoular/xml/acousticam_2c.xml` & `acoular-24.5/acoular/xml/acousticam_2c.xml`

 * *Files identical despite different names*

### Comparing `acoular-24.3/acoular/xml/acousticam_4c.xml` & `acoular-24.5/acoular/xml/acousticam_4c.xml`

 * *Files identical despite different names*

### Comparing `acoular-24.3/acoular/xml/array38.xml` & `acoular-24.5/acoular/xml/array38.xml`

 * *Files identical despite different names*

### Comparing `acoular-24.3/acoular/xml/array92x.xml` & `acoular-24.5/acoular/xml/array92x.xml`

 * *Files identical despite different names*

### Comparing `acoular-24.3/acoular/xml/array_56.xml` & `acoular-24.5/acoular/xml/array_56.xml`

 * *Files identical despite different names*

### Comparing `acoular-24.3/acoular/xml/array_56_10_9.xml` & `acoular-24.5/acoular/xml/array_56_10_9.xml`

 * *Files identical despite different names*

### Comparing `acoular-24.3/acoular/xml/array_56_bomb.xml` & `acoular-24.5/acoular/xml/array_56_bomb.xml`

 * *Files identical despite different names*

### Comparing `acoular-24.3/acoular/xml/array_56_v2.xml` & `acoular-24.5/acoular/xml/array_56_v2.xml`

 * *Files identical despite different names*

### Comparing `acoular-24.3/acoular/xml/array_64.xml` & `acoular-24.5/acoular/xml/array_64.xml`

 * *Files identical despite different names*

### Comparing `acoular-24.3/acoular/xml/array_84_10_9.xml` & `acoular-24.5/acoular/xml/array_84_10_9.xml`

 * *Files identical despite different names*

### Comparing `acoular-24.3/acoular/xml/array_84_bomb_v3.xml` & `acoular-24.5/acoular/xml/array_84_bomb_v3.xml`

 * *Files identical despite different names*

### Comparing `acoular-24.3/acoular/xml/calib_vw_ring32.xml` & `acoular-24.5/acoular/xml/calib_vw_ring32.xml`

 * *Files identical despite different names*

### Comparing `acoular-24.3/acoular/xml/gfai_ring32.xml` & `acoular-24.5/acoular/xml/gfai_ring32.xml`

 * *Files identical despite different names*

### Comparing `acoular-24.3/acoular/xml/tub_vogel64.xml` & `acoular-24.5/acoular/xml/tub_vogel64.xml`

 * *Files identical despite different names*

### Comparing `acoular-24.3/LICENSE` & `acoular-24.5/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-Copyright (c) Acoular Development Team.
-All rights reserved.
+BSD 3-Clause License
 
+Copyright (c) Acoular Development Team
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
-  a. Redistributions of source code must retain the above copyright notice,
-     this list of conditions and the following disclaimer.
-  b. Redistributions in binary form must reproduce the above copyright
-     notice, this list of conditions and the following disclaimer in the
-     documentation and/or other materials provided with the distribution.
-  c. Neither the name of the acoular developers nor the names of
-     its contributors may be used to endorse or promote products
-     derived from this software without specific prior written
-     permission. 
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
 
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
 AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-ARE DISCLAIMED. IN NO EVENT SHALL THE REGENTS OR CONTRIBUTORS BE LIABLE FOR
-ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
-OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH
-DAMAGE.
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `acoular-24.3/README.md` & `acoular-24.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-![Acoular Logo](./docs/source/_static/Acoular_logo.png)
+![Acoular Logo](https://github.com/acoular/acoular/blob/master/docs/source/_static/Acoular_logo.png?raw=true)
 
 [![PyPI](https://img.shields.io/pypi/pyversions/acoular.svg)](https://pypi.org/project/acoular)
 [![PyPI](https://img.shields.io/pypi/v/acoular.svg)](https://pypi.org/project/acoular)
-[![Github](https://github.com/acoular/acoular/actions/workflows/python-package.yml/badge.svg)](https://github.com/acoular/acoular/actions/workflows/python-package.yml)
+[![Actions status](https://github.com/acoular/acoular/actions/workflows/tests.yml/badge.svg)](https://github.com/acoular/acoular/actions)
+[![DOI](https://zenodo.org/badge/29729101.svg)](https://zenodo.org/doi/10.5281/zenodo.3690794)
 
 # Acoular
 Acoular is a Python module for acoustic beamforming that is distributed under the new BSD license. 
 
 It is aimed at applications in acoustic testing. Multichannel data recorded by a microphone array can be processed and analyzed in order to generate mappings of sound source distributions. The maps (acoustic photographs) can then be used to locate sources of interest and to characterize them using their spectra. 
 
 # Features
 - frequency domain beamforming algorithms: delay & sum, Capon (adaptive), MUSIC, functional beamforming, eigenvalue beamforming
 - frequency domain deconvolution algorithms: DAMAS, DAMAS+, Clean, CleanSC, orthogonal deconvolution
 - frequency domain inverse methods: CMF (covariance matrix fitting), general inverse beamforming, SODIX
 - time domain methods: delay & sum beamforming, CleanT deconvolution
-- time domain methods applicable for moving source with arbitrary trajectory (linear, circular, arbitrarily 3D curved), 
+- time domain methods applicable for moving sources with arbitrary trajectory (linear, circular, arbitrarily 3D curved), 
 - frequency domain methods for rotating sources via virtual array rotation for arbitrary arrays and with different interpolation techniques
 - 1D, 2D and 3D mapping grids for all methods
 - gridless option for orthogonal deconvolution
 - four different built-in steering vector formulations
 - arbitrary stationary background flow can be considered for all methods
 - efficient cross spectral matrix computation
 - flexible modular time domain processing: n-th octave band filters, fast, slow, and impulse weighting, A-, C-, and Z-weighting, filter bank, zero delay filters
@@ -30,49 +31,56 @@
 - easily extendable with new algorithms
 
 # License
 Acoular is licensed under the BSD 3-clause. See [LICENSE](LICENSE)
 
 # Citing
 
-If you use Acoular for academic work, please consider citing our
+If you use Acoular for academic work, please consider citing both our
 [publication](https://doi.org/10.1016/j.apacoust.2016.09.015):
 
-    Ennes Sarradj, Gert Herold,
-    A Python framework for microphone array data processing,
-    Applied Acoustics, Volume 116, 2017, Pages 50-58
+    Sarradj, E., & Herold, G. (2017). 
+    A Python framework for microphone array data processing.
+    Applied Acoustics, 116, 50–58. 
+    https://doi.org/10.1016/j.apacoust.2016.09
+
+and our [software](https://zenodo.org/doi/10.5281/zenodo.3690794):
+
+    Sarradj, E., Herold, G., Kujawski, A., Jekosch, S., Pelling, A. J. R., Czuchaj, M., Gensch, T., & Oertwig, S..
+    Acoular – Acoustic testing and source mapping software. 
+    Zenodo. https://zenodo.org/doi/10.5281/zenodo.3690794
 
 # Dependencies
 Acoular runs under Linux, Windows and MacOS and needs Numpy, Scipy, Traits, scikit-learn, pytables, Numba packages available. 
 Matplotlib is needed for some of the examples.
 
-If you want to use input from a soundcard hardware, you will also need to install the [sounddevice](https://python-sounddevice.readthedocs.io/en/0.3.12/installation.html) package. Some solvers for the CMF method need [Pylops](https://pylops.readthedocs.io/en/stable/installation.html).
+If you want to use input from a soundcard, you will also need to install the [sounddevice](https://python-sounddevice.readthedocs.io/en/0.3.12/installation.html) package. Some solvers for the CMF method need [Pylops](https://pylops.readthedocs.io/en/stable/installation.html).
 
 # Installation
 
 Acoular can be installed via [conda](https://docs.conda.io/en/latest/), which is also part of the [Anaconda Python distribution](https://www.anaconda.com/). It is recommended to install into a dedicated [conda environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html). After activating this environment, run
 
     conda install -c acoular acoular
 
-This will install Acoular in your Anaconda Python enviroment and make the Acoular library available from Python. In addition, this will install all dependencies (those other packages mentioned above) if they are not already present on your system. 
+This will install Acoular in your Anaconda Python environment and make the Acoular library available from Python. In addition, this will install all dependencies (those other packages mentioned above) if they are not already present on your system. 
 
 A second option is to install Acoular via [pip](https://pip.pypa.io/en/stable/). It is recommended to use a dedicated [virtual environment](https://virtualenv.pypa.io/en/latest/) and then run
 
     pip install acoular
 
-For more detailed install instructions see the [documentation](http://acoular.org/install/index.html).
+For more detailed installation instructions, see the [documentation](https://acoular.org/install/index.html).
 
 # Documentation and help
-Documentation is available [here](http://acoular.org) with a
-[getting started](http://acoular.org/get_started/index.html) section and
-[examples](http://acoular.org/examples/index.html).
+Documentation is available [here](https://acoular.org) with a
+[getting started](https://acoular.org/get_started/index.html) section and
+[examples](https://acoular.org/examples/index.html).
 
 The Acoular [blog](https://acoular.github.io/blog/) contains some tutorials.
 
-Problems, suggestions and success using Acoular may be reported via the [acoular-users](https://groups.google.com/forum/#!forum/acoular-users) discussion forum.
+If you discover problems with the Acoular software, please report them using the [issue tracker](https://github.com/acoular/acoular/issues) on GitHub. Please use the [Acoular discussions forum](https://github.com/acoular/acoular/discussions) for practical questions, discussions, and demos.
 
 # Example
 This reads data from 64 microphone channels and computes a beamforming map for the 8kHz third octave band:
 
 ```python
 from os import path
 import acoular
@@ -101,8 +109,9 @@
 Lm = acoular.L_p( pm )
 # plot the map
 imshow( Lm.T, origin='lower', vmin=Lm.max()-10, extent=rg.extend(), \
 interpolation='bicubic')
 colorbar()
 ```
 
-![result](./docs/source/get_started/three_source_py3_colormap.png)
+
+![result](https://github.com/acoular/acoular/blob/master/docs/source/get_started/three_source_py3_colormap.png?raw=true)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `acoular-24.3/PKG-INFO` & `acoular-24.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,97 +1,88 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: acoular
-Version: 24.3
+Version: 24.5
 Summary: Python library for acoustic beamforming
 Project-URL: homepage, https://acoular.org
 Project-URL: documentation, https://acoular.org
 Project-URL: repository, https://github.com/acoular/acoular
 Author-email: Acoular Development Team <info@acoular.org>
 Maintainer-email: Adam Kujawski <adam.kujawski@tu-berlin.de>, Art Pelling <a.pelling@tu-berlin.de>, Ennes Sarradj <ennes.sarradj@tu-berlin.de>, Gert Herold <gert.herold@tu-berlin.de>, Mikolaj Czuchaj <mikolaj.czuchaj@tu-berlin.de>, Simon Jekosch <s.jekosch@tu-berlin.de>
-License: Copyright (c) Acoular Development Team.
-        All rights reserved.
+License: BSD 3-Clause License
         
+        Copyright (c) Acoular Development Team
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
-          a. Redistributions of source code must retain the above copyright notice,
-             this list of conditions and the following disclaimer.
-          b. Redistributions in binary form must reproduce the above copyright
-             notice, this list of conditions and the following disclaimer in the
-             documentation and/or other materials provided with the distribution.
-          c. Neither the name of the acoular developers nor the names of
-             its contributors may be used to endorse or promote products
-             derived from this software without specific prior written
-             permission. 
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
         
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
         
         THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
         AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-        ARE DISCLAIMED. IN NO EVENT SHALL THE REGENTS OR CONTRIBUTORS BE LIABLE FOR
-        ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-        LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
-        OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH
-        DAMAGE.
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: AUTHORS.rst
 License-File: LICENSE
 Keywords: acoustics,beamforming,microphone array
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: <=11,>=3.7
+Requires-Python: <=12,>=3.8
 Requires-Dist: numba
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
 Requires-Dist: scipy>=1.1.0
 Requires-Dist: tables>=3.4.4
 Requires-Dist: traits>=6.0
-Provides-Extra: dev
-Requires-Dist: graphviz; extra == 'dev'
-Requires-Dist: ipython; extra == 'dev'
-Requires-Dist: matplotlib; extra == 'dev'
-Requires-Dist: nox; extra == 'dev'
-Requires-Dist: numpydoc; extra == 'dev'
-Requires-Dist: pickleshare; extra == 'dev'
-Requires-Dist: sounddevice; extra == 'dev'
-Requires-Dist: sphinx; extra == 'dev'
 Provides-Extra: full
 Requires-Dist: matplotlib; extra == 'full'
 Requires-Dist: pylops; extra == 'full'
 Requires-Dist: sounddevice; extra == 'full'
 Description-Content-Type: text/markdown
 
-![Acoular Logo](./docs/source/_static/Acoular_logo.png)
+![Acoular Logo](https://github.com/acoular/acoular/blob/master/docs/source/_static/Acoular_logo.png?raw=true)
 
 [![PyPI](https://img.shields.io/pypi/pyversions/acoular.svg)](https://pypi.org/project/acoular)
 [![PyPI](https://img.shields.io/pypi/v/acoular.svg)](https://pypi.org/project/acoular)
-[![Github](https://github.com/acoular/acoular/actions/workflows/python-package.yml/badge.svg)](https://github.com/acoular/acoular/actions/workflows/python-package.yml)
+[![Actions status](https://github.com/acoular/acoular/actions/workflows/tests.yml/badge.svg)](https://github.com/acoular/acoular/actions)
+[![DOI](https://zenodo.org/badge/29729101.svg)](https://zenodo.org/doi/10.5281/zenodo.3690794)
 
 # Acoular
 Acoular is a Python module for acoustic beamforming that is distributed under the new BSD license. 
 
 It is aimed at applications in acoustic testing. Multichannel data recorded by a microphone array can be processed and analyzed in order to generate mappings of sound source distributions. The maps (acoustic photographs) can then be used to locate sources of interest and to characterize them using their spectra. 
 
 # Features
 - frequency domain beamforming algorithms: delay & sum, Capon (adaptive), MUSIC, functional beamforming, eigenvalue beamforming
 - frequency domain deconvolution algorithms: DAMAS, DAMAS+, Clean, CleanSC, orthogonal deconvolution
 - frequency domain inverse methods: CMF (covariance matrix fitting), general inverse beamforming, SODIX
 - time domain methods: delay & sum beamforming, CleanT deconvolution
-- time domain methods applicable for moving source with arbitrary trajectory (linear, circular, arbitrarily 3D curved), 
+- time domain methods applicable for moving sources with arbitrary trajectory (linear, circular, arbitrarily 3D curved), 
 - frequency domain methods for rotating sources via virtual array rotation for arbitrary arrays and with different interpolation techniques
 - 1D, 2D and 3D mapping grids for all methods
 - gridless option for orthogonal deconvolution
 - four different built-in steering vector formulations
 - arbitrary stationary background flow can be considered for all methods
 - efficient cross spectral matrix computation
 - flexible modular time domain processing: n-th octave band filters, fast, slow, and impulse weighting, A-, C-, and Z-weighting, filter bank, zero delay filters
@@ -103,49 +94,56 @@
 - easily extendable with new algorithms
 
 # License
 Acoular is licensed under the BSD 3-clause. See [LICENSE](LICENSE)
 
 # Citing
 
-If you use Acoular for academic work, please consider citing our
+If you use Acoular for academic work, please consider citing both our
 [publication](https://doi.org/10.1016/j.apacoust.2016.09.015):
 
-    Ennes Sarradj, Gert Herold,
-    A Python framework for microphone array data processing,
-    Applied Acoustics, Volume 116, 2017, Pages 50-58
+    Sarradj, E., & Herold, G. (2017). 
+    A Python framework for microphone array data processing.
+    Applied Acoustics, 116, 50–58. 
+    https://doi.org/10.1016/j.apacoust.2016.09
+
+and our [software](https://zenodo.org/doi/10.5281/zenodo.3690794):
+
+    Sarradj, E., Herold, G., Kujawski, A., Jekosch, S., Pelling, A. J. R., Czuchaj, M., Gensch, T., & Oertwig, S..
+    Acoular – Acoustic testing and source mapping software. 
+    Zenodo. https://zenodo.org/doi/10.5281/zenodo.3690794
 
 # Dependencies
 Acoular runs under Linux, Windows and MacOS and needs Numpy, Scipy, Traits, scikit-learn, pytables, Numba packages available. 
 Matplotlib is needed for some of the examples.
 
-If you want to use input from a soundcard hardware, you will also need to install the [sounddevice](https://python-sounddevice.readthedocs.io/en/0.3.12/installation.html) package. Some solvers for the CMF method need [Pylops](https://pylops.readthedocs.io/en/stable/installation.html).
+If you want to use input from a soundcard, you will also need to install the [sounddevice](https://python-sounddevice.readthedocs.io/en/0.3.12/installation.html) package. Some solvers for the CMF method need [Pylops](https://pylops.readthedocs.io/en/stable/installation.html).
 
 # Installation
 
 Acoular can be installed via [conda](https://docs.conda.io/en/latest/), which is also part of the [Anaconda Python distribution](https://www.anaconda.com/). It is recommended to install into a dedicated [conda environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html). After activating this environment, run
 
     conda install -c acoular acoular
 
-This will install Acoular in your Anaconda Python enviroment and make the Acoular library available from Python. In addition, this will install all dependencies (those other packages mentioned above) if they are not already present on your system. 
+This will install Acoular in your Anaconda Python environment and make the Acoular library available from Python. In addition, this will install all dependencies (those other packages mentioned above) if they are not already present on your system. 
 
 A second option is to install Acoular via [pip](https://pip.pypa.io/en/stable/). It is recommended to use a dedicated [virtual environment](https://virtualenv.pypa.io/en/latest/) and then run
 
     pip install acoular
 
-For more detailed install instructions see the [documentation](http://acoular.org/install/index.html).
+For more detailed installation instructions, see the [documentation](https://acoular.org/install/index.html).
 
 # Documentation and help
-Documentation is available [here](http://acoular.org) with a
-[getting started](http://acoular.org/get_started/index.html) section and
-[examples](http://acoular.org/examples/index.html).
+Documentation is available [here](https://acoular.org) with a
+[getting started](https://acoular.org/get_started/index.html) section and
+[examples](https://acoular.org/examples/index.html).
 
 The Acoular [blog](https://acoular.github.io/blog/) contains some tutorials.
 
-Problems, suggestions and success using Acoular may be reported via the [acoular-users](https://groups.google.com/forum/#!forum/acoular-users) discussion forum.
+If you discover problems with the Acoular software, please report them using the [issue tracker](https://github.com/acoular/acoular/issues) on GitHub. Please use the [Acoular discussions forum](https://github.com/acoular/acoular/discussions) for practical questions, discussions, and demos.
 
 # Example
 This reads data from 64 microphone channels and computes a beamforming map for the 8kHz third octave band:
 
 ```python
 from os import path
 import acoular
@@ -174,8 +172,9 @@
 Lm = acoular.L_p( pm )
 # plot the map
 imshow( Lm.T, origin='lower', vmin=Lm.max()-10, extent=rg.extend(), \
 interpolation='bicubic')
 colorbar()
 ```
 
-![result](./docs/source/get_started/three_source_py3_colormap.png)
+
+![result](https://github.com/acoular/acoular/blob/master/docs/source/get_started/three_source_py3_colormap.png?raw=true)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


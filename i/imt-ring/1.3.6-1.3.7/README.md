# Comparing `tmp/imt_ring-1.3.6.tar.gz` & `tmp/imt_ring-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imt_ring-1.3.6.tar", last modified: Wed May 22 11:41:55 2024, max compression
+gzip compressed data, was "imt_ring-1.3.7.tar", last modified: Fri May 24 08:32:45 2024, max compression
```

## Comparing `imt_ring-1.3.6.tar` & `imt_ring-1.3.7.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.406696 imt_ring-1.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-22 11:41:55.406696 imt_ring-1.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-22 11:41:51.000000 imt_ring-1.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-22 11:41:51.000000 imt_ring-1.3.6/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-22 11:41:55.406696 imt_ring-1.3.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.374696 imt_ring-1.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.406696 imt_ring-1.3.6/src/imt_ring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-22 11:41:55.000000 imt_ring-1.3.6/src/imt_ring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-22 11:41:55.000000 imt_ring-1.3.6/src/imt_ring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:41:55.000000 imt_ring-1.3.6/src/imt_ring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-22 11:41:55.000000 imt_ring-1.3.6/src/imt_ring.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 11:41:55.000000 imt_ring-1.3.6/src/imt_ring.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.378696 imt_ring-1.3.6/src/ring/
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algebra.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.378696 imt_ring-1.3.6/src/ring/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.378696 imt_ring-1.3.6/src/ring/algorithms/custom_joints/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/custom_joints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/custom_joints/rr_imp_joint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/custom_joints/rr_joint.py
--rw-r--r--   0 runner    (1001) docker     (127)    16676 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/custom_joints/suntay.py
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/dynamics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.378696 imt_ring-1.3.6/src/ring/algorithms/generator/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14840 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/generator/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/generator/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/generator/motion_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/generator/pd_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/generator/randomize.py
--rw-r--r--   0 runner    (1001) docker     (127)    12782 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/generator/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/generator/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    28260 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/jcalc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)    33947 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.382696 imt_ring-1.3.6/src/ring/io/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.382696 imt_ring-1.3.6/src/ring/io/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/branched.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.382696 imt_ring-1.3.6/src/ring/io/examples/exclude/
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/exclude/knee_trans_dof.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/exclude/standard_sys.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/exclude/standard_sys_rr_imp.xml
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/inv_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/knee_flexible_imus.xml
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/spherical_stiff.xml
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/symmetric.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_all_1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_all_2.xml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_ang0_pos0.xml
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_control.xml
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_double_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_free.xml
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_kinematics.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.382696 imt_ring-1.3.6/src/ring/io/examples/test_morph_system/
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_morph_system/four_seg_seg1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_morph_system/four_seg_seg3.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_randomize_position.xml
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_sensors.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_three_seg_seg2.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/test_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.386696 imt_ring-1.3.6/src/ring/io/xml/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/xml/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/xml/from_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/xml/test_from_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/xml/test_to_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/xml/to_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)    12193 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/maths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.386696 imt_ring-1.3.6/src/ring/ml/
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/ml/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/ml/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/ml/ml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/ml/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.386696 imt_ring-1.3.6/src/ring/ml/params/
--rw-r--r--   0 runner    (1001) docker     (127)  9355838 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/ml/params/0x13e3518065c21cd8.pickle
--rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/ml/ringnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/ml/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/ml/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.398696 imt_ring-1.3.6/src/ring/rendering/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/rendering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/rendering/base_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/rendering/mujoco_render.py
--rw-r--r--   0 runner    (1001) docker     (127)    10260 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/rendering/vispy_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/rendering/vispy_visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.398696 imt_ring-1.3.6/src/ring/sim2real/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/sim2real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/sim2real/sim2real.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/spatial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.402696 imt_ring-1.3.6/src/ring/sys_composer/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/sys_composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/sys_composer/delete_sys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/sys_composer/inject_sys.py
--rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/sys_composer/morph_sys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.402696 imt_ring-1.3.6/src/ring/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/utils/batchsize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/utils/colab.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/utils/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/utils/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.406696 imt_ring-1.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_custom_joints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_jcalc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_jit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_maths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_ml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_motion_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_pd_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_randomize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_rcmg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_sim2real.py
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_sys_composer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_train.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:32:45.996251 imt_ring-1.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-24 08:32:45.996251 imt_ring-1.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-24 08:32:36.000000 imt_ring-1.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-24 08:32:36.000000 imt_ring-1.3.7/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-24 08:32:45.996251 imt_ring-1.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:32:45.960251 imt_ring-1.3.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:32:45.992251 imt_ring-1.3.7/src/imt_ring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-24 08:32:45.000000 imt_ring-1.3.7/src/imt_ring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-24 08:32:45.000000 imt_ring-1.3.7/src/imt_ring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 08:32:45.000000 imt_ring-1.3.7/src/imt_ring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-24 08:32:45.000000 imt_ring-1.3.7/src/imt_ring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-24 08:32:45.000000 imt_ring-1.3.7/src/imt_ring.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:32:45.964251 imt_ring-1.3.7/src/ring/
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/algebra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:32:45.964251 imt_ring-1.3.7/src/ring/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/algorithms/_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:32:45.964251 imt_ring-1.3.7/src/ring/algorithms/custom_joints/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/algorithms/custom_joints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/algorithms/custom_joints/rr_imp_joint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/algorithms/custom_joints/rr_joint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16676 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/algorithms/custom_joints/suntay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/algorithms/dynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:32:45.968251 imt_ring-1.3.7/src/ring/algorithms/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/algorithms/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14840 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/algorithms/generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/algorithms/generator/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/algorithms/generator/motion_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/algorithms/generator/pd_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/algorithms/generator/randomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12782 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/algorithms/generator/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/algorithms/generator/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28260 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/algorithms/jcalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/algorithms/kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/algorithms/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33947 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:32:45.968251 imt_ring-1.3.7/src/ring/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:32:45.972251 imt_ring-1.3.7/src/ring/io/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/examples/branched.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:32:45.972251 imt_ring-1.3.7/src/ring/io/examples/exclude/
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/examples/exclude/knee_trans_dof.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/examples/exclude/standard_sys.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/examples/exclude/standard_sys_rr_imp.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/examples/inv_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/examples/knee_flexible_imus.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/examples/spherical_stiff.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/examples/symmetric.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/examples/test_all_1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/examples/test_all_2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/examples/test_ang0_pos0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/examples/test_control.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/examples/test_double_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/examples/test_free.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/examples/test_kinematics.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:32:45.972251 imt_ring-1.3.7/src/ring/io/examples/test_morph_system/
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/examples/test_morph_system/four_seg_seg1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/examples/test_morph_system/four_seg_seg3.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/examples/test_randomize_position.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/examples/test_sensors.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/examples/test_three_seg_seg2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:32:45.972251 imt_ring-1.3.7/src/ring/io/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/xml/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/xml/from_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/xml/test_from_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/xml/test_to_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/io/xml/to_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12193 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/maths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:32:45.976251 imt_ring-1.3.7/src/ring/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/ml/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/ml/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/ml/ml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/ml/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:32:45.976251 imt_ring-1.3.7/src/ring/ml/params/
+-rw-r--r--   0 runner    (1001) docker     (127)  9355838 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/ml/params/0x13e3518065c21cd8.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/ml/ringnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/ml/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/ml/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:32:45.988251 imt_ring-1.3.7/src/ring/rendering/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/rendering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/rendering/base_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/rendering/mujoco_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10260 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/rendering/vispy_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/rendering/vispy_visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:32:45.988251 imt_ring-1.3.7/src/ring/sim2real/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/sim2real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/sim2real/sim2real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:32:45.988251 imt_ring-1.3.7/src/ring/sys_composer/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/sys_composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/sys_composer/delete_sys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/sys_composer/inject_sys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/sys_composer/morph_sys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:32:45.988251 imt_ring-1.3.7/src/ring/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/utils/batchsize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/utils/colab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/utils/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/utils/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-24 08:32:36.000000 imt_ring-1.3.7/src/ring/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:32:45.992251 imt_ring-1.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-05-24 08:32:36.000000 imt_ring-1.3.7/tests/test_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-24 08:32:36.000000 imt_ring-1.3.7/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-24 08:32:36.000000 imt_ring-1.3.7/tests/test_custom_joints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-24 08:32:36.000000 imt_ring-1.3.7/tests/test_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-24 08:32:36.000000 imt_ring-1.3.7/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-24 08:32:36.000000 imt_ring-1.3.7/tests/test_jcalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-24 08:32:36.000000 imt_ring-1.3.7/tests/test_jit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-05-24 08:32:36.000000 imt_ring-1.3.7/tests/test_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-24 08:32:36.000000 imt_ring-1.3.7/tests/test_maths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-24 08:32:36.000000 imt_ring-1.3.7/tests/test_ml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-24 08:32:36.000000 imt_ring-1.3.7/tests/test_motion_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-24 08:32:36.000000 imt_ring-1.3.7/tests/test_pd_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-24 08:32:36.000000 imt_ring-1.3.7/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-24 08:32:36.000000 imt_ring-1.3.7/tests/test_randomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-24 08:32:36.000000 imt_ring-1.3.7/tests/test_rcmg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-24 08:32:36.000000 imt_ring-1.3.7/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-24 08:32:36.000000 imt_ring-1.3.7/tests/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-05-24 08:32:36.000000 imt_ring-1.3.7/tests/test_sim2real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-05-24 08:32:36.000000 imt_ring-1.3.7/tests/test_sys_composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-24 08:32:36.000000 imt_ring-1.3.7/tests/test_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-24 08:32:36.000000 imt_ring-1.3.7/tests/test_utils.py
```

### Comparing `imt_ring-1.3.6/PKG-INFO` & `imt_ring-1.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imt-ring
-Version: 1.3.6
+Version: 1.3.7
 Summary: RING: Recurrent Inertial Graph-based Estimator
 Author-email: Simon Bachhuber <simon.bachhuber@fau.de>
 Project-URL: Homepage, https://github.com/SimiPixel/ring
 Project-URL: Issues, https://github.com/SimiPixel/ring/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `imt_ring-1.3.6/pyproject.toml` & `imt_ring-1.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "imt-ring"
-version = "1.3.6"
+version = "1.3.7"
 authors = [
   { name="Simon Bachhuber", email="simon.bachhuber@fau.de" },
 ]
 description = "RING: Recurrent Inertial Graph-based Estimator"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `imt_ring-1.3.6/readme.md` & `imt_ring-1.3.7/readme.md`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/imt_ring.egg-info/PKG-INFO` & `imt_ring-1.3.7/src/imt_ring.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imt-ring
-Version: 1.3.6
+Version: 1.3.7
 Summary: RING: Recurrent Inertial Graph-based Estimator
 Author-email: Simon Bachhuber <simon.bachhuber@fau.de>
 Project-URL: Homepage, https://github.com/SimiPixel/ring
 Project-URL: Issues, https://github.com/SimiPixel/ring/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `imt_ring-1.3.6/src/imt_ring.egg-info/SOURCES.txt` & `imt_ring-1.3.7/src/imt_ring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/__init__.py` & `imt_ring-1.3.7/src/ring/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/algebra.py` & `imt_ring-1.3.7/src/ring/algebra.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/algorithms/__init__.py` & `imt_ring-1.3.7/src/ring/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/algorithms/_random.py` & `imt_ring-1.3.7/src/ring/algorithms/_random.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/algorithms/custom_joints/rr_imp_joint.py` & `imt_ring-1.3.7/src/ring/algorithms/custom_joints/rr_imp_joint.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/algorithms/custom_joints/rr_joint.py` & `imt_ring-1.3.7/src/ring/algorithms/custom_joints/rr_joint.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/algorithms/custom_joints/suntay.py` & `imt_ring-1.3.7/src/ring/algorithms/custom_joints/suntay.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/algorithms/dynamics.py` & `imt_ring-1.3.7/src/ring/algorithms/dynamics.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/algorithms/generator/__init__.py` & `imt_ring-1.3.7/src/ring/algorithms/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/algorithms/generator/base.py` & `imt_ring-1.3.7/src/ring/algorithms/generator/base.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/algorithms/generator/batch.py` & `imt_ring-1.3.7/src/ring/algorithms/generator/batch.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/algorithms/generator/motion_artifacts.py` & `imt_ring-1.3.7/src/ring/algorithms/generator/motion_artifacts.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/algorithms/generator/pd_control.py` & `imt_ring-1.3.7/src/ring/algorithms/generator/pd_control.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/algorithms/generator/randomize.py` & `imt_ring-1.3.7/src/ring/algorithms/generator/randomize.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/algorithms/generator/transforms.py` & `imt_ring-1.3.7/src/ring/algorithms/generator/transforms.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/algorithms/generator/types.py` & `imt_ring-1.3.7/src/ring/algorithms/generator/types.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/algorithms/jcalc.py` & `imt_ring-1.3.7/src/ring/algorithms/jcalc.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/algorithms/kinematics.py` & `imt_ring-1.3.7/src/ring/algorithms/kinematics.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/algorithms/sensors.py` & `imt_ring-1.3.7/src/ring/algorithms/sensors.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/base.py` & `imt_ring-1.3.7/src/ring/base.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/io/examples/branched.xml` & `imt_ring-1.3.7/src/ring/io/examples/branched.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/io/examples/exclude/knee_trans_dof.xml` & `imt_ring-1.3.7/src/ring/io/examples/exclude/knee_trans_dof.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/io/examples/exclude/standard_sys.xml` & `imt_ring-1.3.7/src/ring/io/examples/exclude/standard_sys.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/io/examples/exclude/standard_sys_rr_imp.xml` & `imt_ring-1.3.7/src/ring/io/examples/exclude/standard_sys_rr_imp.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/io/examples/inv_pendulum.xml` & `imt_ring-1.3.7/src/ring/io/examples/inv_pendulum.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/io/examples/knee_flexible_imus.xml` & `imt_ring-1.3.7/src/ring/io/examples/knee_flexible_imus.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/io/examples/test_all_1.xml` & `imt_ring-1.3.7/src/ring/io/examples/test_all_1.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/io/examples/test_all_2.xml` & `imt_ring-1.3.7/src/ring/io/examples/test_all_2.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/io/examples/test_control.xml` & `imt_ring-1.3.7/src/ring/io/examples/test_control.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/io/examples/test_double_pendulum.xml` & `imt_ring-1.3.7/src/ring/io/examples/test_double_pendulum.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/io/examples/test_kinematics.xml` & `imt_ring-1.3.7/src/ring/io/examples/test_kinematics.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/io/examples/test_morph_system/four_seg_seg1.xml` & `imt_ring-1.3.7/src/ring/io/examples/test_morph_system/four_seg_seg1.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/io/examples/test_morph_system/four_seg_seg3.xml` & `imt_ring-1.3.7/src/ring/io/examples/test_morph_system/four_seg_seg3.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/io/examples/test_randomize_position.xml` & `imt_ring-1.3.7/src/ring/io/examples/test_randomize_position.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/io/examples/test_three_seg_seg2.xml` & `imt_ring-1.3.7/src/ring/io/examples/test_three_seg_seg2.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/io/examples.py` & `imt_ring-1.3.7/src/ring/io/examples.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/io/xml/abstract.py` & `imt_ring-1.3.7/src/ring/io/xml/abstract.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/io/xml/from_xml.py` & `imt_ring-1.3.7/src/ring/io/xml/from_xml.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/io/xml/test_from_xml.py` & `imt_ring-1.3.7/src/ring/io/xml/test_from_xml.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/io/xml/test_to_xml.py` & `imt_ring-1.3.7/src/ring/io/xml/test_to_xml.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/io/xml/to_xml.py` & `imt_ring-1.3.7/src/ring/io/xml/to_xml.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/maths.py` & `imt_ring-1.3.7/src/ring/maths.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/ml/__init__.py` & `imt_ring-1.3.7/src/ring/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/ml/base.py` & `imt_ring-1.3.7/src/ring/ml/base.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/ml/callbacks.py` & `imt_ring-1.3.7/src/ring/ml/callbacks.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/ml/ml_utils.py` & `imt_ring-1.3.7/src/ring/ml/ml_utils.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/ml/optimizer.py` & `imt_ring-1.3.7/src/ring/ml/optimizer.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/ml/params/0x13e3518065c21cd8.pickle` & `imt_ring-1.3.7/src/ring/ml/params/0x13e3518065c21cd8.pickle`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/ml/ringnet.py` & `imt_ring-1.3.7/src/ring/ml/ringnet.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/ml/train.py` & `imt_ring-1.3.7/src/ring/ml/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from functools import partial
 from pathlib import Path
 from typing import Callable, Optional, Tuple
 
 import jax
 import jax.numpy as jnp
 import optax
+import tree_utils
+
 from ring import maths
 from ring.algorithms.generator import types
 from ring.ml import base as ml_base
 from ring.ml import callbacks as ml_callbacks
 from ring.ml import ml_utils
 from ring.ml import training_loop
 from ring.utils import distribute_batchsize
 from ring.utils import expand_batchsize
 from ring.utils import parse_path
 from ring.utils import pickle_load
-import tree_utils
-
 import wandb
 
 # (T, N, F) -> Scalar
 LOSS_FN = Callable[[jax.Array, jax.Array], float]
 _default_loss_fn = lambda q, qhat: maths.angle_error(q, qhat) ** 2
 
 # reduces (batch_axis, time_axis) -> Scalar
@@ -138,23 +138,25 @@
         key_network: PRNG Key that inits the network state and parameters.
         key_generator: PRNG Key that inits the data stream of the generator.
 
     Returns: bool
         Wether or not the training run was killed by a callback.
     """
 
+    filter = filter.nojit()
+
     if checkpoint is not None:
         checkpoint = Path(checkpoint).with_suffix(".pickle")
         recv_checkpoint: dict = pickle_load(checkpoint)
-        filter.params = recv_checkpoint["params"]
+        filter_params = recv_checkpoint["params"]
         opt_state = recv_checkpoint["opt_state"]
+        del recv_checkpoint
+    else:
+        filter_params = filter.search_attr("params")
 
-    filter = filter.nojit()
-
-    filter_params = filter.search_attr("params")
     if filter_params is None:
         X, _ = generator(jax.random.PRNGKey(1))
         filter_params, _ = filter.init(X=X, seed=seed_network)
         del X
 
     if checkpoint is None:
         opt_state = optimizer.init(filter_params)
```

### Comparing `imt_ring-1.3.6/src/ring/ml/training_loop.py` & `imt_ring-1.3.7/src/ring/ml/training_loop.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/rendering/base_render.py` & `imt_ring-1.3.7/src/ring/rendering/base_render.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/rendering/mujoco_render.py` & `imt_ring-1.3.7/src/ring/rendering/mujoco_render.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/rendering/vispy_render.py` & `imt_ring-1.3.7/src/ring/rendering/vispy_render.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/rendering/vispy_visuals.py` & `imt_ring-1.3.7/src/ring/rendering/vispy_visuals.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/sim2real/sim2real.py` & `imt_ring-1.3.7/src/ring/sim2real/sim2real.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/spatial.py` & `imt_ring-1.3.7/src/ring/spatial.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/sys_composer/delete_sys.py` & `imt_ring-1.3.7/src/ring/sys_composer/delete_sys.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/sys_composer/inject_sys.py` & `imt_ring-1.3.7/src/ring/sys_composer/inject_sys.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/sys_composer/morph_sys.py` & `imt_ring-1.3.7/src/ring/sys_composer/morph_sys.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/utils/__init__.py` & `imt_ring-1.3.7/src/ring/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/utils/batchsize.py` & `imt_ring-1.3.7/src/ring/utils/batchsize.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/utils/colab.py` & `imt_ring-1.3.7/src/ring/utils/colab.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/utils/hdf5.py` & `imt_ring-1.3.7/src/ring/utils/hdf5.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/utils/normalizer.py` & `imt_ring-1.3.7/src/ring/utils/normalizer.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/utils/path.py` & `imt_ring-1.3.7/src/ring/utils/path.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/src/ring/utils/utils.py` & `imt_ring-1.3.7/src/ring/utils/utils.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/tests/test_algebra.py` & `imt_ring-1.3.7/tests/test_algebra.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/tests/test_base.py` & `imt_ring-1.3.7/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/tests/test_custom_joints.py` & `imt_ring-1.3.7/tests/test_custom_joints.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/tests/test_dynamics.py` & `imt_ring-1.3.7/tests/test_dynamics.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/tests/test_generator.py` & `imt_ring-1.3.7/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/tests/test_jcalc.py` & `imt_ring-1.3.7/tests/test_jcalc.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/tests/test_jit.py` & `imt_ring-1.3.7/tests/test_jit.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/tests/test_kinematics.py` & `imt_ring-1.3.7/tests/test_kinematics.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/tests/test_maths.py` & `imt_ring-1.3.7/tests/test_maths.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/tests/test_ml_utils.py` & `imt_ring-1.3.7/tests/test_ml_utils.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/tests/test_motion_artifacts.py` & `imt_ring-1.3.7/tests/test_motion_artifacts.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/tests/test_pd_control.py` & `imt_ring-1.3.7/tests/test_pd_control.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/tests/test_random.py` & `imt_ring-1.3.7/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/tests/test_randomize.py` & `imt_ring-1.3.7/tests/test_randomize.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/tests/test_rcmg.py` & `imt_ring-1.3.7/tests/test_rcmg.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/tests/test_render.py` & `imt_ring-1.3.7/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/tests/test_sensors.py` & `imt_ring-1.3.7/tests/test_sensors.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/tests/test_sim2real.py` & `imt_ring-1.3.7/tests/test_sim2real.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/tests/test_sys_composer.py` & `imt_ring-1.3.7/tests/test_sys_composer.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/tests/test_train.py` & `imt_ring-1.3.7/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.6/tests/test_utils.py` & `imt_ring-1.3.7/tests/test_utils.py`

 * *Files identical despite different names*


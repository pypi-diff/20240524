# Comparing `tmp/gym_jiminy_toolbox-1.8.5.post1-py3-none-any.whl.zip` & `tmp/gym_jiminy_toolbox-1.8.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12899 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-30 00:34 gym_jiminy/toolbox/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-30 00:34 gym_jiminy/toolbox/py.typed
--rw-r--r--  2.0 unx      272 b- defN 24-Apr-30 00:34 gym_jiminy/toolbox/math/__init__.py
--rw-r--r--  2.0 unx     7946 b- defN 24-Apr-30 00:34 gym_jiminy/toolbox/math/qhull.py
--rw-r--r--  2.0 unx    18359 b- defN 24-Apr-30 00:34 gym_jiminy/toolbox/math/spline.py
--rw-r--r--  2.0 unx      270 b- defN 24-Apr-30 00:34 gym_jiminy/toolbox/wrappers/__init__.py
--rw-r--r--  2.0 unx     3053 b- defN 24-Apr-30 00:34 gym_jiminy/toolbox/wrappers/frame_rate_limiter.py
--rw-r--r--  2.0 unx     4921 b- defN 24-Apr-30 00:34 gym_jiminy/toolbox/wrappers/meta_envs.py
--rw-r--r--  2.0 unx      945 b- defN 24-Apr-30 00:35 gym_jiminy_toolbox-1.8.5.post1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-30 00:35 gym_jiminy_toolbox-1.8.5.post1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-30 00:35 gym_jiminy_toolbox-1.8.5.post1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1099 b- defN 24-Apr-30 00:35 gym_jiminy_toolbox-1.8.5.post1.dist-info/RECORD
-12 files, 36968 bytes uncompressed, 11003 bytes compressed:  70.2%
+Zip file size: 12895 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 13:32 gym_jiminy/toolbox/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 13:32 gym_jiminy/toolbox/py.typed
+-rw-r--r--  2.0 unx      272 b- defN 24-May-24 13:32 gym_jiminy/toolbox/math/__init__.py
+-rw-r--r--  2.0 unx     7946 b- defN 24-May-24 13:32 gym_jiminy/toolbox/math/qhull.py
+-rw-r--r--  2.0 unx    18359 b- defN 24-May-24 13:32 gym_jiminy/toolbox/math/spline.py
+-rw-r--r--  2.0 unx      270 b- defN 24-May-24 13:32 gym_jiminy/toolbox/wrappers/__init__.py
+-rw-r--r--  2.0 unx     3136 b- defN 24-May-24 13:32 gym_jiminy/toolbox/wrappers/frame_rate_limiter.py
+-rw-r--r--  2.0 unx     4980 b- defN 24-May-24 13:32 gym_jiminy/toolbox/wrappers/meta_envs.py
+-rw-r--r--  2.0 unx      933 b- defN 24-May-24 13:33 gym_jiminy_toolbox-1.8.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 13:33 gym_jiminy_toolbox-1.8.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-24 13:33 gym_jiminy_toolbox-1.8.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1075 b- defN 24-May-24 13:33 gym_jiminy_toolbox-1.8.6.dist-info/RECORD
+12 files, 37074 bytes uncompressed, 11047 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: gym_jiminy/toolbox/wrappers/frame_rate_limiter.py
 Comment: 
 
 Filename: gym_jiminy/toolbox/wrappers/meta_envs.py
 Comment: 
 
-Filename: gym_jiminy_toolbox-1.8.5.post1.dist-info/METADATA
+Filename: gym_jiminy_toolbox-1.8.6.dist-info/METADATA
 Comment: 
 
-Filename: gym_jiminy_toolbox-1.8.5.post1.dist-info/WHEEL
+Filename: gym_jiminy_toolbox-1.8.6.dist-info/WHEEL
 Comment: 
 
-Filename: gym_jiminy_toolbox-1.8.5.post1.dist-info/top_level.txt
+Filename: gym_jiminy_toolbox-1.8.6.dist-info/top_level.txt
 Comment: 
 
-Filename: gym_jiminy_toolbox-1.8.5.post1.dist-info/RECORD
+Filename: gym_jiminy_toolbox-1.8.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gym_jiminy/toolbox/wrappers/frame_rate_limiter.py

```diff
@@ -1,8 +1,9 @@
-""" TODO: Write documentation.
+"""This module implements a wrapper for maintaining a stable framerate when
+human rendering is enabled during an episode.
 """
 import time
 from typing import Any, List, Optional, Tuple, Generic, Union, SupportsFloat
 
 import gymnasium as gym
 from gymnasium.core import RenderFrame
 
@@ -17,16 +18,16 @@
     """Limit the rendering framerate of an environment to a given threshold,
     which is typically useful if human rendering is enabled.
 
     .. note::
         This wrapper only affects `render`, not `replay`.
 
     .. warning::
-        This wrapper is only compatible with `BasePipelineWrapper` and
-        `BaseJiminyEnv` as it requires having a `step_dt` attribute.
+        This wrapper is only compatible with `InterfaceJiminyEnv` because it
+        requires having access to `step_dt` attribute.
     """
     def __init__(self,  # pylint: disable=unused-argument
                  env: InterfaceJiminyEnv[ObsT, ActT],
                  speed_ratio: float = 1.0,
                  human_only: bool = True,
                  **kwargs: Any):
         """
```

## gym_jiminy/toolbox/wrappers/meta_envs.py

```diff
@@ -57,14 +57,16 @@
     """
     def __init__(self,
                  env: HierarchicalTaskSettableEnv[ObsT, ActT],
                  initial_task_tree: Optional[DataTreeT] = None
                  ) -> None:
         """ TODO: Write documentation.
         """
+        # pylint: disable=possibly-used-before-assignment
+
         # Call base implementation
         super().__init__(env)
 
         # Make sure the task space of the environment is supported
         task_space = env.task_space
         if (not isinstance(task_space, spaces.Tuple) or
             any(not isinstance(space, (
```

## Comparing `gym_jiminy_toolbox-1.8.5.post1.dist-info/METADATA` & `gym_jiminy_toolbox-1.8.6.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-jiminy-toolbox
-Version: 1.8.5.post1
+Version: 1.8.6
 Summary: Generic Reinforcement learning toolbox based on Pytorch for Gym Jiminy.
 Author: Alexis Duburcq
 Author-email: alexis.duburcq@gmail.com
 Maintainer: Alexis Duburcq
 License: MIT
 Keywords: reinforcement-learning robotics gym jiminy
 Classifier: Development Status :: 3 - Alpha
@@ -14,10 +14,10 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<3.13
-Requires-Dist: gym-jiminy ~=1.8.5.post1
+Requires-Dist: gym-jiminy ~=1.8.6
 Requires-Dist: scipy >=1.9.2
```

## Comparing `gym_jiminy_toolbox-1.8.5.post1.dist-info/RECORD` & `gym_jiminy_toolbox-1.8.6.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 gym_jiminy/toolbox/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gym_jiminy/toolbox/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gym_jiminy/toolbox/math/__init__.py,sha256=fJBmFKSbDxHTBtWX_dmu5p3xomaazzs5et2dOM1RZbc,272
 gym_jiminy/toolbox/math/qhull.py,sha256=80WmgA_WBoBk-jYpXkSb_J3zO_AteKuWp413hXW4TWk,7946
 gym_jiminy/toolbox/math/spline.py,sha256=ad4rfZy0zyXwZ0mpDzKnsyLOlH2fHXxuqeoz9_sisHk,18359
 gym_jiminy/toolbox/wrappers/__init__.py,sha256=O3pwKYZTi7nFit0IdKV9YhT7dYGjY-O6fIsR6jAPpig,270
-gym_jiminy/toolbox/wrappers/frame_rate_limiter.py,sha256=klhRjr-Ag7VrV7o_pIs80dCRFzRPaEoDpTR3PKEgESY,3053
-gym_jiminy/toolbox/wrappers/meta_envs.py,sha256=ppOkhyZoYW6NO1q4iQi5_8cpq4vaxNttvxGslK39FTo,4921
-gym_jiminy_toolbox-1.8.5.post1.dist-info/METADATA,sha256=aG03UPHmmH19w-993ONEO3bxZBZU5brtNpfVFoNfnDk,945
-gym_jiminy_toolbox-1.8.5.post1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-gym_jiminy_toolbox-1.8.5.post1.dist-info/top_level.txt,sha256=c6Ipde11Sivat1D9sNj6sn3TCpadD0Qqk9fMzWYQLko,11
-gym_jiminy_toolbox-1.8.5.post1.dist-info/RECORD,,
+gym_jiminy/toolbox/wrappers/frame_rate_limiter.py,sha256=i0Fq24OXFt0KT9oIfLOsZmnJZcRPQe9SsbxCtRtXuAk,3136
+gym_jiminy/toolbox/wrappers/meta_envs.py,sha256=ka1POBD6S54EtVUoZyezhBfgi14_ta87HSrCGDApZbE,4980
+gym_jiminy_toolbox-1.8.6.dist-info/METADATA,sha256=dIHW_2tsNIMAWl_D9b_CkcNu8fPNgvZ_mDCEDGUQOLY,933
+gym_jiminy_toolbox-1.8.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+gym_jiminy_toolbox-1.8.6.dist-info/top_level.txt,sha256=c6Ipde11Sivat1D9sNj6sn3TCpadD0Qqk9fMzWYQLko,11
+gym_jiminy_toolbox-1.8.6.dist-info/RECORD,,
```


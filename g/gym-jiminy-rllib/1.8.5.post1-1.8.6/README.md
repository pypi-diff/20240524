# Comparing `tmp/gym_jiminy_rllib-1.8.5.post1-py3-none-any.whl.zip` & `tmp/gym_jiminy_rllib-1.8.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 25761 bytes, number of entries: 10
--rw-r--r--  2.0 unx      264 b- defN 24-Apr-30 00:34 gym_jiminy/rllib/__init__.py
--rw-r--r--  2.0 unx     3162 b- defN 24-Apr-30 00:34 gym_jiminy/rllib/callbacks.py
--rw-r--r--  2.0 unx    12290 b- defN 24-Apr-30 00:34 gym_jiminy/rllib/curriculum.py
--rw-r--r--  2.0 unx    28124 b- defN 24-Apr-30 00:34 gym_jiminy/rllib/ppo.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-30 00:34 gym_jiminy/rllib/py.typed
--rw-r--r--  2.0 unx    46565 b- defN 24-Apr-30 00:34 gym_jiminy/rllib/utilities.py
--rw-r--r--  2.0 unx      966 b- defN 24-Apr-30 00:35 gym_jiminy_rllib-1.8.5.post1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-30 00:35 gym_jiminy_rllib-1.8.5.post1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-30 00:35 gym_jiminy_rllib-1.8.5.post1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      862 b- defN 24-Apr-30 00:35 gym_jiminy_rllib-1.8.5.post1.dist-info/RECORD
-10 files, 92336 bytes uncompressed, 24275 bytes compressed:  73.7%
+Zip file size: 26896 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      264 b- defN 24-May-24 13:32 gym_jiminy/rllib/__init__.py
+-rw-r--r--  2.0 unx     3162 b- defN 24-May-24 13:32 gym_jiminy/rllib/callbacks.py
+-rw-r--r--  2.0 unx    12290 b- defN 24-May-24 13:32 gym_jiminy/rllib/curriculum.py
+-rw-r--r--  2.0 unx    31838 b- defN 24-May-24 13:32 gym_jiminy/rllib/ppo.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 13:32 gym_jiminy/rllib/py.typed
+-rw-r--r--  2.0 unx    47008 b- defN 24-May-24 13:32 gym_jiminy/rllib/utilities.py
+-rw-r--r--  2.0 unx      954 b- defN 24-May-24 13:33 gym_jiminy_rllib-1.8.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 13:33 gym_jiminy_rllib-1.8.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-24 13:33 gym_jiminy_rllib-1.8.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      838 b- defN 24-May-24 13:33 gym_jiminy_rllib-1.8.6.dist-info/RECORD
+10 files, 96457 bytes uncompressed, 25458 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: gym_jiminy/rllib/py.typed
 Comment: 
 
 Filename: gym_jiminy/rllib/utilities.py
 Comment: 
 
-Filename: gym_jiminy_rllib-1.8.5.post1.dist-info/METADATA
+Filename: gym_jiminy_rllib-1.8.6.dist-info/METADATA
 Comment: 
 
-Filename: gym_jiminy_rllib-1.8.5.post1.dist-info/WHEEL
+Filename: gym_jiminy_rllib-1.8.6.dist-info/WHEEL
 Comment: 
 
-Filename: gym_jiminy_rllib-1.8.5.post1.dist-info/top_level.txt
+Filename: gym_jiminy_rllib-1.8.6.dist-info/top_level.txt
 Comment: 
 
-Filename: gym_jiminy_rllib-1.8.5.post1.dist-info/RECORD
+Filename: gym_jiminy_rllib-1.8.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gym_jiminy/rllib/ppo.py

```diff
@@ -25,14 +25,15 @@
 from ray.rllib.policy.torch_policy_v2 import TorchPolicyV2
 from ray.rllib.policy.view_requirement import ViewRequirement
 from ray.rllib.algorithms.algorithm_config import AlgorithmConfig
 from ray.rllib.algorithms.ppo import PPOConfig as _PPOConfig, PPO as _PPO
 from ray.rllib.algorithms.ppo.ppo_torch_policy import (
     PPOTorchPolicy as _PPOTorchPolicy)
 from ray.rllib.algorithms.ppo.ppo_tf_policy import validate_config
+from ray.rllib.evaluation.postprocessing import Postprocessing
 from ray.rllib.utils.numpy import convert_to_numpy
 from ray.rllib.utils.torch_utils import l2_loss
 from ray.rllib.utils.annotations import override
 from ray.rllib.utils.typing import TensorType
 
 
 def get_action_mean(model: ModelV2,
@@ -198,14 +199,15 @@
         self.enable_adversarial_noise = False
         self.sgld_beta_inv = 1e-8
         self.sgld_n_steps = 10
         self.temporal_barrier_scale = 10.0
         self.temporal_barrier_threshold = float('inf')
         self.temporal_barrier_reg = 0.0
         self.symmetric_policy_reg = 0.0
+        self.enable_symmetry_surrogate_loss = False
         self.caps_temporal_reg = 0.0
         self.caps_spatial_reg = 0.0
         self.caps_global_reg = 0.0
         self.l2_reg = 0.0
 
     @override(_PPOConfig)
     def training(
@@ -215,14 +217,15 @@
         spatial_noise_scale: Optional[float] = None,
         sgld_beta_inv: Optional[float] = None,
         sgld_n_steps: Optional[int] = None,
         temporal_barrier_scale: Optional[float] = None,
         temporal_barrier_threshold: Optional[float] = None,
         temporal_barrier_reg: Optional[float] = None,
         symmetric_policy_reg: Optional[float] = None,
+        enable_symmetry_surrogate_loss: Optional[bool] = None,
         caps_temporal_reg: Optional[float] = None,
         caps_spatial_reg: Optional[float] = None,
         caps_global_reg: Optional[float] = None,
         l2_reg: Optional[float] = None,
         **kwargs: Any,
     ) -> "PPOConfig":
         # Pass kwargs onto super's `training()` method.
@@ -240,14 +243,17 @@
             self.temporal_barrier_scale = temporal_barrier_scale
         if temporal_barrier_threshold is not None:
             self.temporal_barrier_threshold = temporal_barrier_threshold
         if temporal_barrier_reg is not None:
             self.temporal_barrier_reg = temporal_barrier_reg
         if symmetric_policy_reg is not None:
             self.symmetric_policy_reg = symmetric_policy_reg
+        if enable_symmetry_surrogate_loss is not None:
+            self.enable_symmetry_surrogate_loss = \
+                enable_symmetry_surrogate_loss
         if caps_temporal_reg is not None:
             self.caps_temporal_reg = caps_temporal_reg
         if caps_spatial_reg is not None:
             self.caps_spatial_reg = caps_spatial_reg
         if caps_global_reg is not None:
             self.caps_global_reg = caps_global_reg
         if l2_reg is not None:
@@ -281,22 +287,43 @@
 
 
 class PPOTorchPolicy(_PPOTorchPolicy):
     """Add regularization losses on top of the original loss of PPO.
 
     More specifically, it adds:
         - CAPS regularization, which combines the spatial and temporal
-        difference between previous and current state
+        difference between previous and current state.
         - Global regularization, which is the average norm of the action
         - temporal barrier, which is exponential barrier loss when the
         normalized action is above a threshold (much like interior point
         methods).
         - symmetry regularization, which is the error between actions and
         symmetric actions associated with symmetric observations.
-        - L2 regularization of policy network weights
+        - symmetry surrogate loss, which is the surrogate loss associated
+        with the symmetric (actions, observations) spaces. As the surrogate
+        loss goal is to increase the likelihood of selecting higher reward
+        actions given the current state, the symmetry surrogate loss enables
+        equivalent likelihood increase for selecting the symmetric higher
+        reward actions given the symmetric state.
+        - L2 regularization of policy network weights.
+
+    More insights on the regularization losses with their emerging properties,
+    and on how to tune the parameters can be found in the reference articles:
+        - A. Duburcq, F. Schramm, G. Boeris, N. Bredeche, and Y. Chevaleyre,
+        “Reactive Stepping for Humanoid Robots using Reinforcement Learning:
+        Application to Standing Push Recovery on the Exoskeleton Atalante,” in
+        International Conference on Intelligent Robots and Systems (IROS),
+        vol. 2022-Octob. IEEE, oct 2022, pp. 9302–9309
+        - S. Mysore, B. Mabsout, R. Mancuso, and K. Saenko, “Regularizing
+        action policies for smooth control with reinforcement learning,”
+        IEEE International Conference on Robotics and Automation (ICRA),
+        pp. 1810–1816, 2021
+        - M. Mittal, N. Rudin, V. Klemm, A. Allshire, and M. Hutter,
+        “Symmetry considerations for learning task symmetric robot policies,”
+        arXiv preprint arXiv:2403.04359, 2024.
     """
     def __init__(self,
                  observation_space: gym.spaces.Space,
                  action_space: gym.spaces.Space,
                  config: Union[PPOConfig, Dict[str, Any]]) -> None:
         """Initialize PPO Torch policy.
 
@@ -331,15 +358,16 @@
         KLCoeffMixin.__init__(self, config_dict)
 
         # Extract and convert observation and action mirroring transform
         self.obs_mirror_mat: Optional[Union[
             Dict[str, torch.Tensor], torch.Tensor]] = None
         self.action_mirror_mat: Optional[Union[
             Dict[str, torch.Tensor], torch.Tensor]] = None
-        if config_dict["symmetric_policy_reg"] > 0.0:
+        if config_dict["symmetric_policy_reg"] > 0.0 or \
+                config_dict["enable_symmetry_surrogate_loss"]:
             # Observation space
             is_obs_dict = hasattr(observation_space, "original_space")
             if is_obs_dict:
                 observation_space = observation_space.\
                     original_space  # type: ignore[attr-defined]
                 self.obs_mirror_mat = {}
                 for field, mirror_mat in observation_space.\
@@ -382,14 +410,16 @@
     @override(_PPOTorchPolicy)
     def loss(self,
              model: ModelV2,
              dist_class: Type[ActionDistribution],
              train_batch: SampleBatch) -> Union[TensorType, List[TensorType]]:
         """Compute PPO loss with additional regularizations.
         """
+        # pylint: disable=possibly-used-before-assignment
+
         with torch.no_grad():
             # Extract some proxies from convenience
             observation_true = train_batch["obs"]
 
             # Initialize the various training batches to forward to the model
             train_batches = {"true": train_batch}
 
@@ -431,19 +461,20 @@
                     observation_true, self.config["spatial_noise_scale"])
 
                 # Replace current observation by the noisy one
                 train_batch_copy["obs"] = observation_noisy
 
                 # Append the training batches to the set
                 train_batches["noisy"] = train_batch_copy
-            if self.config["symmetric_policy_reg"] > 0.0:
+            if self.config["symmetric_policy_reg"] > 0.0 or \
+                    self.config["enable_symmetry_surrogate_loss"]:
                 # Shallow copy the original training batch
                 train_batch_copy = train_batch.copy(shallow=True)
 
-                # Compute mirrorred observation
+                # Compute mirrored observation
                 assert self.obs_mirror_mat is not None
                 assert isinstance(self.observation_space, gym.spaces.Box)
                 observation_mirror = _compute_mirrored_value(
                     observation_true,
                     self.observation_space,
                     self.obs_mirror_mat)
 
@@ -517,15 +548,16 @@
         if self.config["caps_spatial_reg"] > 0.0 and \
                 self.config["enable_adversarial_noise"]:
             action_worst_logits = action_logits["worst"]
             action_worst_mean = get_action_mean(
                 model, dist_class, action_worst_logits)
 
         # Compute the mirrored mean action corresponding to the mirrored action
-        if self.config["symmetric_policy_reg"] > 0.0:
+        if self.config["symmetric_policy_reg"] > 0.0 or \
+                self.config["enable_symmetry_surrogate_loss"]:
             assert self.action_mirror_mat is not None
             assert isinstance(self.action_space, gym.spaces.Box)
             action_mirror_logits = action_logits["mirrored"]
             action_mirror_mean = get_action_mean(
                 model, dist_class, action_mirror_logits)
             action_revert_mean = _compute_mirrored_value(
                 action_mirror_mean,
@@ -591,14 +623,44 @@
                 (action_revert_mean - action_true_mean) ** 2)
 
             # Add policy symmetry loss to total loss
             stats["symmetric_policy_reg"] = symmetric_policy_reg
             total_loss += \
                 self.config["symmetric_policy_reg"] * symmetric_policy_reg
 
+        if self.config["enable_symmetry_surrogate_loss"]:
+            assert self.action_mirror_mat is not None
+            assert isinstance(self.action_space, gym.spaces.Box)
+
+            # Get the mirror policy probability distribution
+            # i.e. ( x -> pi( x | mirrored observation ) )
+            curr_action_mirror_dist = dist_class(action_mirror_logits, model)
+
+            # The implementation assumes, at any time t, under the policy,
+            # the probability to be in state_t is equal to the probability to
+            # be in the mirrored state_t. Otherwise, their ratio needs to be
+            # added.
+            mirror_logp_ratio = torch.exp(
+                curr_action_mirror_dist.logp(
+                    _compute_mirrored_value(train_batch[SampleBatch.ACTIONS],
+                                            self.action_space,
+                                            self.action_mirror_mat)) -
+                train_batch[SampleBatch.ACTION_LOGP])
+
+            symmetry_surrogate_loss = torch.mean(torch.min(
+                train_batch[Postprocessing.ADVANTAGES] * mirror_logp_ratio,
+                train_batch[Postprocessing.ADVANTAGES] * torch.clamp(
+                    mirror_logp_ratio,
+                    1 - self.config["clip_param"],
+                    1 + self.config["clip_param"])))
+
+            # Add symmetry surrogate loss to total loss
+            stats["symmetry_surrogate_loss"] = symmetry_surrogate_loss
+            total_loss -= symmetry_surrogate_loss
+
         if self.config["l2_reg"] > 0.0:
             # Add actor l2-regularization loss
             l2_reg = 0.0
             assert isinstance(model, torch.nn.Module)
             for name, params in model.named_parameters():
                 if not name.endswith("bias") and params.requires_grad:
                     l2_reg += l2_loss(params)
@@ -611,14 +673,17 @@
 
     @override(_PPOTorchPolicy)
     def stats_fn(self, train_batch: SampleBatch) -> Dict[str, TensorType]:
         """Add regularization statistics.
         """
         stats_dict = super().stats_fn(train_batch)
 
+        if self.config["enable_symmetry_surrogate_loss"]:
+            stats_dict["symmetry_surrogate_loss"] = torch.mean(
+                torch.stack(self.get_tower_stats("symmetry_surrogate_loss")))
         if self.config["symmetric_policy_reg"] > 0.0:
             stats_dict["symmetry"] = torch.mean(
                 torch.stack(self.get_tower_stats("symmetric_policy_reg")))
         if self.config["temporal_barrier_reg"] > 0.0:
             stats_dict["temporal_barrier"] = torch.mean(
                 torch.stack(self.get_tower_stats("temporal_barrier_reg")))
         if self.config["caps_temporal_reg"] > 0.0:
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## gym_jiminy/rllib/utilities.py

```diff
@@ -1,8 +1,14 @@
-""" TODO: Write documentation.
+"""This module provides helper methods to make it easier to run learning
+pipelines using Ray-RLlib framework.
+
+The main focus are:
+  * making it easy to build a policy from a checkpoint
+  * enabling evaluating the performance of a given policy without having to
+    fire up a whole ray server instance, which is normally required
 """
 import os
 import re
 import json
 import time
 import shutil
 import socket
@@ -483,15 +489,16 @@
             for field in PRINT_RESULT_FIELDS_FILTER:
                 if field in result.keys():
                     msg_data.append(f"{field}: {result[field]:.5g}")
             print(" - ".join(msg_data))
 
             # Backup the policy
             if checkpoint_period > 0 and iter_num % checkpoint_period == 0:
-                algo.save()
+                algo.save(
+                    checkpoint_dir=f"{algo.logdir}/checkpoint_{iter_num:06d}")
 
             # Check terminal conditions
             if 0 < max_timesteps < result["timesteps_total"]:
                 break
             if 0 < max_iters < iter_num:
                 break
             if reward_threshold < result["episode_reward_mean"]:
@@ -506,15 +513,16 @@
 
     # Flush and close logger before returning
     if result_logger is not None:
         result_logger.flush()
         result_logger.close()
 
     # Backup trained agent and return file location
-    return algo.save()
+    return algo.save(
+        checkpoint_dir=f"{algo.logdir}/checkpoint_{iter_num:06d}")
 
 
 def _restore_default_connectors() -> None:
     """Restore default connectors.
 
     They would no longer exists after calling `ray.shutdown`, otherwise this
     is a no-op. This is necessary to restore policies resorting on agent and
```

## Comparing `gym_jiminy_rllib-1.8.5.post1.dist-info/METADATA` & `gym_jiminy_rllib-1.8.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-jiminy-rllib
-Version: 1.8.5.post1
+Version: 1.8.6
 Summary: Specialized Reinforcement learning toolbox based on Ray RLlib for Gym Jiminy.
 Author: Alexis Duburcq
 Author-email: alexis.duburcq@gmail.com
 Maintainer: Alexis Duburcq
 License: MIT
 Keywords: reinforcement-learning robotics gym jiminy
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,12 +13,12 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8,<3.12
-Requires-Dist: gym-jiminy ~=1.8.5.post1
+Requires-Dist: gym-jiminy ~=1.8.6
 Requires-Dist: ray[rllib] ~=2.9.0
 Requires-Dist: tensorboardX
 Requires-Dist: plotext >=5.0.0
```


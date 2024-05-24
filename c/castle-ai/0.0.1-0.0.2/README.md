# Comparing `tmp/castle_ai-0.0.1.tar.gz` & `tmp/castle_ai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "castle_ai-0.0.1.tar", last modified: Thu May 23 01:13:46 2024, max compression
+gzip compressed data, was "castle_ai-0.0.2.tar", last modified: Thu May 23 10:09:17 2024, max compression
```

## Comparing `castle_ai-0.0.1.tar` & `castle_ai-0.0.2.tar`

### file list

```diff
@@ -1,122 +1,124 @@
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 01:13:46.144713 castle_ai-0.0.1/
--rw-r--r--   0 raiso     (1000) raiso     (1000)     1713 2024-05-23 01:13:46.144713 castle_ai-0.0.1/PKG-INFO
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      877 2024-05-22 06:57:29.000000 castle_ai-0.0.1/README.md
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 01:13:46.140713 castle_ai-0.0.1/castle/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)       20 2024-05-22 04:34:06.000000 castle_ai-0.0.1/castle/__init__.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 01:13:46.140713 castle_ai-0.0.1/castle/aot/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)       31 2024-05-22 04:48:14.000000 castle_ai-0.0.1/castle/aot/__init__.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 01:13:46.140713 castle_ai-0.0.1/castle/aot/configs/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-23 00:30:16.000000 castle_ai-0.0.1/castle/aot/configs/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     5566 2024-05-22 06:28:08.000000 castle_ai-0.0.1/castle/aot/configs/default.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 01:13:46.140713 castle_ai-0.0.1/castle/aot/configs/models/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-23 00:32:03.000000 castle_ai-0.0.1/castle/aot/configs/models/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      207 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/configs/models/aotb.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      289 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/configs/models/aotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      207 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/configs/models/aots.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      174 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/configs/models/aott.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      206 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/configs/models/deaotb.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      289 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/configs/models/deaotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      206 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/configs/models/deaots.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      173 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/configs/models/deaott.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      957 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/configs/models/default.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      420 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/configs/models/default_deaot.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      545 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/configs/models/r101_aotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      541 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/configs/models/r50_aotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      410 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/configs/models/r50_deaotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      585 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/configs/models/rs101_aotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      645 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/configs/models/swinb_aotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      451 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/configs/models/swinb_deaotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      513 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/configs/pre.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      690 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/configs/pre_dav.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      611 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/configs/pre_ytb.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      668 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/configs/pre_ytb_dav.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      251 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/configs/ytb.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 01:13:46.140713 castle_ai-0.0.1/castle/aot/dataloaders/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/dataloaders/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    14300 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/dataloaders/eval_datasets.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    19828 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/dataloaders/image_transforms.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    24642 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/dataloaders/train_datasets.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    23561 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/dataloaders/video_transforms.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 01:13:46.140713 castle_ai-0.0.1/castle/aot/networks/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 04:49:47.000000 castle_ai-0.0.1/castle/aot/networks/__init__.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 01:13:46.140713 castle_ai-0.0.1/castle/aot/networks/decoders/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      186 2024-05-22 05:12:26.000000 castle_ai-0.0.1/castle/aot/networks/decoders/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     2079 2024-05-22 05:13:06.000000 castle_ai-0.0.1/castle/aot/networks/decoders/fpn.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 01:13:46.140713 castle_ai-0.0.1/castle/aot/networks/encoders/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     1307 2024-05-22 05:08:31.000000 castle_ai-0.0.1/castle/aot/networks/encoders/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     8427 2024-05-22 05:06:53.000000 castle_ai-0.0.1/castle/aot/networks/encoders/mobilenetv2.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     7907 2024-05-22 05:07:00.000000 castle_ai-0.0.1/castle/aot/networks/encoders/mobilenetv3.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 01:13:46.140713 castle_ai-0.0.1/castle/aot/networks/encoders/resnest/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)       23 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/networks/encoders/resnest/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     3343 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/networks/encoders/resnest/resnest.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    16481 2024-05-22 05:10:30.000000 castle_ai-0.0.1/castle/aot/networks/encoders/resnest/resnet.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     4467 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/networks/encoders/resnest/splat.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     6699 2024-05-22 05:07:30.000000 castle_ai-0.0.1/castle/aot/networks/encoders/resnet.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 01:13:46.140713 castle_ai-0.0.1/castle/aot/networks/encoders/swin/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)       35 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/networks/encoders/swin/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      987 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/networks/encoders/swin/build.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    27369 2024-05-22 05:10:57.000000 castle_ai-0.0.1/castle/aot/networks/encoders/swin/swin_transformer.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 01:13:46.140713 castle_ai-0.0.1/castle/aot/networks/engines/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      653 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/networks/engines/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    25206 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/networks/engines/aot_engine.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     5978 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/networks/engines/deaot_engine.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 01:13:46.144713 castle_ai-0.0.1/castle/aot/networks/layers/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/networks/layers/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    32865 2024-05-22 05:11:50.000000 castle_ai-0.0.1/castle/aot/networks/layers/attention.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     5111 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/networks/layers/basic.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     6698 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/networks/layers/loss.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     1700 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/networks/layers/normalization.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     2834 2024-05-22 05:12:08.000000 castle_ai-0.0.1/castle/aot/networks/layers/position.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    24810 2024-05-22 05:11:35.000000 castle_ai-0.0.1/castle/aot/networks/layers/transformer.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 01:13:46.144713 castle_ai-0.0.1/castle/aot/networks/models/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      358 2024-05-22 04:45:04.000000 castle_ai-0.0.1/castle/aot/networks/models/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     4574 2024-05-22 05:03:48.000000 castle_ai-0.0.1/castle/aot/networks/models/aot.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     2109 2024-05-22 05:13:44.000000 castle_ai-0.0.1/castle/aot/networks/models/deaot.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 01:13:46.144713 castle_ai-0.0.1/castle/aot/utils/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/utils/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     6233 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/utils/checkpoint.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     1358 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/utils/cp_ckpt.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     3561 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/utils/ema.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      443 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/utils/eval.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     6075 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/utils/image.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     3454 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/utils/learning.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      829 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/utils/math.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      860 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/utils/meters.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     1102 2024-05-22 03:59:14.000000 castle_ai-0.0.1/castle/aot/utils/metric.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 01:13:46.144713 castle_ai-0.0.1/castle/sam/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 04:03:33.000000 castle_ai-0.0.1/castle/sam/__init__.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 01:13:46.144713 castle_ai-0.0.1/castle/sam/segment_anything/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      427 2024-05-22 04:03:33.000000 castle_ai-0.0.1/castle/sam/segment_anything/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    15132 2024-05-22 04:03:33.000000 castle_ai-0.0.1/castle/sam/segment_anything/automatic_mask_generator.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     2941 2024-05-22 04:03:33.000000 castle_ai-0.0.1/castle/sam/segment_anything/build_sam.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 01:13:46.144713 castle_ai-0.0.1/castle/sam/segment_anything/modeling/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      385 2024-05-22 04:03:33.000000 castle_ai-0.0.1/castle/sam/segment_anything/modeling/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     1479 2024-05-22 04:03:33.000000 castle_ai-0.0.1/castle/sam/segment_anything/modeling/common.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    14407 2024-05-22 04:03:33.000000 castle_ai-0.0.1/castle/sam/segment_anything/modeling/image_encoder.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     6614 2024-05-22 04:03:33.000000 castle_ai-0.0.1/castle/sam/segment_anything/modeling/mask_decoder.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     8594 2024-05-22 04:03:33.000000 castle_ai-0.0.1/castle/sam/segment_anything/modeling/prompt_encoder.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     7225 2024-05-22 04:03:33.000000 castle_ai-0.0.1/castle/sam/segment_anything/modeling/sam.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     8396 2024-05-22 04:03:33.000000 castle_ai-0.0.1/castle/sam/segment_anything/modeling/transformer.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    11818 2024-05-22 04:03:33.000000 castle_ai-0.0.1/castle/sam/segment_anything/predictor.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 01:13:46.144713 castle_ai-0.0.1/castle/sam/segment_anything/utils/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      197 2024-05-22 04:03:33.000000 castle_ai-0.0.1/castle/sam/segment_anything/utils/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    12711 2024-05-22 04:03:33.000000 castle_ai-0.0.1/castle/sam/segment_anything/utils/amg.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     5790 2024-05-22 04:03:33.000000 castle_ai-0.0.1/castle/sam/segment_anything/utils/onnx.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     3968 2024-05-22 04:03:33.000000 castle_ai-0.0.1/castle/sam/segment_anything/utils/transforms.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      541 2024-05-22 04:03:33.000000 castle_ai-0.0.1/castle/sam/setup.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 01:13:46.144713 castle_ai-0.0.1/castle/utils/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)       46 2024-05-22 04:34:17.000000 castle_ai-0.0.1/castle/utils/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 04:05:47.000000 castle_ai-0.0.1/castle/utils/image_segment.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      876 2024-05-23 00:43:48.000000 castle_ai-0.0.1/castle/utils/plot.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     2524 2024-05-22 04:09:41.000000 castle_ai-0.0.1/castle/utils/video_io.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     7910 2024-05-22 06:39:01.000000 castle_ai-0.0.1/castle/utils/video_object_segment.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 04:05:52.000000 castle_ai-0.0.1/castle/utils/visual_latent_extract.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 01:13:46.144713 castle_ai-0.0.1/castle_ai.egg-info/
--rw-r--r--   0 raiso     (1000) raiso     (1000)     1713 2024-05-23 01:13:46.000000 castle_ai-0.0.1/castle_ai.egg-info/PKG-INFO
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     3621 2024-05-23 01:13:46.000000 castle_ai-0.0.1/castle_ai.egg-info/SOURCES.txt
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        1 2024-05-23 01:13:46.000000 castle_ai-0.0.1/castle_ai.egg-info/dependency_links.txt
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        1 2024-05-23 00:05:44.000000 castle_ai-0.0.1/castle_ai.egg-info/not-zip-safe
--rw-rw-r--   0 raiso     (1000) raiso     (1000)       57 2024-05-23 01:13:46.000000 castle_ai-0.0.1/castle_ai.egg-info/requires.txt
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        7 2024-05-23 01:13:46.000000 castle_ai-0.0.1/castle_ai.egg-info/top_level.txt
--rw-rw-r--   0 raiso     (1000) raiso     (1000)       38 2024-05-23 01:13:46.144713 castle_ai-0.0.1/setup.cfg
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     1982 2024-05-23 01:13:44.000000 castle_ai-0.0.1/setup.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 10:09:17.530343 castle_ai-0.0.2/
+-rw-r--r--   0 raiso     (1000) raiso     (1000)     1699 2024-05-23 10:09:17.530343 castle_ai-0.0.2/PKG-INFO
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      863 2024-05-23 10:04:50.000000 castle_ai-0.0.2/README.md
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 10:09:17.526343 castle_ai-0.0.2/castle/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)       20 2024-05-22 04:34:06.000000 castle_ai-0.0.2/castle/__init__.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 10:09:17.526343 castle_ai-0.0.2/castle/aot/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)       31 2024-05-22 04:48:14.000000 castle_ai-0.0.2/castle/aot/__init__.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 10:09:17.526343 castle_ai-0.0.2/castle/aot/configs/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-23 00:30:16.000000 castle_ai-0.0.2/castle/aot/configs/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     5566 2024-05-22 06:28:08.000000 castle_ai-0.0.2/castle/aot/configs/default.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 10:09:17.526343 castle_ai-0.0.2/castle/aot/configs/models/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-23 00:32:03.000000 castle_ai-0.0.2/castle/aot/configs/models/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      207 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/configs/models/aotb.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      289 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/configs/models/aotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      207 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/configs/models/aots.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      174 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/configs/models/aott.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      206 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/configs/models/deaotb.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      289 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/configs/models/deaotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      206 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/configs/models/deaots.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      173 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/configs/models/deaott.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      957 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/configs/models/default.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      420 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/configs/models/default_deaot.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      545 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/configs/models/r101_aotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      541 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/configs/models/r50_aotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      410 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/configs/models/r50_deaotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      585 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/configs/models/rs101_aotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      645 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/configs/models/swinb_aotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      451 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/configs/models/swinb_deaotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      513 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/configs/pre.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      690 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/configs/pre_dav.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      611 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/configs/pre_ytb.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      668 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/configs/pre_ytb_dav.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      251 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/configs/ytb.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 10:09:17.526343 castle_ai-0.0.2/castle/aot/dataloaders/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/dataloaders/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    14300 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/dataloaders/eval_datasets.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    19828 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/dataloaders/image_transforms.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    24642 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/dataloaders/train_datasets.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    23561 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/dataloaders/video_transforms.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 10:09:17.526343 castle_ai-0.0.2/castle/aot/networks/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 04:49:47.000000 castle_ai-0.0.2/castle/aot/networks/__init__.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 10:09:17.526343 castle_ai-0.0.2/castle/aot/networks/decoders/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      186 2024-05-22 05:12:26.000000 castle_ai-0.0.2/castle/aot/networks/decoders/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2079 2024-05-22 05:13:06.000000 castle_ai-0.0.2/castle/aot/networks/decoders/fpn.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 10:09:17.526343 castle_ai-0.0.2/castle/aot/networks/encoders/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1307 2024-05-22 05:08:31.000000 castle_ai-0.0.2/castle/aot/networks/encoders/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     8427 2024-05-22 05:06:53.000000 castle_ai-0.0.2/castle/aot/networks/encoders/mobilenetv2.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     7907 2024-05-22 05:07:00.000000 castle_ai-0.0.2/castle/aot/networks/encoders/mobilenetv3.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 10:09:17.526343 castle_ai-0.0.2/castle/aot/networks/encoders/resnest/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)       23 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/networks/encoders/resnest/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     3343 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/networks/encoders/resnest/resnest.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    16481 2024-05-22 05:10:30.000000 castle_ai-0.0.2/castle/aot/networks/encoders/resnest/resnet.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     4467 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/networks/encoders/resnest/splat.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     6699 2024-05-22 05:07:30.000000 castle_ai-0.0.2/castle/aot/networks/encoders/resnet.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 10:09:17.526343 castle_ai-0.0.2/castle/aot/networks/encoders/swin/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)       35 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/networks/encoders/swin/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      987 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/networks/encoders/swin/build.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    27369 2024-05-22 05:10:57.000000 castle_ai-0.0.2/castle/aot/networks/encoders/swin/swin_transformer.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 10:09:17.526343 castle_ai-0.0.2/castle/aot/networks/engines/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      653 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/networks/engines/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    25206 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/networks/engines/aot_engine.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     5978 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/networks/engines/deaot_engine.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 10:09:17.526343 castle_ai-0.0.2/castle/aot/networks/layers/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/networks/layers/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    32865 2024-05-22 05:11:50.000000 castle_ai-0.0.2/castle/aot/networks/layers/attention.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     5111 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/networks/layers/basic.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     6698 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/networks/layers/loss.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1700 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/networks/layers/normalization.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2834 2024-05-22 05:12:08.000000 castle_ai-0.0.2/castle/aot/networks/layers/position.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    24810 2024-05-22 05:11:35.000000 castle_ai-0.0.2/castle/aot/networks/layers/transformer.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 10:09:17.530343 castle_ai-0.0.2/castle/aot/networks/models/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      358 2024-05-22 04:45:04.000000 castle_ai-0.0.2/castle/aot/networks/models/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     4574 2024-05-22 05:03:48.000000 castle_ai-0.0.2/castle/aot/networks/models/aot.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2109 2024-05-22 05:13:44.000000 castle_ai-0.0.2/castle/aot/networks/models/deaot.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 10:09:17.530343 castle_ai-0.0.2/castle/aot/utils/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/utils/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     6233 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/utils/checkpoint.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1358 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/utils/cp_ckpt.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     3561 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/utils/ema.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      443 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/utils/eval.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     6075 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/utils/image.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     3454 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/utils/learning.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      829 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/utils/math.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      860 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/utils/meters.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1102 2024-05-22 03:59:14.000000 castle_ai-0.0.2/castle/aot/utils/metric.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 10:09:17.530343 castle_ai-0.0.2/castle/sam/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 04:03:33.000000 castle_ai-0.0.2/castle/sam/__init__.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 10:09:17.530343 castle_ai-0.0.2/castle/sam/segment_anything/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      427 2024-05-22 04:03:33.000000 castle_ai-0.0.2/castle/sam/segment_anything/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    15132 2024-05-22 04:03:33.000000 castle_ai-0.0.2/castle/sam/segment_anything/automatic_mask_generator.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2941 2024-05-22 04:03:33.000000 castle_ai-0.0.2/castle/sam/segment_anything/build_sam.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 10:09:17.530343 castle_ai-0.0.2/castle/sam/segment_anything/modeling/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      385 2024-05-22 04:03:33.000000 castle_ai-0.0.2/castle/sam/segment_anything/modeling/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1479 2024-05-22 04:03:33.000000 castle_ai-0.0.2/castle/sam/segment_anything/modeling/common.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    14407 2024-05-22 04:03:33.000000 castle_ai-0.0.2/castle/sam/segment_anything/modeling/image_encoder.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     6614 2024-05-22 04:03:33.000000 castle_ai-0.0.2/castle/sam/segment_anything/modeling/mask_decoder.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     8594 2024-05-22 04:03:33.000000 castle_ai-0.0.2/castle/sam/segment_anything/modeling/prompt_encoder.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     7225 2024-05-22 04:03:33.000000 castle_ai-0.0.2/castle/sam/segment_anything/modeling/sam.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     8396 2024-05-22 04:03:33.000000 castle_ai-0.0.2/castle/sam/segment_anything/modeling/transformer.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    11818 2024-05-22 04:03:33.000000 castle_ai-0.0.2/castle/sam/segment_anything/predictor.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 10:09:17.530343 castle_ai-0.0.2/castle/sam/segment_anything/utils/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      197 2024-05-22 04:03:33.000000 castle_ai-0.0.2/castle/sam/segment_anything/utils/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    12711 2024-05-22 04:03:33.000000 castle_ai-0.0.2/castle/sam/segment_anything/utils/amg.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     5790 2024-05-22 04:03:33.000000 castle_ai-0.0.2/castle/sam/segment_anything/utils/onnx.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     3968 2024-05-22 04:03:33.000000 castle_ai-0.0.2/castle/sam/segment_anything/utils/transforms.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      541 2024-05-22 04:03:33.000000 castle_ai-0.0.2/castle/sam/setup.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 10:09:17.530343 castle_ai-0.0.2/castle/utils/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)       85 2024-05-23 08:43:44.000000 castle_ai-0.0.2/castle/utils/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1002 2024-05-23 07:41:10.000000 castle_ai-0.0.2/castle/utils/download.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     6382 2024-05-23 08:44:58.000000 castle_ai-0.0.2/castle/utils/image_segment.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      881 2024-05-23 09:47:44.000000 castle_ai-0.0.2/castle/utils/plot.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-23 09:11:10.000000 castle_ai-0.0.2/castle/utils/video_align.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2524 2024-05-22 04:09:41.000000 castle_ai-0.0.2/castle/utils/video_io.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     8545 2024-05-23 07:50:24.000000 castle_ai-0.0.2/castle/utils/video_object_segment.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 04:05:52.000000 castle_ai-0.0.2/castle/utils/visual_latent_extract.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-23 10:09:17.530343 castle_ai-0.0.2/castle_ai.egg-info/
+-rw-r--r--   0 raiso     (1000) raiso     (1000)     1699 2024-05-23 10:09:17.000000 castle_ai-0.0.2/castle_ai.egg-info/PKG-INFO
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     3674 2024-05-23 10:09:17.000000 castle_ai-0.0.2/castle_ai.egg-info/SOURCES.txt
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        1 2024-05-23 10:09:17.000000 castle_ai-0.0.2/castle_ai.egg-info/dependency_links.txt
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        1 2024-05-23 00:05:44.000000 castle_ai-0.0.2/castle_ai.egg-info/not-zip-safe
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)       57 2024-05-23 10:09:17.000000 castle_ai-0.0.2/castle_ai.egg-info/requires.txt
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        7 2024-05-23 10:09:17.000000 castle_ai-0.0.2/castle_ai.egg-info/top_level.txt
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)       38 2024-05-23 10:09:17.530343 castle_ai-0.0.2/setup.cfg
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1982 2024-05-23 10:08:55.000000 castle_ai-0.0.2/setup.py
```

### Comparing `castle_ai-0.0.1/PKG-INFO` & `castle_ai-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: castle-ai
-Version: 0.0.1
+Version: 0.0.2
 Summary: Distinguish behavioral clusters Toolbox
 Maintainer: Raiso Liu
 Maintainer-email: rainsoon717@gmail.com
 License: AGPL-3.0 license
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -22,43 +22,23 @@
 Requires-Dist: av
 Requires-Dist: opencv-python
 Requires-Dist: torchvision
 Requires-Dist: matplotlib
 
 # CASTLE
 
-CASTLE integrates the strengths of visual foundation models trained on large datasets possess open-world visual concepts, including Segment Anything (SA), DeAOT, and DINOv2, for one-shot image segmentation and unsupervised visual feature extraction. Furthermore, CASTLE employs unsupervised multi-stage and/or multi-layer UMAP clustering algorithms to distinguish behavioral clusters with unique temporal variability. 
 
-# Install
-```
-git clone https://github.com/RaisoLiu/castle-animal.git
-cd castle-animal
-python install .
-```
+[![PyPI version](https://badge.fury.io/py/castle-ai.svg)](https://badge.fury.io/py/castle-ai)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](???)
 
-# Example
+CASTLE integrates the strengths of visual foundation models trained on large datasets possess open-world visual concepts, including Segment Anything (SA), DeAOT, and DINOv2, for one-shot image segmentation and unsupervised visual feature extraction. Furthermore, CASTLE employs unsupervised multi-stage and/or multi-layer UMAP clustering algorithms to distinguish behavioral clusters with unique temporal variability. 
 
-## Image segmentation
-```python
-1+1
+# Install
 ```
-
-## Video objects segmentation
-```python
-from castle import generate_aot
-
-tracker = generate_aot(ckpt_path, MODEL, DEVICE)
-tracker.add_reference_frame(frame, mask, num_object)
-
-
-new_mask = 
+pip install castle-ai
 ```
 
-## Visual latent extractioin
-```python
-1+1
-```
+# Reference
 
-## UMAP & HDBSCAN analysis
-```python
-1+1
-```
+[Segment Anything](https://github.com/facebookresearch/segment-anything.git)
+[DeAOT](https://github.com/z-x-yang/Segment-and-Track-Anything.git)
+[DINOv2](https://github.com/facebookresearch/dinov2.git)
```

### Comparing `castle_ai-0.0.1/castle/aot/configs/default.py` & `castle_ai-0.0.2/castle/aot/configs/default.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/configs/models/default.py` & `castle_ai-0.0.2/castle/aot/configs/models/default.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/configs/models/r101_aotl.py` & `castle_ai-0.0.2/castle/aot/configs/models/r101_aotl.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/configs/models/r50_aotl.py` & `castle_ai-0.0.2/castle/aot/configs/models/r50_aotl.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/configs/models/rs101_aotl.py` & `castle_ai-0.0.2/castle/aot/configs/models/rs101_aotl.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/configs/models/swinb_aotl.py` & `castle_ai-0.0.2/castle/aot/configs/models/swinb_aotl.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/configs/pre.py` & `castle_ai-0.0.2/castle/aot/configs/pre.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/configs/pre_dav.py` & `castle_ai-0.0.2/castle/aot/configs/pre_dav.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/configs/pre_ytb.py` & `castle_ai-0.0.2/castle/aot/configs/pre_ytb.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/configs/pre_ytb_dav.py` & `castle_ai-0.0.2/castle/aot/configs/pre_ytb_dav.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/dataloaders/eval_datasets.py` & `castle_ai-0.0.2/castle/aot/dataloaders/eval_datasets.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/dataloaders/image_transforms.py` & `castle_ai-0.0.2/castle/aot/dataloaders/image_transforms.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/dataloaders/train_datasets.py` & `castle_ai-0.0.2/castle/aot/dataloaders/train_datasets.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/dataloaders/video_transforms.py` & `castle_ai-0.0.2/castle/aot/dataloaders/video_transforms.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/networks/decoders/fpn.py` & `castle_ai-0.0.2/castle/aot/networks/decoders/fpn.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/networks/encoders/__init__.py` & `castle_ai-0.0.2/castle/aot/networks/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/networks/encoders/mobilenetv2.py` & `castle_ai-0.0.2/castle/aot/networks/encoders/mobilenetv2.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/networks/encoders/mobilenetv3.py` & `castle_ai-0.0.2/castle/aot/networks/encoders/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/networks/encoders/resnest/resnest.py` & `castle_ai-0.0.2/castle/aot/networks/encoders/resnest/resnest.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/networks/encoders/resnest/resnet.py` & `castle_ai-0.0.2/castle/aot/networks/encoders/resnest/resnet.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/networks/encoders/resnest/splat.py` & `castle_ai-0.0.2/castle/aot/networks/encoders/resnest/splat.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/networks/encoders/resnet.py` & `castle_ai-0.0.2/castle/aot/networks/encoders/resnet.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/networks/encoders/swin/build.py` & `castle_ai-0.0.2/castle/aot/networks/encoders/swin/build.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/networks/encoders/swin/swin_transformer.py` & `castle_ai-0.0.2/castle/aot/networks/encoders/swin/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/networks/engines/__init__.py` & `castle_ai-0.0.2/castle/aot/networks/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/networks/engines/aot_engine.py` & `castle_ai-0.0.2/castle/aot/networks/engines/aot_engine.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/networks/engines/deaot_engine.py` & `castle_ai-0.0.2/castle/aot/networks/engines/deaot_engine.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/networks/layers/attention.py` & `castle_ai-0.0.2/castle/aot/networks/layers/attention.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/networks/layers/basic.py` & `castle_ai-0.0.2/castle/aot/networks/layers/basic.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/networks/layers/loss.py` & `castle_ai-0.0.2/castle/aot/networks/layers/loss.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/networks/layers/normalization.py` & `castle_ai-0.0.2/castle/aot/networks/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/networks/layers/position.py` & `castle_ai-0.0.2/castle/aot/networks/layers/position.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/networks/layers/transformer.py` & `castle_ai-0.0.2/castle/aot/networks/layers/transformer.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/networks/models/aot.py` & `castle_ai-0.0.2/castle/aot/networks/models/aot.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/networks/models/deaot.py` & `castle_ai-0.0.2/castle/aot/networks/models/deaot.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/utils/checkpoint.py` & `castle_ai-0.0.2/castle/aot/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/utils/cp_ckpt.py` & `castle_ai-0.0.2/castle/aot/utils/cp_ckpt.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/utils/ema.py` & `castle_ai-0.0.2/castle/aot/utils/ema.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/utils/image.py` & `castle_ai-0.0.2/castle/aot/utils/image.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/utils/learning.py` & `castle_ai-0.0.2/castle/aot/utils/learning.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/utils/math.py` & `castle_ai-0.0.2/castle/aot/utils/math.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/utils/meters.py` & `castle_ai-0.0.2/castle/aot/utils/meters.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/aot/utils/metric.py` & `castle_ai-0.0.2/castle/aot/utils/metric.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/sam/segment_anything/automatic_mask_generator.py` & `castle_ai-0.0.2/castle/sam/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/sam/segment_anything/build_sam.py` & `castle_ai-0.0.2/castle/sam/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/sam/segment_anything/modeling/common.py` & `castle_ai-0.0.2/castle/sam/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/sam/segment_anything/modeling/image_encoder.py` & `castle_ai-0.0.2/castle/sam/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/sam/segment_anything/modeling/mask_decoder.py` & `castle_ai-0.0.2/castle/sam/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/sam/segment_anything/modeling/prompt_encoder.py` & `castle_ai-0.0.2/castle/sam/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/sam/segment_anything/modeling/sam.py` & `castle_ai-0.0.2/castle/sam/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/sam/segment_anything/modeling/transformer.py` & `castle_ai-0.0.2/castle/sam/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/sam/segment_anything/predictor.py` & `castle_ai-0.0.2/castle/sam/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/sam/segment_anything/utils/amg.py` & `castle_ai-0.0.2/castle/sam/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/sam/segment_anything/utils/onnx.py` & `castle_ai-0.0.2/castle/sam/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/sam/segment_anything/utils/transforms.py` & `castle_ai-0.0.2/castle/sam/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/sam/setup.py` & `castle_ai-0.0.2/castle/sam/setup.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/utils/plot.py` & `castle_ai-0.0.2/castle/utils/plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import numpy as np
 from PIL import Image
 
-_palette_hex = ['#BCECF4', '#FAE3F2', '#B7ECAB', '#C1B5EA', '#E29DC0', '#AECBEA', '#F7DCAF']
+_palette_hex = ['#7AE4F0', '#FFD0EC', '#6EE368', '#C1B5EA', '#9E83E3', '#A7CCED', '#FBC471']
 
 _palette = [0,0,0]
 for hex_code in _palette_hex:
     r, g, b = int(hex_code[1:3], 16), int(hex_code[3:5], 16), int(hex_code[5:7], 16)
     _palette.extend([r, g, b])
+    
 
 def colorize_mask(pred_mask):
     save_mask = Image.fromarray(pred_mask.astype(np.uint8))
     save_mask = save_mask.convert(mode='P')
     save_mask.putpalette(_palette)
     save_mask = save_mask.convert(mode='RGB')
     return np.array(save_mask)
```

### Comparing `castle_ai-0.0.1/castle/utils/video_io.py` & `castle_ai-0.0.2/castle/utils/video_io.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.1/castle/utils/video_object_segment.py` & `castle_ai-0.0.2/castle/utils/video_object_segment.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from castle.aot.networks.engines.deaot_engine import DeAOTEngine,DeAOTInferEngine
 import importlib
 import numpy as np
 
 
 from castle.aot.dataloaders import video_transforms as tr
 from castle.aot.utils.checkpoint import load_network
-from castle import aot
 from castle.aot.networks.models import build_vos_model
 from castle.aot.networks.engines import build_engine
+from .download import download_with_gdown
 from torchvision import transforms
 torch.backends.cudnn.benchmark = True
 
 class AOTTracker(object):
     def __init__(self, cfg, device):
         self.device = device
         self.model = build_vos_model(cfg.MODEL_VOS, cfg)
@@ -172,20 +172,37 @@
                 
             if img_embs is None:  # reuse image embeddings
                 img_embs = aot_engine.curr_enc_embs
 
         self.update_size()
 
 
-def generate_aot(ckpt_path, model_type='r50_deaotl', device='cuda'):
+def download_aot_ckpt(model_type):
+    if model_type == 'r50_deaotl':
+        ckpt_path = 'ckpt/R50_DeAOTL_PRE_YTB_DAV.pth'
+        download_with_gdown('1QoChMkTVxdYZ_eBlZhK2acq9KMQZccPJ', ckpt_path)
+        return ckpt_path
+    elif model_type == 'swinb_deaotl':
+        ckpt_path = 'ckpt/SwinB_DeAOTL_PRE_YTB_DAV.pth'
+        download_with_gdown('1g4E-F0RPOx9Nd6J7tU9AE1TjsouL4oZq', ckpt_path)
+        return ckpt_path
+    else:
+        assert False, f"model_type mismatch {model_type}, expect r50_deaotl or swinb_deaotl"
+
+def generate_aot(ckpt_path='', model_type='r50_deaotl', device='cuda'):
+    
+    if len(ckpt_path) == 0:
+        ckpt_path = download_aot_ckpt(model_type)
+
+
     args = {
         'phase': 'PRE_YTB_DAV',
         'model': model_type,
         'model_path': ckpt_path,
-        'long_term_mem_gap': 99999,
+        'long_term_mem_gap': int(1e6),
         'max_len_long_term': 30,
         'device': device,
     }
     engine_config = importlib.import_module('castle.aot.configs.' + 'pre_ytb_dav')
     cfg = engine_config.EngineConfig(args['phase'], args['model'])
     cfg.TEST_CKPT_PATH = args['model_path']
     cfg.TEST_LONG_TERM_MEM_GAP = args['long_term_mem_gap']
```

### Comparing `castle_ai-0.0.1/castle_ai.egg-info/PKG-INFO` & `castle_ai-0.0.2/castle_ai.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: castle-ai
-Version: 0.0.1
+Version: 0.0.2
 Summary: Distinguish behavioral clusters Toolbox
 Maintainer: Raiso Liu
 Maintainer-email: rainsoon717@gmail.com
 License: AGPL-3.0 license
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -22,43 +22,23 @@
 Requires-Dist: av
 Requires-Dist: opencv-python
 Requires-Dist: torchvision
 Requires-Dist: matplotlib
 
 # CASTLE
 
-CASTLE integrates the strengths of visual foundation models trained on large datasets possess open-world visual concepts, including Segment Anything (SA), DeAOT, and DINOv2, for one-shot image segmentation and unsupervised visual feature extraction. Furthermore, CASTLE employs unsupervised multi-stage and/or multi-layer UMAP clustering algorithms to distinguish behavioral clusters with unique temporal variability. 
 
-# Install
-```
-git clone https://github.com/RaisoLiu/castle-animal.git
-cd castle-animal
-python install .
-```
+[![PyPI version](https://badge.fury.io/py/castle-ai.svg)](https://badge.fury.io/py/castle-ai)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](???)
 
-# Example
+CASTLE integrates the strengths of visual foundation models trained on large datasets possess open-world visual concepts, including Segment Anything (SA), DeAOT, and DINOv2, for one-shot image segmentation and unsupervised visual feature extraction. Furthermore, CASTLE employs unsupervised multi-stage and/or multi-layer UMAP clustering algorithms to distinguish behavioral clusters with unique temporal variability. 
 
-## Image segmentation
-```python
-1+1
+# Install
 ```
-
-## Video objects segmentation
-```python
-from castle import generate_aot
-
-tracker = generate_aot(ckpt_path, MODEL, DEVICE)
-tracker.add_reference_frame(frame, mask, num_object)
-
-
-new_mask = 
+pip install castle-ai
 ```
 
-## Visual latent extractioin
-```python
-1+1
-```
+# Reference
 
-## UMAP & HDBSCAN analysis
-```python
-1+1
-```
+[Segment Anything](https://github.com/facebookresearch/segment-anything.git)
+[DeAOT](https://github.com/z-x-yang/Segment-and-Track-Anything.git)
+[DINOv2](https://github.com/facebookresearch/dinov2.git)
```

### Comparing `castle_ai-0.0.1/castle_ai.egg-info/SOURCES.txt` & `castle_ai-0.0.2/castle_ai.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -82,16 +82,18 @@
 castle/sam/segment_anything/modeling/sam.py
 castle/sam/segment_anything/modeling/transformer.py
 castle/sam/segment_anything/utils/__init__.py
 castle/sam/segment_anything/utils/amg.py
 castle/sam/segment_anything/utils/onnx.py
 castle/sam/segment_anything/utils/transforms.py
 castle/utils/__init__.py
+castle/utils/download.py
 castle/utils/image_segment.py
 castle/utils/plot.py
+castle/utils/video_align.py
 castle/utils/video_io.py
 castle/utils/video_object_segment.py
 castle/utils/visual_latent_extract.py
 castle_ai.egg-info/PKG-INFO
 castle_ai.egg-info/SOURCES.txt
 castle_ai.egg-info/dependency_links.txt
 castle_ai.egg-info/not-zip-safe
```

### Comparing `castle_ai-0.0.1/setup.py` & `castle_ai-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         with io.open("README.md", encoding="UTF-8") as readme_file:
             return readme_file.read()
 
 
 
 configuration = {
     "name": "castle-ai",
-    "version": "0.0.1",
+    "version": "0.0.2",
     "description": "Distinguish behavioral clusters Toolbox",
     "long_description": readme(),
     "long_description_content_type": "text/markdown",
     "classifiers": [
         "Development Status :: 1 - Planning",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
```

